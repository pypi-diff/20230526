# Comparing `tmp/piwwwaterflow-0.1.5.tar.gz` & `tmp/piwwwaterflow-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwwwaterflow-0.1.5.tar", last modified: Mon May 22 06:30:33 2023, max compression
+gzip compressed data, was "piwwwaterflow-0.1.6.tar", last modified: Fri May 26 12:01:48 2023, max compression
```

## Comparing `piwwwaterflow-0.1.5.tar` & `piwwwaterflow-0.1.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.452219 piwwwaterflow-0.1.5/piwwwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/piwwwaterflow/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/piwwwaterflow/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/css/iepngfix.htc
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/piwwwaterflow/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/img/blank.gif
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/img/bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/img/icon-256.png
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/img/icon-32.png
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/img/piwaterflow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/img/play.png
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/img/shadow.gif
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/img/top.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/piwwwaterflow/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     9535 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/js/code.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/piwwwaterflow/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/webservice.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/piwwwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-22 06:30:33.000000 piwwwaterflow-0.1.5/piwwwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-22 06:30:33.000000 piwwwaterflow-0.1.5/piwwwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:30:33.000000 piwwwaterflow-0.1.5/piwwwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-22 06:30:33.000000 piwwwaterflow-0.1.5/piwwwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 06:30:33.000000 piwwwaterflow-0.1.5/piwwwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.299708 piwwwaterflow-0.1.6/piwwwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/piwwwaterflow/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/piwwwaterflow/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/css/iepngfix.htc
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/piwwwaterflow/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/img/blank.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/img/bottom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/img/icon-256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/img/icon-32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/img/piwaterflow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/img/play.png
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/img/shadow.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/img/top.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/piwwwaterflow/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/static/js/code.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/piwwwaterflow/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/webservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/piwwwaterflow/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/piwwwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-26 12:01:48.000000 piwwwaterflow-0.1.6/piwwwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 12:01:48.000000 piwwwaterflow-0.1.6/piwwwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:01:48.000000 piwwwaterflow-0.1.6/piwwwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-26 12:01:48.000000 piwwwaterflow-0.1.6/piwwwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 12:01:48.000000 piwwwaterflow-0.1.6/piwwwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:48.303708 piwwwaterflow-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:01:33.000000 piwwwaterflow-0.1.6/tests/__init__.py
```

### Comparing `piwwwaterflow-0.1.5/PKG-INFO` & `piwwwaterflow-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.1.5
+Version: 0.1.6
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.1.5/piwwwaterflow/static/css/iepngfix.htc` & `piwwwaterflow-0.1.6/piwwwaterflow/static/css/iepngfix.htc`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.5/piwwwaterflow/static/css/view.css` & `piwwwaterflow-0.1.6/piwwwaterflow/static/css/view.css`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 body
 {
-	background:#fffff;
-	font-family:"Lucida Grande", Tahoma, Arial, Verdana, sans-serif;
+	background: #ffffff;
+	font-family: "Lucida Grande", Tahoma, Arial, Verdana, sans-serif;
 	font-size: 3em;
 	margin:4px;
 	text-align:center;
 }
 
-
 @media (orientation: landscape) {
 body
 {
 	width:800px;
 	margin: 0 auto;
 }
 }
```

### Comparing `piwwwaterflow-0.1.5/piwwwaterflow/static/img/icon-256.png` & `piwwwaterflow-0.1.6/piwwwaterflow/static/img/icon-256.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.5/piwwwaterflow/static/img/icon-32.png` & `piwwwaterflow-0.1.6/piwwwaterflow/static/img/icon-32.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.5/piwwwaterflow/static/img/piwaterflow.svg` & `piwwwaterflow-0.1.6/piwwwaterflow/static/img/piwaterflow.svg`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.5/piwwwaterflow/static/img/play.png` & `piwwwaterflow-0.1.6/piwwwaterflow/static/img/play.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.5/piwwwaterflow/static/js/code.js` & `piwwwaterflow-0.1.6/piwwwaterflow/static/js/code.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -79,15 +79,15 @@
 }
 
 socket.on('connect', function() {
     update(true);
 });
 
 socket.on('disconnect', function() {
-    document.cookie = "token=; expires=Thu, 01 Jan 1970 00:00:00 UTC; ";
+    //document.cookie = "token=; expires=Thu, 01 Jan 1970 00:00:00 UTC; ";
     location.reload();
 });
 
 setInterval("update(false);", 30000);
 
 function update(first_time) {
     socket.emit('service_request', function service(response) {
```

### Comparing `piwwwaterflow-0.1.5/piwwwaterflow/templates/form.html` & `piwwwaterflow-0.1.6/piwwwaterflow/templates/form.html`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.5/piwwwaterflow/webservice.py` & `piwwwaterflow-0.1.6/piwwwaterflow/webservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.waterflow = Waterflow()
 
         self.app = Flask(__name__,  template_folder=template_folder, static_folder=static_folder)
         self.revproxy_auth = RevProxyAuth(self.app, root_class='piwwwaterflow')
 
         self.app.add_url_rule('/', 'index', self.waterflow_endpoint, methods=['GET', 'POST'])
         Compress(self.app)
-        self.socketio = SocketIO(self.app)
+        self.socketio = SocketIO(self.app, cors_allowed_origins='*')
         self.socketio.on_event('service_request', self.on_service_request)
         self.socketio.on_event('force', self.on_force)
         self.socketio.on_event('stop', self.on_stop)
         self.socketio.on_event('save', self.on_save)
 
     def get_app(self):
         """ Returns WSGI app
```

### Comparing `piwwwaterflow-0.1.5/piwwwaterflow/wsgi.py` & `piwwwaterflow-0.1.6/piwwwaterflow/wsgi.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     """
     wtf_service = create_service()
     return wtf_service.get_app()
 
 # __main__ used for standalone execution (debugging). For WSGI call, the "wsgi:create_app()" function should be called
 if __name__ == '__main__':
     service = create_service()
-    service.get_socket_app().run(service.app, host='0.0.0.0', port=5000, debug=True, use_reloader=False)
+    service.socketio.run(service.app, host='0.0.0.0', port=5000, debug=True, use_reloader=False)
```

### Comparing `piwwwaterflow-0.1.5/piwwwaterflow.egg-info/PKG-INFO` & `piwwwaterflow-0.1.6/piwwwaterflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.1.5
+Version: 0.1.6
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.1.5/piwwwaterflow.egg-info/SOURCES.txt` & `piwwwaterflow-0.1.6/piwwwaterflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.5/setup.py` & `piwwwaterflow-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="piwwwaterflow",
-    version="0.1.5",
+    version="0.1.6",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Waterflow resilient system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/piwwwaterflow",
     packages=setuptools.find_packages(),
@@ -25,11 +25,11 @@
         'Flask>=1.1.2',
         'flask-compress>=1.9.0',
         'importlib-metadata>=4.5.0',
         'python-socketio>=5.8.0',
         'flask-socketio>=5.3.3',
         'eventlet>=0.33.3',
         'piwaterflow>=0.5.4',
-        'revproxy_auth>=0.1.1'
+        'revproxy_auth>=0.1.6'
     ],
     python_requires='>=3.6',
 )
```

