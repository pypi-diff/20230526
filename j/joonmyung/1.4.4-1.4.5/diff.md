# Comparing `tmp/joonmyung-1.4.4.tar.gz` & `tmp/joonmyung-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/joonmyung-1.4.4.tar", last modified: Fri May 12 04:54:10 2023, max compression
+gzip compressed data, was "joonmyung-1.4.5.tar", last modified: Fri May 26 14:18:52 2023, max compression
```

## Comparing `joonmyung-1.4.4.tar` & `joonmyung-1.4.5.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-12 04:54:10.000000 joonmyung-1.4.4/
--rw-r--r--   0 joonmyung   (501) staff       (20)      241 2023-05-12 04:54:10.000000 joonmyung-1.4.4/PKG-INFO
--rw-r--r--   0 joonmyung   (501) staff       (20)     1138 2023-04-06 18:15:10.000000 joonmyung-1.4.4/README.md
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung/
--rw-r--r--   0 joonmyung   (501) staff       (20)       15 2023-02-22 17:22:56.000000 joonmyung-1.4.4/joonmyung/__init__.py
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung/analysis/
--rw-r--r--   0 joonmyung   (501) staff       (20)      110 2023-05-12 04:53:27.000000 joonmyung-1.4.4/joonmyung/analysis/__init__.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     6956 2023-05-12 04:53:27.000000 joonmyung-1.4.4/joonmyung/analysis/analysis.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     4346 2023-05-12 04:53:27.000000 joonmyung-1.4.4/joonmyung/analysis/dataset.py
--rw-r--r--   0 joonmyung   (501) staff       (20)        0 2023-05-12 04:53:27.000000 joonmyung-1.4.4/joonmyung/analysis/hook.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     1192 2023-05-12 04:53:27.000000 joonmyung-1.4.4/joonmyung/analysis/metric.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     1825 2023-05-12 04:53:27.000000 joonmyung-1.4.4/joonmyung/analysis/model.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     6700 2023-04-03 12:26:27.000000 joonmyung-1.4.4/joonmyung/app.py
--rw-r--r--   0 joonmyung   (501) staff       (20)      695 2023-02-24 17:07:52.000000 joonmyung-1.4.4/joonmyung/data.py
--rw-r--r--   0 joonmyung   (501) staff       (20)    13576 2023-04-26 06:40:35.000000 joonmyung-1.4.4/joonmyung/draw.py
--rw-r--r--   0 joonmyung   (501) staff       (20)       29 2023-04-03 12:26:27.000000 joonmyung-1.4.4/joonmyung/dummy.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     2755 2023-02-22 17:22:56.000000 joonmyung-1.4.4/joonmyung/file.py
--rw-r--r--   0 joonmyung   (501) staff       (20)      920 2023-02-22 17:22:56.000000 joonmyung-1.4.4/joonmyung/gradcam.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     5375 2023-04-06 18:13:55.000000 joonmyung-1.4.4/joonmyung/log.py
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung/meta_data/
--rw-r--r--   0 joonmyung   (501) staff       (20)       41 2023-03-01 06:51:46.000000 joonmyung-1.4.4/joonmyung/meta_data/__init__.py
--rw-r--r--   0 joonmyung   (501) staff       (20)    45491 2023-02-22 17:22:56.000000 joonmyung-1.4.4/joonmyung/meta_data/label.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     2252 2023-05-12 04:53:27.000000 joonmyung-1.4.4/joonmyung/meta_data/utils.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     6030 2023-03-04 10:44:55.000000 joonmyung-1.4.4/joonmyung/metric.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     3214 2023-03-30 15:51:49.000000 joonmyung-1.4.4/joonmyung/script.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     1487 2023-03-01 13:25:20.000000 joonmyung-1.4.4/joonmyung/status.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     3949 2023-04-06 17:51:01.000000 joonmyung-1.4.4/joonmyung/utils.py
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung.egg-info/
--rw-r--r--   0 joonmyung   (501) staff       (20)      241 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung.egg-info/PKG-INFO
--rw-r--r--   0 joonmyung   (501) staff       (20)      677 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung.egg-info/SOURCES.txt
--rw-r--r--   0 joonmyung   (501) staff       (20)        1 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung.egg-info/dependency_links.txt
--rw-r--r--   0 joonmyung   (501) staff       (20)        1 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung.egg-info/not-zip-safe
--rw-r--r--   0 joonmyung   (501) staff       (20)       10 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung.egg-info/top_level.txt
--rw-r--r--   0 joonmyung   (501) staff       (20)       38 2023-05-12 04:54:10.000000 joonmyung-1.4.4/setup.cfg
--rw-r--r--   0 joonmyung   (501) staff       (20)      781 2023-05-12 04:53:27.000000 joonmyung-1.4.4/setup.py
+drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-26 14:18:52.750523 joonmyung-1.4.5/
+-rw-r--r--   0 joonmyung   (501) staff       (20)        0 2023-02-22 17:22:56.000000 joonmyung-1.4.5/LICENSE.txt
+-rw-r--r--   0 joonmyung   (501) staff       (20)      256 2023-05-26 14:18:52.750397 joonmyung-1.4.5/PKG-INFO
+-rw-r--r--   0 joonmyung   (501) staff       (20)     1138 2023-04-06 18:15:10.000000 joonmyung-1.4.5/README.md
+drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-26 14:18:52.747009 joonmyung-1.4.5/joonmyung/
+-rw-r--r--   0 joonmyung   (501) staff       (20)       15 2023-02-22 17:22:56.000000 joonmyung-1.4.5/joonmyung/__init__.py
+drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-26 14:18:52.748874 joonmyung-1.4.5/joonmyung/analysis/
+-rw-r--r--   0 joonmyung   (501) staff       (20)      110 2023-03-01 06:50:39.000000 joonmyung-1.4.5/joonmyung/analysis/__init__.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     6956 2023-05-11 09:50:49.000000 joonmyung-1.4.5/joonmyung/analysis/analysis.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     4675 2023-05-21 08:24:43.000000 joonmyung-1.4.5/joonmyung/analysis/dataset.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)        0 2023-03-01 06:34:05.000000 joonmyung-1.4.5/joonmyung/analysis/hook.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     1192 2023-02-25 11:17:51.000000 joonmyung-1.4.5/joonmyung/analysis/metric.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     1784 2023-05-21 08:00:39.000000 joonmyung-1.4.5/joonmyung/analysis/model.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     6700 2023-04-03 12:26:27.000000 joonmyung-1.4.5/joonmyung/app.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)      695 2023-02-24 17:07:52.000000 joonmyung-1.4.5/joonmyung/data.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)    13698 2023-05-21 08:03:13.000000 joonmyung-1.4.5/joonmyung/draw.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)       29 2023-04-03 12:26:27.000000 joonmyung-1.4.5/joonmyung/dummy.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     2755 2023-02-22 17:22:56.000000 joonmyung-1.4.5/joonmyung/file.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)      920 2023-02-22 17:22:56.000000 joonmyung-1.4.5/joonmyung/gradcam.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)    10232 2023-05-21 08:10:17.000000 joonmyung-1.4.5/joonmyung/log.py
+drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-26 14:18:52.750093 joonmyung-1.4.5/joonmyung/meta_data/
+-rw-r--r--   0 joonmyung   (501) staff       (20)       41 2023-03-01 06:51:46.000000 joonmyung-1.4.5/joonmyung/meta_data/__init__.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)    45491 2023-02-22 17:22:56.000000 joonmyung-1.4.5/joonmyung/meta_data/label.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     2182 2023-05-21 09:42:01.000000 joonmyung-1.4.5/joonmyung/meta_data/utils.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     4031 2023-05-26 13:55:28.000000 joonmyung-1.4.5/joonmyung/metric.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     3214 2023-05-11 09:51:38.000000 joonmyung-1.4.5/joonmyung/script.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     1487 2023-03-01 13:25:20.000000 joonmyung-1.4.5/joonmyung/status.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     3949 2023-04-06 17:51:01.000000 joonmyung-1.4.5/joonmyung/utils.py
+drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-26 14:18:52.747736 joonmyung-1.4.5/joonmyung.egg-info/
+-rw-r--r--   0 joonmyung   (501) staff       (20)      256 2023-05-26 14:18:52.000000 joonmyung-1.4.5/joonmyung.egg-info/PKG-INFO
+-rw-r--r--   0 joonmyung   (501) staff       (20)      689 2023-05-26 14:18:52.000000 joonmyung-1.4.5/joonmyung.egg-info/SOURCES.txt
+-rw-r--r--   0 joonmyung   (501) staff       (20)        1 2023-05-26 14:18:52.000000 joonmyung-1.4.5/joonmyung.egg-info/dependency_links.txt
+-rw-r--r--   0 joonmyung   (501) staff       (20)        1 2023-05-26 13:56:46.000000 joonmyung-1.4.5/joonmyung.egg-info/not-zip-safe
+-rw-r--r--   0 joonmyung   (501) staff       (20)       10 2023-05-26 14:18:52.000000 joonmyung-1.4.5/joonmyung.egg-info/top_level.txt
+-rw-r--r--   0 joonmyung   (501) staff       (20)       38 2023-05-26 14:18:52.750572 joonmyung-1.4.5/setup.cfg
+-rw-r--r--   0 joonmyung   (501) staff       (20)      781 2023-05-26 13:56:19.000000 joonmyung-1.4.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `joonmyung-1.4.4/README.md` & `joonmyung-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.4/joonmyung/analysis/analysis.py` & `joonmyung-1.4.5/joonmyung/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.4/joonmyung/analysis/dataset.py` & `joonmyung-1.4.5/joonmyung/analysis/dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 import os
 
 
 class JDataset():
     distributions = {"imagenet": {"mean": [0.485, 0.456, 0.406], "std": [0.229, 0.224, 0.225]},
                         "cifar": {"mean": [0.4914, 0.4822, 0.4465], "std": [0.2023, 0.1994, 0.2010]}}
     transform_cifar    = transforms.Compose([transforms.ToTensor(), transforms.Normalize(distributions["cifar"]["mean"], distributions["cifar"]["std"])])
-    # transform_imagenet = transforms.Compose([transforms.Resize(256), transforms.CenterCrop(224), transforms.ToTensor(), transforms.Normalize(distributions["imagenet"]["mean"], distributions["imagenet"]["std"])])
-    transform_imagenet = transforms.Compose([transforms.ToTensor(), transforms.Normalize(distributions["imagenet"]["mean"], distributions["imagenet"]["std"])])
+    transform_imagenet_ = transforms.Compose([transforms.ToTensor(), transforms.Normalize(distributions["imagenet"]["mean"], distributions["imagenet"]["std"])])
+    # transform_imagenet_vis = transforms.Compose([transforms.Resize(256, interpolation=3), transforms.CenterCrop(224)])
+    transform_imagenet_vis = transforms.Compose([transforms.Resize((224, 224), interpolation=3)])
+    transform_imagenet_norm = transforms.Compose([transforms.ToTensor(), transforms.Normalize(distributions["imagenet"]["mean"], distributions["imagenet"]["std"])])
 
-
-
-    transforms = {"imagenet" : transform_imagenet, "cifar" : transform_cifar}
+    # transforms.Resize(int((256 / 224) * input_size), interpolation=InterpolationMode.BICUBIC),
+    transforms = {"imagenet" : [transform_imagenet_vis, transform_imagenet_norm], "cifar" : transform_cifar}
 
     # CIFAR Setting
     # pip install cifar2png
     # cifar2png cifar100 ./cifar100
     # cifar2png cifar10  ./cifar10
     def validation(self, data):
         return data.lower()
@@ -35,37 +36,38 @@
 
     def normalize(self, image):
         result = copy.deepcopy(image)
         for c, (m, s) in enumerate(zip(self.distributions[self.d_kind]["mean"], self.distributions[self.d_kind]["std"])):
             result[:, c].sub_(m).div_(s)
         return result
 
-    def __init__(self, data_path="/hub_data/joonmyung/data", dataset="imagenet", device="cuda"):
+    def __init__(self, data_path="/hub_data1/joonmyung/data", dataset="imagenet", device="cuda"):
         dataset = dataset.lower()
 
         self.d      = dataset.lower()
         self.num_classes = 1000 if self.d == "imagenet" else 100
         [self.d_kind, self.d_type] = ["imagenet", "val"] if self.d == "imagenet" else ["cifar", "test"]
         # [self.d_kind, self.d_type] = ["imagenet", "train"] if self.d == "imagenet" else ["cifar", "test"]
         self.device = device
 
         self.transform = self.transforms[self.d_kind]
         self.data_path = data_path
         self.label_name = imnet_label if self.d_kind == "imagenet" else cifar_label
         self.label_paths = sorted(getDir(os.path.join(self.data_path, self.d_type)))
         self.img_paths = [sorted(glob.glob(os.path.join(self.data_path, self.d_type, label_path, "*"))) for label_path in self.label_paths]
 
-    def __getitem__(self, index=[0,0]):
-        label_num, img_num= index
+    def __getitem__(self, index):
+        label_num, img_num = index
         img_path = self.img_paths[label_num][img_num]
-        img = PIL.Image.open(img_path).resize((224, 224))
-        data = self.transform(img)
+        img = PIL.Image.open(img_path)
 
+        img = self.transform[0](img)
+        data = self.transform[1](img)
         return data.unsqueeze(0).to(self.device), torch.tensor(label_num).to(self.device), \
-                    img, self.label_name[label_num]
+                    img, self.label_name[int(label_num)]
     def getItems(self, indexs):
         ds, ls, ies, lns = [], [], [], []
         for index in indexs:
             d, l, i, ln = self.__getitem__(index)
             ds.append(d)
             ls.append(l)
             ies.append(i)
@@ -91,15 +93,13 @@
             std=self.distributions[self.d_kind]["std"],
             num_workers=8,
             crop_pct=0.9,
             pin_memory=False,
             tf_preprocessing=False)
         return loader
 
-if __name__ == "__main__":
-    root_path = "/hub_data/joonmyung/data"
-    dataset = "cifar100"
-    dataset = JDataset(root_path, dataset)
-    # sample  = dataset[0, 1]
-    samples = dataset.getitems([[0,1], [0,2], [0,3]])
-
-
+# if __name__ == "__main__":
+#     root_path = "/hub_data1/joonmyung/data"
+#     dataset = "cifar100"
+#     dataset = JDataset(root_path, dataset)
+#     # sample  = dataset[0, 1]
+#     samples = dataset.getitems([[0,1], [0,2], [0,3]])
```

