# Comparing `tmp/dbpyman-0.1.212.tar.gz` & `tmp/dbpyman-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbpyman-0.1.212.tar", last modified: Thu May 25 12:16:45 2023, max compression
+gzip compressed data, was "dbpyman-0.1.22.tar", last modified: Fri May 26 20:03:06 2023, max compression
```

## Comparing `dbpyman-0.1.212.tar` & `dbpyman-0.1.22.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 12:16:45.103324 dbpyman-0.1.212/
--rw-rw-rw-   0        0        0     1091 2023-05-23 11:40:26.000000 dbpyman-0.1.212/LICENSE
--rw-rw-rw-   0        0        0     3936 2023-05-25 12:16:45.103324 dbpyman-0.1.212/PKG-INFO
--rw-rw-rw-   0        0        0     3345 2023-05-25 12:02:42.000000 dbpyman-0.1.212/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 12:16:45.089326 dbpyman-0.1.212/dbpyman.egg-info/
--rw-rw-rw-   0        0        0     3936 2023-05-25 12:16:45.000000 dbpyman-0.1.212/dbpyman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-25 12:16:45.000000 dbpyman-0.1.212/dbpyman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 12:16:45.000000 dbpyman-0.1.212/dbpyman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-25 12:16:45.000000 dbpyman-0.1.212/dbpyman.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 12:16:45.091326 dbpyman-0.1.212/py_discord_db_management/
--rw-rw-rw-   0        0        0        0 2023-05-23 11:40:26.000000 dbpyman-0.1.212/py_discord_db_management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:16:45.097324 dbpyman-0.1.212/py_discord_db_management/classes/
--rw-rw-rw-   0        0        0        0 2023-05-24 13:39:09.000000 dbpyman-0.1.212/py_discord_db_management/classes/__init__.py
--rw-rw-rw-   0        0        0     1560 2023-05-25 11:55:34.000000 dbpyman-0.1.212/py_discord_db_management/classes/column.py
--rw-rw-rw-   0        0        0     3134 2023-05-25 11:55:56.000000 dbpyman-0.1.212/py_discord_db_management/classes/database.py
--rw-rw-rw-   0        0        0     1043 2023-05-25 11:55:56.000000 dbpyman-0.1.212/py_discord_db_management/classes/table.py
--rw-rw-rw-   0        0        0      588 2023-05-24 14:18:46.000000 dbpyman-0.1.212/py_discord_db_management/dbpyman.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:16:45.101325 dbpyman-0.1.212/py_discord_db_management/views/
--rw-rw-rw-   0        0        0        0 2023-05-24 13:39:00.000000 dbpyman-0.1.212/py_discord_db_management/views/__init__.py
--rw-rw-rw-   0        0        0     3732 2023-05-25 12:16:22.000000 dbpyman-0.1.212/py_discord_db_management/views/table_add_data_view.py
--rw-rw-rw-   0        0        0     1448 2023-05-25 07:06:40.000000 dbpyman-0.1.212/py_discord_db_management/views/table_categories_view.py
--rw-rw-rw-   0        0        0      958 2023-05-25 07:22:38.000000 dbpyman-0.1.212/py_discord_db_management/views/table_overview_view.py
--rw-rw-rw-   0        0        0      579 2023-05-25 12:16:31.000000 dbpyman-0.1.212/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 12:16:45.104326 dbpyman-0.1.212/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 20:03:06.351717 dbpyman-0.1.22/
+-rw-rw-rw-   0        0        0     1091 2023-05-09 18:13:07.000000 dbpyman-0.1.22/LICENSE
+-rw-rw-rw-   0        0        0     3935 2023-05-26 20:03:06.350720 dbpyman-0.1.22/PKG-INFO
+-rw-rw-rw-   0        0        0     3345 2023-05-26 19:49:20.000000 dbpyman-0.1.22/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 20:03:06.336757 dbpyman-0.1.22/dbpyman.egg-info/
+-rw-rw-rw-   0        0        0     3935 2023-05-26 20:03:06.000000 dbpyman-0.1.22/dbpyman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-26 20:03:06.000000 dbpyman-0.1.22/dbpyman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 20:03:06.000000 dbpyman-0.1.22/dbpyman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-26 20:03:06.000000 dbpyman-0.1.22/dbpyman.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 20:03:06.339749 dbpyman-0.1.22/py_discord_db_management/
+-rw-rw-rw-   0        0        0        0 2023-05-09 18:05:53.000000 dbpyman-0.1.22/py_discord_db_management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:03:06.343740 dbpyman-0.1.22/py_discord_db_management/classes/
+-rw-rw-rw-   0        0        0        0 2023-05-24 17:07:59.000000 dbpyman-0.1.22/py_discord_db_management/classes/__init__.py
+-rw-rw-rw-   0        0        0     1385 2023-05-26 19:49:20.000000 dbpyman-0.1.22/py_discord_db_management/classes/column.py
+-rw-rw-rw-   0        0        0     2764 2023-05-26 20:02:37.000000 dbpyman-0.1.22/py_discord_db_management/classes/database.py
+-rw-rw-rw-   0        0        0     1234 2023-05-26 20:02:24.000000 dbpyman-0.1.22/py_discord_db_management/classes/table.py
+-rw-rw-rw-   0        0        0      588 2023-05-24 17:07:59.000000 dbpyman-0.1.22/py_discord_db_management/dbpyman.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:03:06.349722 dbpyman-0.1.22/py_discord_db_management/views/
+-rw-rw-rw-   0        0        0        0 2023-05-24 17:07:59.000000 dbpyman-0.1.22/py_discord_db_management/views/__init__.py
+-rw-rw-rw-   0        0        0     3732 2023-05-26 19:49:20.000000 dbpyman-0.1.22/py_discord_db_management/views/table_add_data_view.py
+-rw-rw-rw-   0        0        0     2917 2023-05-26 19:58:55.000000 dbpyman-0.1.22/py_discord_db_management/views/table_categories_view.py
+-rw-rw-rw-   0        0        0      958 2023-05-26 19:49:20.000000 dbpyman-0.1.22/py_discord_db_management/views/table_overview_view.py
+-rw-rw-rw-   0        0        0      578 2023-05-26 20:02:47.000000 dbpyman-0.1.22/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 20:03:06.351717 dbpyman-0.1.22/setup.cfg
```

### Comparing `dbpyman-0.1.212/LICENSE` & `dbpyman-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.212/PKG-INFO` & `dbpyman-0.1.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbpyman
-Version: 0.1.212
+Version: 0.1.22
 Summary: A package used to modify & view your MySQL database data dynamically
 Author-email: JanikCodes <janiksielaff@gmx.de>
 Project-URL: Homepage, https://github.com/JanikCodes/py_discord_db_management
 Project-URL: Bug Tracker, https://github.com/JanikCodes/py_discord_db_management/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dbpyman-0.1.212/README.md` & `dbpyman-0.1.22/README.md`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.212/dbpyman.egg-info/PKG-INFO` & `dbpyman-0.1.22/dbpyman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbpyman
