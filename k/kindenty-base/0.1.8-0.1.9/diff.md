# Comparing `tmp/kindenty_base-0.1.8.tar.gz` & `tmp/kindenty_base-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kindenty_base-0.1.8.tar", last modified: Tue Apr  4 08:19:58 2023, max compression
+gzip compressed data, was "kindenty_base-0.1.9.tar", last modified: Wed Apr  5 05:43:18 2023, max compression
```

## Comparing `kindenty_base-0.1.8.tar` & `kindenty_base-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 08:19:58.642148 kindenty_base-0.1.8/
--rw-rw-rw-   0        0        0      296 2023-04-04 08:19:58.642148 kindenty_base-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1495 2023-04-02 02:58:49.000000 kindenty_base-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 08:19:58.624144 kindenty_base-0.1.8/kindenty/
--rw-rw-rw-   0        0        0        0 2021-05-30 06:13:18.000000 kindenty_base-0.1.8/kindenty/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:19:58.631137 kindenty_base-0.1.8/kindenty/base/
--rw-rw-rw-   0        0        0     3054 2022-07-03 08:49:27.000000 kindenty_base-0.1.8/kindenty/base/BaseDao.py
--rw-rw-rw-   0        0        0      679 2021-06-20 06:43:56.000000 kindenty_base-0.1.8/kindenty/base/BaseEnum.py
--rw-rw-rw-   0        0        0      463 2021-06-20 06:43:56.000000 kindenty_base-0.1.8/kindenty/base/BaseMethod.py
--rw-rw-rw-   0        0        0     2839 2022-07-03 08:49:27.000000 kindenty_base-0.1.8/kindenty/base/BaseModel.py
--rw-rw-rw-   0        0        0     6824 2023-04-03 09:25:52.000000 kindenty_base-0.1.8/kindenty/base/DatabaseDriver.py
--rw-rw-rw-   0        0        0     3434 2022-07-03 08:49:27.000000 kindenty_base-0.1.8/kindenty/base/DatabasePool.py
--rw-rw-rw-   0        0        0     1243 2021-11-26 08:09:16.000000 kindenty_base-0.1.8/kindenty/base/DatabaseType.py
--rw-rw-rw-   0        0        0      556 2021-11-28 11:49:34.000000 kindenty_base-0.1.8/kindenty/base/ExceptionModel.py
--rw-rw-rw-   0        0        0     3511 2022-07-03 08:49:27.000000 kindenty_base-0.1.8/kindenty/base/OrmField.py
--rw-rw-rw-   0        0        0     3949 2022-08-07 06:37:54.000000 kindenty_base-0.1.8/kindenty/base/QueueManager.py
--rw-rw-rw-   0        0        0     1602 2023-04-03 08:41:52.000000 kindenty_base-0.1.8/kindenty/base/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:19:58.632146 kindenty_base-0.1.8/kindenty/dao/
--rw-rw-rw-   0        0        0    33006 2023-02-23 08:14:38.000000 kindenty_base-0.1.8/kindenty/dao/DatabaseDao.py
--rw-rw-rw-   0        0        0        0 2022-07-03 11:35:10.000000 kindenty_base-0.1.8/kindenty/dao/__init__.py
--rw-rw-rw-   0        0        0     1080 2023-04-02 02:57:01.000000 kindenty_base-0.1.8/kindenty/databaseConfig.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:19:58.634146 kindenty_base-0.1.8/kindenty/model/
--rw-rw-rw-   0        0        0     2627 2022-07-03 11:36:47.000000 kindenty_base-0.1.8/kindenty/model/DataDto.py
--rw-rw-rw-   0        0        0     5692 2022-07-03 09:32:22.000000 kindenty_base-0.1.8/kindenty/model/DatabaseModel.py
--rw-rw-rw-   0        0        0        0 2022-07-03 11:35:18.000000 kindenty_base-0.1.8/kindenty/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:19:58.635138 kindenty_base-0.1.8/kindenty/mq/
--rw-rw-rw-   0        0        0        0 2023-04-04 04:41:48.000000 kindenty_base-0.1.8/kindenty/mq/__init__.py
--rw-rw-rw-   0        0        0     2457 2023-04-04 08:18:25.000000 kindenty_base-0.1.8/kindenty/mq/rabbitmq.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:19:58.641148 kindenty_base-0.1.8/kindenty_base.egg-info/
--rw-rw-rw-   0        0        0      296 2023-04-04 08:19:58.000000 kindenty_base-0.1.8/kindenty_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      712 2023-04-04 08:19:58.000000 kindenty_base-0.1.8/kindenty_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 08:19:58.000000 kindenty_base-0.1.8/kindenty_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-04 08:19:58.000000 kindenty_base-0.1.8/kindenty_base.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 08:19:58.642148 kindenty_base-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      384 2023-04-04 08:19:56.000000 kindenty_base-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-05 05:43:18.422240 kindenty_base-0.1.9/
+-rw-rw-rw-   0        0        0      296 2023-04-05 05:43:18.421238 kindenty_base-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1495 2023-04-02 02:58:49.000000 kindenty_base-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-05 05:43:18.349133 kindenty_base-0.1.9/kindenty/
+-rw-rw-rw-   0        0        0        0 2021-05-30 06:13:18.000000 kindenty_base-0.1.9/kindenty/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-05 05:43:18.394143 kindenty_base-0.1.9/kindenty/base/
+-rw-rw-rw-   0        0        0     3054 2022-07-03 08:49:27.000000 kindenty_base-0.1.9/kindenty/base/BaseDao.py
+-rw-rw-rw-   0        0        0      679 2021-06-20 06:43:56.000000 kindenty_base-0.1.9/kindenty/base/BaseEnum.py
+-rw-rw-rw-   0        0        0      463 2021-06-20 06:43:56.000000 kindenty_base-0.1.9/kindenty/base/BaseMethod.py
+-rw-rw-rw-   0        0        0     2839 2022-07-03 08:49:27.000000 kindenty_base-0.1.9/kindenty/base/BaseModel.py
+-rw-rw-rw-   0        0        0     6824 2023-04-03 09:25:52.000000 kindenty_base-0.1.9/kindenty/base/DatabaseDriver.py
+-rw-rw-rw-   0        0        0     3434 2022-07-03 08:49:27.000000 kindenty_base-0.1.9/kindenty/base/DatabasePool.py
+-rw-rw-rw-   0        0        0     1243 2021-11-26 08:09:16.000000 kindenty_base-0.1.9/kindenty/base/DatabaseType.py
+-rw-rw-rw-   0        0        0      556 2021-11-28 11:49:34.000000 kindenty_base-0.1.9/kindenty/base/ExceptionModel.py
+-rw-rw-rw-   0        0        0     3511 2022-07-03 08:49:27.000000 kindenty_base-0.1.9/kindenty/base/OrmField.py
+-rw-rw-rw-   0        0        0     3949 2022-08-07 06:37:54.000000 kindenty_base-0.1.9/kindenty/base/QueueManager.py
+-rw-rw-rw-   0        0        0     1602 2023-04-03 08:41:52.000000 kindenty_base-0.1.9/kindenty/base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-05 05:43:18.401069 kindenty_base-0.1.9/kindenty/dao/
+-rw-rw-rw-   0        0        0    33006 2023-02-23 08:14:38.000000 kindenty_base-0.1.9/kindenty/dao/DatabaseDao.py
+-rw-rw-rw-   0        0        0        0 2022-07-03 11:35:10.000000 kindenty_base-0.1.9/kindenty/dao/__init__.py
+-rw-rw-rw-   0        0        0     1080 2023-04-02 02:57:01.000000 kindenty_base-0.1.9/kindenty/databaseConfig.py
+drwxrwxrwx   0        0        0        0 2023-04-05 05:43:18.410070 kindenty_base-0.1.9/kindenty/model/
+-rw-rw-rw-   0        0        0     2627 2022-07-03 11:36:47.000000 kindenty_base-0.1.9/kindenty/model/DataDto.py
+-rw-rw-rw-   0        0        0     5692 2022-07-03 09:32:22.000000 kindenty_base-0.1.9/kindenty/model/DatabaseModel.py
+-rw-rw-rw-   0        0        0        0 2022-07-03 11:35:18.000000 kindenty_base-0.1.9/kindenty/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-05 05:43:18.411070 kindenty_base-0.1.9/kindenty/mq/
+-rw-rw-rw-   0        0        0        0 2023-04-04 04:41:48.000000 kindenty_base-0.1.9/kindenty/mq/__init__.py
+-rw-rw-rw-   0        0        0     2520 2023-04-05 04:56:26.000000 kindenty_base-0.1.9/kindenty/mq/rabbitmq.py
+drwxrwxrwx   0        0        0        0 2023-04-05 05:43:18.421238 kindenty_base-0.1.9/kindenty_base.egg-info/
+-rw-rw-rw-   0        0        0      296 2023-04-05 05:43:18.000000 kindenty_base-0.1.9/kindenty_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      712 2023-04-05 05:43:18.000000 kindenty_base-0.1.9/kindenty_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-05 05:43:18.000000 kindenty_base-0.1.9/kindenty_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-05 05:43:18.000000 kindenty_base-0.1.9/kindenty_base.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-05 05:43:18.422240 kindenty_base-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      384 2023-04-05 05:42:55.000000 kindenty_base-0.1.9/setup.py
```

### Comparing `kindenty_base-0.1.8/README.md` & `kindenty_base-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `kindenty_base-0.1.8/kindenty/base/BaseDao.py` & `kindenty_base-0.1.9/kindenty/base/BaseDao.py`

 * *Files identical despite different names*

