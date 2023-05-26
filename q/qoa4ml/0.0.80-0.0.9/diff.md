# Comparing `tmp/qoa4ml-0.0.80.tar.gz` & `tmp/qoa4ml-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qoa4ml-0.0.80.tar", last modified: Fri May 26 10:53:37 2023, max compression
+gzip compressed data, was "/Users/tringuyen/workplace/Study/PhD/Gitlab/qoa4ml/dev/package/dist/tmp8wasmwge/qoa4ml-0.0.9.tar", last modified: Wed Mar 23 15:38:02 2022, max compression
```

## Comparing `qoa4ml-0.0.80.tar` & `qoa4ml-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,34 @@
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-05-26 10:53:37.608025 qoa4ml-0.0.80/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.0.80/CHANGELOG.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.0.80/LICENCE.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       30 2022-03-23 13:04:50.000000 qoa4ml-0.0.80/MANIFEST.in
--rw-r--r--   0 tringuyen   (501) wheel        (0)     9190 2023-05-26 10:53:37.607719 qoa4ml-0.0.80/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6843 2023-05-22 10:07:32.000000 qoa4ml-0.0.80/README.md
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-05-26 10:53:37.595736 qoa4ml-0.0.80/conf/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      122 2023-05-22 08:28:02.000000 qoa4ml-0.0.80/conf/client.json
--rw-r--r--   0 tringuyen   (501) wheel        (0)      287 2023-04-18 14:34:40.000000 qoa4ml-0.0.80/conf/collector.json
--rw-r--r--   0 tringuyen   (501) wheel        (0)      251 2022-05-10 09:59:56.000000 qoa4ml-0.0.80/conf/connector.json
--rw-r--r--   0 tringuyen   (501) wheel        (0)      343 2023-05-21 08:59:44.000000 qoa4ml-0.0.80/conf/metrics.json
--rw-r--r--   0 tringuyen   (501) wheel        (0)      795 2022-06-01 03:09:16.000000 qoa4ml-0.0.80/conf/system_metric.json
--rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.0.80/pyproject.toml
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-05-26 10:53:37.599597 qoa4ml-0.0.80/qoa4ml/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-18 16:53:28.000000 qoa4ml-0.0.80/qoa4ml/__init__.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-05-26 10:53:37.602579 qoa4ml-0.0.80/qoa4ml/collector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.0.80/qoa4ml/collector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.0.80/qoa4ml/collector/amqp_collector.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-05-26 10:53:37.606876 qoa4ml-0.0.80/qoa4ml/connector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.0.80/qoa4ml/connector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.0.80/qoa4ml/connector/amqp_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.0.80/qoa4ml/connector/mess_logging.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.0.80/qoa4ml/connector/mqtt_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.0.80/qoa4ml/connector/prom_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4162 2023-05-25 14:14:17.000000 qoa4ml-0.0.80/qoa4ml/probes.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)    10461 2023-05-26 10:52:52.000000 qoa4ml-0.0.80/qoa4ml/qoa_client.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4470 2023-05-22 08:59:17.000000 qoa4ml-0.0.80/qoa4ml/reports.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     9789 2023-05-26 07:48:38.000000 qoa4ml-0.0.80/qoa4ml/utils.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-05-26 10:53:37.601869 qoa4ml-0.0.80/qoa4ml.egg-info/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     9190 2023-05-26 10:53:37.000000 qoa4ml-0.0.80/qoa4ml.egg-info/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)      641 2023-05-26 10:53:37.000000 qoa4ml-0.0.80/qoa4ml.egg-info/SOURCES.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-05-26 10:53:37.000000 qoa4ml-0.0.80/qoa4ml.egg-info/dependency_links.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       56 2023-05-26 10:53:37.000000 qoa4ml-0.0.80/qoa4ml.egg-info/requires.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-05-26 10:53:37.000000 qoa4ml-0.0.80/qoa4ml.egg-info/top_level.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-05-26 10:53:37.608135 qoa4ml-0.0.80/setup.cfg
--rw-r--r--   0 tringuyen   (501) wheel        (0)      585 2023-05-26 10:53:33.000000 qoa4ml-0.0.80/setup.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 15:38:02.771130 qoa4ml-0.0.9/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       90 2022-03-23 14:33:16.000000 qoa4ml-0.0.9/CHANGELOG.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.0.9/LICENCE.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       30 2022-03-23 13:04:50.000000 qoa4ml-0.0.9/MANIFEST.in
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      385 2022-03-23 15:38:02.770846 qoa4ml-0.0.9/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       40 2022-03-23 13:08:51.000000 qoa4ml-0.0.9/README.md
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-03-23 13:35:28.000000 qoa4ml-0.0.9/pyproject.toml
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 15:38:02.764143 qoa4ml-0.0.9/qoa4ml/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-18 16:53:28.000000 qoa4ml-0.0.9/qoa4ml/__init__.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 15:38:02.766490 qoa4ml-0.0.9/qoa4ml/collector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.0.9/qoa4ml/collector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1903 2022-03-23 11:58:56.000000 qoa4ml-0.0.9/qoa4ml/collector/qmqp_collector.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 15:38:02.768303 qoa4ml-0.0.9/qoa4ml/connector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.0.9/qoa4ml/connector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1794 2022-03-23 10:27:57.000000 qoa4ml-0.0.9/qoa4ml/connector/amqp_client.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.0.9/qoa4ml/connector/mess_logging.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.0.9/qoa4ml/connector/mqtt_client.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.0.9/qoa4ml/connector/prom_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     3240 2022-03-23 11:09:47.000000 qoa4ml-0.0.9/qoa4ml/probes.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 15:38:02.770238 qoa4ml-0.0.9/qoa4ml/qoa4ml.egg-info/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      554 2022-03-23 13:59:35.000000 qoa4ml-0.0.9/qoa4ml/qoa4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2022-03-23 13:59:35.000000 qoa4ml-0.0.9/qoa4ml/qoa4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       14 2022-03-23 13:59:35.000000 qoa4ml-0.0.9/qoa4ml/qoa4ml.egg-info/requires.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2022-03-23 13:59:35.000000 qoa4ml-0.0.9/qoa4ml/qoa4ml.egg-info/top_level.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4039 2022-03-23 12:05:46.000000 qoa4ml-0.0.9/qoa4ml/reports.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1281 2022-03-23 15:36:03.000000 qoa4ml-0.0.9/qoa4ml/utils.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 15:38:02.766029 qoa4ml-0.0.9/qoa4ml.egg-info/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      385 2022-03-23 15:38:02.000000 qoa4ml-0.0.9/qoa4ml.egg-info/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      667 2022-03-23 15:38:02.000000 qoa4ml-0.0.9/qoa4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2022-03-23 15:38:02.000000 qoa4ml-0.0.9/qoa4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       14 2022-03-23 15:38:02.000000 qoa4ml-0.0.9/qoa4ml.egg-info/requires.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2022-03-23 15:38:02.000000 qoa4ml-0.0.9/qoa4ml.egg-info/top_level.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2022-03-23 15:38:02.771231 qoa4ml-0.0.9/setup.cfg
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      518 2022-03-23 15:37:47.000000 qoa4ml-0.0.9/setup.py
```

### Comparing `qoa4ml-0.0.80/LICENCE.txt` & `qoa4ml-0.0.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.80/qoa4ml/collector/amqp_collector.py` & `qoa4ml-0.0.9/qoa4ml/collector/qmqp_collector.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,18 +5,15 @@
     def __init__(self, configuration:dict, host_object:object=None):
         self.host_object = host_object  
         self.exchange_name = configuration["exchange_name"]
         self.exchange_type = configuration["exchange_type"]
         self.in_routing_key = configuration["in_routing_key"]
 
         # Connect to RabbitMQ host