### Comparing `joonmyung-1.4.4/joonmyung/analysis/metric.py` & `joonmyung-1.4.5/joonmyung/analysis/metric.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.4/joonmyung/analysis/model.py` & `joonmyung-1.4.5/joonmyung/analysis/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from playground.analysis.project.NeurIPS2023.versions.register_models import get_model
 from joonmyung.utils import isDir
 from timm import create_model
 import torch
 import os
 
 class JModel():
     def __init__(self, num_classes = None, root_path= None,
@@ -19,29 +18,29 @@
 
     def getModel(self, epoch=0, model_number=0, model_name = "deit_tiny", **kwargs):
         model, args = None, None
         if model_number == 0:
             model = create_model(model_name, pretrained=True, num_classes=self.num_classes, in_chans=3, global_pool=None, scriptable=False).to(self.device)
         elif model_number == 1:
             model = torch.hub.load('facebookresearch/deit:main', model_name, pretrained=True).to(self.device)
-        elif model_number == 2:
-            model_path = self.model_path.format(str(epoch))
-            if not isDir(model_path): raise FileExistsError
-
-            checkpoint = torch.load(model_path, map_location='cpu')
-            args = checkpoint['args']
-            if "token_merging" in kwargs.keys():
-                args.task_type[1] = 1 if kwargs["token_merging"] else 0
-
-            model = get_model(args).to(self.device)
-            state_dict = []
-            for n, p in checkpoint['model'].items():
-                if "total_ops" not in n and "total_params" not in n:
-                    state_dict.append((n, p))
-            state_dict = dict(state_dict)
-            model.load_state_dict(state_dict)
+        # elif model_number == 2:
+        #     model_path = self.model_path.format(str(epoch))
+        #     if not isDir(model_path): raise FileExistsError
+        #
+        #     checkpoint = torch.load(model_path, map_location='cpu')
+        #     args = checkpoint['args']
+        #     if "token_merging" in kwargs.keys():
+        #         args.task_type[1] = 1 if kwargs["token_merging"] else 0
+        #
+        #     model = get_model(args).to(self.device)
+        #     state_dict = []
+        #     for n, p in checkpoint['model'].items():
+        #         if "total_ops" not in n and "total_params" not in n:
+        #             state_dict.append((n, p))
+        #     state_dict = dict(state_dict)
+        #     model.load_state_dict(state_dict)
 
         model.eval()
 
         return model, args
```

### Comparing `joonmyung-1.4.4/joonmyung/app.py` & `joonmyung-1.4.5/joonmyung/app.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.4/joonmyung/data.py` & `joonmyung-1.4.5/joonmyung/data.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.4/joonmyung/draw.py` & `joonmyung-1.4.5/joonmyung/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,17 @@
          or type(datas) == PIL.Image.Image:
         pils = datas
     else:
         raise ValueError
     return pils
 
 def drawImgPlot(datas:list, col=1, title:str=None, columns=None, showRows:list=None,
-    output_dir=None, file_name=None, show=True, fmt=1, p=False):
+                output_dir='./', save_name=None, show=True, fmt=1,
+                vis_x = False, vis_y = False,
+                p=False):
     if type(datas) != list or 'shape' not in dir(datas[0]) : datas = [datas]
 
     if showRows is not None:
         for d in range(len(datas)):
             datas[d] = datas[d][showRows]
     data_num = len(datas[0]) * len(datas)
     row = (data_num - 1) // col + 1
