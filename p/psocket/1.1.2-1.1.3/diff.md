# Comparing `tmp/psocket-1.1.2.tar.gz` & `tmp/psocket-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psocket-1.1.2.tar", last modified: Thu May 25 17:28:55 2023, max compression
+gzip compressed data, was "psocket-1.1.3.tar", last modified: Fri May 26 10:54:05 2023, max compression
```

## Comparing `psocket-1.1.2.tar` & `psocket-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-25 17:28:55.520525 psocket-1.1.2/
--rw-r--r--   0 c-pher     (502) staff       (20)     1074 2023-05-25 16:06:10.000000 psocket-1.1.2/LICENSE
--rw-r--r--   0 c-pher     (502) staff       (20)     3800 2023-05-25 17:28:55.520400 psocket-1.1.2/PKG-INFO
--rw-r--r--   0 c-pher     (502) staff       (20)     2997 2023-05-25 17:28:50.000000 psocket-1.1.2/README.md
-drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-25 17:28:55.519646 psocket-1.1.2/psocket/
--rw-r--r--   0 c-pher     (502) staff       (20)     6222 2023-05-25 17:28:50.000000 psocket-1.1.2/psocket/__init__.py
-drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-25 17:28:55.520231 psocket-1.1.2/psocket.egg-info/
--rw-r--r--   0 c-pher     (502) staff       (20)     3800 2023-05-25 17:28:55.000000 psocket-1.1.2/psocket.egg-info/PKG-INFO
--rw-r--r--   0 c-pher     (502) staff       (20)      200 2023-05-25 17:28:55.000000 psocket-1.1.2/psocket.egg-info/SOURCES.txt
--rw-r--r--   0 c-pher     (502) staff       (20)        1 2023-05-25 17:28:55.000000 psocket-1.1.2/psocket.egg-info/dependency_links.txt
--rw-r--r--   0 c-pher     (502) staff       (20)       15 2023-05-25 17:28:55.000000 psocket-1.1.2/psocket.egg-info/requires.txt
--rw-r--r--   0 c-pher     (502) staff       (20)        8 2023-05-25 17:28:55.000000 psocket-1.1.2/psocket.egg-info/top_level.txt
--rw-r--r--   0 c-pher     (502) staff       (20)       38 2023-05-25 17:28:55.520566 psocket-1.1.2/setup.cfg
--rw-r--r--   0 c-pher     (502) staff       (20)     1194 2023-05-25 17:28:50.000000 psocket-1.1.2/setup.py
+drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-26 10:54:05.919239 psocket-1.1.3/
+-rw-r--r--   0 c-pher     (502) staff       (20)     1074 2023-05-25 16:06:10.000000 psocket-1.1.3/LICENSE
+-rw-r--r--   0 c-pher     (502) staff       (20)     3912 2023-05-26 10:54:05.919114 psocket-1.1.3/PKG-INFO
+-rw-r--r--   0 c-pher     (502) staff       (20)     3109 2023-05-26 10:43:49.000000 psocket-1.1.3/README.md
+drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-26 10:54:05.918117 psocket-1.1.3/psocket/
+-rw-r--r--   0 c-pher     (502) staff       (20)     6455 2023-05-26 10:44:07.000000 psocket-1.1.3/psocket/__init__.py
+drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-26 10:54:05.918929 psocket-1.1.3/psocket.egg-info/
+-rw-r--r--   0 c-pher     (502) staff       (20)     3912 2023-05-26 10:54:05.000000 psocket-1.1.3/psocket.egg-info/PKG-INFO
+-rw-r--r--   0 c-pher     (502) staff       (20)      200 2023-05-26 10:54:05.000000 psocket-1.1.3/psocket.egg-info/SOURCES.txt
+-rw-r--r--   0 c-pher     (502) staff       (20)        1 2023-05-26 10:54:05.000000 psocket-1.1.3/psocket.egg-info/dependency_links.txt
+-rw-r--r--   0 c-pher     (502) staff       (20)       15 2023-05-26 10:54:05.000000 psocket-1.1.3/psocket.egg-info/requires.txt
+-rw-r--r--   0 c-pher     (502) staff       (20)        8 2023-05-26 10:54:05.000000 psocket-1.1.3/psocket.egg-info/top_level.txt
+-rw-r--r--   0 c-pher     (502) staff       (20)       38 2023-05-26 10:54:05.919282 psocket-1.1.3/setup.cfg
+-rw-r--r--   0 c-pher     (502) staff       (20)     1194 2023-05-26 10:25:33.000000 psocket-1.1.3/setup.py
```

### Comparing `psocket-1.1.2/LICENSE` & `psocket-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psocket-1.1.2/PKG-INFO` & `psocket-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psocket
-Version: 1.1.2
+Version: 1.1.3
 Summary: The cross-platform tool to work with remote connection using sockets
 Home-page: https://github.com/c-pher/PSocket.git
 Author: Andrey Komissarov
 Author-email: a.komisssarov@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -52,22 +52,28 @@
 
 client = SocketClient(host='172.16.0.48', port=3261)
 print(client)
 ```
 ```python
 from psocket import SocketClient
 
