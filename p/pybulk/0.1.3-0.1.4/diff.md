# Comparing `tmp/pybulk-0.1.3.tar.gz` & `tmp/pybulk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybulk-0.1.3.tar", last modified: Thu May  4 06:53:21 2023, max compression
+gzip compressed data, was "pybulk-0.1.4.tar", last modified: Fri May 26 06:31:07 2023, max compression
```

## Comparing `pybulk-0.1.3.tar` & `pybulk-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 06:52:55.000000 pybulk-0.1.3/
--rwxrwxrwx   0 root         (0) root         (0)     2854 2023-05-04 06:52:55.000000 pybulk-0.1.3/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 06:52:55.000000 pybulk-0.1.3/pybulk/
--rwxrwxrwx   0 root         (0) root         (0)     8939 2023-04-18 08:21:18.000000 pybulk-0.1.3/pybulk/base_db.py
--rwxrwxrwx   0 root         (0) root         (0)     7209 2023-04-18 09:08:08.000000 pybulk-0.1.3/pybulk/dbinterface.py
--rwxrwxrwx   0 root         (0) root         (0)      951 2023-05-04 06:52:06.000000 pybulk-0.1.3/pybulk/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 06:52:55.000000 pybulk-0.1.3/pybulk.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-04 06:52:55.000000 pybulk-0.1.3/pybulk.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)     2854 2023-05-04 06:52:55.000000 pybulk-0.1.3/pybulk.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-05-04 06:52:55.000000 pybulk-0.1.3/pybulk.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)      226 2023-05-04 06:52:55.000000 pybulk-0.1.3/pybulk.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-05-04 06:52:55.000000 pybulk-0.1.3/pybulk.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     1771 2023-04-25 10:08:41.000000 pybulk-0.1.3/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-04 06:52:55.000000 pybulk-0.1.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1059 2023-05-04 06:52:27.000000 pybulk-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:31:07.486927 pybulk-0.1.4/
+-rw-rw-rw-   0        0        0     1083 2023-05-18 07:24:56.000000 pybulk-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2519 2023-05-26 06:31:07.486927 pybulk-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1818 2023-05-18 07:24:56.000000 pybulk-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 06:31:07.475822 pybulk-0.1.4/pybulk/
+-rw-rw-rw-   0        0        0      951 2023-05-18 07:24:56.000000 pybulk-0.1.4/pybulk/__init__.py
+-rw-rw-rw-   0        0        0     9171 2023-05-26 03:55:01.000000 pybulk-0.1.4/pybulk/base_db.py
+-rw-rw-rw-   0        0        0     7221 2023-05-26 03:55:26.000000 pybulk-0.1.4/pybulk/dbinterface.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:31:07.484919 pybulk-0.1.4/pybulk.egg-info/
+-rw-rw-rw-   0        0        0     2519 2023-05-26 06:31:07.000000 pybulk-0.1.4/pybulk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-05-26 06:31:07.000000 pybulk-0.1.4/pybulk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 06:31:07.000000 pybulk-0.1.4/pybulk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-26 06:31:07.000000 pybulk-0.1.4/pybulk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-26 06:31:07.000000 pybulk-0.1.4/pybulk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 06:31:07.486927 pybulk-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1059 2023-05-26 02:56:21.000000 pybulk-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:31:07.485897 pybulk-0.1.4/test/
+-rw-rw-rw-   0        0        0      253 2023-05-26 03:56:32.000000 pybulk-0.1.4/test/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pybulk-0.1.3/pybulk/base_db.py` & `pybulk-0.1.4/pybulk/base_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,47 +12,49 @@
     s = s.replace("\\", "\\\\")
     return s
 
 
 class Database(object):
     is_sqllite = False
     def __init__(self, user=None, password=None, db=None, host='localhost', port=3306,
-            charset='utf8', sqllite_path=None, recycle=300, size=50):
+            charset='utf8', sqllite_path=None, recycle=300, size=50, timeout=20, interval=1):
         self.user = user
         self.pwd = password
         self.db = db
         self.host = host
         self.port = port
         self.charset = charset
         self.sqllite_path = sqllite_path
         self.recycle = recycle
         self.size = size
+        self.timeout = timeout
+        self.interval = interval
 
     def connect(self):
         connection = pymysql.connect(
                             host=self.host,
                             port=self.port,
                             user=self.user,
                             password=self.pwd,
                             db=self.db,
                             charset=self.charset,
                             cursorclass=pymysql.cursors.DictCursor)
         return connection
 
-    def excute_sql_once(self, connection, sql):
+    def execute_sql_once(self, connection, sql):
         with connection.cursor() as cursor:
             cursor.execute(sql)
             result = cursor.fetchall()
             connection.commit()
             return result
 
-    def excute_sql(self, sql):
+    def execute_sql(self, sql):
         connection = self.connect()
         try:
-            return self.excute_sql_once(connection, sql)
+            return self.execute_sql_once(connection, sql)
         finally:
             connection.close()
 
     def get_sql(self, parameters):
         if 'update' in parameters:
             sections = ['update']
             sections.append(parameters['update'])
