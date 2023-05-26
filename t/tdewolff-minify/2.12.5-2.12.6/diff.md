# Comparing `tmp/tdewolff-minify-2.12.5.tar.gz` & `tmp/tdewolff-minify-2.12.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdewolff-minify-2.12.5.tar", last modified: Thu Mar 16 17:19:58 2023, max compression
+gzip compressed data, was "tdewolff-minify-2.12.6.tar", last modified: Fri May 26 14:53:42 2023, max compression
```

## Comparing `tdewolff-minify-2.12.5.tar` & `tdewolff-minify-2.12.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-03-16 17:19:58.477876 tdewolff-minify-2.12.5/
--rw-r--r--   0 taco      (1000) users      (100)       87 2022-09-24 00:44:48.000000 tdewolff-minify-2.12.5/MANIFEST.in
--rw-r--r--   0 taco      (1000) users      (100)     1757 2023-03-16 17:19:58.477876 tdewolff-minify-2.12.5/PKG-INFO
--rw-r--r--   0 taco      (1000) users      (100)     1501 2022-08-30 23:02:13.000000 tdewolff-minify-2.12.5/README.md
--rw-r--r--   0 taco      (1000) users      (100)      144 2023-03-16 17:19:37.000000 tdewolff-minify-2.12.5/go.mod
--rw-r--r--   0 taco      (1000) users      (100)     2035 2023-03-16 17:19:37.000000 tdewolff-minify-2.12.5/go.sum
--rw-r--r--   0 taco      (1000) users      (100)     4818 2022-08-30 23:02:13.000000 tdewolff-minify-2.12.5/minify.c
--rw-r--r--   0 taco      (1000) users      (100)     5056 2022-09-23 23:53:52.000000 tdewolff-minify-2.12.5/minify.go
--rw-r--r--   0 taco      (1000) users      (100)      236 2022-09-23 17:18:06.000000 tdewolff-minify-2.12.5/minify.pyi
--rw-r--r--   0 taco      (1000) users      (100)        0 2022-09-23 16:09:33.000000 tdewolff-minify-2.12.5/py.typed
--rw-r--r--   0 taco      (1000) users      (100)       38 2023-03-16 17:19:58.477876 tdewolff-minify-2.12.5/setup.cfg
--rw-r--r--   0 taco      (1000) users      (100)     1356 2022-09-24 00:44:53.000000 tdewolff-minify-2.12.5/setup.py
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-03-16 17:19:58.477876 tdewolff-minify-2.12.5/tdewolff_minify.egg-info/
--rw-r--r--   0 taco      (1000) users      (100)     1757 2023-03-16 17:19:58.000000 tdewolff-minify-2.12.5/tdewolff_minify.egg-info/PKG-INFO
--rw-r--r--   0 taco      (1000) users      (100)      277 2023-03-16 17:19:58.000000 tdewolff-minify-2.12.5/tdewolff_minify.egg-info/SOURCES.txt
--rw-r--r--   0 taco      (1000) users      (100)        1 2023-03-16 17:19:58.000000 tdewolff-minify-2.12.5/tdewolff_minify.egg-info/dependency_links.txt
--rw-r--r--   0 taco      (1000) users      (100)        1 2023-03-16 17:19:58.000000 tdewolff-minify-2.12.5/tdewolff_minify.egg-info/not-zip-safe
--rw-r--r--   0 taco      (1000) users      (100)        7 2023-03-16 17:19:58.000000 tdewolff-minify-2.12.5/tdewolff_minify.egg-info/top_level.txt
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-05-26 14:53:42.543719 tdewolff-minify-2.12.6/
+-rw-r--r--   0 taco      (1000) users      (100)       87 2022-09-24 00:44:48.000000 tdewolff-minify-2.12.6/MANIFEST.in
+-rw-r--r--   0 taco      (1000) users      (100)     1741 2023-05-26 14:53:42.543719 tdewolff-minify-2.12.6/PKG-INFO
+-rw-r--r--   0 taco      (1000) users      (100)     1485 2023-05-26 14:39:15.000000 tdewolff-minify-2.12.6/README.md
+-rw-r--r--   0 taco      (1000) users      (100)      144 2023-05-26 14:51:39.000000 tdewolff-minify-2.12.6/go.mod
+-rw-r--r--   0 taco      (1000) users      (100)     1652 2023-05-26 14:51:39.000000 tdewolff-minify-2.12.6/go.sum
+-rw-r--r--   0 taco      (1000) users      (100)     4818 2022-08-30 23:02:13.000000 tdewolff-minify-2.12.6/minify.c
+-rw-r--r--   0 taco      (1000) users      (100)     5088 2023-05-26 14:52:13.000000 tdewolff-minify-2.12.6/minify.go
+-rw-r--r--   0 taco      (1000) users      (100)      236 2022-09-23 17:18:06.000000 tdewolff-minify-2.12.6/minify.pyi
+-rw-r--r--   0 taco      (1000) users      (100)        0 2022-09-23 16:09:33.000000 tdewolff-minify-2.12.6/py.typed
+-rw-r--r--   0 taco      (1000) users      (100)       38 2023-05-26 14:53:42.543719 tdewolff-minify-2.12.6/setup.cfg
+-rw-r--r--   0 taco      (1000) users      (100)     1356 2022-09-24 00:44:53.000000 tdewolff-minify-2.12.6/setup.py
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-05-26 14:53:42.543719 tdewolff-minify-2.12.6/tdewolff_minify.egg-info/
+-rw-r--r--   0 taco      (1000) users      (100)     1741 2023-05-26 14:53:42.000000 tdewolff-minify-2.12.6/tdewolff_minify.egg-info/PKG-INFO
+-rw-r--r--   0 taco      (1000) users      (100)      277 2023-05-26 14:53:42.000000 tdewolff-minify-2.12.6/tdewolff_minify.egg-info/SOURCES.txt
+-rw-r--r--   0 taco      (1000) users      (100)        1 2023-05-26 14:53:42.000000 tdewolff-minify-2.12.6/tdewolff_minify.egg-info/dependency_links.txt
+-rw-r--r--   0 taco      (1000) users      (100)        1 2023-05-26 14:53:42.000000 tdewolff-minify-2.12.6/tdewolff_minify.egg-info/not-zip-safe
+-rw-r--r--   0 taco      (1000) users      (100)        7 2023-05-26 14:53:42.000000 tdewolff-minify-2.12.6/tdewolff_minify.egg-info/top_level.txt
```

### Comparing `tdewolff-minify-2.12.5/PKG-INFO` & `tdewolff-minify-2.12.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdewolff-minify
-Version: 2.12.5
+Version: 2.12.6
 Summary: Go minifiers for web formats
 Home-page: https://github.com/tdewolff/minify
 Author: Taco de Wolff
 Author-email: tacodewolff@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