-client = SocketClient(host='172.16.0.48', port=3261, initialize=True)
+client = SocketClient(host='172.16.0.48', port=3261)
 print(client.send_command('<commands>'))
 ```
 
 ---
 
 ## Changelog
 
+##### 1.1.3 (26.05.2023)
+- Reading completion from the socket fixed
+- buffer size reduced to 4k
+- Logger extended
+- Refactoring
+
 ##### 1.1.2 (25.05.2023)
 - buffer size increased to 8k
 - debug log added
 
 ##### 1.1.1 (04.08.2022)
 
 - Detect command is completed by \n\n
```

### Comparing `psocket-1.1.2/README.md` & `psocket-1.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -31,22 +31,28 @@
 
 client = SocketClient(host='172.16.0.48', port=3261)
 print(client)
 ```
 ```python
 from psocket import SocketClient
 
-client = SocketClient(host='172.16.0.48', port=3261, initialize=True)
+client = SocketClient(host='172.16.0.48', port=3261)
 print(client.send_command('<commands>'))
 ```
 
 ---
 
 ## Changelog
 
+##### 1.1.3 (26.05.2023)
+- Reading completion from the socket fixed
+- buffer size reduced to 4k
+- Logger extended
+- Refactoring
+
 ##### 1.1.2 (25.05.2023)
 - buffer size increased to 8k
 - debug log added
 
 ##### 1.1.1 (04.08.2022)
 
 - Detect command is completed by \n\n
```

### Comparing `psocket-1.1.2/psocket/__init__.py` & `psocket-1.1.3/psocket/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     """Create socket and establish connect to service using tuple host+port"""
 
     greeting = None
 
     def __init__(self,
                  host: str,
                  port: int = 0,
-                 buffer_size: int = 8192,
+                 buffer_size: int = 4096,
                  initialize: bool = False,
                  logger_enabled: bool = True,
                  log_level: str = 'INFO',
                  connection_timeout: int = None):
         """Create and connect client to a remote host.
 
         :param host: Host IP
@@ -47,26 +47,31 @@
     def __getattr__(self, attr):
         self.logger.error(f'No such attribute ({attr}) error. Perhaps, object is not initialized.')
         raise AttributeError(f'SocketClient does not have specific attribute "{attr}"')
 
     def __str__(self):
         msg = (f'Host: {self.host}\n'
                f'Port: {self.port}\n'
+               f'Reading buffer size: {self.buffer_size}\n'
                f'Logger name: {self.logger.name}\n'
                f'Connection timeout: {self.connection_timeout}')
         return msg
 
     def connect(self, timeout: int = None):
         """Create connection
 
         :param timeout:
         :return:
         """
 
-        return socket.create_connection((self.host, self.port), timeout=timeout)
+        self.logger.debug(f'Connecting to the <{self.host}:{self.port}>')
+        conn = socket.create_connection((self.host, self.port), timeout=timeout)
+        self.logger.debug('Connection has been established')
+
+        return conn
 
     def is_socket_available(self,
                             port: int = 0,
                             host: str = None,
                             timeout: int = 5,
                             logger_enabled: bool = True) -> bool:
         """Check remote socket is available.
