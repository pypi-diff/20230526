# Comparing `tmp/aars-0.7.3.tar.gz` & `tmp/aars-0.7.4.tar.gz`

## Comparing `aars-0.7.3.tar` & `aars-0.7.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 aars-0.7.3/docs-requirements.txt
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 aars-0.7.3/mkdocs.yml
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 aars-0.7.3/requirements.txt
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aars-0.7.3/.github/workflows/mkdocs-gh-pages.yml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aars-0.7.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aars-0.7.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 aars-0.7.3/docs/FastAPI_Cookbook.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.3/docs/index.md -> ../README.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.7.3/docs/Code_Reference/Exceptions.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aars-0.7.3/docs/Code_Reference/utils.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aars-0.7.3/docs/Code_Reference/core/AARS.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.7.3/docs/Code_Reference/core/Index.md
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aars-0.7.3/docs/Code_Reference/core/Record.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aars-0.7.3/src/aars/__init__.py
--rw-r--r--   0        0        0    41565 2020-02-02 00:00:00.000000 aars-0.7.3/src/aars/core.py
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 aars-0.7.3/src/aars/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.3/src/aars/py.typed
--rw-r--r--   0        0        0    12374 2020-02-02 00:00:00.000000 aars-0.7.3/src/aars/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.3/tests/__init__.py
--rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 aars-0.7.3/tests/aars.py
--rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 aars-0.7.3/tests/aars_cached.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aars-0.7.3/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aars-0.7.3/LICENSE
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 aars-0.7.3/README.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aars-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 aars-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 aars-0.7.4/docs-requirements.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 aars-0.7.4/mkdocs.yml
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 aars-0.7.4/requirements.txt
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aars-0.7.4/.github/workflows/mkdocs-gh-pages.yml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aars-0.7.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aars-0.7.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 aars-0.7.4/docs/FastAPI_Cookbook.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.4/docs/index.md -> ../README.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.7.4/docs/Code_Reference/Exceptions.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aars-0.7.4/docs/Code_Reference/utils.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aars-0.7.4/docs/Code_Reference/core/AARS.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.7.4/docs/Code_Reference/core/Index.md
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aars-0.7.4/docs/Code_Reference/core/Record.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aars-0.7.4/src/aars/__init__.py
+-rw-r--r--   0        0        0    41699 2020-02-02 00:00:00.000000 aars-0.7.4/src/aars/core.py
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 aars-0.7.4/src/aars/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.4/src/aars/py.typed
+-rw-r--r--   0        0        0    12374 2020-02-02 00:00:00.000000 aars-0.7.4/src/aars/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.4/tests/__init__.py
+-rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 aars-0.7.4/tests/aars.py
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 aars-0.7.4/tests/aars_cached.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aars-0.7.4/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aars-0.7.4/LICENSE
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 aars-0.7.4/README.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aars-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 aars-0.7.4/PKG-INFO
```

### Comparing `aars-0.7.3/mkdocs.yml` & `aars-0.7.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `aars-0.7.3/.github/workflows/mkdocs-gh-pages.yml` & `aars-0.7.4/.github/workflows/mkdocs-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `aars-0.7.3/.github/workflows/publish.yml` & `aars-0.7.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aars-0.7.3/.github/workflows/python-publish.yml` & `aars-0.7.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aars-0.7.3/docs/FastAPI_Cookbook.md` & `aars-0.7.4/docs/FastAPI_Cookbook.md`

 * *Files identical despite different names*

### Comparing `aars-0.7.3/src/aars/core.py` & `aars-0.7.4/src/aars/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,18 +303,18 @@
         Initializes a record object from its raw Aleph data.
         Args:
             post: The raw Aleph data to initialize from.
         Returns:
             The initialized object.
         """
         obj = cls(**post["content"])
-        if post.get("ref") is None:
+        if post.get("original_item_hash") is None:
             obj.item_hash = ItemHash(post["item_hash"])
         else:
-            obj.item_hash = ItemHash(post["ref"])
+            obj.item_hash = ItemHash(post["original_item_hash"])
         await obj.update_revision_hashes()
         assert obj.item_hash is not None
         obj.current_revision = obj.revision_hashes.index(obj.item_hash)
         obj.timestamp = post["time"]
         obj.signer = post["sender"]
         return obj
 
@@ -882,19 +882,23 @@
 
     @classmethod
     async def _fetch_records_from_cache(
         cls, record_type: Type[R], item_hashes: List[str]
     ) -> List[R]:
         assert cls.cache, "Cache is not set"
         raw_records = await asyncio.gather(*[cls.cache.get(h) for h in item_hashes])
-        return [
-            record_type.parse_raw(r)
-            for r in raw_records
-            if r is not None and not isinstance(r, BaseException)
-        ]
+        return list(
+            reversed(
+                [
+                    record_type.parse_raw(r)
+                    for r in raw_records
+                    if r is not None and not isinstance(r, BaseException)
+                ]
+            )
+        )
 
     @classmethod
     async def _fetch_message_from_cache(
         cls, record_type: Type[R], item_hashes: List[str]
     ) -> List[R]:
         assert cls.cache, "Cache is not set"
         raw_records = await asyncio.gather(
```

### Comparing `aars-0.7.3/src/aars/exceptions.py` & `aars-0.7.4/src/aars/exceptions.py`

 * *Files identical despite different names*

### Comparing `aars-0.7.3/src/aars/utils.py` & `aars-0.7.4/src/aars/utils.py`

 * *Files identical despite different names*

### Comparing `aars-0.7.3/tests/aars.py` & `aars-0.7.4/tests/aars.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,20 @@
 def event_loop():
     yield AARS.session.http_session.loop
     asyncio.run(AARS.session.http_session.close())
 
 
 @pytest.fixture(scope="session", autouse=True)
 def create_indices(request):
-    Index(Book, "title")
-    Index(Book, ["title", "author"])
-    Index(Library, on="name")
+    try:
+        Index(Book, "title")
+        Index(Book, ["title", "author"])
+        Index(Library, on="name")
+    except ValueError:
+        pass
 
 
 class Book(Record):
     title: str
     author: str
     year: Optional[int]
```

### Comparing `aars-0.7.3/tests/aars_cached.py` & `aars-0.7.4/tests/aars_cached.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,20 @@
 def event_loop():
     yield AARS.session.http_session.loop
     asyncio.run(AARS.session.http_session.close())
 
 
 @pytest.fixture(scope="session", autouse=True)
 def create_indices(request):
-    Index(Book, "title")
-    Index(Book, ["title", "author"])
-    Index(Library, on="name")
+    try:
+        Index(Book, "title")
+        Index(Book, ["title", "author"])
+        Index(Library, on="name")
+    except ValueError:
+        pass
 
 
 @pytest.mark.asyncio
 async def test_deserialization_from_cache():
     book = await Book(title="Cached Book", author="John Doe").save()
     await asyncio.sleep(1)
     book.title = "Cached Book 2: The Recaching"
```

### Comparing `aars-0.7.3/.gitignore` & `aars-0.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `aars-0.7.3/LICENSE` & `aars-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aars-0.7.3/README.md` & `aars-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `aars-0.7.3/pyproject.toml` & `aars-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aars"
-version = "0.7.3"
+version = "0.7.4"
 authors = [
   { name="Mike Hukiewitz", email="mike.hukiewitz@robotter.ai" },
 ]
 description = "Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aars-0.7.3/PKG-INFO` & `aars-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aars
-Version: 0.7.3
+Version: 0.7.4
 Summary: Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im
 Project-URL: Homepage, https://github.com/aleph-im/active-record-sdk
 Project-URL: Bug Tracker, https://github.com/aleph-im/active-record-sdk/issues
 Author-email: Mike Hukiewitz <mike.hukiewitz@robotter.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

