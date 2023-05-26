# Comparing `tmp/openapi3-1.7.0.tar.gz` & `tmp/openapi3-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi3-1.7.0.tar", last modified: Thu Nov 10 05:06:53 2022, max compression
+gzip compressed data, was "dist/openapi3-1.8.0.tar", last modified: Fri May 26 17:44:28 2023, max compression
```

## Comparing `openapi3-1.7.0.tar` & `openapi3-1.8.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 dorthu    (1000) dorthu    (1000)        0 2022-11-10 05:06:53.645574 openapi3-1.7.0/
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)     1484 2022-10-14 02:41:08.000000 openapi3-1.7.0/LICENSE
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)     3633 2022-11-10 05:06:53.645574 openapi3-1.7.0/PKG-INFO
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)     2707 2022-10-14 02:41:08.000000 openapi3-1.7.0/README.rst
-drwxrwxr-x   0 dorthu    (1000) dorthu    (1000)        0 2022-11-10 05:06:53.645574 openapi3-1.7.0/openapi3/
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)      437 2022-10-14 02:41:08.000000 openapi3-1.7.0/openapi3/__init__.py
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)      541 2022-10-14 02:41:08.000000 openapi3-1.7.0/openapi3/__main__.py
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)     1426 2022-10-14 02:41:08.000000 openapi3-1.7.0/openapi3/components.py
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)     1818 2022-10-14 02:41:08.000000 openapi3-1.7.0/openapi3/errors.py
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)      672 2022-10-14 02:41:08.000000 openapi3-1.7.0/openapi3/example.py
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)     1368 2022-11-10 05:05:18.000000 openapi3-1.7.0/openapi3/general.py
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)     1803 2022-10-14 03:25:53.000000 openapi3-1.7.0/openapi3/info.py
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)    24915 2022-10-14 02:41:08.000000 openapi3-1.7.0/openapi3/object_base.py
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)     9121 2022-11-10 05:05:18.000000 openapi3-1.7.0/openapi3/openapi.py
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)    19211 2022-10-14 03:25:53.000000 openapi3-1.7.0/openapi3/paths.py
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)    11075 2022-11-10 05:05:18.000000 openapi3-1.7.0/openapi3/schemas.py
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)     1026 2022-10-14 02:41:08.000000 openapi3-1.7.0/openapi3/security.py
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)     1169 2022-10-14 02:41:08.000000 openapi3-1.7.0/openapi3/servers.py
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)      610 2022-11-10 05:05:18.000000 openapi3-1.7.0/openapi3/tag.py
-drwxrwxr-x   0 dorthu    (1000) dorthu    (1000)        0 2022-11-10 05:06:53.645574 openapi3-1.7.0/openapi3.egg-info/
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)     3633 2022-11-10 05:06:53.000000 openapi3-1.7.0/openapi3.egg-info/PKG-INFO
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)      466 2022-11-10 05:06:53.000000 openapi3-1.7.0/openapi3.egg-info/SOURCES.txt
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)        1 2022-11-10 05:06:53.000000 openapi3-1.7.0/openapi3.egg-info/dependency_links.txt
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)      118 2022-11-10 05:06:53.000000 openapi3-1.7.0/openapi3.egg-info/requires.txt
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)        9 2022-11-10 05:06:53.000000 openapi3-1.7.0/openapi3.egg-info/top_level.txt
--rw-rw-r--   0 dorthu    (1000) dorthu    (1000)       38 2022-11-10 05:06:53.645574 openapi3-1.7.0/setup.cfg
--rwxrwxr-x   0 dorthu    (1000) dorthu    (1000)      777 2022-11-10 05:05:26.000000 openapi3-1.7.0/setup.py
+drwxr-xr-x   0 wsmith     (501) staff       (20)        0 2023-05-26 17:44:28.102370 openapi3-1.8.0/
+-rw-r--r--   0 wsmith     (501) staff       (20)     1484 2020-12-11 20:20:15.000000 openapi3-1.8.0/LICENSE
+-rw-r--r--   0 wsmith     (501) staff       (20)     3633 2023-05-26 17:44:28.102080 openapi3-1.8.0/PKG-INFO
+-rw-r--r--   0 wsmith     (501) staff       (20)     2707 2023-05-25 12:30:25.000000 openapi3-1.8.0/README.rst
+drwxr-xr-x   0 wsmith     (501) staff       (20)        0 2023-05-26 17:44:28.099468 openapi3-1.8.0/openapi3/
+-rw-r--r--   0 wsmith     (501) staff       (20)      437 2022-03-09 16:00:00.000000 openapi3-1.8.0/openapi3/__init__.py
+-rw-r--r--   0 wsmith     (501) staff       (20)      541 2022-01-10 18:30:07.000000 openapi3-1.8.0/openapi3/__main__.py
+-rw-r--r--   0 wsmith     (501) staff       (20)     1531 2023-05-26 17:39:29.000000 openapi3-1.8.0/openapi3/components.py
+-rw-r--r--   0 wsmith     (501) staff       (20)     1818 2022-03-09 16:00:00.000000 openapi3-1.8.0/openapi3/errors.py
+-rw-r--r--   0 wsmith     (501) staff       (20)      672 2022-03-08 20:37:40.000000 openapi3-1.8.0/openapi3/example.py
+-rw-r--r--   0 wsmith     (501) staff       (20)     1718 2023-05-26 17:39:29.000000 openapi3-1.8.0/openapi3/general.py
+-rw-r--r--   0 wsmith     (501) staff       (20)     1803 2023-03-17 12:43:51.000000 openapi3-1.8.0/openapi3/info.py
+-rw-r--r--   0 wsmith     (501) staff       (20)    27370 2023-05-26 17:39:29.000000 openapi3-1.8.0/openapi3/object_base.py
+-rw-r--r--   0 wsmith     (501) staff       (20)     9324 2023-05-26 17:39:29.000000 openapi3-1.8.0/openapi3/openapi.py
+-rw-r--r--   0 wsmith     (501) staff       (20)    19211 2023-03-17 12:43:51.000000 openapi3-1.8.0/openapi3/paths.py
+-rw-r--r--   0 wsmith     (501) staff       (20)    11096 2023-05-26 17:39:29.000000 openapi3-1.8.0/openapi3/schemas.py
+-rw-r--r--   0 wsmith     (501) staff       (20)     1026 2022-01-10 18:30:07.000000 openapi3-1.8.0/openapi3/security.py
+-rw-r--r--   0 wsmith     (501) staff       (20)     1169 2022-01-10 18:30:07.000000 openapi3-1.8.0/openapi3/servers.py
+-rw-r--r--   0 wsmith     (501) staff       (20)      610 2023-03-17 12:43:51.000000 openapi3-1.8.0/openapi3/tag.py
+drwxr-xr-x   0 wsmith     (501) staff       (20)        0 2023-05-26 17:44:28.101615 openapi3-1.8.0/openapi3.egg-info/
+-rw-r--r--   0 wsmith     (501) staff       (20)     3633 2023-05-26 17:44:27.000000 openapi3-1.8.0/openapi3.egg-info/PKG-INFO
+-rw-r--r--   0 wsmith     (501) staff       (20)      466 2023-05-26 17:44:27.000000 openapi3-1.8.0/openapi3.egg-info/SOURCES.txt
+-rw-r--r--   0 wsmith     (501) staff       (20)        1 2023-05-26 17:44:27.000000 openapi3-1.8.0/openapi3.egg-info/dependency_links.txt
+-rw-r--r--   0 wsmith     (501) staff       (20)      118 2023-05-26 17:44:27.000000 openapi3-1.8.0/openapi3.egg-info/requires.txt
+-rw-r--r--   0 wsmith     (501) staff       (20)        9 2023-05-26 17:44:27.000000 openapi3-1.8.0/openapi3.egg-info/top_level.txt
+-rw-r--r--   0 wsmith     (501) staff       (20)       38 2023-05-26 17:44:28.102473 openapi3-1.8.0/setup.cfg
+-rwxr-xr-x   0 wsmith     (501) staff       (20)      777 2023-05-26 17:41:20.000000 openapi3-1.8.0/setup.py
```

### Comparing `openapi3-1.7.0/LICENSE` & `openapi3-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi3-1.7.0/PKG-INFO` & `openapi3-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi3
-Version: 1.7.0
+Version: 1.8.0
 Summary: Client and Validator of OpenAPI 3 Specifications
 Home-page: https://github.com/dorthu/openapi3
 Author: dorthu
 License: BSD 3-Clause License
 Description: openapi3
         ========
         
