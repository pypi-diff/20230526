# Comparing `tmp/pdocr-rpc-1.0.0.tar.gz` & `tmp/pdocr-rpc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/uos/github/pdocr-rpc/dist/.tmp-ik4b4t4i/pdocr-rpc-1.0.0.tar", last modified: Fri May 26 09:55:12 2023, max compression
+gzip compressed data, was "/home/uos/github/pdocr-rpc/dist/.tmp-33hxrb6y/pdocr-rpc-1.0.1.tar", last modified: Fri May 26 10:32:41 2023, max compression
```

## Comparing `pdocr-rpc-1.0.0.tar` & `pdocr-rpc-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-26 09:55:12.000000 pdocr-rpc-1.0.0/
--rw-r--r--   0 uos       (1000) uos       (1000)    11357 2023-05-26 08:16:45.000000 pdocr-rpc-1.0.0/LICENSE
--rw-r--r--   0 uos       (1000) uos       (1000)     4457 2023-05-26 09:55:12.000000 pdocr-rpc-1.0.0/PKG-INFO
--rw-r--r--   0 uos       (1000) uos       (1000)     3960 2023-05-26 09:54:12.000000 pdocr-rpc-1.0.0/README.md
-drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-26 09:55:12.000000 pdocr-rpc-1.0.0/pdocr_rpc/
--rw-r--r--   0 uos       (1000) uos       (1000)        0 2023-05-26 09:13:53.000000 pdocr-rpc-1.0.0/pdocr_rpc/__init__.py
--rw-r--r--   0 uos       (1000) uos       (1000)     5749 2023-05-26 09:14:41.000000 pdocr-rpc-1.0.0/pdocr_rpc/ocr.py
--rw-r--r--   0 uos       (1000) uos       (1000)     1424 2023-05-26 09:14:41.000000 pdocr-rpc-1.0.0/pdocr_rpc/ocr_server.py
--rw-r--r--   0 uos       (1000) uos       (1000)      842 2023-05-26 08:53:13.000000 pdocr-rpc-1.0.0/pdocr_rpc/setting.py
-drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-26 09:55:12.000000 pdocr-rpc-1.0.0/pdocr_rpc.egg-info/
--rw-r--r--   0 uos       (1000) uos       (1000)     4457 2023-05-26 09:55:12.000000 pdocr-rpc-1.0.0/pdocr_rpc.egg-info/PKG-INFO
--rw-r--r--   0 uos       (1000) uos       (1000)      248 2023-05-26 09:55:12.000000 pdocr-rpc-1.0.0/pdocr_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 uos       (1000) uos       (1000)        1 2023-05-26 09:55:12.000000 pdocr-rpc-1.0.0/pdocr_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 uos       (1000) uos       (1000)       10 2023-05-26 09:55:12.000000 pdocr-rpc-1.0.0/pdocr_rpc.egg-info/top_level.txt
--rw-r--r--   0 uos       (1000) uos       (1000)      482 2023-05-26 09:53:12.000000 pdocr-rpc-1.0.0/pyproject.toml
--rw-r--r--   0 uos       (1000) uos       (1000)       38 2023-05-26 09:55:12.000000 pdocr-rpc-1.0.0/setup.cfg
+drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-26 10:32:41.000000 pdocr-rpc-1.0.1/
+-rw-r--r--   0 uos       (1000) uos       (1000)    11357 2023-05-26 08:16:45.000000 pdocr-rpc-1.0.1/LICENSE
+-rw-r--r--   0 uos       (1000) uos       (1000)     3608 2023-05-26 10:32:41.000000 pdocr-rpc-1.0.1/PKG-INFO
+-rw-r--r--   0 uos       (1000) uos       (1000)     3111 2023-05-26 10:31:47.000000 pdocr-rpc-1.0.1/README.md
+drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-26 10:32:41.000000 pdocr-rpc-1.0.1/pdocr_rpc/
+-rw-r--r--   0 uos       (1000) uos       (1000)        0 2023-05-26 09:13:53.000000 pdocr-rpc-1.0.1/pdocr_rpc/__init__.py
+-rw-r--r--   0 uos       (1000) uos       (1000)     5752 2023-05-26 10:18:48.000000 pdocr-rpc-1.0.1/pdocr_rpc/ocr.py
+-rw-r--r--   0 uos       (1000) uos       (1000)     1423 2023-05-26 10:17:38.000000 pdocr-rpc-1.0.1/pdocr_rpc/ocr_server.py
+-rw-r--r--   0 uos       (1000) uos       (1000)      904 2023-05-26 10:18:24.000000 pdocr-rpc-1.0.1/pdocr_rpc/setting.py
+drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-26 10:32:41.000000 pdocr-rpc-1.0.1/pdocr_rpc.egg-info/
+-rw-r--r--   0 uos       (1000) uos       (1000)     3608 2023-05-26 10:32:40.000000 pdocr-rpc-1.0.1/pdocr_rpc.egg-info/PKG-INFO
+-rw-r--r--   0 uos       (1000) uos       (1000)      248 2023-05-26 10:32:40.000000 pdocr-rpc-1.0.1/pdocr_rpc.egg-info/SOURCES.txt
+-rw-r--r--   0 uos       (1000) uos       (1000)        1 2023-05-26 10:32:40.000000 pdocr-rpc-1.0.1/pdocr_rpc.egg-info/dependency_links.txt
+-rw-r--r--   0 uos       (1000) uos       (1000)       10 2023-05-26 10:32:40.000000 pdocr-rpc-1.0.1/pdocr_rpc.egg-info/top_level.txt
+-rw-r--r--   0 uos       (1000) uos       (1000)      482 2023-05-26 10:32:09.000000 pdocr-rpc-1.0.1/pyproject.toml
+-rw-r--r--   0 uos       (1000) uos       (1000)       38 2023-05-26 10:32:41.000000 pdocr-rpc-1.0.1/setup.cfg
```

### Comparing `pdocr-rpc-1.0.0/LICENSE` & `pdocr-rpc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdocr-rpc-1.0.0/PKG-INFO` & `pdocr-rpc-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdocr-rpc
-Version: 1.0.0
+Version: 1.0.1
 Summary: PaddleOCR-RPC
 Author-email: mikigo <1964191531@qq.com>
 Project-URL: Homepage, https://github.com/funny-test/pdocr-rpc
 Project-URL: Bug Tracker, https://github.com/funny-test/pdocr-rpc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,137 +14,101 @@
 
 # RPC-PaddleOCR
 
 基于 PaddleOCR 部署的 RPC 服务。
 
 提供了一个简单易用的函数 `ocr`，通过不同的参数控制返回不同的值。
 