@@ -247,25 +249,26 @@
             ax.imshow(data)
         elif data.shape[-1] == 3: #
             ax.imshow(data)
         elif data.shape[-1] == 1: #
             # ax.imshow(data, cmap="gray")
             sns.heatmap(data[:,:,0], annot=True, fmt=f".{fmt}f", cmap="Greys"
                         , yticklabels=False, xticklabels=False, ax=ax, vmax=1.0, vmin=0.0)
+
         if columns:
             ax.set_title(columns[c_num] + str(r_num)) if len(columns) == col else ax.set_title(columns[i])
-
-    plt.legend(bbox_to_anchor=(1.05, 1.0), loc='upper left')
+        if not vis_x: ax.xaxis.set_visible(False)
+        if not vis_x: ax.yaxis.set_visible(False)
     plt.tight_layout()
 
 
-    if output_dir and file_name:
+    if output_dir and save_name:
         if not os.path.exists(output_dir):
             os.makedirs(output_dir, exist_ok=True)
-        plt.savefig(os.path.join(output_dir, file_name))
+        plt.savefig(os.path.join(output_dir, f'{save_name}.png'))
     if show:
         plt.show()
 
 def overlay_mask(img: Image.Image, mask: Image.Image, colormap: str = "jet", alpha: float = 0.7) -> Image.Image:
     cmap = mpl.cm.get_cmap(colormap)
     # Resize mask and apply colormap
     overlay = mask.resize(img.size, resample=Image.BICUBIC)
