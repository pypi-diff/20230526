# Comparing `tmp/sprites-1.683.tar.gz` & `tmp/sprites-1.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprites-1.683.tar", last modified: Wed Jan 25 13:40:37 2023, max compression
+gzip compressed data, was "sprites-1.69.tar", last modified: Fri May 26 12:45:22 2023, max compression
```

## Comparing `sprites-1.683.tar` & `sprites-1.69.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-01-25 13:40:37.764124 sprites-1.683/
--rw-rw-rw-   0        0        0     1993 2023-01-25 13:40:37.759123 sprites-1.683/PKG-INFO
--rw-rw-rw-   0        0        0     1001 2020-01-01 03:51:20.000000 sprites-1.683/README.md
--rw-rw-rw-   0        0        0       42 2023-01-25 13:40:37.769124 sprites-1.683/setup.cfg
--rw-rw-rw-   0        0        0     1172 2023-01-25 13:37:27.000000 sprites-1.683/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-25 13:40:37.651622 sprites-1.683/sprites/
--rw-rw-rw-   0        0        0  1429766 2023-01-25 13:36:55.000000 sprites-1.683/sprites/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-25 13:40:37.740373 sprites-1.683/sprites.egg-info/
--rw-rw-rw-   0        0        0     1993 2023-01-25 13:40:37.000000 sprites-1.683/sprites.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-01-25 13:40:37.000000 sprites-1.683/sprites.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-25 13:40:37.000000 sprites-1.683/sprites.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-25 13:40:26.000000 sprites-1.683/sprites.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-01-25 13:40:37.000000 sprites-1.683/sprites.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-01-25 13:40:37.000000 sprites-1.683/sprites.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 12:45:22.658787 sprites-1.69/
+-rw-rw-rw-   0        0        0     2099 2023-05-26 12:45:22.656787 sprites-1.69/PKG-INFO
+-rw-rw-rw-   0        0        0     1001 2020-01-01 03:51:20.000000 sprites-1.69/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-26 12:45:22.661787 sprites-1.69/setup.cfg
+-rw-rw-rw-   0        0        0     1306 2023-05-26 12:44:48.000000 sprites-1.69/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:45:22.618785 sprites-1.69/sprites/
+-rw-rw-rw-   0        0        0  1439092 2023-05-11 01:04:21.000000 sprites-1.69/sprites/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:45:22.648786 sprites-1.69/sprites.egg-info/
+-rw-rw-rw-   0        0        0     2099 2023-05-26 12:45:22.000000 sprites-1.69/sprites.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-05-26 12:45:22.000000 sprites-1.69/sprites.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 12:45:22.000000 sprites-1.69/sprites.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-26 12:45:16.000000 sprites-1.69/sprites.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-05-26 12:45:22.000000 sprites-1.69/sprites.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 12:45:22.000000 sprites-1.69/sprites.egg-info/top_level.txt
```

### Comparing `sprites-1.683/PKG-INFO` & `sprites-1.69/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sprites
-Version: 1.683
-Summary: Python Sprites Module for make introductory animations and games and educational purpose。It mainly provides Sprite class inherited from Turtle class。Can be applied to the teaching of elementary mathematics。Pyhton的精灵模块，为教育目的而制作启蒙动画与游戏。主要提供继承自Turtle类的Sprite类,Key类,Mouse类。支持像素级碰撞检测命令及增强的图章命令等等，也可应用于初等数学几何的教学。作者：李兴球。网址： www.lixingqiu.com
+Version: 1.69
+Summary: Python Sprites Module for make introductory animations and games and educational purpose。It mainly provides Sprite class inherited from Turtle class。Can be applied to the teaching of elementary mathematics。Pyhton的精灵模块，为教育目的而制作启蒙动画与游戏。主要提供继承自Turtle类的Sprite类,Key类,Mouse类等及一些工具函数,如洪水填充命令,几何相关命令。它支持像素级碰撞检测命令及增强的图章命令等等，也可应用于初等数学几何的教学。作者：李兴球。微信:scratch8，专业编程私教。网址： www.lixingqiu.com
 Home-page: http://www.lixingqiu.com
 Author: lixingqiu
 Author-email: 406273900@qq.com
 License: MIT
 Description: ﻿# Python sprites module introduce
         
         Python sprites  is a module for make game and animation easily.anybody can make game and animation funny.
