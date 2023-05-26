# Comparing `tmp/kynaylibs-1.8.1.tar.gz` & `tmp/kynaylibs-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kynaylibs-1.8.1.tar", last modified: Tue May 23 19:29:19 2023, max compression
+gzip compressed data, was "kynaylibs-1.8.2.tar", last modified: Fri May 26 19:32:26 2023, max compression
```

## Comparing `kynaylibs-1.8.1.tar` & `kynaylibs-1.8.2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:29:19.521743 kynaylibs-1.8.1/
--rw-r--r--   0 root         (0) root         (0)     2701 2023-05-23 19:29:19.521743 kynaylibs-1.8.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:29:19.509743 kynaylibs-1.8.1/kynaylibs/
--rw-r--r--   0 root         (0) root         (0)     1387 2023-05-23 19:29:08.000000 kynaylibs-1.8.1/kynaylibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:29:19.513743 kynaylibs-1.8.1/kynaylibs/nan/
--rw-r--r--   0 root         (0) root         (0)     1737 2023-05-22 01:04:55.000000 kynaylibs-1.8.1/kynaylibs/nan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-05-22 01:04:55.000000 kynaylibs-1.8.1/kynaylibs/nan/load.py
--rw-r--r--   0 root         (0) root         (0)      890 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:29:19.521743 kynaylibs-1.8.1/kynaylibs/nan/utils/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/PyroHelpers.py
--rw-r--r--   0 root         (0) root         (0)      371 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/adminHelpers.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/ai.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/aiohttp_helper.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/basic.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:29:19.521743 kynaylibs-1.8.1/kynaylibs/nan/utils/db/
--rw-r--r--   0 root         (0) root         (0)    13461 2023-05-23 13:40:32.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/db/permit.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/function.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/get_id.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/http.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-05-22 22:41:21.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/inline.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/interval.py
--rw-r--r--   0 root         (0) root         (0)     3620 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/parser.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/pilter.py
--rw-r--r--   0 root         (0) root         (0)    17772 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/unpack.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/kynaylibs/nan/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-23 19:29:08.000000 kynaylibs-1.8.1/kynaylibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:29:19.513743 kynaylibs-1.8.1/kynaylibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2701 2023-05-23 19:29:19.000000 kynaylibs-1.8.1/kynaylibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      931 2023-05-23 19:29:19.000000 kynaylibs-1.8.1/kynaylibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 19:29:19.000000 kynaylibs-1.8.1/kynaylibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-05-23 19:29:19.000000 kynaylibs-1.8.1/kynaylibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-23 19:29:19.000000 kynaylibs-1.8.1/kynaylibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 19:29:19.521743 kynaylibs-1.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1547 2023-05-21 22:20:35.000000 kynaylibs-1.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 19:32:26.852164 kynaylibs-1.8.2/
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-26 19:32:26.852164 kynaylibs-1.8.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 19:32:26.844164 kynaylibs-1.8.2/kynaylibs/
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-05-23 19:29:08.000000 kynaylibs-1.8.2/kynaylibs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 19:32:26.844164 kynaylibs-1.8.2/kynaylibs/nan/
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-05-22 01:04:55.000000 kynaylibs-1.8.2/kynaylibs/nan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-05-22 01:04:55.000000 kynaylibs-1.8.2/kynaylibs/nan/load.py
+-rw-r--r--   0 root         (0) root         (0)      890 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 19:32:26.852164 kynaylibs-1.8.2/kynaylibs/nan/utils/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/PyroHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/adminHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/ai.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/aiohttp_helper.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/basic.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 19:32:26.852164 kynaylibs-1.8.2/kynaylibs/nan/utils/db/
+-rw-r--r--   0 root         (0) root         (0)    14257 2023-05-26 19:30:03.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-05-26 19:30:03.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/db/permit.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/function.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/get_id.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/http.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-05-22 22:41:21.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/inline.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/interval.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/pilter.py
+-rw-r--r--   0 root         (0) root         (0)    17772 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/unpack.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/kynaylibs/nan/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-26 19:30:03.000000 kynaylibs-1.8.2/kynaylibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 19:32:26.844164 kynaylibs-1.8.2/kynaylibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-26 19:32:26.000000 kynaylibs-1.8.2/kynaylibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      939 2023-05-26 19:32:26.000000 kynaylibs-1.8.2/kynaylibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 19:32:26.000000 kynaylibs-1.8.2/kynaylibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-05-26 19:32:26.000000 kynaylibs-1.8.2/kynaylibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-26 19:32:26.000000 kynaylibs-1.8.2/kynaylibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 19:32:26.852164 kynaylibs-1.8.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-05-21 22:20:35.000000 kynaylibs-1.8.2/setup.py
```

### Comparing `kynaylibs-1.8.1/PKG-INFO` & `kynaylibs-1.8.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 1.8.1
+Version: 1.8.2
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
 Project-URL: Source Code, https://github.com/naya1503/kynaylibs
