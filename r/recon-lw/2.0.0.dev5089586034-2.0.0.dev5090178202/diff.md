# Comparing `tmp/recon_lw-2.0.0.dev5089586034.tar.gz` & `tmp/recon_lw-2.0.0.dev5090178202.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5089586034.tar", last modified: Fri May 26 10:02:06 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5090178202.tar", last modified: Fri May 26 11:13:05 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5089586034.tar` & `recon_lw-2.0.0.dev5090178202.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 10:02:06.000000 recon_lw-2.0.0.dev5089586034/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-26 10:01:18.000000 recon_lw-2.0.0.dev5089586034/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-26 10:02:06.000000 recon_lw-2.0.0.dev5089586034/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-26 10:01:18.000000 recon_lw-2.0.0.dev5089586034/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-26 10:01:44.000000 recon_lw-2.0.0.dev5089586034/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 10:02:06.000000 recon_lw-2.0.0.dev5089586034/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-26 10:01:18.000000 recon_lw-2.0.0.dev5089586034/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-26 10:01:18.000000 recon_lw-2.0.0.dev5089586034/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-05-26 10:01:18.000000 recon_lw-2.0.0.dev5089586034/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-26 10:01:18.000000 recon_lw-2.0.0.dev5089586034/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-26 10:01:18.000000 recon_lw-2.0.0.dev5089586034/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    28839 2023-05-26 10:01:18.000000 recon_lw-2.0.0.dev5089586034/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-26 10:01:18.000000 recon_lw-2.0.0.dev5089586034/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 10:02:06.000000 recon_lw-2.0.0.dev5089586034/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-26 10:02:06.000000 recon_lw-2.0.0.dev5089586034/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-26 10:02:06.000000 recon_lw-2.0.0.dev5089586034/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-26 10:02:06.000000 recon_lw-2.0.0.dev5089586034/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-26 10:02:06.000000 recon_lw-2.0.0.dev5089586034/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-26 10:02:06.000000 recon_lw-2.0.0.dev5089586034/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-26 10:01:18.000000 recon_lw-2.0.0.dev5089586034/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-26 10:02:06.000000 recon_lw-2.0.0.dev5089586034/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-26 10:01:18.000000 recon_lw-2.0.0.dev5089586034/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 10:02:06.000000 recon_lw-2.0.0.dev5089586034/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-26 10:01:18.000000 recon_lw-2.0.0.dev5089586034/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-26 11:12:39.000000 recon_lw-2.0.0.dev5090178202/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29010 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15455 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 11:13:05.000000 recon_lw-2.0.0.dev5090178202/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-26 11:12:03.000000 recon_lw-2.0.0.dev5090178202/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5089586034/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5090178202/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5089586034/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5090178202/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5089586034/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5090178202/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5089586034/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5090178202/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5089586034/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5090178202/recon_lw/recon_ob.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,29 +153,33 @@
     for tupl in operations_batch:
         dbg_event["attachedMessageIds"].append(tupl[2]["messageId"])
     events.append(dbg_event)
 
     if len(obs) > 1 and aggregate_batch_updates:
         top_not_affected = all(ob["aggr_seq"]["top_delta"] == 0 for ob in obs)
         limit_not_affected = all(ob["aggr_seq"]["limit_delta"] == 0 for ob in obs)
-        skip_top = 0
+        updated_v2 = 0
         for i in range(len(obs) - 1):
             if obs[i]["operation"] in ["ob_change_status", "ob_clean_book", "ob_aggr_clean_book", "ob_top_clean_book"]:
+                obs[i]["aggr_seq"]["top_v2"] = updated_v2
+                obs[i]["aggr_seq"]["limit_v2"] = updated_v2
+                updated_v2 += 1
                 continue
+
             obs[i]["aggr_seq"]["top_delta"] = 0
             obs[i]["aggr_seq"]["top_v"] = -1
             obs[i]["aggr_seq"]["top_v2"] = -1
             obs[i]["aggr_seq"]["limit_delta"] = 0
             obs[i]["aggr_seq"]["limit_v"] = -1
             obs[i]["aggr_seq"]["limit_v2"] = -1
 
         obs[-1]["aggr_seq"]["top_delta"] = 0 if top_not_affected else 1
-        obs[-1]["aggr_seq"]["top_v2"] = 0
+        obs[-1]["aggr_seq"]["top_v2"] = updated_v2
         obs[-1]["aggr_seq"]["limit_delta"] = 0 if limit_not_affected else 1
-        obs[-1]["aggr_seq"]["limit_v2"] = 0
+        obs[-1]["aggr_seq"]["limit_v2"] = updated_v2
 
 
 def process_market_data_update(mess_batch, events,  books_cache, get_book_id_func ,update_book_rule,
                                check_book_rule, event_sequence, parent_event, initial_book_params, log_books_filter,
                                log_books_collection, aggregate_batch_updates):
     books_updates = {}
     for m in mess_batch:
```

### Comparing `recon_lw-2.0.0.dev5089586034/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5090178202/recon_lw/recon_ob_cross_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,16 +142,16 @@
                                     "book_id": match[0]["body"]["book_id"],
                                     "time_of_event": match[0]["body"]["time_of_event"],
                                     "limit_v2": match[0]["body"]["aggr_seq"]["limit_v2"],
                                     "sessionId": match[0]["body"]["sessionId"],
                                     "tech_info": tech_info})
         save_events([error_event])
     elif match[1] is not None:
-        error_event = create_event("StreamMismatchNoFull",
-                                   "StreamMismatchNoFull",
+        error_event = create_event("StreamMismatchNoFullvsAggr",
+                                   "StreamMismatchNoFullvsAggr",
                                    False,
                                    {"aggr_book_event": match[1]["eventId"],
                                     "book_id": match[1]["body"]["book_id"],
                                     "time_of_event": match[1]["body"]["time_of_event"],
                                    "limit_v2": match[1]["body"]["aggr_seq"]["limit_v2"],
                                     "sessionId": match[1]["body"]["sessionId"]})
         save_events([error_event])
@@ -178,16 +178,16 @@
                                    {"full_book_event": match[0]["eventId"],
                                     "book_id": match[0]["body"]["book_id"],
                                     "time_of_event": match[0]["body"]["time_of_event"],
                                     "top_v2": match[0]["body"]["aggr_seq"]["top_v2"],
                                     "sessionId": match[0]["body"]["sessionId"]})
         save_events([error_event])
     elif match[1] is not None:
-        error_event = create_event("StreamMismatchNoFull",
-                                   "StreamMismatchNoFull",
+        error_event = create_event("StreamMismatchNoFullvsTop",
+                                   "StreamMismatchNoFullvsTop",
                                    False,
                                    {"top_book_event": match[1]["eventId"],
                                     "book_id": match[1]["body"]["book_id"],
                                     "time_of_event": match[1]["body"]["time_of_event"],
                                     "top_v2": match[1]["body"]["aggr_seq"]["top_v2"],
                                     "sessionId": match[1]["body"]["sessionId"]})
         save_events([error_event])
```

### Comparing `recon_lw-2.0.0.dev5089586034/setup.py` & `recon_lw-2.0.0.dev5090178202/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5089586034/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5090178202/test/test_recon_ob.py`

 * *Files identical despite different names*

