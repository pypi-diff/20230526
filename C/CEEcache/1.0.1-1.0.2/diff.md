# Comparing `tmp/CEEcache-1.0.1.tar.gz` & `tmp/CEEcache-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CEEcache-1.0.1.tar", last modified: Thu May 25 10:30:39 2023, max compression
+gzip compressed data, was "CEEcache-1.0.2.tar", last modified: Fri May 26 05:40:20 2023, max compression
```

## Comparing `CEEcache-1.0.1.tar` & `CEEcache-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-25 10:30:39.643784 CEEcache-1.0.1/
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-25 10:30:39.643784 CEEcache-1.0.1/CEEcache/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     5611 2023-05-25 10:30:17.000000 CEEcache-1.0.1/CEEcache/__init__.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1527 2023-05-25 10:26:33.000000 CEEcache-1.0.1/CEEcache/logger.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-25 10:30:39.643784 CEEcache-1.0.1/CEEcache.egg-info/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      604 2023-05-25 10:30:39.000000 CEEcache-1.0.1/CEEcache.egg-info/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      256 2023-05-25 10:30:39.000000 CEEcache-1.0.1/CEEcache.egg-info/SOURCES.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2023-05-25 10:30:39.000000 CEEcache-1.0.1/CEEcache.egg-info/dependency_links.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       43 2023-05-25 10:30:39.000000 CEEcache-1.0.1/CEEcache.egg-info/requires.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        9 2023-05-25 10:30:39.000000 CEEcache-1.0.1/CEEcache.egg-info/top_level.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       78 2023-05-22 13:09:12.000000 CEEcache-1.0.1/CHANGELOG.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1070 2023-05-22 13:12:22.000000 CEEcache-1.0.1/LICENCE.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       25 2023-05-22 13:10:04.000000 CEEcache-1.0.1/MANIFEST.in
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      604 2023-05-25 10:30:39.643784 CEEcache-1.0.1/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      115 2023-05-22 13:06:57.000000 CEEcache-1.0.1/README.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       38 2023-05-25 10:30:39.643784 CEEcache-1.0.1/setup.cfg
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      626 2023-05-25 10:30:36.000000 CEEcache-1.0.1/setup.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-26 05:40:20.348843 CEEcache-1.0.2/
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-26 05:40:20.344843 CEEcache-1.0.2/CEEcache/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     6610 2023-05-26 05:39:02.000000 CEEcache-1.0.2/CEEcache/__init__.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1527 2023-05-26 05:39:34.000000 CEEcache-1.0.2/CEEcache/logger.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-26 05:40:20.348843 CEEcache-1.0.2/CEEcache.egg-info/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      604 2023-05-26 05:40:20.000000 CEEcache-1.0.2/CEEcache.egg-info/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      256 2023-05-26 05:40:20.000000 CEEcache-1.0.2/CEEcache.egg-info/SOURCES.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2023-05-26 05:40:20.000000 CEEcache-1.0.2/CEEcache.egg-info/dependency_links.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       43 2023-05-26 05:40:20.000000 CEEcache-1.0.2/CEEcache.egg-info/requires.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        9 2023-05-26 05:40:20.000000 CEEcache-1.0.2/CEEcache.egg-info/top_level.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       78 2023-05-22 13:09:12.000000 CEEcache-1.0.2/CHANGELOG.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1070 2023-05-22 13:12:22.000000 CEEcache-1.0.2/LICENCE.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       25 2023-05-22 13:10:04.000000 CEEcache-1.0.2/MANIFEST.in
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      604 2023-05-26 05:40:20.348843 CEEcache-1.0.2/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      115 2023-05-22 13:06:57.000000 CEEcache-1.0.2/README.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       38 2023-05-26 05:40:20.348843 CEEcache-1.0.2/setup.cfg
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      626 2023-05-26 05:39:48.000000 CEEcache-1.0.2/setup.py
```

### Comparing `CEEcache-1.0.1/CEEcache/__init__.py` & `CEEcache-1.0.2/CEEcache/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,50 +26,49 @@
         else:
             return sorted(d)
     else:
         return d
 
 def generate_key(payload, md5_key_include, md5_key_exclude, prepend_key, request_id):
     try:
+        global md5_key
         payload_copy = copy.deepcopy(payload)
         # If both md5_key_include and md5_key_exclude is passed then only md5_key_include will be given selected.
         if md5_key_include:
             filtered_payload = {k: v for k, v in payload_copy.items() if k in md5_key_include}
         elif md5_key_exclude:
             filtered_payload = {k: v for k, v in payload_copy.items() if k not in md5_key_exclude}
         else:
             filtered_payload = payload_copy
         filtered_payload = sort_json_recursively(filtered_payload)
         json_string = json.dumps(filtered_payload)
         md5_hash = hashlib.md5(json_string.encode()).hexdigest()
