# Comparing `tmp/u0_stitcher-0.1.1.tar.gz` & `tmp/u0_stitcher-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "u0_stitcher-0.1.1.tar", last modified: Thu May 25 09:18:58 2023, max compression
+gzip compressed data, was "u0_stitcher-0.1.4.tar", last modified: Fri May 26 02:35:12 2023, max compression
```

## Comparing `u0_stitcher-0.1.1.tar` & `u0_stitcher-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-05-25 09:18:58.325023 u0_stitcher-0.1.1/
--rw-r--r--   0 u03013112   (502) staff       (20)     3916 2023-05-25 09:18:58.324878 u0_stitcher-0.1.1/PKG-INFO
--rw-r--r--   0 u03013112   (502) staff       (20)     2877 2023-05-24 11:03:20.000000 u0_stitcher-0.1.1/README.md
--rw-r--r--   0 u03013112   (502) staff       (20)       38 2023-05-25 09:18:58.325195 u0_stitcher-0.1.1/setup.cfg
--rw-r--r--   0 u03013112   (502) staff       (20)      865 2023-05-25 09:18:48.000000 u0_stitcher-0.1.1/setup.py
-drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-05-25 09:18:58.323615 u0_stitcher-0.1.1/u0_stitcher/
--rw-r--r--   0 u03013112   (502) staff       (20)       46 2023-05-25 08:29:16.000000 u0_stitcher-0.1.1/u0_stitcher/__init__.py
--rw-r--r--   0 u03013112   (502) staff       (20)      163 2023-05-25 09:15:53.000000 u0_stitcher-0.1.1/u0_stitcher/errors.py
--rw-r--r--   0 u03013112   (502) staff       (20)     3148 2023-05-25 08:30:19.000000 u0_stitcher-0.1.1/u0_stitcher/fisheye2Equirectangular.py
--rw-r--r--   0 u03013112   (502) staff       (20)    10771 2023-05-25 07:51:21.000000 u0_stitcher-0.1.1/u0_stitcher/stitchEasy3.py
--rw-r--r--   0 u03013112   (502) staff       (20)     9763 2023-05-25 09:15:51.000000 u0_stitcher-0.1.1/u0_stitcher/stitcher.py
-drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-05-25 09:18:58.324660 u0_stitcher-0.1.1/u0_stitcher.egg-info/
--rw-r--r--   0 u03013112   (502) staff       (20)     3916 2023-05-25 09:18:58.000000 u0_stitcher-0.1.1/u0_stitcher.egg-info/PKG-INFO
--rw-r--r--   0 u03013112   (502) staff       (20)      328 2023-05-25 09:18:58.000000 u0_stitcher-0.1.1/u0_stitcher.egg-info/SOURCES.txt
--rw-r--r--   0 u03013112   (502) staff       (20)        1 2023-05-25 09:18:58.000000 u0_stitcher-0.1.1/u0_stitcher.egg-info/dependency_links.txt
--rw-r--r--   0 u03013112   (502) staff       (20)       20 2023-05-25 09:18:58.000000 u0_stitcher-0.1.1/u0_stitcher.egg-info/requires.txt
--rw-r--r--   0 u03013112   (502) staff       (20)       12 2023-05-25 09:18:58.000000 u0_stitcher-0.1.1/u0_stitcher.egg-info/top_level.txt
+drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-05-26 02:35:12.579029 u0_stitcher-0.1.4/
+-rw-r--r--   0 u03013112   (502) staff       (20)     4254 2023-05-26 02:35:12.578881 u0_stitcher-0.1.4/PKG-INFO
+-rw-r--r--   0 u03013112   (502) staff       (20)     3167 2023-05-25 09:48:10.000000 u0_stitcher-0.1.4/README.md
+-rw-r--r--   0 u03013112   (502) staff       (20)       38 2023-05-26 02:35:12.579078 u0_stitcher-0.1.4/setup.cfg
+-rw-r--r--   0 u03013112   (502) staff       (20)      865 2023-05-26 02:33:56.000000 u0_stitcher-0.1.4/setup.py
+drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-05-26 02:35:12.577654 u0_stitcher-0.1.4/u0_stitcher/
+-rw-r--r--   0 u03013112   (502) staff       (20)       46 2023-05-25 08:29:16.000000 u0_stitcher-0.1.4/u0_stitcher/__init__.py
+-rw-r--r--   0 u03013112   (502) staff       (20)      163 2023-05-25 09:15:53.000000 u0_stitcher-0.1.4/u0_stitcher/errors.py
+-rw-r--r--   0 u03013112   (502) staff       (20)     4466 2023-05-25 11:37:38.000000 u0_stitcher-0.1.4/u0_stitcher/fisheye2Equirectangular.py
+-rw-r--r--   0 u03013112   (502) staff       (20)    10771 2023-05-25 07:51:21.000000 u0_stitcher-0.1.4/u0_stitcher/stitchEasy3.py
+-rw-r--r--   0 u03013112   (502) staff       (20)    12166 2023-05-25 11:49:35.000000 u0_stitcher-0.1.4/u0_stitcher/stitcher.py
+drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-05-26 02:35:12.578646 u0_stitcher-0.1.4/u0_stitcher.egg-info/
+-rw-r--r--   0 u03013112   (502) staff       (20)     4254 2023-05-26 02:35:12.000000 u0_stitcher-0.1.4/u0_stitcher.egg-info/PKG-INFO
+-rw-r--r--   0 u03013112   (502) staff       (20)      328 2023-05-26 02:35:12.000000 u0_stitcher-0.1.4/u0_stitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 u03013112   (502) staff       (20)        1 2023-05-26 02:35:12.000000 u0_stitcher-0.1.4/u0_stitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 u03013112   (502) staff       (20)       20 2023-05-26 02:35:12.000000 u0_stitcher-0.1.4/u0_stitcher.egg-info/requires.txt
+-rw-r--r--   0 u03013112   (502) staff       (20)       12 2023-05-26 02:35:12.000000 u0_stitcher-0.1.4/u0_stitcher.egg-info/top_level.txt
```

### Comparing `u0_stitcher-0.1.1/PKG-INFO` & `u0_stitcher-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: u0_stitcher
-Version: 0.1.1
+Version: 0.1.4
 Summary: stitcher for two fisheye camera
 Home-page: https://github.com/u03013112/pano
 Author: u03013112
 Author-email: u03013112@hotmail.com
 License: UNKNOWN
 Description: # pano
         