@@ -27,15 +27,15 @@
     'html-keep-default-attr-vals': False,
     'html-keep-document-tags': False,
     'html-keep-end-tags': False,
     'html-keep-whitespace': False,
     'html-keep-quotes': False,
     'js-precision': 0,
     'js-keep-var-names': False,
-    'js-no-nullish-operator': False,
+    'js-version': 0,
     'json-precision': 0,
     'json-keep-numbers': False,
     'svg-keep-comments': False,
     'svg-precision': 0,
     'xml-keep-whitespace': False,
 })
```

### Comparing `tdewolff-minify-2.12.5/README.md` & `tdewolff-minify-2.12.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'html-keep-default-attr-vals': False,
     'html-keep-document-tags': False,
     'html-keep-end-tags': False,
     'html-keep-whitespace': False,
     'html-keep-quotes': False,
     'js-precision': 0,
     'js-keep-var-names': False,
-    'js-no-nullish-operator': False,
+    'js-version': 0,
     'json-precision': 0,
     'json-keep-numbers': False,
     'svg-keep-comments': False,
     'svg-precision': 0,
     'xml-keep-whitespace': False,
 })
```

### Comparing `tdewolff-minify-2.12.5/go.sum` & `tdewolff-minify-2.12.6/go.sum`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 github.com/cheekybits/is v0.0.0-20150225183255-68e9c0620927/go.mod h1:h/aW8ynjgkuj+NQRlZcDbAbM1ORAbXjXX77sX7T289U=
 github.com/djherbis/atime v1.1.0/go.mod h1:28OF6Y8s3NQWwacXc5eZTsEsiMzp7LF8MbXE+XJPdBE=
-github.com/dustin/go-humanize v1.0.0/go.mod h1:HtrtbFcZ19U5GC7JDqmcUSB87Iq5E25KnS6fMYU6eOk=
 github.com/dustin/go-humanize v1.0.1/go.mod h1:Mu1zIs6XwVuF/gI1OepvI0qD18qycQx+mFykh5fBlto=
-github.com/fsnotify/fsnotify v1.5.4/go.mod h1:OVB6XrOHzAwXMpEM7uPOzcehqUV2UqJxmVXmkdnm1bU=
 github.com/fsnotify/fsnotify v1.6.0/go.mod h1:sl3t1tCWJFWoRz9R8WJCbQihKKwmorjAbSClcnxKAGw=
 github.com/matryer/try v0.0.0-20161228173917-9ac251b645a2/go.mod h1:0KeJpeMD6o+O4hW7qJOT7vyQPKrWmj26uf5wMc/IiIs=
 github.com/spf13/pflag v1.0.5/go.mod h1:McXfInJRrz4CZXVZOBLb0bTZqETkiAhM9Iw0y3An2Bg=
-github.com/tdewolff/minify/v2 v2.12.1 h1:zcjJTcO0uI+asdT+nd4TjXi3KUmVV/G2kxOKKrgKlGw=
-github.com/tdewolff/minify/v2 v2.12.1/go.mod h1:p5pwbvNs1ghbFED/ZW1towGsnnWwzvM8iz8l0eURi9g=
-github.com/tdewolff/minify/v2 v2.12.2 h1:AKIoVwJj/HgBm+d/fPqpEZ31EtCM5FJfJNGagdR9Ecg=
-github.com/tdewolff/minify/v2 v2.12.2/go.mod h1:p5pwbvNs1ghbFED/ZW1towGsnnWwzvM8iz8l0eURi9g=
 github.com/tdewolff/minify/v2 v2.12.5 h1:s2KDBt/D/3ayE3gcqQF8VIgTmYgkx+btuLvVAeePzZM=
 github.com/tdewolff/minify/v2 v2.12.5/go.mod h1:i8QXtVyL7Ddwc4I5gqzvgBqKlTMgMNTbiXaPO4Iqg+A=
-github.com/tdewolff/parse/v2 v2.6.3 h1:O5rshbkaRmpRtD7k2lG65bEJpcfUMNg5Cx2uRKWVsI8=
-github.com/tdewolff/parse/v2 v2.6.3/go.mod h1:woz0cgbLwFdtbjJu8PIKxhW05KplTFQkOdX78o+Jgrs=
+github.com/tdewolff/minify/v2 v2.12.6 h1:kw5FU0ErJyd7fs+TMojIlBvLyEjsN93wP1n8NUOs320=
+github.com/tdewolff/minify/v2 v2.12.6/go.mod h1:ZRKTheiOGyLSK8hOZWWv+YoJAECzDivNgAlVYDHp/Ws=
 github.com/tdewolff/parse/v2 v2.6.5 h1:lYvWBk55GkqKl0JJenGpmrgu/cPHQQ6/Mm1hBGswoGQ=
 github.com/tdewolff/parse/v2 v2.6.5/go.mod h1:woz0cgbLwFdtbjJu8PIKxhW05KplTFQkOdX78o+Jgrs=
-github.com/tdewolff/test v1.0.7 h1:8Vs0142DmPFW/bQeHRP3MV19m1gvndjUb1sn8yy74LM=
+github.com/tdewolff/parse/v2 v2.6.6 h1:Yld+0CrKUJaCV78DL1G2nk3C9lKrxyRTux5aaK/AkDo=
+github.com/tdewolff/parse/v2 v2.6.6/go.mod h1:woz0cgbLwFdtbjJu8PIKxhW05KplTFQkOdX78o+Jgrs=
 github.com/tdewolff/test v1.0.7/go.mod h1:6DAvZliBAAnD7rhVgwaM7DE5/d9NMOAJ09SqYqeK4QE=
-golang.org/x/sys v0.0.0-20220412211240-33da011f77ad/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
+github.com/tdewolff/test v1.0.9/go.mod h1:6DAvZliBAAnD7rhVgwaM7DE5/d9NMOAJ09SqYqeK4QE=
 golang.org/x/sys v0.0.0-20220908164124-27713097b956/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
+golang.org/x/sys v0.6.0/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
```