@@ -119,60 +124,60 @@
         """Send network command and receive response.
 
         :param cmd:
         """
 
         command = self._encode_command(cmd)
 
-        self.logger.info(f'{self.host:<14} | -> {cmd}')
+        self.logger.info(f'{self.host:<14} | -> <{cmd}>')
 
         try:
-            self.logger.debug('"Sendall" command')
             self.client.sendall(command)
 
-            response = self._receive_all()
+            response = self.receive_all()
 
             # Save the greeting message for the first time only
             if self.greeting is None:
-                self.logger.debug(f'Save "greetings": {response}')
+                self.logger.debug(f'Store "greetings": {response}')
                 self.greeting = response
 
             return response
         except AttributeError as err:
             self.logger.error(f'{self.host:<14} | {err}')
             raise err
 
-    def _receive_all(self, stop_signs: str = '\r\n\r\n'):
+    def receive_all(self, stop_signs: str = '\r\n\r\n'):
         """Get and decode socket response
 
         Args:
             buffer_size: 4096 by default
             stop_signs: Symbols which will stop socket reading
         """
 
         self.logger.debug(f'Start reading from socket.\n\t'
                           f'{self.buffer_size = }\n\t'
                           f'{stop_signs = }')
 
         data = bytearray()
 
-        self.logger.debug(f'{data = }')
+        self.logger.debug(f'Initial data: {data}')
 
         while True:
             chunk = self.client.recv(self.buffer_size)
-            self.logger.debug(f'{chunk = }')
+            self.logger.debug(f'Chunk ({len(chunk)}): {chunk}')
 
             data.extend(chunk)
 
-            if chunk.endswith(stop_signs.encode()):
-                self.logger.debug(f'End symbols ({stop_signs = }) detected. Stop reading from socket')
+            if data.endswith(stop_signs.encode()):
+                self.logger.debug(f'Reading response ran to completion. <{stop_signs = }> received.')
                 break
 
         self.logger.debug('Parse response: decode, strip and splitlines')
         response = data.decode().strip().splitlines()
+        self.logger.debug('Completed')
 
         self.logger.info(f'{self.host:<14} | <- {response}')
         return response
 
     def close_connection(self):
         self.client.close()
```

### Comparing `psocket-1.1.2/psocket.egg-info/PKG-INFO` & `psocket-1.1.3/psocket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psocket
-Version: 1.1.2
+Version: 1.1.3
 Summary: The cross-platform tool to work with remote connection using sockets
 Home-page: https://github.com/c-pher/PSocket.git
 Author: Andrey Komissarov
 Author-email: a.komisssarov@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -52,22 +52,28 @@
 
 client = SocketClient(host='172.16.0.48', port=3261)
 print(client)
 ```
 ```python
 from psocket import SocketClient
 
-client = SocketClient(host='172.16.0.48', port=3261, initialize=True)
+client = SocketClient(host='172.16.0.48', port=3261)
 print(client.send_command('<commands>'))
 ```
 
 ---
 
 ## Changelog
 
+##### 1.1.3 (26.05.2023)
+- Reading completion from the socket fixed
+- buffer size reduced to 4k
+- Logger extended
+- Refactoring
+
 ##### 1.1.2 (25.05.2023)
 - buffer size increased to 8k
 - debug log added
 
 ##### 1.1.1 (04.08.2022)
 
 - Detect command is completed by \n\n
```

### Comparing `psocket-1.1.2/setup.py` & `psocket-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='psocket',
-    version='1.1.2',
+    version='1.1.3',
     packages=['psocket'],
     url='https://github.com/c-pher/PSocket.git',
     license='MIT',
     author='Andrey Komissarov',
     author_email='a.komisssarov@gmail.com',
     description='The cross-platform tool to work with remote connection using sockets',
     long_description=long_description,
```

