# Comparing `tmp/mysql-replication-0.8.tar.gz` & `tmp/mysql-replication-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mysql-replication-0.8.tar", last modified: Sat Jan  2 21:17:44 2016, max compression
+gzip compressed data, was "dist/mysql-replication-0.9.tar", last modified: Fri May 20 08:34:46 2016, max compression
```

## Comparing `mysql-replication-0.8.tar` & `mysql-replication-0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 noplay     (501) staff       (20)        0 2016-01-02 21:17:44.000000 mysql-replication-0.8/
-drwxr-xr-x   0 noplay     (501) staff       (20)        0 2016-01-02 21:17:44.000000 mysql-replication-0.8/mysql_replication.egg-info/
--rw-r--r--   0 noplay     (501) staff       (20)        1 2016-01-02 21:17:43.000000 mysql-replication-0.8/mysql_replication.egg-info/dependency_links.txt
--rw-r--r--   0 noplay     (501) staff       (20)       47 2016-01-02 21:17:43.000000 mysql-replication-0.8/mysql_replication.egg-info/pbr.json
--rw-r--r--   0 noplay     (501) staff       (20)      334 2016-01-02 21:17:43.000000 mysql-replication-0.8/mysql_replication.egg-info/PKG-INFO
--rw-r--r--   0 noplay     (501) staff       (20)        8 2016-01-02 21:17:43.000000 mysql-replication-0.8/mysql_replication.egg-info/requires.txt
--rw-r--r--   0 noplay     (501) staff       (20)      875 2016-01-02 21:17:44.000000 mysql-replication-0.8/mysql_replication.egg-info/SOURCES.txt
--rw-r--r--   0 noplay     (501) staff       (20)       19 2016-01-02 21:17:43.000000 mysql-replication-0.8/mysql_replication.egg-info/top_level.txt
--rw-r--r--   0 noplay     (501) staff       (20)      334 2016-01-02 21:17:44.000000 mysql-replication-0.8/PKG-INFO
-drwxr-xr-x   0 noplay     (501) staff       (20)        0 2016-01-02 21:17:44.000000 mysql-replication-0.8/pymysqlreplication/
--rw-r--r--   0 noplay     (501) staff       (20)      734 2013-07-07 15:10:06.000000 mysql-replication-0.8/pymysqlreplication/__init__.py
--rw-r--r--   0 noplay     (501) staff       (20)    14556 2016-01-02 21:14:50.000000 mysql-replication-0.8/pymysqlreplication/binlogstream.py
--rw-r--r--   0 noplay     (501) staff       (20)     1315 2015-05-10 19:50:48.000000 mysql-replication-0.8/pymysqlreplication/bitmap.py
--rw-r--r--   0 noplay     (501) staff       (20)     3452 2015-08-25 07:39:25.000000 mysql-replication-0.8/pymysqlreplication/column.py
-drwxr-xr-x   0 noplay     (501) staff       (20)        0 2016-01-02 21:17:44.000000 mysql-replication-0.8/pymysqlreplication/constants/
--rw-r--r--   0 noplay     (501) staff       (20)       73 2013-07-07 15:10:06.000000 mysql-replication-0.8/pymysqlreplication/constants/__init__.py
--rw-r--r--   0 noplay     (501) staff       (20)      928 2015-05-10 19:50:48.000000 mysql-replication-0.8/pymysqlreplication/constants/BINLOG.py
--rw-r--r--   0 noplay     (501) staff       (20)     1540 2013-07-07 15:10:06.000000 mysql-replication-0.8/pymysqlreplication/constants/FIELD_TYPE.py
--rw-r--r--   0 noplay     (501) staff       (20)     7669 2015-06-19 08:06:38.000000 mysql-replication-0.8/pymysqlreplication/event.py
--rw-r--r--   0 noplay     (501) staff       (20)     3085 2015-08-25 07:39:25.000000 mysql-replication-0.8/pymysqlreplication/gtid.py
--rw-r--r--   0 noplay     (501) staff       (20)     9627 2015-06-19 08:06:38.000000 mysql-replication-0.8/pymysqlreplication/packet.py
--rw-r--r--   0 noplay     (501) staff       (20)    22205 2016-01-02 21:14:50.000000 mysql-replication-0.8/pymysqlreplication/row_event.py
--rw-r--r--   0 noplay     (501) staff       (20)     1048 2015-08-25 07:39:25.000000 mysql-replication-0.8/pymysqlreplication/table.py
-drwxr-xr-x   0 noplay     (501) staff       (20)        0 2016-01-02 21:17:44.000000 mysql-replication-0.8/pymysqlreplication/tests/
--rw-r--r--   0 noplay     (501) staff       (20)      339 2015-08-25 07:39:25.000000 mysql-replication-0.8/pymysqlreplication/tests/__init__.py
--rw-r--r--   0 noplay     (501) staff       (20)     2398 2015-08-25 07:39:25.000000 mysql-replication-0.8/pymysqlreplication/tests/base.py
--rw-r--r--   0 noplay     (501) staff       (20)     1761 2015-05-10 19:50:48.000000 mysql-replication-0.8/pymysqlreplication/tests/benchmark.py
--rw-r--r--   0 noplay     (501) staff       (20)    29061 2015-08-25 07:39:25.000000 mysql-replication-0.8/pymysqlreplication/tests/test_basic.py
--rw-r--r--   0 noplay     (501) staff       (20)     2618 2015-08-25 07:39:25.000000 mysql-replication-0.8/pymysqlreplication/tests/test_data_objects.py
--rw-r--r--   0 noplay     (501) staff       (20)    22804 2015-08-25 07:39:25.000000 mysql-replication-0.8/pymysqlreplication/tests/test_data_type.py
--rw-r--r--   0 noplay     (501) staff       (20)       59 2016-01-02 21:17:44.000000 mysql-replication-0.8/setup.cfg
--rw-r--r--   0 noplay     (501) staff       (20)     1264 2016-01-02 21:16:44.000000 mysql-replication-0.8/setup.py
+drwxr-xr-x   0 noplay     (501) staff       (20)        0 2016-05-20 08:34:46.000000 mysql-replication-0.9/
+drwxr-xr-x   0 noplay     (501) staff       (20)        0 2016-05-20 08:34:46.000000 mysql-replication-0.9/mysql_replication.egg-info/
+-rw-r--r--   0 noplay     (501) staff       (20)        1 2016-05-20 08:34:45.000000 mysql-replication-0.9/mysql_replication.egg-info/dependency_links.txt
+-rw-r--r--   0 noplay     (501) staff       (20)       47 2016-05-20 08:34:45.000000 mysql-replication-0.9/mysql_replication.egg-info/pbr.json
+-rw-r--r--   0 noplay     (501) staff       (20)      334 2016-05-20 08:34:45.000000 mysql-replication-0.9/mysql_replication.egg-info/PKG-INFO
+-rw-r--r--   0 noplay     (501) staff       (20)        8 2016-05-20 08:34:45.000000 mysql-replication-0.9/mysql_replication.egg-info/requires.txt
+-rw-r--r--   0 noplay     (501) staff       (20)      875 2016-05-20 08:34:46.000000 mysql-replication-0.9/mysql_replication.egg-info/SOURCES.txt
+-rw-r--r--   0 noplay     (501) staff       (20)       19 2016-05-20 08:34:45.000000 mysql-replication-0.9/mysql_replication.egg-info/top_level.txt
+-rw-r--r--   0 noplay     (501) staff       (20)      334 2016-05-20 08:34:46.000000 mysql-replication-0.9/PKG-INFO
+drwxr-xr-x   0 noplay     (501) staff       (20)        0 2016-05-20 08:34:46.000000 mysql-replication-0.9/pymysqlreplication/
+-rw-r--r--   0 noplay     (501) staff       (20)      734 2013-07-07 15:10:06.000000 mysql-replication-0.9/pymysqlreplication/__init__.py
+-rw-r--r--   0 noplay     (501) staff       (20)    19034 2016-05-20 08:29:08.000000 mysql-replication-0.9/pymysqlreplication/binlogstream.py
+-rw-r--r--   0 noplay     (501) staff       (20)     1315 2015-05-10 19:50:48.000000 mysql-replication-0.9/pymysqlreplication/bitmap.py
+-rw-r--r--   0 noplay     (501) staff       (20)     3452 2015-08-25 07:39:25.000000 mysql-replication-0.9/pymysqlreplication/column.py
+drwxr-xr-x   0 noplay     (501) staff       (20)        0 2016-05-20 08:34:46.000000 mysql-replication-0.9/pymysqlreplication/constants/
+-rw-r--r--   0 noplay     (501) staff       (20)       73 2013-07-07 15:10:06.000000 mysql-replication-0.9/pymysqlreplication/constants/__init__.py
+-rw-r--r--   0 noplay     (501) staff       (20)     1041 2016-05-20 08:29:08.000000 mysql-replication-0.9/pymysqlreplication/constants/BINLOG.py
+-rw-r--r--   0 noplay     (501) staff       (20)     1540 2013-07-07 15:10:06.000000 mysql-replication-0.9/pymysqlreplication/constants/FIELD_TYPE.py
+-rw-r--r--   0 noplay     (501) staff       (20)     8251 2016-05-20 08:29:08.000000 mysql-replication-0.9/pymysqlreplication/event.py
+-rw-r--r--   0 noplay     (501) staff       (20)     3098 2016-05-20 08:29:08.000000 mysql-replication-0.9/pymysqlreplication/gtid.py
+-rw-r--r--   0 noplay     (501) staff       (20)     9619 2016-05-20 08:29:08.000000 mysql-replication-0.9/pymysqlreplication/packet.py
+-rw-r--r--   0 noplay     (501) staff       (20)    22205 2016-01-02 21:14:50.000000 mysql-replication-0.9/pymysqlreplication/row_event.py
+-rw-r--r--   0 noplay     (501) staff       (20)     1048 2015-08-25 07:39:25.000000 mysql-replication-0.9/pymysqlreplication/table.py
+drwxr-xr-x   0 noplay     (501) staff       (20)        0 2016-05-20 08:34:46.000000 mysql-replication-0.9/pymysqlreplication/tests/
+-rw-r--r--   0 noplay     (501) staff       (20)      339 2015-08-25 07:39:25.000000 mysql-replication-0.9/pymysqlreplication/tests/__init__.py
+-rw-r--r--   0 noplay     (501) staff       (20)     3724 2016-05-20 08:29:08.000000 mysql-replication-0.9/pymysqlreplication/tests/base.py
+-rw-r--r--   0 noplay     (501) staff       (20)     1761 2015-05-10 19:50:48.000000 mysql-replication-0.9/pymysqlreplication/tests/benchmark.py
+-rw-r--r--   0 noplay     (501) staff       (20)    29548 2016-05-20 08:29:08.000000 mysql-replication-0.9/pymysqlreplication/tests/test_basic.py
+-rw-r--r--   0 noplay     (501) staff       (20)     2618 2015-08-25 07:39:25.000000 mysql-replication-0.9/pymysqlreplication/tests/test_data_objects.py
+-rw-r--r--   0 noplay     (501) staff       (20)    23116 2016-05-20 08:29:08.000000 mysql-replication-0.9/pymysqlreplication/tests/test_data_type.py
+-rw-r--r--   0 noplay     (501) staff       (20)       59 2016-05-20 08:34:46.000000 mysql-replication-0.9/setup.cfg
+-rw-r--r--   0 noplay     (501) staff       (20)     1264 2016-05-20 08:29:47.000000 mysql-replication-0.9/setup.py
```

### Comparing `mysql-replication-0.8/mysql_replication.egg-info/SOURCES.txt` & `mysql-replication-0.9/mysql_replication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mysql-replication-0.8/pymysqlreplication/__init__.py` & `mysql-replication-0.9/pymysqlreplication/__init__.py`

 * *Files identical despite different names*

### Comparing `mysql-replication-0.8/pymysqlreplication/binlogstream.py` & `mysql-replication-0.9/pymysqlreplication/binlogstream.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import pymysql
 import struct
 