-
-
 ## 安装
 
 ```shell
 pip install pdocr-rpc
 ```
 
+另外还需要手动安装以下依赖：
 
+### 客户端依赖
 
-## 1、客户端
+客户端仅需要安装**截图工具**；
 
-### 1.1、使用方法
-
-```python
-# ocr.py
+- `Windows` 上使用：
 
-def ocr(*target_strings, picture_abspath=None, similarity=0.6, return_default=False, return_first=False, lang="ch"):
-    """
-     通过 OCR 进行识别。
-    :param target_strings: 
-        目标字符,识别一个字符串或多个字符串,并返回其在图片中的坐标;
-        如果不传参，返回图片中识别到的所有字符串。
-    :param picture_abspath: 要识别的图片路径。
-    :param similarity: 匹配度。
-    :param return_default: 返回识别的原生数据。
-    :param return_first: 只返回第一个,默认为 False,返回识别到的所有数据。
-    :param lang: `ch`, `en`, `fr`, `german`, `korean`, `japan`
-    :return: 返回的坐标是目标字符串所在行的中心坐标。
-    """
+```shell
+pip3 install pillow
 ```
 
-### 1.2、使用场景
-
-#### 1.1.1、指定某张图片识别
-
-```python
-ocr("~/Desktop/test.png")
-```
+- `Linux` 上使用：
 
-返回识别图片 `test.png` 的内容。 
+[PIL](https://en.wikipedia.org/wiki/Python_Imaging_Library) 的 `ImageGrab` 模块在部分的 `Linux` 上可能存在问题，报错：`ImportError: ImageGrab is macOS and Windows only` ；
 
-#### 1.1.2、识别当前屏幕
+`Linux` 上推荐安装 `pyscreenshot`；
 
-```python
-ocr()
+```shell
+pip3 install pyscreenshot
 ```
 
-自动识别当前整个屏幕的所有内容。
+### 服务端依赖
 
