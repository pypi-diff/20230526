# Comparing `tmp/lifetimefitting-0.0.11.tar.gz` & `tmp/lifetimefitting-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifetimefitting-0.0.11.tar", last modified: Thu May 25 21:01:01 2023, max compression
+gzip compressed data, was "lifetimefitting-0.0.12.tar", last modified: Fri May 26 05:00:50 2023, max compression
```

## Comparing `lifetimefitting-0.0.11.tar` & `lifetimefitting-0.0.12.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:01:01.291925 lifetimefitting-0.0.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-25 21:00:47.000000 lifetimefitting-0.0.11/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-25 21:01:01.291925 lifetimefitting-0.0.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-25 21:00:47.000000 lifetimefitting-0.0.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:01:01.291925 lifetimefitting-0.0.11/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:01:01.291925 lifetimefitting-0.0.11/app/lifetimefitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:00:47.000000 lifetimefitting-0.0.11/app/lifetimefitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-05-25 21:00:47.000000 lifetimefitting-0.0.11/app/lifetimefitting/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-25 21:00:47.000000 lifetimefitting-0.0.11/app/lifetimefitting/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12256 2023-05-25 21:00:47.000000 lifetimefitting-0.0.11/app/lifetimefitting/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-25 21:00:47.000000 lifetimefitting-0.0.11/app/lifetimefitting/phd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:01:01.291925 lifetimefitting-0.0.11/app/lifetimefitting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-25 21:01:01.000000 lifetimefitting-0.0.11/app/lifetimefitting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-25 21:01:01.000000 lifetimefitting-0.0.11/app/lifetimefitting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:01:01.000000 lifetimefitting-0.0.11/app/lifetimefitting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-25 21:01:01.000000 lifetimefitting-0.0.11/app/lifetimefitting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 21:01:01.000000 lifetimefitting-0.0.11/app/lifetimefitting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:01:01.291925 lifetimefitting-0.0.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-25 21:00:47.000000 lifetimefitting-0.0.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:00:50.536514 lifetimefitting-0.0.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-26 05:00:39.000000 lifetimefitting-0.0.12/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-26 05:00:50.536514 lifetimefitting-0.0.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-26 05:00:39.000000 lifetimefitting-0.0.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:00:50.536514 lifetimefitting-0.0.12/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:00:50.536514 lifetimefitting-0.0.12/app/lifetimefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 05:00:39.000000 lifetimefitting-0.0.12/app/lifetimefitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-05-26 05:00:39.000000 lifetimefitting-0.0.12/app/lifetimefitting/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-26 05:00:39.000000 lifetimefitting-0.0.12/app/lifetimefitting/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-05-26 05:00:39.000000 lifetimefitting-0.0.12/app/lifetimefitting/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-26 05:00:39.000000 lifetimefitting-0.0.12/app/lifetimefitting/phd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:00:50.536514 lifetimefitting-0.0.12/app/lifetimefitting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-26 05:00:50.000000 lifetimefitting-0.0.12/app/lifetimefitting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-26 05:00:50.000000 lifetimefitting-0.0.12/app/lifetimefitting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 05:00:50.000000 lifetimefitting-0.0.12/app/lifetimefitting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-26 05:00:50.000000 lifetimefitting-0.0.12/app/lifetimefitting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 05:00:50.000000 lifetimefitting-0.0.12/app/lifetimefitting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 05:00:50.536514 lifetimefitting-0.0.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-26 05:00:39.000000 lifetimefitting-0.0.12/setup.py
```

### Comparing `lifetimefitting-0.0.11/LICENSE.md` & `lifetimefitting-0.0.12/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.11/PKG-INFO` & `lifetimefitting-0.0.12/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.11
+Version: 0.0.12
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.11/README.md` & `lifetimefitting-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.11/app/lifetimefitting/__main__.py` & `lifetimefitting-0.0.12/app/lifetimefitting/__main__.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.11/app/lifetimefitting/funcs.py` & `lifetimefitting-0.0.12/app/lifetimefitting/funcs.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.11/app/lifetimefitting/gui.py` & `lifetimefitting-0.0.12/app/lifetimefitting/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,23 +188,23 @@
         self.verticalLayout_11.addWidget(self.groupBox)
 
         self.retranslateUi(Form)
         QtCore.QMetaObject.connectSlotsByName(Form)
 
     def retranslateUi(self, Form):
         _translate = QtCore.QCoreApplication.translate
-        Form.setWindowTitle(_translate("Form", "Form"))
+        Form.setWindowTitle(_translate("Form", "Lifetime Fitting"))
         self.groupBox_4.setTitle(_translate("Form", "Input"))
         self.trf_browse.setText(_translate("Form", "Browse for TRF"))
         self.irf_browse.setText(_translate("Form", "Browse for IRF"))
         self.groupBox.setTitle(_translate("Form", "Fitting"))
         self.label.setText(_translate("Form", "Bin Width (ps)"))
         self.label_2.setText(_translate("Form", "Maximum Fitting Iterations"))
         self.label_5.setText(_translate("Form", "Offset for the Starting Bin"))
-        self.label_6.setText(_translate("Form", "Minimum Time (ns)"))
+        self.label_6.setText(_translate("Form", "Maximum Time to fit (ns)"))
         self.label_24.setText(_translate("Form", "Number of Decays to fit"))
         self.label_3.setText(_translate("Form", "Maximum Time to Plot (ns)"))
         self.logFit_widg.setText(_translate("Form", "Fit in Log Space"))
         self.plotIRF_widg.setText(_translate("Form", "Plot the IRF (This will not be aligned to anything)"))
         self.scaled_widg.setText(_translate("Form", "Plot the Decays scaled by Their Coefficients"))
         self.fit_button.setText(_translate("Form", "Fit"))
         self.label_4.setText(_translate("Form", "Output"))
```

### Comparing `lifetimefitting-0.0.11/app/lifetimefitting/phd.py` & `lifetimefitting-0.0.12/app/lifetimefitting/phd.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.11/app/lifetimefitting.egg-info/PKG-INFO` & `lifetimefitting-0.0.12/app/lifetimefitting.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.11
+Version: 0.0.12
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.11/setup.py` & `lifetimefitting-0.0.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "lifetimefitting",
-    version = "0.0.11",
+    version = "0.0.12",
     author = "Adrea Snow",
     author_email = "adrea.snow@gmail.com",
     description = "PicoHarp TCSPC lifetime fitting tool",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adreasnow/LifetimeFittingTool",
     classifiers = [
```

