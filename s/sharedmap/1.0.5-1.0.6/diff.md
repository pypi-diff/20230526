# Comparing `tmp/sharedmap-1.0.5.tar.gz` & `tmp/sharedmap-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharedmap-1.0.5.tar", last modified: Fri May 26 11:01:11 2023, max compression
+gzip compressed data, was "sharedmap-1.0.6.tar", last modified: Fri May 26 12:36:11 2023, max compression
```

## Comparing `sharedmap-1.0.5.tar` & `sharedmap-1.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-05-26 11:01:11.382239 sharedmap-1.0.5/
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)    11558 2023-04-21 03:28:39.000000 sharedmap-1.0.5/LICENSE
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4382 2023-05-26 11:01:11.382239 sharedmap-1.0.5/PKG-INFO
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     3934 2023-04-25 09:14:13.000000 sharedmap-1.0.5/README.md
-drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-05-26 11:01:11.382239 sharedmap-1.0.5/native/
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7713 2023-04-20 08:09:14.000000 sharedmap-1.0.5/native/avltree.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1449 2023-04-18 07:54:55.000000 sharedmap-1.0.5/native/avltree.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1787 2023-05-26 07:46:29.000000 sharedmap-1.0.5/native/pynative.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      354 2023-05-26 07:39:32.000000 sharedmap-1.0.5/native/pynative.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7289 2023-05-26 09:52:50.000000 sharedmap-1.0.5/native/pyrbtree.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4401 2023-05-26 09:50:35.000000 sharedmap-1.0.5/native/pyshareabledict.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     6740 2023-05-26 10:52:55.000000 sharedmap-1.0.5/native/pysharedbitmap.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     3916 2023-05-26 10:47:44.000000 sharedmap-1.0.5/native/pytree.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)    11790 2022-08-26 03:07:03.000000 sharedmap-1.0.5/native/rbtree.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1116 2023-04-18 07:55:26.000000 sharedmap-1.0.5/native/rbtree.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1603 2023-04-20 03:55:37.000000 sharedmap-1.0.5/native/stringbox.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      990 2023-04-19 13:10:42.000000 sharedmap-1.0.5/native/stringbox.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     9429 2023-04-20 13:09:10.000000 sharedmap-1.0.5/native/tree.cpp
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     2759 2023-04-18 07:55:18.000000 sharedmap-1.0.5/native/tree.h
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)       38 2023-05-26 11:01:11.382239 sharedmap-1.0.5/setup.cfg
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1729 2023-05-26 10:48:55.000000 sharedmap-1.0.5/setup.py
-drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-05-26 11:01:11.382239 sharedmap-1.0.5/sharedmap.egg-info/
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4382 2023-05-26 11:01:11.000000 sharedmap-1.0.5/sharedmap.egg-info/PKG-INFO
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      425 2023-05-26 11:01:11.000000 sharedmap-1.0.5/sharedmap.egg-info/SOURCES.txt
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)        1 2023-05-26 11:01:11.000000 sharedmap-1.0.5/sharedmap.egg-info/dependency_links.txt
--rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)       10 2023-05-26 11:01:11.000000 sharedmap-1.0.5/sharedmap.egg-info/top_level.txt
+drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-05-26 12:36:11.349715 sharedmap-1.0.6/
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)    11558 2023-04-21 03:28:39.000000 sharedmap-1.0.6/LICENSE
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4382 2023-05-26 12:36:11.345715 sharedmap-1.0.6/PKG-INFO
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     3934 2023-04-25 09:14:13.000000 sharedmap-1.0.6/README.md
+drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-05-26 12:36:11.345715 sharedmap-1.0.6/native/
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7713 2023-04-20 08:09:14.000000 sharedmap-1.0.6/native/avltree.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1449 2023-04-18 07:54:55.000000 sharedmap-1.0.6/native/avltree.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1787 2023-05-26 07:46:29.000000 sharedmap-1.0.6/native/pynative.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      354 2023-05-26 07:39:32.000000 sharedmap-1.0.6/native/pynative.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7289 2023-05-26 09:52:50.000000 sharedmap-1.0.6/native/pyrbtree.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4401 2023-05-26 09:50:35.000000 sharedmap-1.0.6/native/pyshareabledict.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     7202 2023-05-26 12:30:08.000000 sharedmap-1.0.6/native/pysharedbitmap.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4445 2023-05-26 12:32:50.000000 sharedmap-1.0.6/native/pytree.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)    11790 2022-08-26 03:07:03.000000 sharedmap-1.0.6/native/rbtree.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1116 2023-04-18 07:55:26.000000 sharedmap-1.0.6/native/rbtree.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1603 2023-04-20 03:55:37.000000 sharedmap-1.0.6/native/stringbox.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      990 2023-04-19 13:10:42.000000 sharedmap-1.0.6/native/stringbox.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     9429 2023-04-20 13:09:10.000000 sharedmap-1.0.6/native/tree.cpp
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     2759 2023-04-18 07:55:18.000000 sharedmap-1.0.6/native/tree.h
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)       38 2023-05-26 12:36:11.349715 sharedmap-1.0.6/setup.cfg
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     1729 2023-05-26 12:33:45.000000 sharedmap-1.0.6/setup.py
+drwxrwxr-x   0 lyramilk  (1000) lyramilk  (1000)        0 2023-05-26 12:36:11.345715 sharedmap-1.0.6/sharedmap.egg-info/
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)     4382 2023-05-26 12:36:11.000000 sharedmap-1.0.6/sharedmap.egg-info/PKG-INFO
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)      425 2023-05-26 12:36:11.000000 sharedmap-1.0.6/sharedmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)        1 2023-05-26 12:36:11.000000 sharedmap-1.0.6/sharedmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 lyramilk  (1000) lyramilk  (1000)       10 2023-05-26 12:36:11.000000 sharedmap-1.0.6/sharedmap.egg-info/top_level.txt
```

### Comparing `sharedmap-1.0.5/LICENSE` & `sharedmap-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.5/PKG-INFO` & `sharedmap-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharedmap
-Version: 1.0.5
+Version: 1.0.6
 Summary: sharedmap
 Home-page: UNKNOWN
 Author: lyramilk
 Author-email: lyramilk@qq.com
 License: Apache License 2.0
 Keywords: sharedmap,sharememory,rbtree,avltree
 Platform: UNKNOWN