-#### 1.1.3、指定查找某个字符串的坐标
+安装 PaddleOCR` 环境
 
-```python
-ocr("天天向上")
+```
+pip3 install paddlepaddle -i https://mirror.baidu.com/pypi/simple
+pip3 install "paddleocr>=2.0.1" -i https://mirror.baidu.com/pypi/simple
 ```
 
-返回当前屏幕中，“天天向上”的坐标，如果存在多个，则返回一个字典。
-
-通过不同的参数可以改变返回值的类型；
 
-### 1.3、安装依赖
 
-客户端仅需要安装截图工具；
+## 1、使用方法
 
-- `Windows` 上使用：
+### 1.1、导入
 
-```shell
-pip install pillow
+```python
+from pdocr_rpc import ocr
 ```
 
-- `Linux` 上使用：
-
-[PIL](https://en.wikipedia.org/wiki/Python_Imaging_Library) ImageGrab 模块在部分的 `Linux` 上可能存在问题，报错：`ImportError: ImageGrab is macOS and Windows only` ；
+### 1.2、使用场景
 
-`Linux` 上推荐安装 `pyscreenshot`；
+#### 1.1.1、识别当前屏幕的所有文字内容
 
-```shell
-sudo pip3 install pyscreenshot
+```python
+ocr()
 ```
 
-然后修改导入代码：
+自动识别当前整个屏幕的所有内容。
+
+#### 1.1.2、指定某张图片识别的所有文字内容
 
 ```python
-# Linux
-import pyscreenshot as ImageGrab
-# Windows or macOS
-# from PIL import ImageGrab
+ocr(picture_abspath="~/Desktop/test.png")
 ```
 
-## 2、服务端
-
-使用 `Linux` 操作系统进行部署，`debian`、`ubuntu`、`centos`、`UOS`、`deepin` 等常见的发行版都是可以的。
-
-推荐 `pipenv` 进行环境搭建；
+返回识别图片 `test.png` 的内容。 
 
-安装 `pipenv` ：
+#### 1.1.3、在全屏指定查找某个字符串的坐标
 
+```python
+ocr("天天向上")
 ```
-sudo pip3 install pipenv
-```
-
-新建一个目录作为环境包 `ocr_env`：
 
-```
-cd ~
-mkdir ocr_env
-```
+返回当前屏幕中，“天天向上”的坐标，如果存在多个，则返回一个字典。
 
-创建 `python 3.7` 环境：
+#### 1.1.4、指定某张图片查找某个字符串的坐标
 
-```
-cd ocr_env
-pipenv --python 3.7
+```python
+ocr("天天向上"，picture_abspath="~/Desktop/test.png")
 ```
 
-安装 `OCR` 依赖包：
+### 1.3、其他参数
 
+```shell
+similarity: 匹配度。
+return_default: 返回识别的原生数据。
+return_first: 只返回第一个,默认为 False,返回识别到的所有数据。
+lang: `ch`, `en`, `fr`, `german`, `korean`, `japan`
 ```
-pipenv install paddlepaddle -i https://mirror.baidu.com/pypi/simple
-pipenv install "paddleocr>=2.0.1" -i https://mirror.baidu.com/pypi/simple
-```
-
-不出意外，这样就把依赖安装好了。
 
 ### 2.1、启动服务
 
 将 `ocr_server.py` 文件拷贝到 `ocr_env` 目录，后台执行它就好了：
 
 ```
 cd ocr_env
```

### Comparing `pdocr-rpc-1.0.0/README.md` & `pdocr-rpc-1.0.1/pdocr_rpc.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,136 +1,114 @@
+Metadata-Version: 2.1
+Name: pdocr-rpc
+Version: 1.0.1
+Summary: PaddleOCR-RPC
+Author-email: mikigo <1964191531@qq.com>
+Project-URL: Homepage, https://github.com/funny-test/pdocr-rpc
+Project-URL: Bug Tracker, https://github.com/funny-test/pdocr-rpc/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # RPC-PaddleOCR
 
 基于 PaddleOCR 部署的 RPC 服务。
 
 提供了一个简单易用的函数 `ocr`，通过不同的参数控制返回不同的值。
 
-
-
 ## 安装
 
 ```shell
 pip install pdocr-rpc
 ```
 
+另外还需要手动安装以下依赖：
 
+### 客户端依赖
 
-## 1、客户端
-
-### 1.1、使用方法
+客户端仅需要安装**截图工具**；
 
