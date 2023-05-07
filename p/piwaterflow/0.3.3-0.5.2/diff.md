# Comparing `tmp/piwaterflow-0.3.3.tar.gz` & `tmp/piwaterflow-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwaterflow-0.3.3.tar", last modified: Mon May 16 10:00:37 2022, max compression
+gzip compressed data, was "piwaterflow-0.5.2.tar", last modified: Sun May  7 08:13:46 2023, max compression
```

## Comparing `piwaterflow-0.3.3.tar` & `piwaterflow-0.5.2.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-05-16 10:00:37.613107 piwaterflow-0.3.3/
--rw-rw-rw-   0        0        0     1450 2022-05-16 10:00:37.613107 piwaterflow-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      813 2021-04-11 07:56:46.000000 piwaterflow-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2022-05-16 10:00:37.581861 piwaterflow-0.3.3/piwaterflow/
--rw-rw-rw-   0        0        0      124 2022-03-02 18:58:32.000000 piwaterflow-0.3.3/piwaterflow/__init__.py
--rw-rw-rw-   0        0        0      534 2021-04-21 16:27:40.000000 piwaterflow-0.3.3/piwaterflow/config-template.yml
--rw-rw-rw-   0        0        0      930 2021-12-03 09:31:55.000000 piwaterflow-0.3.3/piwaterflow/configwaterflow.py
--rw-rw-rw-   0        0        0    16503 2022-05-16 09:53:18.000000 piwaterflow-0.3.3/piwaterflow/waterflow.py
--rw-rw-rw-   0        0        0     5330 2022-03-07 18:03:28.000000 piwaterflow-0.3.3/piwaterflow/webservice.py
-drwxrwxrwx   0        0        0        0 2022-05-16 10:00:37.613107 piwaterflow-0.3.3/piwaterflow.egg-info/
--rw-rw-rw-   0        0        0     1450 2022-05-16 10:00:37.000000 piwaterflow-0.3.3/piwaterflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2022-05-16 10:00:37.000000 piwaterflow-0.3.3/piwaterflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-16 10:00:37.000000 piwaterflow-0.3.3/piwaterflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2022-05-16 10:00:37.000000 piwaterflow-0.3.3/piwaterflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-05-16 10:00:37.000000 piwaterflow-0.3.3/piwaterflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-16 10:00:37.613107 piwaterflow-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      999 2022-05-16 09:59:29.000000 piwaterflow-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:13:46.541840 piwaterflow-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-07 08:13:46.541840 piwaterflow-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:13:46.537840 piwaterflow-0.5.2/piwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/piwaterflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/piwaterflow/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/piwaterflow/config_waterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:13:46.537840 piwaterflow-0.5.2/piwaterflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/piwaterflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/piwaterflow/tests/test_000.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21519 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/piwaterflow/waterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:13:46.537840 piwaterflow-0.5.2/piwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-07 08:13:46.000000 piwaterflow-0.5.2/piwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-07 08:13:46.000000 piwaterflow-0.5.2/piwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 08:13:46.000000 piwaterflow-0.5.2/piwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-07 08:13:46.000000 piwaterflow-0.5.2/piwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 08:13:46.000000 piwaterflow-0.5.2/piwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 08:13:46.541840 piwaterflow-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:13:46.541840 piwaterflow-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/tests/test_000_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/tests/test_001_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/tests/test_002_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/tests/test_003_lock.py
```

### Comparing `piwaterflow-0.3.3/PKG-INFO` & `piwaterflow-0.5.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: piwaterflow
-Version: 0.3.3
-Summary: Raspberry Pi Waterflow resilient system
-Home-page: https://github.com/Phornee/piwaterflow
-Author: Ismael Raya
-Author-email: phornee@gmail.com
-License: UNKNOWN
-Description: # PiWaterflow
-        This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
-        It's intended to be executed periodically (i.e. cron every 5 minutes).
-        - Requirements:
-          - Raspberry Pi (any model)
-          - Relays to control the valves
-          - Optional control relay to enable alternative power inverter
-        - It supports 2 watering programs every day.
-          - Programs can be forced at any time.
-        - Valves can be manually triggered.
-        - Programs, forced programs and manual Valves can be manually stopped.
-        - Metrics can be emitted to influxdb, mongodb or mariaDB to register actions (programs and valves).
-        - This package fits with piwwwaterflow, so that it can be controlled via HTTP page.
-        
-        TODO:
-        - Abort watering if humidity is above threshold (90% default). Send email warning
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Home Automation
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: piwaterflow
+Version: 0.5.2
+Summary: Raspberry Pi Waterflow resilient system
+Home-page: https://github.com/Phornee/piwaterflow
+Author: Ismael Raya
+Author-email: phornee@gmail.com
+License: UNKNOWN
+Description: # PiWaterflow
+        This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
+        It's intended to be executed periodically (i.e. cron every 5 minutes).
+        - Requirements:
+          - Raspberry Pi (any model)
+          - Relays to control the valves
+          - Optional control relay to enable alternative power inverter
+        - It supports 2 watering programs every day.
+          - Programs can be forced at any time.
+        - Valves can be manually triggered.
+        - Programs, forced programs and manual Valves can be manually stopped.
+        - Metrics can be emitted to influxdb to register actions (programs and valves).
+        - This package fits with piwwwaterflow, so that it can be controlled via HTTP page.
+        
+        TODO:
+        - Abort watering if humidity is above threshold (90% default). Send email warning
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Home Automation
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `piwaterflow-0.3.3/piwaterflow/waterflow.py` & `piwaterflow-0.5.2/piwaterflow/waterflow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,258 +1,357 @@
-import RPi.GPIO as GPIO
+""" Loop for watering system. It will properly activate watering valves according to the schedulling set
+    in the config file
+    All times are local to the watering system location
+"""
 import os
 import time
-from datetime import datetime, timedelta, timezone
-import pytz
+import shutil
+from datetime import datetime, timedelta
 from pathlib import Path
-from baseutils_phornee import ManagedClass, Logger
-from piwaterflow import WaterflowConfig
-from influxdb import InfluxDBClient
-
 import json
 
-class Waterflow(ManagedClass):
+try:
+    from RPi import GPIO
+except (ModuleNotFoundError, ImportError, RuntimeError):
+    from fake_rpi.RPi import GPIO
+    from fake_rpi import toggle_print
+    toggle_print(False)
+
+from influxdb_wrapper import influxdb_factory
+from log_mgr import Logger
+from .config_waterflow import WaterflowConfig
+
+class Waterflow():
+    """ Waterflow class that manages a loop system to activate/deactivate watering valves.
+        This should run in a raspberry pi or similar, with watering valves connected through relays.
+        At this moment it can support up to 2 valves, and 2 different programs alnog the day.
+        Those programs/valves can be switched on/off in a forced way apart from the programs.
+        This is autonomous, and could be controlled by directly changing the programs´configuration in the
+        config.yml file.
+        However, it can work together with the piwwwwaterflow package that serves a http page to remotely control
+        the waterflow system.
+    """
+    def __init__(self, template_config_path: str = None, dry_run: bool = False):
+        """__init__ of the function
+        Args:
+            template_config_path (str, optional): Template config to use. Defaults to None.
+            dry_run (bool, optional): If true, it will just simulate, and wont make any change. Defaults to False.
+        """
+        self.homevar = os.path.join(str(Path.home()), 'var', self.class_name())
+
+        if dry_run:
+            self.dry_run = True
+            self.homevar = os.path.join(self.homevar, 'dryrun')
+            if os.path.exists(self.homevar): # Only one instance of waterflow can run at a time, so this is safe
+                shutil.rmtree(self.homevar)
+            if not os.path.exists(self.homevar):
+                os.makedirs(self.homevar)
+            dry_run_abs_path = ""
+        else:
+            self.dry_run = False
+            dry_run_abs_path = None
+
+        self.debuglogger = Logger(self.class_name(), 'waterflow', dry_run=dry_run)
+        self.userlogger = Logger(self.class_name(), 'loop', dry_run=dry_run)
 
-    def __init__(self):
-        super().__init__(execpath=__file__)
+        if not template_config_path:
+            template_config_path = os.path.join(Path(__file__).parent.resolve(), './config-template.yml')
 
-        self.logger = Logger({'modulename': self.getClassName(), 'logpath': 'log', 'logname': 'waterflow'})
-        self.looplogger = Logger({'modulename': self.getClassName(), 'logpath': 'log', 'logname': 'loop'})
-        self.config = WaterflowConfig({'modulename': self.getClassName(), 'execpath': __file__})
-
-        try:
-            host = self.config['influxdbconn']['host']
-            user = self.config['influxdbconn']['user']
-            password = self.config['influxdbconn']['password']
-            bucket = self.config['influxdbconn']['bucket']
-        except Exception as e:
-            self.logger.warning('Error getting connection credentials to InfluxDB.')
-            pass
-
-        try:
-            self.conn = InfluxDBClient(host=host, username=user, password=password, database=bucket)
-        except Exception as e:
-            self.logger.warning('Connection to InfluxDB failed: %s.' % host)
-            self.conn = None
-            pass
+        self.config = WaterflowConfig(package_name=self.class_name(),
+                                        template_path=template_config_path,
+                                        config_file_name="config.yml",
+                                        dry_run_abs_path=dry_run_abs_path)
+
+        influx_conn_type = self.config['influxdbconn'].get('type', 'influx')
+        self.conn = influxdb_factory(influx_conn_type)
+        self.conn.openConn(self.config['influxdbconn'])
+
+    def __del__(self):
+        if self.dry_run:
+            shutil.rmtree(self.homevar)
 
     @classmethod
-    def getClassName(cls):
+    def class_name(cls):
+        """ class name """
         return "waterflow"
 
-    def updateConfig(self, programs):
+    def _get_homevar_path(self, rel_path):
+        return os.path.join(self.homevar, rel_path)
+
+    def update_config(self, programs: dict):
+        """Updates the config file with modified programs
+        Args:
+            programs (dict): New programs to be modified
+        """
         # Update config in mem
         self.config.update({'programs': programs})
 
         # Write back config to disk
         self.config.write()
 
-    def _setTimezoneUTC(self, date):
-        import pytz
-
-        return pytz.timezone('UTC').localize(date)
+    def _get_program_data(self, program):
+        return next(iter(program.values()))
 
-    def _getNowUTC(self):
-        return datetime.now(timezone.utc)
+    @staticmethod
+    def time_to_str(time_var: datetime) -> str:
+        """ Transform a datetime into custom formatted string
+        Args:
+            time_var (datetime): Datetime
+        Returns:
+            str: Date written into a string
+        """
+        return time_var.strftime('%Y-%m-%d %H:%M:%S')
 
-    def _timeToStr(self, time_var):
-        return time_var.strftime('%Y-%m-%d %H:%M:%S\n')
+    @staticmethod
+    def str_to_time(date_str: str) -> datetime:
+        """ Extracts a datetime out of a string
+        Args:
+            date_str (str): String containing a date
+        Returns:
+            datetime: Time in local timezone
+        """
+        return datetime.strptime(date_str, '%Y-%m-%d %H:%M:%S').astimezone()
 
-    def _setupGPIO(self, valves):
+    def _setup_gpio(self, valves):
         GPIO.setmode(GPIO.BOARD)
         GPIO.setwarnings(False)
 
         GPIO.setup(self.config['inverter_relay_pin'], GPIO.OUT)
         GPIO.output(self.config['inverter_relay_pin'], GPIO.LOW)
         GPIO.setup(self.config['external_ac_signal_pin'], GPIO.IN)
         for valve in valves:
             GPIO.setup(valve['pin'], GPIO.OUT)
             GPIO.output(valve['pin'], GPIO.LOW)
-            pass
-
 
-    def _recalcNextProgram(self, last_program_time_utc):
+    def _recalc_next_program(self, last_program_time: datetime, today: datetime = None):
+        """ Calculates which is the next program to be executed, depending on the one previously executed
+        Args:
+            last_program_time: (datetime): Time in which previous program was executed (local aware to watering system)
+            today (datetime, optional): Naive time to make the calculations. Normally used just for debug/unittesting
+        Returns:
+            tuple: time of next program, and program name
         """
-        Calculates which is the next program to be executed
-        Return: UTC time of next program
-        """
-        next_program_time_utc = None
-        program_number = -1
+        next_program_time = None
+        program_name = None
+
+        # Only used to get "today"... hour and minute will be overwritten for comparations with last_program_time
+        if today:
+            current_time = today.astimezone() # Make aware
+        else:
+            current_time = datetime.now().astimezone().replace(microsecond=0)
 
-        current_time = datetime.now().replace(microsecond=0)
+        # Transform into a list to sort them
+        prog_list = []
+        for key, value in self.config['programs'].items():
+            temp = value
+            temp['name'] = key
+            prog_list.append(temp)
+        prog_list.sort(key=lambda prog: prog['start_time'])
 
         # Find if next program is today, considering the last program time executed
-        for idx, program in enumerate(self.config['programs']):
-            if program['enabled'] == True:
+        for program in prog_list:
+            if program['enabled'] is True:
                 candidate_time = current_time.replace(hour=program['start_time'].hour,
                                                       minute=program['start_time'].minute,
-                                                      second=0)
-                candidate_time_utc = candidate_time.astimezone(pytz.utc)
-                # If this candidate is after the last one executed AND its no more that 10 minutes in the past, choose it
-                if candidate_time_utc > last_program_time_utc:
-                    next_program_time_utc = candidate_time_utc
-                    program_number = idx
+                                                      second=0).astimezone()
+                # If this candidate is after the last one executed AND its not older than 10 minutes, choose it
+                if candidate_time > last_program_time:
+                    next_program_time = candidate_time
+                    program_name = program['name']
                     break
 
         # If its not today, it could be tomorrow... find the first one enabled
-        if next_program_time_utc is None:
-            for idx, program in enumerate(self.config['programs']):
-                if program['enabled'] == True:
+        if next_program_time is None:
+            for program in prog_list:
+                if program['enabled'] is True:
                     next_program_time = current_time + timedelta(days=1)
-                    next_program_time_utc = next_program_time.replace(hour=program['start_time'].hour,
-                                                                      minute=program['start_time'].minute,
-                                                                      second=0).astimezone(pytz.utc)
-                    program_number = idx
+                    next_program_time = next_program_time.replace(hour=program['start_time'].hour,
+                                                                  minute=program['start_time'].minute,
+                                                                  second=0).astimezone()
+                    program_name = program['name']
                     break
 
-        return next_program_time_utc, program_number
+        return next_program_time, program_name
 
-    def _getLastProgramPath(self):
-        return os.path.join(self.homevar, 'lastprogram.yml')
+    def _last_program_path(self):
+        return self._get_homevar_path('lastprogram.yml')
 
-    def _readLastProgramTime(self):
-        last_program_path = self._getLastProgramPath()
+    def _read_last_program_time(self):
+        last_program_path = self._last_program_path()
 
-        try:
-            with open(last_program_path, 'r') as file:
+        if os.path.exists(last_program_path):
+            with open(last_program_path, 'r', encoding="utf-8") as file:
                 data = file.readlines()
-                last_program_time = datetime.strptime(data[0][:-1], '%Y-%m-%d %H:%M:%S').replace(tzinfo=timezone.utc)
-
-        except Exception as e:
-            last_program_time = self._getNowUTC()
-            #last_program_time = datetime.now()
-            with open(last_program_path, 'w') as file:
-                time_str = self._timeToStr(last_program_time)
+                last_program_time = self.str_to_time(data[0][:-1])
+        else:
+            last_program_time = datetime.now().astimezone()
+            with open(last_program_path, 'w', encoding="utf-8") as file:
+                time_str = self.time_to_str(last_program_time)
                 file.writelines([time_str, time_str])
         return last_program_time
 
-    def _writeLastProgramTime(self, timelist):
-        last_program_path = self._getLastProgramPath()
-        with open(last_program_path, 'w') as file:
+    def _write_last_program_time(self, timelist):
+        last_program_path = self._last_program_path()
+        with open(last_program_path, 'w', encoding="utf-8") as file:
             file.writelines(timelist)
 
-    def getLock(self):
+    def get_lock(self):
         """
         This is to ensure that only one execution will run from cron at the same time
         Use file as a lock... not using DB locks because we want to maximize resiliency
         """
-        lock_path = os.path.join(self.homevar, 'lock')
+        lock_path = self._get_homevar_path('lock')
 
         if not os.path.exists(lock_path):
-            with open(lock_path, 'w'):
+            with open(lock_path, 'w', encoding="utf-8"):
                 return True
         else:
-            modified_time = datetime.fromtimestamp(os.path.getmtime(lock_path))
-            if (datetime.utcnow() - modified_time) > timedelta(minutes=20):
-                self.logger.warning('Lock expired: Last loop ended abnormally?.')
-                Path(lock_path).touch() # Previous token expired (previous loop crashed?)... so we will retouch to try again
+            modified_time = datetime.fromtimestamp(os.path.getmtime(lock_path)).astimezone()
+            if (datetime.now().astimezone() - modified_time) > timedelta(minutes=self.config['max_loop_time']):
+                self.userlogger.warning('Lock expired: Last loop ended abnormally?.')
+                Path(lock_path).touch()  # Previous token expired (previous loop crashed?)... we will retouch to retry
                 return True
         return False
 
-    def releaseLock(self):
-        lock_path = os.path.join(self.homevar, 'lock')
+    def release_lock(self):
+        """Lock the loop... so the 2 loops cannot happen at the same time
+        """
+        lock_path = self._get_homevar_path('lock')
 
         if os.path.exists(lock_path):
             os.remove(lock_path)
         else:
-            self.logger.error(f"Could not release lock.")
+            self.userlogger.error("Could not release lock.")
 
-    def isLoopingCorrectly(self):
-        return (datetime.utcnow() - self.getLastLoopTime()) < timedelta(minutes=10)
+    def is_looping_correctly(self):
+        """ Returns if a loop has succesfully run in the last x minutes
+        Returns:
+           bool: 
+        """
+        time_now = datetime.now().astimezone()
+        return (time_now - self.last_loop_time()) < timedelta(minutes=self.config['max_loop_time'])
 
-    def getLastLoopTime(self):
-        tokenpath = os.path.join(self.getHomevarPath(), 'token')
+    def last_loop_time(self):
+        """ Returns the last time in that a loop was succesfully executed
+        Returns:
+           datetime: Time in which last loop was executed
+        """
+        token_path = self._get_homevar_path('token')
+        if os.path.exists(token_path):
+            mod_time_since_epoc = os.path.getmtime(token_path)
+            modification_time = datetime.fromtimestamp(mod_time_since_epoc).astimezone()
+        else:
+            modification_time = datetime.fromtimestamp(0) # Loop never run ok. Return oldest possible date
 
-        modTimesinceEpoc = os.path.getmtime(tokenpath)
-        modificationTime = datetime.utcfromtimestamp(modTimesinceEpoc)
+        return modification_time
 
-        return modificationTime
+    def force(self, type_force: str, value: int):
+        """ Set the force-flag, so that the loop will start the execution of a program or valve
+            If a program is forced, it will execute with the times defined in the config
+            If a valve is forced, it will start delivering water, until manually stopped
+        Args:
+            type_force (str): Can be "program" or "valve"
+            value (int): Index of the item to be forced
 
-    def force(self, type_force, value):
-        config = self.config.getDict()
+        Returns:
+            bool: If forced correctly
+        """
+        config = self.config.get_dict()
         if (type_force == 'program' and 0 <= value < len(config['programs'])) or \
            (type_force == 'valve' and 0 <= value < len(config['valves'])):
-            force_file_path = os.path.join(self.getHomevarPath(), 'force')
-            with open(force_file_path, 'w') as force_file:
-                force_file.write('{{"type":"{0}","value":{1}}}'.format(type_force, value))
+            with open(self._get_homevar_path('force'), 'w', encoding="utf-8") as force_file:
+                force_file.write(f'{{"type":"{type_force}","value":{value}}}')
                 return True
         else:
             return False
 
     def stop(self):
-        stop_req_path = os.path.join(self.getHomevarPath(), 'stop')
+        """ Set the Stop-flag, so that the loop will stop the forced valve or program execution
+        Returns:
+            _type_: _description_
+        """
+        stop_req_path = self._get_homevar_path('stop')
         Path(stop_req_path).touch()
         return True
 
-    def stopRequested(self):
-        stop_req_path = os.path.join(self.getHomevarPath(), 'stop')
-        return os.path.exists(stop_req_path)
-
-    def stopRemove(self):
-        stop_req_path = os.path.join(self.getHomevarPath(), 'stop')
+    def stop_remove(self):
+        """ Returns if a stop has already been requested
+        Returns:
+           bool: Return true if a stop has been requested
+        """
+        stop_req_path = self._get_homevar_path('stop')
         return os.remove(stop_req_path)
 
-    def getForcedInfo(self):
-        force_file_path = os.path.join(self.getHomevarPath(), 'force')
+    def stop_requested(self):
+        """ Returns if a stop has already been requested
+        Returns:
+           bool: Return true if a stop has been requested
+        """
+        stop_req_path = self._get_homevar_path('stop')
+        return os.path.exists(stop_req_path)
+
+    def get_forced_info(self):
+        """ Returns the forced info of the waterflow
+        Returns:
+            dict: Forced info
+        """
+        force_file_path = self._get_homevar_path('force')
         if os.path.exists(force_file_path):
-            with open(force_file_path, 'r') as force_file:
+            with open(force_file_path, 'r', encoding="utf-8") as force_file:
                 data = json.load(force_file)
                 return data
         else:
             return None
 
-    def getLog(self):
-        return self.logger.getLog()
+    def get_log(self):
+        """ Get the user log (not the debug log). This is the one the is shown in the wwwaterflow
+        Returns:
+            str: The whole user logs
+        """
+        return self.userlogger.get_log()
 
     def _sleep(self, time_sleep):
-        """
-        Sleep "time_sleep" time, but checks every 5 seconds if a stop has been requested
+        """ Sleep "time_sleep" time, but checks every 5 seconds if a stop has been requested
+        Args:
+            time_sleep (int): Number of seconds to sleep
         """
         time_count = 0
-        while not self.stopRequested() and time_count < time_sleep:
+        while not self.stop_requested() and time_count < time_sleep:
             time_count = time_count + 5
             time.sleep(5)  # Every X seconds
 
-    def _emitActionMetric(self, action, forced):
-        if self.config['metrics']:
-            if self.conn:
-                json_body = [
-                    {
-                        "measurement": "piwaterflow",
-                        "tags": {
-                            "action": action,
-                            "forced": forced
-                        },
-                        "time": datetime.utcnow(),
-                        "fields": {
-                            "fake": 0
-                        }
-                    }
-                ]
-                self.conn.write_points(json_body)
+    def _emit_action_metric(self, action, forced):
+        if self.config['metrics'] and self.conn:
+            action_body = [
+                {
+                    "tags": {"action": action, "forced": forced},
+                    "fields": {"fake": 0}
+                }
+            ]
+            self.conn.insert("piwaterflow", action_body)
 
-    def _executeValve(self, valve):
+    def _execute_valve(self, valve):
         # ------------------------------------
         # inverter_enable =  not GPIO.input(self.config['external_ac_signal_pin'])
         # if inverter_enable: # If we dont have external 220V power input, then activate inverter
         GPIO.output(self.config['inverter_relay_pin'], GPIO.HIGH)
-        self.logger.info('Inverter relay ON.')
+        self.userlogger.info('Inverter relay ON.')
         valve_pin = self.config['valves'][valve]['pin']
         GPIO.output(valve_pin, GPIO.HIGH)
-        self.logger.info('Valve %s ON.' % valve)
+        self.userlogger.info(f'Valve {valve} ON.')
 
         self._sleep(self.config['max_valve_time']*60)
 
         GPIO.output(valve_pin, GPIO.LOW)
-        self.logger.info('Valve %s OFF.' % valve)
+        self.userlogger.info(f'Valve {valve} OFF.')
         # if inverter_enable: # If we dont have external 220V power input, then activate inverter
         GPIO.output(self.config['inverter_relay_pin'], GPIO.LOW)  # INVERTER always OFF after operations
-        self.logger.info('Inverter relay OFF.')
+        self.userlogger.info('Inverter relay OFF.')
 
-    def _skipProgram(self):
+    def _skip_program(self):
         # print(self.config['humidity_threshold'])
         # if self.is_raspberry_pi():
         #     import adafruit_dht
         #     dhtSensor = adafruit_dht.DHT22(self.config['pin'])
         #     humidity = dhtSensor.humidity
         #     temp_c = dhtSensor.temperature
         #     if humidity >= self.config['humidity_threshold']:
@@ -260,123 +359,131 @@
         #         return True
         #     else:
         #         return False
         # else:
         #    return False
         return False
 
-    def _executeProgram(self, program_number):
+    def _execute_program(self, program_name: str):
         """
         Works for regular programs, or forced ones (if program number is sent)
         """
-        self.logger.info('Executing program %s.' % program_number)
+        self.userlogger.info(f'Executing program {program_name}.')
         # inverter_enable =  not GPIO.input(self.config['external_ac_signal_pin'])
         # if inverter_enable: # If we don't have external 220V power input, then activate inverter
         GPIO.output(self.config['inverter_relay_pin'], GPIO.HIGH)
-        self.logger.info('Inverter relay ON.')
-        for idx, valve_time in enumerate(self.config['programs'][program_number]['valves_times']):
-            if valve_time > 0 and not self.stopRequested():
+        self.userlogger.info('Inverter relay ON.')
+        program_data = self._get_program_data(self.config['programs'][program_name])
+        for idx, valve_time in enumerate(program_data['valves_times']):
+            if valve_time > 0 and not self.stop_requested():
                 valve_pin = self.config['valves'][idx]['pin']
                 GPIO.output(valve_pin, GPIO.HIGH)
-                self.logger.info('Valve %s ON.' % idx)
+                self.userlogger.info(f'Valve {idx} ON.')
 
                 self._sleep(valve_time * 60)
 
                 GPIO.output(valve_pin, GPIO.LOW)
-                self.logger.info('Valve %s OFF.' % idx)
+                self.userlogger.info(f'Valve {idx} OFF.')
             else:
-                self.logger.info('Valve %s Skipped.' % idx)
+                self.userlogger.info(f'Valve {idx} Skipped.')
         # if inverter_enable: # If we dont have external 220V power input, then activate inverter
         GPIO.output(self.config['inverter_relay_pin'], GPIO.LOW)  # INVERTER always OFF after operations
-        self.logger.info('Inverter relay OFF.')
+        self.userlogger.info('Inverter relay OFF.')
 
-    def _logNextProgramTime(self, current_time_utc):
+    def _log_next_program_time(self, current_time):
 
-        log = self.logger.getLog()
+        log = self.userlogger.get_log()
 
         lines = log.split('\n')
 
-        new_next_program_time_utc, _ = self._recalcNextProgram(current_time_utc)
+        new_next_program_time, _ = self._recalc_next_program(current_time)
 
-        if new_next_program_time_utc:
-            from tzlocal import get_localzone
-            new_next_program_time_local = new_next_program_time_utc.astimezone(get_localzone())
-
-            string_to_log = 'Next program: %s.' % new_next_program_time_local.strftime('%Y-%m-%d %H:%M')
+        if new_next_program_time:
+            string_to_log = f"Next program: {self.time_to_str(new_next_program_time)}."
         else:
             string_to_log = 'NO active program!'
 
-        # If previous log empty, or if last line outputs different information... log it. This is to avoid duplicated logs
+        # If previous log empty, or if last line outputs different information... log it. (to avoid duplicated logs)
         if len(lines) <= 1 or (lines[-2][20:] != string_to_log and string_to_log != ''):
-            self.logger.info(string_to_log)
+            self.userlogger.info(string_to_log)
 
-    def loop(self):
-        if self.getLock():  # To ensure a single execution despite of cron overlapping
+    def _execute_forced(self, forced_info: dict, curr_time: datetime):
+        forced_type = forced_info.get("type")
+        forced_value = forced_info.get("value")
+        if forced_type == "program":
+            self.userlogger.info(f'Forced program {forced_value} executing now.')
+            # ------------------------
+            self._emit_action_metric(f'prog{forced_value}', True)
+            self._execute_program(forced_value)
+            self._write_last_program_time(self.time_to_str(curr_time))
+        elif forced_type == "valve":
+            # ------------------------
+            self._emit_action_metric('valve{forced_value}', True)
+            self._execute_valve(forced_value)
+
+    def _check_and_execute_program(self, curr_time: datetime):
+        last_program_time = self._read_last_program_time()
+        new_next_program, new_program_name = self._recalc_next_program(last_program_time)
+        if new_next_program:
+            # ------------------------
+            time_reached = curr_time >= new_next_program
+            time_threshold_exceeded = curr_time > (new_next_program + timedelta(minutes=self.config['max_loop_time']))
+            skip_program = self._skip_program()
+            # If we have reached the time of the new_program_time, BUT not by more than 10 minutes...
+            if time_reached and not time_threshold_exceeded and not skip_program:
+                self._emit_action_metric(f'prog_{new_program_name}', False)
+                self._execute_program(new_program_name)
+                program_executed = True
+            else:
+                program_executed = False
+
+            if program_executed or skip_program or time_threshold_exceeded:
+                self._write_last_program_time(self.time_to_str(curr_time))
+
+    def loop(self, date_now: datetime = None):
+        """ Loop executed every x minutes... in crontab for example.
+        Args:
+            date_now (datetime): Naive date to consider the execution of the loop. 
+                                 Normally used only for debuggin/unittesting
+        """
+        if self.get_lock():  # To ensure a single execution despite of cron overlapping
             try:
-                current_time_utc = self._getNowUTC()
-                forced_info = self.getForcedInfo()
+                if date_now:
+                    curr_time = date_now.astimezone() # Make aware
+                else:
+                    curr_time = datetime.now().astimezone()
+                forced_info = self.get_forced_info()
 
-                if not self.stopRequested():
-                    self.looplogger.info('Looping...')
-                    self._setupGPIO(self.config['valves'])
-                    last_program_time = self._readLastProgramTime()
+                if not self.stop_requested():
+                    self.debuglogger.info('Looping...')
+                    self._setup_gpio(self.config['valves'])
 
                     if forced_info:
-                        forced_type = forced_info.get("type")
-                        forced_value = forced_info.get("value")
-                        if forced_type == "program":
-                            self.logger.info('Forced program {} executing now.'.format(forced_value))
-                            # ------------------------
-                            self._emitActionMetric('prog{}'.format(forced_value), True)
-                            self._executeProgram(forced_value)
-                            self._writeLastProgramTime(self._timeToStr(current_time_utc))
-                        elif forced_type == "valve":
-                            # ------------------------
-                            self._emitActionMetric('valve{}'.format(forced_value), True)
-                            self._executeValve(forced_value)
+                        self._execute_forced(forced_info, curr_time)
                     else:
-                        new_next_program_time_utc, calculated_program_number = self._recalcNextProgram(last_program_time)
-                        if new_next_program_time_utc:
-                            # ------------------------
-                            time_reached = current_time_utc >= new_next_program_time_utc
-                            time_threshold_exceeded = current_time_utc > (new_next_program_time_utc + timedelta(minutes=10))
-                            skip_program = self._skipProgram()
-                            # If we have reached the time of the new_program_time, BUT not by more than 10 minutes...
-                            if time_reached and not time_threshold_exceeded and not skip_program:
-                                self._emitActionMetric('prog{}'.format(calculated_program_number), False)
-                                self._executeProgram(calculated_program_number)
-                                program_executed = True
-                            else:
-                                program_executed = False
-
-                            if program_executed or skip_program or time_threshold_exceeded:
-                                self._writeLastProgramTime(self._timeToStr(current_time_utc))
+                        self._check_and_execute_program(curr_time)
                 else:
-                    self.looplogger.info('Loop skipped (Stop request).')
-                    self.logger.info('Activity stopped.')
-                    self._emitActionMetric('Stop', True)
-                    self.stopRemove()
+                    self.debuglogger.info('Loop skipped (Stop request).')
+                    self.userlogger.info('Activity stopped.')
+                    self._emit_action_metric('Stop', True)
+                    self.stop_remove()
 
                 if forced_info:
                     # Remove force token file
-                    os.remove(os.path.join(self.getHomevarPath(), 'force'))
+                    os.remove(os.path.join(self.homevar, 'force'))
 
                 # Recalc next program time
-                self._logNextProgramTime(current_time_utc)
+                self._log_next_program_time(curr_time)
 
                 # Updates "modified" time AT THE END, so that we can keep track about waterflow looping SUCCESFULLY.
                 token_path = os.path.join(self.homevar, 'token')
                 Path(token_path).touch()
 
-            except Exception as e:
-                self.logger.error("Exception looping: {}".format(str(e)))
-                raise
+            except Exception as ex:
+                self.debuglogger.error(f'Exception looping: {str(ex)}')
+                self.userlogger.error(f'Exception looping: {str(ex)}')
+                raise RuntimeError(ex) from ex
             finally:
                 GPIO.cleanup()
-                self.releaseLock()
-
-if __name__ == "__main__":
-
-    waterflow_instance = Waterflow()
-    waterflow_instance.loop()
-
-
+                self.release_lock()
+        else:
+            self.debuglogger.error('Loop executed while locked by previous execution.')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `piwaterflow-0.3.3/piwaterflow.egg-info/PKG-INFO` & `piwaterflow-0.5.2/piwaterflow.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: piwaterflow
-Version: 0.3.3
-Summary: Raspberry Pi Waterflow resilient system
-Home-page: https://github.com/Phornee/piwaterflow
-Author: Ismael Raya
-Author-email: phornee@gmail.com
-License: UNKNOWN
-Description: # PiWaterflow
-        This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
-        It's intended to be executed periodically (i.e. cron every 5 minutes).
-        - Requirements:
-          - Raspberry Pi (any model)
-          - Relays to control the valves
-          - Optional control relay to enable alternative power inverter
-        - It supports 2 watering programs every day.
-          - Programs can be forced at any time.
-        - Valves can be manually triggered.
-        - Programs, forced programs and manual Valves can be manually stopped.
-        - Metrics can be emitted to influxdb, mongodb or mariaDB to register actions (programs and valves).
-        - This package fits with piwwwaterflow, so that it can be controlled via HTTP page.
-        
-        TODO:
-        - Abort watering if humidity is above threshold (90% default). Send email warning
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Home Automation
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: piwaterflow
+Version: 0.5.2
+Summary: Raspberry Pi Waterflow resilient system
+Home-page: https://github.com/Phornee/piwaterflow
+Author: Ismael Raya
+Author-email: phornee@gmail.com
+License: UNKNOWN
+Description: # PiWaterflow
+        This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
+        It's intended to be executed periodically (i.e. cron every 5 minutes).
+        - Requirements:
+          - Raspberry Pi (any model)
+          - Relays to control the valves
+          - Optional control relay to enable alternative power inverter
+        - It supports 2 watering programs every day.
+          - Programs can be forced at any time.
+        - Valves can be manually triggered.
+        - Programs, forced programs and manual Valves can be manually stopped.
+        - Metrics can be emitted to influxdb to register actions (programs and valves).
+        - This package fits with piwwwaterflow, so that it can be controlled via HTTP page.
+        
+        TODO:
+        - Abort watering if humidity is above threshold (90% default). Send email warning
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Home Automation
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