@@ -49,14 +49,20 @@
         3、校准主副镜头的图像，即圆心+半径。这里由于是超级广角，所以图像是一个圆，但是随着镜头的物理位置不稳定，需要进行校准。这里会强制要求两个图片的半径一致，即获得的等距投影图分辨率一致。
         4、拼接矫正，尝试用等距投影进行拼接。
         以上校准全部保存校准结果至本地文件，当本地文件不存在，强制要求校准，否则不需要校准。如果有必要可以随时进行校准。
         5、拼接输入图片，这是一个全流程，输入一张图片（横向拼接原图输入），输出一张图片（等距投影拼接）。
         
         暂时封装成一个类。
         
+        ## 2023-05-25 进展
+        
+        基础功能完成，在比较合适的图片上表现还是挺好的，但是在一些特殊情况，比如校准时的距离与实际视频距离有较大变化的情况下，拼接效果就不好了。
+        
+        所以可能需要手动或者自动进行不断的校准。
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `u0_stitcher-0.1.1/README.md` & `u0_stitcher-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,7 +40,13 @@
 2、校准主副镜头，由于目前的两个摄像头都是usb摄像头，usb的可插拔等特性导致，每次启动时，主副镜头的顺序都可能不一致，所以需要校准。
 3、校准主副镜头的图像，即圆心+半径。这里由于是超级广角，所以图像是一个圆，但是随着镜头的物理位置不稳定，需要进行校准。这里会强制要求两个图片的半径一致，即获得的等距投影图分辨率一致。
 4、拼接矫正，尝试用等距投影进行拼接。
 以上校准全部保存校准结果至本地文件，当本地文件不存在，强制要求校准，否则不需要校准。如果有必要可以随时进行校准。
 5、拼接输入图片，这是一个全流程，输入一张图片（横向拼接原图输入），输出一张图片（等距投影拼接）。
 
 暂时封装成一个类。
+
+## 2023-05-25 进展
+
+基础功能完成，在比较合适的图片上表现还是挺好的，但是在一些特殊情况，比如校准时的距离与实际视频距离有较大变化的情况下，拼接效果就不好了。
+
+所以可能需要手动或者自动进行不断的校准。
```