-        client_id = payload_copy['cid']
-        key = f'{client_id}_{md5_hash}'
+        client_id = payload_copy["cid"]
+        md5_key = f"{client_id}_{md5_hash}"
         if prepend_key:
-            key = prepend_key + "_" + key
-        log_emmiter({'request_id': request_id, 'key_generated': key})
-        return key
+            md5_key = prepend_key + "_" + md5_key
+        log_emmiter({"request_id": request_id, "key_generated": md5_key})
     except:
         e = sys.exc_info()
         traceback_output = "".join(traceback.format_exception(e[0], e[1], e[2]))
         err_msg = f"Error occured while generating key for request_id: {request_id}\n{str(traceback_output)}"
         print(err_msg)
-        log_emmiter({'request_id': request_id, 'message': err_msg}, 'ERROR')
+        log_emmiter({"request_id": request_id, "message": err_msg}, "ERROR")
         send_slack_alert(err_msg, request_id)
-        return None
+        md5_key = None
 
 def send_slack_alert(err_msg, request_id):
-    
     url = os.environ.get("slack_web_hook", "")
-    headers = {'Content-Type': 'application/json'}
-    payload = {'text': err_msg}
+    headers = {"Content-Type": "application/json"}
+    payload = {"text": err_msg}
     response = requests.post(url, headers=headers, data=json.dumps(payload))
     if response.status_code != 200:
-        err_msg = f'Failed to send Slack message. Error: {response.text}'
+        err_msg = f"Failed to send Slack message. Error: {response.text}"
         print(err_msg)
-        log_emmiter({'request_id': request_id, 'message': err_msg}, 'ERROR')
+        log_emmiter({"request_id": request_id, "message": err_msg}, "ERROR")
 
 def connect_to_redis(request_id):
     max_attempts = 3
     retry_delay = 3
     host = os.environ.get("cache_redis_host", "")
     port = int(os.environ.get("cache_redis_port", 0))
     r = redis.Redis(host, port, db = 0)
@@ -79,85 +78,108 @@
                 return r
             else:
                 time.sleep(retry_delay)
         except:
             time.sleep(retry_delay)
     err_msg = f"Error occured while connecting to redis host: {host}, port: {port} within the caching library.\nrequest_id: {request_id}"
     print(err_msg)
-    log_emmiter({'request_id': request_id, 'message': err_msg}, 'ERROR')
+    log_emmiter({"request_id": request_id, "message": err_msg}, "ERROR")
     send_slack_alert(err_msg, request_id)
     return None
 
-def read_from_redis(key, request_id):
+def read_from_redis(request_id):
     r = connect_to_redis(request_id)
     if r is None:
         return None
     resp = None
-    if r.exists(key):
-        resp_str = r.hget(key, 'value').decode('utf-8')
+    if r.exists(md5_key):
+        resp_str = r.hget(md5_key, "value").decode("utf-8")
         resp = json.loads(resp_str)
     r.close()
     return resp
 
-def write_to_redis(key, value, ttl, force_reset, request_id):
-    if key is None:
+def write_to_redis(payload, value):
+    caching_info = payload.get("caching_info", {})
+    ttl = caching_info.get("stale_time_acceptable", int(os.environ.get("stale_time_acceptable", 0)))
+    force_reset = caching_info.get("force_reset", 0)
+    request_id = payload.get("request_id", "")
+    
+    if ttl == 0:
         return None
+    if md5_key is None:
+        return None
+    
     r = connect_to_redis(request_id)
     if r is None:
         return None
+    
     timestamp = time.time()
-    r.hset(key, 'value', json.dumps(value))
-    r.hset(key, 'set_time', timestamp)
-    if force_reset == 1 or r.ttl(key) < ttl * 60:
-        r.expire(key, ttl * 60)
+    r.hset(md5_key, "value", json.dumps(value))
+    r.hset(md5_key, "set_time", timestamp)
+    if force_reset == 1 or r.ttl(md5_key) < ttl * 60:
+        r.expire(md5_key, ttl * 60)
     r.close()
 
-def get_cache_set_time(key, request_id):
+def get_cache_set_time(request_id):
     r = connect_to_redis(request_id)
     if r is None:
         return None
-    resp_str = r.hget(key, 'set_time').decode('utf-8')
+    resp_str = r.hget(md5_key, "set_time").decode("utf-8")
     resp = float(resp_str)
     r.close()
     return resp
 
-def change_ttl(key, ttl, request_id):
+def change_ttl(ttl, request_id):
     r = connect_to_redis(request_id)
     if r is None:
         return None
-    if r.ttl(key) < ttl * 60:
-        r.expire(key, ttl * 60)
+    if r.ttl(md5_key) < ttl * 60:
+        r.expire(md5_key, ttl * 60)
     r.close()
 
