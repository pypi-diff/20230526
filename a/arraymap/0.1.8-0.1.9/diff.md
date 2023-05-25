# Comparing `tmp/arraymap-0.1.8.tar.gz` & `tmp/arraymap-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraymap-0.1.8.tar", last modified: Mon May  8 23:12:41 2023, max compression
+gzip compressed data, was "arraymap-0.1.9.tar", last modified: Thu May 25 21:41:47 2023, max compression
```

## Comparing `arraymap-0.1.8.tar` & `arraymap-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:12:41.135154 arraymap-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-08 23:12:39.000000 arraymap-0.1.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-08 23:12:39.000000 arraymap-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-08 23:12:41.135154 arraymap-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-08 23:12:39.000000 arraymap-0.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    90930 2023-05-08 23:12:39.000000 arraymap-0.1.8/arraymap.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:12:41.131153 arraymap-0.1.8/arraymap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-08 23:12:41.000000 arraymap-0.1.8/arraymap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-08 23:12:41.000000 arraymap-0.1.8/arraymap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 23:12:41.000000 arraymap-0.1.8/arraymap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 23:12:41.000000 arraymap-0.1.8/arraymap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 23:12:41.000000 arraymap-0.1.8/arraymap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-08 23:12:41.135154 arraymap-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-08 23:12:39.000000 arraymap-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:12:41.135154 arraymap-0.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-05-08 23:12:39.000000 arraymap-0.1.8/test/test_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    25456 2023-05-08 23:12:39.000000 arraymap-0.1.8/test/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:41:47.475441 arraymap-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-25 21:41:46.000000 arraymap-0.1.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-25 21:41:46.000000 arraymap-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-25 21:41:47.475441 arraymap-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-25 21:41:46.000000 arraymap-0.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    90885 2023-05-25 21:41:46.000000 arraymap-0.1.9/arraymap.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:41:47.475441 arraymap-0.1.9/arraymap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-25 21:41:47.000000 arraymap-0.1.9/arraymap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-25 21:41:47.000000 arraymap-0.1.9/arraymap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:41:47.000000 arraymap-0.1.9/arraymap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 21:41:47.000000 arraymap-0.1.9/arraymap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 21:41:47.000000 arraymap-0.1.9/arraymap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 21:41:47.475441 arraymap-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-25 21:41:46.000000 arraymap-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:41:47.475441 arraymap-0.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-05-25 21:41:46.000000 arraymap-0.1.9/test/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25455 2023-05-25 21:41:46.000000 arraymap-0.1.9/test/test_unit.py
```

### Comparing `arraymap-0.1.8/LICENSE.md` & `arraymap-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arraymap-0.1.8/PKG-INFO` & `arraymap-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arraymap
-Version: 0.1.8
+Version: 0.1.9
 Summary: Dictionary-like lookup from NumPy array values to their integer positions
 Home-page: https://github.com/static-frame/arraymap
 Author: Christopher Ariza, Brandt Bucher
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
@@ -54,14 +54,26 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayMap
 -------------------------
 
+0.1.9
+........
+
+Improvements to ``PyObject`` struct layout and other internal refactoring.
+
+
+0.1.8
+........
+
+Corrected issue when using ``get_all()`` and ``get_any()`` on ``FrozenAutoMap`` backed by numerical arrays with less than 64-bit element size.
+
+
 0.1.7
 ........
 
 Corrected issue when creating a ``FrozenAutoMap`` from a ``datetime64`` array that has duplicates.
 
 
 0.1.6
```

### Comparing `arraymap-0.1.8/README.rst` & `arraymap-0.1.9/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -32,14 +32,26 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayMap
 -------------------------
 
+0.1.9
+........
+
+Improvements to ``PyObject`` struct layout and other internal refactoring.
+
+
+0.1.8
+........
+
+Corrected issue when using ``get_all()`` and ``get_any()`` on ``FrozenAutoMap`` backed by numerical arrays with less than 64-bit element size.
+
+
 0.1.7
 ........
 
 Corrected issue when creating a ``FrozenAutoMap`` from a ``datetime64`` array that has duplicates.
 
 
 0.1.6