```

### Comparing `sprites-1.683/README.md` & `sprites-1.69/README.md`

 * *Files identical despite different names*

### Comparing `sprites-1.683/setup.py` & `sprites-1.69/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 with open("README.md", encoding='utf-8') as fh:
     long_d = fh.read()
 
 
 setup(name='sprites',
       long_description_content_type="text/markdown",
-      version = '1.683',
-      description = 'Python Sprites Module for make introductory animations and games and educational purpose。It mainly provides Sprite class inherited from Turtle class。Can be applied to the teaching of elementary mathematics。Pyhton的精灵模块，为教育目的而制作启蒙动画与游戏。主要提供继承自Turtle类的Sprite类,Key类,Mouse类。支持像素级碰撞检测命令及增强的图章命令等等，也可应用于初等数学几何的教学。作者：李兴球。网址： www.lixingqiu.com',
+      version = '1.69',
+      description = 'Python Sprites Module for make introductory animations and games and educational purpose。It mainly provides Sprite class inherited from Turtle class。Can be applied to the teaching of elementary mathematics。Pyhton的精灵模块，为教育目的而制作启蒙动画与游戏。主要提供继承自Turtle类的Sprite类,Key类,Mouse类等及一些工具函数,如洪水填充命令,几何相关命令。它支持像素级碰撞检测命令及增强的图章命令等等，也可应用于初等数学几何的教学。作者：李兴球。微信:scratch8，专业编程私教。网址： www.lixingqiu.com',
       long_description = long_d,      
       keywords = 'creative game pygame turtle animation sprite geometry math Elementary Mathematics Teaching',
       url = 'http://www.lixingqiu.com',
+      wechat = 'scratch8',
       author ='lixingqiu',
       author_email = '406273900@qq.com',
       license = 'MIT',
       packages = ['sprites'],
       zip_safe = False,
       install_requires = [ 'pillow>=2.7.0','numpy==1.21.4']
      )
