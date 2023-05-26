# Comparing `tmp/tkintertools_dev-2.6.1.tar.gz` & `tmp/tkintertools-dev-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools_dev-2.6.1.tar", last modified: Sat May 20 23:06:04 2023, max compression
+gzip compressed data, was "tkintertools-dev-2.6.2.tar", last modified: Fri May 26 12:10:48 2023, max compression
```

## Comparing `tkintertools_dev-2.6.1.tar` & `tkintertools-dev-2.6.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 23:06:04.505702 tkintertools_dev-2.6.1/
--rw-rw-rw-   0        0        0     7548 2023-05-20 23:03:00.000000 tkintertools_dev-2.6.1/LICENSE
--rw-rw-rw-   0        0        0    26585 2023-05-20 23:06:04.505702 tkintertools_dev-2.6.1/PKG-INFO
--rw-rw-rw-   0        0        0    26099 2023-05-20 23:01:09.000000 tkintertools_dev-2.6.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 23:06:04.505702 tkintertools_dev-2.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1456 2023-05-20 23:05:28.000000 tkintertools_dev-2.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 23:06:04.499700 tkintertools_dev-2.6.1/tkintertools/
--rw-rw-rw-   0        0        0     1877 2023-05-20 20:35:35.000000 tkintertools_dev-2.6.1/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    59823 2023-05-20 20:59:55.000000 tkintertools_dev-2.6.1/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     1295 2023-05-20 20:58:40.000000 tkintertools_dev-2.6.1/tkintertools/constants.py
--rw-rw-rw-   0        0        0      870 2023-05-14 13:27:34.000000 tkintertools_dev-2.6.1/tkintertools/md.py
-drwxrwxrwx   0        0        0        0 2023-05-20 23:06:04.503701 tkintertools_dev-2.6.1/tkintertools_dev.egg-info/
--rw-rw-rw-   0        0        0    26585 2023-05-20 23:06:04.000000 tkintertools_dev-2.6.1/tkintertools_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-05-20 23:06:04.000000 tkintertools_dev-2.6.1/tkintertools_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 23:06:04.000000 tkintertools_dev-2.6.1/tkintertools_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-20 23:06:04.000000 tkintertools_dev-2.6.1/tkintertools_dev.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 12:10:48.146677 tkintertools-dev-2.6.2/
+-rw-rw-rw-   0        0        0     7548 2023-05-20 23:03:00.000000 tkintertools-dev-2.6.2/LICENSE
+-rw-rw-rw-   0        0        0    24785 2023-05-26 12:10:48.144676 tkintertools-dev-2.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0    24276 2023-05-26 12:08:22.000000 tkintertools-dev-2.6.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-26 12:10:48.146677 tkintertools-dev-2.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-05-26 12:10:07.000000 tkintertools-dev-2.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:10:48.138692 tkintertools-dev-2.6.2/tkintertools/
+-rw-rw-rw-   0        0        0     1852 2023-05-26 05:11:00.000000 tkintertools-dev-2.6.2/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    60774 2023-05-26 05:03:13.000000 tkintertools-dev-2.6.2/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     1295 2023-05-22 14:06:44.000000 tkintertools-dev-2.6.2/tkintertools/constants.py
+-rw-rw-rw-   0        0        0     9992 2023-05-26 12:02:58.000000 tkintertools-dev-2.6.2/tkintertools/tools_3d.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:10:48.143674 tkintertools-dev-2.6.2/tkintertools_dev.egg-info/
+-rw-rw-rw-   0        0        0    24785 2023-05-26 12:10:47.000000 tkintertools-dev-2.6.2/tkintertools_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-26 12:10:48.000000 tkintertools-dev-2.6.2/tkintertools_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 12:10:47.000000 tkintertools-dev-2.6.2/tkintertools_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-26 12:10:47.000000 tkintertools-dev-2.6.2/tkintertools_dev.egg-info/top_level.txt
```

### Comparing `tkintertools_dev-2.6.1/LICENSE` & `tkintertools-dev-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tkintertools_dev-2.6.1/PKG-INFO` & `tkintertools-dev-2.6.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: tkintertools_dev
-Version: 2.6.1
-Summary: An auxiliary module of the tkinder module
-Home-page: https://gitcode.net/weixin_62651706/tkintertools
-Author: Xiaokang2022
-Author-email: 2951256653@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
     <p><img height="120px" alt="logo.png"
         src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/tkintertools.png" />
     </p>
     <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
     <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
@@ -22,18 +9,18 @@
         <a href="./tkintertools/__init__.py">
             <img src="https://img.shields.io/badge/Version-2.6.1-blue" alt="latest version" />
         </a>
         <a href="./LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
         <a href="./CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/05/21-orange" alt="ChangeLog" />
+            <img src="https://img.shields.io/badge/ChangeLog-2023/05/26-orange" alt="ChangeLog" />
         </a>
         <a href="./TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-9-yellow" alt="ToDos" />
+            <img src="https://img.shields.io/badge/ToDos-10-yellow" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
             <img src="https://img.shields.io/badge/Downloads-3k-purple" alt="Downloads" />
         </a>
     </p>
     <p>
         <a href="mailto:2951256653@qq.com">
@@ -49,35 +36,35 @@
 </div>
 
 Installation/模块安装
 -----------------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.0
-* Release Date/发布日期 : 2023/03/28
+* Version/版本 : 2.6.1
+* Release Date/发布日期 : 2023/05/21
 
 ```
-pip install tkintertools==2.6.0
+pip install tkintertools==2.6.1
 ```
 或者
 ```
 pip install tkintertools
 ```
 
 这个是目前的最新版，比较稳定，bug 没有那么多，推荐使用这个。  
 稳定版有文档可以查看，有 issue 我会去查看并尝试解决 issue。
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.1
-* Release Date/发布日期 : 2023/05/21
+* Version/版本 : 2.6.2
+* Release Date/发布日期 : 2023/05/26
 
 ```
-pip install tkintertools-dev==2.6.1
+pip install tkintertools-dev==2.6.2
 ```
 
 这个是作者正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
 开发版本没有对应的文档，大家可以在 issue 中提出建议，我会适当采纳一些并在开发版本中更改或实现。
 
 Description/模块说明
 ----------------------
@@ -95,15 +82,15 @@
 
 tkintertools 模块还具有一些特色的功能：
 
 * 利用 tkinter 和 tkintertools 创建的程序，在高分辨率的情况下，tkintertools 的会更加清晰（这点对于笔记本用户很友好，比如我）
 * 可以迅速实现渐变色的效果
 * 窗口缩放，所有的控件的大小跟着缩放（当然，也可以设置为不跟随缩放）
 
-注意：需要 Python3.7 及更高版本才能运行 tkintertools！
+注意：需要 **Python3.7** 及更高版本才能运行 tkintertools！
 
 Provides/模块功能
 -------------------
 
 Here, only the more distinctive features will be listed  
 这里只会列举出比较具有特色的功能
 
@@ -133,27 +120,27 @@
 见 [DPI 级别设置函数](#DPI)
 
 ### Detailed type hints/详细的类型提示
 
 参考 [PEP 526](https://peps.python.org/pep-0526/)、[PEP 586](https://peps.python.org/pep-0586/)、[PEP 604](https://peps.python.org/pep-0604/) 和 [PEP 612](https://peps.python.org/pep-0612/)，我采用了最兼容的方式去实现详细的类型提示，可适用 IDE 有 VScode、Pycharm 等。  
 那什么是类型提示呢？话不多说，直接看图就行：
 
-<p><img height="350px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/type_hint_vscode.png" alt="type_hint.png"/></p>
+![type_hint.png](docs/images/type_hint_vscode.png)
 
 在 VSCode 编辑器中，当鼠标移至类或者函数的名字上面时，会自动显示该类或者函数的注释文档。通过这种方式，不需要看太多的帮助文档和资料就能熟练地使用 tkintertools 模块！
 
 ### Across Platforms/跨平台
 
 [test.py](./test.py) 在 Windows 系统（Windows10）上运行的界面如下：
 
-<p><img height="383px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/test_win32.png" alt="test_win32.png"/></p>
+![test_win32.png](docs/images/test_win32.png)
 
 [test.py](./test.py) 在 Linux 系统（Ubuntu22.04）上运行的界面如下：
 
-<p><img height="408px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/test_linux.png" alt="test_linux.png"/></p>
+![test_linux.png](docs/images/test_linux.png)
 
 Contents/模块内容
 -------------------
 
 Each non internal class and function in the module will be described in detail here  
 这里会详细说明模块中的每个非内部类和函数
 
@@ -173,24 +160,24 @@
 
 ### Virtual Canvas Widget/虚拟画布控件
 
 1. `Label`: 标签控件
 
     标签控件的功能和`tkinter.Label`的功能类似，但更加的多元化  
     下面是`Label`控件的外观：  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/LabelTest.png" alt="LabelTest.png" /></p>
+
+    ![LabelTest.png](docs/images/LabelTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('LabelTest', 1000, 400)
-    canvas = tkt.Canvas(root, 1000, 400)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 1000, 400, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -207,25 +194,25 @@
     ```
 
     </details>
 
 2. `Button`: 按钮控件
 
     按钮控件相较于`tkinter.Button`，其自由度更高，`tkinter.Button`只有在按下的时候才能触发绑定的关联事件，而`Button`却可以在鼠标移至按钮上方时、鼠标按下时、鼠标松开时都可以绑定关联事件  
-    下面是`Button`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ButtonTest.png" alt="ButtonTest.png" /></p>
+    下面是`Button`控件的外观：
+
+    ![ButtonTest.png](docs/images/ButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ButtonTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -243,24 +230,24 @@
 
     </details>
 
 3. `CheckButton`: 复选框控件
 
     复选框控件相对于`tkinter`原生的`tkinter.CheckButton`在使用方面更加地简单，同时颜值也上升了不少  
     下面是`CheckButton`控件的外观：
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/CheckButtonTest.png" alt="CheckButtonTest.png"/></p>
+
+    ![CheckButtonTest.png](docs/images/CheckButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('CheckButtonTest', 500, 300)
-    canvas = tkt.Canvas(root, 500, 300)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 300, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -278,25 +265,25 @@
     ```
 
     </details>
 
 4. `Entry`: 输入框控件
 
     输入框控件可以轻松地设置输入的文本位置（靠左、居中和靠右），同时，它可以在鼠标移至输入框上方、鼠标未在输入框上方两种状态显示不同的默认文本  
-    下面是`Entry`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/EntryTest.png" alt="EntryTest.png" /></p>
+    下面是`Entry`控件的外观：
+
+    ![EntryTest.png](docs/images/EntryTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('EntryTest', 500, 400)
-    canvas = tkt.Canvas(root, 500, 400)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 400, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -310,39 +297,39 @@
         'RightEntry', 'Enter'), justify='right')
     tkt.Entry(canvas, 270, 20, 200, 30, radius=8, text='LeftEntry')
     tkt.Entry(canvas, 270, 55, 200, 30, radius=8,
             text='CenterEntry', justify='center')
     tkt.Entry(canvas, 270, 90, 200, 30, radius=8,
             text='RightEntry', justify='right')
     tkt.Entry(canvas, 100, 150, 300, 35, text=('PasswordEntry',
-            'Click To Enter'), justify='center', show='•')
+            'Click To Enter'), justify='center', show='●')
     tkt.Entry(canvas, 100, 200, 300, 35, text='DisableEntry',
             justify='center').set_live(False)
     tkt.Entry(canvas, 100, 250, 300, 35, text='TransparentEntry',
             justify='center', color_fill=tkt.COLOR_NONE)
 
     root.mainloop()
     ```
 
     </details>
 
 5. `Text`: 文本框控件
 
     文本框类似于输入框，这里就不再赘述  
-    下面是`Text`控件的外观：  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/TextTest.png" alt="TextTest.png" /></p>
+    下面是`Text`控件的外观：
+
+    ![TextTest.png](docs/images/TextTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('TextTest', 1000, 400)
-    canvas = tkt.Canvas(root, 1000, 400)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 1000, 400, 0, 0)
 
 
     def colorful(x, y, width, height) -> None:  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -360,36 +347,35 @@
     ```
 
     </details>
 
 6. `Progressbar`: 进度条控件
 
     进度条控件相比`tkinter.ttk.Progressbar`，外观上的自由度较大  
-    下面是`Progressbar`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ProgressbarTest.png" alt="ProgressbarTest.png" /></p>
+    下面是`Progressbar`控件的外观：
+
+    ![ProgressbarTest.png](docs/images/ProgressbarTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ProgressbarTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height) -> None:  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
 
 
     colorful(30, 290, 440, 50)
-
     tkt.Progressbar(canvas, 50, 50, 400, 30)
     tkt.Progressbar(canvas, 50, 100, 400, 30).load(.6667)
     tkt.Progressbar(canvas, 50, 150, 400, 30, borderwidth=5).load(1)
     (_ := tkt.Progressbar(canvas, 50, 200, 400, 30)).load(0.3333)
     _.set_live(False)
     tkt.Progressbar(canvas, 50, 250, 400, 30, color_bar=(
         'lightyellow', 'skyblue')).load(.5)
@@ -423,25 +409,25 @@
 
     单例模式，不用介绍了吧？通过继承它来使用
 
 ### Tool Function/工具函数
 
 1. `move`: <a name="move">移动函数</a>
 