```

### Comparing `arraymap-0.1.8/arraymap.c` & `arraymap-0.1.9/arraymap.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // For background on the hashtable design first implemented in AutoMap, see the following:
 // https://github.com/brandtbucher/automap/blob/b787199d38d6bfa1b55484e5ea1e89b31cc1fa72/automap.c#L12
-
-
 # include <math.h>
+# include "stdbool.h"
+
 # define PY_SSIZE_T_CLEAN
 # include "Python.h"
 
 # define PY_ARRAY_UNIQUE_SYMBOL AK_ARRAY_API
 # define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
 
 # include "numpy/arrayobject.h"
@@ -25,36 +25,32 @@
 
 static PyTypeObject AMType;
 static PyTypeObject FAMIType;
 static PyTypeObject FAMVType;
 static PyTypeObject FAMType;
 static PyObject *NonUniqueError;
 
-
 // The main storage "table" is an array of TableElement
 typedef struct TableElement{
     Py_ssize_t keys_pos;
     Py_hash_t hash;
 } TableElement;
 
-
 // Table configuration; experimentation shows that these values work well:
 # define LOAD 0.9
 # define SCAN 16
 
 const static size_t UCS4_SIZE = sizeof(Py_UCS4);
 
-
 // Partial, two-argument version of PyUnicode_FromKindAndData for consistent templating with bytes version.
 static inline PyObject*
 PyUnicode_FromUCS4AndData(const void *buffer, Py_ssize_t size) {
     return PyUnicode_FromKindAndData(PyUnicode_4BYTE_KIND, buffer, size);
 }
 
-
 typedef enum KeysArrayType{
     KAT_LIST = 0, // must be falsy
 
     KAT_INT8, // order matters as ranges of size are used in selection
     KAT_INT16,
     KAT_INT32,
     KAT_INT64,
@@ -81,35 +77,30 @@
     KAT_DTs,
     KAT_DTms,
     KAT_DTus,
     KAT_DTns,
     KAT_DTps,
     KAT_DTfs,
     KAT_DTas,
-
 } KeysArrayType;
 
-
 NPY_DATETIMEUNIT
 dt_unit_from_array(PyArrayObject* a) {
     // This is based on get_datetime_metadata_from_dtype in the NumPy source, but that function is private. This does not check that the dytpe is of the appropriate type.
     PyArray_DatetimeMetaData* dma = &(((PyArray_DatetimeDTypeMetaData *)PyArray_DESCR(a)->c_metadata)->meta);
     return dma->base;
 }
 
-
 NPY_DATETIMEUNIT
 dt_unit_from_scalar(PyDatetimeScalarObject* dts) {
     // Based on convert_pyobject_to_datetime and related usage in datetime.c
     PyArray_DatetimeMetaData* dma = &(dts->obmeta);
     return dma->base;
 }
 
-
-
 KeysArrayType
 at_to_kat(int array_t, PyArrayObject* a) {
     switch (array_t) {
         case NPY_INT64:
             return KAT_INT64;
         case NPY_INT32:
             return KAT_INT32;
@@ -174,16 +165,15 @@
             }
         }
         default:
             return KAT_LIST;
     }
 }
 
-
-// To determine when we can use direct array lookups, this function return 1 if we match, 0 if we do not match. Given a keys array type and the kind of lookup key, return true only for the largest KAT types.s
+// To determine when we can use direct array lookups, this function return 1 if we match, 0 if we do not match. Given a keys array type and the kind of lookup key, return true only for the largest KAT types.
 int
 kat_is_kind(KeysArrayType kat, char kind) {
     switch (kat) {
         case KAT_INT64:
         // case KAT_INT32:
         // case KAT_INT16:
         // case KAT_INT8:
@@ -222,103 +212,99 @@
 
         default:
             return 0;
     }
 }
 
 // Given a KAT, determine if it matches a NumPy dt64 unit.