-Version: 0.1.212
+Version: 0.1.22
 Summary: A package used to modify & view your MySQL database data dynamically
 Author-email: JanikCodes <janiksielaff@gmx.de>
 Project-URL: Homepage, https://github.com/JanikCodes/py_discord_db_management
 Project-URL: Bug Tracker, https://github.com/JanikCodes/py_discord_db_management/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dbpyman-0.1.212/dbpyman.egg-info/SOURCES.txt` & `dbpyman-0.1.22/dbpyman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.212/py_discord_db_management/classes/column.py` & `dbpyman-0.1.22/py_discord_db_management/classes/column.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,14 @@
         self.__null = null
         self.__key = key
         self.__default = default
         self.__extra = extra
 
         # variable that is used to attach values to that specific column
         self.__attached_data = None
-        self.__hidden = False
-
-    def get_hidden(self):
-        return self.__hidden
-
-    def set_hidden(self, new_visibility):
-        self.__hidden = new_visibility
 
     def set_attached_data(self, attached_data):
         # value is empty
         if not attached_data:
             self.__attached_data = self.__default
         else:
             self.__attached_data = attached_data
```

### Comparing `dbpyman-0.1.212/py_discord_db_management/classes/database.py` & `dbpyman-0.1.22/py_discord_db_management/classes/database.py`

 * *Files 24% similar despite different names*

```diff
@@ -43,27 +43,14 @@
         for table in self.tables:
             if table.get_table_name().lower() == table_name.lower():
                 # we found the table
                 table.set_hidden(True)
                 return
 
         warnings.warn(f"Couldn't find table with name: {table_name}")
-
-    def set_column_hidden(self, table_name, column_name):
-        for table in self.tables:
-            if table.get_table_name().lower() == table_name.lower():
-                # we found the table
-                for column in table.get_columns():
-                    if column.get_field().lower() == column_name.lower():
-                        # we found the column
-                        column.set_hidden(True)
-                        return
-
-                warnings.warn(f"Couldn't find column with name: {column_name}")
-        warnings.warn(f"Couldn't find table with name: {table_name}")
     def set_column_default_value(self, table_name, column_name, value):
         for table in self.tables:
             if table.get_table_name().lower() == table_name.lower():
                 # we found the table
                 for column in table.get_columns():
                     if column.get_field().lower() == column_name.lower():
                         # we found the column
@@ -80,9 +67,14 @@
 
         sql = f'INSERT INTO {table.get_table_name()} VALUES({val_str});'
 
         column_data = [column.get_attached_data() for column in columns]
         self.cursor.execute(sql, column_data)
         self.mydb.commit()
 
+    def remove_data_from_table(self, table, primary_key):
+        sql = f'DELETE FROM {table.get_table_name()} WHERE {table.get_primary_column().get_field()} = %s'
+        self.cursor.execute(sql, primary_key)
+        self.mydb.commit()
+
     def get_charset(self):
         return self.charset
```

### Comparing `dbpyman-0.1.212/py_discord_db_management/dbpyman.py` & `dbpyman-0.1.22/py_discord_db_management/dbpyman.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.212/py_discord_db_management/views/table_add_data_view.py` & `dbpyman-0.1.22/py_discord_db_management/views/table_add_data_view.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.212/py_discord_db_management/views/table_overview_view.py` & `dbpyman-0.1.22/py_discord_db_management/views/table_overview_view.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.212/pyproject.toml` & `dbpyman-0.1.22/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbpyman"
-version = "0.1.212"
+version = "0.1.22"
 authors = [
   { name="JanikCodes", email="janiksielaff@gmx.de" },
 ]
 description = "A package used to modify & view your MySQL database data dynamically"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

