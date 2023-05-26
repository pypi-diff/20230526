# Comparing `tmp/hiyobot-0.2.5.tar.gz` & `tmp/hiyobot-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiyobot-0.2.5.tar", last modified: Wed May 24 13:16:18 2023, max compression
+gzip compressed data, was "hiyobot-0.2.6.tar", last modified: Fri May 26 14:40:41 2023, max compression
```

## Comparing `hiyobot-0.2.5.tar` & `hiyobot-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:16:18.870009 hiyobot-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-24 13:16:07.000000 hiyobot-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-24 13:16:18.870009 hiyobot-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-24 13:16:07.000000 hiyobot-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:16:18.870009 hiyobot-0.2.5/hiyobot/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 13:16:07.000000 hiyobot-0.2.5/hiyobot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:16:18.870009 hiyobot-0.2.5/hiyobot/hackchat/
--rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-05-24 13:16:07.000000 hiyobot-0.2.5/hiyobot/hackchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-24 13:16:07.000000 hiyobot-0.2.5/hiyobot/hc-wait4inp.test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:16:18.870009 hiyobot-0.2.5/hiyobot/zhangchat/
--rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-05-24 13:16:07.000000 hiyobot-0.2.5/hiyobot/zhangchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-24 13:16:07.000000 hiyobot-0.2.5/hiyobot/zhc-wait4inp.test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:16:18.870009 hiyobot-0.2.5/hiyobot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-24 13:16:18.000000 hiyobot-0.2.5/hiyobot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-24 13:16:18.000000 hiyobot-0.2.5/hiyobot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:16:18.000000 hiyobot-0.2.5/hiyobot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-24 13:16:18.000000 hiyobot-0.2.5/hiyobot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 13:16:18.000000 hiyobot-0.2.5/hiyobot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 13:16:18.870009 hiyobot-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-24 13:16:07.000000 hiyobot-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:40:41.236904 hiyobot-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-26 14:40:28.000000 hiyobot-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-26 14:40:41.236904 hiyobot-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-26 14:40:28.000000 hiyobot-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:40:41.236904 hiyobot-0.2.6/hiyobot/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 14:40:28.000000 hiyobot-0.2.6/hiyobot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:40:41.236904 hiyobot-0.2.6/hiyobot/hackchat/
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-05-26 14:40:28.000000 hiyobot-0.2.6/hiyobot/hackchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-26 14:40:28.000000 hiyobot-0.2.6/hiyobot/hc-wait4inp.test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:40:41.236904 hiyobot-0.2.6/hiyobot/zhangchat/
+-rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-05-26 14:40:28.000000 hiyobot-0.2.6/hiyobot/zhangchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-26 14:40:28.000000 hiyobot-0.2.6/hiyobot/zhc-wait4inp.test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:40:41.236904 hiyobot-0.2.6/hiyobot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-26 14:40:41.000000 hiyobot-0.2.6/hiyobot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-26 14:40:41.000000 hiyobot-0.2.6/hiyobot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:40:41.000000 hiyobot-0.2.6/hiyobot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-26 14:40:41.000000 hiyobot-0.2.6/hiyobot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 14:40:41.000000 hiyobot-0.2.6/hiyobot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 14:40:41.236904 hiyobot-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-26 14:40:28.000000 hiyobot-0.2.6/setup.py
```

### Comparing `hiyobot-0.2.5/LICENSE` & `hiyobot-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hiyobot-0.2.5/PKG-INFO` & `hiyobot-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiyobot
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple bot framework for Hack.chat.
 Home-page: https://github.com/Hiyoteam/hiyobot
 Author: MaggieLOL
 Author-email: tanhanzesnd@gmail.com
 License: GPL-2.0
 Keywords: bot hack.chat hack.chat-bot
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hiyobot-0.2.5/README.md` & `hiyobot-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `hiyobot-0.2.5/hiyobot/hackchat/__init__.py` & `hiyobot-0.2.6/hiyobot/hackchat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import websocket,ssl,json,threading,uuid,time,logging,re,traceback,inspect,asyncio,queue
 from functools import wraps
-HIYOBOT_VERSION=(0,2,5)
+HIYOBOT_VERSION=(0,2,6)
 MAX_RECV_LOG_LIMIT=100 #0 for no limit
 def _isasync(func):
     if inspect.isasyncgenfunction(func) or inspect.iscoroutinefunction(func):
         return True
     else:
         return False
 class Bot:
```

### Comparing `hiyobot-0.2.5/hiyobot/zhangchat/__init__.py` & `hiyobot-0.2.6/hiyobot/zhangchat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import websocket,ssl,json,threading,uuid,time,logging,re,traceback,inspect,asyncio,queue
 from functools import wraps
-HIYOBOT_VERSION=(0,2,5)
+HIYOBOT_VERSION=(0,2,6)
 MAX_RECV_LOG_LIMIT=100 #0 for no limit
 def _isasync(func):
     if inspect.isasyncgenfunction(func) or inspect.iscoroutinefunction(func):
         return True
     else:
         return False
 class Bot:
```

### Comparing `hiyobot-0.2.5/hiyobot.egg-info/PKG-INFO` & `hiyobot-0.2.6/hiyobot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiyobot
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple bot framework for Hack.chat.
 Home-page: https://github.com/Hiyoteam/hiyobot
 Author: MaggieLOL
 Author-email: tanhanzesnd@gmail.com
 License: GPL-2.0
 Keywords: bot hack.chat hack.chat-bot
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hiyobot-0.2.5/setup.py` & `hiyobot-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hiyobot', # 你的项目名称
-    version="0.2.5", # 你的项目版本
+    version="0.2.6", # 你的项目版本
     description='A simple bot framework for Hack.chat.', # 你的项目简介
     long_description=open('README.md').read(), # 你的项目详细介绍，一般从README.md文件中读取
     long_description_content_type='text/markdown', # 你的项目详细介绍的格式，一般为markdown格式
     url='https://github.com/Hiyoteam/hiyobot', # 你的项目主页，一般为github仓库地址
     author='MaggieLOL', # 你的姓名或者团队名称
     author_email='tanhanzesnd@gmail.com', # 你的邮箱或者团队邮箱
     license='GPL-2.0', # 你的项目使用的许可证，一般为MIT或者其他开源许可证
@@ -19,11 +19,11 @@
     ],
     keywords='bot hack.chat hack.chat-bot', # 一些关键词，用于描述你的项目特点或者功能
     packages=find_packages(include="*",exclude=["*.test.py"]), # 需要打包的python模块，一般使用find_packages函数自动查找，排除测试模块等不需要打包的模块
     install_requires="""cffi==1.15.1
 gevent==22.10.2
 greenlet==2.0.2
 pycparser==2.21
-websocket==0.2.1
+websocket-client==1.3.2
 zope.event==4.6
 zope.interface==6.0""".splitlines(),
 )
```