-from pymysql.constants.COMMAND import COM_BINLOG_DUMP
+from pymysql.constants.COMMAND import COM_BINLOG_DUMP, COM_REGISTER_SLAVE
 from pymysql.cursors import DictCursor
 from pymysql.util import int2byte
 
 from .packet import BinLogPacketWrapper
 from .constants.BINLOG import TABLE_MAP_EVENT, ROTATE_EVENT
 from .gtid import GtidSet
 from .event import (
@@ -26,39 +26,134 @@
     COM_BINLOG_DUMP_GTID = 0x1e
 
 # 2013 Connection Lost
 # 2006 MySQL server has gone away
 MYSQL_EXPECTED_ERROR_CODES = [2013, 2006]
 
 
+class ReportSlave(object):
+
+    """Represent the values that you may report when connecting as a slave
+    to a master. SHOW SLAVE HOSTS related"""
+
+    hostname = ''
+    username = ''
+    password = ''
+    port = 0
+
+    def __init__(self, value):
+        """
+        Attributes:
+            value: string or tuple
+                   if string, then it will be used hostname
+                   if tuple it will be used as (hostname, user, password, port)
+        """
+
+        if isinstance(value, (tuple, list)):
+            try:
+                self.hostname = value[0]
+                self.username = value[1]
+                self.password = value[2]
+                self.port = int(value[3])
+            except IndexError:
+                pass
+        elif isinstance(value, dict):
+            for key in ['hostname', 'username', 'password', 'port']:
+                try:
+                    setattr(self, key, value[key])
+                except KeyError:
+                    pass
+        else:
+            self.hostname = value
+
+    def __repr__(self):
+        return '<ReportSlave hostname=%s username=%s password=%s port=%d>' %\
+            (self.hostname, self.username, self.password, self.port)
+
+    def encoded(self, server_id, master_id=0):
+        """
+        server_id: the slave server-id
+        master_id: usually 0. Appears as "master id" in SHOW SLAVE HOSTS
+                   on the master. Unknown what else it impacts.
+        """
+
+        # 1              [15] COM_REGISTER_SLAVE
+        # 4              server-id
+        # 1              slaves hostname length
+        # string[$len]   slaves hostname
+        # 1              slaves user len
+        # string[$len]   slaves user
+        # 1              slaves password len
+        # string[$len]   slaves password
+        # 2              slaves mysql-port
+        # 4              replication rank
+        # 4              master-id
+
+        lhostname = len(self.hostname)
+        lusername = len(self.username)
+        lpassword = len(self.password)
+
+        packet_len = (1 +  # command
+                      4 +  # server-id
+                      1 +  # hostname length
+                      lhostname +
+                      1 +  # username length
+                      lusername +
+                      1 +  # password length
+                      lpassword +
+                      2 +  # slave mysql port
+                      4 +  # replication rank
+                      4)  # master-id
+
+        MAX_STRING_LEN = 257  # one byte for length + 256 chars
+
+        return (struct.pack('<i', packet_len) +
+                int2byte(COM_REGISTER_SLAVE) +
+                struct.pack('<L', server_id) +
+                struct.pack('<%dp' % min(MAX_STRING_LEN, lhostname + 1),
+                            self.hostname) +
+                struct.pack('<%dp' % min(MAX_STRING_LEN, lusername + 1),
+                            self.username) +
+                struct.pack('<%dp' % min(MAX_STRING_LEN, lpassword + 1),
+                            self.password) +
+                struct.pack('<H', self.port) +
+                struct.pack('<l', 0) +
+                struct.pack('<l', master_id))
+
 
 class BinLogStreamReader(object):
+
     """Connect to replication stream and read event
     """
+    report_slave = None
 
     def __init__(self, connection_settings, server_id, resume_stream=False,
                  blocking=False, only_events=None, log_file=None, log_pos=None,
                  filter_non_implemented_events=True,
                  ignored_events=None, auto_position=None,
                  only_tables=None, only_schemas=None,
-                 freeze_schema=False, skip_to_timestamp=None):
+                 freeze_schema=False, skip_to_timestamp=None,
+                 report_slave=None, slave_uuid=None,
+                 pymysql_wrapper=None):
         """
         Attributes:
             resume_stream: Start for event from position or the latest event of
                            binlog or from older available event
             blocking: Read on stream is blocking
             only_events: Array of allowed events
             ignored_events: Array of ignored events
             log_file: Set replication start log file
             log_pos: Set replication start log pos (resume_stream should be true)
             auto_position: Use master_auto_position gtid to set position
             only_tables: An array with the tables you want to watch
             only_schemas: An array with the schemas you want to watch
             freeze_schema: If true do not support ALTER TABLE. It's faster.
             skip_to_timestamp: Ignore all events until reaching specified timestamp.
+            report_slave: Report slave in SHOW SLAVE HOSTS.
+            slave_uuid: Report slave_uuid in SHOW SLAVE HOSTS.
         """
         self.__connection_settings = connection_settings
         self.__connection_settings["charset"] = "utf8"
 
         self.__connected_stream = False
         self.__connected_ctl = False
         self.__resume_stream = resume_stream