@@ -45,15 +45,15 @@
         
            # authenticate using a securityScheme defined in the spec's components.securitySchemes
            api.authenticate('personalAccessToken', my_token)
         
            # call an operation that requires authentication
            linodes  = api.call_getLinodeInstances()
         
-           # call an opertaion with parameters
+           # call an operation with parameters
            linode = api.call_getLinodeInstance(parameters={"linodeId": 123})
         
            # the models returns are all of the same (generated) type
            print(type(linode))                      # openapi.schemas.Linode
            type(linode) == type(linodes.data[0])    # True
         
            # call an operation with a request body
```

### Comparing `openapi3-1.7.0/README.rst` & `openapi3-1.8.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
    # authenticate using a securityScheme defined in the spec's components.securitySchemes
    api.authenticate('personalAccessToken', my_token)
 
    # call an operation that requires authentication
    linodes  = api.call_getLinodeInstances()
 
-   # call an opertaion with parameters
+   # call an operation with parameters
    linode = api.call_getLinodeInstance(parameters={"linodeId": 123})
 
    # the models returns are all of the same (generated) type
    print(type(linode))                      # openapi.schemas.Linode
    type(linode) == type(linodes.data[0])    # True
 
    # call an operation with a request body
```

### Comparing `openapi3-1.7.0/openapi3/__main__.py` & `openapi3-1.8.0/openapi3/__main__.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.7.0/openapi3/components.py` & `openapi3-1.8.0/openapi3/components.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         "schemas",
         "responses",
         "parameters",
         "examples",
         "headers",
         "requestBodies",
         "securitySchemes",