```

### Comparing `sprites-1.683/sprites/__init__.py` & `sprites-1.69/sprites/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,36 +176,37 @@
    原因是绑定盒命令得到的是先前没有刷新的角色的坐标，这样获取的不是最新坐标，当然会导致程序出意外。
    4. 屏幕的update命令会重新渲染所有的角色，如果角色较多，反而会让程序运行更慢。
    5. 本模块给RawTurtle类增加了update方法，这样能单独渲染一个角色。本模块已经把屏幕的自动绘画延时设为0及速度也设为最快了。
    6. 其实Turtle模块可以支持png图片,但要像以下这样写:
    screen.addshape('scratch.png',Shape("image", screen._image('scratch.png')))
 """
 __author__ = 'lixingqiu'
-__date__ = '2023/1/25'
+__date__ = '2023/5/3'
 __blog__ = 'www.lixingqiu.com'
 
 import os
 import re
 import sys
 import math
 import glob
 import time
 import base64
 import random
 import colorsys
+import collections
 import numpy as np
 from io import BytesIO
 from copy import deepcopy
 from tkinter import filedialog
 from tkinter import colorchooser
 from winsound import PlaySound,SND_ASYNC,SND_LOOP,SND_PURGE
-from PIL import ImageTk,ImageOps,Image,ImageGrab,ImageDraw,ImageFont,ImagePath
+from PIL import ImageTk,ImageOps,Image,ImageGrab,ImageDraw,ImageFont,ImagePath,ImageColor
 from turtle import TK,_Root,ScrolledCanvas,_CFG ,TNavigator,Tbuffer,TPen,_Screen,Screen,Turtle,Vec2D, RawTurtle,TurtleScreenBase,Shape,TurtleScreen,_TurtleImage,TurtleGraphicsError 
 
-_VERSION = 1.683 # 增加rotate_points单独函数， 增加了InputBox类和屏幕的inputbox方法及更多的内置造型图
+_VERSION = 1.69 # 增加foold_fill洪水填充函数,rotate_points单独函数， 增加了InputBox类和屏幕的inputbox方法及更多的内置造型图
 _CFG['delay'] = 0
 # 定义资源文件夹
 _resfld = os.path.join(os.getcwd(),'res')
 if not os.path.exists(_resfld):os.mkdir(_resfld)
 
 class InputBox:
     def __init__(self,master,title='输入对话框',prompt='请输入字符:'):
@@ -275,15 +276,15 @@
         self.the_menu.entryconfigure("剪切",command=lambda: e_widget.event_generate("<<Cut>>"))
         self.the_menu.entryconfigure("复制",command=lambda: e_widget.event_generate("<<Copy>>"))
         self.the_menu.entryconfigure("粘贴",command=lambda: e_widget.event_generate("<<Paste>>"))
         self.the_menu.entryconfigure("全选",command=lambda: e_widget.select_range(0, 'end'))
         self.the_menu.tk.call("tk_popup", self.the_menu, event.x_root, event.y_root)
     
     
-def makerndfilename(ext):
+def makerndfilename(ext=''):
     """生成随机文件名,ext是扩展名,如.png """
     s = 'abcdefghijklmnopqrstuvwxyz0123456789'
     t = time.localtime()
     year = str(t.tm_year)
     mon = str(t.tm_mon)
     day = str(t.tm_mday)
     minu = str(t.tm_min)
@@ -614,15 +615,15 @@
     self.screen.isplaying=False             # 这句并不是多余的2023/1/25
     self.clear()        # 清除所写,所以要放歌典,最好用单独的海龟对象
     PlaySound(None,SND_PURGE)
 RawTurtle.stop = RawTurtle_stop
 
 # 给原生海龟对象增加play方法
 def RawTurtle_play(self,song_file,lrc_file=None,fontstyle=("",24,"normal"),loop=False ):
-    """在海龟屏幕显示歌词并播放歌曲，本函数只支持无损wav文件。
+    """在海龟屏幕显示歌词并播放歌曲，本函数只支持wav文件,推荐用单独的海龟播放音乐。
        self：海龟对象或其子类的实例
        song_file：歌曲文件
        lrc_file：歌词文件，诸如：[00:00.00]月满西楼
                                  [01:00.12]红藕香残 玉簟秋
        上面这样的歌词文件。
        fontstyle为三元组，表示用write写字时的字体风格。
        loop:为假示不循环播放,为True表示循环播放
@@ -689,14 +690,16 @@
             self.write(display_words_,align='center',font=fontstyle)
             self.goto(x-1,y+1)
             self.color(fgcolor)
             self.write(display_words_,align='center',font=fontstyle)    
             words_index=words_index+1            
         if words_index < words_lines and self.screen.isplaying:        
             self.screen.ontimer(display_subtitle,100)
+        else:
+            self.clear()
     # 调用显示标题的函数
     display_subtitle()
 RawTurtle.play = RawTurtle_play
 
 # 给原生海龟增加get_tag方法,用于获取标签
 RawTurtle.get_tag = lambda self:self._tag
 
@@ -914,16 +917,14 @@
         if angle%90==0:continue
         x = long * math.cos(math.radians(angle))
         y = long * math.sin(math.radians(angle))
         self.cv.create_line(0,0,x,y,fill=linecolors[colorindex])# 斜angle度的射线
     for i in range(long//step):        
         r = (i+1) * step
         self.cv.create_oval(-r,r,r,-r,outline=linecolors[colorindex])
-
-
     self.cv.create_line(left,0,right,0,fill=xaxiscolors[colorindex]) # x轴
     self.cv.create_line(0,bottom,0,top,fill=yaxiscolors[colorindex])# y轴
     self.cv.create_text(100-15,0+15,text='100',fill=xtextcolors[colorindex],font=('Arial',12,'normal'),angle=45)
     self.cv.create_text(-100-15,0+15,text='-100',fill=xtextcolors[colorindex],font=('Arial',12,'normal'),angle=45)
     self.cv.create_text(-15,15-100,text='100',fill=ytextcolors[colorindex],font=('Arial',12,'normal'),angle=45)
     self.cv.create_text(-15,15+100,text='-100',fill=ytextcolors[colorindex],font=('Arial',12,'normal'),angle=45)
 
@@ -996,14 +997,17 @@
       self._ontimer_call_counter = 0  # 定时器调用次数跟踪器
       self._root.bind("<FocusIn>", self.got_focus)
       self._root.bind("<FocusOut>", self.lost_focus)
 
       # 让屏幕可拖动而新增的属性
       self._oldx = 0
       self._oldy = 0
+      # 使用新的填充方法,保存填充块的编号,以便使用dfs时排除这些编号填充块
+      # 这个填充块实际是海龟造型,详见fill_area函数
+      self.fillitems = {self._bgpic}
       
 def _got_focus(self, event):
     """得到焦点而发生的事件"""
     #self.cv.config(background="red")
     self._focus = True
 
 def _lost_focus(self, event):
@@ -2142,25 +2146,22 @@
     return guaidians
 
 def adjust_pts_order(points):
     """逆时钟排序坐标点 ，只适合于凸多边形"""
     cen_x, cen_y = np.mean(points, axis=0)    
     d2s = []
     for i in range(len(points)):
-
         o_x = points[i][0] - cen_x
         o_y = points[i][1] - cen_y
         atan2 = np.arctan2(o_y, o_x)
         if atan2 < 0:
             atan2 += np.pi * 2
         d2s.append([points[i], atan2])
-
     d2s = sorted(d2s, key=lambda x:x[1])
     order_2ds = np.array([x[0] for x in d2s])
-
     return order_2ds
  
 
 # 以下定义屏幕的鼠标移动事件
 def __onmousemove(self, fun, add=None):
     """绑定鼠标移动事件"""
     
@@ -2353,14 +2354,47 @@
     else:
         return mouse_pos()
 pmouse_position = pmouse_pos
 pmouseposition = pmouse_pos
 pmousepos = pmouse_pos
 pgetmousepos = pmouse_pos
 pgetmouseposition = pmouse_pos
+
+def cors2image(points,color=(0,0,0) ): # 2023/5/3
+    """坐标位置变最小矩形图像函数,用于fill_area的函数,然后flood_fill需要调用fill_area"""    
+    all_x = [x for x,y in points]       # 所有的x
+    all_y = [y for x,y in points]       # 所有的y
+    left = min(all_x) # 最小x坐标
+    right = max(all_x) # 最大x坐标
+    top = max(all_y) # 最大y坐标
+    bottom = min(all_y) # 最小y坐标
+    img_width = int(right - left) + 1        # 生成的图像宽度    
+    img_height = int(top - bottom) + 1       # 生成的图像高度
+    points = [(x-left,y-bottom) for x ,y in points] # 左下平移
+    image_array = [[(0,0,0,0) for _ in range(img_width)] for _ in range(img_height)]
+    # 再次生成all_x和all_y
+    all_x = [int(x) for x,y in points]       # 所有的x,做numpy高级索引的
+    all_y = [int(y) for x,y in points]       # 所有的y
+    image_array = np.array(image_array)    
+    image_array[all_y,all_x] = color[0],color[1],color[2],255 # 同时设定这些位置上的值为color
+    image_array = np.flip(image_array,axis=0)
+    im = Image.fromarray(np.uint8(image_array))    
+    return im,left,top,img_width,img_height
+
+def fill_area(points,color=(0,0,0)):      # 2023/5/3
+    """填充所有points所组成的最小矩形区域"""
+    screen = Screen()
+    im,left,top,img_width,img_height = cors2image(points,color)     
+    name = 'fill_costume' + makerndfilename()
+    screen._shapes[name] = ImageTk.PhotoImage(im) # 本来是要存储造型的,这里是借用造型字典,存的值却是pillow图形对象,所以不能把它设为turtle造型  
+    x = left+img_width/2
+    y = top-img_height/2
+    if y<0:y=y+1
+    item = screen.cv.create_image(x,-y,image=screen._shapes[name])
+    screen.fillitems.add(item)    
         
 # 给背景增加坐标定位方法
 def _bg_goto(self,x,y):
     """背景坐标定位"""
     self.cv.coords(self._bgpic,(x,-y))    
 TurtleScreen.goto = _bg_goto
 
@@ -2588,28 +2622,79 @@
 
 
 def _findframes(foldername):
     """本函数返回文件夹下面序列帧图,要求这些图片的文件名形式为
        0.png,1.png,2.png,3.png......
        返回所有图片列表。
     """
-    exts = ['.png','.gif','.jpg','.jpeg']
-    
+    exts = ['.png','.gif','.jpg','.jpeg']    
     for ext in exts:
         files = glob.glob(foldername + os.sep + '*' + ext)
         if files == []:continue
         frames = []
         for index in range(len(files)):
             file = foldername + os.sep + str(index) + ext
             if os.path.exists(file):
                 frames.append(file)
 
         if frames!=[]:break
     return frames
 
+tkcolors = {'lightpink': '#FFB6C1', 'pink': '#FFC0CB', 'crimson': '#DC143C', 'lavenderblush': '#FFF0F5', 'palevioletred': '#DB7093', 'hotpink': '#FF69B4', 'deeppink': '#FF1493', 'mediumvioletred': '#C71585', 'orchid': '#DA70D6', 'thistle': '#D8BFD8', 'plum': '#DDA0DD', 'violet': '#EE82EE', 'magenta': '#FF00FF', 'fuchsia': '#FF00FF', 'darkmagenta': '#8B008B', 'purple': '#800080', 'mediumorchid': '#BA55D3', 'darkviolet': '#9400D3', 'darkorchid': '#9932CC', 'indigo': '#4B0082', 'blueviolet': '#8A2BE2', 'mediumpurple': '#9370DB', 'mediumslateblue': '#7B68EE', 'slateblue': '#6A5ACD', 'darkslateblue': '#483D8B', 'lavender': '#E6E6FA', 'ghostwhite': '#F8F8FF', 'blue': '#0000FF', 'mediumblue': '#0000CD', 'midnightblue': '#191970', 'darkblue': '#00008B', 'navy': '#000080', 'royalblue': '#4169E1', 'cornflowerblue': '#6495ED', 'lightsteelblue': '#B0C4DE', 'lightslategray': '#778899', 'slategray': '#708090', 'dodgerblue': '#1E90FF', 'aliceblue': '#F0F8FF', 'steelblue': '#4682B4', 'lightskyblue': '#87CEFA', 'skyblue': '#87CEEB', 'deepskyblue': '#00BFFF', 'lightblue': '#ADD8E6', 'powderblue': '#B0E0E6', 'cadetblue': '#5F9EA0', 'azure': '#F0FFFF', 'lightcyan': '#E0FFFF', 'paleturquoise': '#AFEEEE', 'cyan': '#00FFFF', 'aqua': '#00FFFF', 'darkturquoise': '#00CED1', 'darkslategray': '#2F4F4F', 'darkcyan': '#008B8B', 'teal': '#008080', 'mediumturquoise': '#48D1CC', 'lightseagreen': '#20B2AA', 'turquoise': '#40E0D0', 'aquamarine': '#7FFFD4', 'mediumaquamarine': '#66CDAA', 'mediumspringgreen': '#00FA9A', 'mintcream': '#F5FFFA', 'springgreen': '#00FF7F', 'mediumseagreen': '#3CB371', 'seagreen': '#2E8B57', 'honeydew': '#F0FFF0', 'lightgreen': '#90EE90', 'palegreen': '#98FB98', 'darkseagreen': '#8FBC8F', 'limegreen': '#32CD32', 'lime': '#00FF00', 'forestgreen': '#228B22', 'green': '#008000', 'darkgreen': '#006400', 'chartreuse': '#7FFF00', 'lawngreen': '#7CFC00', 'greenyellow': '#ADFF2F', 'darkolivegreen': '#556B2F', 'yellowgreen': '#9ACD32', 'olivedrab': '#6B8E23', 'beige': '#F5F5DC', 'lightgoldenrodyellow': '#FAFAD2', 'ivory': '#FFFFF0', 'lightyellow': '#FFFFE0', 'yellow': '#FFFF00', 'olive': '#808000', 'darkkhaki': '#BDB76B', 'lemonchiffon': '#FFFACD', 'palegoldenrod': '#EEE8AA', 'khaki': '#F0E68C', 'gold': '#FFD700', 'cornsilk': '#FFF8DC', 'goldenrod': '#DAA520', 'darkgoldenrod': '#B8860B', 'floralwhite': '#FFFAF0', 'oldlace': '#FDF5E6', 'wheat': '#F5DEB3', 'moccasin': '#FFE4B5', 'orange': '#FFA500', 'papayawhip': '#FFEFD5', 'blanchedalmond': '#FFEBCD', 'navajowhite': '#FFDEAD', 'antiquewhite': '#FAEBD7', 'tan': '#D2B48C', 'burlywood': '#DEB887', 'bisque': '#FFE4C4', 'darkorange': '#FF8C00', 'linen': '#FAF0E6', 'peru': '#CD853F', 'peachpuff': '#FFDAB9', 'sandybrown': '#F4A460', 'chocolate': '#D2691E', 'saddlebrown': '#8B4513', 'seashell': '#FFF5EE', 'sienna': '#A0522D', 'lightsalmon': '#FFA07A', 'coral': '#FF7F50', 'orangered': '#FF4500', 'darksalmon': '#E9967A', 'tomato': '#FF6347', 'mistyrose': '#FFE4E1', 'salmon': '#FA8072', 'snow': '#FFFAFA', 'lightcoral': '#F08080', 'rosybrown': '#BC8F8F', 'indianred': '#CD5C5C', 'red': '#FF0000', 'brown': '#A52A2A', 'firebrick': '#B22222', 'darkred': '#8B0000', 'maroon': '#800000', 'white': '#FFFFFF', 'whitesmoke': '#F5F5F5', 'gainsboro': '#DCDCDC', 'lightgrey': '#D3D3D3', 'silver': '#C0C0C0', 'darkgray': '#A9A9A9', 'gray': '#808080', 'dimgray': '#696969', 'black': '#000000'}
+def convert_colorRGBA255(fillcolor):  # 把'red','#FF0000',(0.8,0.5,0.2)这样的转换成RGBA255形式,如'red' 转为 (255,0,0,255)
+    screen = Screen()
+    if screen._iscolorstring(fillcolor):     # 如果是合法的颜色字符串,则转换成RGBA255
+        if not fillcolor.startswith('#'):         # 如果不是以#开头的
+            fillcolor = tkcolors[fillcolor.lower()]  # 转换成以#开头的,通过查tkcolors字典
+        fillcolor = ImageColor.getcolor(fillcolor, "RGB")
+    else:                                        # 否则认为传入的是三元组
+        if screen.colormode()==1.0:
+            r,g,b = fillcolor[0],fillcolor[1],fillcolor[2]
+            fillcolor = int(r*255),int(g*255),int(b*255)
+    return fillcolor
+                
+# 为查找轮廓的dfs单独函数
+def dfs(pos,exclude=set()):
+    """深度优先搜索,从pos开始查找,exclude是排除集,里面放些item"""
+    start_time = time.time()
+    screen = Screen()
+    cv = screen.getcanvas()
+    width = screen.window_width()
+    height = screen.window_height()
+    pos = pos[0],-pos[1]
+    heading = [(1,0),(0,1),(-1,0),(0,-1)]  # 右下左上 4个方向   
+    stack = [pos] # stack保存坐标
+    cors = {}
+    cors[pos] = 1
+    counter = 0
+    while stack:
+        begin = time.time()
+        x,y  = stack.pop()
+        i = 0        
+        while i < 4:
+            counter += 1
+            next_x = x + heading[i][0]
+            next_y = y + heading[i][1]                 
+            if (next_x ,next_y) in cors :
+                i = i + 1
+                continue
+            items= cv.find_overlapping(next_x,next_y,next_x,next_y)            
+            items = set(items)           
+            [items.discard(item) for item in  exclude]
+            if items or abs(next_x)>width/2 or abs(next_y)>height/2: # 如果发现了此点是边界                     
+                 cors[(next_x,next_y)] = 2   # 轮廓点
+                 i = i + 1                     
+            else:
+                 stack.append((next_x,next_y))
+                 cors[(next_x,next_y)] = 1   #  图形内的点
+                 x = next_x
+                 y = next_y       
+    #print('dfs函数运行所花时间:',time.time() - start_time,'执行次数:',counter)    
+    return cors
+    
 class Pointer:
     """用于辅助的Pointer类,它能像海龟一样移动,可以认为是无画笔的极简版海龟"""
     def __init__(self,pos=(0,0),angle=0):
         """
            初始化方法，pos:坐标,angle:角度
         """
         self._angle = angle        # 朝向,也就是和x轴的夹角angle
@@ -4578,117 +4663,121 @@
         self.fd(radius*1.2)
         if label==None:
             s = str(degree) + "°"           
         else:
             s = label
         self.write2(s,align='center',font=('宋体',size,'normal'))
         self.goto(old_xy)
-        if isdown:self.pendown()      
-        
+        if isdown:self.pendown()              
 
     # 下面是为fill命令设计的几个方法
-    def find_contours(self,pos,value):
+    def find_contours(self,pos,exclude=set()):  
         """从一个点开始查找轮廓，一定要是封闭区域。
            由于find_overlapping在canvas中的查找是以y轴向下为正,所以y值要取反。
            pos：列表或者元组表示的二维点坐标，如(10,20)
