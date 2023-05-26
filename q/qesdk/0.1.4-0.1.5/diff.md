# Comparing `tmp/qesdk-0.1.4.tar.gz` & `tmp/qesdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qesdk-0.1.4.tar", last modified: Fri Apr 21 16:06:59 2023, max compression
+gzip compressed data, was "qesdk-0.1.5.tar", last modified: Fri May 26 12:43:35 2023, max compression
```

## Comparing `qesdk-0.1.4.tar` & `qesdk-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 16:06:59.776979 qesdk-0.1.4/
--rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qesdk-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       36 2022-09-22 03:32:43.000000 qesdk-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6225 2023-04-21 16:06:59.775980 qesdk-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4459 2022-11-07 05:15:24.000000 qesdk-0.1.4/README.md
--rw-rw-rw-   0        0        0      751 2023-04-21 16:05:25.000000 qesdk-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 16:06:59.776979 qesdk-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 16:06:59.756980 qesdk-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 16:06:59.762979 qesdk-0.1.4/src/qesdk/
--rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.4/src/qesdk/__init__.py
--rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.4/src/qesdk/aio_api.py
--rw-rw-rw-   0        0        0    29263 2023-04-21 15:11:52.000000 qesdk-0.1.4/src/qesdk/api.py
--rw-rw-rw-   0        0        0     4929 2023-04-21 16:05:08.000000 qesdk-0.1.4/src/qesdk/client.py
--rw-rw-rw-   0        0        0      183 2022-09-19 13:40:24.000000 qesdk-0.1.4/src/qesdk/config.py
--rw-rw-rw-   0        0        0      599 2022-10-09 06:46:09.000000 qesdk-0.1.4/src/qesdk/qedata.thrift
--rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.4/src/qesdk/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 16:06:59.768979 qesdk-0.1.4/src/qesdk.egg-info/
--rw-rw-rw-   0        0        0     6225 2023-04-21 16:06:59.000000 qesdk-0.1.4/src/qesdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-04-21 16:06:59.000000 qesdk-0.1.4/src/qesdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 16:06:59.000000 qesdk-0.1.4/src/qesdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-04-21 16:06:59.000000 qesdk-0.1.4/src/qesdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-21 16:06:59.000000 qesdk-0.1.4/src/qesdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 16:06:59.774980 qesdk-0.1.4/src/qesdk2/
--rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.4/src/qesdk2/__init__.py
--rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.4/src/qesdk2/aio_api.py
--rw-rw-rw-   0        0        0    29263 2023-04-21 15:11:52.000000 qesdk-0.1.4/src/qesdk2/api.py
--rw-rw-rw-   0        0        0     4929 2023-04-10 16:40:24.000000 qesdk-0.1.4/src/qesdk2/client.py
--rw-rw-rw-   0        0        0      178 2022-11-30 10:59:44.000000 qesdk-0.1.4/src/qesdk2/config.py
--rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.4/src/qesdk2/utils.py
--rw-rw-rw-   0        0        0     1163 2023-04-21 16:01:50.000000 qesdk-0.1.4/src/test.py
--rw-rw-rw-   0        0        0     1589 2023-04-21 15:17:21.000000 qesdk-0.1.4/src/test2.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:43:35.358160 qesdk-0.1.5/
+-rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qesdk-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       36 2022-09-22 03:32:43.000000 qesdk-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6225 2023-05-26 12:43:35.358160 qesdk-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4459 2022-11-07 05:15:24.000000 qesdk-0.1.5/README.md
+-rw-rw-rw-   0        0        0      751 2023-05-26 12:41:35.000000 qesdk-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 12:43:35.358160 qesdk-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 12:43:35.339160 qesdk-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 12:43:35.346160 qesdk-0.1.5/src/qesdk/
+-rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.5/src/qesdk/__init__.py
+-rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.5/src/qesdk/aio_api.py
+-rw-rw-rw-   0        0        0    29263 2023-04-21 15:11:52.000000 qesdk-0.1.5/src/qesdk/api.py
+-rw-rw-rw-   0        0        0     6805 2023-05-26 12:41:18.000000 qesdk-0.1.5/src/qesdk/client.py
+-rw-rw-rw-   0        0        0      237 2023-05-26 12:40:26.000000 qesdk-0.1.5/src/qesdk/config.py
+-rw-rw-rw-   0        0        0      599 2022-10-09 06:46:09.000000 qesdk-0.1.5/src/qesdk/qedata.thrift
+-rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.5/src/qesdk/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:43:35.351163 qesdk-0.1.5/src/qesdk.egg-info/
+-rw-rw-rw-   0        0        0     6225 2023-05-26 12:43:35.000000 qesdk-0.1.5/src/qesdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-05-26 12:43:35.000000 qesdk-0.1.5/src/qesdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 12:43:35.000000 qesdk-0.1.5/src/qesdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-05-26 12:43:35.000000 qesdk-0.1.5/src/qesdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-26 12:43:35.000000 qesdk-0.1.5/src/qesdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 12:43:35.357159 qesdk-0.1.5/src/qesdk2/
+-rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.5/src/qesdk2/__init__.py
+-rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.5/src/qesdk2/aio_api.py
+-rw-rw-rw-   0        0        0    29263 2023-04-21 15:11:52.000000 qesdk-0.1.5/src/qesdk2/api.py
+-rw-rw-rw-   0        0        0     4929 2023-05-15 05:31:36.000000 qesdk-0.1.5/src/qesdk2/client.py
+-rw-rw-rw-   0        0        0     5339 2023-05-15 05:35:29.000000 qesdk-0.1.5/src/qesdk2/clienttest.py
+-rw-rw-rw-   0        0        0      183 2023-05-19 14:14:05.000000 qesdk-0.1.5/src/qesdk2/config.py
+-rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.5/src/qesdk2/utils.py
+-rw-rw-rw-   0        0        0     2092 2023-05-24 14:13:05.000000 qesdk-0.1.5/src/test.py
+-rw-rw-rw-   0        0        0     2219 2023-05-26 11:43:19.000000 qesdk-0.1.5/src/test2.py
```

### Comparing `qesdk-0.1.4/LICENSE` & `qesdk-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.4/PKG-INFO` & `qesdk-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qesdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Quantease SDK for quants
 Author-email: Scott Zhang <scott2011@qq.com>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `qesdk-0.1.4/README.md` & `qesdk-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.4/pyproject.toml` & `qesdk-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qesdk"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Scott Zhang", email="scott2011@qq.com" },
 ]
 description = "Quantease SDK for quants"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `qesdk-0.1.4/src/qesdk/aio_api.py` & `qesdk-0.1.5/src/qesdk/aio_api.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.4/src/qesdk/api.py` & `qesdk-0.1.5/src/qesdk/api.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.4/src/qesdk/client.py` & `qesdk-0.1.5/src/qesdk2/client.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.4/src/qesdk/qedata.thrift` & `qesdk-0.1.5/src/qesdk/qedata.thrift`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.4/src/qesdk/utils.py` & `qesdk-0.1.5/src/qesdk/utils.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.4/src/qesdk.egg-info/PKG-INFO` & `qesdk-0.1.5/src/qesdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qesdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Quantease SDK for quants
 Author-email: Scott Zhang <scott2011@qq.com>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `qesdk-0.1.4/src/qesdk2/aio_api.py` & `qesdk-0.1.5/src/qesdk2/aio_api.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.4/src/qesdk2/api.py` & `qesdk-0.1.5/src/qesdk2/api.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.4/src/qesdk2/client.py` & `qesdk-0.1.5/src/qesdk2/clienttest.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,33 +11,31 @@
 import pickle
 import msgpack
 import json
 import sys
 from os import getenv, path
 
 from thriftpy2.rpc import make_aio_client
