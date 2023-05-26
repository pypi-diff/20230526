# Comparing `tmp/huanyuan-3.0.1-py3-none-any.whl.zip` & `tmp/huanyuan-3.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 34610 bytes, number of entries: 9
+Zip file size: 34602 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 14:19 HUANYUAN/__init__.py
 -rw-r--r--  2.0 unx     4050 b- defN 23-May-26 15:02 HUANYUAN/huanyuan.py
--rwxr-xr-x  2.0 unx   159640 b- defN 23-May-26 15:21 huanyuan-3.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     7267 b- defN 23-May-26 15:21 huanyuan-3.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 15:21 huanyuan-3.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-May-26 15:21 huanyuan-3.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 23-May-26 15:21 huanyuan-3.0.1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-26 15:21 huanyuan-3.0.1.dist-info/zip-safe
--rw-rw-r--  2.0 unx      727 b- defN 23-May-26 15:21 huanyuan-3.0.1.dist-info/RECORD
-9 files, 171847 bytes uncompressed, 33348 bytes compressed:  80.6%
+-rwxr-xr-x  2.0 unx   159640 b- defN 23-May-26 17:58 huanyuan-3.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7274 b- defN 23-May-26 17:58 huanyuan-3.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 17:58 huanyuan-3.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-May-26 17:58 huanyuan-3.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-May-26 17:58 huanyuan-3.0.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-26 17:52 huanyuan-3.0.2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      727 b- defN 23-May-26 17:58 huanyuan-3.0.2.dist-info/RECORD
+9 files, 171854 bytes uncompressed, 33340 bytes compressed:  80.6%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: HUANYUAN/__init__.py
 Comment: 
 
 Filename: HUANYUAN/huanyuan.py
 Comment: 
 
-Filename: huanyuan-3.0.1.dist-info/LICENSE
+Filename: huanyuan-3.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: huanyuan-3.0.1.dist-info/METADATA
+Filename: huanyuan-3.0.2.dist-info/METADATA
 Comment: 
 
-Filename: huanyuan-3.0.1.dist-info/WHEEL
+Filename: huanyuan-3.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: huanyuan-3.0.1.dist-info/entry_points.txt
+Filename: huanyuan-3.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: huanyuan-3.0.1.dist-info/top_level.txt
+Filename: huanyuan-3.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: huanyuan-3.0.1.dist-info/zip-safe
+Filename: huanyuan-3.0.2.dist-info/zip-safe
 Comment: 
 
-Filename: huanyuan-3.0.1.dist-info/RECORD
+Filename: huanyuan-3.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `huanyuan-3.0.1.dist-info/LICENSE` & `huanyuan-3.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `huanyuan-3.0.1.dist-info/METADATA` & `huanyuan-3.0.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: huanyuan
-Version: 3.0.1
+Version: 3.0.2
 Summary: Fast switching PyPi mirror image source
 Home-page: https://gitee.com/qsbye/python-huanyuan
-Author: Original:HangfengYang,Changed by qsbye
+Author: Original:HangfengYang,Edited by qsbye
 Author-email: yhf5fhy@gmail.com,2557877116@qq.com
 License: MIT
 Keywords: python、PyPi source、terminal
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: docopt
 
@@ -66,26 +66,25 @@
     <a href="https://github.com/yhangf/PyQuickInstall">
     <img src="./picture/star.svg">
         </a>
     <a href="https://github.com/yhangf/PyQuickInstall">
     <img src="./picture/fork.svg">
         </a>
 </p>
-由于国内通过pip下载python包的速度真的很慢，很容易因为超时而失败，而pqi可以把PyPi源迅速切换为国内源tuna, douban, aliyun, ustc从而大大加快python包的安装速度，提速效果见下图所示。huanyuan是对pqi的修改版本,添加类似`python -m huanyuan`的模块方式访问模块,解决某些情况下安装pqi后在命令行显示无此命令或者修改指定版本Python的下载源.
+由于国内通过pip下载python包的速度真的很慢，很容易因为超时而失败，而pqi可以把PyPi源迅速切换为国内源tuna, douban, aliyun, ustc从而大大加快python包的安装速度，提速效果见下图所示。huanyuan是对pqi的修改版本,添加类似`python -m HUANYUAN.huanyuan`的模块方式访问模块,解决某些情况下安装pqi后在命令行显示无此命令或者修改指定版本Python的下载源.
 
 ![](./picture/db.png)
 
 ## 怎么使用(兼容py2/py3/linux/windows/MacOS)
 
 ### 1.安装
 #### 方法一（推荐）
 
 ```
->>> pip install huanyuan(还没上架)
->>> pip install -i https://www.qsbye.cn/pypi/simple huanyuan
+>>> pip install -i https://pypi.org/simple huanyuan
 ```
 
 #### 方法二
 ```
 >>> git clone https://gitee.com/qsbye/python-huanyuan.git
 >>> python3 setup.py install
 ```
@@ -110,14 +109,16 @@
 ```
 >>> huanyuan ls
 ```
 
 * 改变PyPi源
 ```
 >>> huanyuan use <name>
+或
+>>> python -m HUANYUAN.huanyuan use douban
 ```
 例子，比如运行`huanyuan use tuna`即把当前PyPi源改为清华的PyPi源
 
 * 显示当前PyPi源
 ```
 >>> huanyuan show
 ```
```

