# Comparing `tmp/sharedmap-1.0.4.tar.gz` & `tmp/sharedmap-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharedmap-1.0.4.tar", last modified: Tue Apr 25 09:22:56 2023, max compression
+gzip compressed data, was "sharedmap-1.0.5.tar", last modified: Fri May 26 11:01:11 2023, max compression
```

## Comparing `sharedmap-1.0.4.tar` & `sharedmap-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-04-25 09:22:56.691034 sharedmap-1.0.4/
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)    11558 2023-04-21 03:28:39.000000 sharedmap-1.0.4/LICENSE
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4382 2023-04-25 09:22:56.691034 sharedmap-1.0.4/PKG-INFO
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     3934 2023-04-25 09:14:13.000000 sharedmap-1.0.4/README.md
-drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-04-25 09:22:56.691034 sharedmap-1.0.4/native/
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7713 2023-04-20 08:09:14.000000 sharedmap-1.0.4/native/avltree.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1449 2023-04-18 07:54:55.000000 sharedmap-1.0.4/native/avltree.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1551 2023-04-21 03:58:52.000000 sharedmap-1.0.4/native/pynative.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      354 2023-04-25 08:55:57.000000 sharedmap-1.0.4/native/pynative.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7178 2023-04-25 09:10:45.000000 sharedmap-1.0.4/native/pyrbtree.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4336 2023-04-25 09:10:35.000000 sharedmap-1.0.4/native/pyshareabledict.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     3441 2023-04-20 13:10:17.000000 sharedmap-1.0.4/native/pytree.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)    11790 2022-08-26 03:07:03.000000 sharedmap-1.0.4/native/rbtree.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1116 2023-04-18 07:55:26.000000 sharedmap-1.0.4/native/rbtree.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1603 2023-04-20 03:55:37.000000 sharedmap-1.0.4/native/stringbox.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      990 2023-04-19 13:10:42.000000 sharedmap-1.0.4/native/stringbox.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     9429 2023-04-20 13:09:10.000000 sharedmap-1.0.4/native/tree.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     2759 2023-04-18 07:55:18.000000 sharedmap-1.0.4/native/tree.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)       38 2023-04-25 09:22:56.691034 sharedmap-1.0.4/setup.cfg
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1698 2023-04-25 09:22:42.000000 sharedmap-1.0.4/setup.py
-drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-04-25 09:22:56.691034 sharedmap-1.0.4/sharedmap.egg-info/
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4382 2023-04-25 09:22:56.000000 sharedmap-1.0.4/sharedmap.egg-info/PKG-INFO
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      399 2023-04-25 09:22:56.000000 sharedmap-1.0.4/sharedmap.egg-info/SOURCES.txt
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)        1 2023-04-25 09:22:56.000000 sharedmap-1.0.4/sharedmap.egg-info/dependency_links.txt
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)       10 2023-04-25 09:22:56.000000 sharedmap-1.0.4/sharedmap.egg-info/top_level.txt
+drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-05-26 11:01:11.382239 sharedmap-1.0.5/
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)    11558 2023-04-21 03:28:39.000000 sharedmap-1.0.5/LICENSE
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4382 2023-05-26 11:01:11.382239 sharedmap-1.0.5/PKG-INFO
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     3934 2023-04-25 09:14:13.000000 sharedmap-1.0.5/README.md
+drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-05-26 11:01:11.382239 sharedmap-1.0.5/native/
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7713 2023-04-20 08:09:14.000000 sharedmap-1.0.5/native/avltree.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1449 2023-04-18 07:54:55.000000 sharedmap-1.0.5/native/avltree.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1787 2023-05-26 07:46:29.000000 sharedmap-1.0.5/native/pynative.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      354 2023-05-26 07:39:32.000000 sharedmap-1.0.5/native/pynative.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7289 2023-05-26 09:52:50.000000 sharedmap-1.0.5/native/pyrbtree.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4401 2023-05-26 09:50:35.000000 sharedmap-1.0.5/native/pyshareabledict.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     6740 2023-05-26 10:52:55.000000 sharedmap-1.0.5/native/pysharedbitmap.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     3916 2023-05-26 10:47:44.000000 sharedmap-1.0.5/native/pytree.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)    11790 2022-08-26 03:07:03.000000 sharedmap-1.0.5/native/rbtree.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1116 2023-04-18 07:55:26.000000 sharedmap-1.0.5/native/rbtree.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1603 2023-04-20 03:55:37.000000 sharedmap-1.0.5/native/stringbox.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      990 2023-04-19 13:10:42.000000 sharedmap-1.0.5/native/stringbox.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     9429 2023-04-20 13:09:10.000000 sharedmap-1.0.5/native/tree.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     2759 2023-04-18 07:55:18.000000 sharedmap-1.0.5/native/tree.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)       38 2023-05-26 11:01:11.382239 sharedmap-1.0.5/setup.cfg
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1729 2023-05-26 10:48:55.000000 sharedmap-1.0.5/setup.py
+drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-05-26 11:01:11.382239 sharedmap-1.0.5/sharedmap.egg-info/
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4382 2023-05-26 11:01:11.000000 sharedmap-1.0.5/sharedmap.egg-info/PKG-INFO
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      425 2023-05-26 11:01:11.000000 sharedmap-1.0.5/sharedmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)        1 2023-05-26 11:01:11.000000 sharedmap-1.0.5/sharedmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)       10 2023-05-26 11:01:11.000000 sharedmap-1.0.5/sharedmap.egg-info/top_level.txt
```

### Comparing `sharedmap-1.0.4/LICENSE` & `sharedmap-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.4/PKG-INFO` & `sharedmap-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharedmap
-Version: 1.0.4
+Version: 1.0.5
 Summary: sharedmap
 Home-page: UNKNOWN
 Author: lyramilk
 Author-email: lyramilk@qq.com
 License: Apache License 2.0
 Keywords: sharedmap,sharememory,rbtree,avltree
 Platform: UNKNOWN
