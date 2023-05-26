# Comparing `tmp/spreadsheet-migrator-0.3.tar.gz` & `tmp/spreadsheet-migrator-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spreadsheet-migrator-0.3.tar", last modified: Fri May 26 14:27:53 2023, max compression
+gzip compressed data, was "spreadsheet-migrator-0.4.tar", last modified: Fri May 26 15:26:45 2023, max compression
```

## Comparing `spreadsheet-migrator-0.3.tar` & `spreadsheet-migrator-0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 14:27:53.538342 spreadsheet-migrator-0.3/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     1094 2023-05-25 14:35:20.000000 spreadsheet-migrator-0.3/LICENSE
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       95 2023-05-26 10:58:38.000000 spreadsheet-migrator-0.3/MANIFEST.in
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)    10047 2023-05-26 14:27:53.536339 spreadsheet-migrator-0.3/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     9928 2023-05-26 13:46:29.000000 spreadsheet-migrator-0.3/README.md
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       38 2023-05-26 14:27:53.538342 spreadsheet-migrator-0.3/setup.cfg
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      594 2023-05-26 14:22:06.000000 spreadsheet-migrator-0.3/setup.py
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 14:27:53.239525 spreadsheet-migrator-0.3/spreadsheet_migrator/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      387 2023-05-07 20:07:02.000000 spreadsheet-migrator-0.3/spreadsheet_migrator/__init__.py
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 14:27:53.351873 spreadsheet-migrator-0.3/spreadsheet_migrator/spreadsheet_migrator_lib/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      191 2023-03-29 14:56:36.000000 spreadsheet-migrator-0.3/spreadsheet_migrator/spreadsheet_migrator_lib/__init__.py
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 14:27:53.418143 spreadsheet-migrator-0.3/spreadsheet_migrator/spreadsheet_migrator_lib/logs/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-07 08:40:57.000000 spreadsheet-migrator-0.3/spreadsheet_migrator/spreadsheet_migrator_lib/logs/__init__.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      220 2023-04-20 07:50:40.000000 spreadsheet-migrator-0.3/spreadsheet_migrator/spreadsheet_migrator_lib/logs/cases_logs.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      225 2023-04-03 13:21:26.000000 spreadsheet-migrator-0.3/spreadsheet_migrator/spreadsheet_migrator_lib/logs/parameters_logs.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      220 2023-04-03 13:21:36.000000 spreadsheet-migrator-0.3/spreadsheet_migrator/spreadsheet_migrator_lib/logs/plans_logs.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      221 2023-04-03 13:21:18.000000 spreadsheet-migrator-0.3/spreadsheet_migrator/spreadsheet_migrator_lib/logs/suites_logs.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)    12358 2023-05-25 14:47:36.000000 spreadsheet-migrator-0.3/spreadsheet_migrator/spreadsheet_migrator_lib/parser.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     6173 2023-05-25 13:57:04.000000 spreadsheet-migrator-0.3/spreadsheet_migrator/spreadsheet_migrator_lib/service.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)    12695 2023-05-25 11:51:41.000000 spreadsheet-migrator-0.3/spreadsheet_migrator/spreadsheet_migrator_lib/testy_creator.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      100 2023-03-16 20:10:58.000000 spreadsheet-migrator-0.3/spreadsheet_migrator/spreadsheet_migrator_lib/testy_exception.py
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 14:27:53.172999 spreadsheet-migrator-0.3/spreadsheet_migrator/static/
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 14:27:53.175001 spreadsheet-migrator-0.3/spreadsheet_migrator/static/excel_parser/
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 14:27:53.513340 spreadsheet-migrator-0.3/spreadsheet_migrator/static/excel_parser/js/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)  3738283 2023-05-25 14:52:36.000000 spreadsheet-migrator-0.3/spreadsheet_migrator/static/excel_parser/js/index.js
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       34 2023-05-25 14:52:36.000000 spreadsheet-migrator-0.3/spreadsheet_migrator/static/excel_parser/js/mix-manifest.json
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 14:27:53.526340 spreadsheet-migrator-0.3/spreadsheet_migrator/templates/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      195 2023-05-07 15:01:57.000000 spreadsheet-migrator-0.3/spreadsheet_migrator/templates/spreadsheet_migrator_index.html
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      551 2023-05-07 22:17:30.000000 spreadsheet-migrator-0.3/spreadsheet_migrator/urls.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     1931 2023-05-22 20:32:22.000000 spreadsheet-migrator-0.3/spreadsheet_migrator/views.py
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 14:27:53.295526 spreadsheet-migrator-0.3/spreadsheet_migrator.egg-info/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)    10047 2023-05-26 14:27:53.000000 spreadsheet-migrator-0.3/spreadsheet_migrator.egg-info/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     1198 2023-05-26 14:27:53.000000 spreadsheet-migrator-0.3/spreadsheet_migrator.egg-info/SOURCES.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-05-26 14:27:53.000000 spreadsheet-migrator-0.3/spreadsheet_migrator.egg-info/dependency_links.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-05-26 14:27:52.000000 spreadsheet-migrator-0.3/spreadsheet_migrator.egg-info/not-zip-safe
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       16 2023-05-26 14:27:53.000000 spreadsheet-migrator-0.3/spreadsheet_migrator.egg-info/requires.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       21 2023-05-26 14:27:53.000000 spreadsheet-migrator-0.3/spreadsheet_migrator.egg-info/top_level.txt
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 15:26:45.664948 spreadsheet-migrator-0.4/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)     1094 2023-05-25 14:35:20.000000 spreadsheet-migrator-0.4/LICENSE
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       95 2023-05-26 10:58:38.000000 spreadsheet-migrator-0.4/MANIFEST.in
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)    10224 2023-05-26 15:26:45.660946 spreadsheet-migrator-0.4/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)    10106 2023-05-26 15:17:39.000000 spreadsheet-migrator-0.4/README.md
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       38 2023-05-26 15:26:45.664948 spreadsheet-migrator-0.4/setup.cfg
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      594 2023-05-26 15:25:27.000000 spreadsheet-migrator-0.4/setup.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 15:26:45.028402 spreadsheet-migrator-0.4/spreadsheet_migrator/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      387 2023-05-07 20:07:02.000000 spreadsheet-migrator-0.4/spreadsheet_migrator/__init__.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 15:26:45.272442 spreadsheet-migrator-0.4/spreadsheet_migrator/spreadsheet_migrator_lib/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      191 2023-03-29 14:56:36.000000 spreadsheet-migrator-0.4/spreadsheet_migrator/spreadsheet_migrator_lib/__init__.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 15:26:45.468944 spreadsheet-migrator-0.4/spreadsheet_migrator/spreadsheet_migrator_lib/logs/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-07 08:40:57.000000 spreadsheet-migrator-0.4/spreadsheet_migrator/spreadsheet_migrator_lib/logs/__init__.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      220 2023-04-20 07:50:40.000000 spreadsheet-migrator-0.4/spreadsheet_migrator/spreadsheet_migrator_lib/logs/cases_logs.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      225 2023-04-03 13:21:26.000000 spreadsheet-migrator-0.4/spreadsheet_migrator/spreadsheet_migrator_lib/logs/parameters_logs.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      220 2023-04-03 13:21:36.000000 spreadsheet-migrator-0.4/spreadsheet_migrator/spreadsheet_migrator_lib/logs/plans_logs.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      221 2023-04-03 13:21:18.000000 spreadsheet-migrator-0.4/spreadsheet_migrator/spreadsheet_migrator_lib/logs/suites_logs.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)    12358 2023-05-25 14:47:36.000000 spreadsheet-migrator-0.4/spreadsheet_migrator/spreadsheet_migrator_lib/parser.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)     6173 2023-05-25 13:57:04.000000 spreadsheet-migrator-0.4/spreadsheet_migrator/spreadsheet_migrator_lib/service.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)    12695 2023-05-25 11:51:41.000000 spreadsheet-migrator-0.4/spreadsheet_migrator/spreadsheet_migrator_lib/testy_creator.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      100 2023-03-16 20:10:58.000000 spreadsheet-migrator-0.4/spreadsheet_migrator/spreadsheet_migrator_lib/testy_exception.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 15:26:44.868433 spreadsheet-migrator-0.4/spreadsheet_migrator/static/
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 15:26:44.872435 spreadsheet-migrator-0.4/spreadsheet_migrator/static/excel_parser/
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 15:26:45.596944 spreadsheet-migrator-0.4/spreadsheet_migrator/static/excel_parser/js/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)  3738226 2023-05-26 15:23:58.000000 spreadsheet-migrator-0.4/spreadsheet_migrator/static/excel_parser/js/index.js
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       34 2023-05-26 15:25:25.000000 spreadsheet-migrator-0.4/spreadsheet_migrator/static/excel_parser/js/mix-manifest.json
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 15:26:45.640948 spreadsheet-migrator-0.4/spreadsheet_migrator/templates/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      195 2023-05-07 15:01:57.000000 spreadsheet-migrator-0.4/spreadsheet_migrator/templates/spreadsheet_migrator_index.html
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      551 2023-05-07 22:17:30.000000 spreadsheet-migrator-0.4/spreadsheet_migrator/urls.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)     1931 2023-05-22 20:32:22.000000 spreadsheet-migrator-0.4/spreadsheet_migrator/views.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-26 15:26:45.120400 spreadsheet-migrator-0.4/spreadsheet_migrator.egg-info/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)    10224 2023-05-26 15:26:44.000000 spreadsheet-migrator-0.4/spreadsheet_migrator.egg-info/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)     1198 2023-05-26 15:26:44.000000 spreadsheet-migrator-0.4/spreadsheet_migrator.egg-info/SOURCES.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-05-26 15:26:44.000000 spreadsheet-migrator-0.4/spreadsheet_migrator.egg-info/dependency_links.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-05-26 15:26:44.000000 spreadsheet-migrator-0.4/spreadsheet_migrator.egg-info/not-zip-safe
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       16 2023-05-26 15:26:44.000000 spreadsheet-migrator-0.4/spreadsheet_migrator.egg-info/requires.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       21 2023-05-26 15:26:44.000000 spreadsheet-migrator-0.4/spreadsheet_migrator.egg-info/top_level.txt
```

### Comparing `spreadsheet-migrator-0.3/LICENSE` & `spreadsheet-migrator-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spreadsheet-migrator-0.3/PKG-INFO` & `spreadsheet-migrator-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spreadsheet-migrator
-Version: 0.3
+Version: 0.4
 Summary: Plugin to migrate your data from spreadsheets
 Author: Daniel
 Author-email: danielsheh02@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Плагин для переноса данных из таблиц в систему TestY