```

### Comparing `joonmyung-1.4.4/joonmyung/file.py` & `joonmyung-1.4.5/joonmyung/file.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.4/joonmyung/gradcam.py` & `joonmyung-1.4.5/joonmyung/gradcam.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.4/joonmyung/meta_data/label.py` & `joonmyung-1.4.5/joonmyung/meta_data/label.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.4/joonmyung/meta_data/utils.py` & `joonmyung-1.4.5/joonmyung/meta_data/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,43 @@
+from joonmyung.meta_data.label import imnet_label, cifar_label
 import torch.nn.functional as F
 import pandas as pd
 import numpy as np
 import torch
+import socket
 import os
 
-from joonmyung.meta_data.label import imnet_label, cifar_label
 
 
-def data2path(server, dataset,
-              conference="", wandb_version="", wandb_name=""):
+def data2path(dataset, server = "",
+              conference="", wandb_version="", wandb_name="",
+              kisti_id=""):
+
+    # server = server if server else
+    hostname = socket.gethostname()
+    server = server if server is not "" \
+                else server if "mlv" in server \
+                    else "kakao" if "dakao" in hostname \
+                        else "kisti"
+
     if "kakao" in server:
-        data_path = "/data/opensets/imagenet-pytorch"
+        data_path = "/data/opensets"
         output_dir = "/data/project/rw/joonmyung/conference"