### Comparing `kindenty_base-0.1.8/kindenty/base/BaseEnum.py` & `kindenty_base-0.1.9/kindenty/base/BaseEnum.py`

 * *Files identical despite different names*

### Comparing `kindenty_base-0.1.8/kindenty/base/BaseModel.py` & `kindenty_base-0.1.9/kindenty/base/BaseModel.py`

 * *Files identical despite different names*

### Comparing `kindenty_base-0.1.8/kindenty/base/DatabaseDriver.py` & `kindenty_base-0.1.9/kindenty/base/DatabaseDriver.py`

 * *Files identical despite different names*

### Comparing `kindenty_base-0.1.8/kindenty/base/DatabasePool.py` & `kindenty_base-0.1.9/kindenty/base/DatabasePool.py`

 * *Files identical despite different names*

### Comparing `kindenty_base-0.1.8/kindenty/base/DatabaseType.py` & `kindenty_base-0.1.9/kindenty/base/DatabaseType.py`

 * *Files identical despite different names*

### Comparing `kindenty_base-0.1.8/kindenty/base/ExceptionModel.py` & `kindenty_base-0.1.9/kindenty/base/ExceptionModel.py`

 * *Files identical despite different names*

### Comparing `kindenty_base-0.1.8/kindenty/base/OrmField.py` & `kindenty_base-0.1.9/kindenty/base/OrmField.py`

 * *Files identical despite different names*