@@ -23,15 +23,16 @@
     volumes:
         - ./reports:/tmp/testy_spreadsheet_reports
 
 ## Инструкция пользователя
 Для переноса данных в Testy из таблицы необходимо в форме
 генерации данных выбрать файл расширения .xlsx и выбрать
 соответствующие колонки с именами, описаниями и прочими атрибутами для
-сущностей. В случае если для обязательного атрибута сущности не
+сущностей. Таблицы обязательно должны содержать заголовок, либо необходимо оставить пустой первую строку.
+В случае если для обязательного атрибута сущности не
 указана колонка или значение в ячейке для обязательного атрибута отсутствует, а так же если
 сущность с такими же атрибутами уже существует в базе данных, она не будет создана. При успешном
 завершении переноса данных будет доступна ссылка на отчет о проделанной работе.
 
 ![Not found](https://drive.google.com/uc?id=1DO4_Ds8u7uXkZIiFA9uEHulygcIQML5A)
 
 ### Сьюты
```

### Comparing `spreadsheet-migrator-0.3/README.md` & `spreadsheet-migrator-0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     volumes:
         - ./reports:/tmp/testy_spreadsheet_reports
 
 ## Инструкция пользователя
 Для переноса данных в Testy из таблицы необходимо в форме
 генерации данных выбрать файл расширения .xlsx и выбрать
 соответствующие колонки с именами, описаниями и прочими атрибутами для
-сущностей. В случае если для обязательного атрибута сущности не
+сущностей. Таблицы обязательно должны содержать заголовок, либо необходимо оставить пустой первую строку.
+В случае если для обязательного атрибута сущности не
 указана колонка или значение в ячейке для обязательного атрибута отсутствует, а так же если
 сущность с такими же атрибутами уже существует в базе данных, она не будет создана. При успешном
 завершении переноса данных будет доступна ссылка на отчет о проделанной работе.
 
 ![Not found](https://drive.google.com/uc?id=1DO4_Ds8u7uXkZIiFA9uEHulygcIQML5A)
 
 ### Сьюты
```

### Comparing `spreadsheet-migrator-0.3/setup.py` & `spreadsheet-migrator-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='spreadsheet-migrator',
-    version='0.3',
+    version='0.4',
     author="Daniel",
     author_email="danielsheh02@gmail.com",
     description='Plugin to migrate your data from spreadsheets',
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     install_requires=[
```

### Comparing `spreadsheet-migrator-0.3/spreadsheet_migrator/spreadsheet_migrator_lib/parser.py` & `spreadsheet-migrator-0.4/spreadsheet_migrator/spreadsheet_migrator_lib/parser.py`

 * *Files identical despite different names*

### Comparing `spreadsheet-migrator-0.3/spreadsheet_migrator/spreadsheet_migrator_lib/service.py` & `spreadsheet-migrator-0.4/spreadsheet_migrator/spreadsheet_migrator_lib/service.py`

 * *Files identical despite different names*

### Comparing `spreadsheet-migrator-0.3/spreadsheet_migrator/spreadsheet_migrator_lib/testy_creator.py` & `spreadsheet-migrator-0.4/spreadsheet_migrator/spreadsheet_migrator_lib/testy_creator.py`

 * *Files identical despite different names*

### Comparing `spreadsheet-migrator-0.3/spreadsheet_migrator/static/excel_parser/js/index.js` & `spreadsheet-migrator-0.4/spreadsheet_migrator/static/excel_parser/js/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -43833,23 +43833,21 @@
                         for (var i = 1; i < fileRows.length; i++) {
                             _loop();
                         }
                         setShowTable(true);
                     };
                     var getExtension = function getExtension(filename) {
                         var parts = filename.split('.');
-                        console.log(parts);
                         return parts[parts.length - 1];
                     };
                     (0, react__WEBPACK_IMPORTED_MODULE_1__.useEffect)(function() {
                         if (filesSelected.length > 0) {
                             var ext = getExtension(filesSelected[0].name);
                             if (ext === "xlsx") {
                                 (0, read_excel_file__WEBPACK_IMPORTED_MODULE_7__["default"])(filesSelected[0]).then(function(fileRows) {
-                                    console.log(fileRows);
                                     fillDatasForTableInUi(fileRows);
                                 });
                             } else {
                                 setServerResponse({
                                     isOk: false,
                                     msg: "Данный формат файлов не поддерживается"
                                 });
```

### Comparing `spreadsheet-migrator-0.3/spreadsheet_migrator/urls.py` & `spreadsheet-migrator-0.4/spreadsheet_migrator/urls.py`

 * *Files identical despite different names*

### Comparing `spreadsheet-migrator-0.3/spreadsheet_migrator/views.py` & `spreadsheet-migrator-0.4/spreadsheet_migrator/views.py`

 * *Files identical despite different names*

### Comparing `spreadsheet-migrator-0.3/spreadsheet_migrator.egg-info/PKG-INFO` & `spreadsheet-migrator-0.4/spreadsheet_migrator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spreadsheet-migrator
-Version: 0.3
+Version: 0.4
 Summary: Plugin to migrate your data from spreadsheets
 Author: Daniel
 Author-email: danielsheh02@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Плагин для переноса данных из таблиц в систему TestY
@@ -23,15 +23,16 @@
     volumes:
         - ./reports:/tmp/testy_spreadsheet_reports
 
 ## Инструкция пользователя
 Для переноса данных в Testy из таблицы необходимо в форме
 генерации данных выбрать файл расширения .xlsx и выбрать
 соответствующие колонки с именами, описаниями и прочими атрибутами для
-сущностей. В случае если для обязательного атрибута сущности не
+сущностей. Таблицы обязательно должны содержать заголовок, либо необходимо оставить пустой первую строку.
+В случае если для обязательного атрибута сущности не
 указана колонка или значение в ячейке для обязательного атрибута отсутствует, а так же если
 сущность с такими же атрибутами уже существует в базе данных, она не будет создана. При успешном
 завершении переноса данных будет доступна ссылка на отчет о проделанной работе.
 
 ![Not found](https://drive.google.com/uc?id=1DO4_Ds8u7uXkZIiFA9uEHulygcIQML5A)
 
 ### Сьюты
```

### Comparing `spreadsheet-migrator-0.3/spreadsheet_migrator.egg-info/SOURCES.txt` & `spreadsheet-migrator-0.4/spreadsheet_migrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