-    移动函数可以轻松地按一定的规律、移动速度、移动时间去移动`tkintertools`模块内的所有对象，同时兼容了`tkinter`内的对象，即`tkinter`中的对象也可以很方便地移动，甚至它还可以移动窗口的位置！  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/MoveTest.gif" alt="MoveTest.gif" /></p>
+    移动函数可以轻松地按一定的规律、移动速度、移动时间去移动`tkintertools`模块内的所有对象，同时兼容了`tkinter`内的对象，即`tkinter`中的对象也可以很方便地移动，甚至它还可以移动窗口的位置！
+
+    ![MoveTest.gif](docs/images/MoveTest.gif)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('MoveTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
     rect = canvas.create_rectangle(50, 350, 150, 450)
 
 
     def move_window(switch=[True]):  # type: (list[bool]) -> None
         tkt.move(root, None, 1000 if switch[0] else -1000, 0, 800, mode='flat')
         switch[0] = not switch[0]
 
@@ -460,15 +446,14 @@
     tkt.Button(canvas, 50, 50, 200, 40, radius=10,
             text='MoveWindow', command=move_window)
     tkt.Button(canvas, 50, 100, 200, 40, radius=10,
             text='MoveRect', command=move_rect)
     button = tkt.Button(canvas, 50, 150, 200, 40, radius=10,
                         text='MoveButton', command=move_button)
 
-
     root.mainloop()
     ```
 
     </details>
 
 2. `text`: 文本函数
 
@@ -478,26 +463,27 @@
     `left`   : "tkintertools        "  
     `center` : "    tkintertools    "  
     `right`  : "        tkintertools"</pre>
 
 3. `color`: <a name="Gradient">颜色函数</a>
 
     颜色函数可以轻松求出一个颜色到另外一个颜色的过渡颜色，因此可以轻松得到渐变色的效果，同时，改变传入的参数还可以得到传入颜色的对比色  
-    第二张图是 test.py 在图像测试中绘制的图案  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ColorTest.png" alt="ColorTest.png" />
-    <img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/Test_Draw.png" alt="Test_Draw.png" /></p>
+    第二张图是 test.py 在图像测试中绘制的图案
+
+    ![ColorTest.png](docs/images/ColorTest.png)
+
+    ![Test_Draw.png](docs/images/Test_Draw.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ColorTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#00FF00'), i/width)
             color_2 = tkt.color(('#FFFFFF', '#000000'), i/width)
@@ -517,18 +503,22 @@
     `askfont`函数可以打开默认的字体选择窗口，这个窗口虽然是默认的，但它实际上无法在`tkinter`中打开，因为`tkinter`并没有对应的 API 能够做到这一点。但是，`tkintertools`调用并封装了原生的 tcl 的命令，使得字体选择框能够被我们使用。
 
     <p><img width="540px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/font.png" alt="font.png" /></p>
 
 5. `SetProcessDpiAwareness`: <a name="DPI">DPI 级别设置函数</a>
 
     这个函数实际上只是对函数`ctypes.WinDLL('shcore').SetProcessDpiAwareness`的一个简单包装，其值可为 0、1 和 2，分别代表程序 DPI 的不同级别，那么缩放效果也就不同，`tkintertools`选择的值是 1，但程序默认值实际为 0  
-    下面是执行了这个函数的效果
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/SetProcessDpiAwareness_0.png" alt="SetProcessDpiAwareness_1.png" /></p>
-    <p>下面是未执行这个函数的效果</p>
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/SetProcessDpiAwareness_1.png" alt="SetProcessDpiAwareness_0.png" /></p>
+    下面是未执行这个函数的效果
+    
+    ![SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
+
+    <p>下面是执行了这个函数的效果</p>
+
+    ![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
+
     从上面的两张图中可以很明显的看出第一张很模糊，第二张很清晰，这就是 DPI 级别不同的原因，不过这一点在屏幕缩放比不是 100% 的时候才会出现  
     大家对上面的图肯定很熟悉，这不就是 IDLE 吗！？对，这个的问题的解决办法也是来自于 IDLE 的源代码 [pyshell.py line 18~20]  
     注意：该函数在程序的不同位置执行的效果不一样！一般用在`mainloop`之前，但`tkintertools`已经在`mainloop`函数中嵌入了该函数，无需再设置一次 DPI 级别，此函数是为了原生`tkinter`程序用的。
 
 Examples/实战示例
 ----------------
 
@@ -570,28 +560,23 @@
 * 文章链接: 暂无
 * 代码仓库: https://gitcode.net/weixin_62651706/tester
 * 程序下载: 暂无
 * 推荐指数: 👍👍👍
 
 这个案例使用了最新稳定版的 tkintertools-v2.6.0，界面非常稳定，几乎没有 bug，完全采用 tkintertools 的控件，颜值很高，界面非常流畅。体现了 tkintertools 模块与 tkinter 模块相比在性能上的优越性！
 
-<p>
-    <img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/examples/exam3_1.png" alt="client.png"/>
-    <img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/examples/exam3_2.png" alt="client.png"/>
-</p>
+![exam3_1.png](docs/examples/exam3_1.png)
+![exam3_2.png](docs/examples/exam3_2.png)
 
 More/更多
 ---------
 
 > GitCode:  
 > https://gitcode.net/weixin_62651706/tkintertools
 
 > GitHub(Mirror/镜像):  
 > https://github.com/XiaoKang2022-CSDN/tkintertools
 
 > Column/专栏:  
 > https://blog.csdn.net/weixin_62651706/category_11600888.html
 
-> Tutorials/教程:  
-> https://xiaokang2022.blog.csdn.net/article/details/127374661
-
 还有更多内容请在 [源代码](./tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,28 +1,21 @@
-Metadata-Version: 2.1 Name: tkintertools_dev Version: 2.6.1 Summary: An
-auxiliary module of the tkinder module Home-page: https://gitcode.net/
-weixin_62651706/tkintertools Author: Xiaokang2022 Author-email:
-2951256653@qq.com Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
-Classifier: Operating System :: OS Independent Description-Content-Type: text/
-markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
                             [Email] [Blog] [Author]
 Installation/æ¨¡åå®è£ ----------------------- ### Stable version/
-ç¨³å®çæ¬ * Version/çæ¬ : 2.6.0 * Release Date/åå¸æ¥æ : 2023/03/28
-``` pip install tkintertools==2.6.0 ``` æè ``` pip install tkintertools ```
+ç¨³å®çæ¬ * Version/çæ¬ : 2.6.1 * Release Date/åå¸æ¥æ : 2023/05/21
+``` pip install tkintertools==2.6.1 ``` æè ``` pip install tkintertools ```
 è¿ä¸ªæ¯ç®åçææ°çï¼æ¯è¾ç¨³å®ï¼bug
 æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã ç¨³å®çæææ¡£å¯ä»¥æ¥çï¼æ
 issue æä¼å»æ¥çå¹¶å°è¯è§£å³ issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.1 * Release Date/åå¸æ¥æ : 2023/05/21
-``` pip install tkintertools-dev==2.6.1 ```
+å¼åçæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/26
+``` pip install tkintertools-dev==2.6.2 ```
 è¿ä¸ªæ¯ä½èæ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
 å¯è½ä¼æ¯è¾å¤ã å¼åçæ¬æ²¡æå¯¹åºçææ¡£ï¼å¤§å®¶å¯ä»¥å¨ issue
 ä¸­æåºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
 Description/æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº
 tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
@@ -34,18 +27,18 @@
 ä½åæ¶ä¹äº§çäºä¸äºç¼ºç¹ï¼ * èæçæ§ä»¶æ æ³è·åç¦ç¹ *
 èæçæ§ä»¶å¨ææ¬è¾å¥åæ¾ç¤ºçåè½ä¸å­å¨ä¸äºç¼ºé·ï¼è¿ä¸ªç¼ºé·ä¸æ¯å¾ææ¾ï¼ä½å¼ºè¿«çå°±æç¹é¾åäºï¼æ¯å¦æï¼
 tkintertools æ¨¡åè¿å·æä¸äºç¹è²çåè½ï¼ * å©ç¨ tkinter å
 tkintertools åå»ºçç¨åºï¼å¨é«åè¾¨ççæåµä¸ï¼tkintertools
 çä¼æ´å æ¸æ°ï¼è¿ç¹å¯¹äºç¬è®°æ¬ç¨æ·å¾åå¥½ï¼æ¯å¦æï¼ *
 å¯ä»¥è¿éå®ç°æ¸åè²çææ *
 çªå£ç¼©æ¾ï¼ææçæ§ä»¶çå¤§å°è·çç¼©æ¾ï¼å½ç¶ï¼ä¹å¯ä»¥è®¾ç½®ä¸ºä¸è·éç¼©æ¾ï¼
-æ³¨æï¼éè¦ Python3.7 åæ´é«çæ¬æè½è¿è¡ tkintertoolsï¼ Provides/
-æ¨¡ååè½ ------------------- Here, only the more distinctive features will
-be listed è¿éåªä¼åä¸¾åºæ¯è¾å·æç¹è²çåè½ ### Customizable
-widgets/å¯èªå®ä¹çæ§ä»¶ tkintertools
+æ³¨æï¼éè¦ **Python3.7** åæ´é«çæ¬æè½è¿è¡ tkintertoolsï¼
+Provides/æ¨¡ååè½ ------------------- Here, only the more distinctive
+features will be listed è¿éåªä¼åä¸¾åºæ¯è¾å·æç¹è²çåè½ ###
+Customizable widgets/å¯èªå®ä¹çæ§ä»¶ tkintertools
 æ¨¡åçæ§ä»¶æ¥æè®¸å¤åæ°ä¾æä»¬è®¾ç½®ï¼æ¯å¦åè§çåå¾ãææ¬åè¾¹æ¡ä»¥åæ§ä»¶åé¨çé¢è²ï¼å³èäºä»¶ç­ç­ã
 è¿éè¦è¯´æçæ¯ï¼æ¯ä¸ªæ§ä»¶å¯ä»¥è®¾ç½®çå³èäºä»¶ä¸æ­¢ä¸ç§ï¼å¨é¼ æ ç»è¿æ§ä»¶æ¶å¯ä»¥ç»å®äºä»¶ï¼é¼ æ ç¹å»æ§ä»¶ä¹å¯ä»¥ï¼é¼ æ ç¹å»åæ¾å¼ä¹è¡ç­ç­ã
 ææ¬åè¾¹æ¡ä»¥åæ§ä»¶çå¡«åè²ä¹æ¯ç±»ä¼¼çï¼å¨é¼ æ ç»è¿æ§ä»¶ãç¹å»æ§ä»¶ãç¹å»åæ¾å¼é½å¯ä»¥è®¾å®é¢è²ã
 ææ¬ç±»æ§ä»¶è¿è½å¤ä»å³è¾¹éæ­¥è¾å¥ææ¬ï¼ææ¬è¾å¥æç¤ºç¬¦ä¹å¯ä»¥ä¸æ¯åè°æ è¶£çç«çº¿ï¼å¯ä»¥æ¯å¶ä»çï¼æ¯å¦ä¸åçº¿ç­ã
 æåï¼å¤§å®¶å¯ä»¥çä¸ä¸ [test.py](./test.py)
 æä»¶éé¢çç¤ºä¾ï¼è¿ä¸ªç¤ºä¾å±ç¤ºäº tkintertools
 æ¨¡åçç»å¤§é¨ååè½ï¼ç¤ºä¾ä¸­æ´æéèç âå¤å½©åå¹»â
@@ -58,117 +51,108 @@
 (#Gradient) ### Automatically adapt to DPI/èªå¨éåºDPI è§ [DPI
 çº§å«è®¾ç½®å½æ°](#DPI) ### Detailed type hints/è¯¦ç»çç±»åæç¤º åè
 [PEP 526](https://peps.python.org/pep-0526/)ã[PEP 586](https://
 peps.python.org/pep-0586/)ã[PEP 604](https://peps.python.org/pep-0604/) å
 [PEP 612](https://peps.python.org/pep-0612/
 )ï¼æéç¨äºæå¼å®¹çæ¹å¼å»å®ç°è¯¦ç»çç±»åæç¤ºï¼å¯éç¨
 IDE æ VScodeãPycharm ç­ã
-é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼
-[type_hint.png]
-å¨ VSCode
+é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼ !
+[type_hint.png](docs/images/type_hint_vscode.png) å¨ VSCode
 ç¼è¾å¨ä¸­ï¼å½é¼ æ ç§»è³ç±»æèå½æ°çåå­ä¸é¢æ¶ï¼ä¼èªå¨æ¾ç¤ºè¯¥ç±»æèå½æ°çæ³¨éææ¡£ãéè¿è¿ç§æ¹å¼ï¼ä¸éè¦çå¤ªå¤çå¸®å©ææ¡£åèµæå°±è½çç»å°ä½¿ç¨
 tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](./test.py) å¨
-Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼
-[test_win32.png]
-[test.py](./test.py) å¨ Linux
-ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼
-[test_linux.png]
-Contents/æ¨¡ååå®¹ ------------------- Each non internal class and function
-in the module will be described in detail here
+Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_win32.png]
+(docs/images/test_win32.png) [test.py](./test.py) å¨ Linux
+ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png](docs/
+images/test_linux.png) Contents/æ¨¡ååå®¹ ------------------- Each non
+internal class and function in the module will be described in detail here
 è¿éä¼è¯¦ç»è¯´ææ¨¡åä¸­çæ¯ä¸ªéåé¨ç±»åå½æ° ### Container
 Widget/å®¹å¨æ§ä»¶ 1. `Tk`: çªå£ç±»
 ç»§æ¿äº`tkinter.Tk`ï¼å¨ç»§æ¿äº`tkinter`æ¨¡åå`Tk`çåºç¡ä¸ï¼åå å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¹¶å å¥äºæ£æµçªå£å¤§å°æ¯å¦ç¼©æ¾çæºå¶ï¼ä»¥ä½¿å¾å¶å­`Canvas`åè½æ­£ç¡®å°è¿è¡ç¼©æ¾
 2. `Toplevel`: é¡¶çº§çªå£ç±»
 ç»§æ¿äº`tkinter.Toplevel`å`Tk`ï¼å å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¶ä½åä¸`Tk`ä¸æ ·
 3. `Canvas`: ç»å¸ç±»
 ç»§æ¿äº`tkinter.Canvas`ï¼å å¥äºå¯¹ç»å¸èææ§ä»¶çæ¯æï¼åæ¶æ¯åç±»ååºäºä»¶ãç¼©æ¾æ§å¶çç®¡çèï¼ä¹å¯¹`tkinter.Canvas`çå®ä¾æ¹æ³æä¸å®çå¼å®¹æ§
 ### Virtual Canvas Widget/èæç»å¸æ§ä»¶ 1. `Label`: æ ç­¾æ§ä»¶
 æ ç­¾æ§ä»¶çåè½å`tkinter.Label`çåè½ç±»ä¼¼ï¼ä½æ´å çå¤åå
-ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼
-[LabelTest.png]
+ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼ ![LabelTest.png](docs/images/LabelTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('LabelTest', 1000,
-400) canvas = tkt.Canvas(root, 1000, 400) canvas.place(x=0, y=0) def colorful
-(x, y, width, height): # type: (int, int, int, int) -> None """ Gradient colors
-""" for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Label(canvas, 50, 50, 400, 100, text='NormalLabel\nHere is the text')
 tkt.Label(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerLabel')
 tkt.Label(canvas, 550, 50, 400, 100, text='DisableLabel').set_live(False)
 tkt.Label(canvas, 550, 200, 400, 100, radius=20, text='TransparentLabel',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  2. `Button`: æé®æ§ä»¶
 æé®æ§ä»¶ç¸è¾äº`tkinter.Button`ï¼å¶èªç±åº¦æ´é«ï¼`tkinter.Button`åªæå¨æä¸çæ¶åæè½è§¦åç»å®çå³èäºä»¶ï¼è`Button`å´å¯ä»¥å¨é¼ æ ç§»è³æé®ä¸æ¹æ¶ãé¼ æ æä¸æ¶ãé¼ æ æ¾å¼æ¶é½å¯ä»¥ç»å®å³èäºä»¶
-ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼
-[ButtonTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ButtonTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) canvas.place(x=0, y=0) def colorful(x,
-y, width, height): # type: (int, int, int, int) -> None """ Gradient colors """
-for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼ ![ButtonTest.png](docs/images/
+ButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk
+('ButtonTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful
+(x, y, width, height): # type: (int, int, int, int) -> None """ Gradient colors
+""" for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 280, 400,
 100) tkt.Button(canvas, 150, 135, 200, 50, text='NormalButton') tkt.Button
 (canvas, 100, 195, 300, 50, radius=10, text='RoundCornerButton') tkt.Button
 (canvas, 150, 255, 200, 50, text='DisableButton').set_live(False) tkt.Button
 (canvas, 100, 315, 300, 50, radius=10, text='TransparentButton',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  3. `CheckButton`:
 å¤éæ¡æ§ä»¶
 å¤éæ¡æ§ä»¶ç¸å¯¹äº`tkinter`åçç`tkinter.CheckButton`å¨ä½¿ç¨æ¹é¢æ´å å°ç®åï¼åæ¶é¢å¼ä¹ä¸åäºä¸å°
-ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼
-[CheckButtonTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('CheckButtonTest',
-500, 300) canvas = tkt.Canvas(root, 500, 300) canvas.place(x=0, y=0) def
-colorful(x, y, width, height): # type: (int, int, int, int) -> None """
+ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼ ![CheckButtonTest.png](docs/images/
+CheckButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root =
+tkt.Tk('CheckButtonTest', 500, 300) canvas = tkt.Canvas(root, 500, 300, 0, 0)
+def colorful(x, y, width, height): # type: (int, int, int, int) -> None """
 Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
 '#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
 colorful(40, 190, 420, 50) tkt.CheckButton(canvas, 50, 50, 30,
 text='NormalCheckButton', value=True) tkt.CheckButton(canvas, 50, 100, 30,
 text='DisableCheckButton', value=True).set_live(False) tkt.CheckButton(canvas,
 50, 150, 30, radius=10, text='RoundCornerCheckButton') tkt.CheckButton(canvas,
 50, 200, 30, radius=15, text='TransparentCheckButton',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  4. `Entry`: è¾å¥æ¡æ§ä»¶
 è¾å¥æ¡æ§ä»¶å¯ä»¥è½»æ¾å°è®¾ç½®è¾å¥çææ¬ä½ç½®ï¼é å·¦ãå±ä¸­åé å³ï¼ï¼åæ¶ï¼å®å¯ä»¥å¨é¼ æ ç§»è³è¾å¥æ¡ä¸æ¹ãé¼ æ æªå¨è¾å¥æ¡ä¸æ¹ä¸¤ç§ç¶ææ¾ç¤ºä¸åçé»è®¤ææ¬
-ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼
-[EntryTest.png]
+ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼ ![EntryTest.png](docs/images/EntryTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('EntryTest', 500,
-400) canvas = tkt.Canvas(root, 500, 400) canvas.place(x=0, y=0) def colorful(x,
-y, width, height): # type: (int, int, int, int) -> None """ Gradient colors """
-for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+400) canvas = tkt.Canvas(root, 500, 400, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 193, 400,
 100) tkt.Entry(canvas, 20, 20, 200, 30, text=('LeftEntry', 'Enter')) tkt.Entry
 (canvas, 20, 55, 200, 30, text=( 'CenterEntry', 'Enter'), justify='center')
 tkt.Entry(canvas, 20, 90, 200, 30, text=( 'RightEntry', 'Enter'),
 justify='right') tkt.Entry(canvas, 270, 20, 200, 30, radius=8,
 text='LeftEntry') tkt.Entry(canvas, 270, 55, 200, 30, radius=8,
 text='CenterEntry', justify='center') tkt.Entry(canvas, 270, 90, 200, 30,
 radius=8, text='RightEntry', justify='right') tkt.Entry(canvas, 100, 150, 300,
-35, text=('PasswordEntry', 'Click To Enter'), justify='center', show='â¢')
+35, text=('PasswordEntry', 'Click To Enter'), justify='center', show='â')
 tkt.Entry(canvas, 100, 200, 300, 35, text='DisableEntry',
 justify='center').set_live(False) tkt.Entry(canvas, 100, 250, 300, 35,
 text='TransparentEntry', justify='center', color_fill=tkt.COLOR_NONE)
 root.mainloop() ```  5. `Text`: ææ¬æ¡æ§ä»¶
 ææ¬æ¡ç±»ä¼¼äºè¾å¥æ¡ï¼è¿éå°±ä¸åèµè¿°
-ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼
-[TextTest.png]
+ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼ ![TextTest.png](docs/images/TextTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('TextTest', 1000,
-400) canvas = tkt.Canvas(root, 1000, 400) canvas.place(x=0, y=0) def colorful
-(x, y, width, height) -> None: # type: (int, int, int, int) -> None """
-Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
-'#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
-colorful(510, 175, 480, 150) tkt.Text(canvas, 50, 50, 400, 100, text=
-('NormalText(Left)', 'Click To Enter')) tkt.Text(canvas, 50, 200, 400, 100,
-radius=20, text='RoundCornerText(Center)', justify='center') tkt.Text(canvas,
-550, 50, 400, 100, text='DisableText').set_live(False) tkt.Text(canvas, 550,
-200, 400, 100, radius=20, text='TransparentText(Right)', justify='right',
+400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
+height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
+for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
+150) tkt.Text(canvas, 50, 50, 400, 100, text=('NormalText(Left)', 'Click To
+Enter')) tkt.Text(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerText
+(Center)', justify='center') tkt.Text(canvas, 550, 50, 400, 100,
+text='DisableText').set_live(False) tkt.Text(canvas, 550, 200, 400, 100,
+radius=20, text='TransparentText(Right)', justify='right',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  6. `Progressbar`:
 è¿åº¦æ¡æ§ä»¶
 è¿åº¦æ¡æ§ä»¶ç¸æ¯`tkinter.ttk.Progressbar`ï¼å¤è§ä¸çèªç±åº¦è¾å¤§
-ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼
-[ProgressbarTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ProgressbarTest',
-500, 500) canvas = tkt.Canvas(root, 500, 500) canvas.place(x=0, y=0) def
-colorful(x, y, width, height) -> None: # type: (int, int, int, int) -> None """
-Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
+ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼ ![ProgressbarTest.png](docs/images/
+ProgressbarTest.png) æºä»£ç  ```python import tkintertools as tkt root =
+tkt.Tk('ProgressbarTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0)
+def colorful(x, y, width, height) -> None: # type: (int, int, int, int) -> None
+""" Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
 '#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
 colorful(30, 290, 440, 50) tkt.Progressbar(canvas, 50, 50, 400, 30)
 tkt.Progressbar(canvas, 50, 100, 400, 30).load(.6667) tkt.Progressbar(canvas,
 50, 150, 400, 30, borderwidth=5).load(1) (_ := tkt.Progressbar(canvas, 50, 200,
 400, 30)).load(0.3333) _.set_live(False) tkt.Progressbar(canvas, 50, 250, 400,
 30, color_bar=( 'lightyellow', 'skyblue')).load(.5) tkt.Progressbar(canvas, 50,
 300, 400, 30, color_bar=('', 'orange')).load(.1667) progressbar =
@@ -182,59 +166,58 @@
 å¨å¾æå¾å¥½çæ¯æï¼ä»éæå°éä»£ç å³å¯å®ç°å¨å¾çæ¾ç¤ºï¼è¿å¯ä»¥è®¾ç½®å¨å¾æ¾ç¤ºçéåº¦ï¼æ­¤å¤ï¼å¯¹
 png
 ç±»åçå¾ççæ¯æä¹æå¼ºåï¼å¯ä»¥å¨ä¸ä¾èµä»»ä½ç¬¬ä¸æ¹æ¨¡åæèåºçæåµä¸ï¼å¯¹
 png å¾çè¿è¡ç¼©æ¾ 2. `Singleton`: åä¾æ¨¡å¼ç±»
 åä¾æ¨¡å¼ï¼ä¸ç¨ä»ç»äºå§ï¼éè¿ç»§æ¿å®æ¥ä½¿ç¨ ### Tool Function/
 å·¥å·å½æ° 1. `move`: ç§»å¨å½æ°
 ç§»å¨å½æ°å¯ä»¥è½»æ¾å°æä¸å®çè§å¾ãç§»å¨éåº¦ãç§»å¨æ¶é´å»ç§»å¨`tkintertools`æ¨¡ååçææå¯¹è±¡ï¼åæ¶å¼å®¹äº`tkinter`åçå¯¹è±¡ï¼å³`tkinter`ä¸­çå¯¹è±¡ä¹å¯ä»¥å¾æ¹ä¾¿å°ç§»å¨ï¼çè³å®è¿å¯ä»¥ç§»å¨çªå£çä½ç½®ï¼
-[MoveTest.gif]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('MoveTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) canvas.place(x=0, y=0) rect =
-canvas.create_rectangle(50, 350, 150, 450) def move_window(switch=[True]): #
-type: (list[bool]) -> None tkt.move(root, None, 1000 if switch[0] else -1000,
-0, 800, mode='flat') switch[0] = not switch[0] def move_button(switch=[True]) -
-> None: # type: (list[bool]) -> None tkt.move(canvas, button, 200 if switch[0]
-else -200, 0, 500, mode='rebound') switch[0] = not switch[0] def move_rect
-(switch=[True]): # type: (list[bool]) -> None tkt.move(canvas, rect, 200 if
-switch[0] else -200, 0, 500, mode='smooth') switch[0] = not switch[0]
-tkt.Button(canvas, 50, 50, 200, 40, radius=10, text='MoveWindow',
-command=move_window) tkt.Button(canvas, 50, 100, 200, 40, radius=10,
-text='MoveRect', command=move_rect) button = tkt.Button(canvas, 50, 150, 200,
-40, radius=10, text='MoveButton', command=move_button) root.mainloop() ```  2.
-`text`: ææ¬å½æ°
+![MoveTest.gif](docs/images/MoveTest.gif) æºä»£ç  ```python import
+tkintertools as tkt root = tkt.Tk('MoveTest', 500, 500) canvas = tkt.Canvas
+(root, 500, 500, 0, 0) rect = canvas.create_rectangle(50, 350, 150, 450) def
+move_window(switch=[True]): # type: (list[bool]) -> None tkt.move(root, None,
+1000 if switch[0] else -1000, 0, 800, mode='flat') switch[0] = not switch[0]
+def move_button(switch=[True]) -> None: # type: (list[bool]) -> None tkt.move
+(canvas, button, 200 if switch[0] else -200, 0, 500, mode='rebound') switch[0]
+= not switch[0] def move_rect(switch=[True]): # type: (list[bool]) -> None
+tkt.move(canvas, rect, 200 if switch[0] else -200, 0, 500, mode='smooth')
+switch[0] = not switch[0] tkt.Button(canvas, 50, 50, 200, 40, radius=10,
+text='MoveWindow', command=move_window) tkt.Button(canvas, 50, 100, 200, 40,
+radius=10, text='MoveRect', command=move_rect) button = tkt.Button(canvas, 50,
+150, 200, 40, radius=10, text='MoveButton', command=move_button) root.mainloop
+() ```  2. `text`: ææ¬å½æ°
 å¯ä»¥å¿«éå¹¶æ¹ä¾¿å°å¾å°ä¸ä¸ªåæ°é¿åº¦çå­ç¬¦ä¸²ï¼ä¸å­ç¬¦ä¸²çåå®¹å¯ä»¥æå®ä½ç½®
 å¦ï¼å¾å°ä¸ä¸ª 20 é¿åº¦çå­ç¬¦ä¸² âtkintertoolsâ
     `left`   : "tkintertools        "
     `center` : "    tkintertools    "
     `right`  : "        tkintertools"
 3. `color`: é¢è²å½æ°
 é¢è²å½æ°å¯ä»¥è½»æ¾æ±åºä¸ä¸ªé¢è²å°å¦å¤ä¸ä¸ªé¢è²çè¿æ¸¡é¢è²ï¼å æ­¤å¯ä»¥è½»æ¾å¾å°æ¸åè²çææï¼åæ¶ï¼æ¹åä¼ å¥çåæ°è¿å¯ä»¥å¾å°ä¼ å¥é¢è²çå¯¹æ¯è²
-ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡
-[ColorTest.png] [Test_Draw.png]
+ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡ ![ColorTest.png]
+(docs/images/ColorTest.png) ![Test_Draw.png](docs/images/Test_Draw.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ColorTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) canvas.place(x=0, y=0) def colorful(x,
-y, width, height): # type: (int, int, int, int) -> None """ Gradient colors """
-for i in range(width): color = tkt.color(('#FF0000', '#00FF00'), i/width)
-color_2 = tkt.color(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y,
-x+i, y+height, fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 +
-i/3, outline=color_2, width=2) colorful(50, 50, 400, 100) root.mainloop() ```
-4. `askfont`: å­ä½éæ©å¯¹è¯æ¡
+500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 =
+tkt.color(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i,
+y+height, fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
+outline=color_2, width=2) colorful(50, 50, 400, 100) root.mainloop() ```  4.
+`askfont`: å­ä½éæ©å¯¹è¯æ¡
 `askfont`å½æ°å¯ä»¥æå¼é»è®¤çå­ä½éæ©çªå£ï¼è¿ä¸ªçªå£è½ç¶æ¯é»è®¤çï¼ä½å®å®éä¸æ æ³å¨`tkinter`ä¸­æå¼ï¼å ä¸º`tkinter`å¹¶æ²¡æå¯¹åºç
 API è½å¤åå°è¿ä¸ç¹ãä½æ¯ï¼`tkintertools`è°ç¨å¹¶å°è£äºåçç
 tcl çå½ä»¤ï¼ä½¿å¾å­ä½éæ©æ¡è½å¤è¢«æä»¬ä½¿ç¨ã
 [font.png]
 5. `SetProcessDpiAwareness`: DPI çº§å«è®¾ç½®å½æ°
 è¿ä¸ªå½æ°å®éä¸åªæ¯å¯¹å½æ°`ctypes.WinDLL
 ('shcore').SetProcessDpiAwareness`çä¸ä¸ªç®ååè£ï¼å¶å¼å¯ä¸º 0ã1
 å 2ï¼åå«ä»£è¡¨ç¨åº DPI
 çä¸åçº§å«ï¼é£ä¹ç¼©æ¾ææä¹å°±ä¸åï¼`tkintertools`éæ©çå¼æ¯
-1ï¼ä½ç¨åºé»è®¤å¼å®éä¸º 0 ä¸é¢æ¯æ§è¡äºè¿ä¸ªå½æ°çææ
-[SetProcessDpiAwareness_1.png]
-ä¸é¢æ¯æªæ§è¡è¿ä¸ªå½æ°çææ
-[SetProcessDpiAwareness_0.png]
+1ï¼ä½ç¨åºé»è®¤å¼å®éä¸º 0 ä¸é¢æ¯æªæ§è¡è¿ä¸ªå½æ°çææ !
+[SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
+ä¸é¢æ¯æ§è¡äºè¿ä¸ªå½æ°çææ
+![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
 ä»ä¸é¢çä¸¤å¼ å¾ä¸­å¯ä»¥å¾ææ¾ççåºç¬¬ä¸å¼ å¾æ¨¡ç³ï¼ç¬¬äºå¼ å¾æ¸æ°ï¼è¿å°±æ¯
 DPI çº§å«ä¸åçåå ï¼ä¸è¿è¿ä¸ç¹å¨å±å¹ç¼©æ¾æ¯ä¸æ¯ 100%
 çæ¶åæä¼åºç° å¤§å®¶å¯¹ä¸é¢çå¾è¯å®å¾çæï¼è¿ä¸å°±æ¯ IDLE
 åï¼ï¼å¯¹ï¼è¿ä¸ªçé®é¢çè§£å³åæ³ä¹æ¯æ¥èªäº IDLE çæºä»£ç 
 [pyshell.py line 18~20]
 æ³¨æï¼è¯¥å½æ°å¨ç¨åºçä¸åä½ç½®æ§è¡çææä¸ä¸æ ·ï¼ä¸è¬ç¨å¨`mainloop`ä¹åï¼ä½`tkintertools`å·²ç»å¨`mainloop`å½æ°ä¸­åµå¥äºè¯¥å½æ°ï¼æ éåè®¾ç½®ä¸æ¬¡
 DPI çº§å«ï¼æ­¤å½æ°æ¯ä¸ºäºåç`tkinter`ç¨åºç¨çã Examples/
@@ -263,15 +246,13 @@
 æ¨¡åçå¼å®¹æ§ï¼
 [chess.png] [chess.png]
 ### ç®æç»å½çé¢ * æç« é¾æ¥: ææ  * ä»£ç ä»åº: https://
 gitcode.net/weixin_62651706/tester * ç¨åºä¸è½½: ææ  * æ¨èææ°:
 ððð è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
-æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼
-[client.png] [client.png]
-More/æ´å¤ --------- > GitCode: > https://gitcode.net/weixin_62651706/
-tkintertools > GitHub(Mirror/éå): > https://github.com/XiaoKang2022-CSDN/
-tkintertools > Column/ä¸æ : > https://blog.csdn.net/weixin_62651706/
-category_11600888.html > Tutorials/æç¨: > https://
-xiaokang2022.blog.csdn.net/article/details/127374661 è¿ææ´å¤åå®¹è¯·å¨
-[æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
+æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png](docs/
+examples/exam3_1.png) ![exam3_2.png](docs/examples/exam3_2.png) More/æ´å¤ ---
+------ > GitCode: > https://gitcode.net/weixin_62651706/tkintertools > GitHub
+(Mirror/éå): > https://github.com/XiaoKang2022-CSDN/tkintertools > Column/
+ä¸æ : > https://blog.csdn.net/weixin_62651706/category_11600888.html
+è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
```

### Comparing `tkintertools_dev-2.6.1/README.md` & `tkintertools-dev-2.6.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: tkintertools-dev
+Version: 2.6.2
+Summary: An auxiliary module of the tkinder module
+Home-page: https://gitcode.net/weixin_62651706/tkintertools
+Author: Xiaokang2022
+Author-email: 2951256653@qq.com
+License: MulanPSL-2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
     <p><img height="120px" alt="logo.png"
         src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/tkintertools.png" />
     </p>
     <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
     <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
@@ -9,18 +23,18 @@
         <a href="./tkintertools/__init__.py">
             <img src="https://img.shields.io/badge/Version-2.6.1-blue" alt="latest version" />
         </a>
         <a href="./LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
         <a href="./CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/05/21-orange" alt="ChangeLog" />
+            <img src="https://img.shields.io/badge/ChangeLog-2023/05/26-orange" alt="ChangeLog" />
         </a>
         <a href="./TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-9-yellow" alt="ToDos" />
+            <img src="https://img.shields.io/badge/ToDos-10-yellow" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
             <img src="https://img.shields.io/badge/Downloads-3k-purple" alt="Downloads" />
         </a>
     </p>
     <p>
         <a href="mailto:2951256653@qq.com">
@@ -36,35 +50,35 @@
 </div>
 
 Installation/模块安装
 -----------------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.0
-* Release Date/发布日期 : 2023/03/28
+* Version/版本 : 2.6.1
+* Release Date/发布日期 : 2023/05/21
 
 ```
-pip install tkintertools==2.6.0
+pip install tkintertools==2.6.1
 ```
 或者
 ```
 pip install tkintertools
 ```
 
 这个是目前的最新版，比较稳定，bug 没有那么多，推荐使用这个。  
 稳定版有文档可以查看，有 issue 我会去查看并尝试解决 issue。
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.1
-* Release Date/发布日期 : 2023/05/21
+* Version/版本 : 2.6.2
+* Release Date/发布日期 : 2023/05/26
 
 ```
-pip install tkintertools-dev==2.6.1
+pip install tkintertools-dev==2.6.2
 ```
 
 这个是作者正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
 开发版本没有对应的文档，大家可以在 issue 中提出建议，我会适当采纳一些并在开发版本中更改或实现。
 
 Description/模块说明
 ----------------------
@@ -82,15 +96,15 @@
 
 tkintertools 模块还具有一些特色的功能：
 
 * 利用 tkinter 和 tkintertools 创建的程序，在高分辨率的情况下，tkintertools 的会更加清晰（这点对于笔记本用户很友好，比如我）
 * 可以迅速实现渐变色的效果
 * 窗口缩放，所有的控件的大小跟着缩放（当然，也可以设置为不跟随缩放）
 
-注意：需要 Python3.7 及更高版本才能运行 tkintertools！
+注意：需要 **Python3.7** 及更高版本才能运行 tkintertools！
 
 Provides/模块功能
 -------------------
 
 Here, only the more distinctive features will be listed  
 这里只会列举出比较具有特色的功能
 
@@ -120,27 +134,27 @@
 见 [DPI 级别设置函数](#DPI)
 
 ### Detailed type hints/详细的类型提示
 
 参考 [PEP 526](https://peps.python.org/pep-0526/)、[PEP 586](https://peps.python.org/pep-0586/)、[PEP 604](https://peps.python.org/pep-0604/) 和 [PEP 612](https://peps.python.org/pep-0612/)，我采用了最兼容的方式去实现详细的类型提示，可适用 IDE 有 VScode、Pycharm 等。  
 那什么是类型提示呢？话不多说，直接看图就行：
 
-<p><img height="350px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/type_hint_vscode.png" alt="type_hint.png"/></p>
+![type_hint.png](docs/images/type_hint_vscode.png)
 
 在 VSCode 编辑器中，当鼠标移至类或者函数的名字上面时，会自动显示该类或者函数的注释文档。通过这种方式，不需要看太多的帮助文档和资料就能熟练地使用 tkintertools 模块！
 
 ### Across Platforms/跨平台
 
 [test.py](./test.py) 在 Windows 系统（Windows10）上运行的界面如下：
 
-<p><img height="383px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/test_win32.png" alt="test_win32.png"/></p>
+![test_win32.png](docs/images/test_win32.png)
 
 [test.py](./test.py) 在 Linux 系统（Ubuntu22.04）上运行的界面如下：
 
-<p><img height="408px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/test_linux.png" alt="test_linux.png"/></p>
+![test_linux.png](docs/images/test_linux.png)
 
 Contents/模块内容
 -------------------
 
 Each non internal class and function in the module will be described in detail here  
 这里会详细说明模块中的每个非内部类和函数
 
@@ -160,24 +174,24 @@
 
 ### Virtual Canvas Widget/虚拟画布控件
 
 1. `Label`: 标签控件
 
     标签控件的功能和`tkinter.Label`的功能类似，但更加的多元化  
     下面是`Label`控件的外观：  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/LabelTest.png" alt="LabelTest.png" /></p>
+
+    ![LabelTest.png](docs/images/LabelTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('LabelTest', 1000, 400)
-    canvas = tkt.Canvas(root, 1000, 400)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 1000, 400, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -194,25 +208,25 @@
     ```
 
     </details>
 
 2. `Button`: 按钮控件
 
     按钮控件相较于`tkinter.Button`，其自由度更高，`tkinter.Button`只有在按下的时候才能触发绑定的关联事件，而`Button`却可以在鼠标移至按钮上方时、鼠标按下时、鼠标松开时都可以绑定关联事件  
-    下面是`Button`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ButtonTest.png" alt="ButtonTest.png" /></p>
+    下面是`Button`控件的外观：
+
+    ![ButtonTest.png](docs/images/ButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ButtonTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -230,24 +244,24 @@
 
     </details>
 
 3. `CheckButton`: 复选框控件
 
     复选框控件相对于`tkinter`原生的`tkinter.CheckButton`在使用方面更加地简单，同时颜值也上升了不少  
     下面是`CheckButton`控件的外观：
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/CheckButtonTest.png" alt="CheckButtonTest.png"/></p>
+
+    ![CheckButtonTest.png](docs/images/CheckButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('CheckButtonTest', 500, 300)
-    canvas = tkt.Canvas(root, 500, 300)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 300, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -265,25 +279,25 @@
     ```
 
     </details>
 
 4. `Entry`: 输入框控件
 
     输入框控件可以轻松地设置输入的文本位置（靠左、居中和靠右），同时，它可以在鼠标移至输入框上方、鼠标未在输入框上方两种状态显示不同的默认文本  
-    下面是`Entry`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/EntryTest.png" alt="EntryTest.png" /></p>
+    下面是`Entry`控件的外观：
+
+    ![EntryTest.png](docs/images/EntryTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('EntryTest', 500, 400)
-    canvas = tkt.Canvas(root, 500, 400)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 400, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -297,39 +311,39 @@
         'RightEntry', 'Enter'), justify='right')
     tkt.Entry(canvas, 270, 20, 200, 30, radius=8, text='LeftEntry')
     tkt.Entry(canvas, 270, 55, 200, 30, radius=8,
             text='CenterEntry', justify='center')
     tkt.Entry(canvas, 270, 90, 200, 30, radius=8,
             text='RightEntry', justify='right')
     tkt.Entry(canvas, 100, 150, 300, 35, text=('PasswordEntry',
-            'Click To Enter'), justify='center', show='•')
+            'Click To Enter'), justify='center', show='●')
     tkt.Entry(canvas, 100, 200, 300, 35, text='DisableEntry',
             justify='center').set_live(False)
     tkt.Entry(canvas, 100, 250, 300, 35, text='TransparentEntry',
             justify='center', color_fill=tkt.COLOR_NONE)
 
     root.mainloop()
     ```
 
     </details>
 
 5. `Text`: 文本框控件
 
     文本框类似于输入框，这里就不再赘述  
-    下面是`Text`控件的外观：  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/TextTest.png" alt="TextTest.png" /></p>
+    下面是`Text`控件的外观：
+
+    ![TextTest.png](docs/images/TextTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('TextTest', 1000, 400)
-    canvas = tkt.Canvas(root, 1000, 400)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 1000, 400, 0, 0)
 
 
     def colorful(x, y, width, height) -> None:  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -347,36 +361,35 @@
     ```
 
     </details>
 
 6. `Progressbar`: 进度条控件
 
     进度条控件相比`tkinter.ttk.Progressbar`，外观上的自由度较大  
-    下面是`Progressbar`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ProgressbarTest.png" alt="ProgressbarTest.png" /></p>
+    下面是`Progressbar`控件的外观：
+
+    ![ProgressbarTest.png](docs/images/ProgressbarTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ProgressbarTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height) -> None:  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
 
 
     colorful(30, 290, 440, 50)
-
     tkt.Progressbar(canvas, 50, 50, 400, 30)
     tkt.Progressbar(canvas, 50, 100, 400, 30).load(.6667)
     tkt.Progressbar(canvas, 50, 150, 400, 30, borderwidth=5).load(1)
     (_ := tkt.Progressbar(canvas, 50, 200, 400, 30)).load(0.3333)
     _.set_live(False)
     tkt.Progressbar(canvas, 50, 250, 400, 30, color_bar=(
         'lightyellow', 'skyblue')).load(.5)
@@ -410,25 +423,25 @@
 
     单例模式，不用介绍了吧？通过继承它来使用
 
 ### Tool Function/工具函数
 
 1. `move`: <a name="move">移动函数</a>
 
-    移动函数可以轻松地按一定的规律、移动速度、移动时间去移动`tkintertools`模块内的所有对象，同时兼容了`tkinter`内的对象，即`tkinter`中的对象也可以很方便地移动，甚至它还可以移动窗口的位置！  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/MoveTest.gif" alt="MoveTest.gif" /></p>
+    移动函数可以轻松地按一定的规律、移动速度、移动时间去移动`tkintertools`模块内的所有对象，同时兼容了`tkinter`内的对象，即`tkinter`中的对象也可以很方便地移动，甚至它还可以移动窗口的位置！
+
+    ![MoveTest.gif](docs/images/MoveTest.gif)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('MoveTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
     rect = canvas.create_rectangle(50, 350, 150, 450)
 
 
     def move_window(switch=[True]):  # type: (list[bool]) -> None
         tkt.move(root, None, 1000 if switch[0] else -1000, 0, 800, mode='flat')
         switch[0] = not switch[0]
 
@@ -447,15 +460,14 @@
     tkt.Button(canvas, 50, 50, 200, 40, radius=10,
             text='MoveWindow', command=move_window)
     tkt.Button(canvas, 50, 100, 200, 40, radius=10,
             text='MoveRect', command=move_rect)
     button = tkt.Button(canvas, 50, 150, 200, 40, radius=10,
                         text='MoveButton', command=move_button)
 
-
     root.mainloop()
     ```
 
     </details>
 
 2. `text`: 文本函数
 
@@ -465,26 +477,27 @@
     `left`   : "tkintertools        "  
     `center` : "    tkintertools    "  
     `right`  : "        tkintertools"</pre>
 
 3. `color`: <a name="Gradient">颜色函数</a>
 
     颜色函数可以轻松求出一个颜色到另外一个颜色的过渡颜色，因此可以轻松得到渐变色的效果，同时，改变传入的参数还可以得到传入颜色的对比色  
-    第二张图是 test.py 在图像测试中绘制的图案  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ColorTest.png" alt="ColorTest.png" />
-    <img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/Test_Draw.png" alt="Test_Draw.png" /></p>
+    第二张图是 test.py 在图像测试中绘制的图案
+
+    ![ColorTest.png](docs/images/ColorTest.png)
+
+    ![Test_Draw.png](docs/images/Test_Draw.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ColorTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#00FF00'), i/width)
             color_2 = tkt.color(('#FFFFFF', '#000000'), i/width)
@@ -504,18 +517,22 @@
     `askfont`函数可以打开默认的字体选择窗口，这个窗口虽然是默认的，但它实际上无法在`tkinter`中打开，因为`tkinter`并没有对应的 API 能够做到这一点。但是，`tkintertools`调用并封装了原生的 tcl 的命令，使得字体选择框能够被我们使用。
 
     <p><img width="540px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/font.png" alt="font.png" /></p>
 
 5. `SetProcessDpiAwareness`: <a name="DPI">DPI 级别设置函数</a>
 
     这个函数实际上只是对函数`ctypes.WinDLL('shcore').SetProcessDpiAwareness`的一个简单包装，其值可为 0、1 和 2，分别代表程序 DPI 的不同级别，那么缩放效果也就不同，`tkintertools`选择的值是 1，但程序默认值实际为 0  
-    下面是执行了这个函数的效果
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/SetProcessDpiAwareness_0.png" alt="SetProcessDpiAwareness_1.png" /></p>
-    <p>下面是未执行这个函数的效果</p>
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/SetProcessDpiAwareness_1.png" alt="SetProcessDpiAwareness_0.png" /></p>
+    下面是未执行这个函数的效果
+    
+    ![SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
+
+    <p>下面是执行了这个函数的效果</p>
+
+    ![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
+
     从上面的两张图中可以很明显的看出第一张很模糊，第二张很清晰，这就是 DPI 级别不同的原因，不过这一点在屏幕缩放比不是 100% 的时候才会出现  
     大家对上面的图肯定很熟悉，这不就是 IDLE 吗！？对，这个的问题的解决办法也是来自于 IDLE 的源代码 [pyshell.py line 18~20]  
     注意：该函数在程序的不同位置执行的效果不一样！一般用在`mainloop`之前，但`tkintertools`已经在`mainloop`函数中嵌入了该函数，无需再设置一次 DPI 级别，此函数是为了原生`tkinter`程序用的。
 
 Examples/实战示例
 ----------------
 
@@ -557,28 +574,23 @@
 * 文章链接: 暂无
 * 代码仓库: https://gitcode.net/weixin_62651706/tester
 * 程序下载: 暂无
 * 推荐指数: 👍👍👍
 
 这个案例使用了最新稳定版的 tkintertools-v2.6.0，界面非常稳定，几乎没有 bug，完全采用 tkintertools 的控件，颜值很高，界面非常流畅。体现了 tkintertools 模块与 tkinter 模块相比在性能上的优越性！
 
-<p>
-    <img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/examples/exam3_1.png" alt="client.png"/>
-    <img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/examples/exam3_2.png" alt="client.png"/>
-</p>
+![exam3_1.png](docs/examples/exam3_1.png)
+![exam3_2.png](docs/examples/exam3_2.png)
 
 More/更多
 ---------
 
 > GitCode:  
 > https://gitcode.net/weixin_62651706/tkintertools
 
 > GitHub(Mirror/镜像):  
 > https://github.com/XiaoKang2022-CSDN/tkintertools
 
 > Column/专栏:  
 > https://blog.csdn.net/weixin_62651706/category_11600888.html
 
-> Tutorials/教程:  
-> https://xiaokang2022.blog.csdn.net/article/details/127374661
-
 还有更多内容请在 [源代码](./tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,21 +1,28 @@
+Metadata-Version: 2.1 Name: tkintertools-dev Version: 2.6.2 Summary: An
+auxiliary module of the tkinder module Home-page: https://gitcode.net/
+weixin_62651706/tkintertools Author: Xiaokang2022 Author-email:
+2951256653@qq.com License: MulanPSL-2.0 Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: Mulan Permissive Software
+License v2 (MulanPSL-2.0) Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
                             [Email] [Blog] [Author]
 Installation/æ¨¡åå®è£ ----------------------- ### Stable version/
-ç¨³å®çæ¬ * Version/çæ¬ : 2.6.0 * Release Date/åå¸æ¥æ : 2023/03/28
-``` pip install tkintertools==2.6.0 ``` æè ``` pip install tkintertools ```
+ç¨³å®çæ¬ * Version/çæ¬ : 2.6.1 * Release Date/åå¸æ¥æ : 2023/05/21
+``` pip install tkintertools==2.6.1 ``` æè ``` pip install tkintertools ```
 è¿ä¸ªæ¯ç®åçææ°çï¼æ¯è¾ç¨³å®ï¼bug
 æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã ç¨³å®çæææ¡£å¯ä»¥æ¥çï¼æ
 issue æä¼å»æ¥çå¹¶å°è¯è§£å³ issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.1 * Release Date/åå¸æ¥æ : 2023/05/21
-``` pip install tkintertools-dev==2.6.1 ```
+å¼åçæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/26
+``` pip install tkintertools-dev==2.6.2 ```
 è¿ä¸ªæ¯ä½èæ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
 å¯è½ä¼æ¯è¾å¤ã å¼åçæ¬æ²¡æå¯¹åºçææ¡£ï¼å¤§å®¶å¯ä»¥å¨ issue
 ä¸­æåºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
 Description/æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº
 tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
@@ -27,18 +34,18 @@
 ä½åæ¶ä¹äº§çäºä¸äºç¼ºç¹ï¼ * èæçæ§ä»¶æ æ³è·åç¦ç¹ *
 èæçæ§ä»¶å¨ææ¬è¾å¥åæ¾ç¤ºçåè½ä¸å­å¨ä¸äºç¼ºé·ï¼è¿ä¸ªç¼ºé·ä¸æ¯å¾ææ¾ï¼ä½å¼ºè¿«çå°±æç¹é¾åäºï¼æ¯å¦æï¼
 tkintertools æ¨¡åè¿å·æä¸äºç¹è²çåè½ï¼ * å©ç¨ tkinter å
 tkintertools åå»ºçç¨åºï¼å¨é«åè¾¨ççæåµä¸ï¼tkintertools
 çä¼æ´å æ¸æ°ï¼è¿ç¹å¯¹äºç¬è®°æ¬ç¨æ·å¾åå¥½ï¼æ¯å¦æï¼ *
 å¯ä»¥è¿éå®ç°æ¸åè²çææ *
 çªå£ç¼©æ¾ï¼ææçæ§ä»¶çå¤§å°è·çç¼©æ¾ï¼å½ç¶ï¼ä¹å¯ä»¥è®¾ç½®ä¸ºä¸è·éç¼©æ¾ï¼
-æ³¨æï¼éè¦ Python3.7 åæ´é«çæ¬æè½è¿è¡ tkintertoolsï¼ Provides/
-æ¨¡ååè½ ------------------- Here, only the more distinctive features will
-be listed è¿éåªä¼åä¸¾åºæ¯è¾å·æç¹è²çåè½ ### Customizable
-widgets/å¯èªå®ä¹çæ§ä»¶ tkintertools
+æ³¨æï¼éè¦ **Python3.7** åæ´é«çæ¬æè½è¿è¡ tkintertoolsï¼
+Provides/æ¨¡ååè½ ------------------- Here, only the more distinctive
+features will be listed è¿éåªä¼åä¸¾åºæ¯è¾å·æç¹è²çåè½ ###
+Customizable widgets/å¯èªå®ä¹çæ§ä»¶ tkintertools
 æ¨¡åçæ§ä»¶æ¥æè®¸å¤åæ°ä¾æä»¬è®¾ç½®ï¼æ¯å¦åè§çåå¾ãææ¬åè¾¹æ¡ä»¥åæ§ä»¶åé¨çé¢è²ï¼å³èäºä»¶ç­ç­ã
 è¿éè¦è¯´æçæ¯ï¼æ¯ä¸ªæ§ä»¶å¯ä»¥è®¾ç½®çå³èäºä»¶ä¸æ­¢ä¸ç§ï¼å¨é¼ æ ç»è¿æ§ä»¶æ¶å¯ä»¥ç»å®äºä»¶ï¼é¼ æ ç¹å»æ§ä»¶ä¹å¯ä»¥ï¼é¼ æ ç¹å»åæ¾å¼ä¹è¡ç­ç­ã
 ææ¬åè¾¹æ¡ä»¥åæ§ä»¶çå¡«åè²ä¹æ¯ç±»ä¼¼çï¼å¨é¼ æ ç»è¿æ§ä»¶ãç¹å»æ§ä»¶ãç¹å»åæ¾å¼é½å¯ä»¥è®¾å®é¢è²ã
 ææ¬ç±»æ§ä»¶è¿è½å¤ä»å³è¾¹éæ­¥è¾å¥ææ¬ï¼ææ¬è¾å¥æç¤ºç¬¦ä¹å¯ä»¥ä¸æ¯åè°æ è¶£çç«çº¿ï¼å¯ä»¥æ¯å¶ä»çï¼æ¯å¦ä¸åçº¿ç­ã
 æåï¼å¤§å®¶å¯ä»¥çä¸ä¸ [test.py](./test.py)
 æä»¶éé¢çç¤ºä¾ï¼è¿ä¸ªç¤ºä¾å±ç¤ºäº tkintertools
 æ¨¡åçç»å¤§é¨ååè½ï¼ç¤ºä¾ä¸­æ´æéèç âå¤å½©åå¹»â
@@ -51,117 +58,108 @@
 (#Gradient) ### Automatically adapt to DPI/èªå¨éåºDPI è§ [DPI
 çº§å«è®¾ç½®å½æ°](#DPI) ### Detailed type hints/è¯¦ç»çç±»åæç¤º åè
 [PEP 526](https://peps.python.org/pep-0526/)ã[PEP 586](https://
 peps.python.org/pep-0586/)ã[PEP 604](https://peps.python.org/pep-0604/) å
 [PEP 612](https://peps.python.org/pep-0612/
 )ï¼æéç¨äºæå¼å®¹çæ¹å¼å»å®ç°è¯¦ç»çç±»åæç¤ºï¼å¯éç¨
 IDE æ VScodeãPycharm ç­ã
-é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼
-[type_hint.png]
-å¨ VSCode
+é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼ !
+[type_hint.png](docs/images/type_hint_vscode.png) å¨ VSCode
 ç¼è¾å¨ä¸­ï¼å½é¼ æ ç§»è³ç±»æèå½æ°çåå­ä¸é¢æ¶ï¼ä¼èªå¨æ¾ç¤ºè¯¥ç±»æèå½æ°çæ³¨éææ¡£ãéè¿è¿ç§æ¹å¼ï¼ä¸éè¦çå¤ªå¤çå¸®å©ææ¡£åèµæå°±è½çç»å°ä½¿ç¨
 tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](./test.py) å¨
-Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼
-[test_win32.png]
-[test.py](./test.py) å¨ Linux
-ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼
-[test_linux.png]
-Contents/æ¨¡ååå®¹ ------------------- Each non internal class and function
-in the module will be described in detail here
+Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_win32.png]
+(docs/images/test_win32.png) [test.py](./test.py) å¨ Linux
+ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png](docs/
+images/test_linux.png) Contents/æ¨¡ååå®¹ ------------------- Each non
+internal class and function in the module will be described in detail here
 è¿éä¼è¯¦ç»è¯´ææ¨¡åä¸­çæ¯ä¸ªéåé¨ç±»åå½æ° ### Container
 Widget/å®¹å¨æ§ä»¶ 1. `Tk`: çªå£ç±»
 ç»§æ¿äº`tkinter.Tk`ï¼å¨ç»§æ¿äº`tkinter`æ¨¡åå`Tk`çåºç¡ä¸ï¼åå å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¹¶å å¥äºæ£æµçªå£å¤§å°æ¯å¦ç¼©æ¾çæºå¶ï¼ä»¥ä½¿å¾å¶å­`Canvas`åè½æ­£ç¡®å°è¿è¡ç¼©æ¾
 2. `Toplevel`: é¡¶çº§çªå£ç±»
 ç»§æ¿äº`tkinter.Toplevel`å`Tk`ï¼å å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¶ä½åä¸`Tk`ä¸æ ·
 3. `Canvas`: ç»å¸ç±»
 ç»§æ¿äº`tkinter.Canvas`ï¼å å¥äºå¯¹ç»å¸èææ§ä»¶çæ¯æï¼åæ¶æ¯åç±»ååºäºä»¶ãç¼©æ¾æ§å¶çç®¡çèï¼ä¹å¯¹`tkinter.Canvas`çå®ä¾æ¹æ³æä¸å®çå¼å®¹æ§
 ### Virtual Canvas Widget/èæç»å¸æ§ä»¶ 1. `Label`: æ ç­¾æ§ä»¶
 æ ç­¾æ§ä»¶çåè½å`tkinter.Label`çåè½ç±»ä¼¼ï¼ä½æ´å çå¤åå
-ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼
-[LabelTest.png]
+ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼ ![LabelTest.png](docs/images/LabelTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('LabelTest', 1000,
-400) canvas = tkt.Canvas(root, 1000, 400) canvas.place(x=0, y=0) def colorful
-(x, y, width, height): # type: (int, int, int, int) -> None """ Gradient colors
-""" for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Label(canvas, 50, 50, 400, 100, text='NormalLabel\nHere is the text')
 tkt.Label(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerLabel')
 tkt.Label(canvas, 550, 50, 400, 100, text='DisableLabel').set_live(False)
 tkt.Label(canvas, 550, 200, 400, 100, radius=20, text='TransparentLabel',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  2. `Button`: æé®æ§ä»¶
 æé®æ§ä»¶ç¸è¾äº`tkinter.Button`ï¼å¶èªç±åº¦æ´é«ï¼`tkinter.Button`åªæå¨æä¸çæ¶åæè½è§¦åç»å®çå³èäºä»¶ï¼è`Button`å´å¯ä»¥å¨é¼ æ ç§»è³æé®ä¸æ¹æ¶ãé¼ æ æä¸æ¶ãé¼ æ æ¾å¼æ¶é½å¯ä»¥ç»å®å³èäºä»¶
-ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼
-[ButtonTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ButtonTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) canvas.place(x=0, y=0) def colorful(x,
-y, width, height): # type: (int, int, int, int) -> None """ Gradient colors """
-for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼ ![ButtonTest.png](docs/images/
+ButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk
+('ButtonTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful
+(x, y, width, height): # type: (int, int, int, int) -> None """ Gradient colors
+""" for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 280, 400,
 100) tkt.Button(canvas, 150, 135, 200, 50, text='NormalButton') tkt.Button
 (canvas, 100, 195, 300, 50, radius=10, text='RoundCornerButton') tkt.Button
 (canvas, 150, 255, 200, 50, text='DisableButton').set_live(False) tkt.Button
 (canvas, 100, 315, 300, 50, radius=10, text='TransparentButton',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  3. `CheckButton`:
 å¤éæ¡æ§ä»¶
 å¤éæ¡æ§ä»¶ç¸å¯¹äº`tkinter`åçç`tkinter.CheckButton`å¨ä½¿ç¨æ¹é¢æ´å å°ç®åï¼åæ¶é¢å¼ä¹ä¸åäºä¸å°
-ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼
-[CheckButtonTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('CheckButtonTest',
-500, 300) canvas = tkt.Canvas(root, 500, 300) canvas.place(x=0, y=0) def
-colorful(x, y, width, height): # type: (int, int, int, int) -> None """
+ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼ ![CheckButtonTest.png](docs/images/
+CheckButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root =
+tkt.Tk('CheckButtonTest', 500, 300) canvas = tkt.Canvas(root, 500, 300, 0, 0)
+def colorful(x, y, width, height): # type: (int, int, int, int) -> None """
 Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
 '#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
 colorful(40, 190, 420, 50) tkt.CheckButton(canvas, 50, 50, 30,
 text='NormalCheckButton', value=True) tkt.CheckButton(canvas, 50, 100, 30,
 text='DisableCheckButton', value=True).set_live(False) tkt.CheckButton(canvas,
 50, 150, 30, radius=10, text='RoundCornerCheckButton') tkt.CheckButton(canvas,
 50, 200, 30, radius=15, text='TransparentCheckButton',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  4. `Entry`: è¾å¥æ¡æ§ä»¶
 è¾å¥æ¡æ§ä»¶å¯ä»¥è½»æ¾å°è®¾ç½®è¾å¥çææ¬ä½ç½®ï¼é å·¦ãå±ä¸­åé å³ï¼ï¼åæ¶ï¼å®å¯ä»¥å¨é¼ æ ç§»è³è¾å¥æ¡ä¸æ¹ãé¼ æ æªå¨è¾å¥æ¡ä¸æ¹ä¸¤ç§ç¶ææ¾ç¤ºä¸åçé»è®¤ææ¬
-ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼
-[EntryTest.png]
+ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼ ![EntryTest.png](docs/images/EntryTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('EntryTest', 500,
-400) canvas = tkt.Canvas(root, 500, 400) canvas.place(x=0, y=0) def colorful(x,
-y, width, height): # type: (int, int, int, int) -> None """ Gradient colors """
-for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+400) canvas = tkt.Canvas(root, 500, 400, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 193, 400,
 100) tkt.Entry(canvas, 20, 20, 200, 30, text=('LeftEntry', 'Enter')) tkt.Entry
 (canvas, 20, 55, 200, 30, text=( 'CenterEntry', 'Enter'), justify='center')
 tkt.Entry(canvas, 20, 90, 200, 30, text=( 'RightEntry', 'Enter'),
 justify='right') tkt.Entry(canvas, 270, 20, 200, 30, radius=8,
 text='LeftEntry') tkt.Entry(canvas, 270, 55, 200, 30, radius=8,
 text='CenterEntry', justify='center') tkt.Entry(canvas, 270, 90, 200, 30,
 radius=8, text='RightEntry', justify='right') tkt.Entry(canvas, 100, 150, 300,
-35, text=('PasswordEntry', 'Click To Enter'), justify='center', show='â¢')
+35, text=('PasswordEntry', 'Click To Enter'), justify='center', show='â')
 tkt.Entry(canvas, 100, 200, 300, 35, text='DisableEntry',
 justify='center').set_live(False) tkt.Entry(canvas, 100, 250, 300, 35,
 text='TransparentEntry', justify='center', color_fill=tkt.COLOR_NONE)
 root.mainloop() ```  5. `Text`: ææ¬æ¡æ§ä»¶
 ææ¬æ¡ç±»ä¼¼äºè¾å¥æ¡ï¼è¿éå°±ä¸åèµè¿°
-ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼
-[TextTest.png]
+ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼ ![TextTest.png](docs/images/TextTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('TextTest', 1000,
-400) canvas = tkt.Canvas(root, 1000, 400) canvas.place(x=0, y=0) def colorful
-(x, y, width, height) -> None: # type: (int, int, int, int) -> None """
-Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
-'#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
-colorful(510, 175, 480, 150) tkt.Text(canvas, 50, 50, 400, 100, text=
-('NormalText(Left)', 'Click To Enter')) tkt.Text(canvas, 50, 200, 400, 100,
-radius=20, text='RoundCornerText(Center)', justify='center') tkt.Text(canvas,
-550, 50, 400, 100, text='DisableText').set_live(False) tkt.Text(canvas, 550,
-200, 400, 100, radius=20, text='TransparentText(Right)', justify='right',
+400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
+height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
+for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
+150) tkt.Text(canvas, 50, 50, 400, 100, text=('NormalText(Left)', 'Click To
+Enter')) tkt.Text(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerText
+(Center)', justify='center') tkt.Text(canvas, 550, 50, 400, 100,
+text='DisableText').set_live(False) tkt.Text(canvas, 550, 200, 400, 100,
+radius=20, text='TransparentText(Right)', justify='right',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  6. `Progressbar`:
 è¿åº¦æ¡æ§ä»¶
 è¿åº¦æ¡æ§ä»¶ç¸æ¯`tkinter.ttk.Progressbar`ï¼å¤è§ä¸çèªç±åº¦è¾å¤§
-ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼
-[ProgressbarTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ProgressbarTest',
-500, 500) canvas = tkt.Canvas(root, 500, 500) canvas.place(x=0, y=0) def
-colorful(x, y, width, height) -> None: # type: (int, int, int, int) -> None """
-Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
+ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼ ![ProgressbarTest.png](docs/images/
+ProgressbarTest.png) æºä»£ç  ```python import tkintertools as tkt root =
+tkt.Tk('ProgressbarTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0)
+def colorful(x, y, width, height) -> None: # type: (int, int, int, int) -> None
+""" Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
 '#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
 colorful(30, 290, 440, 50) tkt.Progressbar(canvas, 50, 50, 400, 30)
 tkt.Progressbar(canvas, 50, 100, 400, 30).load(.6667) tkt.Progressbar(canvas,
 50, 150, 400, 30, borderwidth=5).load(1) (_ := tkt.Progressbar(canvas, 50, 200,
 400, 30)).load(0.3333) _.set_live(False) tkt.Progressbar(canvas, 50, 250, 400,
 30, color_bar=( 'lightyellow', 'skyblue')).load(.5) tkt.Progressbar(canvas, 50,
 300, 400, 30, color_bar=('', 'orange')).load(.1667) progressbar =
@@ -175,59 +173,58 @@
 å¨å¾æå¾å¥½çæ¯æï¼ä»éæå°éä»£ç å³å¯å®ç°å¨å¾çæ¾ç¤ºï¼è¿å¯ä»¥è®¾ç½®å¨å¾æ¾ç¤ºçéåº¦ï¼æ­¤å¤ï¼å¯¹
 png
 ç±»åçå¾ççæ¯æä¹æå¼ºåï¼å¯ä»¥å¨ä¸ä¾èµä»»ä½ç¬¬ä¸æ¹æ¨¡åæèåºçæåµä¸ï¼å¯¹
 png å¾çè¿è¡ç¼©æ¾ 2. `Singleton`: åä¾æ¨¡å¼ç±»
 åä¾æ¨¡å¼ï¼ä¸ç¨ä»ç»äºå§ï¼éè¿ç»§æ¿å®æ¥ä½¿ç¨ ### Tool Function/
 å·¥å·å½æ° 1. `move`: ç§»å¨å½æ°
 ç§»å¨å½æ°å¯ä»¥è½»æ¾å°æä¸å®çè§å¾ãç§»å¨éåº¦ãç§»å¨æ¶é´å»ç§»å¨`tkintertools`æ¨¡ååçææå¯¹è±¡ï¼åæ¶å¼å®¹äº`tkinter`åçå¯¹è±¡ï¼å³`tkinter`ä¸­çå¯¹è±¡ä¹å¯ä»¥å¾æ¹ä¾¿å°ç§»å¨ï¼çè³å®è¿å¯ä»¥ç§»å¨çªå£çä½ç½®ï¼
-[MoveTest.gif]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('MoveTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) canvas.place(x=0, y=0) rect =
-canvas.create_rectangle(50, 350, 150, 450) def move_window(switch=[True]): #
-type: (list[bool]) -> None tkt.move(root, None, 1000 if switch[0] else -1000,
-0, 800, mode='flat') switch[0] = not switch[0] def move_button(switch=[True]) -
-> None: # type: (list[bool]) -> None tkt.move(canvas, button, 200 if switch[0]
-else -200, 0, 500, mode='rebound') switch[0] = not switch[0] def move_rect
-(switch=[True]): # type: (list[bool]) -> None tkt.move(canvas, rect, 200 if
-switch[0] else -200, 0, 500, mode='smooth') switch[0] = not switch[0]
-tkt.Button(canvas, 50, 50, 200, 40, radius=10, text='MoveWindow',
-command=move_window) tkt.Button(canvas, 50, 100, 200, 40, radius=10,
-text='MoveRect', command=move_rect) button = tkt.Button(canvas, 50, 150, 200,
-40, radius=10, text='MoveButton', command=move_button) root.mainloop() ```  2.
-`text`: ææ¬å½æ°
+![MoveTest.gif](docs/images/MoveTest.gif) æºä»£ç  ```python import
+tkintertools as tkt root = tkt.Tk('MoveTest', 500, 500) canvas = tkt.Canvas
+(root, 500, 500, 0, 0) rect = canvas.create_rectangle(50, 350, 150, 450) def
+move_window(switch=[True]): # type: (list[bool]) -> None tkt.move(root, None,
+1000 if switch[0] else -1000, 0, 800, mode='flat') switch[0] = not switch[0]
+def move_button(switch=[True]) -> None: # type: (list[bool]) -> None tkt.move
+(canvas, button, 200 if switch[0] else -200, 0, 500, mode='rebound') switch[0]
+= not switch[0] def move_rect(switch=[True]): # type: (list[bool]) -> None
+tkt.move(canvas, rect, 200 if switch[0] else -200, 0, 500, mode='smooth')
+switch[0] = not switch[0] tkt.Button(canvas, 50, 50, 200, 40, radius=10,
+text='MoveWindow', command=move_window) tkt.Button(canvas, 50, 100, 200, 40,
+radius=10, text='MoveRect', command=move_rect) button = tkt.Button(canvas, 50,
+150, 200, 40, radius=10, text='MoveButton', command=move_button) root.mainloop
+() ```  2. `text`: ææ¬å½æ°
 å¯ä»¥å¿«éå¹¶æ¹ä¾¿å°å¾å°ä¸ä¸ªåæ°é¿åº¦çå­ç¬¦ä¸²ï¼ä¸å­ç¬¦ä¸²çåå®¹å¯ä»¥æå®ä½ç½®
 å¦ï¼å¾å°ä¸ä¸ª 20 é¿åº¦çå­ç¬¦ä¸² âtkintertoolsâ
     `left`   : "tkintertools        "
     `center` : "    tkintertools    "
     `right`  : "        tkintertools"
 3. `color`: é¢è²å½æ°
 é¢è²å½æ°å¯ä»¥è½»æ¾æ±åºä¸ä¸ªé¢è²å°å¦å¤ä¸ä¸ªé¢è²çè¿æ¸¡é¢è²ï¼å æ­¤å¯ä»¥è½»æ¾å¾å°æ¸åè²çææï¼åæ¶ï¼æ¹åä¼ å¥çåæ°è¿å¯ä»¥å¾å°ä¼ å¥é¢è²çå¯¹æ¯è²
-ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡
-[ColorTest.png] [Test_Draw.png]
+ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡ ![ColorTest.png]
+(docs/images/ColorTest.png) ![Test_Draw.png](docs/images/Test_Draw.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ColorTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) canvas.place(x=0, y=0) def colorful(x,
-y, width, height): # type: (int, int, int, int) -> None """ Gradient colors """
-for i in range(width): color = tkt.color(('#FF0000', '#00FF00'), i/width)
-color_2 = tkt.color(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y,
-x+i, y+height, fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 +
-i/3, outline=color_2, width=2) colorful(50, 50, 400, 100) root.mainloop() ```
-4. `askfont`: å­ä½éæ©å¯¹è¯æ¡
+500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 =
+tkt.color(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i,
+y+height, fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
+outline=color_2, width=2) colorful(50, 50, 400, 100) root.mainloop() ```  4.
+`askfont`: å­ä½éæ©å¯¹è¯æ¡
 `askfont`å½æ°å¯ä»¥æå¼é»è®¤çå­ä½éæ©çªå£ï¼è¿ä¸ªçªå£è½ç¶æ¯é»è®¤çï¼ä½å®å®éä¸æ æ³å¨`tkinter`ä¸­æå¼ï¼å ä¸º`tkinter`å¹¶æ²¡æå¯¹åºç
 API è½å¤åå°è¿ä¸ç¹ãä½æ¯ï¼`tkintertools`è°ç¨å¹¶å°è£äºåçç
 tcl çå½ä»¤ï¼ä½¿å¾å­ä½éæ©æ¡è½å¤è¢«æä»¬ä½¿ç¨ã
 [font.png]
 5. `SetProcessDpiAwareness`: DPI çº§å«è®¾ç½®å½æ°
 è¿ä¸ªå½æ°å®éä¸åªæ¯å¯¹å½æ°`ctypes.WinDLL
 ('shcore').SetProcessDpiAwareness`çä¸ä¸ªç®ååè£ï¼å¶å¼å¯ä¸º 0ã1
 å 2ï¼åå«ä»£è¡¨ç¨åº DPI
 çä¸åçº§å«ï¼é£ä¹ç¼©æ¾ææä¹å°±ä¸åï¼`tkintertools`éæ©çå¼æ¯
-1ï¼ä½ç¨åºé»è®¤å¼å®éä¸º 0 ä¸é¢æ¯æ§è¡äºè¿ä¸ªå½æ°çææ
-[SetProcessDpiAwareness_1.png]
-ä¸é¢æ¯æªæ§è¡è¿ä¸ªå½æ°çææ
-[SetProcessDpiAwareness_0.png]
+1ï¼ä½ç¨åºé»è®¤å¼å®éä¸º 0 ä¸é¢æ¯æªæ§è¡è¿ä¸ªå½æ°çææ !
+[SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
+ä¸é¢æ¯æ§è¡äºè¿ä¸ªå½æ°çææ
+![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
 ä»ä¸é¢çä¸¤å¼ å¾ä¸­å¯ä»¥å¾ææ¾ççåºç¬¬ä¸å¼ å¾æ¨¡ç³ï¼ç¬¬äºå¼ å¾æ¸æ°ï¼è¿å°±æ¯
 DPI çº§å«ä¸åçåå ï¼ä¸è¿è¿ä¸ç¹å¨å±å¹ç¼©æ¾æ¯ä¸æ¯ 100%
 çæ¶åæä¼åºç° å¤§å®¶å¯¹ä¸é¢çå¾è¯å®å¾çæï¼è¿ä¸å°±æ¯ IDLE
 åï¼ï¼å¯¹ï¼è¿ä¸ªçé®é¢çè§£å³åæ³ä¹æ¯æ¥èªäº IDLE çæºä»£ç 
 [pyshell.py line 18~20]
 æ³¨æï¼è¯¥å½æ°å¨ç¨åºçä¸åä½ç½®æ§è¡çææä¸ä¸æ ·ï¼ä¸è¬ç¨å¨`mainloop`ä¹åï¼ä½`tkintertools`å·²ç»å¨`mainloop`å½æ°ä¸­åµå¥äºè¯¥å½æ°ï¼æ éåè®¾ç½®ä¸æ¬¡
 DPI çº§å«ï¼æ­¤å½æ°æ¯ä¸ºäºåç`tkinter`ç¨åºç¨çã Examples/
@@ -256,15 +253,13 @@
 æ¨¡åçå¼å®¹æ§ï¼
 [chess.png] [chess.png]
 ### ç®æç»å½çé¢ * æç« é¾æ¥: ææ  * ä»£ç ä»åº: https://
 gitcode.net/weixin_62651706/tester * ç¨åºä¸è½½: ææ  * æ¨èææ°:
 ððð è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
-æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼
-[client.png] [client.png]
-More/æ´å¤ --------- > GitCode: > https://gitcode.net/weixin_62651706/
-tkintertools > GitHub(Mirror/éå): > https://github.com/XiaoKang2022-CSDN/
-tkintertools > Column/ä¸æ : > https://blog.csdn.net/weixin_62651706/
-category_11600888.html > Tutorials/æç¨: > https://
-xiaokang2022.blog.csdn.net/article/details/127374661 è¿ææ´å¤åå®¹è¯·å¨
-[æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
+æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png](docs/
+examples/exam3_1.png) ![exam3_2.png](docs/examples/exam3_2.png) More/æ´å¤ ---
+------ > GitCode: > https://gitcode.net/weixin_62651706/tkintertools > GitHub
+(Mirror/éå): > https://github.com/XiaoKang2022-CSDN/tkintertools > Column/
+ä¸æ : > https://blog.csdn.net/weixin_62651706/category_11600888.html
+è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
```

### Comparing `tkintertools_dev-2.6.1/setup.py` & `tkintertools-dev-2.6.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 """ 上传 pypi """
 
 import setuptools
 
-from tkintertools import __version__
-
-mode = 1
-# 0 : 正式版
-# 1 : 开发版
-# 2 : 测试版
-
-name = ('tkintertools', 'tkintertools_dev', 'tkintertools_test')[mode]
-version = __version__ if mode == 0 else input(
-    '输入%s版本号: ' % ('开发' if mode == 1 else '测试'))
 
 setuptools.setup(
-    name=name,
-    version=version,
+    name='tkintertools-dev',
+    version="2.6.2",
     author='Xiaokang2022',
+    license='MulanPSL-2.0',
     author_email='2951256653@qq.com',
     description='An auxiliary module of the tkinder module',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://gitcode.net/weixin_62651706/tkintertools',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)',
         'Operating System :: OS Independent',
     ],
 )
 
 # python -m pip install --user --upgrade setuptools wheel [检查更新]
+
 # python setup.py sdist bdist_wheel [打包]
 # twine upload dist/* [上传]
 
 # pip install -U pypistats [数据分析]
 # pip install socksio [数据分析]
 
 # pypistats overall tkintertools [数据分析]
```

### Comparing `tkintertools_dev-2.6.1/tkintertools/__init__.py` & `tkintertools-dev-2.6.2/tkintertools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,21 +33,20 @@
 if sys.version_info < (3, 7):  # Version Check
     error_info = '\n\033[31mOperation Requirements: \033[32m\nPython version shall not be less than\033[33m 3.7.0 !\033[0m'
     raise RuntimeError(error_info)
 
 from .__main__ import (Button, Canvas, CheckButton, Entry, Label, PhotoImage,
                        Progressbar, SetProcessDpiAwareness, Singleton, Text,
                        Tk, Toplevel, askfont, color, move, text)
-from .constants import *
 
 __author__ = 'Xiaokang2022<2951256653@qq.com>'
 __version__ = '2.6.1'
 __all__ = [
     # Container Widgets
     'Tk', 'Toplevel', 'Canvas',
     # Virtual Canvas Widgets
     'Label', 'Button', 'CheckButton', 'Entry', 'Text', 'Progressbar',
     # Tool Classes
     'PhotoImage', 'Singleton',
     # Tool Functions
-    'move', 'text', 'color', 'askfont', 'SetProcessDpiAwareness'
+    'move', 'text', 'color', 'askfont', 'SetProcessDpiAwareness',
 ]
```

### Comparing `tkintertools_dev-2.6.1/tkintertools/__main__.py` & `tkintertools-dev-2.6.2/tkintertools/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Main File """
 
-import math  # 数学函数
+import math  # 数学支持
 import sys  # DPI 兼容
 import tkinter  # 基础模块
 from fractions import Fraction  # 图片缩放
 from typing import Any, Callable, Generator, Iterable  # 类型提示
 
 try:  # NOTE: 为了兼容 Python3.7，从 typing_extensions 引入 Literal 而不是 typing
     from typing_extensions import Literal
@@ -41,27 +41,26 @@
         `y`: 窗口左上角纵坐标\n
         `shutdown`: 关闭窗口之前执行的函数，但会覆盖原关闭操作\n
         `**kw`: 与 tkinter.Tk 类的参数相同\n
         """
         if type(self) == Tk:  # NOTE:方便后面的 Toplevel 类继承
             tkinter.Tk.__init__(self, **kw)
 
-        self.width: list[int] = [100, 1]  # [初始宽度, 当前宽度]
-        self.height: list[int] = [100, 1]  # [初始高度, 当前高度]
-        self._canvas: list[Canvas] = []  # 子画布列表
+        self.width = [100, 1]  # type: list[int]  # [初始宽度, 当前宽度]
+        self.height = [100, 1]  # type: list[int]  # [初始高度, 当前高度]
+        self._canvas = []  # type: list[Canvas]  # 子画布列表
 
         if width and height:
-            if x != None and y != None:
+            if x is not None and y is not None:  # BUG: 可能需要修改
                 self.geometry('%dx%d+%d+%d' % (width, height, x, y))
             else:
                 self.geometry('%dx%d' % (width, height))
 
         self.title(title if title else None)
         self.protocol('WM_DELETE_WINDOW', shutdown if shutdown else None)
-
         self.bind('<Configure>', lambda _: self.__zoom())  # 开启窗口缩放检测
 
     def canvas(self):  # type: () -> tuple[Canvas]
         """ 返回`Tk`类的`Canvas`元组 """
         return tuple(self._canvas)
 
     def __zoom(self):  # type: () -> None
@@ -98,15 +97,15 @@
     def mainloop(
         self,
         n=0,  # type: int
         *,
         dpi_awareness=1  # type: Literal[1, 2, 3]
     ):  # type: (...) -> None
         """
-        Call the mainloop of Tk.\n
+        根（主）窗口的消息循环\n
         `dpi_awareness`: 程序的DPI级别，值可以为0、1和2，程序默认为0，默认值为1
         """
         SetProcessDpiAwareness(dpi_awareness)
         return tkinter.Tk.mainloop(self, n)
 
 
 class Toplevel(tkinter.Toplevel, Tk):
@@ -140,52 +139,60 @@
 
 
 class Canvas(tkinter.Canvas):
     """ 用于承载虚拟的画布控件，并处理部分绑定事件 """
 
     def __init__(
         self,
-        master,  # type: Tk
+        master,  # type: Tk | Toplevel
         width,  # type: int
         height,  # type: int
+        x=None,  # type: int | None
+        y=None,  # type: int | None
         *,
         lock=True,  # type: bool
         expand=True,  # type: bool
         keep=False,  # type: bool
         **kw
     ):  # type: (...) -> None
         """
         `master`: 父控件\n
         `width`: 画布宽度\n
         `height`: 画布高度\n
+        `x`: 画布左上角的横坐标\n
+        `y`: 画布左上角的纵坐标\n
         `lock`: 画布内控件的功能锁，False 时功能暂时失效\n
         `expand`: 画布内控件是否能缩放\n
-        `keep`: 保持画布比例不变\n
+        `keep`: 画布比例是否保持不变\n
         `**kw`: 与 tkinter.Canvas 类的参数相同\n
         """
         self.width = [width]*2  # [初始宽度, 当前宽度]
         self.height = [height]*2  # [初始高度, 当前高度]
         self._lock = lock
         self.expand = expand
         self.keep = keep
 
+        self.master = master  # type: Tk | Toplevel  # NOTE: 此语句虽冗余，实则为类型提示
+
         self.rx = 1.  # 横向放缩比率
         self.ry = 1.  # 纵向放缩比率
-        self._widget: list[BaseWidget] = []  # 子控件列表（与事件绑定有关）
+        self._widget = []  # type: list[BaseWidget]  # 子控件列表（与事件绑定有关）
         self._font = {}  # type: dict[tkinter._CanvasItemId, float]
         self._image = {}  # type: dict[tkinter._CanvasItemId, list]
 
         tkinter.Canvas.__init__(
             self, master, width=width, height=height, highlightthickness=0, **kw)
 
         if not (kw.get('bg', None) or kw.get('background', None)):
             # Linux 系统上背景默认值不是 #F1F1F1，影响模块默认值的效果
             self.configure(bg=BACKGROUND)
 
         master._canvas.append(self)  # 将实例添加到 Tk 的画布列表中
+        if x is not None and y is not None:
+            self.place(x=x, y=y)
 
         self.bind('<Motion>', self.__touch)  # 绑定鼠标触碰控件
         self.bind('<Any-Key>', self.__input)  # 绑定键盘输入字符（和Ctrl+v的代码顺序不可错）
         self.bind('<Button-1>', self.__click)  # 绑定鼠标左键按下
         self.bind('<B1-Motion>', self.__click)  # 绑定鼠标左键按下移动
         self.bind('<MouseWheel>', self.__mousewheel)  # 绑定鼠标滚轮滚动
         self.bind('<ButtonRelease-1>', self.__release)  # 绑定鼠标左键松开
@@ -333,20 +340,20 @@
         return item
 
     def itemconfigure(
         self,
         tagOrId,  # type: str | tkinter._CanvasItemId
         **kw
     ):  # type: (...) -> dict[str, tuple[str, str, str, str, str]] | None
-        # 重写：创建空image的_CanvasItemId时漏去对图像大小的控制
+        # 重写：创建空 image 的 _CanvasItemId 时漏去对图像大小的控制
         if type(kw.get('image')) == PhotoImage:
             self._image[tagOrId] = [kw.get('image'), None]
         return tkinter.Canvas.itemconfigure(self, tagOrId, **kw)
 
-    def place(self, *args, **kw):  # type: (...) -> None
+    def place(self, *args, **kw):  # type: (...) -> None  # BUG: 缩放就会恢复原样
         # 重写：增加一些特定功能
         self.width[0] = kw.get('wdith', self.width[0])
         self.height[0] = kw.get('height', self.height[0])
         return tkinter.Canvas.place(self, *args, **kw)
 
     def destroy(self):  # type: () -> None
         # 重写：兼容
@@ -374,41 +381,49 @@
         image,  # type: PhotoImage | None
         color_text,  # type: tuple[str, str, str]
         color_fill,  # type: tuple[str, str, str]
         color_outline  # type: tuple[str, str, str]
     ):  # type: (...) -> None
         """
         ### 标准参数
+        标准参数是所有控件都有的\n
+        ---
         `canvas`: 父画布容器控件\n
         `x`: 控件左上角的横坐标\n
         `y`: 控件左上角的纵坐标\n
         `width`: 控件的宽度\n
         `height`: 控件的高度\n
         `radius`: 控件圆角化半径\n
         `text`: 控件显示的文本，对于文本控件而言，可以为一个元组：(默认文本, 鼠标触碰文本)\n
         `justify`: 文本的对齐方式\n
         `borderwidth`: 外框的宽度\n
         `font`: 控件的字体设定 (字体, 大小, 样式)\n
         `image`: 控件的背景（支持 png 类型，大小必须小于控件，否则会溢出）\n
         `color_text`: 控件文本的颜色\n
         `color_fill`: 控件内部的颜色\n
         `color_outline`: 控件外框的颜色\n
+        ---
         ### 特定参数
+        特定参数只有某些控件类才有\n
+        ---
         `command`: 按钮控件的关联函数\n
         `show`: 文本控件的显示文本\n
         `limit`: 文本控件的输入字数限制，为负数时表示没有字数限制\n
         `read`: 文本控件的只读模式\n
         `cursor`: 输入提示符的字符，默认为一竖线\n
+        ---
         ### 详细说明
-        字体的值为一个包含两个或三个值的元组，共两种形式\n
-        形式一: `(字体名称, 字体大小)`\n
-        形式二: `(字体名称, 字体大小, 字体样式)`\n
-        颜色为一个包含三个或四个 RGB 颜色字符串的元组，共两种形式\n
-        不使用禁用功能时: `(正常颜色, 触碰颜色, 交互颜色)`\n
-        需使用禁用功能时: `(正常颜色, 触碰颜色, 交互颜色, 禁用颜色)`\n
+        1. 字体的值为一个包含两个或三个值的元组或者单个的字符串，共三种形式\n
+            * 形式一: `字体名称`
+            * 形式二: `(字体名称, 字体大小)`
+            * 形式三: `(字体名称, 字体大小, 字体样式)`
+        2. 颜色为一个包含三个或四个 RGB 颜色字符串的元组，共两种形式\n
+            * 不使用禁用功能时: `(正常颜色, 触碰颜色, 交互颜色)`
+            * 需使用禁用功能时: `(正常颜色, 触碰颜色, 交互颜色, 禁用颜色)`
+            * 特别地，进度条控件的参数`color_bar`为: `(底色, 进度条颜色)`
         """
         self.master = canvas
         self.value = text
         self.justify = justify
         self.font = font
         self.photoimage = image
         self.color_text = list(color_text)
@@ -592,15 +607,14 @@
         `y`: 改变到的纵坐标\n
         """
         self.move(x - self.x1, y - self.y1)
 
     def configure(self, *args, **kw):  # type: (...) -> str | tuple | None
         """
         修改或查询原有参数的值，可供修改或查询的参数有\n
-        ---
         1. 所有控件: `color_text`、`color_fill`、`color_outline`
         2. 非文本控件: `text`\n
         注意：颜色修改不会立即生效，可通过鼠标经过生效，或者调用 state 方法立即刷新状态！
         """
         if args:
             if args[0] == 'text':
                 if isinstance(self, CheckButton):
@@ -610,27 +624,27 @@
                 return getattr(self, args[0])
 
         value = kw.get('text', None)
         text = kw.get('color_text', None)
         fill = kw.get('color_fill', None)
         outline = kw.get('color_outline', None)
 
-        if value != None:
+        if value is not None:
             if isinstance(self, CheckButton):
                 self.master.itemconfigure(self._text, text=value)
             else:
                 self.value = value
         if text:
             self.color_text = text
         if fill:
             self.color_fill = fill
         if outline:
             self.color_outline = outline
 
-        if isinstance(self, (Label, Button, Progressbar)) and value != None and not isinstance(self, CheckButton):
+        if isinstance(self, (Label, Button, Progressbar)) and value is not None and not isinstance(self, CheckButton):
             self.master.itemconfigure(self.text, text=value)
 
     def destroy(self):  # type: () -> None
         """ 摧毁控件释放内存 """
         self.live = False
         self.master._widget.remove(self)
 
@@ -814,15 +828,15 @@
         y,  # type: int
         width,  # type: int
         height,  # type: int
         *,
         radius=RADIUS,  # type: float
         text='',  # type: str
         borderwidth=BORDERWIDTH,  # type: int
-        justify=tkinter.CENTER,  # type: str
+        justify='center',  # type: Literal['left', 'center', 'right']
         font=(FONT, SIZE),  # type: tuple[str, int, str]
         image=None,  # type: PhotoImage | None
         color_text=COLOR_TEXT,  # type: tuple[str, str, str]
         color_fill=COLOR_BUTTON_FILL,  # type: tuple[str, str, str]
         color_outline=COLOR_BUTTON_OUTLINE  # type: tuple[str, str, str]
     ):  # type: (...) -> None
         BaseWidget.__init__(self, canvas, x, y, width, height, radius, text, justify,
@@ -845,15 +859,15 @@
         y,  # type: int
         width,  # type: int
         height,  # type: int
         *,
         radius=RADIUS,  # type: float
         text='',  # type: str
         borderwidth: int = BORDERWIDTH,  # type: int
-        justify=tkinter.CENTER,  # type: str
+        justify='center',  # type: Literal['left', 'center', 'right']
         font=(FONT, SIZE),  # type: tuple[str, int, str]
         command=None,  # type: Callable | None
         image=None,  # type: PhotoImage | None
         color_text=COLOR_TEXT,  # type: tuple[str, str, str]
         color_fill=COLOR_BUTTON_FILL,  # type: tuple[str, str, str]
         color_outline=COLOR_BUTTON_OUTLINE,  # type: tuple[str, str, str]
     ):  # type: (...) -> None
@@ -931,20 +945,20 @@
         canvas,  # type: Canvas
         x,  # type: int
         y,  # type: int
         width,  # type: int
         height,  # type: int
         *,
         radius=RADIUS,  # type: float
-        text='',  # type: tuple[str] | str
+        text='',  # type: tuple[str, str] | str
         show=None,  # type: str | None
         limit=LIMIT,  # type: int
         cursor=CURSOR,  # type: str
         borderwidth=BORDERWIDTH,  # type: int
-        justify=tkinter.LEFT,  # type: str
+        justify='left',  # type: Literal['left', 'center', 'right']
         font=(FONT, SIZE),  # type: tuple[str, int, str]
         image=None,  # type: PhotoImage | None
         color_text=COLOR_TEXT,  # type: tuple[str, str, str]
         color_fill=COLOR_TEXT_FILL,  # type: tuple[str, str, str]
         color_outline=COLOR_TEXT_OUTLINE  # type: tuple[str, str, str]
     ):  # type: (...) -> None
         TextWidget.__init__(self, canvas, x, y, width, height, radius, text, limit, justify,
@@ -1011,20 +1025,20 @@
         canvas,  # type: Canvas
         x,  # type: int
         y,  # type: int
         width,  # type: int
         height,  # type: int
         *,
         radius=RADIUS,  # type: float
-        text='',  # type: tuple[str] | str
+        text='',  # type: tuple[str, str] | str
         limit=LIMIT,  # type: int
         read=False,  # type: bool
         cursor=CURSOR,  # type: str
         borderwidth=BORDERWIDTH,  # type: int
-        justify=tkinter.LEFT,  # type: str
+        justify='left',  # type: Literal['left', 'center', 'right']
         font=(FONT, SIZE),  # type: tuple[str, int, str]
         image=None,  # type: PhotoImage | None
         color_text=COLOR_TEXT,  # type: tuple[str, str, str]
         color_fill=COLOR_TEXT_FILL,  # type: tuple[str, str, str]
         color_outline=COLOR_TEXT_OUTLINE  # type: tuple[str, str, str]
     ):  # type: (...) -> None
         TextWidget.__init__(self, canvas, x, y, width, height, radius, text, limit, justify,
@@ -1163,15 +1177,15 @@
         canvas,  # type: Canvas
         x,  # type: int
         y,  # type: int
         width,  # type: int
         height,  # type: int
         *,
         borderwidth=BORDERWIDTH,  # type: int
-        justify=tkinter.CENTER,  # type: str
+        justify='center',  # type: Literal['left', 'center', 'right']
         font=(FONT, SIZE),  # type: tuple[str, int, str]
         image=None,  # type: PhotoImage | None
         color_text=COLOR_TEXT,  # type: tuple[str, str, str]
         color_outline=COLOR_TEXT_OUTLINE,  # type: tuple[str, str, str]
         color_bar=COLOR_BAR  # type: tuple[str, str]
     ):  # type: (...) -> None
         self.bottom = canvas.create_rectangle(
@@ -1217,15 +1231,15 @@
         `**kw`: 与 tkinter.PhotoImage 的参数相同\n
         """
         self.file = file  # 图片文件的路径
         self.extension = file.rsplit('.', 1)[-1]  # 文件扩展名
         self._item = {}  # type: dict[tkinter._CanvasItemId, Canvas | None]
 
         if self.extension == 'gif':  # 动态图片
-            self.image: list[tkinter.PhotoImage] = []
+            self.image = []  # type: list[tkinter.PhotoImage]
         else:  # 静态图片
             self.image = tkinter.PhotoImage.__init__(self, file=file, **kw)
 
     def parse(self, start=0):  # type: (int) -> Generator[int, None, None]
         """
         ### 解析动图
         解析并得到动图的每一帧动画，该方法返回一个生成器\n
@@ -1292,15 +1306,15 @@
         ### 缩放图片
         不会缩放该图片对象本身，只是返回一个缩放后的图片对象\n
         ---
         `rate_x`: 横向缩放倍率\n
         `rate_y`: 纵向缩放倍率\n
         `precision`: 精度到小数点后的位数（推荐 1.2），越大运算就越慢（默认值代表绝对精确）\n
         """
-        if precision != None:
+        if precision is not None:
             limit = round(10**precision)
             rate_x = Fraction(str(rate_x)).limit_denominator(limit)
             rate_y = Fraction(str(rate_y)).limit_denominator(limit)
             image = tkinter.PhotoImage.zoom(
                 self, rate_x.numerator, rate_y.numerator)
             image = image.subsample(rate_x.denominator, rate_y.denominator)
         else:
```

### Comparing `tkintertools_dev-2.6.1/tkintertools/constants.py` & `tkintertools-dev-2.6.2/tkintertools/constants.py`

 * *Files identical despite different names*

### Comparing `tkintertools_dev-2.6.1/tkintertools_dev.egg-info/PKG-INFO` & `tkintertools-dev-2.6.2/tkintertools_dev.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: tkintertools-dev
-Version: 2.6.1
+Version: 2.6.2
 Summary: An auxiliary module of the tkinder module
 Home-page: https://gitcode.net/weixin_62651706/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
+License: MulanPSL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
@@ -22,18 +23,18 @@
         <a href="./tkintertools/__init__.py">
             <img src="https://img.shields.io/badge/Version-2.6.1-blue" alt="latest version" />
         </a>
         <a href="./LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
         <a href="./CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/05/21-orange" alt="ChangeLog" />
+            <img src="https://img.shields.io/badge/ChangeLog-2023/05/26-orange" alt="ChangeLog" />
         </a>
         <a href="./TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-9-yellow" alt="ToDos" />
+            <img src="https://img.shields.io/badge/ToDos-10-yellow" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
             <img src="https://img.shields.io/badge/Downloads-3k-purple" alt="Downloads" />
         </a>
     </p>
     <p>
         <a href="mailto:2951256653@qq.com">
@@ -49,35 +50,35 @@
 </div>
 
 Installation/模块安装
 -----------------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.0
-* Release Date/发布日期 : 2023/03/28
+* Version/版本 : 2.6.1
+* Release Date/发布日期 : 2023/05/21
 
 ```
-pip install tkintertools==2.6.0
+pip install tkintertools==2.6.1
 ```
 或者
 ```
 pip install tkintertools
 ```
 
 这个是目前的最新版，比较稳定，bug 没有那么多，推荐使用这个。  
 稳定版有文档可以查看，有 issue 我会去查看并尝试解决 issue。
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.1
-* Release Date/发布日期 : 2023/05/21
+* Version/版本 : 2.6.2
+* Release Date/发布日期 : 2023/05/26
 
 ```
-pip install tkintertools-dev==2.6.1
+pip install tkintertools-dev==2.6.2
 ```
 
 这个是作者正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
 开发版本没有对应的文档，大家可以在 issue 中提出建议，我会适当采纳一些并在开发版本中更改或实现。
 
 Description/模块说明
 ----------------------
@@ -95,15 +96,15 @@
 
 tkintertools 模块还具有一些特色的功能：
 
 * 利用 tkinter 和 tkintertools 创建的程序，在高分辨率的情况下，tkintertools 的会更加清晰（这点对于笔记本用户很友好，比如我）
 * 可以迅速实现渐变色的效果
 * 窗口缩放，所有的控件的大小跟着缩放（当然，也可以设置为不跟随缩放）
 
-注意：需要 Python3.7 及更高版本才能运行 tkintertools！
+注意：需要 **Python3.7** 及更高版本才能运行 tkintertools！
 
 Provides/模块功能
 -------------------
 
 Here, only the more distinctive features will be listed  
 这里只会列举出比较具有特色的功能
 
@@ -133,27 +134,27 @@
 见 [DPI 级别设置函数](#DPI)
 
 ### Detailed type hints/详细的类型提示
 
 参考 [PEP 526](https://peps.python.org/pep-0526/)、[PEP 586](https://peps.python.org/pep-0586/)、[PEP 604](https://peps.python.org/pep-0604/) 和 [PEP 612](https://peps.python.org/pep-0612/)，我采用了最兼容的方式去实现详细的类型提示，可适用 IDE 有 VScode、Pycharm 等。  
 那什么是类型提示呢？话不多说，直接看图就行：
 
-<p><img height="350px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/type_hint_vscode.png" alt="type_hint.png"/></p>
+![type_hint.png](docs/images/type_hint_vscode.png)
 
 在 VSCode 编辑器中，当鼠标移至类或者函数的名字上面时，会自动显示该类或者函数的注释文档。通过这种方式，不需要看太多的帮助文档和资料就能熟练地使用 tkintertools 模块！
 
 ### Across Platforms/跨平台
 
 [test.py](./test.py) 在 Windows 系统（Windows10）上运行的界面如下：
 
-<p><img height="383px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/test_win32.png" alt="test_win32.png"/></p>
+![test_win32.png](docs/images/test_win32.png)
 
 [test.py](./test.py) 在 Linux 系统（Ubuntu22.04）上运行的界面如下：
 
-<p><img height="408px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/test_linux.png" alt="test_linux.png"/></p>
+![test_linux.png](docs/images/test_linux.png)
 
 Contents/模块内容
 -------------------
 
 Each non internal class and function in the module will be described in detail here  
 这里会详细说明模块中的每个非内部类和函数
 
@@ -173,24 +174,24 @@
 
 ### Virtual Canvas Widget/虚拟画布控件
 
 1. `Label`: 标签控件
 
     标签控件的功能和`tkinter.Label`的功能类似，但更加的多元化  
     下面是`Label`控件的外观：  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/LabelTest.png" alt="LabelTest.png" /></p>
+
+    ![LabelTest.png](docs/images/LabelTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('LabelTest', 1000, 400)
-    canvas = tkt.Canvas(root, 1000, 400)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 1000, 400, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -207,25 +208,25 @@
     ```
 
     </details>
 
 2. `Button`: 按钮控件
 
     按钮控件相较于`tkinter.Button`，其自由度更高，`tkinter.Button`只有在按下的时候才能触发绑定的关联事件，而`Button`却可以在鼠标移至按钮上方时、鼠标按下时、鼠标松开时都可以绑定关联事件  
-    下面是`Button`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ButtonTest.png" alt="ButtonTest.png" /></p>
+    下面是`Button`控件的外观：
+
+    ![ButtonTest.png](docs/images/ButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ButtonTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -243,24 +244,24 @@
 
     </details>
 
 3. `CheckButton`: 复选框控件
 
     复选框控件相对于`tkinter`原生的`tkinter.CheckButton`在使用方面更加地简单，同时颜值也上升了不少  
     下面是`CheckButton`控件的外观：
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/CheckButtonTest.png" alt="CheckButtonTest.png"/></p>
+
+    ![CheckButtonTest.png](docs/images/CheckButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('CheckButtonTest', 500, 300)
-    canvas = tkt.Canvas(root, 500, 300)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 300, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -278,25 +279,25 @@
     ```
 
     </details>
 
 4. `Entry`: 输入框控件
 
     输入框控件可以轻松地设置输入的文本位置（靠左、居中和靠右），同时，它可以在鼠标移至输入框上方、鼠标未在输入框上方两种状态显示不同的默认文本  
-    下面是`Entry`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/EntryTest.png" alt="EntryTest.png" /></p>
+    下面是`Entry`控件的外观：
+
+    ![EntryTest.png](docs/images/EntryTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('EntryTest', 500, 400)
-    canvas = tkt.Canvas(root, 500, 400)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 400, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -310,39 +311,39 @@
         'RightEntry', 'Enter'), justify='right')
     tkt.Entry(canvas, 270, 20, 200, 30, radius=8, text='LeftEntry')
     tkt.Entry(canvas, 270, 55, 200, 30, radius=8,
             text='CenterEntry', justify='center')
     tkt.Entry(canvas, 270, 90, 200, 30, radius=8,
             text='RightEntry', justify='right')
     tkt.Entry(canvas, 100, 150, 300, 35, text=('PasswordEntry',
-            'Click To Enter'), justify='center', show='•')
+            'Click To Enter'), justify='center', show='●')
     tkt.Entry(canvas, 100, 200, 300, 35, text='DisableEntry',
             justify='center').set_live(False)
     tkt.Entry(canvas, 100, 250, 300, 35, text='TransparentEntry',
             justify='center', color_fill=tkt.COLOR_NONE)
 
     root.mainloop()
     ```
 
     </details>
 
 5. `Text`: 文本框控件
 
     文本框类似于输入框，这里就不再赘述  
-    下面是`Text`控件的外观：  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/TextTest.png" alt="TextTest.png" /></p>
+    下面是`Text`控件的外观：
+
+    ![TextTest.png](docs/images/TextTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('TextTest', 1000, 400)
-    canvas = tkt.Canvas(root, 1000, 400)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 1000, 400, 0, 0)
 
 
     def colorful(x, y, width, height) -> None:  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -360,36 +361,35 @@
     ```
 
     </details>
 
 6. `Progressbar`: 进度条控件
 
     进度条控件相比`tkinter.ttk.Progressbar`，外观上的自由度较大  
-    下面是`Progressbar`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ProgressbarTest.png" alt="ProgressbarTest.png" /></p>
+    下面是`Progressbar`控件的外观：
+
+    ![ProgressbarTest.png](docs/images/ProgressbarTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ProgressbarTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height) -> None:  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
 
 
     colorful(30, 290, 440, 50)
-
     tkt.Progressbar(canvas, 50, 50, 400, 30)
     tkt.Progressbar(canvas, 50, 100, 400, 30).load(.6667)
     tkt.Progressbar(canvas, 50, 150, 400, 30, borderwidth=5).load(1)
     (_ := tkt.Progressbar(canvas, 50, 200, 400, 30)).load(0.3333)
     _.set_live(False)
     tkt.Progressbar(canvas, 50, 250, 400, 30, color_bar=(
         'lightyellow', 'skyblue')).load(.5)
@@ -423,25 +423,25 @@
 
     单例模式，不用介绍了吧？通过继承它来使用
 
 ### Tool Function/工具函数
 
 1. `move`: <a name="move">移动函数</a>
 
-    移动函数可以轻松地按一定的规律、移动速度、移动时间去移动`tkintertools`模块内的所有对象，同时兼容了`tkinter`内的对象，即`tkinter`中的对象也可以很方便地移动，甚至它还可以移动窗口的位置！  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/MoveTest.gif" alt="MoveTest.gif" /></p>
+    移动函数可以轻松地按一定的规律、移动速度、移动时间去移动`tkintertools`模块内的所有对象，同时兼容了`tkinter`内的对象，即`tkinter`中的对象也可以很方便地移动，甚至它还可以移动窗口的位置！
+
+    ![MoveTest.gif](docs/images/MoveTest.gif)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('MoveTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
     rect = canvas.create_rectangle(50, 350, 150, 450)
 
 
     def move_window(switch=[True]):  # type: (list[bool]) -> None
         tkt.move(root, None, 1000 if switch[0] else -1000, 0, 800, mode='flat')
         switch[0] = not switch[0]
 
@@ -460,15 +460,14 @@
     tkt.Button(canvas, 50, 50, 200, 40, radius=10,
             text='MoveWindow', command=move_window)
     tkt.Button(canvas, 50, 100, 200, 40, radius=10,
             text='MoveRect', command=move_rect)
     button = tkt.Button(canvas, 50, 150, 200, 40, radius=10,
                         text='MoveButton', command=move_button)
 
-
     root.mainloop()
     ```
 
     </details>
 
 2. `text`: 文本函数
 
@@ -478,26 +477,27 @@
     `left`   : "tkintertools        "  
     `center` : "    tkintertools    "  
     `right`  : "        tkintertools"</pre>
 
 3. `color`: <a name="Gradient">颜色函数</a>
 
     颜色函数可以轻松求出一个颜色到另外一个颜色的过渡颜色，因此可以轻松得到渐变色的效果，同时，改变传入的参数还可以得到传入颜色的对比色  
-    第二张图是 test.py 在图像测试中绘制的图案  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ColorTest.png" alt="ColorTest.png" />
-    <img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/Test_Draw.png" alt="Test_Draw.png" /></p>
+    第二张图是 test.py 在图像测试中绘制的图案
+
+    ![ColorTest.png](docs/images/ColorTest.png)
+
+    ![Test_Draw.png](docs/images/Test_Draw.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ColorTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
-    canvas.place(x=0, y=0)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#00FF00'), i/width)
             color_2 = tkt.color(('#FFFFFF', '#000000'), i/width)
@@ -517,18 +517,22 @@
     `askfont`函数可以打开默认的字体选择窗口，这个窗口虽然是默认的，但它实际上无法在`tkinter`中打开，因为`tkinter`并没有对应的 API 能够做到这一点。但是，`tkintertools`调用并封装了原生的 tcl 的命令，使得字体选择框能够被我们使用。
 
     <p><img width="540px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/font.png" alt="font.png" /></p>
 
 5. `SetProcessDpiAwareness`: <a name="DPI">DPI 级别设置函数</a>
 
     这个函数实际上只是对函数`ctypes.WinDLL('shcore').SetProcessDpiAwareness`的一个简单包装，其值可为 0、1 和 2，分别代表程序 DPI 的不同级别，那么缩放效果也就不同，`tkintertools`选择的值是 1，但程序默认值实际为 0  
-    下面是执行了这个函数的效果
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/SetProcessDpiAwareness_0.png" alt="SetProcessDpiAwareness_1.png" /></p>
-    <p>下面是未执行这个函数的效果</p>
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/SetProcessDpiAwareness_1.png" alt="SetProcessDpiAwareness_0.png" /></p>
+    下面是未执行这个函数的效果
+    
+    ![SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
+
+    <p>下面是执行了这个函数的效果</p>
+
+    ![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
+
     从上面的两张图中可以很明显的看出第一张很模糊，第二张很清晰，这就是 DPI 级别不同的原因，不过这一点在屏幕缩放比不是 100% 的时候才会出现  
     大家对上面的图肯定很熟悉，这不就是 IDLE 吗！？对，这个的问题的解决办法也是来自于 IDLE 的源代码 [pyshell.py line 18~20]  
     注意：该函数在程序的不同位置执行的效果不一样！一般用在`mainloop`之前，但`tkintertools`已经在`mainloop`函数中嵌入了该函数，无需再设置一次 DPI 级别，此函数是为了原生`tkinter`程序用的。
 
 Examples/实战示例
 ----------------
 
@@ -570,28 +574,23 @@
 * 文章链接: 暂无
 * 代码仓库: https://gitcode.net/weixin_62651706/tester
 * 程序下载: 暂无
 * 推荐指数: 👍👍👍
 
 这个案例使用了最新稳定版的 tkintertools-v2.6.0，界面非常稳定，几乎没有 bug，完全采用 tkintertools 的控件，颜值很高，界面非常流畅。体现了 tkintertools 模块与 tkinter 模块相比在性能上的优越性！
 
-<p>
-    <img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/examples/exam3_1.png" alt="client.png"/>
-    <img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/examples/exam3_2.png" alt="client.png"/>
-</p>
+![exam3_1.png](docs/examples/exam3_1.png)
+![exam3_2.png](docs/examples/exam3_2.png)
 
 More/更多
 ---------
 
 > GitCode:  
 > https://gitcode.net/weixin_62651706/tkintertools
 
 > GitHub(Mirror/镜像):  
 > https://github.com/XiaoKang2022-CSDN/tkintertools
 
 > Column/专栏:  
 > https://blog.csdn.net/weixin_62651706/category_11600888.html
 
-> Tutorials/教程:  
-> https://xiaokang2022.blog.csdn.net/article/details/127374661
-
 还有更多内容请在 [源代码](./tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: tkintertools-dev Version: 2.6.1 Summary: An
+Metadata-Version: 2.1 Name: tkintertools-dev Version: 2.6.2 Summary: An
 auxiliary module of the tkinder module Home-page: https://gitcode.net/
 weixin_62651706/tkintertools Author: Xiaokang2022 Author-email:
-2951256653@qq.com Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
-Classifier: Operating System :: OS Independent Description-Content-Type: text/
-markdown License-File: LICENSE
+2951256653@qq.com License: MulanPSL-2.0 Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: Mulan Permissive Software
+License v2 (MulanPSL-2.0) Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
                             [Email] [Blog] [Author]
 Installation/æ¨¡åå®è£ ----------------------- ### Stable version/
-ç¨³å®çæ¬ * Version/çæ¬ : 2.6.0 * Release Date/åå¸æ¥æ : 2023/03/28
-``` pip install tkintertools==2.6.0 ``` æè ``` pip install tkintertools ```
+ç¨³å®çæ¬ * Version/çæ¬ : 2.6.1 * Release Date/åå¸æ¥æ : 2023/05/21
+``` pip install tkintertools==2.6.1 ``` æè ``` pip install tkintertools ```
 è¿ä¸ªæ¯ç®åçææ°çï¼æ¯è¾ç¨³å®ï¼bug
 æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã ç¨³å®çæææ¡£å¯ä»¥æ¥çï¼æ
 issue æä¼å»æ¥çå¹¶å°è¯è§£å³ issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.1 * Release Date/åå¸æ¥æ : 2023/05/21
-``` pip install tkintertools-dev==2.6.1 ```
+å¼åçæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/26
+``` pip install tkintertools-dev==2.6.2 ```
 è¿ä¸ªæ¯ä½èæ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
 å¯è½ä¼æ¯è¾å¤ã å¼åçæ¬æ²¡æå¯¹åºçææ¡£ï¼å¤§å®¶å¯ä»¥å¨ issue
 ä¸­æåºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
 Description/æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº
 tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
@@ -34,18 +34,18 @@
 ä½åæ¶ä¹äº§çäºä¸äºç¼ºç¹ï¼ * èæçæ§ä»¶æ æ³è·åç¦ç¹ *
 èæçæ§ä»¶å¨ææ¬è¾å¥åæ¾ç¤ºçåè½ä¸å­å¨ä¸äºç¼ºé·ï¼è¿ä¸ªç¼ºé·ä¸æ¯å¾ææ¾ï¼ä½å¼ºè¿«çå°±æç¹é¾åäºï¼æ¯å¦æï¼
 tkintertools æ¨¡åè¿å·æä¸äºç¹è²çåè½ï¼ * å©ç¨ tkinter å
 tkintertools åå»ºçç¨åºï¼å¨é«åè¾¨ççæåµä¸ï¼tkintertools
 çä¼æ´å æ¸æ°ï¼è¿ç¹å¯¹äºç¬è®°æ¬ç¨æ·å¾åå¥½ï¼æ¯å¦æï¼ *
 å¯ä»¥è¿éå®ç°æ¸åè²çææ *
 çªå£ç¼©æ¾ï¼ææçæ§ä»¶çå¤§å°è·çç¼©æ¾ï¼å½ç¶ï¼ä¹å¯ä»¥è®¾ç½®ä¸ºä¸è·éç¼©æ¾ï¼
-æ³¨æï¼éè¦ Python3.7 åæ´é«çæ¬æè½è¿è¡ tkintertoolsï¼ Provides/
-æ¨¡ååè½ ------------------- Here, only the more distinctive features will
-be listed è¿éåªä¼åä¸¾åºæ¯è¾å·æç¹è²çåè½ ### Customizable
-widgets/å¯èªå®ä¹çæ§ä»¶ tkintertools
+æ³¨æï¼éè¦ **Python3.7** åæ´é«çæ¬æè½è¿è¡ tkintertoolsï¼
+Provides/æ¨¡ååè½ ------------------- Here, only the more distinctive
+features will be listed è¿éåªä¼åä¸¾åºæ¯è¾å·æç¹è²çåè½ ###
+Customizable widgets/å¯èªå®ä¹çæ§ä»¶ tkintertools
 æ¨¡åçæ§ä»¶æ¥æè®¸å¤åæ°ä¾æä»¬è®¾ç½®ï¼æ¯å¦åè§çåå¾ãææ¬åè¾¹æ¡ä»¥åæ§ä»¶åé¨çé¢è²ï¼å³èäºä»¶ç­ç­ã
 è¿éè¦è¯´æçæ¯ï¼æ¯ä¸ªæ§ä»¶å¯ä»¥è®¾ç½®çå³èäºä»¶ä¸æ­¢ä¸ç§ï¼å¨é¼ æ ç»è¿æ§ä»¶æ¶å¯ä»¥ç»å®äºä»¶ï¼é¼ æ ç¹å»æ§ä»¶ä¹å¯ä»¥ï¼é¼ æ ç¹å»åæ¾å¼ä¹è¡ç­ç­ã
 ææ¬åè¾¹æ¡ä»¥åæ§ä»¶çå¡«åè²ä¹æ¯ç±»ä¼¼çï¼å¨é¼ æ ç»è¿æ§ä»¶ãç¹å»æ§ä»¶ãç¹å»åæ¾å¼é½å¯ä»¥è®¾å®é¢è²ã
 ææ¬ç±»æ§ä»¶è¿è½å¤ä»å³è¾¹éæ­¥è¾å¥ææ¬ï¼ææ¬è¾å¥æç¤ºç¬¦ä¹å¯ä»¥ä¸æ¯åè°æ è¶£çç«çº¿ï¼å¯ä»¥æ¯å¶ä»çï¼æ¯å¦ä¸åçº¿ç­ã
 æåï¼å¤§å®¶å¯ä»¥çä¸ä¸ [test.py](./test.py)
 æä»¶éé¢çç¤ºä¾ï¼è¿ä¸ªç¤ºä¾å±ç¤ºäº tkintertools
 æ¨¡åçç»å¤§é¨ååè½ï¼ç¤ºä¾ä¸­æ´æéèç âå¤å½©åå¹»â
@@ -58,117 +58,108 @@
 (#Gradient) ### Automatically adapt to DPI/èªå¨éåºDPI è§ [DPI
 çº§å«è®¾ç½®å½æ°](#DPI) ### Detailed type hints/è¯¦ç»çç±»åæç¤º åè
 [PEP 526](https://peps.python.org/pep-0526/)ã[PEP 586](https://
 peps.python.org/pep-0586/)ã[PEP 604](https://peps.python.org/pep-0604/) å
 [PEP 612](https://peps.python.org/pep-0612/
 )ï¼æéç¨äºæå¼å®¹çæ¹å¼å»å®ç°è¯¦ç»çç±»åæç¤ºï¼å¯éç¨
 IDE æ VScodeãPycharm ç­ã
-é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼
-[type_hint.png]
-å¨ VSCode
+é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼ !
+[type_hint.png](docs/images/type_hint_vscode.png) å¨ VSCode
 ç¼è¾å¨ä¸­ï¼å½é¼ æ ç§»è³ç±»æèå½æ°çåå­ä¸é¢æ¶ï¼ä¼èªå¨æ¾ç¤ºè¯¥ç±»æèå½æ°çæ³¨éææ¡£ãéè¿è¿ç§æ¹å¼ï¼ä¸éè¦çå¤ªå¤çå¸®å©ææ¡£åèµæå°±è½çç»å°ä½¿ç¨
 tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](./test.py) å¨
-Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼
-[test_win32.png]
-[test.py](./test.py) å¨ Linux
-ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼
-[test_linux.png]
-Contents/æ¨¡ååå®¹ ------------------- Each non internal class and function
-in the module will be described in detail here
+Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_win32.png]
+(docs/images/test_win32.png) [test.py](./test.py) å¨ Linux
+ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png](docs/
+images/test_linux.png) Contents/æ¨¡ååå®¹ ------------------- Each non
+internal class and function in the module will be described in detail here
 è¿éä¼è¯¦ç»è¯´ææ¨¡åä¸­çæ¯ä¸ªéåé¨ç±»åå½æ° ### Container
 Widget/å®¹å¨æ§ä»¶ 1. `Tk`: çªå£ç±»
 ç»§æ¿äº`tkinter.Tk`ï¼å¨ç»§æ¿äº`tkinter`æ¨¡åå`Tk`çåºç¡ä¸ï¼åå å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¹¶å å¥äºæ£æµçªå£å¤§å°æ¯å¦ç¼©æ¾çæºå¶ï¼ä»¥ä½¿å¾å¶å­`Canvas`åè½æ­£ç¡®å°è¿è¡ç¼©æ¾
 2. `Toplevel`: é¡¶çº§çªå£ç±»
 ç»§æ¿äº`tkinter.Toplevel`å`Tk`ï¼å å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¶ä½åä¸`Tk`ä¸æ ·
 3. `Canvas`: ç»å¸ç±»
 ç»§æ¿äº`tkinter.Canvas`ï¼å å¥äºå¯¹ç»å¸èææ§ä»¶çæ¯æï¼åæ¶æ¯åç±»ååºäºä»¶ãç¼©æ¾æ§å¶çç®¡çèï¼ä¹å¯¹`tkinter.Canvas`çå®ä¾æ¹æ³æä¸å®çå¼å®¹æ§
 ### Virtual Canvas Widget/èæç»å¸æ§ä»¶ 1. `Label`: æ ç­¾æ§ä»¶
 æ ç­¾æ§ä»¶çåè½å`tkinter.Label`çåè½ç±»ä¼¼ï¼ä½æ´å çå¤åå
-ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼
-[LabelTest.png]
+ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼ ![LabelTest.png](docs/images/LabelTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('LabelTest', 1000,
-400) canvas = tkt.Canvas(root, 1000, 400) canvas.place(x=0, y=0) def colorful
-(x, y, width, height): # type: (int, int, int, int) -> None """ Gradient colors
-""" for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Label(canvas, 50, 50, 400, 100, text='NormalLabel\nHere is the text')
 tkt.Label(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerLabel')
 tkt.Label(canvas, 550, 50, 400, 100, text='DisableLabel').set_live(False)
 tkt.Label(canvas, 550, 200, 400, 100, radius=20, text='TransparentLabel',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  2. `Button`: æé®æ§ä»¶
 æé®æ§ä»¶ç¸è¾äº`tkinter.Button`ï¼å¶èªç±åº¦æ´é«ï¼`tkinter.Button`åªæå¨æä¸çæ¶åæè½è§¦åç»å®çå³èäºä»¶ï¼è`Button`å´å¯ä»¥å¨é¼ æ ç§»è³æé®ä¸æ¹æ¶ãé¼ æ æä¸æ¶ãé¼ æ æ¾å¼æ¶é½å¯ä»¥ç»å®å³èäºä»¶
-ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼
-[ButtonTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ButtonTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) canvas.place(x=0, y=0) def colorful(x,
-y, width, height): # type: (int, int, int, int) -> None """ Gradient colors """
-for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼ ![ButtonTest.png](docs/images/
+ButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk
+('ButtonTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful
+(x, y, width, height): # type: (int, int, int, int) -> None """ Gradient colors
+""" for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 280, 400,
 100) tkt.Button(canvas, 150, 135, 200, 50, text='NormalButton') tkt.Button
 (canvas, 100, 195, 300, 50, radius=10, text='RoundCornerButton') tkt.Button
 (canvas, 150, 255, 200, 50, text='DisableButton').set_live(False) tkt.Button
 (canvas, 100, 315, 300, 50, radius=10, text='TransparentButton',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  3. `CheckButton`:
 å¤éæ¡æ§ä»¶
 å¤éæ¡æ§ä»¶ç¸å¯¹äº`tkinter`åçç`tkinter.CheckButton`å¨ä½¿ç¨æ¹é¢æ´å å°ç®åï¼åæ¶é¢å¼ä¹ä¸åäºä¸å°
-ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼
-[CheckButtonTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('CheckButtonTest',
-500, 300) canvas = tkt.Canvas(root, 500, 300) canvas.place(x=0, y=0) def
-colorful(x, y, width, height): # type: (int, int, int, int) -> None """
+ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼ ![CheckButtonTest.png](docs/images/
+CheckButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root =
+tkt.Tk('CheckButtonTest', 500, 300) canvas = tkt.Canvas(root, 500, 300, 0, 0)
+def colorful(x, y, width, height): # type: (int, int, int, int) -> None """
 Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
 '#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
 colorful(40, 190, 420, 50) tkt.CheckButton(canvas, 50, 50, 30,
 text='NormalCheckButton', value=True) tkt.CheckButton(canvas, 50, 100, 30,
 text='DisableCheckButton', value=True).set_live(False) tkt.CheckButton(canvas,
 50, 150, 30, radius=10, text='RoundCornerCheckButton') tkt.CheckButton(canvas,
 50, 200, 30, radius=15, text='TransparentCheckButton',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  4. `Entry`: è¾å¥æ¡æ§ä»¶
 è¾å¥æ¡æ§ä»¶å¯ä»¥è½»æ¾å°è®¾ç½®è¾å¥çææ¬ä½ç½®ï¼é å·¦ãå±ä¸­åé å³ï¼ï¼åæ¶ï¼å®å¯ä»¥å¨é¼ æ ç§»è³è¾å¥æ¡ä¸æ¹ãé¼ æ æªå¨è¾å¥æ¡ä¸æ¹ä¸¤ç§ç¶ææ¾ç¤ºä¸åçé»è®¤ææ¬
-ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼
-[EntryTest.png]
+ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼ ![EntryTest.png](docs/images/EntryTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('EntryTest', 500,
-400) canvas = tkt.Canvas(root, 500, 400) canvas.place(x=0, y=0) def colorful(x,
-y, width, height): # type: (int, int, int, int) -> None """ Gradient colors """
-for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+400) canvas = tkt.Canvas(root, 500, 400, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 193, 400,
 100) tkt.Entry(canvas, 20, 20, 200, 30, text=('LeftEntry', 'Enter')) tkt.Entry
 (canvas, 20, 55, 200, 30, text=( 'CenterEntry', 'Enter'), justify='center')
 tkt.Entry(canvas, 20, 90, 200, 30, text=( 'RightEntry', 'Enter'),
 justify='right') tkt.Entry(canvas, 270, 20, 200, 30, radius=8,
 text='LeftEntry') tkt.Entry(canvas, 270, 55, 200, 30, radius=8,
 text='CenterEntry', justify='center') tkt.Entry(canvas, 270, 90, 200, 30,
 radius=8, text='RightEntry', justify='right') tkt.Entry(canvas, 100, 150, 300,
-35, text=('PasswordEntry', 'Click To Enter'), justify='center', show='â¢')
+35, text=('PasswordEntry', 'Click To Enter'), justify='center', show='â')
 tkt.Entry(canvas, 100, 200, 300, 35, text='DisableEntry',
 justify='center').set_live(False) tkt.Entry(canvas, 100, 250, 300, 35,
 text='TransparentEntry', justify='center', color_fill=tkt.COLOR_NONE)
 root.mainloop() ```  5. `Text`: ææ¬æ¡æ§ä»¶
 ææ¬æ¡ç±»ä¼¼äºè¾å¥æ¡ï¼è¿éå°±ä¸åèµè¿°
-ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼
-[TextTest.png]
+ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼ ![TextTest.png](docs/images/TextTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('TextTest', 1000,
-400) canvas = tkt.Canvas(root, 1000, 400) canvas.place(x=0, y=0) def colorful
-(x, y, width, height) -> None: # type: (int, int, int, int) -> None """
-Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
-'#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
-colorful(510, 175, 480, 150) tkt.Text(canvas, 50, 50, 400, 100, text=
-('NormalText(Left)', 'Click To Enter')) tkt.Text(canvas, 50, 200, 400, 100,
-radius=20, text='RoundCornerText(Center)', justify='center') tkt.Text(canvas,
-550, 50, 400, 100, text='DisableText').set_live(False) tkt.Text(canvas, 550,
-200, 400, 100, radius=20, text='TransparentText(Right)', justify='right',
+400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
+height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
+for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
+150) tkt.Text(canvas, 50, 50, 400, 100, text=('NormalText(Left)', 'Click To
+Enter')) tkt.Text(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerText
+(Center)', justify='center') tkt.Text(canvas, 550, 50, 400, 100,
+text='DisableText').set_live(False) tkt.Text(canvas, 550, 200, 400, 100,
+radius=20, text='TransparentText(Right)', justify='right',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  6. `Progressbar`:
 è¿åº¦æ¡æ§ä»¶
 è¿åº¦æ¡æ§ä»¶ç¸æ¯`tkinter.ttk.Progressbar`ï¼å¤è§ä¸çèªç±åº¦è¾å¤§
-ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼
-[ProgressbarTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ProgressbarTest',
-500, 500) canvas = tkt.Canvas(root, 500, 500) canvas.place(x=0, y=0) def
-colorful(x, y, width, height) -> None: # type: (int, int, int, int) -> None """
-Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
+ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼ ![ProgressbarTest.png](docs/images/
+ProgressbarTest.png) æºä»£ç  ```python import tkintertools as tkt root =
+tkt.Tk('ProgressbarTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0)
+def colorful(x, y, width, height) -> None: # type: (int, int, int, int) -> None
+""" Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
 '#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
 colorful(30, 290, 440, 50) tkt.Progressbar(canvas, 50, 50, 400, 30)
 tkt.Progressbar(canvas, 50, 100, 400, 30).load(.6667) tkt.Progressbar(canvas,
 50, 150, 400, 30, borderwidth=5).load(1) (_ := tkt.Progressbar(canvas, 50, 200,
 400, 30)).load(0.3333) _.set_live(False) tkt.Progressbar(canvas, 50, 250, 400,
 30, color_bar=( 'lightyellow', 'skyblue')).load(.5) tkt.Progressbar(canvas, 50,
 300, 400, 30, color_bar=('', 'orange')).load(.1667) progressbar =
@@ -182,59 +173,58 @@
 å¨å¾æå¾å¥½çæ¯æï¼ä»éæå°éä»£ç å³å¯å®ç°å¨å¾çæ¾ç¤ºï¼è¿å¯ä»¥è®¾ç½®å¨å¾æ¾ç¤ºçéåº¦ï¼æ­¤å¤ï¼å¯¹
 png
 ç±»åçå¾ççæ¯æä¹æå¼ºåï¼å¯ä»¥å¨ä¸ä¾èµä»»ä½ç¬¬ä¸æ¹æ¨¡åæèåºçæåµä¸ï¼å¯¹
 png å¾çè¿è¡ç¼©æ¾ 2. `Singleton`: åä¾æ¨¡å¼ç±»
 åä¾æ¨¡å¼ï¼ä¸ç¨ä»ç»äºå§ï¼éè¿ç»§æ¿å®æ¥ä½¿ç¨ ### Tool Function/
 å·¥å·å½æ° 1. `move`: ç§»å¨å½æ°
 ç§»å¨å½æ°å¯ä»¥è½»æ¾å°æä¸å®çè§å¾ãç§»å¨éåº¦ãç§»å¨æ¶é´å»ç§»å¨`tkintertools`æ¨¡ååçææå¯¹è±¡ï¼åæ¶å¼å®¹äº`tkinter`åçå¯¹è±¡ï¼å³`tkinter`ä¸­çå¯¹è±¡ä¹å¯ä»¥å¾æ¹ä¾¿å°ç§»å¨ï¼çè³å®è¿å¯ä»¥ç§»å¨çªå£çä½ç½®ï¼
-[MoveTest.gif]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('MoveTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) canvas.place(x=0, y=0) rect =
-canvas.create_rectangle(50, 350, 150, 450) def move_window(switch=[True]): #
-type: (list[bool]) -> None tkt.move(root, None, 1000 if switch[0] else -1000,
-0, 800, mode='flat') switch[0] = not switch[0] def move_button(switch=[True]) -
-> None: # type: (list[bool]) -> None tkt.move(canvas, button, 200 if switch[0]
-else -200, 0, 500, mode='rebound') switch[0] = not switch[0] def move_rect
-(switch=[True]): # type: (list[bool]) -> None tkt.move(canvas, rect, 200 if
-switch[0] else -200, 0, 500, mode='smooth') switch[0] = not switch[0]
-tkt.Button(canvas, 50, 50, 200, 40, radius=10, text='MoveWindow',
-command=move_window) tkt.Button(canvas, 50, 100, 200, 40, radius=10,
-text='MoveRect', command=move_rect) button = tkt.Button(canvas, 50, 150, 200,
-40, radius=10, text='MoveButton', command=move_button) root.mainloop() ```  2.
-`text`: ææ¬å½æ°
+![MoveTest.gif](docs/images/MoveTest.gif) æºä»£ç  ```python import
+tkintertools as tkt root = tkt.Tk('MoveTest', 500, 500) canvas = tkt.Canvas
+(root, 500, 500, 0, 0) rect = canvas.create_rectangle(50, 350, 150, 450) def
+move_window(switch=[True]): # type: (list[bool]) -> None tkt.move(root, None,
+1000 if switch[0] else -1000, 0, 800, mode='flat') switch[0] = not switch[0]
+def move_button(switch=[True]) -> None: # type: (list[bool]) -> None tkt.move
+(canvas, button, 200 if switch[0] else -200, 0, 500, mode='rebound') switch[0]
+= not switch[0] def move_rect(switch=[True]): # type: (list[bool]) -> None
+tkt.move(canvas, rect, 200 if switch[0] else -200, 0, 500, mode='smooth')
+switch[0] = not switch[0] tkt.Button(canvas, 50, 50, 200, 40, radius=10,
+text='MoveWindow', command=move_window) tkt.Button(canvas, 50, 100, 200, 40,
+radius=10, text='MoveRect', command=move_rect) button = tkt.Button(canvas, 50,
+150, 200, 40, radius=10, text='MoveButton', command=move_button) root.mainloop
+() ```  2. `text`: ææ¬å½æ°
 å¯ä»¥å¿«éå¹¶æ¹ä¾¿å°å¾å°ä¸ä¸ªåæ°é¿åº¦çå­ç¬¦ä¸²ï¼ä¸å­ç¬¦ä¸²çåå®¹å¯ä»¥æå®ä½ç½®
 å¦ï¼å¾å°ä¸ä¸ª 20 é¿åº¦çå­ç¬¦ä¸² âtkintertoolsâ
     `left`   : "tkintertools        "
     `center` : "    tkintertools    "
     `right`  : "        tkintertools"
 3. `color`: é¢è²å½æ°
 é¢è²å½æ°å¯ä»¥è½»æ¾æ±åºä¸ä¸ªé¢è²å°å¦å¤ä¸ä¸ªé¢è²çè¿æ¸¡é¢è²ï¼å æ­¤å¯ä»¥è½»æ¾å¾å°æ¸åè²çææï¼åæ¶ï¼æ¹åä¼ å¥çåæ°è¿å¯ä»¥å¾å°ä¼ å¥é¢è²çå¯¹æ¯è²
-ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡
-[ColorTest.png] [Test_Draw.png]
+ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡ ![ColorTest.png]
+(docs/images/ColorTest.png) ![Test_Draw.png](docs/images/Test_Draw.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ColorTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) canvas.place(x=0, y=0) def colorful(x,
-y, width, height): # type: (int, int, int, int) -> None """ Gradient colors """
-for i in range(width): color = tkt.color(('#FF0000', '#00FF00'), i/width)
-color_2 = tkt.color(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y,
-x+i, y+height, fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 +
-i/3, outline=color_2, width=2) colorful(50, 50, 400, 100) root.mainloop() ```
-4. `askfont`: å­ä½éæ©å¯¹è¯æ¡
+500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 =
+tkt.color(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i,
+y+height, fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
+outline=color_2, width=2) colorful(50, 50, 400, 100) root.mainloop() ```  4.
+`askfont`: å­ä½éæ©å¯¹è¯æ¡
 `askfont`å½æ°å¯ä»¥æå¼é»è®¤çå­ä½éæ©çªå£ï¼è¿ä¸ªçªå£è½ç¶æ¯é»è®¤çï¼ä½å®å®éä¸æ æ³å¨`tkinter`ä¸­æå¼ï¼å ä¸º`tkinter`å¹¶æ²¡æå¯¹åºç
 API è½å¤åå°è¿ä¸ç¹ãä½æ¯ï¼`tkintertools`è°ç¨å¹¶å°è£äºåçç
 tcl çå½ä»¤ï¼ä½¿å¾å­ä½éæ©æ¡è½å¤è¢«æä»¬ä½¿ç¨ã
 [font.png]
 5. `SetProcessDpiAwareness`: DPI çº§å«è®¾ç½®å½æ°
 è¿ä¸ªå½æ°å®éä¸åªæ¯å¯¹å½æ°`ctypes.WinDLL
 ('shcore').SetProcessDpiAwareness`çä¸ä¸ªç®ååè£ï¼å¶å¼å¯ä¸º 0ã1
 å 2ï¼åå«ä»£è¡¨ç¨åº DPI
 çä¸åçº§å«ï¼é£ä¹ç¼©æ¾ææä¹å°±ä¸åï¼`tkintertools`éæ©çå¼æ¯
-1ï¼ä½ç¨åºé»è®¤å¼å®éä¸º 0 ä¸é¢æ¯æ§è¡äºè¿ä¸ªå½æ°çææ
-[SetProcessDpiAwareness_1.png]
-ä¸é¢æ¯æªæ§è¡è¿ä¸ªå½æ°çææ
-[SetProcessDpiAwareness_0.png]
+1ï¼ä½ç¨åºé»è®¤å¼å®éä¸º 0 ä¸é¢æ¯æªæ§è¡è¿ä¸ªå½æ°çææ !
+[SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
+ä¸é¢æ¯æ§è¡äºè¿ä¸ªå½æ°çææ
+![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
 ä»ä¸é¢çä¸¤å¼ å¾ä¸­å¯ä»¥å¾ææ¾ççåºç¬¬ä¸å¼ å¾æ¨¡ç³ï¼ç¬¬äºå¼ å¾æ¸æ°ï¼è¿å°±æ¯
 DPI çº§å«ä¸åçåå ï¼ä¸è¿è¿ä¸ç¹å¨å±å¹ç¼©æ¾æ¯ä¸æ¯ 100%
 çæ¶åæä¼åºç° å¤§å®¶å¯¹ä¸é¢çå¾è¯å®å¾çæï¼è¿ä¸å°±æ¯ IDLE
 åï¼ï¼å¯¹ï¼è¿ä¸ªçé®é¢çè§£å³åæ³ä¹æ¯æ¥èªäº IDLE çæºä»£ç 
 [pyshell.py line 18~20]
 æ³¨æï¼è¯¥å½æ°å¨ç¨åºçä¸åä½ç½®æ§è¡çææä¸ä¸æ ·ï¼ä¸è¬ç¨å¨`mainloop`ä¹åï¼ä½`tkintertools`å·²ç»å¨`mainloop`å½æ°ä¸­åµå¥äºè¯¥å½æ°ï¼æ éåè®¾ç½®ä¸æ¬¡
 DPI çº§å«ï¼æ­¤å½æ°æ¯ä¸ºäºåç`tkinter`ç¨åºç¨çã Examples/
@@ -263,15 +253,13 @@
 æ¨¡åçå¼å®¹æ§ï¼
 [chess.png] [chess.png]
 ### ç®æç»å½çé¢ * æç« é¾æ¥: ææ  * ä»£ç ä»åº: https://
 gitcode.net/weixin_62651706/tester * ç¨åºä¸è½½: ææ  * æ¨èææ°:
 ððð è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
-æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼
-[client.png] [client.png]
-More/æ´å¤ --------- > GitCode: > https://gitcode.net/weixin_62651706/
-tkintertools > GitHub(Mirror/éå): > https://github.com/XiaoKang2022-CSDN/
-tkintertools > Column/ä¸æ : > https://blog.csdn.net/weixin_62651706/
-category_11600888.html > Tutorials/æç¨: > https://
-xiaokang2022.blog.csdn.net/article/details/127374661 è¿ææ´å¤åå®¹è¯·å¨
-[æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
+æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png](docs/
+examples/exam3_1.png) ![exam3_2.png](docs/examples/exam3_2.png) More/æ´å¤ ---
+------ > GitCode: > https://gitcode.net/weixin_62651706/tkintertools > GitHub
+(Mirror/éå): > https://github.com/XiaoKang2022-CSDN/tkintertools > Column/
+ä¸æ : > https://blog.csdn.net/weixin_62651706/category_11600888.html
+è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
```

