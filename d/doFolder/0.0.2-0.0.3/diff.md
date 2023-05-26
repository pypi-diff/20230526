# Comparing `tmp/doFolder-0.0.2.tar.gz` & `tmp/doFolder-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doFolder-0.0.2.tar", last modified: Thu May 25 15:23:20 2023, max compression
+gzip compressed data, was "doFolder-0.0.3.tar", last modified: Fri May 26 06:31:49 2023, max compression
```

## Comparing `doFolder-0.0.2.tar` & `doFolder-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 15:23:20.874165 doFolder-0.0.2/
--rw-rw-rw-   0        0        0     3132 2023-05-25 15:23:20.874165 doFolder-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2440 2023-05-25 15:16:05.000000 doFolder-0.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-25 15:23:20.865164 doFolder-0.0.2/doFolder/
--rw-rw-rw-   0        0        0       63 2023-05-25 15:20:42.000000 doFolder-0.0.2/doFolder/__init__.py
--rw-rw-rw-   0        0        0     8382 2023-05-25 15:18:43.000000 doFolder-0.0.2/doFolder/compare.py
--rw-rw-rw-   0        0        0    17480 2023-05-25 14:42:53.000000 doFolder-0.0.2/doFolder/main.py
--rw-rw-rw-   0        0        0    13042 2023-05-25 15:18:16.000000 doFolder-0.0.2/doFolder/terminal.py
-drwxrwxrwx   0        0        0        0 2023-05-25 15:23:20.873165 doFolder-0.0.2/doFolder.egg-info/
--rw-rw-rw-   0        0        0     3132 2023-05-25 15:23:20.000000 doFolder-0.0.2/doFolder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-25 15:23:20.000000 doFolder-0.0.2/doFolder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 15:23:20.000000 doFolder-0.0.2/doFolder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-25 15:23:20.000000 doFolder-0.0.2/doFolder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-05-25 15:23:20.000000 doFolder-0.0.2/doFolder.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-25 15:23:20.000000 doFolder-0.0.2/doFolder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 15:23:20.874165 doFolder-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1159 2023-05-25 15:16:41.000000 doFolder-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:31:49.887162 doFolder-0.0.3/
+-rw-rw-rw-   0        0        0     3245 2023-05-26 06:31:49.886162 doFolder-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2553 2023-05-26 06:30:22.000000 doFolder-0.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-26 06:31:49.841162 doFolder-0.0.3/doFolder/
+-rw-rw-rw-   0        0        0       63 2023-05-25 15:20:42.000000 doFolder-0.0.3/doFolder/__init__.py
+-rw-rw-rw-   0        0        0     9443 2023-05-26 06:31:25.000000 doFolder-0.0.3/doFolder/compare.py
+-rw-rw-rw-   0        0        0    17480 2023-05-25 14:42:53.000000 doFolder-0.0.3/doFolder/main.py
+-rw-rw-rw-   0        0        0    13265 2023-05-26 05:13:05.000000 doFolder-0.0.3/doFolder/terminal.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:31:49.884161 doFolder-0.0.3/doFolder.egg-info/
+-rw-rw-rw-   0        0        0     3245 2023-05-26 06:31:49.000000 doFolder-0.0.3/doFolder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-26 06:31:49.000000 doFolder-0.0.3/doFolder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 06:31:49.000000 doFolder-0.0.3/doFolder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-26 06:31:49.000000 doFolder-0.0.3/doFolder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-05-26 06:31:49.000000 doFolder-0.0.3/doFolder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 06:31:49.000000 doFolder-0.0.3/doFolder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 06:31:49.887162 doFolder-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-05-26 04:09:05.000000 doFolder-0.0.3/setup.py
```

### Comparing `doFolder-0.0.2/PKG-INFO` & `doFolder-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.0.2
+Version: 0.0.3
 Summary: download files quickly
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
@@ -74,14 +74,16 @@
       -  *参数* ``compareContent`` 文件内容的比较方法
 
          -  ``ignore`` 忽略文件内容
          -  ``hash`` 比较文件哈希值
          -  ``content`` 比较文件内容
          -  ``size`` 比较文件大小
 
+      -  *参数* ``threaded`` 是否线程化 ``bool``
+      -  *参数* ``threaded`` 最大线程数:``int``
       -  *返回* 比较结果:``CompareResult``
 
 命令行使用
 ~~~~~~~~~~
 
 .. code:: bash