### Comparing `u0_stitcher-0.1.1/setup.py` & `u0_stitcher-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="u0_stitcher",
-    version="0.1.1",
+    version="0.1.4",
     packages=find_packages(),
     install_requires=[
         'numpy',
         'opencv-python',
     ],
     author="u03013112",
     author_email="u03013112@hotmail.com",
```

### Comparing `u0_stitcher-0.1.1/u0_stitcher/fisheye2Equirectangular.py` & `u0_stitcher-0.1.4/u0_stitcher/fisheye2Equirectangular.py`

 * *Files 21% similar despite different names*

```diff
@@ -51,14 +51,51 @@
     if needShow:
         cv2.imshow('Equirectangular Image', equirectangular_image)
         cv2.waitKey(0)
         cv2.destroyAllWindows()
 
     return equirectangular_image
 
+# 为了提高效率，把上面fisheye2Equirectangular拆分成两个函数
+def buildMap(fisheye_image, fov_degrees):
+    src_height, src_width, _ = fisheye_image.shape
+    dst_width = src_width
+    dst_height = src_height
+
+    map_x, map_y = buildmap(src_width, src_height, dst_width, dst_height, fov_degrees)
+    return map_x, map_y
+
+def remap(fisheye_image, map_x, map_y):
+    equirectangular_image = cv2.remap(fisheye_image, map_x, map_y, cv2.INTER_LINEAR)
+    return equirectangular_image
+
+import time
+def fisheye2EquirectangularDebug(fisheye_image, fov_degrees, needShow=False):
+    src_height, src_width, _ = fisheye_image.shape
+    dst_width = src_width
+    dst_height = src_height
+
+    start_time = time.time()
+    map_x, map_y = buildmap(src_width, src_height, dst_width, dst_height, fov_degrees)
+    buildmap_time = time.time() - start_time
+
+    start_time = time.time()
+    equirectangular_image = cv2.remap(fisheye_image, map_x, map_y, cv2.INTER_LINEAR)
+    remap_time = time.time() - start_time
+
+    if needShow:
+        cv2.imshow('Equirectangular Image', equirectangular_image)
+        cv2.waitKey(0)
+        cv2.destroyAllWindows()
+
+    print("buildmap耗时：{:.2f} ms".format(buildmap_time * 1000))
+    print("remap耗时：{:.2f} ms".format(remap_time * 1000))
+
+    return equirectangular_image
+
 import os
 import sys
 if __name__ == '__main__':
     if len(sys.argv) < 2:
         print("错误：请输入图片文件名")
         print("用法：python readFishEyePic.py 图片文件名")
         sys.exit(1)
```

### Comparing `u0_stitcher-0.1.1/u0_stitcher/stitchEasy3.py` & `u0_stitcher-0.1.4/u0_stitcher/stitchEasy3.py`

 * *Files identical despite different names*

### Comparing `u0_stitcher-0.1.1/u0_stitcher/stitcher.py` & `u0_stitcher-0.1.4/u0_stitcher/stitcher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import cv2 
 import json
 
 import numpy as np