-int
+bool
 kat_is_datetime_unit(KeysArrayType kat, NPY_DATETIMEUNIT unit) {
     switch (kat) {
         case KAT_DTY:
-            if (unit == NPY_FR_Y ) {return 1;}
+            if (unit == NPY_FR_Y ) {return true;}
             break;
         case KAT_DTM:
-            if (unit == NPY_FR_M ) {return 1;}
+            if (unit == NPY_FR_M ) {return true;}
             break;
         case KAT_DTW:
-            if (unit == NPY_FR_W ) {return 1;}
+            if (unit == NPY_FR_W ) {return true;}
             break;
         case KAT_DTD:
-            if (unit == NPY_FR_D ) {return 1;}
+            if (unit == NPY_FR_D ) {return true;}
             break;
         case KAT_DTh:
-            if (unit == NPY_FR_h ) {return 1;}
+            if (unit == NPY_FR_h ) {return true;}
             break;
         case KAT_DTm:
-            if (unit == NPY_FR_m ) {return 1;}
+            if (unit == NPY_FR_m ) {return true;}
             break;
         case KAT_DTs:
-            if (unit == NPY_FR_s ) {return 1;}
+            if (unit == NPY_FR_s ) {return true;}
             break;
         case KAT_DTms:
-            if (unit == NPY_FR_ms) {return 1;}
+            if (unit == NPY_FR_ms) {return true;}
             break;
         case KAT_DTus:
-            if (unit == NPY_FR_us) {return 1;}
+            if (unit == NPY_FR_us) {return true;}
             break;
         case KAT_DTns:
-            if (unit == NPY_FR_ns) {return 1;}
+            if (unit == NPY_FR_ns) {return true;}
             break;
         case KAT_DTps:
-            if (unit == NPY_FR_ps) {return 1;}
+            if (unit == NPY_FR_ps) {return true;}
             break;
         case KAT_DTfs:
-            if (unit == NPY_FR_fs) {return 1;}
+            if (unit == NPY_FR_fs) {return true;}
             break;
         case KAT_DTas:
-            if (unit == NPY_FR_as) {return 1;}
+            if (unit == NPY_FR_as) {return true;}
             break;
         default: // non dt64 KATs
-            return 0;
+            return false;
     }
-    return 0;
+    return false;
 }
 
 typedef struct FAMObject{
-    PyObject_VAR_HEAD
+    PyObject_HEAD
     Py_ssize_t table_size;
     TableElement *table;    // an array of TableElement structs
     PyObject *keys;
     KeysArrayType keys_array_type;
     Py_ssize_t keys_size;
     Py_UCS4* key_buffer;
 } FAMObject;
 
-
 typedef enum ViewKind{
     ITEMS,
     KEYS,
     VALUES,
 } ViewKind;
 
-
 // Return the end pointer, or the pointer to the location after the last valid character. The end pointer minus the start pointer is the number of characters. For an empty string, all characters are NULL, and the start pointer and end pointer should be equal. NOTE: would like to use strchr(str, '\0') instead of this routine, but some buffers might not have a null terminator and stread by full to the the dt_size.
 static inline Py_UCS4*
 ucs4_get_end_p(Py_UCS4* p_start, Py_ssize_t dt_size) {
     for (Py_UCS4* p = p_start + dt_size - 1; p >= p_start; p--) {
         if (*p != '\0') {
             return p + 1; // 1 after first non-null
         }
     }
     return p_start;
 }
 
-
 static inline char*
 char_get_end_p(char* p_start, Py_ssize_t dt_size) {
     for (char* p = p_start + dt_size - 1; p >= p_start; p--) {
         if (*p != '\0') {
             return p + 1; // 1 after first non-null
         }
     }
     return p_start;
 }
 
-
 // This masks the input with INT64_MAX, which removes the MSB; we then cast to an int64; the range is now between 0 and INT64_MAX. We then use the MSB of the original value; if set, we negate the number, producing negative values for the upper half of the uint64 range. Note that we only need to check for hash -1 in this branch.
 static inline Py_hash_t
 uint_to_hash(npy_uint64 v) {
     Py_hash_t hash = (Py_hash_t)(v & INT64_MAX);
     if (v >> 63) {
         hash = -hash;
     }
@@ -333,15 +319,14 @@
     Py_hash_t hash = (Py_hash_t)v;
     if (hash == -1) {
         return -2;
     }
     return hash;
 }
 