-           value：值为1或者2，为1时返回封闭图形内的点，为2时返回边界点。
-           这是一个测试版本。
+           exclude：查找重叠时要排除的item集。
+           这是一个测试版本。深度优先搜索算法,floodfill方法.
         """    
-        screen = self.getscreen()
-        cv = screen.getcanvas()
-        width = screen.window_width()
-        height = screen.window_height()
-        pos = pos[0],-pos[1]
-        fx = [(1,0),(0,1),(-1,0),(0,-1)]  # 右下左上 4个方向   
-        stack = [pos]
-        cors = {pos:1}
-        while stack:
-            x,y = stack.pop()
-            for dx,dy in fx:            
-                next_x = x + dx
-                next_y = y + dy
-                if (next_x ,next_y) in cors :continue            
-                items=cv.find_overlapping(next_x,next_y,next_x,next_y)
-                if items or abs(next_x)>width or abs(next_y)>height:           # 如果发现了此点是边界
-                     cors[(next_x,next_y)] = 2   # 标记为边界               
-                else:
-                     cors[(next_x,next_y)] = 1   #  图形内的点              
-                     stack.append((next_x,next_y))
-        points = [ (k[0],-k[1]) for k,v in cors.items() if v==value ]
+        cors = dfs(pos,exclude=exclude)  # 返回封装图形内所有点,包括边界点
+        contours = [ (k[0],-k[1]) for k,v in cors.items() if v==2 ] # 边界点即轮廓点
+        #print('边界点数量=',len(contours))
+        inners = [ (k[0],-k[1]) for k,v in cors.items() if v==1 ]
+        return contours,inners        # 返回边界点和内部点,
+        # 下面代码准备作废
         # 需要对points里的点进行优化,如:同一线段上的点只要取两个端点即可,中间点要删除
         # 以下处理方法是查找折线的拐点,然后只保留points的第一个点,拐点集和points的最后一个点.
-        knee_points = inflection_points(points)      # 拐点集     
-        knee_points.insert(0,points[0])
-        knee_points.append(points[-1])    
+        knee_points = inflection_points(inners)      # 拐点集     
+        knee_points.insert(0,inners[0])
+        knee_points.append(inners[-1])
+        print(len(points),len(knee_points))
+        return inners
         return knee_points
-
-    def fill_concave(self,x,y,fillcolor):
+    
+    def godot(self,x,y,diameter,fc):   #  去打点
+        self.goto(x,y)        
+        self.dot(diameter,fc)
+        self.screen.update()
+        
+    def fill_concave(self,x,y):
         """以start为起点,查找封闭图形并进行填充,本函数是测试版本，
            请不要让start在封闭图形外,否则填充时间长导致无响应,并会出现意外!
            这是填充凹多边形版本,速度较慢。
         """
-        def goto_and_dot(x,y,color):
-            self.goto(x,y)           
-            self.dot(3,color)
-            self.screen.update()
+        fc = self.fillcolor()         # 填充颜色
+        if isinstance(fc,tuple) and self.screen.colormode()==255:
+            fc = int(fc[0]),int(fc[1]),int(fc[2])
         start = x,y
         screen = self.getscreen()
         tr = screen.tracer()    
-        points = self.find_contours(start,1) # 查找轮廓
-        if fillcolor!=None:
-            fc = fillcolor
-        else:
-            fc = self.fillcolor()        
+        contours,innters = self.find_contours(start,{self.turtle._item}) # 查找轮廓                
         isd = self.isdown()            # 记录当前是否落笔的状态    
-        self.penup()                   # 不管当前是否有无落笔,都要抬笔
-        pz = self.pensize()
-        self.pensize(3)        
-        [goto_and_dot(x,y,fc) for x,y in points ]         
+        self.penup()                   # 不管当前是否有无落笔,都要抬笔         
+        [self.godot(x,y,1,fc) for x,y in contours+innters ]  # 用打点填充内部,速度慢        
         screen.tracer(tr,0)
         if isd:self.pendown()           # 如果填充前是落笔状态,则恢复
-        self.pensize(pz)
+        return contours , innters
 
-    def fill_convex(self,x,y,fillcolor):
+    def fill_convex(self,x,y):
         """以start为起点,查找封闭图形并进行填充,本函数是测试版本，
            请不要让start在封闭图形外,否则填充时间长导致无响应,并会出现意外!