```

### Comparing `sharedmap-1.0.4/README.md` & `sharedmap-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.4/native/avltree.cpp` & `sharedmap-1.0.5/native/avltree.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.4/native/avltree.h` & `sharedmap-1.0.5/native/avltree.h`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.4/native/pynative.cpp` & `sharedmap-1.0.5/native/pynative.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 	}
 	if(PyType_Ready(&shareabledict_ObjectType) < 0){
 		printf("sharedmap.sharedmap not ready\n");
 	}else{
 		Py_INCREF(&shareabledict_ObjectType);
 		PyModule_AddObject(m, "sharedmap", (PyObject *)&shareabledict_ObjectType);
 	}
+
+	if(PyType_Ready(&shareablebitmap_ObjectType) < 0){
+		printf("sharedmap.sharedbitmap not ready\n");
+	}else{
+		Py_INCREF(&shareablebitmap_ObjectType);
+		PyModule_AddObject(m, "sharedbitmap", (PyObject *)&shareablebitmap_ObjectType);
+	}
 	return true;
 }
 
 
 
 
 #if PY_MAJOR_VERSION == 3
```

### Comparing `sharedmap-1.0.4/native/pyrbtree.cpp` & `sharedmap-1.0.5/native/pyrbtree.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -89,22 +89,24 @@
 	unsigned long avlsize = tv.bytescount();
 
 	unsigned long avlid = obj->sb->alloc(avlptr,avlsize);
 
 	unsigned long totalsize = sizeof(unsigned long long)/*totalsize的值*/ + sizeof(unsigned int)/*魔法数*/ + sizeof(unsigned long)/*avl树在stringbox中的id*/ + obj->sb->size();
 
 