-Description: # Kynanlibs Library
-        
-        Core library of [Naya-Pyro](https://github.com/naya1503/Naya-Pyro), a python based telegram userbot.
-        
-        [![CodeFactor](https://www.codefactor.io/repository/github/naya1503/kynaylibs/badge)](https://www.codefactor.io/repository/github/naya1503/kynaylibs)
-        [![PyPI - Version](https://img.shields.io/pypi/v/py-Naya-Pyro?style=round)](https://pypi.org/project/kynaylibs)    
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/py-Naya-Pyro?label=DOWNLOADS&style=round)](https://pypi.org/project/kynaylibs)    
-        [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/naya1503/Naya-Pyro/graphs/commit-activity)
-        [![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/naya1503/Naya-Pyro)
-        [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
-        
-        # Installation
-        ```bash
-        pip3 install -U py-Ayra
-        ```
-        
-        # Documentation 
-        [![Documentation](https://img.shields.io/badge/Documentation-kynaylibs-blue)](http://ayra.tech/)
-        
-        
-        
-        See more working plugins on [the offical repository](https://github.com/naya1503/Naya-Pyro)!
-        
-        > Made with 💕 by [Kynan](https://t.me/Rizzvbss).    
-        
-        
-        # License
-        [![License](https://www.gnu.org/graphics/agplv3-155x51.png)](LICENSE)   
-        Ultroid is licensed under [GNU Affero General Public License](https://www.gnu.org/licenses/agpl-3.0.en.html) v3 or later.
-        
-        # Credits
-        * [![Kynan-Devs](https://img.shields.io/static/v1?label=Kynan&message=devs&color=critical)](https://t.me/Rizzvbss)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.7, <3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Kynanlibs Library
+
+Core library of [Naya-Pyro](https://github.com/naya1503/Naya-Pyro), a python based telegram userbot.
+
+[![CodeFactor](https://www.codefactor.io/repository/github/naya1503/kynaylibs/badge)](https://www.codefactor.io/repository/github/naya1503/kynaylibs)
+[![PyPI - Version](https://img.shields.io/pypi/v/py-Naya-Pyro?style=round)](https://pypi.org/project/kynaylibs)    
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/py-Naya-Pyro?label=DOWNLOADS&style=round)](https://pypi.org/project/kynaylibs)    
+[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/naya1503/Naya-Pyro/graphs/commit-activity)
+[![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/naya1503/Naya-Pyro)
+[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
+
+# Installation
+```bash
+pip3 install -U py-Ayra
+```
+
+# Documentation 
+[![Documentation](https://img.shields.io/badge/Documentation-kynaylibs-blue)](http://ayra.tech/)
+
+
+
+See more working plugins on [the offical repository](https://github.com/naya1503/Naya-Pyro)!
+
+> Made with 💕 by [Kynan](https://t.me/Rizzvbss).    
+
+
+# License
+[![License](https://www.gnu.org/graphics/agplv3-155x51.png)](LICENSE)   
+Ultroid is licensed under [GNU Affero General Public License](https://www.gnu.org/licenses/agpl-3.0.en.html) v3 or later.
+
+# Credits
+* [![Kynan-Devs](https://img.shields.io/static/v1?label=Kynan&message=devs&color=critical)](https://t.me/Rizzvbss)
+
```

### Comparing `kynaylibs-1.8.1/README.md` & `kynaylibs-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/__init__.py` & `kynaylibs-1.8.2/kynaylibs/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/__init__.py` & `kynaylibs-1.8.2/kynaylibs/nan/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/load.py` & `kynaylibs-1.8.2/kynaylibs/nan/load.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/log.py` & `kynaylibs-1.8.2/kynaylibs/nan/log.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/PyroHelpers.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/adminHelpers.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/ai.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/ai.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/aiohttp_helper.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/basic.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/basic.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/constants.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/constants.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/db/__init__.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/db/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 usersdb = db.users
 logdb = db.gruplog
 blchatdb = db.blchat
 pmdb = db.pmpermit
 afkdb = db.afk
 resell = db.seles
 expdb = db.expired
+vardb = db.variable
 sudoersdb = db.sudoers
 
 MSG_ON = """
 **Naya Premium Actived ✅**
 ╼┅━━━━━━━━━━╍━━━━━━━━━━┅╾
 ◉ **Versi** : `{}`
 ◉ **Phython** : `{}`
@@ -137,14 +138,42 @@
 
     if botlog_chat_id is None:
         return None
 
     return int(botlog_chat_id)
 
 
+async def set_var(user_id, var, value):
+    vari = await vardb.find_one({"user_id": user_id, "var": var})
+    if vari:
+        await vardb.update_one(
+            {"user_id": user_id, "var": var}, {"$set": {"vardb": value}}
+        )
+    else:
+        await vardb.insert_one({"user_id": user_id, "var": var, "vardb": value})
+
+
+async def get_var(user_id, var):
+    cosvar = await vardb.find_one({"user_id": user_id, "var": var})
+    if not cosvar:
+        return None
+    else:
+        get_cosvar = cosvar["vardb"]
+        return get_cosvar
+
+
+async def del_var(user_id, var):
+    cosvar = await vardb.find_one({"user_id": user_id, "var": var})
+    if cosvar:
+        await vardb.delete_one({"user_id": user_id, "var": var})
+        return True
+    else:
+        return False
+
+
 async def get_botlog(user_id: int):
     user_data = await logdb.users.find_one({"user_id": user_id})
     botlog_chat_id = user_data.get("bot_log_group_id") if user_data else None
     return botlog_chat_id
 
 
 async def set_botlog(user_id: int, botlog_chat_id: int):
```

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/function.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/function.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/get_id.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/get_id.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/http.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/http.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/inline.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/inline.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/interval.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/interval.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/misc.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/parser.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/parser.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/pilter.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/tools.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/tools.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/unpack.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs/nan/utils/utility.py` & `kynaylibs-1.8.2/kynaylibs/nan/utils/utility.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.1/kynaylibs.egg-info/PKG-INFO` & `kynaylibs-1.8.2/kynaylibs.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 1.8.1
+Version: 1.8.2
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
 Project-URL: Source Code, https://github.com/naya1503/kynaylibs
-Description: # Kynanlibs Library
-        
-        Core library of [Naya-Pyro](https://github.com/naya1503/Naya-Pyro), a python based telegram userbot.
-        
-        [![CodeFactor](https://www.codefactor.io/repository/github/naya1503/kynaylibs/badge)](https://www.codefactor.io/repository/github/naya1503/kynaylibs)
-        [![PyPI - Version](https://img.shields.io/pypi/v/py-Naya-Pyro?style=round)](https://pypi.org/project/kynaylibs)    
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/py-Naya-Pyro?label=DOWNLOADS&style=round)](https://pypi.org/project/kynaylibs)    
-        [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/naya1503/Naya-Pyro/graphs/commit-activity)
-        [![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/naya1503/Naya-Pyro)
-        [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
-        
-        # Installation
-        ```bash
-        pip3 install -U py-Ayra
-        ```
-        
-        # Documentation 
-        [![Documentation](https://img.shields.io/badge/Documentation-kynaylibs-blue)](http://ayra.tech/)
-        
-        
-        
-        See more working plugins on [the offical repository](https://github.com/naya1503/Naya-Pyro)!
-        
-        > Made with 💕 by [Kynan](https://t.me/Rizzvbss).    
-        
-        
-        # License
-        [![License](https://www.gnu.org/graphics/agplv3-155x51.png)](LICENSE)   
-        Ultroid is licensed under [GNU Affero General Public License](https://www.gnu.org/licenses/agpl-3.0.en.html) v3 or later.
-        
-        # Credits
-        * [![Kynan-Devs](https://img.shields.io/static/v1?label=Kynan&message=devs&color=critical)](https://t.me/Rizzvbss)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.7, <3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Kynanlibs Library
+
+Core library of [Naya-Pyro](https://github.com/naya1503/Naya-Pyro), a python based telegram userbot.
+
+[![CodeFactor](https://www.codefactor.io/repository/github/naya1503/kynaylibs/badge)](https://www.codefactor.io/repository/github/naya1503/kynaylibs)
+[![PyPI - Version](https://img.shields.io/pypi/v/py-Naya-Pyro?style=round)](https://pypi.org/project/kynaylibs)    
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/py-Naya-Pyro?label=DOWNLOADS&style=round)](https://pypi.org/project/kynaylibs)    
+[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/naya1503/Naya-Pyro/graphs/commit-activity)
+[![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/naya1503/Naya-Pyro)
+[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
+
+# Installation
+```bash
+pip3 install -U py-Ayra
+```
+
+# Documentation 
+[![Documentation](https://img.shields.io/badge/Documentation-kynaylibs-blue)](http://ayra.tech/)
+
+
+
+See more working plugins on [the offical repository](https://github.com/naya1503/Naya-Pyro)!
+
+> Made with 💕 by [Kynan](https://t.me/Rizzvbss).    
+
+
+# License
+[![License](https://www.gnu.org/graphics/agplv3-155x51.png)](LICENSE)   
+Ultroid is licensed under [GNU Affero General Public License](https://www.gnu.org/licenses/agpl-3.0.en.html) v3 or later.
+
+# Credits
+* [![Kynan-Devs](https://img.shields.io/static/v1?label=Kynan&message=devs&color=critical)](https://t.me/Rizzvbss)
+
```

### Comparing `kynaylibs-1.8.1/kynaylibs.egg-info/SOURCES.txt` & `kynaylibs-1.8.2/kynaylibs.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 kynaylibs/__init__.py
 kynaylibs/version.py
 kynaylibs.egg-info/PKG-INFO
 kynaylibs.egg-info/SOURCES.txt
```

### Comparing `kynaylibs-1.8.1/setup.py` & `kynaylibs-1.8.2/setup.py`

 * *Files identical despite different names*