-```python
-# ocr.py
+- `Windows` 上使用：
 
-def ocr(*target_strings, picture_abspath=None, similarity=0.6, return_default=False, return_first=False, lang="ch"):
-    """
-     通过 OCR 进行识别。
-    :param target_strings: 
-        目标字符,识别一个字符串或多个字符串,并返回其在图片中的坐标;
-        如果不传参，返回图片中识别到的所有字符串。
-    :param picture_abspath: 要识别的图片路径。
-    :param similarity: 匹配度。
-    :param return_default: 返回识别的原生数据。
-    :param return_first: 只返回第一个,默认为 False,返回识别到的所有数据。
-    :param lang: `ch`, `en`, `fr`, `german`, `korean`, `japan`
-    :return: 返回的坐标是目标字符串所在行的中心坐标。
-    """
+```shell
+pip3 install pillow
 ```
 
-### 1.2、使用场景
-
-#### 1.1.1、指定某张图片识别
-
-```python
-ocr("~/Desktop/test.png")
-```
+- `Linux` 上使用：
 
-返回识别图片 `test.png` 的内容。 
+[PIL](https://en.wikipedia.org/wiki/Python_Imaging_Library) 的 `ImageGrab` 模块在部分的 `Linux` 上可能存在问题，报错：`ImportError: ImageGrab is macOS and Windows only` ；
 
-#### 1.1.2、识别当前屏幕
+`Linux` 上推荐安装 `pyscreenshot`；
 
-```python
-ocr()
+```shell
+pip3 install pyscreenshot
 ```
 
-自动识别当前整个屏幕的所有内容。
+### 服务端依赖
 
-#### 1.1.3、指定查找某个字符串的坐标
+安装 PaddleOCR` 环境
 
-```python
-ocr("天天向上")
+```
+pip3 install paddlepaddle -i https://mirror.baidu.com/pypi/simple
+pip3 install "paddleocr>=2.0.1" -i https://mirror.baidu.com/pypi/simple
 ```
 
-返回当前屏幕中，“天天向上”的坐标，如果存在多个，则返回一个字典。
-
-通过不同的参数可以改变返回值的类型；
 
-### 1.3、安装依赖
 
-客户端仅需要安装截图工具；
+## 1、使用方法
 
-- `Windows` 上使用：
+### 1.1、导入
 
-```shell
-pip install pillow
+```python
+from pdocr_rpc import ocr
 ```
 
-- `Linux` 上使用：
+### 1.2、使用场景
 
-[PIL](https://en.wikipedia.org/wiki/Python_Imaging_Library) ImageGrab 模块在部分的 `Linux` 上可能存在问题，报错：`ImportError: ImageGrab is macOS and Windows only` ；
+#### 1.1.1、识别当前屏幕的所有文字内容
 
-`Linux` 上推荐安装 `pyscreenshot`；
-
-```shell
-sudo pip3 install pyscreenshot
+```python
+ocr()
 ```
 
-然后修改导入代码：
+自动识别当前整个屏幕的所有内容。
+
+#### 1.1.2、指定某张图片识别的所有文字内容
 
 ```python
-# Linux
-import pyscreenshot as ImageGrab
-# Windows or macOS
-# from PIL import ImageGrab
+ocr(picture_abspath="~/Desktop/test.png")
 ```
 
-## 2、服务端
-
-使用 `Linux` 操作系统进行部署，`debian`、`ubuntu`、`centos`、`UOS`、`deepin` 等常见的发行版都是可以的。
-
-推荐 `pipenv` 进行环境搭建；
+返回识别图片 `test.png` 的内容。 
 
-安装 `pipenv` ：
+#### 1.1.3、在全屏指定查找某个字符串的坐标
 
+```python
+ocr("天天向上")
 ```
-sudo pip3 install pipenv
-```
-
-新建一个目录作为环境包 `ocr_env`：
 
-```
-cd ~
-mkdir ocr_env
-```
+返回当前屏幕中，“天天向上”的坐标，如果存在多个，则返回一个字典。
 
-创建 `python 3.7` 环境：
+#### 1.1.4、指定某张图片查找某个字符串的坐标
 
-```
-cd ocr_env
-pipenv --python 3.7
+```python
+ocr("天天向上"，picture_abspath="~/Desktop/test.png")
 ```
 
-安装 `OCR` 依赖包：
+### 1.3、其他参数
 
