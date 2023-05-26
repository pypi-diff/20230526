# Comparing `tmp/event2vec-0.0.31.tar.gz` & `tmp/event2vec-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event2vec-0.0.31.tar", max compression
+gzip compressed data, was "event2vec-0.0.32.tar", max compression
```

## Comparing `event2vec-0.0.31.tar` & `event2vec-0.0.32.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    15731 2023-03-14 22:29:01.448203 event2vec-0.0.31/LICENSE
--rw-r--r--   0        0        0      762 2023-03-14 22:29:01.448203 event2vec-0.0.31/README.md
--rw-r--r--   0        0        0      242 2023-03-14 22:29:01.448203 event2vec-0.0.31/bin/config.cfg
--rw-r--r--   0        0        0     5993 2023-04-21 19:43:26.765843 event2vec-0.0.31/bin/submit_i2b2.py
--rw-r--r--   0        0        0     5384 2023-04-21 19:43:24.325844 event2vec-0.0.31/bin/submit_omop.py
--rw-r--r--   0        0        0       17 2023-03-14 22:29:01.778203 event2vec-0.0.31/event2vec/__init__.py
--rw-r--r--   0        0        0     1148 2023-03-14 22:29:01.778203 event2vec-0.0.31/event2vec/concept_proximity.py
--rw-r--r--   0        0        0     1411 2023-05-25 16:23:01.245183 event2vec-0.0.31/event2vec/config.py
--rw-r--r--   0        0        0     3999 2023-04-21 19:54:05.145765 event2vec-0.0.31/event2vec/cooccurrence_matrix_pandas.py
--rw-r--r--   0        0        0     7099 2023-04-22 02:17:00.822933 event2vec-0.0.31/event2vec/cooccurrence_matrix_spark.py
--rw-r--r--   0        0        0     1818 2023-05-25 19:08:52.021601 event2vec-0.0.31/event2vec/datasets.py
--rw-r--r--   0        0        0    20171 2023-05-25 20:05:43.830384 event2vec-0.0.31/event2vec/event_transformer.py
--rw-r--r--   0        0        0     6425 2023-03-14 22:29:01.778203 event2vec-0.0.31/event2vec/nomenclatures.py
--rw-r--r--   0        0        0     6867 2023-05-25 20:21:37.250039 event2vec-0.0.31/event2vec/svd_ppmi.py
--rw-r--r--   0        0        0     2040 2023-05-25 20:07:29.250350 event2vec-0.0.31/event2vec/utils.py
--rw-r--r--   0        0        0     4603 2023-05-25 20:51:34.289397 event2vec-0.0.31/pyproject.toml
--rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 event2vec-0.0.31/PKG-INFO
+-rw-r--r--   0        0        0    15731 2023-03-14 22:29:01.448203 event2vec-0.0.32/LICENSE
+-rw-r--r--   0        0        0      762 2023-03-14 22:29:01.448203 event2vec-0.0.32/README.md
+-rw-r--r--   0        0        0      242 2023-03-14 22:29:01.448203 event2vec-0.0.32/bin/config.cfg
+-rw-r--r--   0        0        0     5993 2023-04-21 19:43:26.765843 event2vec-0.0.32/bin/submit_i2b2.py
+-rw-r--r--   0        0        0     5384 2023-04-21 19:43:24.325844 event2vec-0.0.32/bin/submit_omop.py
+-rw-r--r--   0        0        0       17 2023-03-14 22:29:01.778203 event2vec-0.0.32/event2vec/__init__.py
+-rw-r--r--   0        0        0     1148 2023-03-14 22:29:01.778203 event2vec-0.0.32/event2vec/concept_proximity.py
+-rw-r--r--   0        0        0     1411 2023-05-25 16:23:01.245183 event2vec-0.0.32/event2vec/config.py
+-rw-r--r--   0        0        0     3999 2023-04-21 19:54:05.145765 event2vec-0.0.32/event2vec/cooccurrence_matrix_pandas.py
+-rw-r--r--   0        0        0     7099 2023-04-22 02:17:00.822933 event2vec-0.0.32/event2vec/cooccurrence_matrix_spark.py
+-rw-r--r--   0        0        0     1818 2023-05-25 19:08:52.021601 event2vec-0.0.32/event2vec/datasets.py
+-rw-r--r--   0        0        0    20149 2023-05-26 19:09:13.964381 event2vec-0.0.32/event2vec/event_transformer.py
+-rw-r--r--   0        0        0     6425 2023-03-14 22:29:01.778203 event2vec-0.0.32/event2vec/nomenclatures.py
+-rw-r--r--   0        0        0     6867 2023-05-25 20:21:37.250039 event2vec-0.0.32/event2vec/svd_ppmi.py
+-rw-r--r--   0        0        0     2040 2023-05-25 20:07:29.250350 event2vec-0.0.32/event2vec/utils.py
+-rw-r--r--   0        0        0     4603 2023-05-26 19:14:04.514315 event2vec-0.0.32/pyproject.toml
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 event2vec-0.0.32/PKG-INFO
```

### Comparing `event2vec-0.0.31/LICENSE` & `event2vec-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.31/README.md` & `event2vec-0.0.32/README.md`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.31/bin/submit_i2b2.py` & `event2vec-0.0.32/bin/submit_i2b2.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.31/bin/submit_omop.py` & `event2vec-0.0.32/bin/submit_omop.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.31/event2vec/concept_proximity.py` & `event2vec-0.0.32/event2vec/concept_proximity.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.31/event2vec/config.py` & `event2vec-0.0.32/event2vec/config.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.31/event2vec/cooccurrence_matrix_pandas.py` & `event2vec-0.0.32/event2vec/cooccurrence_matrix_pandas.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.31/event2vec/cooccurrence_matrix_spark.py` & `event2vec-0.0.32/event2vec/cooccurrence_matrix_spark.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.31/event2vec/datasets.py` & `event2vec-0.0.32/event2vec/datasets.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.31/event2vec/event_transformer.py` & `event2vec-0.0.32/event2vec/event_transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -379,15 +379,15 @@
         event,
         on=COLNAME_PERSON,
         how="inner",
     )
     event["delta_to_followup"] = (
         pd.to_datetime(event[COLNAME_FOLLOWUP_START])
         - pd.to_datetime(event[COLNAME_START])
-    ).astype("timedelta64[D]")
+    ).dt.total_seconds() / (24 * 3600)
     for half_life in decay_half_life_in_days:
         if half_life < 0:
             raise ValueError(f"half_life should be positive, got {half_life}")
         # not necessary to set as a variable
         if half_life > 0:
             event[COLNAME_VALUE] = np.exp(
                 -event["delta_to_followup"] / half_life
@@ -516,53 +516,53 @@
     events_of_interest = event_restricted.merge(
         first_event_datetime, on=aggregation_col, how="inner"
     ).merge(last_event_datetime, on=aggregation_col, how="inner")
 
     events_of_interest["observation_delta"] = (
         events_of_interest[OBSERVATION_END]
         - events_of_interest[OBSERVATION_START]
-    ).astype("timedelta64[s]")
+    ).dt.total_seconds()
     X = []
     for sub_period in periods:
         logger.info(f"Computing period {sub_period}")
         events_of_interest["period_span_second"] = (
             events_of_interest["observation_delta"] * sub_period / 100
         )
         if sub_period >= 0:
             mask = (
                 (
                     pd.to_datetime(events_of_interest[COLNAME_START])
                     - pd.to_datetime(events_of_interest[OBSERVATION_START])
-                ).astype("timedelta64[s]")
+                ).dt.total_seconds()
                 >= -eps
             ) & (
                 (
                     pd.to_datetime(events_of_interest[COLNAME_START])
                     - pd.to_datetime(events_of_interest[OBSERVATION_START])
-                ).astype("timedelta64[s]")
+                ).dt.total_seconds()
                 <= (events_of_interest["period_span_second"] + eps)
             )
         else:
             mask = (
                 (
                     pd.to_datetime(events_of_interest[COLNAME_START])
                     - pd.to_datetime(events_of_interest[OBSERVATION_START])
-                ).astype("timedelta64[s]")
+                ).dt.total_seconds()
                 >= (
                     (
                         events_of_interest["observation_delta"]
                         + events_of_interest["period_span_second"]
                     )
                     - eps
                 )
             ) & (
                 (
                     pd.to_datetime(events_of_interest[COLNAME_START])
                     - pd.to_datetime(events_of_interest[OBSERVATION_END])
-                ).astype("timedelta64[s]")
+                ).dt.total_seconds()
                 <= eps + events_of_interest["observation_delta"]
             )
         period_events = events_of_interest.loc[mask, :]
         period_events = pd.concat((period_events, fake_lines), axis=0)
         period_statistics = (
             period_events.groupby(by=[aggregation_col, COLNAME_SOURCE_CODE])
             .agg(**statistics_dict)
```

### Comparing `event2vec-0.0.31/event2vec/nomenclatures.py` & `event2vec-0.0.32/event2vec/nomenclatures.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.31/event2vec/svd_ppmi.py` & `event2vec-0.0.32/event2vec/svd_ppmi.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.31/event2vec/utils.py` & `event2vec-0.0.32/event2vec/utils.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.31/pyproject.toml` & `event2vec-0.0.32/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "event2vec"
-version = "0.0.31"
+version = "0.0.32"
 description = "event2vec"
 authors = ["Matthieu Doutreligne <matt.dout@gmail.com>"]
 license = "EUPL-v1.2"
 readme = "README.md"
 repository = "https://gitlab.com/strayMat/event2vec"
 homepage = "https://gitlab.com/strayMat/event2vec"
 include = ["bin"]
```

### Comparing `event2vec-0.0.31/PKG-INFO` & `event2vec-0.0.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event2vec
-Version: 0.0.31
+Version: 0.0.32
 Summary: event2vec
 Home-page: https://gitlab.com/strayMat/event2vec
 License: EUPL-v1.2
 Author: Matthieu Doutreligne
 Author-email: matt.dout@gmail.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: Intended Audience :: Developers
```