-           这是填充凸多边形版本,速度稍快。
-        """
+           这是填充凸多边形版本,速度稍快。        """
+        fc = self.fillcolor()         # 填充颜色
+        if isinstance(fc,tuple) and self.screen.colormode()==255:
+            fc = int(fc[0]),int(fc[1]),int(fc[2])
         start = x,y
         screen = self.getscreen()
         tr = screen.tracer()
         screen.tracer(0,0)
-        points = self.find_contours(start,2) # 查找轮廓        
-        points = adjust_pts_order(points)  # 点集以逆时钟排序
+        contours,inners = self.find_contours(start) # 查找轮廓        
+        points = adjust_pts_order(contours)  # 点集以逆时钟排序
         isd = self.isdown()            # 记录当前是否落笔的状态    
         self.penup()                   # 不管当前是否有无落笔,都要抬笔
-        if fillcolor!=None:
-            fc = self.fillcolor()
-            self.fillcolor(fillcolor)
-         
-        self.begin_fill()
+        self.goto(points[0])
+        self.begin_fill()         
+        [self.godot(x,y,1,fc) for x,y in points[1:] ]        
         self.goto(points[0]) 
-        [self.goto(x,y) for x,y in points[1:-1] ]
+        self.end_fill()
         screen.update()        
         screen.tracer(tr,0)
