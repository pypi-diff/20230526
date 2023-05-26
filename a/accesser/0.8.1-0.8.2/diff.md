# Comparing `tmp/accesser-0.8.1.tar.gz` & `tmp/accesser-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accesser-0.8.1.tar", last modified: Sun Apr  9 13:04:10 2023, max compression
+gzip compressed data, was "accesser-0.8.2.tar", last modified: Fri May 26 03:10:02 2023, max compression
```

## Comparing `accesser-0.8.1.tar` & `accesser-0.8.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-09 13:04:10.321170 accesser-0.8.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35147 2023-01-25 05:10:28.000000 accesser-0.8.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3595 2023-04-09 13:04:10.321170 accesser-0.8.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3004 2023-04-09 13:00:08.000000 accesser-0.8.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-09 13:04:10.317170 accesser-0.8.1/accesser/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8334 2023-04-09 12:52:48.000000 accesser-0.8.1/accesser/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      110 2023-01-29 01:22:09.000000 accesser-0.8.1/accesser/__main__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6985 2023-04-02 08:16:41.000000 accesser-0.8.1/accesser/config.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2207 2023-04-02 08:09:43.000000 accesser-0.8.1/accesser/pac
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-09 13:04:10.321170 accesser-0.8.1/accesser/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-25 05:10:28.000000 accesser-0.8.1/accesser/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1937 2023-01-25 05:10:28.000000 accesser-0.8.1/accesser/utils/cert_verify.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3619 2023-01-28 13:43:50.000000 accesser-0.8.1/accesser/utils/certmanager.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4363 2023-01-25 05:10:28.000000 accesser-0.8.1/accesser/utils/importca.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      570 2023-01-25 09:11:59.000000 accesser-0.8.1/accesser/utils/log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      785 2023-04-01 14:10:46.000000 accesser-0.8.1/accesser/utils/setting.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1003 2023-01-30 05:39:03.000000 accesser-0.8.1/accesser/utils/sysproxy.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-09 13:04:10.317170 accesser-0.8.1/accesser.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3595 2023-04-09 13:04:10.000000 accesser-0.8.1/accesser.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      491 2023-04-09 13:04:10.000000 accesser-0.8.1/accesser.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-09 13:04:10.000000 accesser-0.8.1/accesser.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-04-09 13:04:10.000000 accesser-0.8.1/accesser.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       89 2023-04-09 13:04:10.000000 accesser-0.8.1/accesser.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-04-09 13:04:10.000000 accesser-0.8.1/accesser.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      916 2023-04-09 12:52:48.000000 accesser-0.8.1/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-09 13:04:10.321170 accesser-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:10:02.889395 accesser-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-26 03:09:52.000000 accesser-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-26 03:10:02.889395 accesser-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-26 03:09:52.000000 accesser-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:10:02.885395 accesser-0.8.2/accesser/
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/pac
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:10:02.889395 accesser-0.8.2/accesser/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/utils/cert_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/utils/certmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/utils/importca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/utils/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-26 03:09:52.000000 accesser-0.8.2/accesser/utils/sysproxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:10:02.885395 accesser-0.8.2/accesser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-26 03:10:02.000000 accesser-0.8.2/accesser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-26 03:10:02.000000 accesser-0.8.2/accesser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 03:10:02.000000 accesser-0.8.2/accesser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 03:10:02.000000 accesser-0.8.2/accesser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-26 03:10:02.000000 accesser-0.8.2/accesser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 03:10:02.000000 accesser-0.8.2/accesser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-26 03:09:52.000000 accesser-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 03:10:02.889395 accesser-0.8.2/setup.cfg
```

### Comparing `accesser-0.8.1/LICENSE` & `accesser-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `accesser-0.8.1/PKG-INFO` & `accesser-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accesser
-Version: 0.8.1
+Version: 0.8.2
 Summary: 🌏一个解决SNI RST导致维基百科、Pixiv等站点无法访问的工具 | A tool for solving SNI RST
 Author: URenko
 Project-URL: Homepage, https://github.com/URenko/Accesser
 Project-URL: Bug Tracker, https://github.com/URenko/Accesser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 [![](https://img.shields.io/github/release/URenko/Accesser.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/pypi/v/accesser)](https://pypi.org/project/accesser/)
 [![](https://img.shields.io/github/downloads/URenko/Accesser/total.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/github/license/URenko/Accesser.svg)](https://github.com/URenko/Accesser/blob/master/LICENSE)
 
 ## 使用
 ### 如果不知道什么是Python
-从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.1/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
+从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.2/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
 ### 如果已经安装了Python 3.10*或更高版本
 ```
 pip3 install -U accesser[doh]
 ```
 如果你不需要DNS-over-HTTPS，则可以不用带`[doh]`。
 
 然后通过如下命令启动：
```