```

### Comparing `doFolder-0.0.2/README.rst` & `doFolder-0.0.3/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -54,14 +54,16 @@
       -  *参数* ``compareContent`` 文件内容的比较方法
 
          -  ``ignore`` 忽略文件内容
          -  ``hash`` 比较文件哈希值
          -  ``content`` 比较文件内容
          -  ``size`` 比较文件大小
 
+      -  *参数* ``threaded`` 是否线程化 ``bool``
+      -  *参数* ``threaded`` 最大线程数:``int``
       -  *返回* 比较结果:``CompareResult``
 
 命令行使用
 ~~~~~~~~~~
 
 .. code:: bash
```

### Comparing `doFolder-0.0.2/doFolder/compare.py` & `doFolder-0.0.3/doFolder/compare.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import doFolder.main as doFolder
 from typing import Literal,List,Union
+from concurrent.futures import ThreadPoolExecutor
 class RepeatedExecutionError(Exception):
     def __init__(self,message:str):
         self.message=message
     def __str__(self):
         return self.message
 class FileMissing(doFolder._HasName):
     def __init__(self,file:doFolder.File,root:doFolder.Folder,anotherFolder:doFolder.Folder):
@@ -141,36 +142,51 @@
             self.cacheFolderMissingList=self._folderMissingList.values
             for  i in self._FolderDifferentList:
                 self.cacheFolderMissingList+=i.folderMissingList
         return self.cacheFolderMissingList
     @property
     def differentList(self)->List[Union[FileMissing,FolderMissing,FileDifferent]]:
         return self.fileMissingList+self.folderMissingList+self.fileDifferentList
-def compare(folder1:doFolder.Folder,folder2:doFolder.Folder,compareContent:Literal["ignore","hash","content","size"]="ignore",root1:Union[doFolder.Folder,None]=None,root2:Union[doFolder.Folder,None]=None)->CompareResult:
-    root1=root1 if root1!=None else folder1
-    root2=root2 if root2!=None else folder2
+def _compareFile(result:CompareResult,file1:doFolder.File,file2:doFolder.File,compareContent:Literal["ignore","hash","content","size"],root1:doFolder.Folder
+            ,root2:doFolder.Folder)->None:
+    if compareContent=="hash" and file1.hash!=file2.hash:
+        result.newDifferent(FileDifferent(file1,file2,root1,root2))
+    elif compareContent=="content" and file1.content!=file2.content:
+        result.newDifferent(FileDifferent(file1,file2,root1,root2))
+    elif compareContent=="size" and file1.size!=file2.size:
+        result.newDifferent(FileDifferent(file1,file2,root1,root2))
+def compare(folder1:doFolder.Folder,folder2:doFolder.Folder,compareContent:Literal["ignore","hash","content","size"]="ignore",threaded:bool=False,threads:Union[None,int]=None)->CompareResult:
+    threadPool=ThreadPoolExecutor(max_workers=threads) if threaded else None
+    result=_compare(folder1,folder2,folder1,folder2,compareContent,threadPool)
+    assert result
+    if threadPool:threadPool.shutdown(wait=True)
+    return result
+def _compare(folder1:doFolder.Folder,folder2:doFolder.Folder,root1:doFolder.Folder
+            ,root2:doFolder.Folder,compareContent:Literal["ignore","hash","content","size"]="ignore",threadPool:Union[ThreadPoolExecutor,None]=None,parent:Union[CompareResult,None]=None)->Union[CompareResult,None]:
     result=CompareResult(folder1,folder2)
     for file1 in folder1.files:
         file2=folder2.files[file1.name]
         if file2==None:
             result.newDifferent(FileMissing(file1,root1,root2))
-        elif compareContent=="hash" and file1.hash!=file2.hash:
-            result.newDifferent(FileDifferent(file1,file2,root1,root2))
-        elif compareContent=="content" and file1.content!=file2.content:
-            result.newDifferent(FileDifferent(file1,file2,root1,root2))
-        elif compareContent=="size" and file1.size!=file2.size:
-            result.newDifferent(FileDifferent(file1,file2,root1,root2))
+        else:
+            if threadPool:threadPool.submit(_compareFile,result,file1,file2,compareContent,root1,root2)
+            else:_compareFile(result,file1,file2,compareContent,root1,root2)
     for file2 in folder2.files:
         file1=folder1.files[file2.name]
         if file1==None:
             result.newDifferent(FileMissing(file2,root2,root1))
     for subfolder1 in folder1.subfolder:
         subfolder2=folder2.subfolder[subfolder1.name]
         if subfolder2==None:
             result.newDifferent(FolderMissing(subfolder1,root1,root2))
         else:
-            result.newDifferent(compare(subfolder1,subfolder2,compareContent,root1,root2))
+            if threadPool:threadPool.submit(_compare,subfolder1,subfolder2,root1,root2,compareContent,threadPool,result)
+            else:_compare(subfolder1,subfolder2,root1,root2,compareContent,threadPool,result)
     for subfolder2 in folder2.subfolder:
         subfolder1=folder1.subfolder[subfolder2.name]
         if subfolder1==None:
             result.newDifferent(FolderMissing(subfolder2,root2,root1))
-    return result
+    if parent:
+        parent.newDifferent(result)
+        return
+    else:
+        return result
```

### Comparing `doFolder-0.0.2/doFolder/main.py` & `doFolder-0.0.3/doFolder/main.py`

 * *Files identical despite different names*

### Comparing `doFolder-0.0.2/doFolder/terminal.py` & `doFolder-0.0.3/doFolder/terminal.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,31 +3,33 @@
 from rich.console import Console
 from rich.table import Table,Column
 from rich.style import Style
 import datetime
 import sys
 from typing import List,Union,Set
 
-def compare():
+def docompare():
     import argparse
     statueMapping={
         'copied':"[green]copied[/green]",
         "removed":'[red]removed[/red]', 
         'waiting':"[yellow]waiting[/yellow]", 
         'choice1':"[cyan]choice1[/cyan]",
         'choice2':"[cyan]choice2[/cyan]"
     }
     argparser = argparse.ArgumentParser()
     argparser.add_argument('folder1',type = str, help = 'The first folder to compare')
     argparser.add_argument('folder2',type = str, help = 'The second folder to compare')
     argparser.add_argument('-c', '--content', type = str, choices=["ignore","hash","content","size"] ,default="ignore", help = 'How to compare the content of the file')
+    argparser.add_argument('-t', '--threaded', action="store_true", help = 'Use multithreaded scanning')
+    argparser.add_argument('-n', '--num', help = 'Maximum number of threads')
     args = argparser.parse_args()
     folder1 = doFolder.Folder(args.folder1)
     folder2 = doFolder.Folder(args.folder2)
-    retsult=comp.compare(folder1, folder2,args.content)
+    retsult=comp.compare(folder1, folder2,args.content,args.threaded,args.num)
     fileMissingList=retsult.fileMissingList
     folderMissingList=retsult.folderMissingList
     fileDifferentList=retsult.fileDifferentList
     console=Console()
     all:List[Union[comp.FileMissing,comp.FolderMissing,comp.FileDifferent]]=[]
     errSum:int = 0
     result:List=[]
@@ -269,8 +271,9 @@
         console.print("[yellow]No different found[/yellow]")
         sys.exit(0)
     showTable()
     while True:
         command=console.input("")
         result.append(">>>"+command)
         result.append(doCommand(command))
-        showTable()
+        showTable()
+docompare()
```

### Comparing `doFolder-0.0.2/doFolder.egg-info/PKG-INFO` & `doFolder-0.0.3/doFolder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.0.2
+Version: 0.0.3
 Summary: download files quickly
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
@@ -74,14 +74,16 @@
       -  *参数* ``compareContent`` 文件内容的比较方法
 
          -  ``ignore`` 忽略文件内容
          -  ``hash`` 比较文件哈希值
          -  ``content`` 比较文件内容
          -  ``size`` 比较文件大小
 
+      -  *参数* ``threaded`` 是否线程化 ``bool``
+      -  *参数* ``threaded`` 最大线程数:``int``
       -  *返回* 比较结果:``CompareResult``
 
 命令行使用
 ~~~~~~~~~~
 
 .. code:: bash
```

### Comparing `doFolder-0.0.2/setup.py` & `doFolder-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 setup(
     name = 'doFolder',
-    version = '0.0.2',
+    version = '0.0.3',
     keywords = ['file',"foler","path","filesystem"],
     description = 'download files quickly',
     long_description = open("README.rst","r",encoding="utf-8").read(),
     author = 'kuankuan',
     author_email = '2163826131@qq.com',
     url="https://kuankuan2007.gitee.io/docs/do-folder/",
     install_requires = [
@@ -29,11 +29,11 @@
         'Operating System :: MacOS',
         'Operating System :: POSIX :: Linux',
         'Operating System :: Microsoft :: Windows',
         'License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)'
     ],
     entry_points = {
         'console_scripts': [
-            'compare = doFolder.terminal:compare',
+            'do-compare = doFolder.terminal:doCompare',
         ],
     }
 )
```