@@ -81,14 +176,23 @@
         # Store table meta information
         self.table_map = {}
         self.log_pos = log_pos
         self.log_file = log_file
         self.auto_position = auto_position
         self.skip_to_timestamp = skip_to_timestamp
 
+        if report_slave:
+            self.report_slave = ReportSlave(report_slave)
+        self.slave_uuid = slave_uuid
+
+        if pymysql_wrapper:
+            self.pymysql_wrapper = pymysql_wrapper
+        else:
+            self.pymysql_wrapper = pymysql.connect
+
     def close(self):
         if self.__connected_stream:
             self._stream_connection.close()
             self.__connected_stream = False
         if self.__connected_ctl:
             # break reference cycle between stream reader and underlying
             # mysql connection object
@@ -96,15 +200,15 @@
             self._ctl_connection.close()
             self.__connected_ctl = False
 
     def __connect_to_ctl(self):
         self._ctl_connection_settings = dict(self.__connection_settings)
         self._ctl_connection_settings["db"] = "information_schema"
         self._ctl_connection_settings["cursorclass"] = DictCursor
-        self._ctl_connection = pymysql.connect(**self._ctl_connection_settings)
+        self._ctl_connection = self.pymysql_wrapper(**self._ctl_connection_settings)
         self._ctl_connection._get_table_information = self.__get_table_information
         self.__connected_ctl = True
 
     def __checksum_enabled(self):
         """Return True if binlog-checksum = CRC32. Only for MySQL > 5.6"""
         cur = self._stream_connection.cursor()
         cur.execute("SHOW GLOBAL VARIABLES LIKE 'BINLOG_CHECKSUM'")