-def main(key, stale_time_acceptable, force_reset, request_id):
-    if key is None:
+def main(payload, md5_key_include, md5_key_exclude):
+    request_id = payload.get("request_id", "")
+    caching_info = payload.get("caching_info", {})
+    stale_time_acceptable = caching_info.get("stale_time_acceptable", int(os.environ.get("stale_time_acceptable", 0)))
+    force_reset = caching_info.get("force_reset", 0)
+    prepend_key = caching_info.get("prepend_key", os.environ.get("prepend_key", None))
+    
+    if stale_time_acceptable == 0:
+        message = "stale_time_acceptable == 0. Real Time data request. Querying vertica..."
+        print(message)
+        log_emmiter({"request_id": request_id, "message": message})
+        return None
+    
+    generate_key(payload, md5_key_include, md5_key_exclude, prepend_key, request_id)
+        
+    if md5_key is None:
         return None
 
     if force_reset == 1:
         message = "force_reset == 1. Querying vertica and writing to redis"
         print(message)
-        log_emmiter({'request_id': request_id, 'message': message})
+        log_emmiter({"request_id": request_id, "message": message})
         return None
     
-    ret = read_from_redis(key, request_id)
+    ret = read_from_redis(request_id)
 
     if ret is None:
         message = "Key not found in redis. Querying vertica and writing to redis."
         print(message)
-        log_emmiter({'request_id': request_id, 'message': message})
+        log_emmiter({"request_id": request_id, "message": message})
         return None
     
-    set_time = get_cache_set_time(key, request_id)
+    set_time = get_cache_set_time(request_id)
     if set_time is None:
         return None
     acceptable_time_for_key = set_time + stale_time_acceptable * 60
     if acceptable_time_for_key < time.time():
         message = "Data is older than stale_time_acceptable. Querying vertica and writing to redis."
         print(message)
-        log_emmiter({'request_id': request_id, 'message': message})
+        log_emmiter({"request_id": request_id, "message": message})
         return None
     
     message = "Data found within the stale_time_acceptable. Returning from redis."
     print(message)
-    log_emmiter({'request_id': request_id, 'message': message})
-    change_ttl(key, stale_time_acceptable, request_id)
+    log_emmiter({"request_id": request_id, "message": message})
+    change_ttl(stale_time_acceptable, request_id)
     return ret
```

### Comparing `CEEcache-1.0.1/CEEcache/logger.py` & `CEEcache-1.0.2/CEEcache/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 
 
 def overflow_handler(pendings):
     unpacker = msgpack.Unpacker(BytesIO(pendings))
     for unpacked in unpacker:
         print(unpacked)
 
-def log_emmiter(msg, typ='INFO'):
+def log_emmiter(msg, typ="INFO"):
     try:
         #eval file name to log to from typ
         log_sender = asyncsender.FluentSender(component_name, host=fluentd_host, port=fluentd_port, buffer_overflow_handler=overflow_handler)
         log_sender.emit(typ, {"message": f"{msg}"})
         log_sender.close()
     except:
         e = sys.exc_info()
         traceback_output = "".join(traceback.format_exception(e[0], e[1], e[2]))
         print("Error occured in caching logger", str(traceback_output))
 
-def logger(fn, typ='INFO'):
+def logger(fn, typ="INFO"):
     from functools import wraps
     from datetime import datetime, timezone
 
     @wraps(fn)
     def inner(*args, **kwargs):
         run_time = datetime.now()
         line_num = inspect.currentframe().f_back.f_lineno
```

### Comparing `CEEcache-1.0.1/CEEcache.egg-info/PKG-INFO` & `CEEcache-1.0.2/CEEcache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CEEcache
-Version: 1.0.1
+Version: 1.0.2
 Summary: Caching the JSON request payload and the value in RedisQ
 Home-page: UNKNOWN
 Author: Netcore Cloud
 Author-email: aditya.singh@netcorecloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `CEEcache-1.0.1/LICENCE.txt` & `CEEcache-1.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `CEEcache-1.0.1/PKG-INFO` & `CEEcache-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CEEcache
-Version: 1.0.1
+Version: 1.0.2
 Summary: Caching the JSON request payload and the value in RedisQ
 Home-page: UNKNOWN
 Author: Netcore Cloud
 Author-email: aditya.singh@netcorecloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `CEEcache-1.0.1/setup.py` & `CEEcache-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   'Operating System :: OS Independent',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='CEEcache',
-  version='1.0.1',
+  version='1.0.2',
   description='Caching the JSON request payload and the value in RedisQ',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Netcore Cloud',
   author_email='aditya.singh@netcorecloud.com',
   license='MIT', 
   classifiers=classifiers,
```