-        if "amqps://" in configuration["end_point"]:
-            self.in_connection = pika.BlockingConnection(pika.URLParameters(configuration["end_point"]))
-        else:
-            self.in_connection = pika.BlockingConnection(pika.ConnectionParameters(host=configuration["end_point"]))
+        self.in_connection = pika.BlockingConnection(pika.ConnectionParameters(host=configuration["end_point"]))
         
         # Create a channel
         self.in_channel = self.in_connection.channel()
         
         # Init an Exchange 
         self.in_channel.exchange_declare(exchange=self.exchange_name, exchange_type=self.exchange_type)
         
@@ -39,12 +36,11 @@
     def start(self):
         # Start rabbit MQ
         self.in_channel.basic_qos(prefetch_count=1)
         self.in_channel.basic_consume(queue=self.queue_name,on_message_callback=self.on_request,auto_ack=True)
         self.in_channel.start_consuming()
 
     def stop(self):
-        self.in_channel.stop_consuming()
         self.in_channel.close()
 
     def get_queue(self):
         return self.queue.method.queue
```

### Comparing `qoa4ml-0.0.80/qoa4ml/connector/amqp_connector.py` & `qoa4ml-0.0.9/qoa4ml/connector/amqp_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pika, uuid
+import pika
 from .mess_logging import Mess_Logging
 
 class Amqp_Connector(object):
     # Init an amqp client handling the connection to amqp servier
     def __init__(self, configuration:dict, log:bool=False): 
         """
         AMQP connector
@@ -12,34 +12,29 @@
         self.conf = configuration
         self.exchange_name = configuration["exchange_name"]
         self.exchange_type = configuration["exchange_type"]
         self.out_routing_key = configuration["out_routing_key"]
         self.log_flag = log
 
         # Connect to RabbitMQ host
-        if "amqps://" in configuration["end_point"]:
-            self.out_connection = pika.BlockingConnection(pika.URLParameters(configuration["end_point"]))
-        else:
-            self.out_connection = pika.BlockingConnection(pika.ConnectionParameters(host=configuration["end_point"]))        
+        self.out_connection = pika.BlockingConnection(pika.ConnectionParameters(host=configuration["end_point"]))        
 
         # Create a channel
         self.out_channel = self.out_connection.channel()
         
         # Init an Exchange 
         self.out_channel.exchange_declare(exchange=self.exchange_name, exchange_type=self.exchange_type)
         
 
-    def send_data(self, body_mess, corr_id=None, routing_key=None,expiration=1000):
+    def send_data(self, body_mess, corr_id, routing_key=None):
         # Sending data to desired destination
         # if sender is client, it will include the "reply_to" attribute to specify where to reply this message
         # if sender is server, it will reply the message to "reply_to" via default exchange 
-        if corr_id == None:
-            corr_id = str(uuid.uuid4())
         if routing_key == None:
             routing_key = self.out_routing_key
-        self.sub_properties = pika.BasicProperties(correlation_id=corr_id,expiration=str(expiration))
+        self.sub_properties = pika.BasicProperties(correlation_id=corr_id)
         self.out_channel.basic_publish(exchange=self.exchange_name,routing_key=routing_key,properties=self.sub_properties,body=body_mess)
         # if self.log_flag:
         #     self.mess_logging.log_request(body_mess,corr_id)
 
     def get(self):
         return self.conf
```

### Comparing `qoa4ml-0.0.80/qoa4ml/connector/mess_logging.py` & `qoa4ml-0.0.9/qoa4ml/connector/mess_logging.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.80/qoa4ml/connector/mqtt_connector.py` & `qoa4ml-0.0.9/qoa4ml/connector/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.80/qoa4ml/connector/prom_connector.py` & `qoa4ml-0.0.9/qoa4ml/connector/prom_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.80/qoa4ml.egg-info/SOURCES.txt` & `qoa4ml-0.0.9/qoa4ml/qoa4ml.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 CHANGELOG.txt
 LICENCE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
-conf/client.json
-conf/collector.json
-conf/connector.json
-conf/metrics.json
-conf/system_metric.json
+test_client.py
+test_collector.py
 qoa4ml/__init__.py
 qoa4ml/probes.py
-qoa4ml/qoa_client.py
 qoa4ml/reports.py
 qoa4ml/utils.py
-qoa4ml.egg-info/PKG-INFO
-qoa4ml.egg-info/SOURCES.txt
-qoa4ml.egg-info/dependency_links.txt
-qoa4ml.egg-info/requires.txt
-qoa4ml.egg-info/top_level.txt
-qoa4ml/collector/__init__.py
-qoa4ml/collector/amqp_collector.py
+qoa4ml/collector/qmqp_collector.py
 qoa4ml/connector/__init__.py
-qoa4ml/connector/amqp_connector.py
+qoa4ml/connector/amqp_client.py
 qoa4ml/connector/mess_logging.py
-qoa4ml/connector/mqtt_connector.py
-qoa4ml/connector/prom_connector.py
+qoa4ml/connector/mqtt_client.py
+qoa4ml/connector/prom_connector.py
+qoa4ml/qoa4ml.egg-info/PKG-INFO
+qoa4ml/qoa4ml.egg-info/SOURCES.txt
+qoa4ml/qoa4ml.egg-info/dependency_links.txt
+qoa4ml/qoa4ml.egg-info/requires.txt
+qoa4ml/qoa4ml.egg-info/top_level.txt
```

### Comparing `qoa4ml-0.0.80/setup.py` & `qoa4ml-0.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import find_packages, setup
 
 setup(
     name='qoa4ml',
-    version='0.0.80',
+    version='0.0.9',
     description='Quality of Analysis for Machine Learning',
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     long_description_content_type='text/markdown',
     url='https://rdsea.github.io/',
     author='Aaltosea',
     email='tri.m.nguyen@aalto.fi',
     keyword='Monitoring Machine Learning',
-    install_requires=['pika','requests','paho-mqtt','prometheus-client','psutil', 'docker'],
+    install_requires=['pika','requests'],
     packages=find_packages(),
-    license='Apache License 2.0'
+    license='MIT'
 )
```