@@ -208,31 +210,34 @@
         for x in range(5):
             try:
                 return self.engine.connect()
             except Exception as e:
                 pass
         return self.engine.connect()
 
-    def excute_sql_once(self, connection, sql):
+    def execute_sql_once(self, connection, sql):
         sql = sql.replace('%', '%%')
-        for x in range(5):
+        endtime = time.time() + self.timeout
+        while True:
             try:
                 result = connection.execute(sql)
                 if result.returns_rows:
                     return result.fetchall()
                 else:
                     return None
             except Exception as e:
                 if 'Lost connection to' in str(e) or 'MySQL server has gone away' in str(e):
-                    print(f'与数据库失去连接，第{x+1}次等待重试...')
-                    time.sleep(15)
+                    print(f'与数据库失去连接，等待重试...')
+                    time.sleep(self.interval)
                 else:
                     raise e
+            if time.time() > endtime:
+                raise Exception('数据库连接超时')
 
-    def excute_sql(self, sql):
+    def execute_sql(self, sql):
         connection = self.connect()
         try:
-            result = self.excute_sql_once(connection, sql)
+            result = self.execute_sql_once(connection, sql)
         finally:
             connection.close()
         return result
```

### Comparing `pybulk-0.1.3/pybulk/dbinterface.py` & `pybulk-0.1.4/pybulk/dbinterface.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                     'table': storage_type,
                     'values': datas[start:end],
                 }
                 if self.db.is_sqllite:
                     params['operator'] = 'insert'
                 sql = self.db.get_insert_sql(params, keys=keys)
                 try:
-                    self.db.excute_sql_once(conn, sql)
+                    self.db.execute_sql_once(conn, sql)
                 except Exception as e:
                     print(sql[:2500])
                     raise e
         finally:
             conn.close()
 
     def update_same_val(self, table, vals, ids, key='id', size=1000):
@@ -84,15 +84,15 @@
                     ids_txt = '","'.join(ids[start:end])
                     where_sql = f'where {key} in ("{ids_txt}")'
                 elif type(ids[0]) in (int, float):
                     ids_txt = ','.join((str(x)for x in ids[start:end]))
                     where_sql = f'where {key} in ({ids_txt})'
                 else:
                     raise Exception(f'update_same_val id type error:{ids[0]}')
-                self.db.excute_sql_once(conn, ' '.join(sql + [where_sql]))
+                self.db.execute_sql_once(conn, ' '.join(sql + [where_sql]))
         finally:
             conn.close()
 
     def update_data(self, storage_type, datas, key='id'):
         conn = self.db.connect()
         try:
             for _data in datas:
@@ -101,40 +101,40 @@
                     'set': _data,
                     'where':[
                         (key, 'equals', str(_data[key])),
                     ],
                 }
                 sql = self.db.get_sql(params)
                 try:
-                    self.db.excute_sql_once(conn, sql)
+                    self.db.execute_sql_once(conn, sql)
                 except Exception as e:
                     print(_data),
                     print(sql)
                     raise e
         finally:
             conn.close()
 
-    def excute_sql(self, sql):
+    def execute_sql(self, sql):
         '''
         执行一次SQL
         param:sql,SQL语句
         '''
-        return self.db.excute_sql(sql)
+        return self.db.execute_sql(sql)
 
     def sign_length(self, storage_type, sign='sign'):
         '''
         获取指定表sign字段的数量
         param：storage_type，表名
         '''
         params = {
             'select': ['count(%s)' %sign],
             'from': [storage_type],
         }
         sql = self.db.get_sql(params)
-        data = self.db.excute_sql(sql)
+        data = self.db.execute_sql(sql)
         return data[0][0]
 
     def get_signs_in_set(self, storage_type, sign='sign'):
         '''
         获取指定表所有sign字段内容
         param：storage_type，表名
         '''
@@ -143,50 +143,50 @@
         for pg in range(99999):
             sql = ' '.join((
                 'select %s' %sign,
                 'from %s' %storage_type,
                 'order by id',
                 'limit %d, %d' %(pg * limit, limit),
             ))
-            datas = self.db.excute_sql(sql)
+            datas = self.db.execute_sql(sql)
             if len(datas) == 0:
                 break
             for data in datas:
                 result.add(data[sign])
         return result
 
     def clean_table(self, table_name):
-        self.excute_sql('TRUNCATE %s' %table_name)
+        self.execute_sql('TRUNCATE %s' %table_name)
 
     def rename(self, old_name, new_name):
         '''
         重命名
         '''
         sql = '\n'.join((
             'ALTER TABLE `%s`' %old_name,
             'RENAME TO `%s`;' %new_name,
         ))
-        self.excute_sql(sql)
+        self.execute_sql(sql)
 
     def exist_table(self, table_name):
         '''
         检查表是否存在
         '''
         sql = f'show tables like "{table_name}"'
-        return True if len(self.excute_sql(sql)) > 0 else False
+        return True if len(self.execute_sql(sql)) > 0 else False
 
     def get_column_names(self, table_name):
         '''
         获取数据表的所有字段名称
         '''
         sql = ' '.join((
             'select column_name from information_schema.columns',
             f'where table_name="{table_name}"',
         ))