@@ -114,30 +218,52 @@
         if result is None:
             return False
         var, value = result[:2]
         if value == 'NONE':
             return False
         return True
 
+    def _register_slave(self):
+        if not self.report_slave:
+            return
+
+        packet = self.report_slave.encoded(self.__server_id)
+
+        if pymysql.__version__ < "0.6":
+            self._stream_connection.wfile.write(packet)
+            self._stream_connection.wfile.flush()
+            self._stream_connection.read_packet()
+        else:
+            self._stream_connection._write_bytes(packet)
+            self._stream_connection._next_seq_id = 1
+            self._stream_connection._read_packet()
+
     def __connect_to_stream(self):
         # log_pos (4) -- position in the binlog-file to start the stream with
         # flags (2) BINLOG_DUMP_NON_BLOCK (0 or 1)
         # server_id (4) -- server id of this slave
         # log_file (string.EOF) -- filename of the binlog on the master
-        self._stream_connection = pymysql.connect(**self.__connection_settings)
+        self._stream_connection = self.pymysql_wrapper(**self.__connection_settings)
 
         self.__use_checksum = self.__checksum_enabled()
 
         # If checksum is enabled we need to inform the server about the that
         # we support it
         if self.__use_checksum:
             cur = self._stream_connection.cursor()
             cur.execute("set @master_binlog_checksum= @@global.binlog_checksum")
             cur.close()
 