-        self.goto(points[0]) 
-        self.end_fill()
-        if fillcolor!=None:
-            self.fillcolor(fc)         # 还原填充颜色
         if isd:self.pendown()           # 如果填充前是落笔状态,则恢复
-
-    def fill(self,x,y,mode=0,fillcolor=None):
-        """测试版函数，慎用！x,y则是封闭图形内的一个点。
-           mode:值为1或者0，值为0时调用凸版，即fill_convex函数，
-                            值为1则调用凹版，即fill_concave函数，目前速度较慢，请耐心等待。"""
-        if mode==0:
-            self.fill_convex(x,y,fillcolor=fillcolor)     # 凸
-        else:
-            self.fill_concave(x,y,fillcolor=fillcolor)    # 凹
-    
+        return  points,tuple()
         
+    def flood_fill(self,x,y): # 洪水填充函数
+        """漫水填充方法要调用find_contours,cors2image与fill_area方法"""        
+        start = x,y
+        screen = self.getscreen()
+        tr = screen.tracer()
+        screen.tracer(0,0)
+        # exds是要排除的item列表,(在用find_contour查找轮廓时要排除一些item
+        pop = self._draw_bubble_turtle
+        exds = screen.fillitems | { self.currentLineItem,self.drawingLineItem,pop.currentLineItem,pop.drawingLineItem}         
+        contours,innters = self.find_contours(start,exds) # 查找轮廓         
+        fc = convert_colorRGBA255(self.fillcolor()) # 把颜色字符串和1.0模式的RGB转为255
+        
+        fill_area( innters+contours,fc)          # 填充由points组成的最小矩形区域
+        fc = self.fillcolor()         # 填充颜色
+        
+        if isinstance(fc,tuple) and self.screen.colormode()==255:
+            fc = int(fc[0]),int(fc[1]),int(fc[2])
+        [self.godot(x,y,1,fc) for x,y in contours ]  # 勾勒轮廓
+        screen.tracer(tr,0)
+        return contours,innters
+          
+    def fill(self,x,y,mode=2):
+        """Sprite类的填充函数，x,y则是封闭图形内的一个点。
+           mode:值为0,1,2，值为0时调用凸版，即fill_convex函数，适合于画的图形为凸多边形。
+           值为1则调用凹版，即fill_concave函数，适合于任何封装图形，速度较慢，请耐心等待。
+           值为3时调用 flood_fill即洪水填充方法。"""            
+        if mode==0:
+            contours,innters = self.fill_convex(x,y)     # 凸
+        elif mode==1:           
+            contours,innters = self.fill_concave(x,y)    # 凹
+        else:           
+            contours,innters = self.flood_fill(x,y)      # 洪水填充
+        return contours,innters
         
     movestamp = stampmove           # 移动图章
     stampglide = stampslide         # 滑行图章到指定坐标
     glidestamp = stampslide
     slidestamp = stampslide
     stamphide = hidestamp           # 隐藏图章
     stampshow = showstamp           # 显示图章