+```shell
+similarity: 匹配度。
+return_default: 返回识别的原生数据。
+return_first: 只返回第一个,默认为 False,返回识别到的所有数据。
+lang: `ch`, `en`, `fr`, `german`, `korean`, `japan`
 ```
-pipenv install paddlepaddle -i https://mirror.baidu.com/pypi/simple
-pipenv install "paddleocr>=2.0.1" -i https://mirror.baidu.com/pypi/simple
-```
-
-不出意外，这样就把依赖安装好了。
 
 ### 2.1、启动服务
 
 将 `ocr_server.py` 文件拷贝到 `ocr_env` 目录，后台执行它就好了：
 
 ```
 cd ocr_env
```

### Comparing `pdocr-rpc-1.0.0/pdocr_rpc/ocr.py` & `pdocr-rpc-1.0.1/pdocr_rpc/ocr.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 
 
 def _pdocr_client(lang, picture_abspath=None):
     """
      通过 RPC 协议进行 OCR 识别。
     :return: 返回 PaddleOCR 的原始数据
     """
-    if picture_abspath is None:
+    if not picture_abspath:
         picture_abspath = setting.SCREEN_CACHE
         if setting.IS_X11:
             ImageGrab.grab().save(os.path.expanduser(picture_abspath))
         else:
             picture_abspath = (
                 popen("qdbus org.kde.KWin /Screenshot screenshotFullscreen")
                     .read()
                     .strip("\n")
             )
-    server = ServerProxy(f"http://{setting.IP}:{setting.PORT}", allow_none=True)
+    server = ServerProxy(f"http://{setting.SERVER_IP}:{setting.PORT}", allow_none=True)
     put_handle = open(os.path.expanduser(picture_abspath), "rb")
     try:
         # 将图片上传到服务端
         pic_dir = server.image_put(Binary(put_handle.read()))
         put_handle.close()
         # 返回识别结果
         return server.paddle_ocr(pic_dir, lang)
```

### Comparing `pdocr-rpc-1.0.0/pdocr_rpc/ocr_server.py` & `pdocr-rpc-1.0.1/pdocr_rpc/ocr_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,12 +45,12 @@
     """
     ocr = PaddleOCR(use_angle_cls=True, lang=lang)
     result = ocr.ocr(pic_path, cls=True)
     return result
 
 
 if __name__ == "__main__":
-    server = ThreadXMLRPCServer((setting.IP, setting.PORT), allow_none=True)
+    server = ThreadXMLRPCServer(("0.0.0.0", setting.PORT), allow_none=True)
     server.register_function(image_put, "image_put")
     server.register_function(paddle_ocr, "paddle_ocr")
     print("监听客户端请求。。")
     server.serve_forever()
```

### Comparing `pdocr-rpc-1.0.0/pdocr_rpc/setting.py` & `pdocr-rpc-1.0.1/pdocr_rpc/setting.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import enum
 import os
-import platform
 import sys
 
-
 @enum.unique
 class DisplayServer(enum.Enum):
     wayland = "wayland"
     x11 = "x11"
 
 @enum.unique
 class PlatForm(enum.Enum):
-    win = "win"
+    win = "win32"
     linux = "linux"
 
 
 
 class _Setting:
     """配置模块"""
 
-    IP = "0.0.0.0"
+    SERVER_IP = "127.0.0.1"
     PORT = 8890
 
-    if sys.platform == "win32":
+    IS_LINUX = False
+    IS_WINDOWS = False
+    if sys.platform == PlatForm.win.value:
         # windows
         IS_WINDOWS = True
         # TODO
         ...
-    elif platform.system() == PlatForm.linux:
+    elif sys.platform == PlatForm.linux.value:
         # Linux
         IS_LINUX = True
         # 显示服务器
         DISPLAY_SERVER = os.popen(
             "cat ~/.xsession-errors | grep XDG_SESSION_TYPE | head -n 1"
         ).read().split("=")[-1].strip("\n")
 
-        IS_X11 = (DISPLAY_SERVER == DisplayServer.x11)
-        IS_WAYLAND = (DISPLAY_SERVER == DisplayServer.wayland)
+        IS_X11 = (DISPLAY_SERVER == DisplayServer.x11.value)
+        IS_WAYLAND = (DISPLAY_SERVER == DisplayServer.wayland.value)
         SCREEN_CACHE = "/tmp/screen.png"
 
 
 setting = _Setting()
```