+        if self.slave_uuid:
+            cur = self._stream_connection.cursor()
+            cur.execute("set @slave_uuid= '%s'" % self.slave_uuid)
+            cur.close()
+
+        self._register_slave()
+
         if not self.auto_position:
             # only when log_file and log_pos both provided, the position info is
             # valid, if not, get the current position from master
             if self.log_file is None or self.log_pos is None:
                 cur = self._stream_connection.cursor()
                 cur.execute("SHOW MASTER STATUS")
                 self.log_file, self.log_pos = cur.fetchone()[:2]
@@ -222,14 +348,15 @@
             prelude += gtid_set.encoded()
 
         if pymysql.__version__ < "0.6":
             self._stream_connection.wfile.write(prelude)
             self._stream_connection.wfile.flush()
         else:
             self._stream_connection._write_bytes(prelude)
+            self._stream_connection._next_seq_id = 1
         self.__connected_stream = True
 
     def fetchone(self):
         while True:
             if not self.__connected_stream:
                 self.__connect_to_stream()
```

### Comparing `mysql-replication-0.8/pymysqlreplication/bitmap.py` & `mysql-replication-0.9/pymysqlreplication/bitmap.py`

 * *Files identical despite different names*

### Comparing `mysql-replication-0.8/pymysqlreplication/column.py` & `mysql-replication-0.9/pymysqlreplication/column.py`

 * *Files identical despite different names*

### Comparing `mysql-replication-0.8/pymysqlreplication/constants/FIELD_TYPE.py` & `mysql-replication-0.9/pymysqlreplication/constants/FIELD_TYPE.py`

 * *Files identical despite different names*

### Comparing `mysql-replication-0.8/pymysqlreplication/event.py` & `mysql-replication-0.9/pymysqlreplication/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -209,12 +209,33 @@
         print("Status vars length: %d" % (self.status_vars_length))
         print("File id: %d" % (self.file_id))
         print("Start pos: %d" % (self.start_pos))
         print("End pos: %d" % (self.end_pos))
         print("Dup handling flags: %d" % (self.dup_handling_flags))
 
 
