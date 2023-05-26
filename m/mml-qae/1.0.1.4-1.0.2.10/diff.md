# Comparing `tmp/mml_qae-1.0.1.4.tar.gz` & `tmp/mml_qae-1.0.2.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mml_qae-1.0.1.4.tar", last modified: Mon May 15 13:33:01 2023, max compression
+gzip compressed data, was "dist\mml_qae-1.0.2.10.tar", last modified: Fri May 26 14:54:20 2023, max compression
```

## Comparing `mml_qae-1.0.1.4.tar` & `mml_qae-1.0.2.10.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 13:33:01.000000 mml_qae-1.0.1.4/
--rw-rw-rw-   0        0        0        0 2023-05-13 07:15:44.000000 mml_qae-1.0.1.4/LICENSE
--rw-rw-rw-   0        0        0     4193 2023-05-15 13:33:01.000000 mml_qae-1.0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3431 2023-05-15 13:32:28.000000 mml_qae-1.0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 13:33:01.000000 mml_qae-1.0.1.4/mml_qae/
--rw-rw-rw-   0        0        0     1664 2023-05-14 08:17:49.000000 mml_qae-1.0.1.4/mml_qae/MoreErrors.py
--rw-rw-rw-   0        0        0        0 2023-05-13 07:17:18.000000 mml_qae-1.0.1.4/mml_qae/__init__.py
--rw-rw-rw-   0        0        0     2905 2023-05-15 13:22:26.000000 mml_qae-1.0.1.4/mml_qae/lists_of_number.py
--rw-rw-rw-   0        0        0     1407 2023-05-15 13:23:01.000000 mml_qae-1.0.1.4/mml_qae/one_list_of_number.py
-drwxrwxrwx   0        0        0        0 2023-05-15 13:33:01.000000 mml_qae-1.0.1.4/mml_qae.egg-info/
--rw-rw-rw-   0        0        0     4193 2023-05-15 13:33:00.000000 mml_qae-1.0.1.4/mml_qae.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-15 13:33:01.000000 mml_qae-1.0.1.4/mml_qae.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 13:33:00.000000 mml_qae-1.0.1.4/mml_qae.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-15 13:33:00.000000 mml_qae-1.0.1.4/mml_qae.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      689 2023-05-15 13:32:45.000000 mml_qae-1.0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 13:33:01.000000 mml_qae-1.0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      668 2023-05-15 13:32:55.000000 mml_qae-1.0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:54:20.000000 mml_qae-1.0.2.10/
+-rw-rw-rw-   0        0        0        0 2023-05-13 07:15:44.000000 mml_qae-1.0.2.10/LICENSE
+-rw-rw-rw-   0        0        0     4337 2023-05-26 14:54:20.000000 mml_qae-1.0.2.10/PKG-INFO
+-rw-rw-rw-   0        0        0     3574 2023-05-26 14:54:14.000000 mml_qae-1.0.2.10/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 14:54:20.000000 mml_qae-1.0.2.10/mml_qae/
+-rw-rw-rw-   0        0        0     1960 2023-05-26 14:52:53.000000 mml_qae-1.0.2.10/mml_qae/Chinese_dealing.py
+-rw-rw-rw-   0        0        0     1916 2023-05-15 13:52:21.000000 mml_qae-1.0.2.10/mml_qae/MoreErrors.py
+-rw-rw-rw-   0        0        0        0 2023-05-13 07:17:18.000000 mml_qae-1.0.2.10/mml_qae/__init__.py
+-rw-rw-rw-   0        0        0     2905 2023-05-15 13:22:26.000000 mml_qae-1.0.2.10/mml_qae/lists_of_number.py
+-rw-rw-rw-   0        0        0     1407 2023-05-15 13:23:01.000000 mml_qae-1.0.2.10/mml_qae/one_list_of_number.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:54:20.000000 mml_qae-1.0.2.10/mml_qae.egg-info/
+-rw-rw-rw-   0        0        0     4337 2023-05-26 14:54:19.000000 mml_qae-1.0.2.10/mml_qae.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-05-26 14:54:19.000000 mml_qae-1.0.2.10/mml_qae.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 14:54:19.000000 mml_qae-1.0.2.10/mml_qae.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 14:54:19.000000 mml_qae-1.0.2.10/mml_qae.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      690 2023-05-26 14:53:53.000000 mml_qae-1.0.2.10/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 14:54:20.000000 mml_qae-1.0.2.10/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-05-26 14:53:51.000000 mml_qae-1.0.2.10/setup.py
```

### Comparing `mml_qae-1.0.1.4/PKG-INFO` & `mml_qae-1.0.2.10/mml_qae.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mml_qae
-Version: 1.0.1.4
+Name: mml-qae
+Version: 1.0.2.10
 Summary: The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning.
 Home-page: https://www.python.org
 Author: ETRO_secondleader
 Author-email: ETRO_secondleader <ETRO_gfyx@163.com>
 Project-URL: Homepage, https://github.com/pypa/mml_qae
 Project-URL: Author's Git, https://github.com/ZYpS-leader?tab=repositories
 Classifier: Programming Language :: Python :: 3