### Comparing `kindenty_base-0.1.8/kindenty/base/QueueManager.py` & `kindenty_base-0.1.9/kindenty/base/QueueManager.py`

 * *Files identical despite different names*

### Comparing `kindenty_base-0.1.8/kindenty/base/__init__.py` & `kindenty_base-0.1.9/kindenty/base/__init__.py`

 * *Files identical despite different names*

### Comparing `kindenty_base-0.1.8/kindenty/dao/DatabaseDao.py` & `kindenty_base-0.1.9/kindenty/dao/DatabaseDao.py`

 * *Files identical despite different names*

### Comparing `kindenty_base-0.1.8/kindenty/databaseConfig.py` & `kindenty_base-0.1.9/kindenty/databaseConfig.py`

 * *Files identical despite different names*

### Comparing `kindenty_base-0.1.8/kindenty/model/DataDto.py` & `kindenty_base-0.1.9/kindenty/model/DataDto.py`

 * *Files identical despite different names*

### Comparing `kindenty_base-0.1.8/kindenty/model/DatabaseModel.py` & `kindenty_base-0.1.9/kindenty/model/DatabaseModel.py`

 * *Files identical despite different names*

### Comparing `kindenty_base-0.1.8/kindenty/mq/rabbitmq.py` & `kindenty_base-0.1.9/kindenty/mq/rabbitmq.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,54 +4,54 @@
 import pika
 from kindenty.base import log
 from pika.exchange_type import ExchangeType
 
 
 class RabbitMq:
     def __init__(self):
+        self.connection = None
         self.queue = None
         self.channel = None
         configParser = ConfigParser()
         configParser.read('conf/config.ini')
         host = configParser.get('rabbitmq', 'host')
         user = configParser.get('rabbitmq', 'userName')
         password = configParser.get('rabbitmq', 'password')
         virtualHost = configParser.get('rabbitmq', 'virtualHost')
         self.queueName = configParser.get('rabbitmq', 'queueName')
         self.routingKey = configParser.get('rabbitmq', 'routingKey')
         self.exchange = 'strategy.topic.exchange'
         userX = pika.PlainCredentials(user, password)
-        parameters = pika.ConnectionParameters(host=host, virtual_host=virtualHost, credentials=userX)
-        self.connection = pika.BlockingConnection(parameters)
+        self.parameters = pika.ConnectionParameters(host=host, virtual_host=virtualHost, credentials=userX)
         self.connect()
 
     def bindConsumer(self, fun):
         def callback(ch, method, prop, body):
             log.debug('method:%s,prop:%s,body:%s' % (method, prop, body))
             fun(method.routing_key, body)
             # self.channel.basic_ack(delivery_tag=method.delivery_tag)
-
         self.channel.basic_consume(queue=self.queueName, on_message_callback=callback, auto_ack=True)
         while True:
             try:
                 self.channel.start_consuming()
             except Exception as e:
                 log.error('rabbitmq consumer error', exc_info=e)
-                if self.channel.is_closed:
+                if not self.connection or self.channel.is_closed:
                     self.connect()
                     self.channel.basic_consume(queue=self.queueName, on_message_callback=callback, auto_ack=True)
                 time.sleep(1)
 
     def sendMsg(self, routingKey, body):
         self.channel.basic_publish(self.exchange, routing_key=routingKey, body=body)
 
     def close(self):
         self.connection.close()
 
     def connect(self):
+        self.connection = pika.BlockingConnection(self.parameters)
         self.channel = self.connection.channel()
         self.channel.exchange_declare(exchange=self.exchange, exchange_type=ExchangeType.topic,
                                       durable=True)
         self.queue = self.channel.queue_declare(self.queueName, durable=True)
         keys = self.routingKey.split(',')
         for key in keys:
             self.channel.queue_bind(queue=self.queueName, exchange=self.exchange, routing_key=key)
```

### Comparing `kindenty_base-0.1.8/kindenty_base.egg-info/SOURCES.txt` & `kindenty_base-0.1.9/kindenty_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