-
 // This is a adapted from https://github.com/python/cpython/blob/ba65a065cf07a7a9f53be61057a090f7311a5ad7/Python/pyhash.c#L92
 #define HASH_MODULUS (((size_t)1 << 61) - 1)
 #define HASH_BITS 61
 static inline Py_hash_t
 double_to_hash(double v)
 {
     int e, sign;
@@ -375,15 +360,14 @@
     x = ((x << e) & HASH_MODULUS) | x >> (HASH_BITS - e);
     x = x * sign;
     if (x == (Py_uhash_t)-1)
         x = (Py_uhash_t)-2;
     return (Py_hash_t)x;
 }
 
-
 // The `str` arg is a pointer to a C-array of Py_UCS4; we will only read `len` characters from this. This is a "djb2" hash algorithm.
 static inline Py_hash_t
 unicode_to_hash(Py_UCS4 *str, Py_ssize_t len) {
     Py_UCS4* p = str;
     Py_UCS4* p_end = str + len;
     Py_hash_t hash = 5381;
     while (p < p_end) {
@@ -391,40 +375,36 @@
     }
     if (hash == -1) {
         return -2;
     }
     return hash;
 }
 
-
 static inline Py_hash_t
 string_to_hash(char *str, Py_ssize_t len) {
     char* p = str;
     char* p_end = str + len;
     Py_hash_t hash = 5381;
     while (p < p_end) {
         hash = ((hash << 5) + hash) + *p++;
     }
     if (hash == -1) {
         return -2;
     }
     return hash;
 }
 
-
 //------------------------------------------------------------------------------
 // the global int_cache is shared among all instances
 
 static PyObject *int_cache = NULL;
 
-
 // NOTE: this used to be a Py_ssize_t, which can be 32 bits on some machines and might easily overflow with a few very large indices. Using an explicit 64-bit int seems safer
 static npy_int64 key_count_global = 0;
 
-
 // Fill the int_cache up to size_needed with PyObject ints; `size` is not the key_count_global.
 static int
 int_cache_fill(Py_ssize_t size_needed)
 {
     PyObject *item;
     if (!int_cache) {
         int_cache = PyList_New(0);
@@ -442,58 +422,54 @@
             return -1;
         }
         Py_DECREF(item);
     }
     return 0;
 }
 
-
 // Given the current key_count_global, remove cache elements only if the key_count is less than the the current size of the int_cache.
 void
 int_cache_remove(Py_ssize_t key_count)
 {
     if (!key_count) {
         Py_CLEAR(int_cache);
     }
     else if (key_count < PyList_GET_SIZE(int_cache)) {
         // del int_cache[key_count:]
         PyList_SetSlice(int_cache, key_count, PyList_GET_SIZE(int_cache), NULL);
     }
 }
 
-
 //------------------------------------------------------------------------------
 // FrozenAutoMapIterator functions
 
 typedef struct FAMIObject {
-    PyObject_VAR_HEAD
+    PyObject_HEAD
     FAMObject *fam;
     PyArrayObject* keys_array;
     ViewKind kind;
-    int reversed;
+    bool reversed;
     Py_ssize_t index; // current index state, mutated in-place
 } FAMIObject;
 
 
 static void
 fami_dealloc(FAMIObject *self)
 {
     Py_DECREF(self->fam);
-    Py_TYPE(self)->tp_free((PyObject *)self);
+    PyObject_Del((PyObject *)self);
 }
 
-
 static FAMIObject *
 fami_iter(FAMIObject *self)
 {
     Py_INCREF(self);
     return self;
 }
 
-
 // For a FAMI, Return appropriate PyObject for items, keys, and values. When values are needed they are retrieved from the int_cache. For consistency with NumPy array iteration, arrays use PyArray_ToScalar instead of PyArray_GETITEM.
 static PyObject *
 fami_iternext(FAMIObject *self)
 {
     Py_ssize_t index;
     if (self->reversed) {
         index = self->fam->keys_size - ++self->index;
@@ -539,53 +515,48 @@
             Py_INCREF(yield);
             return yield;
         }
     }
     Py_UNREACHABLE();
 }
 