```

### Comparing `sharedmap-1.0.5/README.md` & `sharedmap-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.5/native/avltree.cpp` & `sharedmap-1.0.6/native/avltree.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.5/native/avltree.h` & `sharedmap-1.0.6/native/avltree.h`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.5/native/pynative.cpp` & `sharedmap-1.0.6/native/pynative.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.5/native/pyrbtree.cpp` & `sharedmap-1.0.6/native/pyrbtree.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.5/native/pyshareabledict.cpp` & `sharedmap-1.0.6/native/pyshareabledict.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.5/native/pysharedbitmap.cpp` & `sharedmap-1.0.6/native/pysharedbitmap.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -35,24 +35,22 @@
 
 
 
 bool static load_data(shared_bitmap_object* obj)
 {
 	char* pbase = obj->sm.ptr();
 
-	unsigned long totalsize = 0;
-	memcpy(&totalsize,pbase,sizeof(totalsize));
 	unsigned int magic = 0x5026;
-	memcpy(&magic,pbase+sizeof(unsigned long)/*totalsize的值*/,sizeof(magic));
+	memcpy(&magic,pbase,sizeof(magic));
 	if(magic != 0x5026){
 		return false;
 	}
 
-	obj->p = (long*)(pbase + 16);
-	obj->size = (long)(pbase + totalsize - (const char*)obj->p + 7) >> intc<sizeof(long)>::square;
+	obj->p = (long*)(pbase + 8);
+	obj->size = (long)(pbase + obj->sm.size() - (const char*)obj->p + 7) >> intc<sizeof(long)>::square;
 	return true;
 }
 
 PyObject * py_shared_bitmap_set(PyObject *self, PyObject *args)
 {
 	if(self == NULL){
 		return NULL;
@@ -75,14 +73,43 @@
 		obj->p[bytesindex] |= 1<<offset;
 	}else{
 		obj->p[bytesindex] &= ~(1<<offset);
 	}
 	Py_RETURN_NONE;
 }
 
+PyObject * py_shared_bitmap_size(PyObject *self, PyObject *args)
+{
+	if(self == NULL){
+		return NULL;
+	}
+	shared_bitmap_object* obj = ((pylyramilkObject<shared_bitmap_object>*)(self))->obj;
+	return Py_BuildValue("l",obj->size << intc<sizeof(long)>::square);
+}
+
+PyObject * py_shared_bitmap_resize(PyObject *self, PyObject *args)
+{
+	if(self == NULL){
+		return NULL;
+	}
+	long size = 0;
+	if (!(PyArg_ParseTuple(args, "l",&size))) {
+		return NULL;
+	}
+	long totalsize = size + 8;
+	shared_bitmap_object* obj = ((pylyramilkObject<shared_bitmap_object>*)(self))->obj;
+
+	if(obj->sm.resize(totalsize)){
+		if(load_data(obj)){
+			Py_RETURN_TRUE;
+		}
+	}
+	Py_RETURN_FALSE;
+}
+
 PyObject * py_shared_bitmap_get(PyObject *self, PyObject *args)
 {
 	if(self == NULL){
 		return NULL;
 	}
 	long index = 0;
 	if (!(PyArg_ParseTuple(args, "l",&index))) {
@@ -95,18 +122,16 @@
 	if(bytesindex > obj->size){
 		PyErr_SetString(PyExc_KeyError, "index out of range");
 		return NULL;
 	}
 
 	if(obj->p[bytesindex] & (1<<offset)){
 		Py_RETURN_TRUE;
-	}else{
-		Py_RETURN_FALSE;
 	}
-
+	Py_RETURN_FALSE;
 }
 
 PyObject * py_shared_bitmap_new(PyTypeObject *type, PyObject *args, PyObject *kwds)
 {
 	PyObject * self = type->tp_alloc(type, 0);
 	if(self){
 		char *sname;
@@ -141,61 +166,59 @@
 		PyErr_SetString(PyExc_OSError, strerror(errno));
 		return NULL;
 	}
 	PyErr_SetString(PyExc_OSError, strerror(errno));
 	return NULL;
 }
 
-//	{"create", py_shared_bitmap_create, METH_VARARGS | METH_STATIC|METH_KEYWORDS},
 PyObject * py_shared_bitmap_create(PyTypeObject *, PyObject *args, PyObject *kwds)
 {
 	PyTypeObject *type = &shareablebitmap_ObjectType;
 
 	PyObject * self = type->tp_alloc(type, 0);
 	if(self){
 		char *sname;
 		Py_ssize_t lname;
 		long size = 0;
 		char force = 0;
 
 		static const char *kwlist[] = {"name", "size", "force",NULL};
 		if (PyArg_ParseTupleAndKeywords(args,kwds, "s#l|b",(char**)kwlist, &sname, &lname, &size,&force)) {
+			long totalsize = size + 8;
 			pylyramilkObject<shared_bitmap_object>* pobj = ((pylyramilkObject<shared_bitmap_object>*)(self));
 			shared_bitmap_object* obj = pobj->obj = new shared_bitmap_object;
 			obj->sharedmemoryname.assign(sname,lname);
 			obj->key = strtokey(sname,lname,SHARED_TYPE_BITMAP);
 
-			if(!obj->sm.init(obj->key,size,IPC_CREAT|IPC_EXCL|0666)){
+			if(!obj->sm.init(obj->key,totalsize,IPC_CREAT|IPC_EXCL|0666)){
 				if(errno == EEXIST && force == 1){
 					if(!sharememory::remove(obj->key)){
 						delete obj;
 						Py_TYPE(self)->tp_free((PyObject*)self);
 						PyErr_SetString(PyExc_OSError, strerror(errno));
 						return NULL;
 					}
-					if(!obj->sm.init(obj->key,size,IPC_CREAT|IPC_EXCL|0666)){
+					if(!obj->sm.init(obj->key,totalsize,IPC_CREAT|IPC_EXCL|0666)){
 						delete obj;
 						Py_TYPE(self)->tp_free((PyObject*)self);
 						PyErr_SetString(PyExc_OSError, strerror(errno));
 						return NULL;
 					}
 				}else{
 					delete obj;
 					Py_TYPE(self)->tp_free((PyObject*)self);
 					PyErr_SetString(PyExc_OSError, strerror(errno));
 					return NULL;
 				}
 			}
 
 
-			long totalsize = size + 16;
 			char* psharedmemory = obj->sm.ptr();
-			memcpy(psharedmemory,&totalsize,sizeof(totalsize));
 			unsigned int magic = 0x5026;
-			memcpy(psharedmemory + sizeof(unsigned long long)/*totalsize的值*/,&magic,sizeof(magic));
+			memcpy(psharedmemory,&magic,sizeof(magic));
 
 			if(load_data(obj)){
 				return self;
 			}
 			delete obj;
 		}
 		Py_TYPE(self)->tp_free((PyObject*)self);
@@ -222,14 +245,16 @@
 */
 
 
 PyMethodDef pyshareablebitmapObjectClassMethods[] = {
 	{"create", (PyCFunction)py_shared_bitmap_create, METH_VARARGS | METH_STATIC|METH_KEYWORDS},
 	{"set", py_shared_bitmap_set, METH_VARARGS},
 	{"get", py_shared_bitmap_get, METH_VARARGS},
+	{"size", py_shared_bitmap_size, METH_VARARGS},
+	{"resize", py_shared_bitmap_resize, METH_VARARGS},
 	{NULL, NULL},
 };
 
 PyTypeObject shareablebitmap_ObjectType = {
 	PyVarObject_HEAD_INIT(NULL, 0)
 	"sharedmap.sharedbitmap",				/*tp_name*/
 	sizeof(pylyramilkObject<shared_bitmap_object>),		/*tp_basicsize*/
```