-        res = self.excute_sql(sql)
+        res = self.execute_sql(sql)
         try:
             return [x['column_name']for x in res]
         except Exception as e:
             return [x['COLUMN_NAME']for x in res]
 
     def get_same_keys(self, keys, table):
         '''
@@ -206,14 +206,14 @@
         
     def all_tb_name(self, db_name):
         sql = ' '.join((
             'select table_name',
             'from information_schema.tables',
             f'where table_schema="{db_name}"'
         ))
-        res = self.excute_sql(sql)
+        res = self.execute_sql(sql)
         return [x['table_name']for x in res]
     
     def close(self):
         pass
 
 CLS_NAME = DBInterface
```

### Comparing `pybulk-0.1.3/pybulk/__init__.py` & `pybulk-0.1.4/pybulk/__init__.py`

 * *Files identical despite different names*

### Comparing `pybulk-0.1.3/README.md` & `pybulk-0.1.4/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# PyBulk 🚀
-[简体中文](README_CN.md) | English
-
-PyBulk is a Python module that wraps PyMySQL to allow simple and fast bulk data insertion into databases. With PyBulk, you can insert thousands of records into a database table in just a few lines of code.
-
-PyBulk builds on top of the PyMySQL library and connection pool to efficiently reuse connections and minimize latency. It handles all the low-level details of executing multiple INSERT statements while protecting your database from overload.
-
-Some of the main features of PyBulk include:
-* **Simple API**: Insert bulk data with just a few function calls. No complicated setup required.
-* **Speed**: Leverages PyMySQL's connection pool to quickly insert thousands of records.
-* **Reliability**: Includes error handling and recovery mechanisms to handle transient database errors. Retries failed queries automatically.
-* **Support for REPLACE INTO**: Upsert support allows you to replace existing records in a table or insert new ones.
-* **Compatibility**: Works with MySQL, MariaDB and AWS RDS. Compatible with Python 2 and 3.
-
-PyBulk allows you to focus on your application's logic rather than spending time building infrastructure to handle database load. It is a robust but lightweight solution ideal for batch data processing applications. 
-## 💾 Installation
-
-```
-pip install pybulk
-```
-
-## 🔧 Usage:
-```
-import pybulk
-
-cfg = {
-'host': 'localhost',
-'port':  3306,
-'user':  'root',
-'password': 'root',
-'db': 'info',
-'charset': 'utf8',
-}
-
-db = pybulk.client(cfg)
-
-my_data = [
-{'name': 'Peter', 'age': 21,},
-{'name': 'Harry', 'age': 35,},
-{'name': 'Mark', 'age': 40,},
-]
-
-db.push_data('student', my_data, size=2000)
-
-# You can also run sql in pybulk like:
-
-data = db.excute_sql('select * from school')
+# PyBulk 🚀
+[简体中文](README_CN.md) | English
+
+PyBulk is a Python module that wraps PyMySQL to allow simple and fast bulk data insertion into databases. With PyBulk, you can insert thousands of records into a database table in just a few lines of code.
+
+PyBulk builds on top of the PyMySQL library and connection pool to efficiently reuse connections and minimize latency. It handles all the low-level details of executing multiple INSERT statements while protecting your database from overload.
+
+Some of the main features of PyBulk include:
+* **Simple API**: Insert bulk data with just a few function calls. No complicated setup required.
+* **Speed**: Leverages PyMySQL's connection pool to quickly insert thousands of records.
+* **Reliability**: Includes error handling and recovery mechanisms to handle transient database errors. Retries failed queries automatically.
+* **Support for REPLACE INTO**: Upsert support allows you to replace existing records in a table or insert new ones.
+* **Compatibility**: Works with MySQL, MariaDB and AWS RDS. Compatible with Python 2 and 3.
+
+PyBulk allows you to focus on your application's logic rather than spending time building infrastructure to handle database load. It is a robust but lightweight solution ideal for batch data processing applications. 
+## 💾 Installation
+
+```
+pip install pybulk
+```
+
+## 🔧 Usage:
+```
+import pybulk
+
+cfg = {
+'host': 'localhost',
+'port':  3306,
+'user':  'root',
+'password': 'root',
+'db': 'info',
+'charset': 'utf8',
+}
+
+db = pybulk.client(cfg)
+
+my_data = [
+{'name': 'Peter', 'age': 21,},
+{'name': 'Harry', 'age': 35,},
+{'name': 'Mark', 'age': 40,},
+]
+
+db.push_data('student', my_data, size=2000)
+
+# You can also run sql in pybulk like:
+
+data = db.excute_sql('select * from school')
 ```
```

### Comparing `pybulk-0.1.3/setup.py` & `pybulk-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
  
  
 setuptools.setup(
     name='pybulk',
-    version="0.1.3",
+    version="0.1.4",
     author="pengkailiao",
     author_email="pengkailiao@gmail.com",
     description="PyBulk is a Python module that to allow simple and fast bulk data insertion into databases",
     long_description=long_description, 
     long_description_content_type="text/markdown",
     url="https://github.com/MrLpk/pybulk",
     packages=setuptools.find_packages(),
```