@@ -4719,14 +4808,23 @@
 
 # 定义类的别名
 Js  = Sprite
 Juese = Sprite
 角色 = Sprite
 精灵 = Sprite
 
+def fill(x,y,fillcolor='black',mode=2):  # 单独的填充命令,方便配合turtle模块使用
+    if Turtle._screen is None:return    
+    screen = Screen()            # 返回屏幕对象
+    if not hasattr(screen,'_fill_sprite'):  # 第一次没这个属性,则建立专用于填充的角色
+        screen._fill_sprite =  Sprite('blank',visible=False)
+    screen._fill_sprite.fillcolor(fillcolor)
+    contours,innters = screen._fill_sprite.fill(x,y,mode=mode)
+    return contours,innters
+    
 def find_in_square(x,y,half_length=1):    
     """返回以x,y为方形中心点坐标,half_length为半边长内的所有角色"""        
     if Turtle._screen is None:return    
     screen = Screen()            # 返回屏幕对象
     cv = screen.getcanvas()      # 得到画布
  
     w = screen._window_size()[0]
```

### Comparing `sprites-1.683/sprites.egg-info/PKG-INFO` & `sprites-1.69/sprites.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sprites
-Version: 1.683
-Summary: Python Sprites Module for make introductory animations and games and educational purpose。It mainly provides Sprite class inherited from Turtle class。Can be applied to the teaching of elementary mathematics。Pyhton的精灵模块，为教育目的而制作启蒙动画与游戏。主要提供继承自Turtle类的Sprite类,Key类,Mouse类。支持像素级碰撞检测命令及增强的图章命令等等，也可应用于初等数学几何的教学。作者：李兴球。网址： www.lixingqiu.com
+Version: 1.69
+Summary: Python Sprites Module for make introductory animations and games and educational purpose。It mainly provides Sprite class inherited from Turtle class。Can be applied to the teaching of elementary mathematics。Pyhton的精灵模块，为教育目的而制作启蒙动画与游戏。主要提供继承自Turtle类的Sprite类,Key类,Mouse类等及一些工具函数,如洪水填充命令,几何相关命令。它支持像素级碰撞检测命令及增强的图章命令等等，也可应用于初等数学几何的教学。作者：李兴球。微信:scratch8，专业编程私教。网址： www.lixingqiu.com
 Home-page: http://www.lixingqiu.com
 Author: lixingqiu
 Author-email: 406273900@qq.com
 License: MIT
 Description: ﻿# Python sprites module introduce
         
         Python sprites  is a module for make game and animation easily.anybody can make game and animation funny.
```