-from .fisheye2Equirectangular import fisheye2Equirectangular
+from .fisheye2Equirectangular import fisheye2Equirectangular,fisheye2EquirectangularDebug
+from .fisheye2Equirectangular import buildMap,remap
 from .stitchEasy3 import stitch2,stitch3
 
 from .errors import CircleCenterNotCalibratedException, StitchNotCalibratedException
 
 # 其他导入...
 
 # 您的主文件代码...
@@ -63,14 +64,15 @@
     cropped_image[top - (y - r):bottom - (y - r), left - (x - r):right - (x - r)] = image[top:bottom, left:right]
     return cropped_image
 
 class Stitcher:
     def __init__(self) -> None:
         self.config_path = './config.json'
         self.config = self.readConfig()
+        self.tmpConfig = {}
     
     def readConfig(self):
         # 读取配置文件，配置文件在 './config.json' 中
         # 如果文件不存在，那么就初始化一个配置文件
         # 如果文件存在，那么就读取配置文件
         # 返回一个字典
         # 初始值 就是一个空字典
@@ -151,14 +153,22 @@
         r = int((r1+r2)/2)
         # 写配置
         self.config['img1CircleCenter'] = [x1,y1]
         self.config['img2CircleCenter'] = [x2,y2]
         self.config['imgCircleRadius'] = r
         self.writeConfig()
 
+    def buildMap(self,img1):
+        if 'mapX' not in self.tmpConfig:
+            self.tmpConfig['mapX'],self.tmpConfig['mapY'] = buildMap(img1,self.config['fov'])
+        return self.tmpConfig['mapX'],self.tmpConfig['mapY']
+    def fisheye2Equirectangular(self,img1):
+        mapX,mapY = self.buildMap(img1)
+        return remap(img1,mapX,mapY)
+
     def calibStitch(self,img):
         # 进行判断，
         # 如果配置文件中没有img1，则默认左侧是img1
         # 如果配置文件中没有圆心和半径的配置，那么就报错，调用者收到这个报错应该调用calibCircleCenter
         if 'img1' not in self.config:
             self.calibMainCamera()
         if 'img1CircleCenter' not in self.config or 'img2CircleCenter' not in self.config or 'imgCircleRadius' not in self.config:
@@ -169,16 +179,16 @@
         img2 = img[:, int(img.shape[1] / 2):]
         
         img1Croped = crop_image(img1,(self.config['img1CircleCenter'][0],self.config['img1CircleCenter'][1],self.config['imgCircleRadius']))
         img2Croped = crop_image(img2,(self.config['img2CircleCenter'][0],self.config['img2CircleCenter'][1],self.config['imgCircleRadius']))
 
 
         # 将两张方图分别做成等距投影
-        img1EC = fisheye2Equirectangular(img1Croped, self.config['fov'])
-        img2EC = fisheye2Equirectangular(img2Croped, self.config['fov'])
+        img1EC = self.fisheye2Equirectangular(img1Croped)
+        img2EC = self.fisheye2Equirectangular(img2Croped)
 
         overlap_width1,overlap_width2,dh = stitch2(img1EC,img2EC)
         # 写配置文件
         self.config['overlap_width1'] = overlap_width1
         self.config['overlap_width2'] = overlap_width2
         self.config['dh'] = dh
         self.writeConfig()
@@ -199,21 +209,61 @@
         img2 = img[:, int(img.shape[1] / 2):]
 
         img1Croped = crop_image(img1,(self.config['img1CircleCenter'][0],self.config['img1CircleCenter'][1],self.config['imgCircleRadius']))
         img2Croped = crop_image(img2,(self.config['img2CircleCenter'][0],self.config['img2CircleCenter'][1],self.config['imgCircleRadius']))
 
 
         # 将两张方图分别做成等距投影
-        img1EC = fisheye2Equirectangular(img1Croped, self.config['fov'])
-        img2EC = fisheye2Equirectangular(img2Croped, self.config['fov'])
+        img1EC = self.fisheye2Equirectangular(img1Croped)
+        img2EC = self.fisheye2Equirectangular(img2Croped)
 
         stitchedResult = stitch3(img1EC,img2EC,self.config['overlap_width1'],self.config['overlap_width2'],self.config['dh'])
 
         return stitchedResult
 