+class IntvarEvent(BinLogEvent):
+    """
+
+    Attributes:
+        type
+        value
+    """
+    def __init__(self, from_packet, event_size, table_map, ctl_connection, **kwargs):
+        super(IntvarEvent, self).__init__(from_packet, event_size, table_map,
+                                          ctl_connection, **kwargs)
+
+        # Payload
+        self.type = self.packet.read_uint8()
+        self.value = self.packet.read_uint32()
+
+    def _dump(self):
+        super(IntvarEvent, self)._dump()
+        print("type: %d" % (self.type))
+        print("Value: %d" % (self.value))
+
+
 class NotImplementedEvent(BinLogEvent):
     def __init__(self, from_packet, event_size, table_map, ctl_connection, **kwargs):
         super(NotImplementedEvent, self).__init__(
             from_packet, event_size, table_map, ctl_connection, **kwargs)
         self.packet.advance(event_size)
```

### Comparing `mysql-replication-0.8/pymysqlreplication/gtid.py` & `mysql-replication-0.9/pymysqlreplication/gtid.py`

 * *Files 7% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 
 class GtidSet(object):
     def __init__(self, gtid_set):
         if not gtid_set:
             self.gtids = []
         else:
-            self.gtids = [Gtid(x) for x in gtid_set.split(',')]
+            self.gtids = [Gtid(x.strip(' \n')) for x in gtid_set.split(',')]
 
     def __str__(self):
         return ','.join(str(x) for x in self.gtids)
 
     def __repr__(self):
         return '<GtidSet "%s"' % ','.join(repr(x) for x in self.gtids)
```

### Comparing `mysql-replication-0.8/pymysqlreplication/packet.py` & `mysql-replication-0.9/pymysqlreplication/packet.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     __event_map = {
         # event
         constants.QUERY_EVENT: event.QueryEvent,
         constants.ROTATE_EVENT: event.RotateEvent,
         constants.FORMAT_DESCRIPTION_EVENT: event.FormatDescriptionEvent,
         constants.XID_EVENT: event.XidEvent,
-        constants.INTVAR_EVENT: event.NotImplementedEvent,
+        constants.INTVAR_EVENT: event.IntvarEvent,
         constants.GTID_LOG_EVENT: event.GtidEvent,
         constants.STOP_EVENT: event.StopEvent,
         constants.BEGIN_LOAD_QUERY_EVENT: event.BeginLoadQueryEvent,
         constants.EXECUTE_LOAD_QUERY_EVENT: event.ExecuteLoadQueryEvent,
         # row_event
         constants.UPDATE_ROWS_EVENT_V1: row_event.UpdateRowsEvent,
         constants.WRITE_ROWS_EVENT_V1: row_event.WriteRowsEvent,