-
 static PyObject *
-fami___length_hint__(FAMIObject *self)
+fami_length_hint(FAMIObject *self)
 {
     Py_ssize_t len = Py_MAX(0, self->fam->keys_size - self->index);
     return PyLong_FromSsize_t(len);
 }
 
-
-static PyObject *fami_new(FAMObject *, ViewKind, int);
-
+static PyObject *fami_new(FAMObject *, ViewKind, bool);
 
 static PyObject *
-fami___reversed__(FAMIObject *self)
+fami_reversed(FAMIObject *self)
 {
     return fami_new(self->fam, self->kind, !self->reversed);
 }
 
-
 static PyMethodDef fami_methods[] = {
-    {"__length_hint__", (PyCFunction)fami___length_hint__, METH_NOARGS, NULL},
-    {"__reversed__", (PyCFunction)fami___reversed__, METH_NOARGS, NULL},
+    {"__length_hint__", (PyCFunction)fami_length_hint, METH_NOARGS, NULL},
+    {"__reversed__", (PyCFunction)fami_reversed, METH_NOARGS, NULL},
     {NULL},
 };
 
-
 static PyTypeObject FAMIType = {
     PyVarObject_HEAD_INIT(NULL, 0)
     .tp_basicsize = sizeof(FAMIObject),
     .tp_dealloc = (destructor) fami_dealloc,
     .tp_iter = (getiterfunc) fami_iter,
     .tp_iternext = (iternextfunc) fami_iternext,
     .tp_methods = fami_methods,
     .tp_name = "arraymap.FrozenAutoMapIterator",
 };
 
 
 static PyObject *
-fami_new(FAMObject *fam, ViewKind kind, int reversed)
+fami_new(FAMObject *fam, ViewKind kind, bool reversed)
 {
     FAMIObject *fami = PyObject_New(FAMIObject, &FAMIType);
     if (!fami) {
         return NULL;
     }
     Py_INCREF(fam);
     fami->fam = fam;
@@ -602,15 +573,15 @@
 }
 
 //------------------------------------------------------------------------------
 // FrozenAutoMapView functions
 
 // A FAMVObject contains a reference to the FAM from which it was derived
 typedef struct FAMVObject{
-    PyObject_VAR_HEAD
+    PyObject_HEAD
     FAMObject *fam;
     ViewKind kind;
 } FAMVObject;
 
 # define FAMV_SET_OP(name, op)                            \
 static PyObject *                                         \
 name(PyObject *left, PyObject *right)                     \
@@ -672,36 +643,36 @@
 };
 
 
 static void
 famv_dealloc(FAMVObject *self)
 {
     Py_DECREF(self->fam);
-    Py_TYPE(self)->tp_free((PyObject *)self);
+    PyObject_Del((PyObject *)self);
 }
 
 
 static PyObject *
 famv_fami_new(FAMVObject *self)
 {
-    return fami_new(self->fam, self->kind, 0);
+    return fami_new(self->fam, self->kind, false);
 }
 
 
 static PyObject *
-famv___length_hint__(FAMVObject *self)
+famv_length_hint(FAMVObject *self)
 {
     return PyLong_FromSsize_t(self->fam->keys_size);
 }
 
 
 static PyObject *
-famv___reversed__(FAMVObject *self)
+famv_reversed(FAMVObject *self)
 {
-    return fami_new(self->fam, self->kind, 1);
+    return fami_new(self->fam, self->kind, true);
 }
 
 
 static PyObject *
 famv_isdisjoint(FAMVObject *self, PyObject *other)
 {
     PyObject *intersection = famv_and((PyObject *)self, other);
@@ -730,16 +701,16 @@
     Py_DECREF(left);
     Py_DECREF(right);
     return result;
 }
 
 
 static PyMethodDef famv_methods[] = {
-    {"__length_hint__", (PyCFunction) famv___length_hint__, METH_NOARGS, NULL},
-    {"__reversed__", (PyCFunction) famv___reversed__, METH_NOARGS, NULL},
+    {"__length_hint__", (PyCFunction) famv_length_hint, METH_NOARGS, NULL},
+    {"__reversed__", (PyCFunction) famv_reversed, METH_NOARGS, NULL},
     {"isdisjoint", (PyCFunction) famv_isdisjoint, METH_O, NULL},
     {NULL},
 };
 
 
 static PyTypeObject FAMVType = {
     PyVarObject_HEAD_INIT(NULL, 0)
@@ -751,15 +722,15 @@
     .tp_methods = famv_methods,
     .tp_name = "arraymap.FrozenAutoMapView",
     .tp_richcompare = (richcmpfunc) famv_richcompare,
 };
 
 
 static PyObject *