### Comparing `tdewolff-minify-2.12.5/minify.c` & `tdewolff-minify-2.12.6/minify.c`

 * *Files identical despite different names*

### Comparing `tdewolff-minify-2.12.5/minify.go` & `tdewolff-minify-2.12.6/minify.go`

 * *Files 5% similar despite different names*

```diff
@@ -77,16 +77,18 @@
 			htmlMinifier.KeepQuotes, err = strconv.ParseBool(vals[i])
 		case "js-precision":
 			var precision int64
 			precision, err = strconv.ParseInt(vals[i], 10, 64)
 			jsMinifier.Precision = int(precision)
 		case "js-keep-var-names":
 			jsMinifier.KeepVarNames, err = strconv.ParseBool(vals[i])
-		case "js-no-nullish-operator":
-			jsMinifier.NoNullishOperator, err = strconv.ParseBool(vals[i])
+		case "js-version":
+			var version int64
+			version, err = strconv.ParseInt(vals[i], 10, 64)
+			jsMinifier.Version = int(version)
 		case "json-precision":
 			var precision int64
 			precision, err = strconv.ParseInt(vals[i], 10, 64)
 			jsonMinifier.Precision = int(precision)
 		case "json-keep-numbers":
 			jsonMinifier.KeepNumbers, err = strconv.ParseBool(vals[i])
 		case "svg-keep-comments":
```

### Comparing `tdewolff-minify-2.12.5/setup.py` & `tdewolff-minify-2.12.6/setup.py`

 * *Files identical despite different names*

### Comparing `tdewolff-minify-2.12.5/tdewolff_minify.egg-info/PKG-INFO` & `tdewolff-minify-2.12.6/tdewolff_minify.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdewolff-minify
-Version: 2.12.5
+Version: 2.12.6
 Summary: Go minifiers for web formats
 Home-page: https://github.com/tdewolff/minify
 Author: Taco de Wolff
 Author-email: tacodewolff@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
@@ -27,15 +27,15 @@
     'html-keep-default-attr-vals': False,
     'html-keep-document-tags': False,
     'html-keep-end-tags': False,
     'html-keep-whitespace': False,
     'html-keep-quotes': False,
     'js-precision': 0,
     'js-keep-var-names': False,
-    'js-no-nullish-operator': False,
+    'js-version': 0,
     'json-precision': 0,
     'json-keep-numbers': False,
     'svg-keep-comments': False,
     'svg-precision': 0,
     'xml-keep-whitespace': False,
 })
```