```

### Comparing `mysql-replication-0.8/pymysqlreplication/row_event.py` & `mysql-replication-0.9/pymysqlreplication/row_event.py`

 * *Files identical despite different names*

### Comparing `mysql-replication-0.8/pymysqlreplication/table.py` & `mysql-replication-0.9/pymysqlreplication/table.py`

 * *Files identical despite different names*

### Comparing `mysql-replication-0.8/pymysqlreplication/tests/benchmark.py` & `mysql-replication-0.9/pymysqlreplication/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `mysql-replication-0.8/pymysqlreplication/tests/test_basic.py` & `mysql-replication-0.9/pymysqlreplication/tests/test_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,30 +28,30 @@
 
     def test_read_query_event(self):
         query = "CREATE TABLE test (id INT NOT NULL AUTO_INCREMENT, data VARCHAR (50) NOT NULL, PRIMARY KEY (id))"
         self.execute(query)
 
         event = self.stream.fetchone()
         self.assertEqual(event.position, 4)
-        self.assertEqual(event.next_binlog, "mysql-bin.000001")
+        self.assertEqual(event.next_binlog, self.bin_log_basename() + ".000001")
         self.assertIsInstance(event, RotateEvent)
 
         self.assertIsInstance(self.stream.fetchone(), FormatDescriptionEvent)
 
         event = self.stream.fetchone()
         self.assertIsInstance(event, QueryEvent)
         self.assertEqual(event.query, query)
 
     def test_read_query_event_with_unicode(self):
         query = u"CREATE TABLE `testÈ` (id INT NOT NULL AUTO_INCREMENT, dataÈ VARCHAR (50) NOT NULL, PRIMARY KEY (id))"
         self.execute(query)
 
         event = self.stream.fetchone()
         self.assertEqual(event.position, 4)
-        self.assertEqual(event.next_binlog, "mysql-bin.000001")
+        self.assertEqual(event.next_binlog, self.bin_log_basename() + ".000001")
         self.assertIsInstance(event, RotateEvent)
 
         self.assertIsInstance(self.stream.fetchone(), FormatDescriptionEvent)
 
         event = self.stream.fetchone()
         self.assertIsInstance(event, QueryEvent)
         self.assertEqual(event.query, query)
@@ -142,14 +142,15 @@
         self.execute(query)
 
         event = self.stream.fetchone()
         self.assertIsInstance(event, RotateEvent)
 
     def test_filtering_table_event(self):
         self.stream.close()
+        self.assertEqual(self.bin_log_format(), "ROW")
         self.stream = BinLogStreamReader(
             self.database,
             server_id=1024,
             only_events=[WriteRowsEvent],
             only_tables = ["test_2"])
 
         query = "CREATE TABLE test_2 (id INT NOT NULL AUTO_INCREMENT, data VARCHAR (50) NOT NULL, PRIMARY KEY (id))"
@@ -701,11 +702,20 @@
     def test_gtidset_representation(self):
         set_repr = '57b70f4e-20d3-11e5-a393-4a63946f7eac:1-56,' \
                    '4350f323-7565-4e59-8763-4b1b83a0ce0e:1-20'
 
         myset = GtidSet(set_repr)
         self.assertEqual(str(myset), set_repr)
 
+    def test_gtidset_representation_newline(self):
+        set_repr = '57b70f4e-20d3-11e5-a393-4a63946f7eac:1-56,' \
+                   '4350f323-7565-4e59-8763-4b1b83a0ce0e:1-20'
+        mysql_repr = '57b70f4e-20d3-11e5-a393-4a63946f7eac:1-56,\n' \
+                   '4350f323-7565-4e59-8763-4b1b83a0ce0e:1-20'
+
+        myset = GtidSet(mysql_repr)
+        self.assertEqual(str(myset), set_repr)
+
 
 if __name__ == "__main__":
     import unittest
     unittest.main()
```

### Comparing `mysql-replication-0.8/pymysqlreplication/tests/test_data_objects.py` & `mysql-replication-0.9/pymysqlreplication/tests/test_data_objects.py`

 * *Files identical despite different names*

### Comparing `mysql-replication-0.8/pymysqlreplication/tests/test_data_type.py` & `mysql-replication-0.9/pymysqlreplication/tests/test_data_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,15 @@
         insert_query = "INSERT INTO test VALUES('1984-12-03 12:33:07')"
         event = self.create_and_insert_value(create_query, insert_query)
         self.assertEqual(event.rows[0]["values"]["test"], datetime.datetime(1984, 12, 3, 12, 33, 7))
 
     def test_timestamp_mysql56(self):
         if not self.isMySQL56AndMore():
             self.skipTest("Not supported in this version of MySQL")
