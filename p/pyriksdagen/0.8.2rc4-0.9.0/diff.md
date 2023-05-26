# Comparing `tmp/pyriksdagen-0.8.2rc4.tar.gz` & `tmp/pyriksdagen-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriksdagen-0.8.2rc4.tar", max compression
+gzip compressed data, was "pyriksdagen-0.9.0.tar", max compression
```

## Comparing `pyriksdagen-0.8.2rc4.tar` & `pyriksdagen-0.9.0.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0     1249 2022-11-01 12:04:45.361073 pyriksdagen-0.8.2rc4/LICENSE
--rw-r--r--   0        0        0     3520 2023-04-13 08:26:17.120385 pyriksdagen-0.8.2rc4/README.md
--rw-r--r--   0        0        0      748 2023-05-10 13:36:26.745446 pyriksdagen-0.8.2rc4/pyproject.toml
--rw-r--r--   0        0        0     1107 2022-11-01 12:05:01.901342 pyriksdagen-0.8.2rc4/pyriksdagen/LICENSE
--rw-r--r--   0        0        0       84 2022-11-01 12:05:01.901407 pyriksdagen-0.8.2rc4/pyriksdagen/__init__.py
--rw-r--r--   0        0        0      225 2022-11-01 12:05:01.901564 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries/alias.rq
--rw-r--r--   0        0        0      494 2023-02-07 15:52:31.495339 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries/government.rq
--rw-r--r--   0        0        0      729 2023-02-07 15:52:31.495749 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries/member_of_parliament.rq
--rw-r--r--   0        0        0      148 2022-11-01 12:05:01.901748 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries/member_of_parliament.txt
--rw-r--r--   0        0        0     1380 2022-11-01 12:05:01.901837 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries/minister.rq
--rw-r--r--   0        0        0      235 2022-11-01 12:05:01.901892 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries/minister.txt
--rw-r--r--   0        0        0      262 2022-11-01 12:05:01.901962 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries/name_location_specifier.rq
--rw-r--r--   0        0        0      484 2023-02-07 15:52:31.496167 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries/party_affiliation.rq
--rw-r--r--   0        0        0      549 2023-02-07 15:52:31.496580 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries/person.rq
--rw-r--r--   0        0        0      616 2022-11-01 12:05:01.902171 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries/speaker.rq
--rw-r--r--   0        0        0      253 2022-11-01 12:05:01.902229 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries/speaker.txt
--rw-r--r--   0        0        0      208 2022-11-01 12:05:01.902286 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries/twitter.rq
--rw-r--r--   0        0        0      225 2022-11-01 12:05:01.902412 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries_backup/alias.rq
--rw-r--r--   0        0        0      482 2022-11-01 12:05:01.902473 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries_backup/government.rq
--rw-r--r--   0        0        0      722 2022-11-01 12:05:01.902539 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries_backup/member_of_parliament.rq
--rw-r--r--   0        0        0     1380 2022-11-01 12:05:01.902591 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries_backup/minister.rq
--rw-r--r--   0        0        0     1013 2022-11-01 12:05:01.902681 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries_backup/name_location_specifier.rq
--rw-r--r--   0        0        0     1230 2022-11-01 12:05:01.902743 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries_backup/party_affiliation.rq
--rw-r--r--   0        0        0     1412 2022-11-01 12:05:01.902796 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries_backup/person.rq
--rw-r--r--   0        0        0      616 2022-11-01 12:05:01.902856 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries_backup/speaker.rq
--rw-r--r--   0        0        0      959 2022-11-01 12:05:01.902940 pyriksdagen-0.8.2rc4/pyriksdagen/data/queries_backup/twitter.rq
--rw-r--r--   0        0        0     2195 2022-11-01 12:05:01.903003 pyriksdagen-0.8.2rc4/pyriksdagen/dataset.py
--rw-r--r--   0        0        0     6193 2023-02-07 15:52:31.497165 pyriksdagen-0.8.2rc4/pyriksdagen/db.py
--rw-r--r--   0        0        0     9747 2023-03-01 12:15:10.843910 pyriksdagen-0.8.2rc4/pyriksdagen/download.py
--rw-r--r--   0        0        0     6813 2023-03-01 12:15:10.844248 pyriksdagen-0.8.2rc4/pyriksdagen/export.py
--rw-r--r--   0        0        0     4532 2022-11-01 12:05:01.903384 pyriksdagen-0.8.2rc4/pyriksdagen/match_mp.py
--rw-r--r--   0        0        0     6915 2023-02-07 15:52:31.497997 pyriksdagen-0.8.2rc4/pyriksdagen/metadata.py
--rw-r--r--   0        0        0    11120 2022-11-01 12:05:01.903558 pyriksdagen-0.8.2rc4/pyriksdagen/mp.py
--rw-r--r--   0        0        0    16019 2023-05-10 13:27:42.432881 pyriksdagen-0.8.2rc4/pyriksdagen/refine.py
--rwxr-xr-x   0        0        0      237 2023-03-01 12:15:10.846196 pyriksdagen-0.8.2rc4/pyriksdagen/requirements.txt
--rw-r--r--   0        0        0     7053 2023-04-24 11:26:47.963013 pyriksdagen-0.8.2rc4/pyriksdagen/segmentation.py
--rw-r--r--   0        0        0     5497 2023-03-01 12:15:10.850360 pyriksdagen-0.8.2rc4/pyriksdagen/utils.py
--rw-r--r--   0        0        0     5265 2023-03-01 12:14:56.389831 pyriksdagen-0.8.2rc4/pyriksdagen/wikidata.py
--rw-r--r--   0        0        0     4549 2023-05-10 13:36:35.985588 pyriksdagen-0.8.2rc4/setup.py
--rw-r--r--   0        0        0     4596 2023-05-10 13:36:35.985826 pyriksdagen-0.8.2rc4/PKG-INFO
+-rw-r--r--   0        0        0     1249 2023-05-26 15:41:53.433045 pyriksdagen-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3520 2023-05-26 15:41:53.433045 pyriksdagen-0.9.0/README.md
+-rw-r--r--   0        0        0      756 2023-05-26 15:44:43.406691 pyriksdagen-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1107 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/LICENSE
+-rw-r--r--   0        0        0       84 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/__init__.py
+-rw-r--r--   0        0        0      225 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries/alias.rq
+-rw-r--r--   0        0        0      494 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries/government.rq
+-rw-r--r--   0        0        0      729 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries/member_of_parliament.rq
+-rw-r--r--   0        0        0      148 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries/member_of_parliament.txt
+-rw-r--r--   0        0        0     1380 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries/minister.rq
+-rw-r--r--   0        0        0      235 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries/minister.txt
+-rw-r--r--   0        0        0      262 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries/name_location_specifier.rq
+-rw-r--r--   0        0        0      484 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries/party_affiliation.rq
+-rw-r--r--   0        0        0      549 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries/person.rq
+-rw-r--r--   0        0        0      616 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries/speaker.rq
+-rw-r--r--   0        0        0      253 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries/speaker.txt
+-rw-r--r--   0        0        0      208 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries/twitter.rq
+-rw-r--r--   0        0        0      225 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries_backup/alias.rq
+-rw-r--r--   0        0        0      482 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries_backup/government.rq
+-rw-r--r--   0        0        0      722 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries_backup/member_of_parliament.rq
+-rw-r--r--   0        0        0     1380 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries_backup/minister.rq
+-rw-r--r--   0        0        0     1013 2023-05-26 15:42:44.877544 pyriksdagen-0.9.0/pyriksdagen/data/queries_backup/name_location_specifier.rq
+-rw-r--r--   0        0        0     1230 2023-05-26 15:42:44.881544 pyriksdagen-0.9.0/pyriksdagen/data/queries_backup/party_affiliation.rq
+-rw-r--r--   0        0        0     1412 2023-05-26 15:42:44.881544 pyriksdagen-0.9.0/pyriksdagen/data/queries_backup/person.rq
+-rw-r--r--   0        0        0      616 2023-05-26 15:42:44.881544 pyriksdagen-0.9.0/pyriksdagen/data/queries_backup/speaker.rq
+-rw-r--r--   0        0        0      959 2023-05-26 15:42:44.881544 pyriksdagen-0.9.0/pyriksdagen/data/queries_backup/twitter.rq
+-rw-r--r--   0        0        0     2195 2023-05-26 15:42:44.881544 pyriksdagen-0.9.0/pyriksdagen/dataset.py
+-rw-r--r--   0        0        0     6193 2023-05-26 15:42:44.881544 pyriksdagen-0.9.0/pyriksdagen/db.py
+-rw-r--r--   0        0        0     9747 2023-05-26 15:42:44.881544 pyriksdagen-0.9.0/pyriksdagen/download.py
+-rw-r--r--   0        0        0     6813 2023-05-26 15:42:44.881544 pyriksdagen-0.9.0/pyriksdagen/export.py
+-rw-r--r--   0        0        0     5201 2023-05-26 15:42:44.881544 pyriksdagen-0.9.0/pyriksdagen/match_mp.py
+-rw-r--r--   0        0        0     6915 2023-05-26 15:42:44.881544 pyriksdagen-0.9.0/pyriksdagen/metadata.py
+-rw-r--r--   0        0        0    11120 2023-05-26 15:42:44.881544 pyriksdagen-0.9.0/pyriksdagen/mp.py
+-rw-r--r--   0        0        0    16323 2023-05-26 15:42:44.881544 pyriksdagen-0.9.0/pyriksdagen/refine.py
+-rwxr-xr-x   0        0        0      237 2023-05-26 15:42:44.881544 pyriksdagen-0.9.0/pyriksdagen/requirements.txt
+-rw-r--r--   0        0        0     7259 2023-05-26 15:42:44.881544 pyriksdagen-0.9.0/pyriksdagen/segmentation.py
+-rw-r--r--   0        0        0     5497 2023-05-26 15:42:44.881544 pyriksdagen-0.9.0/pyriksdagen/utils.py
+-rw-r--r--   0        0        0     5265 2023-05-26 15:42:44.881544 pyriksdagen-0.9.0/pyriksdagen/wikidata.py
+-rw-r--r--   0        0        0     4664 1970-01-01 00:00:00.000000 pyriksdagen-0.9.0/PKG-INFO
```

### Comparing `pyriksdagen-0.8.2rc4/LICENSE` & `pyriksdagen-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/README.md` & `pyriksdagen-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyproject.toml` & `pyriksdagen-0.9.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyriksdagen"
-version = "0.8.2rc4"
+version = "0.9.0"
 description = "Access the Riksdagen corpus"
 authors = ["ninpnin <vainoyrjanainen@icloud.com>"]
 repository = "https://github.com/welfare-state-analytics/riksdagen-corpus"
 readme = "README.md"
 license = "MIT"
 packages = [
     { include = "pyriksdagen", from = "" }
@@ -23,14 +23,15 @@
 beautifulsoup4 = "*"
 requests = "*"
 numpy = "*"
 SPARQLWrapper = "*"
 tqdm = "*"
 matplotlib = "*"
 importlib_resources = "*"
+nltk = "*"
 
 [tool.poetry.dev-dependencies]
 devtools = "^0.5.1"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/LICENSE` & `pyriksdagen-0.9.0/pyriksdagen/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/data/queries/member_of_parliament.rq` & `pyriksdagen-0.9.0/pyriksdagen/data/queries/member_of_parliament.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/data/queries/minister.rq` & `pyriksdagen-0.9.0/pyriksdagen/data/queries/minister.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/data/queries/person.rq` & `pyriksdagen-0.9.0/pyriksdagen/data/queries/person.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/data/queries/speaker.rq` & `pyriksdagen-0.9.0/pyriksdagen/data/queries/speaker.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/data/queries_backup/member_of_parliament.rq` & `pyriksdagen-0.9.0/pyriksdagen/data/queries_backup/member_of_parliament.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/data/queries_backup/minister.rq` & `pyriksdagen-0.9.0/pyriksdagen/data/queries_backup/minister.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/data/queries_backup/name_location_specifier.rq` & `pyriksdagen-0.9.0/pyriksdagen/data/queries_backup/name_location_specifier.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/data/queries_backup/party_affiliation.rq` & `pyriksdagen-0.9.0/pyriksdagen/data/queries_backup/party_affiliation.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/data/queries_backup/person.rq` & `pyriksdagen-0.9.0/pyriksdagen/data/queries_backup/person.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/data/queries_backup/speaker.rq` & `pyriksdagen-0.9.0/pyriksdagen/data/queries_backup/speaker.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/data/queries_backup/twitter.rq` & `pyriksdagen-0.9.0/pyriksdagen/data/queries_backup/twitter.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/dataset.py` & `pyriksdagen-0.9.0/pyriksdagen/dataset.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/db.py` & `pyriksdagen-0.9.0/pyriksdagen/db.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/download.py` & `pyriksdagen-0.9.0/pyriksdagen/download.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/export.py` & `pyriksdagen-0.9.0/pyriksdagen/export.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/match_mp.py` & `pyriksdagen-0.9.0/pyriksdagen/match_mp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import pandas as pd
 import re
 from unidecode import unidecode
+from nltk.metrics.distance import edit_distance
 
 def multiple_replace(text, i_start=192, i_end=383):
 	d = [chr(c) for c in range(i_start, i_end+1)]
 	d = {c:unidecode(c) for c in d if c not in 'åäöÅÄÖ'}
 	regex = re.compile("(%s)" % "|".join(map(re.escape, d.keys())))
 	return regex.sub(lambda mo: d[mo.string[mo.start():mo.end()]], text) 
 
@@ -22,14 +23,37 @@
 		names = names.str.lower()
 	return names
 
 def name_equals(name, db):
 	matches = db[db["name"] == name]
 	return matches
 
+def name_almost_equals(name, db):
+	def _rough_equality(s1, s2):
+		perfect_matches = 0
+		s1, s2 = s1.replace(".", ""), s2.replace(".", "")
+		l1 = s1.split()
+		l2 = s2.split()
+		if len(l1) != len(l2):
+			return False
+		for w1, w2 in zip(l1, l2):
+			shorter_len = min(len(w1), len(w2))
+			w1, w2 = w1.lower(), w2.lower()
+			if w1 == w2:
+				perfect_matches += 1
+			if edit_distance(w1, w2) <= 1:
+				if w1[0] == w2[0]:
+					perfect_matches += 1
+			elif w1[:shorter_len] != w2[:shorter_len]:
+				return False
+		return perfect_matches >= 1
+
+	matches = db[db["name"].apply(lambda x: _rough_equality(name, x))]
+	return matches
+
 def names_in(name, db):
 	names = name.split()
 	matches = db[db["name"].apply(lambda x:
 		len([n for n in names if n in x.split()]) == len(names))]
 	return matches
 
 def names_in_rev(name, db):
```

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/metadata.py` & `pyriksdagen-0.9.0/pyriksdagen/metadata.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/mp.py` & `pyriksdagen-0.9.0/pyriksdagen/mp.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/refine.py` & `pyriksdagen-0.9.0/pyriksdagen/refine.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,21 @@
 
 
 def detect_mps(root, names_ids, pattern_db, mp_db=None, minister_db=None, minister_db_secondary=None, speaker_db=None, metadata=None, party_map=None, join_intros=None, protocol_id=None, unknown_variables=None):
     """
     Re-detect MPs in a parla clarin protocol, based on the (updated)
     MP database.
     """
+    scanned_protocol = False
+    try:
+        if root.findall(".//{http://www.tei-c.org/ns/1.0}pb")[0].get('facs').startswith("https://betalab.kb.se/"):
+            scanned_protocol = True
+    except:
+        pass
+
     mp_expressions = load_expressions(phase="mp")
     ids_to_join = set(join_intros['xml_id1'].tolist()+join_intros['xml_id2'].tolist())
     
     xml_ns = "{http://www.w3.org/XML/1998/namespace}"
     current_speaker = None
     prev = None
     mp_db_secondary = pd.DataFrame()
@@ -109,21 +116,21 @@
         if tag == "u":
             # Deleting and adding attributes changes their order;
             # Mark as 'delete' instead and delete later
             elem.set("prev", "delete")
             elem.set("next", "delete")
             if current_speaker is not None:
                 elem.attrib["who"] = current_speaker
-                if prev is not None:
-                    prev_id = prev.attrib[xml_ns + "id"]
-                    elem_id = elem.attrib[xml_ns + "id"]
-                    elem.set("prev", prev_id)
-                    prev.set("next", elem_id)
-
-                prev = elem
+                if prev is None:
+                    prev = elem
+                else:
+                    new_prev = prev.attrib[xml_ns + "id"]
+                    new_next = elem.attrib[xml_ns + "id"]
+                    elem.set("prev", new_prev)
+                    prev.set("next", new_next)
 
             else:
                 elem.attrib["who"] = "unknown"
                 prev = None
         elif tag == "note":
             if elem.attrib.get("type", None) == "speaker":
                 text = elem.text
@@ -150,18 +157,18 @@
                         else:
                             current_speaker = None
 
                     # Match mp if not minister/talman and a name is identified
                     # if current_speaker is None and 'name' in d:
                     elif 'name' in d:
 
-                        current_speaker = detect_mp(d, db=mp_db, party_map=party_map)
+                        current_speaker = detect_mp(d, db=mp_db, party_map=party_map, match_fuzzily=scanned_protocol)
 
                         if current_speaker is None and len(mp_db_secondary) > 0:
-                            current_speaker = detect_mp(d, db=mp_db_secondary, party_map=party_map)
+                            current_speaker = detect_mp(d, db=mp_db_secondary, party_map=party_map, match_fuzzily=scanned_protocol)
                     else:
                         current_speaker = None
 
                     if current_speaker is None:
                         unknowns.append([protocol_id, elem.attrib.get(f'{xml_ns}id')] + [d.get(key, "") for key in unknown_variables])
                     
                     prev = None
```

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/segmentation.py` & `pyriksdagen-0.9.0/pyriksdagen/segmentation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Implements the segmentation of the data into speeches and
 ultimately into the Parla-Clarin XML format.
 """
 import numpy as np
 import re, hashlib
 from .db import load_expressions
-from .match_mp import match_mp, name_equals, names_in, names_in_rev
+from .match_mp import match_mp, name_equals, name_almost_equals, names_in, names_in_rev
 from itertools import combinations
 
 # Classify paragraph
 def classify_paragraph(paragraph, classifier, prior=np.log([0.8, 0.2])):
     """
     Classify paragraph into speeches / descriptions with provided classifier
 
@@ -96,27 +96,29 @@
     elif role := re.search(r'[A-Za-zÀ-ÿ]+minister', lower_txt):
         r = role.group(0).replace('minister', '')
         role_matches = minister_db[minister_db["role"].str.contains(r, regex=False)]
         if not role_matches.empty:
             if len(set(role_matches["id"])) == 1:
                 return role_matches["id"].iloc[0]
 
-def detect_mp(intro_dict, db, party_map=None):
+def detect_mp(intro_dict, db, party_map=None, match_fuzzily=False):
     """
     Match an MP in a text snippet. Returns an MP id (str) if found, otherwise None.
 
     If multiple people are matched, defaults to returning None.
     """
 
     intro_dict["party_abbrev"] = party_map.get(intro_dict.get("party", ""), "")
     variables = ['party_abbrev', 'specifier', 'name']
     variables = [v for v in variables if v in list(db.columns)] # removes missing variables
     variables = sum([list(map(list, combinations(variables, i))) for i in range(len(variables) + 1)], [])[1:]
-    matching_funs = [name_equals, names_in]
-
+    if match_fuzzily:
+        matching_funs = [name_equals, name_almost_equals, names_in]
+    else:
+        matching_funs = [name_equals, names_in]
     return match_mp(intro_dict, db, variables, matching_funs)
 
 def intro_to_dict(intro_text, expressions=None):
     if expressions is None:
         expressions = load_expressions(phase="mp")
     intro_text = intro_text.strip()
     d = {}
@@ -142,14 +144,15 @@
         if d["gender"] in ["herr", "friherre"]:
             d["gender"] = "man"
         if d["gender"] in ["fru", "fröken"]:
             d["gender"] = "woman"
 
     if "specifier" in d:
         d["specifier"] = d["specifier"].replace("i ", "")
+        d["specifier"] = d["specifier"].replace("från ", "")
 
     return d
 
 def expression_dicts(pattern_db):
     expressions = dict()
     manual = dict()
     for _, row in pattern_db.iterrows():
```

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/utils.py` & `pyriksdagen-0.9.0/pyriksdagen/utils.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/pyriksdagen/wikidata.py` & `pyriksdagen-0.9.0/pyriksdagen/wikidata.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc4/setup.py` & `pyriksdagen-0.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,73 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyriksdagen
+Version: 0.9.0
+Summary: Access the Riksdagen corpus
+Home-page: https://github.com/welfare-state-analytics/riksdagen-corpus
+License: MIT
+Author: ninpnin
+Author-email: vainoyrjanainen@icloud.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: SPARQLWrapper
+Requires-Dist: base58
+Requires-Dist: beautifulsoup4
+Requires-Dist: dateparser
+Requires-Dist: importlib_resources
+Requires-Dist: kblab-client
+Requires-Dist: lxml
+Requires-Dist: matplotlib
+Requires-Dist: nltk
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: progressbar2
+Requires-Dist: pyparlaclarin
+Requires-Dist: requests
+Requires-Dist: tqdm
+Requires-Dist: unidecode
+Project-URL: Repository, https://github.com/welfare-state-analytics/riksdagen-corpus
+Description-Content-Type: text/markdown
+
+[![Check unchanged](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/check_unchanged.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/check_unchanged.yml)
+[![Unit tests](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/push.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/push.yml)
+[![Validate Parla-Clarin XML](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/validate.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/validate.yml)
+
+# Swedish parliamentary proceedings - Riksdagens protokoll 1867-today
+
+_Westac Project, 2020-2023_
+
+The full data set consists of multiple parts:
+
+- Riksdagens protokoll between from 1867 until today in the [Parla-clarin](https://github.com/clarin-eric/parla-clarin) format
+- Comprehensive list of MPs and cabinet members during this period
+- [Documentation](https://github.com/welfare-state-analytics/riksdagen-corpus/wiki/) of the corpus and the curation process
+- [A Google Colab notebook](https://colab.research.google.com/drive/1C3e2gwi9z83ikXbYXNPfB6RF7spTgzxA?usp=sharing) that demonstrates how the dataset can be used with Python
+
+## Basic use
+
+A full dataset is available under [this download link](https://github.com/welfare-state-analytics/riksdagen-corpus/releases/latest/download/corpus.zip). It has the following structure
+
+- Annual protocol files in the ```corpus/protocols/``` folder
+- Structured metadata on MPs, speakers, ministers, and governments in the ```corpus/metadata/``` folder
+
+The workflow to use the data is demonstrated in [this Google Colab notebook](https://colab.research.google.com/drive/1C3e2gwi9z83ikXbYXNPfB6RF7spTgzxA?usp=sharing).
+
+## Design choices of the project
+
+The Riksdagen corpus is released as an iterative process, where the corpus is curated and expanded. Semantic versioning is used for the whole corpus, following the established major-minor-patch practices as they apply to data. For each major and minor release, a statistical sample is drawn, annotated and quantitatively evaluated. Errors are fixed as they are detected in order of priority. Moreover, the edit history is kept as a traceable git repository.
+
+![Estimate of mapping accuracy](https://raw.githubusercontent.com/welfare-state-analytics/riksdagen-corpus/main/input/accuracy/version_plot.png)
 
-package_dir = \
-{'': '.'}
+While the contents of the corpus will change due to curation and expansion, we aim to keep the deliverable API, the corpus/ folder, as stable as possible. This means we avoid relocating files or folders, changing formats, changing columns in metadata files, or any other changes that might break downstream scripts. Conversely, files outside the corpus/ folder are internal to the project. End users may find utility in them but we make no effort to keep them consistent.
 
-packages = \
-['pyriksdagen']
+The data in the corpus is delivered as TEI XML files to follow established practices. The metadata is delivered as CSV files, following a normal form database structure while allowing for a legible git history. A more detailed description of the data and metadata structure and formats can be found in the README files in the corpus/ folder.
 
-package_data = \
-{'': ['*'], 'pyriksdagen': ['data/queries/*', 'data/queries_backup/*']}
-
-install_requires = \
-['SPARQLWrapper',
- 'base58',
- 'beautifulsoup4',
- 'dateparser',
- 'importlib_resources',
- 'kblab-client',
- 'lxml',
- 'matplotlib',
- 'numpy',
- 'pandas',
- 'progressbar2',
- 'pyparlaclarin',
- 'requests',
- 'tqdm',
- 'unidecode']
-
-setup_kwargs = {
-    'name': 'pyriksdagen',
-    'version': '0.8.2rc4',
-    'description': 'Access the Riksdagen corpus',
-    'long_description': '[![Check unchanged](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/check_unchanged.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/check_unchanged.yml)\n[![Unit tests](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/push.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/push.yml)\n[![Validate Parla-Clarin XML](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/validate.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/validate.yml)\n\n# Swedish parliamentary proceedings - Riksdagens protokoll 1867-today\n\n_Westac Project, 2020-2023_\n\nThe full data set consists of multiple parts:\n\n- Riksdagens protokoll between from 1867 until today in the [Parla-clarin](https://github.com/clarin-eric/parla-clarin) format\n- Comprehensive list of MPs and cabinet members during this period\n- [Documentation](https://github.com/welfare-state-analytics/riksdagen-corpus/wiki/) of the corpus and the curation process\n- [A Google Colab notebook](https://colab.research.google.com/drive/1C3e2gwi9z83ikXbYXNPfB6RF7spTgzxA?usp=sharing) that demonstrates how the dataset can be used with Python\n\n## Basic use\n\nA full dataset is available under [this download link](https://github.com/welfare-state-analytics/riksdagen-corpus/releases/latest/download/corpus.zip). It has the following structure\n\n- Annual protocol files in the ```corpus/protocols/``` folder\n- Structured metadata on MPs, speakers, ministers, and governments in the ```corpus/metadata/``` folder\n\nThe workflow to use the data is demonstrated in [this Google Colab notebook](https://colab.research.google.com/drive/1C3e2gwi9z83ikXbYXNPfB6RF7spTgzxA?usp=sharing).\n\n## Design choices of the project\n\nThe Riksdagen corpus is released as an iterative process, where the corpus is curated and expanded. Semantic versioning is used for the whole corpus, following the established major-minor-patch practices as they apply to data. For each major and minor release, a statistical sample is drawn, annotated and quantitatively evaluated. Errors are fixed as they are detected in order of priority. Moreover, the edit history is kept as a traceable git repository.\n\n![Estimate of mapping accuracy](https://raw.githubusercontent.com/welfare-state-analytics/riksdagen-corpus/main/input/accuracy/version_plot.png)\n\nWhile the contents of the corpus will change due to curation and expansion, we aim to keep the deliverable API, the corpus/ folder, as stable as possible. This means we avoid relocating files or folders, changing formats, changing columns in metadata files, or any other changes that might break downstream scripts. Conversely, files outside the corpus/ folder are internal to the project. End users may find utility in them but we make no effort to keep them consistent.\n\nThe data in the corpus is delivered as TEI XML files to follow established practices. The metadata is delivered as CSV files, following a normal form database structure while allowing for a legible git history. A more detailed description of the data and metadata structure and formats can be found in the README files in the corpus/ folder.\n\n## Participate in the curation process\n\nIf you find any errors, it is possible to submit corrections to them. This is documented in the [project wiki](https://github.com/welfare-state-analytics/riksdagen-corpus/wiki/Submit-corrections).\n',
-    'author': 'ninpnin',
-    'author_email': 'vainoyrjanainen@icloud.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/welfare-state-analytics/riksdagen-corpus',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+## Participate in the curation process
 
+If you find any errors, it is possible to submit corrections to them. This is documented in the [project wiki](https://github.com/welfare-state-analytics/riksdagen-corpus/wiki/Submit-corrections).
 
-setup(**setup_kwargs)
```