-	key_t key = strtokey(sname,lname);
+	key_t key = strtokey(sname,lname,SHARED_TYPE_AVL);
 
 	sharememory sm;
 	if(!sm.init(key,totalsize,IPC_CREAT|IPC_EXCL|0666)){
 		if(errno == EEXIST && force == 1){
-			sm.init(key,totalsize,IPC_CREAT|0666);
-			sm.del();
-			if(!sm.init(key,totalsize,IPC_CREAT|0666)){
+			if(!sharememory::remove(key)){
+				PyErr_SetString(PyExc_OSError, strerror(errno));
+				return NULL;
+			}
+			if(!sm.init(key,totalsize,IPC_CREAT|IPC_EXCL|0666)){
 				PyErr_SetString(PyExc_OSError, strerror(errno));
 				return NULL;
 			}
 		}else{
 			PyErr_SetString(PyExc_OSError, strerror(errno));
 			return NULL;
 		}
@@ -159,21 +161,21 @@
 	const char *sname;
 	Py_ssize_t lname;
 	if (!(PyArg_ParseTuple(args, "s#", &sname, &lname))) {
 		Py_RETURN_NONE;
 	}
 
 
-	key_t key = strtokey(sname,lname);
+	key_t key = strtokey(sname,lname,SHARED_TYPE_AVL);
 	sharememory sm;
 	if(!sm.init(key,0,0)){
 		Py_RETURN_FALSE;
 	}
 
-	sm.del();
+	sharememory::remove(key);
 
 	Py_RETURN_TRUE;
 }
 
 PyObject * py_rbtree_new(PyTypeObject *type, PyObject *args, PyObject *kwds)
 {
 	PyObject * self = type->tp_alloc(type, 0);
```

### Comparing `sharedmap-1.0.4/native/pyshareabledict.cpp` & `sharedmap-1.0.5/native/pyshareabledict.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #include "pytree.h"
 #include <string.h>
 #include <errno.h>
 
-bool load_data(shareabledict_object* obj)
+bool static load_data(shareabledict_object* obj)
 {
 	if(obj->avt){
 		delete obj->avt;
 		obj->avt = NULL;
 	}
 	if(obj->sbr){
 		delete obj->sbr;
@@ -87,40 +87,39 @@
 	Py_RETURN_NONE;
 }
 
 PyObject * py_shareabledict_new(PyTypeObject *type, PyObject *args, PyObject *kwds)
 {
 	PyObject * self = type->tp_alloc(type, 0);
 	if(self){
-
 		char *sname;
 		Py_ssize_t lname;
 		if (PyArg_ParseTuple(args, "s#", &sname, &lname)) {
 
 			pylyramilkObject<shareabledict_object>* pobj = ((pylyramilkObject<shareabledict_object>*)(self));
 			shareabledict_object* obj = pobj->obj = new shareabledict_object;
 
 
-			obj->key = strtokey(sname,lname);
+			obj->key = strtokey(sname,lname,SHARED_TYPE_AVL);
 			sharememory sm;
 			if(!sm.init(obj->key,0,0)){
-				PyErr_SetString(PyExc_OSError, strerror(errno));
-
 				delete obj;
 				Py_TYPE(self)->tp_free((PyObject*)self);
+				PyErr_SetString(PyExc_OSError, strerror(errno));
 				return NULL;
 			}
 
 			if(load_data(obj)){
 				return self;
 			}
+			delete obj;
+			Py_TYPE(self)->tp_free((PyObject*)self);
 			PyErr_SetString(PyExc_OSError, strerror(errno));
 			return NULL;
 		}
-		return NULL;
 	}
 	PyErr_SetString(PyExc_OSError, strerror(errno));
 	return NULL;
 }
 
 void py_shareabledict_dealloc(PyObject* self)
 {
```

### Comparing `sharedmap-1.0.4/native/pytree.h` & `sharedmap-1.0.5/native/pytree.h`

 * *Files 14% similar despite different names*

```diff
@@ -32,34 +32,39 @@
 	}
 
 	bool init(key_t key, size_t size, int shmflg)
 	{
 		if(p){
 			clear();
 		}
+
 		shmid = shmget(key,size,shmflg);
 		if(shmid == -1){
 			return false;
 		}
 
 		_size = size;
 		return true;
 	}
 
-	void clear()
+	bool clear()
 	{
-		if(p) shmdt(p);
+		if(p){
+			int r = shmdt(p);
+			if(r == -1) return false;
+		}
 		p = NULL;
+		return true;
 	}
 
-	bool del()
+	bool static remove(key_t key)
 	{
+		int shmid = shmget(key,0,0);
 		if(shmid){
-			shmctl(shmid,IPC_RMID,NULL);
-			return true;
+			return shmctl(shmid,IPC_RMID,NULL) == 0;
 		}
 		return false;
 	}
 
 	char* ptr()
 	{
 		if (p) return p;
@@ -76,18 +81,26 @@
 
 	~sharememory()
 	{
 		clear();
 	}
 };
 
-key_t inline strtokey(const char* sname,unsigned long lname)
+
+const int SHARED_TYPE_AVL = 1;
+const int SHARED_TYPE_BITMAP = 1;
+
+
+
+
+key_t inline strtokey(const char* sname,unsigned long lname,int stype)
 {
 	std::string sharedmemoryname = "lyramilk.sharedmemory.";
 	sharedmemoryname.append(sname,lname);
+	sharedmemoryname.append((const char*)&stype,sizeof(stype));
 	key_t key = bkdr(sharedmemoryname.c_str(),sharedmemoryname.size());
 	return key;
 }
 
 
 struct boxdata
 {
@@ -208,8 +221,24 @@
 PyObject * py_shareabledict_get(PyObject *self, PyObject *args);
 PyObject * py_shareabledict_new(PyTypeObject *type, PyObject *args, PyObject *kwds);
 void py_shareabledict_dealloc(PyObject* self);
 
 extern PyMethodDef pyshareabledictObjectClassMethods[];
 extern PyTypeObject shareabledict_ObjectType;
 
+
+
+
+struct shared_bitmap_object
+{
+	std::string sharedmemoryname;
+	key_t key;
+	sharememory sm;
+	long* p;
+	long size;
+};
+
+
+extern PyMethodDef pyshareablebitmapObjectClassMethods[];
+extern PyTypeObject shareablebitmap_ObjectType;
+
 #endif
```

### Comparing `sharedmap-1.0.4/native/rbtree.cpp` & `sharedmap-1.0.5/native/rbtree.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.4/native/rbtree.h` & `sharedmap-1.0.5/native/rbtree.h`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.4/native/stringbox.cpp` & `sharedmap-1.0.5/native/stringbox.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.4/native/stringbox.h` & `sharedmap-1.0.5/native/stringbox.h`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.4/native/tree.cpp` & `sharedmap-1.0.5/native/tree.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.4/native/tree.h` & `sharedmap-1.0.5/native/tree.h`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.4/setup.py` & `sharedmap-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 other_sources = [
 	"native/stringbox.cpp",
 	"native/tree.cpp",
 	"native/avltree.cpp",
 	"native/rbtree.cpp",
 	"native/pyshareabledict.cpp",
+	"native/pysharedbitmap.cpp",
 	"native/pyrbtree.cpp",
 	"native/pynative.cpp",
 ]
 
 include_files = [
 	"native/avltree.h",
 	"native/pynative.h",
@@ -38,15 +39,15 @@
 	with open("README.md", "r") as fh:
 		long_description = fh.read()
 except Exception as e:
 	long_description = "";
 
 
 setup (name = projname,
-	version = '1.0.4',
+	version = '1.0.5',
 	description = projname,
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	author = "lyramilk",
 	packages=[],
 	ext_modules = [module1],
 	data_files=include_files,
```

### Comparing `sharedmap-1.0.4/sharedmap.egg-info/PKG-INFO` & `sharedmap-1.0.5/sharedmap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharedmap
-Version: 1.0.4
+Version: 1.0.5
 Summary: sharedmap
 Home-page: UNKNOWN
 Author: lyramilk
 Author-email: lyramilk@qq.com
 License: Apache License 2.0
 Keywords: sharedmap,sharememory,rbtree,avltree
 Platform: UNKNOWN
```