### Comparing `sharedmap-1.0.5/native/pytree.h` & `sharedmap-1.0.6/native/pytree.h`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #include "pynative.h"
 
 #include "avltree.h"
 #include "rbtree.h"
 #include "stringbox.h"
 
 #include <sys/shm.h>
+#include <memory.h>
 
 
 unsigned int inline bkdr(const char* p,std::size_t l)
 {
 	unsigned int r = 0;
 	for(;l > 0;--l){
 		r = r*131 + (*p++);
@@ -19,47 +20,75 @@
 
 
 class sharememory
 {
 	int shmid;
 	char* p;
 
-	unsigned long _size;
+	long _size;
+	key_t key;
   public:
 	sharememory()
 	{
 		shmid = -1;
 		p = NULL;
+		key = 0;
 	}
 
 	bool init(key_t key, size_t size, int shmflg)
 	{
 		if(p){
 			clear();
 		}
 
 		shmid = shmget(key,size,shmflg);
 		if(shmid == -1){
 			return false;
 		}
 
-		_size = size;
+		this->key = key;
+
+		struct shmid_ds ds;
+		if(shmctl(shmid,IPC_STAT,&ds) != 0) return false;
+		_size = ds.shm_segsz;
 		return true;
 	}
 
 	bool clear()
 	{
 		if(p){
 			int r = shmdt(p);
 			if(r == -1) return false;
 		}
 		p = NULL;
 		return true;
 	}
 
+	bool resize(long size)
+	{
+		if(_size >= size) return true;
+		if(shmctl(shmid,IPC_RMID,NULL) != 0) return false;
+
+		int newshmid = shmget(key,size,IPC_CREAT|IPC_EXCL|0666);
+		char* newptr = (char*)shmat(newshmid,0,0);
+		memcpy(newptr,p,_size);
+		shmdt(p);
+
+		memset(newptr + _size,0,size - _size);
+
+		_size = size;
+		p = newptr;
+		return true;
+	}
+
+	unsigned long size()
+	{
+		return _size;
+	}
+
 	bool static remove(key_t key)
 	{
 		int shmid = shmget(key,0,0);
 		if(shmid){
 			return shmctl(shmid,IPC_RMID,NULL) == 0;
 		}
 		return false;
```

### Comparing `sharedmap-1.0.5/native/rbtree.cpp` & `sharedmap-1.0.6/native/rbtree.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.5/native/rbtree.h` & `sharedmap-1.0.6/native/rbtree.h`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.5/native/stringbox.cpp` & `sharedmap-1.0.6/native/stringbox.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.5/native/stringbox.h` & `sharedmap-1.0.6/native/stringbox.h`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.5/native/tree.cpp` & `sharedmap-1.0.6/native/tree.cpp`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.5/native/tree.h` & `sharedmap-1.0.6/native/tree.h`

 * *Files identical despite different names*

### Comparing `sharedmap-1.0.5/setup.py` & `sharedmap-1.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 	with open("README.md", "r") as fh:
 		long_description = fh.read()
 except Exception as e:
 	long_description = "";
 
 
 setup (name = projname,
-	version = '1.0.5',
+	version = '1.0.6',
 	description = projname,
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	author = "lyramilk",
 	packages=[],
 	ext_modules = [module1],
 	data_files=include_files,
```

### Comparing `sharedmap-1.0.5/sharedmap.egg-info/PKG-INFO` & `sharedmap-1.0.6/sharedmap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharedmap
-Version: 1.0.5
+Version: 1.0.6
 Summary: sharedmap
 Home-page: UNKNOWN
 Author: lyramilk
 Author-email: lyramilk@qq.com
 License: Apache License 2.0
 Keywords: sharedmap,sharememory,rbtree,avltree
 Platform: UNKNOWN
```