+        self.set_sql_mode()
         create_query = '''CREATE TABLE test (test0 TIMESTAMP(0),
             test1 TIMESTAMP(1),
             test2 TIMESTAMP(2),
             test3 TIMESTAMP(3),
             test4 TIMESTAMP(4),
             test5 TIMESTAMP(5),
             test6 TIMESTAMP(6));'''
@@ -245,21 +246,23 @@
         create_query = "CREATE TABLE test (id INTEGER, test DATE, test2 DATE);"
         insert_query = "INSERT INTO test (id, test2) VALUES(1, '0000-01-21')"
         event = self.create_and_insert_value(create_query, insert_query)
         self.assertEqual(event.rows[0]["values"]["test"], None)
         self.assertEqual(event.rows[0]["values"]["test2"], None)
 
     def test_zero_month(self):
+        self.set_sql_mode()
         create_query = "CREATE TABLE test (id INTEGER, test DATE, test2 DATE);"
         insert_query = "INSERT INTO test (id, test2) VALUES(1, '2015-00-21')"
         event = self.create_and_insert_value(create_query, insert_query)
         self.assertEqual(event.rows[0]["values"]["test"], None)
         self.assertEqual(event.rows[0]["values"]["test2"], None)
 
     def test_zero_day(self):
+        self.set_sql_mode()
         create_query = "CREATE TABLE test (id INTEGER, test DATE, test2 DATE);"
         insert_query = "INSERT INTO test (id, test2) VALUES(1, '2015-05-00')"
         event = self.create_and_insert_value(create_query, insert_query)
         self.assertEqual(event.rows[0]["values"]["test"], None)
         self.assertEqual(event.rows[0]["values"]["test2"], None)
 
     def test_time(self):
@@ -277,26 +280,31 @@
     def test_datetime(self):
         create_query = "CREATE TABLE test (test DATETIME);"
         insert_query = "INSERT INTO test VALUES('1984-12-03 12:33:07')"
         event = self.create_and_insert_value(create_query, insert_query)
         self.assertEqual(event.rows[0]["values"]["test"], datetime.datetime(1984, 12, 3, 12, 33, 7))
 
     def test_zero_datetime(self):
+        self.set_sql_mode()
         create_query = "CREATE TABLE test (id INTEGER, test DATETIME NOT NULL DEFAULT 0);"
         insert_query = "INSERT INTO test (id) VALUES(1)"
         event = self.create_and_insert_value(create_query, insert_query)
         self.assertEqual(event.rows[0]["values"]["test"], None)
 
     def test_broken_datetime(self):
+        self.set_sql_mode()
         create_query = "CREATE TABLE test (test DATETIME NOT NULL);"
         insert_query = "INSERT INTO test VALUES('2013-00-00 00:00:00')"
         event = self.create_and_insert_value(create_query, insert_query)
         self.assertEqual(event.rows[0]["values"]["test"], None)
 
     def test_year(self):
+        if self.isMySQL57():
+            # https://dev.mysql.com/doc/refman/5.7/en/migrating-to-year4.html
+            self.skipTest("YEAR(2) is unsupported in mysql 5.7")
         create_query = "CREATE TABLE test (a YEAR(4), b YEAR(2))"
         insert_query = "INSERT INTO test VALUES(1984, 1984)"
         event = self.create_and_insert_value(create_query, insert_query)
         self.assertEqual(event.rows[0]["values"]["a"], 1984)
         self.assertEqual(event.rows[0]["values"]["b"], 1984)
 
     def test_varchar(self):
```

### Comparing `mysql-replication-0.8/setup.py` & `mysql-replication-0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         """
         from pymysqlreplication import tests
         import unittest
 
         unittest.main(tests, argv=sys.argv[:1])
 
 
-version = "0.8"
+version = "0.9"
 
 setup(
     name="mysql-replication",
     version=version,
     url="https://github.com/noplay/python-mysql-replication",
     author="Julien Duponchelle",
     author_email="julien@duponchelle.info",
```