@@ -24,40 +24,42 @@
     此处将放置每一个的更新日志.与历史版本一栏不同的是,这里是实时更新且更加详细的.
 + 1.0.0 2023.5.14 初代版本.框架构建.
 + 1.0.1 ----------- 略微扩充了方法.
 + 1.0.1.1 --------- 向pypi.org中扩充了项目描述.
 + 1.0.1.2 --------- 向pypi.org中扩充了说明文档.(由于作者脑抽忘记再1.0.1.1时上传了不得不新增一个版本)
 + 1.0.1.3 --------- 加入了子模块MoreErrors以提供更多错误支持.
 + 1.0.1.4 2023.5.15 突然引起的恶性错误,此为紧急修复版本.
++ 1.0.2.10 2023.5.26 中文语言处理(简易版).在测试中本版本出现了一些问题待修复.请见谅.
 ---
 ## 开发者发言
 + We now have packages to deal with big data like statsmodels, sklearn, Spark, or packages to deal with natural language, such as jieba or spaCy. I admit that those packages are really useful while facing whith tons of csv data. BUT! I think we need a nicer package to deal with data, don't we? So, the mml-qae package(the whole name is My Machine Learning-Quicker and Easier) is here to help you. Alright, so, I have to say that I didn't do anything new, but I put those complex codes together into grand-new methods, so that you will be able to deal with MachineLearning and DataDealing. I started this project on 14th, May 2023 with version 1.0.1. In a more proper way, I worked on this project with my team ETRO(to see the Author's Email). I promise to update it regularly, but I cannot say how long the interval between two updataions will be for certain. Another thing needed to be paid attentioned is, this package only works at Python3.7.2, and you MUST pip install the packages needed in mml, like statsmodels. I will speak of all those packages you need to preinstall in README.md. Last but not least, never use 'from mml-qae import *'. Many methods in mml are the same name with the built-in functions! That'll be all, and have fun with MachineLearning and DataDealing!
 + Packages needed
 > + statsmodels
 > + sklearn
 > + jieba
 > + spaCy
 > + pandas
 > + numpy
 > + matplotlib
 > + wordcloud
+> + opencv-python
 ---
 ## 历史版本(包括部分未公布的版本)
 + 1 简易大数据处理与网络构建
 > +  1.0 预发布版本
 > > + 1.0.0 
 >      初代版本，无项目描述。
 > > + 1.0.1
 >      修复1.0.0中的明显问题。
 > > > + 1.0.1.1  加入项目描述.
 > > > + 1.0.1.2  加入帮助文档README.md并修复一些小问题
 > > > + 1.0.1.3  加入一些自定义错误和修复一些小问题
 > >  + 1.0.2
 >      加入封装好的自然语言处理快捷方法。
-> > > + 1.0.2.1  加入中文处理模型.
+> > > + 1.0.2.10  加入中文处理模型(初步).
 > > > + 1.0.2.2  加入英语处理模型.
 > >  + 1.0.3     修复1.0版本的bug和问题。
 > +  1.1 完善版本
 > >  + 1.1.1 加入数据库处理方法。
 > > > + 1.1.1.1 MySQL
 > > > + 1.1.1.2 NoSQL
 > > > + 1.1.1.3 更多数据库
```

### Comparing `mml_qae-1.0.1.4/README.md` & `mml_qae-1.0.2.10/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,40 +8,42 @@
     此处将放置每一个的更新日志.与历史版本一栏不同的是,这里是实时更新且更加详细的.
 + 1.0.0 2023.5.14 初代版本.框架构建.
 + 1.0.1 ----------- 略微扩充了方法.
 + 1.0.1.1 --------- 向pypi.org中扩充了项目描述.
 + 1.0.1.2 --------- 向pypi.org中扩充了说明文档.(由于作者脑抽忘记再1.0.1.1时上传了不得不新增一个版本)
 + 1.0.1.3 --------- 加入了子模块MoreErrors以提供更多错误支持.
 + 1.0.1.4 2023.5.15 突然引起的恶性错误,此为紧急修复版本.
++ 1.0.2.10 2023.5.26 中文语言处理(简易版).在测试中本版本出现了一些问题待修复.请见谅.
 ---
 ## 开发者发言
 + We now have packages to deal with big data like statsmodels, sklearn, Spark, or packages to deal with natural language, such as jieba or spaCy. I admit that those packages are really useful while facing whith tons of csv data. BUT! I think we need a nicer package to deal with data, don't we? So, the mml-qae package(the whole name is My Machine Learning-Quicker and Easier) is here to help you. Alright, so, I have to say that I didn't do anything new, but I put those complex codes together into grand-new methods, so that you will be able to deal with MachineLearning and DataDealing. I started this project on 14th, May 2023 with version 1.0.1. In a more proper way, I worked on this project with my team ETRO(to see the Author's Email). I promise to update it regularly, but I cannot say how long the interval between two updataions will be for certain. Another thing needed to be paid attentioned is, this package only works at Python3.7.2, and you MUST pip install the packages needed in mml, like statsmodels. I will speak of all those packages you need to preinstall in README.md. Last but not least, never use 'from mml-qae import *'. Many methods in mml are the same name with the built-in functions! That'll be all, and have fun with MachineLearning and DataDealing!
 + Packages needed
 > + statsmodels
 > + sklearn
 > + jieba
 > + spaCy
 > + pandas
 > + numpy
 > + matplotlib
 > + wordcloud
+> + opencv-python
 ---
 ## 历史版本(包括部分未公布的版本)
 + 1 简易大数据处理与网络构建
 > +  1.0 预发布版本
 > > + 1.0.0 
 >      初代版本，无项目描述。
 > > + 1.0.1
 >      修复1.0.0中的明显问题。
 > > > + 1.0.1.1  加入项目描述.
 > > > + 1.0.1.2  加入帮助文档README.md并修复一些小问题
 > > > + 1.0.1.3  加入一些自定义错误和修复一些小问题
 > >  + 1.0.2
 >      加入封装好的自然语言处理快捷方法。
-> > > + 1.0.2.1  加入中文处理模型.
+> > > + 1.0.2.10  加入中文处理模型(初步).
 > > > + 1.0.2.2  加入英语处理模型.
 > >  + 1.0.3     修复1.0版本的bug和问题。
 > +  1.1 完善版本
 > >  + 1.1.1 加入数据库处理方法。
 > > > + 1.1.1.1 MySQL
 > > > + 1.1.1.2 NoSQL
 > > > + 1.1.1.3 更多数据库
```

### Comparing `mml_qae-1.0.1.4/mml_qae/MoreErrors.py` & `mml_qae-1.0.2.10/mml_qae/MoreErrors.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,8 +37,15 @@
 		print("训练错误:给定的数组(或列表)在机器学习训练中出现异常.请查看lists_of_number.py源码解决问题或在Git上联系作者: ZYpS_leader.")        
 		
 class DataError5(MyError):
 	"""数据异常:需要分析的数据(或分析结果)包含inf或nan."""
 	def __init__(self) -> None:
 		pass
 	def __str__(self) -> str:
-		print("数据异常:需要分析的数据(或分析结果)包含inf或nan.")        
+		print("数据异常:需要分析的数据(或分析结果)包含inf或nan.")       
+
+class DataError6(MyError):
+	"""数据异常:应当有相同规格的数组(或列表)规格不同!"""	
+	def __init__(self) -> None:
+		pass
+	def __str__(self) -> str:
+		print("数据异常:应当有相同规格的数组(或列表)规格不同!")
```

### Comparing `mml_qae-1.0.1.4/mml_qae/lists_of_number.py` & `mml_qae-1.0.2.10/mml_qae/lists_of_number.py`

 * *Files identical despite different names*

### Comparing `mml_qae-1.0.1.4/mml_qae/one_list_of_number.py` & `mml_qae-1.0.2.10/mml_qae/one_list_of_number.py`

 * *Files identical despite different names*

### Comparing `mml_qae-1.0.1.4/mml_qae.egg-info/PKG-INFO` & `mml_qae-1.0.2.10/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mml-qae
-Version: 1.0.1.4
+Name: mml_qae
+Version: 1.0.2.10
 Summary: The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning.
 Home-page: https://www.python.org
 Author: ETRO_secondleader
 Author-email: ETRO_secondleader <ETRO_gfyx@163.com>
 Project-URL: Homepage, https://github.com/pypa/mml_qae
 Project-URL: Author's Git, https://github.com/ZYpS-leader?tab=repositories
 Classifier: Programming Language :: Python :: 3
@@ -24,40 +24,42 @@
     此处将放置每一个的更新日志.与历史版本一栏不同的是,这里是实时更新且更加详细的.
 + 1.0.0 2023.5.14 初代版本.框架构建.
 + 1.0.1 ----------- 略微扩充了方法.
 + 1.0.1.1 --------- 向pypi.org中扩充了项目描述.
 + 1.0.1.2 --------- 向pypi.org中扩充了说明文档.(由于作者脑抽忘记再1.0.1.1时上传了不得不新增一个版本)
 + 1.0.1.3 --------- 加入了子模块MoreErrors以提供更多错误支持.
 + 1.0.1.4 2023.5.15 突然引起的恶性错误,此为紧急修复版本.
++ 1.0.2.10 2023.5.26 中文语言处理(简易版).在测试中本版本出现了一些问题待修复.请见谅.
 ---
 ## 开发者发言
 + We now have packages to deal with big data like statsmodels, sklearn, Spark, or packages to deal with natural language, such as jieba or spaCy. I admit that those packages are really useful while facing whith tons of csv data. BUT! I think we need a nicer package to deal with data, don't we? So, the mml-qae package(the whole name is My Machine Learning-Quicker and Easier) is here to help you. Alright, so, I have to say that I didn't do anything new, but I put those complex codes together into grand-new methods, so that you will be able to deal with MachineLearning and DataDealing. I started this project on 14th, May 2023 with version 1.0.1. In a more proper way, I worked on this project with my team ETRO(to see the Author's Email). I promise to update it regularly, but I cannot say how long the interval between two updataions will be for certain. Another thing needed to be paid attentioned is, this package only works at Python3.7.2, and you MUST pip install the packages needed in mml, like statsmodels. I will speak of all those packages you need to preinstall in README.md. Last but not least, never use 'from mml-qae import *'. Many methods in mml are the same name with the built-in functions! That'll be all, and have fun with MachineLearning and DataDealing!
 + Packages needed
 > + statsmodels
 > + sklearn
 > + jieba
 > + spaCy
 > + pandas
 > + numpy
 > + matplotlib
 > + wordcloud
+> + opencv-python
 ---
 ## 历史版本(包括部分未公布的版本)
 + 1 简易大数据处理与网络构建
 > +  1.0 预发布版本
 > > + 1.0.0 
 >      初代版本，无项目描述。
 > > + 1.0.1
 >      修复1.0.0中的明显问题。
 > > > + 1.0.1.1  加入项目描述.
 > > > + 1.0.1.2  加入帮助文档README.md并修复一些小问题
 > > > + 1.0.1.3  加入一些自定义错误和修复一些小问题
 > >  + 1.0.2
 >      加入封装好的自然语言处理快捷方法。
-> > > + 1.0.2.1  加入中文处理模型.
+> > > + 1.0.2.10  加入中文处理模型(初步).
 > > > + 1.0.2.2  加入英语处理模型.
 > >  + 1.0.3     修复1.0版本的bug和问题。
 > +  1.1 完善版本
 > >  + 1.1.1 加入数据库处理方法。
 > > > + 1.1.1.1 MySQL
 > > > + 1.1.1.2 NoSQL
 > > > + 1.1.1.3 更多数据库
```

### Comparing `mml_qae-1.0.1.4/pyproject.toml` & `mml_qae-1.0.2.10/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mml_qae"
-version = "1.0.1.4"
+version = "1.0.2.10"
 authors = [
   { name="ETRO_secondleader", email="ETRO_gfyx@163.com" },
 ]
 description = "The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning."
 readme = "README.md"
 requires-python = "==3.7.2"
 classifiers = [
```

### Comparing `mml_qae-1.0.1.4/setup.py` & `mml_qae-1.0.2.10/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools 
 
 with open("README.md", "r",encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
       name='mml_qae',
-      version='1.0.1.4',
+      version='1.0.2.10',
       description='The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='ETRO_secondleader',
       author_email='ETRO_gfyx@163.com',
       url='https://www.python.org', 
       packages=setuptools.find_packages(),
```