### Comparing `accesser-0.8.1/README.md` & `accesser-0.8.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [![](https://img.shields.io/github/release/URenko/Accesser.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/pypi/v/accesser)](https://pypi.org/project/accesser/)
 [![](https://img.shields.io/github/downloads/URenko/Accesser/total.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/github/license/URenko/Accesser.svg)](https://github.com/URenko/Accesser/blob/master/LICENSE)
 
 ## 使用
 ### 如果不知道什么是Python
-从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.1/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
+从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.2/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
 ### 如果已经安装了Python 3.10*或更高版本
 ```
 pip3 install -U accesser[doh]
 ```
 如果你不需要DNS-over-HTTPS，则可以不用带`[doh]`。
 
 然后通过如下命令启动：
```

### Comparing `accesser-0.8.1/accesser/__init__.py` & `accesser-0.8.2/accesser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = '0.8.1'
+__version__ = '0.8.2'
 
 import os, sys
 import json
 import random
 import ssl
 import asyncio
 import traceback
```

### Comparing `accesser-0.8.1/accesser/config.toml` & `accesser-0.8.2/accesser/config.toml`

 * *Files 1% similar despite different names*

```diff
@@ -138,7 +138,8 @@
 ".wikinews.org" = "91.198.174.192"
 ".wikiversity.org" = "91.198.174.192"
 ".wiktionary.org" = "91.198.174.192"
 ".wikibooks.org" = "91.198.174.192"
 ".wikiyoyage.org" = "91.198.174.192"
 ".wikisource.org" = "91.198.174.192"
 ".wikidata.org" = "91.198.174.192"
+"exhentai.org" = "178.175.128.252"
```

### Comparing `accesser-0.8.1/accesser/pac` & `accesser-0.8.2/accesser/pac`

 * *Files 8% similar despite different names*

```diff
@@ -54,15 +54,22 @@
   "*://steamuserimages-a.akamaihd.net/*": 1,
   "*://*.amazon.co.jp/*": 1,
   "*://*onedrive.live.com/*": 1,
   "*://*.bbc.co.uk/*": 1,
   "*://*.bbci.co.uk/*": 1,
   "*://*.japantimes.co.jp/*": 1,
   "*://*.yahoo.co.jp/*": 1,
-  "*://*.cna.com.tw/*": 1
+  "*://*.cna.com.tw/*": 1,
+  "*://*.discord.com/*": 1,
+  "*://*.discordapp.com/*": 1,
+  "*://*.discord.gg/*": 1,
+  "*://images-ext-*.discordapp.net/*": 1,
+  "*://*.duckduckgo.com/*": 1,
+  "*://*.v2ex.com/*":1,
+  "*://*.twitch.tv/*":1
 };
 
 var proxy = "PROXY {{host}}:{{port}};";
 
 var direct = 'DIRECT;';
 
 var hasOwnProperty = Object.hasOwnProperty;
```

### Comparing `accesser-0.8.1/accesser/utils/cert_verify.py` & `accesser-0.8.2/accesser/utils/cert_verify.py`

 * *Files identical despite different names*

### Comparing `accesser-0.8.1/accesser/utils/certmanager.py` & `accesser-0.8.2/accesser/utils/certmanager.py`

 * *Files identical despite different names*

### Comparing `accesser-0.8.1/accesser/utils/importca.py` & `accesser-0.8.2/accesser/utils/importca.py`

 * *Files identical despite different names*

### Comparing `accesser-0.8.1/accesser/utils/log.py` & `accesser-0.8.2/accesser/utils/log.py`

 * *Files identical despite different names*

### Comparing `accesser-0.8.1/accesser/utils/setting.py` & `accesser-0.8.2/accesser/utils/setting.py`

 * *Files identical despite different names*

### Comparing `accesser-0.8.1/accesser/utils/sysproxy.py` & `accesser-0.8.2/accesser/utils/sysproxy.py`

 * *Files identical despite different names*

### Comparing `accesser-0.8.1/accesser.egg-info/PKG-INFO` & `accesser-0.8.2/accesser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accesser
-Version: 0.8.1
+Version: 0.8.2
 Summary: 🌏一个解决SNI RST导致维基百科、Pixiv等站点无法访问的工具 | A tool for solving SNI RST
 Author: URenko
 Project-URL: Homepage, https://github.com/URenko/Accesser
 Project-URL: Bug Tracker, https://github.com/URenko/Accesser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 [![](https://img.shields.io/github/release/URenko/Accesser.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/pypi/v/accesser)](https://pypi.org/project/accesser/)
 [![](https://img.shields.io/github/downloads/URenko/Accesser/total.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/github/license/URenko/Accesser.svg)](https://github.com/URenko/Accesser/blob/master/LICENSE)
 
 ## 使用
 ### 如果不知道什么是Python
-从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.1/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
+从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.2/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
 ### 如果已经安装了Python 3.10*或更高版本
 ```
 pip3 install -U accesser[doh]
 ```
 如果你不需要DNS-over-HTTPS，则可以不用带`[doh]`。
 
 然后通过如下命令启动：
```

### Comparing `accesser-0.8.1/pyproject.toml` & `accesser-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "accesser"
-version = "0.8.1"
+version = "0.8.2"
 authors = [
   { name="URenko" },
 ]
 description = "🌏一个解决SNI RST导致维基百科、Pixiv等站点无法访问的工具 | A tool for solving SNI RST"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