+        "pathItems",
         "links",
         "callback",
     ]
 
     def _parse_data(self):
         """
         Implementation of :any:`ObjectBase._parse_data`
@@ -28,9 +29,10 @@
         self.examples = self._get("examples", ["Example", "Reference"], is_map=True)
         self.parameters = self._get("parameters", ["Parameter", "Reference"], is_map=True)
         self.requestBodies = self._get("requestBody", ["RequestBody", "Reference"], is_map=True)
         self.responses = self._get("responses", ["Response", "Reference"], is_map=True)
         self.schemas = self._get("schemas", ["Schema", "Reference"], is_map=True)
         self.securitySchemes = self._get("securitySchemes", ["SecurityScheme", "Reference"], is_map=True)
         # self.headers       = self._get('headers', ['Header', 'Reference'], is_map=True)
+        self.pathItems = self._get("pathItems", ['Path', 'Reference'], is_map=True)
         self.links = self._get("links", ["Link", "Reference"], is_map=True)
         # self.callbacks     = self._get('callbacks', ['Callback', 'Reference'], is_map=True)
```

### Comparing `openapi3-1.7.0/openapi3/errors.py` & `openapi3-1.8.0/openapi3/errors.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.7.0/openapi3/example.py` & `openapi3-1.8.0/openapi3/example.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.7.0/openapi3/general.py` & `openapi3-1.8.0/openapi3/general.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,23 +21,28 @@
     """
     A `Reference Object`_ designates a reference to another node in the specification.
 
     .. _Reference Object: https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.1.md#referenceObject
     """
 
     # can't start a variable name with a $
-    __slots__ = ["ref"]
+    __slots__ = ["ref", "summary", "description"]
     required_fields = ["$ref"]
 
     def _parse_data(self):
         self.ref = self._get("$ref", str)
+        self.summary = self._get("summary", str)
+        self.description = self._get("description", str)
 
     @classmethod
     def can_parse(cls, dct):
         """
         Override ObjectBase.can_parse because we had to remove the $ from $ref
         in __slots__ (since that's not a valid python variable name)
         """
         # TODO - can a reference object have spec extensions?
-        cleaned_keys = [k for k in dct.keys() if not k.startswith("x-")]
+        # summary and description are optional keys; their presence shouldn't
+        # affect what we can and can't parse (so remove them for the purpose of
+        # checking)
+        cleaned_keys = [k for k in dct.keys() if not k.startswith("x-") and k not in ("summary", "description")]
 
         return len(cleaned_keys) == 1 and "$ref" in dct
```

### Comparing `openapi3-1.7.0/openapi3/info.py` & `openapi3-1.8.0/openapi3/info.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.7.0/openapi3/object_base.py` & `openapi3-1.8.0/openapi3/object_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -509,18 +509,20 @@
                     resolved_value = self._root.resolve_path(reference_path)
                 except ReferenceResolutionError as e:
                     # add metadata to the error
                     e.path = self.path
                     e.element = self
                     raise
 
+                # TODO: remove _original_ref, as proxy objects now handle this
                 resolved_value._original_ref = value
+                proxy = ReferenceProxy(resolved_value, value)
 
                 # resolved
-                setattr(self, slot, resolved_value)
+                setattr(self, slot, proxy)
             elif issubclass(type(value), ObjectBase) or isinstance(value, Map):
                 # otherwise, continue resolving down the tree
                 value._resolve_references()
             elif isinstance(value, list):
                 # if it's a list, resolve its item's references
                 resolved_list = []
                 for item in value:
@@ -532,16 +534,18 @@
                             resolved_value = self._root.resolve_path(reference_path)
                         except ReferenceResolutionError as e:
                             # add metadata to the error
                             e.path = self.path
                             e.element = self
                             raise
 
+                        # TODO: remove _original_ref
                         resolved_value._original_ref = value
-                        resolved_list.append(resolved_value)
+                        proxy = ReferenceProxy(resolved_value, value)
+                        resolved_list.append(proxy)
                     else:
                         if issubclass(type(item), ObjectBase) or isinstance(item, Map):
                             item._resolve_references()
                         resolved_list.append(item)
 
                 setattr(self, slot, resolved_list)
 
@@ -644,18 +648,20 @@
                     resolved_value = self._root.resolve_path(reference_path)
                 except ReferenceResolutionError as e:
                     # add metadata to the error
                     e.path = self.path
                     e.element = self
                     raise
 
+                # TODO: Remove _original_ref
                 resolved_value._original_ref = value
+                proxy = ReferenceProxy(resolved_value, value)
 
                 # resolved
-                self[key] = resolved_value
+                self[key] = proxy
             else:
                 value._resolve_references()
 
     def _clone(self):
         """
         Returns a copy of this object and all its values
         """
@@ -678,7 +684,59 @@
         """
         Get the full path for this element in the spec
 
         :returns: The path in the spec for this element
         :rtype: str
         """
         return ".".join(self.path)
+
+
+class ReferenceProxy(ObjectBase):
+    """
+    This is a proxy class that is used to handle a resolved reference; for all
+    intents and purposes, it behaves like the object it proxies, except for the
+    following:
+
+     * If a "summary" or "description" were set in the Reference object _and_ the
+       proxies object has this attributes, the Reference object's values are used
+       instead
+     * This holds the original Reference object that it is proxying for, allowing
+       code to track down the reference
+     * Calling `type` on a ReferenceProxy will return the ReferenceProxy type;
+       use `type(ref._proxy)` or `isinstance(ref, Type)` to see the proxied type
+    """
+    def __init__(self, proxy, reference):
+        self._proxy = proxy
+        self._original_ref = reference
+
+    def __eq__(self, other):
+        """
+        Use the proxy object when comparing identity
+        """
+        return self._proxy == other
+
+    @property
+    def __class__(self):
+        """
+        Fake our class so we look like the proxied object's class
+        """
+        return self._proxy.__class__
+
+    def __getattribute__(self, value):
+        """
+        Overriding __getattribute__ allows us to act as the proxied object except
+        in very special cases.  This should make the proxy type virtually transparent
+        to a normal user.
+        """
+        # allow _proxy and _original_ref to access members of this class directly
+        if value in ("_proxy", "_original_ref", "__eq__"):
+            return object.__getattribute__(self, value)
+
+        # OpenAPI 3.1.0 allows Reference objects to make the summary and description
+        # fields of the object they're referencing, but only if they have the field
+        # defined _and_ the field exists in the type they're referencing.
+        if value in ("summary", "description"):
+            if hasattr(self._proxy, value) and getattr(self._original_ref, value) is not None:
+                return getattr(self._original_ref, value)
+
+        # otherwise, return the value of the proxied object
+        return getattr(self._proxy, value)
```

### Comparing `openapi3-1.7.0/openapi3/openapi.py` & `openapi3-1.8.0/openapi3/openapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         :param validate: If True, don't fail on errors, but instead capture all
                          errors, continuing along the spec as best as possible,
                          and make them available when parsing is complete.
         :type validate: bool
         :param ssl_verify: Decide if to use ssl verification to the requests or not,
                            in case an str is passed, will be used as the CA.
         :type ssl_verify: bool, str, None
-        :param use_session: Should we use a consistant session between API calls
+        :param use_session: Should we use a consistent session between API calls
         :type use_session: bool
         """
         # do this first so super().__init__ can see it
         self.validation_mode = validate
 
         if validate:
             self._spec_errors = []
@@ -171,20 +171,23 @@
         """
         self._operation_map = {}
 
         self.components = self._get("components", ["Components"])
         self.externalDocs = self._get("externalDocs", "ExternalDocumentation")
         self.info = self._get("info", "Info")
         self.openapi = self._get("openapi", str)
-        self.paths = self._get("paths", ["Path"], is_map=True)
+        self.paths = self._get("paths", ["Path", "Reference"], is_map=True)
         self.security = self._get("security", ["SecurityRequirement"], is_list=True)
         self.servers = self._get("servers", ["Server"], is_list=True)
         self.tags = self._get("tags", ["Tag"], is_list=True)
 
-        # now that we've parsed _all_ the data, resolve all references
+        # now that we've parsed _all_ the data, resolve all references; start with
+        # components so that paths that reference them will see the resolved references
+        if self.components is not None:
+            self.components._resolve_references()
         self._resolve_references()
         self._resolve_allOfs()
 
     def _get_callable(self, operation):
         """
         A helper function to create OperationCallable objects for __getattribute__,
         pre-initialized with the required values from this object.
```

### Comparing `openapi3-1.7.0/openapi3/paths.py` & `openapi3-1.8.0/openapi3/paths.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.7.0/openapi3/schemas.py` & `openapi3-1.8.0/openapi3/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 TYPE_LOOKUP = {
     "array": list,
     "integer": int,
     "object": dict,
     "string": str,
     "boolean": bool,
+    "number": float,
 }
 
 
 class Schema(ObjectBase):
     """
     The `Schema Object`_ allows the definition of input and output data types.
 
@@ -70,15 +71,15 @@
         self.title = self._get("title", str)
         self.maximum = self._get("maximum", [int, float])
         self.minimum = self._get("minimum", [int, float])
         self.maxLength = self._get("maxLength", int)
         self.minLength = self._get("minLength", int)
         self.pattern = self._get("pattern", str)
         self.maxItems = self._get("maxItems", int)
-        self.minItems = self._get("minItmes", int)
+        self.minItems = self._get("minItems", int)
         self.required = self._get("required", list)
         self.enum = self._get("enum", list)
         self.type = self._get("type", str)
         self.allOf = self._get("allOf", ["Schema", "Reference"], is_list=True)
         self.oneOf = self._get("oneOf", list)
         self.anyOf = self._get("anyOf", list)
         self.items = self._get("items", ["Schema", "Reference"])
@@ -124,15 +125,15 @@
 
            isinstance(object1, example._schema.get_type()) # true
            type(object1) == type(object2) # true
         """
         # this is defined in ObjectBase.__init__ as all slots are
         if self._model_type is None:  # pylint: disable=access-member-before-definition
             type_name = self.title or self.path[-1]
-            # if there are no defined properites for this model, use an empty dict
+            # if there are no defined properties for this model, use an empty dict
             # to allow the model to be set up correctly
             model_properties = self.properties or {}
 
             self._model_type = type(
                 type_name,
                 (Model,),
                 {"__slots__": model_properties.keys()},  # pylint: disable=attribute-defined-outside-init
```

### Comparing `openapi3-1.7.0/openapi3/security.py` & `openapi3-1.8.0/openapi3/security.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.7.0/openapi3/servers.py` & `openapi3-1.8.0/openapi3/servers.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.7.0/openapi3/tag.py` & `openapi3-1.8.0/openapi3/tag.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.7.0/openapi3.egg-info/PKG-INFO` & `openapi3-1.8.0/openapi3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi3
-Version: 1.7.0
+Version: 1.8.0
 Summary: Client and Validator of OpenAPI 3 Specifications
 Home-page: https://github.com/dorthu/openapi3
 Author: dorthu
 License: BSD 3-Clause License
 Description: openapi3
         ========
         
@@ -45,15 +45,15 @@
         
            # authenticate using a securityScheme defined in the spec's components.securitySchemes
            api.authenticate('personalAccessToken', my_token)
         
            # call an operation that requires authentication
            linodes  = api.call_getLinodeInstances()
         
-           # call an opertaion with parameters
+           # call an operation with parameters
            linode = api.call_getLinodeInstance(parameters={"linodeId": 123})
         
            # the models returns are all of the same (generated) type
            print(type(linode))                      # openapi.schemas.Linode
            type(linode) == type(linodes.data[0])    # True
         
            # call an operation with a request body
```

### Comparing `openapi3-1.7.0/setup.py` & `openapi3-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # get the long description from the README.rst
 with open(path.join(here, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="openapi3",
-    version="1.7.0",
+    version="1.8.0",
     description="Client and Validator of OpenAPI 3 Specifications",
     long_description=long_description,
     author="dorthu",
     url="https://github.com/dorthu/openapi3",
     packages=["openapi3"],
     license="BSD 3-Clause License",
     install_requires=["PyYaml", "requests"],
```