-    elif server in ["148", "137", "151", "152", "113", "68", "67", "64"]:
+    elif "mlv" in server:
         data_path = "/hub_data1/joonmyung/data"
         output_dir = "/hub_data1/joonmyung/conference"
-    elif server in ["154"]:
-        data_path = "/data1/joonmyung/data"
-        output_dir = "/data1/joonmyung/conference"
-    elif server in ["65"]:
-        data_path = "/hub_data2/joonmyung/data"
-        output_dir = "/hub_data2/joonmyung/conference"
     elif server in ["kisti"]:
-        data_path = "/scratch/x2487a05/data"
-        output_dir = "/scratch/x2487a05/data"
+        data_path = f"/scratch/{kisti_id}/data"
+        output_dir = f"/scratch/{kisti_id}/result"
     else:
         raise ValueError
 
     if dataset in ["imagenet", "IMNET"]:
-        if "kakao" in server:
-            data_path = os.path.join(data_path, "imagenet-pytorch")
-        else:
-            data_path = os.path.join(data_path, "imagenet")
-
-
-    output_dir = os.path.join(output_dir, conference, wandb_version, wandb_name) if conference else None
-
+        data_path = os.path.join(data_path, "imagenet") if "kakao" not in server else os.path.join(data_path, "imagenet-pytorch")
+    output_dir = os.path.join(output_dir, conference, wandb_version, wandb_name)
 
     return data_path, output_dir
 
 def get_label(key, d_name ="imagenet"):
     d_name = d_name.lower()
     if d_name in ["imagenet", "IMNET"] :
         return imnet_label[key]