-famv_new(FAMObject *fam, int kind)
+famv_new(FAMObject *fam, ViewKind kind)
 {
     FAMVObject *famv = (FAMVObject *)PyObject_New(FAMVObject, &FAMVType);
     if (!famv) {
         return NULL;
     }
     famv->kind = kind;
     famv->fam = fam;
@@ -1631,15 +1602,14 @@
 
     // if we have an old table, move them into the new table
     if (size_old) {
         if (self->keys_array_type) {
             PyErr_SetString(PyExc_NotImplementedError, "Cannot grow table for array keys");
             goto restore;
         }
-
         Py_ssize_t i;
         Py_hash_t h;
         for (table_pos = 0; table_pos < size_old + SCAN - 1; table_pos++) {
             i = table_old[table_pos].keys_pos;
             h = table_old[table_pos].hash;
             if ((h != -1) && insert_obj(self, PyList_GET_ITEM(self->keys, i), i, h))
             {
@@ -2293,34 +2263,34 @@
     return hash;
 }
 
 
 static PyObject *
 fam_iter(FAMObject *self)
 {
-    return fami_new(self, KEYS, 0);
+    return fami_new(self, KEYS, false);
 }
 
 
 static PyObject *
-fam___getnewargs__(FAMObject *self)
+fam_getnewargs(FAMObject *self)
 {
     return PyTuple_Pack(1, self->keys);
 }
 
 
 static PyObject *
-fam___reversed__(FAMObject *self)
+fam_reversed(FAMObject *self)
 {
-    return fami_new(self, KEYS, 1);
+    return fami_new(self, KEYS, true);
 }
 
 
 static PyObject *
-fam___sizeof__(FAMObject *self)
+fam_sizeof(FAMObject *self)
 {
     PyObject *listsizeof = PyObject_CallMethod(self->keys, "__sizeof__", NULL);
     if (!listsizeof) {
         return NULL;
     }
     Py_ssize_t listbytes = PyLong_AsSsize_t(listsizeof);
     Py_DECREF(listsizeof);
@@ -2376,15 +2346,14 @@
     if (!self) {
         return NULL;
     }
     self->table = NULL;
     self->keys = NULL;
     self->key_buffer = NULL;
     self->keys_size = 0;
-
     return (PyObject*)self;
 }
 
 
 // This macro can be used with integer and floating point NumPy types, given an `npy_type` and a specialized `insert_func`. Uses context of `fam_init` to get `fam`, `contiguous`, `a`, `keys_size`, and `i`. An optional `post_deref` function can be supplied to transform extracted values before calling the appropriate insert function.
 # define INSERT_SCALARS(npy_type, insert_func, kat, post_deref)   \
 {                                                                 \
@@ -2631,24 +2600,24 @@
         Py_RETURN_NOTIMPLEMENTED;
     }
     return PyObject_RichCompare(self->keys, ((FAMObject *)other)->keys, op);
 }
 
 
 static PyObject*
-fam___getstate__(FAMObject *self)
+fam_getstate(FAMObject *self)
 {
     PyObject* state = PyTuple_Pack(1, self->keys);
     return state;
 }
 
 
 // State returned here is a tuple of keys, suitable for usage as an `args` argument.
 static PyObject*
-fam___setstate__(FAMObject *self, PyObject *state)
+fam_setstate(FAMObject *self, PyObject *state)
 {
     if (!PyTuple_CheckExact(state) || !PyTuple_GET_SIZE(state)) {
         PyErr_SetString(PyExc_ValueError, "Unexpected pickled object.");
         return NULL;
     }
     PyObject *keys = PyTuple_GetItem(state, 0);
     if (PyArray_Check(keys)) {
@@ -2657,19 +2626,19 @@
     }
     fam_init((PyObject*)self, state, NULL);
     Py_RETURN_NONE;
 }
 
 
 static PyMethodDef fam_methods[] = {
-    {"__getnewargs__", (PyCFunction) fam___getnewargs__, METH_NOARGS, NULL},
-    {"__reversed__", (PyCFunction) fam___reversed__, METH_NOARGS, NULL},
-    {"__sizeof__", (PyCFunction) fam___sizeof__, METH_NOARGS, NULL},
-    {"__getstate__", (PyCFunction) fam___getstate__, METH_NOARGS, NULL},
-    {"__setstate__", (PyCFunction) fam___setstate__, METH_O, NULL},
+    {"__getnewargs__", (PyCFunction) fam_getnewargs, METH_NOARGS, NULL},
+    {"__reversed__", (PyCFunction) fam_reversed, METH_NOARGS, NULL},
+    {"__sizeof__", (PyCFunction) fam_sizeof, METH_NOARGS, NULL},
+    {"__getstate__", (PyCFunction) fam_getstate, METH_NOARGS, NULL},
+    {"__setstate__", (PyCFunction) fam_setstate, METH_O, NULL},
     {"get", (PyCFunction) fam_get, METH_VARARGS, NULL},
     {"items", (PyCFunction) fam_items, METH_NOARGS, NULL},
     {"keys", (PyCFunction) fam_keys, METH_NOARGS, NULL},
     {"values", (PyCFunction) fam_values, METH_NOARGS, NULL},
     {"get_all", (PyCFunction) fam_get_all, METH_O, NULL},
     {"get_any", (PyCFunction) fam_get_any, METH_O, NULL},
     {NULL},
```

### Comparing `arraymap-0.1.8/arraymap.egg-info/PKG-INFO` & `arraymap-0.1.9/arraymap.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arraymap
-Version: 0.1.8
+Version: 0.1.9
 Summary: Dictionary-like lookup from NumPy array values to their integer positions
 Home-page: https://github.com/static-frame/arraymap
 Author: Christopher Ariza, Brandt Bucher
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
@@ -54,14 +54,26 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayMap
 -------------------------
 
+0.1.9
+........
+
+Improvements to ``PyObject`` struct layout and other internal refactoring.
+
+
+0.1.8
+........
+
+Corrected issue when using ``get_all()`` and ``get_any()`` on ``FrozenAutoMap`` backed by numerical arrays with less than 64-bit element size.
+
+
 0.1.7
 ........
 
 Corrected issue when creating a ``FrozenAutoMap`` from a ``datetime64`` array that has duplicates.
 
 
 0.1.6
```

### Comparing `arraymap-0.1.8/setup.py` & `arraymap-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 import typing as tp
 import site
 import os
 
 
-AM_VERSION = "0.1.8"
+AM_VERSION = "0.1.9"
 
 
 with open("README.rst") as file:
     LONG_DESCRIPTION = file.read()
 
 
 def get_ext_dir(*components: tp.Iterable[str]) -> tp.Sequence[str]:
```

### Comparing `arraymap-0.1.8/test/test_property.py` & `arraymap-0.1.9/test/test_property.py`

 * *Files identical despite different names*

### Comparing `arraymap-0.1.8/test/test_unit.py` & `arraymap-0.1.9/test/test_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -918,15 +918,14 @@
     post1 = fam.get_all(np.array([30, 100], dtype=np.int64))
     assert post1.tolist() == [2, 1]
 
     post2 = fam.get_all(np.array([30, 100], dtype=np.int8))
     assert post2.tolist() == [2, 1]
 
 
-
 # -------------------------------------------------------------------------------
 
 
 def test_fam_array_get_any_a1():
     a1 = np.array(("a", "bb", "ccc"))
     a1.flags.writeable = False
     fam = FrozenAutoMap(a1)
```

