# Comparing `tmp/tracebloc_package-dev-0.3.9.tar.gz` & `tmp/tracebloc_package-dev-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.3.9.tar", last modified: Thu May 25 07:52:03 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.4.0.tar", last modified: Fri May 26 09:14:22 2023, max compression
```

## Comparing `tracebloc_package-dev-0.3.9.tar` & `tracebloc_package-dev-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-25 07:52:03.570465 tracebloc_package-dev-0.3.9/
--rw-r--r--   0 divyasingh   (501) staff       (20)     1048 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.3.9/LICENSE.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-05-25 07:52:03.570543 tracebloc_package-dev-0.3.9/PKG-INFO
--rw-r--r--   0 divyasingh   (501) staff       (20)      188 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.3.9/README.md
--rw-r--r--   0 divyasingh   (501) staff       (20)       78 2023-05-25 07:52:03.570940 tracebloc_package-dev-0.3.9/setup.cfg
--rw-r--r--   0 divyasingh   (501) staff       (20)      949 2023-05-25 07:51:03.000000 tracebloc_package-dev-0.3.9/setup.py
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-25 07:52:03.569141 tracebloc_package-dev-0.3.9/tracebloc_package/
--rw-r--r--   0 divyasingh   (501) staff       (20)       67 2023-03-16 07:45:22.000000 tracebloc_package-dev-0.3.9/tracebloc_package/__init__.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     5669 2023-05-19 09:01:53.000000 tracebloc_package-dev-0.3.9/tracebloc_package/check_parameters.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    20669 2023-05-25 06:32:21.000000 tracebloc_package-dev-0.3.9/tracebloc_package/functional_test.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    59111 2023-05-24 09:14:21.000000 tracebloc_package-dev-0.3.9/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     7100 2022-07-01 07:02:58.000000 tracebloc_package-dev-0.3.9/tracebloc_package/messages.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     8594 2023-05-25 06:18:17.000000 tracebloc_package-dev-0.3.9/tracebloc_package/upload.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    10152 2023-05-19 09:01:53.000000 tracebloc_package-dev-0.3.9/tracebloc_package/user.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     5839 2023-05-23 18:03:05.000000 tracebloc_package-dev-0.3.9/tracebloc_package/utils.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     3203 2022-06-09 14:39:28.000000 tracebloc_package-dev-0.3.9/tracebloc_package/weights.py
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-25 07:52:03.570306 tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/
--rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-05-25 07:52:03.000000 tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 divyasingh   (501) staff       (20)      591 2023-05-25 07:52:03.000000 tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-05-25 07:52:03.000000 tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-05-25 07:52:03.000000 tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 divyasingh   (501) staff       (20)      119 2023-05-25 07:52:03.000000 tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)       18 2023-05-25 07:52:03.000000 tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-26 09:14:22.374938 tracebloc_package-dev-0.4.0/
+-rw-r--r--   0 divyasingh   (501) staff       (20)     1048 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.4.0/LICENSE.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-05-26 09:14:22.374996 tracebloc_package-dev-0.4.0/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      188 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.4.0/README.md
+-rw-r--r--   0 divyasingh   (501) staff       (20)       78 2023-05-26 09:14:22.375195 tracebloc_package-dev-0.4.0/setup.cfg
+-rw-r--r--   0 divyasingh   (501) staff       (20)      949 2023-05-26 09:14:17.000000 tracebloc_package-dev-0.4.0/setup.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-26 09:14:22.373816 tracebloc_package-dev-0.4.0/tracebloc_package/
+-rw-r--r--   0 divyasingh   (501) staff       (20)       67 2023-03-16 07:45:22.000000 tracebloc_package-dev-0.4.0/tracebloc_package/__init__.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     5669 2023-05-19 09:01:53.000000 tracebloc_package-dev-0.4.0/tracebloc_package/check_parameters.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    20852 2023-05-26 09:12:37.000000 tracebloc_package-dev-0.4.0/tracebloc_package/functional_test.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    59111 2023-05-24 09:14:21.000000 tracebloc_package-dev-0.4.0/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     7100 2022-07-01 07:02:58.000000 tracebloc_package-dev-0.4.0/tracebloc_package/messages.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     8594 2023-05-25 06:18:17.000000 tracebloc_package-dev-0.4.0/tracebloc_package/upload.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    10203 2023-05-25 09:39:24.000000 tracebloc_package-dev-0.4.0/tracebloc_package/user.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     5839 2023-05-23 18:03:05.000000 tracebloc_package-dev-0.4.0/tracebloc_package/utils.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     3203 2022-06-09 14:39:28.000000 tracebloc_package-dev-0.4.0/tracebloc_package/weights.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-26 09:14:22.374816 tracebloc_package-dev-0.4.0/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-05-26 09:14:22.000000 tracebloc_package-dev-0.4.0/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      591 2023-05-26 09:14:22.000000 tracebloc_package-dev-0.4.0/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-05-26 09:14:22.000000 tracebloc_package-dev-0.4.0/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-05-26 09:14:22.000000 tracebloc_package-dev-0.4.0/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 divyasingh   (501) staff       (20)      119 2023-05-26 09:14:22.000000 tracebloc_package-dev-0.4.0/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)       18 2023-05-26 09:14:22.000000 tracebloc_package-dev-0.4.0/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.3.9/LICENSE.txt` & `tracebloc_package-dev-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.9/PKG-INFO` & `tracebloc_package-dev-0.4.0/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tracebloc_package-dev
-Version: 0.3.9
+Name: tracebloc-package-dev
+Version: 0.4.0
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `tracebloc_package-dev-0.3.9/setup.py` & `tracebloc_package-dev-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.3.9",
+    version="0.4.0",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.3.9/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.4.0/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.9/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.4.0/tracebloc_package/functional_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,17 @@
                 if linenum in remove_lines:
                     continue
                 else:
                     if self.framework == TENSORFLOW_FRAMEWORK:
                         if re.search(f"def {self.method_name}\(.*\)", fileline):
                             fileline = fileline.replace(str(self.method_name), "MyModel")
                         fileline = self.replace_vars(fileline)
+                    elif self.framework == PYTORCH_FRAMEWORK:
+                        if re.search(f"class {self.class_name}\(.*\)", fileline):
+                            fileline = fileline.replace(str(self.class_name), "MyModel")
                     edited_data.append(fileline)
             tmp_fp.writelines("\n".join(edited_data))
         tmp_fp.close()
 
     def get_imports(self, codelines):
         instructions = dis.get_instructions(codelines)
         instructions = [__ for __ in instructions]
@@ -254,16 +257,15 @@
     def load_model(self, filename, update_progress_bar=False):
         try:
             sys.path.append(self.tmp_file_path)
             self.model = SourceFileLoader(
                 f"{filename}", f"{self.tmp_file}"
             ).load_module()
             if self.framework == PYTORCH_FRAMEWORK:
-                class_ = getattr(self.model, self.class_name)
-                self.model = class_()
+                self.model = self.model.MyModel()
             if update_progress_bar:
                 self.progress_bar.update(1)
         except Exception as e:
             if self.message == "":
                 self.message = f"Error loading the model file, {str(e)}"
             raise
```