-from .utils import get_mac_address
+from utils import get_mac_address
 import nest_asyncio
 nest_asyncio.apply()
 
 try:
     from .config import outside_server_config
     server_config = outside_server_config
 except ImportError:
     server_config = {'host' : '192.168.123.13',
                      'port' : 6001}    
 
 
 
-__version__='0.1.3'
+__version__='0.1.4'
 
-thrift_path = path.join(sys.modules["ROOT_DIR"], "qedata.thrift")
-thrift_path = path.abspath(thrift_path)
 #print(thrift_path)
-qedata_thrift = thriftpy2.load(thrift_path, module_name="qedata_thrift")
+qedata_thrift = thriftpy2.load("qedata.thrift", module_name="qedata_thrift")
 loop = asyncio.get_event_loop()
 def setTimeout(client, timeout):
     try:
         try:
                 sock = client._iprot.trans._trans.sock
         except AttributeError:
                 sock = client._iprot.trans.sock
@@ -154,7 +152,24 @@
 def check_auth():
     return qedataClient.check_auth()
     
     
 def testClient():
     #loop.run_until_complete(qedataClient.instance().auth('quantease','$1$$k7yjPQKv8AJuZERDA.eQX.'))
     asyncio.run(qedataClient.instance().echo('test'))
+
+async def connect():
+
+    try:
+        print(server_config)
+        client = await make_aio_client(qedata_thrift.TestService, server_config['host'],  server_config['port'],timeout=10000)
+    except:
+        print('timeout')
+        try:
+            client = await make_aio_client(qedata_thrift.TestService, '103.36.172.183',  6001,timeout=10000)
+        except:
+            print('timeout 2')
+        else:
+            print('connected')
+if __name__ == "__main__":
+    asyncio.run(connect())
+
```

### Comparing `qesdk-0.1.4/src/qesdk2/utils.py` & `qesdk-0.1.5/src/qesdk2/utils.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.4/src/test.py` & `qesdk-0.1.5/src/test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,60 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri Sep 23 21:41:10 2022
 
 @author: ScottStation
 """
 
-
 import qesdk
+import pandas as pd
 qesdk.auth('quantease','$1$$k7yjPQKv8AJuZERDA.eQX.')
 #qesdk.auth('qestratmarket','$1$$BbR4MSZT9isFx3PBepvxd/')
 #qesdk.auth('Scott_1665208401','$1$$oaWXYSWPp1jpTQmndXJcK/')
 #print(qesdk.check_auth())
-print(qesdk.get_bar_data(["AU2312.SFE"], "2023-04-24"))
+
+#for p in ["AG",'ME',"RO","TC","WS","ER"]:
+#    con = qesdk.get_valid_instID(p+"9999")
+#    print(con,qesdk.get_price(con,'2023-05-03','2023-05-05'))
+print(qesdk.get_price('SI2308.GFE','2023-04-27','2023-05-26','daily'))
+print(qesdk.get_price('SI2308.GFE','2023-04-27','2023-05-26','minute'))
+print(qesdk.get_ticks('IF2306.CCF','2023-05-21','2023-05-26'))
+print(qesdk.get_prod_open_time('AU2312.SFE'))
+print(qesdk.get_prod_open_time('IC2306.CCF'))
+#print(qesdk.get_dominant_instID("IC",'2023-05-08','9999'))
+#print(qesdk.get_dominant_instIDs(['IC','AG','SI'], '2023-05-01', "2023-05-09"))
+#print(qesdk.get_instrument_setting('T2305.CCF'))
+inst = "AG2312.SFE"
+ddict = qesdk.get_bar_data([inst], "2023-05-23")
+print(ddict)
+df = ddict[inst]
+#print(type(df.index[0]))
+#df['runtime']= pd.to_datetime(df.index, format='%Y%m%d%H%M%S',errors='ignore')
+#df.set_index(["runtime"], inplace=True)
+print(df)
+#print(ddict[inst].columns)
+
 #print(qesdk.update_public_ip('180.161.73.253'))
-'''
+
 qesdk.login('scott','12345678')
+
 stratlist=(qesdk.sm_get_clone_strat_list())
 print('strats',stratlist)
+'''
 if stratlist and isinstance(stratlist,list) and len(stratlist) > 0:
     print(qesdk.sm_get_clone_strat_position(stratlist))
 
 #df = qesdk.get_instrument_broker_pnl('东证期货','AU2306.SFE','2023-02-24','2023-02-28')
 #df = qesdk.get_product_invent_orders('CU', '2023-02-01','2023-02-14')
 inst = 'AU2312.SFE'
 data = qesdk.get_bar_data([inst], '',5,freq=5)
 #df = qesdk.get_realtime_minute_prices(['AU2312.SFE','AG2401.SFE'])
 print(data[inst])'''
 #print(df['510300.SSE'].columns)
     
 #qesdk.auth('quantease','$1$$k7yjPQKv8AJuZERDA.eQX.')
 #
 #print(df)
-#print(qesdk2.get_price('AG2212.SFE','2022-09-01','2022-09-22'))
+#print(qesdk2.get_price('AG2212.SFE','2022-09-01','2022-09-22'))口红  
+
+
+
```

### Comparing `qesdk-0.1.4/src/test2.py` & `qesdk-0.1.5/src/test2.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,15 +21,32 @@
     vers= sys.version.split('.')
     return '_'.join(vers[:2])
 
 def get_plat():
     return platform.system().lower()
 
 qesdk2.auth('quantease','$1$$k7yjPQKv8AJuZERDA.eQX.')
-qesdk2.update_public_ip('1.1.1.1')
+
+print(qesdk2.get_price('SI2308.GFE','2023-04-27','2023-05-28','daily'))
+#print(qesdk2.get_price('SI2308.GFE','2023-04-27','2023-05-28','minute'))
+#print(qesdk2.get_ticks('IF2305.CCF','2023-04-28','2023-05-26'))
+print(qesdk2.get_prod_open_time('AU2312.SFE'))
+print(qesdk2.get_prod_open_time('IC2306.CCF'))
+#print(qesdk.get_dominant_instID("IC",'2023-05-08','9999'))
+#print(qesdk.get_dominant_instIDs(['IC','AG','SI'], '2023-05-01', "2023-05-09"))
+#print(qesdk.get_instrument_setting('T2305.CCF'))
+inst = "AG2312.SFE"
+ddict = qesdk2.get_bar_data([inst], "2023-05-26")
+print(ddict)
+#qesdk2.update_public_ip('1.1.1.1')
+'''
+qesdk2.login('scott','12345678')
+
+stratlist=(qesdk2.sm_get_clone_strat_list())
+print('strats',stratlist)
 
 #df = qesdk2.get_product_invent_orders('CU', '2023-02-01','2023-02-14')
 #print(df)
 #msg = qesdk2.get_package_address('algoex', get_plat(), get_ver(), get_mac_address())
 #print(msg)
 #print(qesdk2.get_plugin_permission('algoex','windows','3_8',get_mac_address(),'test','quantease'))
 #df = qesdk.get_price('AG2212.SFE','2022-10-01','2022-11-01','daily')
@@ -39,14 +56,12 @@
 #print(qesdk2.get_broker_info('cjqh3'))
 #print(qesdk2.get_valid_instID('si9w'))#
 #print(qesdk2.is_valid_instID('IC2309.SFE'))
 #print(qesdk2.is_valid_trade_time('IC2306.SFE',datetime.now()+timedelta(hours=5)))
 #df = qesdk.get_realtime_minute_prices(['AU2212_SFE','AG2301.SFE'])
 #print(df)
 
-testdf = qesdk2.get_bar_data(['AU2312.SFE'],'2022-12-06')
-print(testdf)
-'''
+
 for i in testdf['AU2212.SFE'].index:
     print(testdf['AU2212.SFE'].loc[i,'time'],testdf['AU2212.SFE'].loc[i, 'close'])
 testdf['AU2212.SFE']['close'].plot()    
 '''
```