@@ -66,7 +64,9 @@
     return F.softmax(torch.randn(shape), dim=dim)
 
 def set_dtype(df, dtypes):
     for c_n, d_t in dtypes.items():
         if c_n in df.columns:
             df[c_n] = df[c_n].astype(d_t)
     return df
+
+
```

### Comparing `joonmyung-1.4.4/joonmyung/script.py` & `joonmyung-1.4.5/joonmyung/script.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.4/joonmyung/status.py` & `joonmyung-1.4.5/joonmyung/status.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.4/joonmyung/utils.py` & `joonmyung-1.4.5/joonmyung/utils.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.4/joonmyung.egg-info/SOURCES.txt` & `joonmyung-1.4.5/joonmyung.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.py
 joonmyung/__init__.py
 joonmyung/app.py
 joonmyung/data.py
 joonmyung/draw.py
 joonmyung/dummy.py
```

### Comparing `joonmyung-1.4.4/setup.py` & `joonmyung-1.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from setuptools import find_packages
 setuptools.setup(
     name="joonmyung",
-    version="1.4.4",
+    version="1.4.5",
     author="JoonMyung Choi",
     author_email="pizard@korea.ac.kr",
     description="JoonMyung's Library",
     url="https://github.com/pizard/JoonMyung.git",
     license="MIT",
     packages=find_packages(exclude=["playground",
                                     "playground.*",
```