### Comparing `tracebloc_package-dev-0.3.9/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.4.0/tracebloc_package/linkModelDataSet.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.9/tracebloc_package/messages.py` & `tracebloc_package-dev-0.4.0/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.9/tracebloc_package/upload.py` & `tracebloc_package-dev-0.4.0/tracebloc_package/upload.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.9/tracebloc_package/user.py` & `tracebloc_package-dev-0.4.0/tracebloc_package/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,15 @@
                 f"{self.__url}check-model/",
                 headers=header,
                 data={
                     "datasetId": datasetId,
                     "modelName": self.__modelId,
                     "file_type": self.__ext,
                     "type": "linking_dataset",
+                    "framework": self.__framework,
                 },
             )
             if re.status_code == 403 or re.status_code == 400:
                 text = colored(
                     f"There is no dataset with ID: {datasetId} in your dataset table.\n"
                     f"Please check your dataset ID.",
                     "red",
```

### Comparing `tracebloc_package-dev-0.3.9/tracebloc_package/utils.py` & `tracebloc_package-dev-0.4.0/tracebloc_package/utils.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.9/tracebloc_package/weights.py` & `tracebloc_package-dev-0.4.0/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tracebloc-package-dev
-Version: 0.3.9
+Name: tracebloc_package-dev
+Version: 0.4.0
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `tracebloc_package-dev-0.3.9/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.4.0/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