+    def stitchDebug(self, img):
+        import time
+        start_time = time.time()
+
+        if 'img1' not in self.config:
+            self.calibMainCamera()
+        if 'img1CircleCenter' not in self.config or 'img2CircleCenter' not in self.config or 'imgCircleRadius' not in self.config:
+            raise CircleCenterNotCalibratedException('请先校准圆心和半径，调用calibCircleCenter')
+        if 'overlap_width1' not in self.config or 'overlap_width2' not in self.config or 'dh' not in self.config:
+            raise StitchNotCalibratedException('请先校准拼接，调用calibStitch')
+
+        step1_time = time.time()
+
+        img1 = img[:, :int(img.shape[1] / 2)]
+        img2 = img[:, int(img.shape[1] / 2):]
+
+        step2_time = time.time()
+
+        img1Croped = crop_image(img1, (self.config['img1CircleCenter'][0], self.config['img1CircleCenter'][1], self.config['imgCircleRadius']))
+        img2Croped = crop_image(img2, (self.config['img2CircleCenter'][0], self.config['img2CircleCenter'][1], self.config['imgCircleRadius']))
+
+        step3_time = time.time()
+
+        img1EC = self.fisheye2Equirectangular(img1Croped)
+        img2EC = self.fisheye2Equirectangular(img2Croped)
+
+        step4_time = time.time()
+
+        stitchedResult = stitch3(img1EC, img2EC, self.config['overlap_width1'], self.config['overlap_width2'], self.config['dh'])
+
+        step5_time = time.time()
+
+        print("Step 1 (calibration checks) duration: {:.4f} seconds".format(step1_time - start_time))
+        print("Step 2 (split image) duration: {:.4f} seconds".format(step2_time - step1_time))
+        print("Step 3 (crop image) duration: {:.4f} seconds".format(step3_time - step2_time))
+        print("Step 4 (fisheye to equirectangular) duration: {:.4f} seconds".format(step4_time - step3_time))
+        print("Step 5 (stitching) duration: {:.4f} seconds".format(step5_time - step4_time))
+        print("All duration: {:.4f} seconds".format(step5_time - start_time))
+
+        return stitchedResult
 
 
     
 
 if __name__ == '__main__':
     pano = Stitcher()
     # pano.calibMainCamera('left')
```

### Comparing `u0_stitcher-0.1.1/u0_stitcher.egg-info/PKG-INFO` & `u0_stitcher-0.1.4/u0_stitcher.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: u0-stitcher
-Version: 0.1.1
+Version: 0.1.4
 Summary: stitcher for two fisheye camera
 Home-page: https://github.com/u03013112/pano
 Author: u03013112
 Author-email: u03013112@hotmail.com
 License: UNKNOWN
 Description: # pano
         
@@ -49,14 +49,20 @@
         3、校准主副镜头的图像，即圆心+半径。这里由于是超级广角，所以图像是一个圆，但是随着镜头的物理位置不稳定，需要进行校准。这里会强制要求两个图片的半径一致，即获得的等距投影图分辨率一致。
         4、拼接矫正，尝试用等距投影进行拼接。
         以上校准全部保存校准结果至本地文件，当本地文件不存在，强制要求校准，否则不需要校准。如果有必要可以随时进行校准。
         5、拼接输入图片，这是一个全流程，输入一张图片（横向拼接原图输入），输出一张图片（等距投影拼接）。
         
         暂时封装成一个类。
         
+        ## 2023-05-25 进展
+        
+        基础功能完成，在比较合适的图片上表现还是挺好的，但是在一些特殊情况，比如校准时的距离与实际视频距离有较大变化的情况下，拼接效果就不好了。
+        
+        所以可能需要手动或者自动进行不断的校准。
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

