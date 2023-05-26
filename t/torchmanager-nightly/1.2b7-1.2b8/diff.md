# Comparing `tmp/torchmanager_nightly-1.2b7.tar.gz` & `tmp/torchmanager_nightly-1.2b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager_nightly-1.2b7.tar", max compression
+gzip compressed data, was "torchmanager_nightly-1.2b8.tar", max compression
```

## Comparing `torchmanager_nightly-1.2b7.tar` & `torchmanager_nightly-1.2b8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1318 2023-03-14 14:54:20.813363 torchmanager_nightly-1.2b7/LICENSE
--rw-r--r--   0        0        0      659 2023-05-23 18:57:38.725893 torchmanager_nightly-1.2b7/pyproject.toml
--rw-r--r--   0        0        0      290 2023-05-23 18:57:38.726329 torchmanager_nightly-1.2b7/torchmanager/__init__.py
--rw-r--r--   0        0        0    10862 2023-05-23 18:57:38.726797 torchmanager_nightly-1.2b7/torchmanager/basic.py
--rw-r--r--   0        0        0      638 2023-05-23 18:57:38.727334 torchmanager_nightly-1.2b7/torchmanager/callbacks/__init__.py
--rw-r--r--   0        0        0     4444 2023-05-23 18:57:38.727736 torchmanager_nightly-1.2b7/torchmanager/callbacks/callback.py
--rw-r--r--   0        0        0     4628 2023-05-15 18:28:33.014982 torchmanager_nightly-1.2b7/torchmanager/callbacks/ckpt.py
--rw-r--r--   0        0        0     3523 2023-05-09 14:19:55.056821 torchmanager_nightly-1.2b7/torchmanager/callbacks/dynamic.py
--rw-r--r--   0        0        0     1608 2023-05-09 14:19:55.056902 torchmanager_nightly-1.2b7/torchmanager/callbacks/early_stop.py
--rw-r--r--   0        0        0     4642 2023-05-23 18:57:38.728136 torchmanager_nightly-1.2b7/torchmanager/callbacks/experiment.py
--rw-r--r--   0        0        0     2224 2023-05-09 14:19:55.057101 torchmanager_nightly-1.2b7/torchmanager/callbacks/lr.py
--rw-r--r--   0        0        0     2599 2023-05-23 18:57:38.728530 torchmanager_nightly-1.2b7/torchmanager/callbacks/tensorboard.py
--rw-r--r--   0        0        0      964 2023-05-23 18:57:38.729162 torchmanager_nightly-1.2b7/torchmanager/compatibility.py
--rw-r--r--   0        0        0       26 2023-05-23 18:57:38.729492 torchmanager_nightly-1.2b7/torchmanager/configs/__init__.py
--rw-r--r--   0        0        0     3013 2023-05-23 18:57:38.729718 torchmanager_nightly-1.2b7/torchmanager/configs/basic.py
--rw-r--r--   0        0        0       85 2023-05-09 14:19:55.057599 torchmanager_nightly-1.2b7/torchmanager/data/__init__.py
--rw-r--r--   0        0        0     6968 2023-05-23 18:57:38.730045 torchmanager_nightly-1.2b7/torchmanager/data/dataset.py
--rw-r--r--   0        0        0     2238 2023-05-23 18:57:38.730234 torchmanager_nightly-1.2b7/torchmanager/data/sliding.py
--rw-r--r--   0        0        0      156 2023-05-23 18:57:38.730592 torchmanager_nightly-1.2b7/torchmanager/losses/__init__.py
--rw-r--r--   0        0        0     5386 2023-05-09 14:19:55.058468 torchmanager_nightly-1.2b7/torchmanager/losses/cross_entropy.py
--rw-r--r--   0        0        0     1047 2023-05-23 18:57:38.731189 torchmanager_nightly-1.2b7/torchmanager/losses/dice.py
--rw-r--r--   0        0        0     5757 2023-05-23 18:57:38.731564 torchmanager_nightly-1.2b7/torchmanager/losses/loss.py
--rw-r--r--   0        0        0     3117 2023-05-23 18:57:38.731935 torchmanager_nightly-1.2b7/torchmanager/losses/mse.py
--rw-r--r--   0        0        0      362 2023-05-23 18:58:49.721266 torchmanager_nightly-1.2b7/torchmanager/metrics/__init__.py
--rw-r--r--   0        0        0     4033 2023-05-23 18:57:38.732808 torchmanager_nightly-1.2b7/torchmanager/metrics/accuracy.py
--rw-r--r--   0        0        0     3678 2023-05-23 18:57:38.733030 torchmanager_nightly-1.2b7/torchmanager/metrics/conf_met.py
--rw-r--r--   0        0        0     5139 2023-05-23 18:57:38.733329 torchmanager_nightly-1.2b7/torchmanager/metrics/extractor.py
--rw-r--r--   0        0        0     2070 2023-05-23 18:57:38.733518 torchmanager_nightly-1.2b7/torchmanager/metrics/iou.py
--rw-r--r--   0        0        0     4003 2023-05-23 18:57:38.734103 torchmanager_nightly-1.2b7/torchmanager/metrics/metric.py
--rw-r--r--   0        0        0     2220 2023-05-23 18:57:38.734335 torchmanager_nightly-1.2b7/torchmanager/metrics/similarity.py
--rw-r--r--   0        0        0     9558 2023-05-23 18:57:38.734660 torchmanager_nightly-1.2b7/torchmanager/testing.py
--rw-r--r--   0        0        0       96 2023-05-23 18:57:38.734979 torchmanager_nightly-1.2b7/torchmanager/train/__init__.py
--rw-r--r--   0        0        0     4964 2023-05-09 14:19:55.060536 torchmanager_nightly-1.2b7/torchmanager/train/checkpoint.py
--rw-r--r--   0        0        0      694 2023-05-23 18:57:38.735541 torchmanager_nightly-1.2b7/torchmanager/train/learning_rate.py
--rw-r--r--   0        0        0    13808 2023-05-23 18:57:38.736027 torchmanager_nightly-1.2b7/torchmanager/training.py
--rw-r--r--   0        0        0      459 2023-05-23 18:57:38.736545 torchmanager_nightly-1.2b7/torchmanager_core/__init__.py
--rw-r--r--   0        0        0      109 2023-05-23 18:57:38.737397 torchmanager_nightly-1.2b7/torchmanager_core/devices/__init__.py
--rw-r--r--   0        0        0     4879 2023-05-23 18:57:38.737605 torchmanager_nightly-1.2b7/torchmanager_core/devices/device.py
--rw-r--r--   0        0        0      264 2023-05-09 14:19:55.062103 torchmanager_nightly-1.2b7/torchmanager_core/devices/protocols.py
--rw-r--r--   0        0        0      153 2023-05-09 14:25:54.610406 torchmanager_nightly-1.2b7/torchmanager_core/errors/__init__.py
--rw-r--r--   0        0        0      350 2023-05-09 14:19:55.062828 torchmanager_nightly-1.2b7/torchmanager_core/errors/runtime.py
--rw-r--r--   0        0        0      669 2023-05-09 14:19:55.063042 torchmanager_nightly-1.2b7/torchmanager_core/errors/train.py
--rw-r--r--   0        0        0     2772 2023-05-23 18:57:38.737932 torchmanager_nightly-1.2b7/torchmanager_core/protocols.py
--rw-r--r--   0        0        0       44 2023-05-23 18:57:38.738272 torchmanager_nightly-1.2b7/torchmanager_core/random/__init__.py
--rw-r--r--   0        0        0     1029 2023-05-23 18:57:38.738579 torchmanager_nightly-1.2b7/torchmanager_core/random/seed.py
--rw-r--r--   0        0        0      204 2023-05-09 14:19:55.064483 torchmanager_nightly-1.2b7/torchmanager_core/typing.py
--rw-r--r--   0        0        0     5260 2023-05-23 18:57:38.738874 torchmanager_nightly-1.2b7/torchmanager_core/version.py
--rw-r--r--   0        0        0      439 2023-05-23 18:57:38.739234 torchmanager_nightly-1.2b7/torchmanager_core/view/__init__.py
--rw-r--r--   0        0        0      313 2023-05-09 14:19:55.065240 torchmanager_nightly-1.2b7/torchmanager_core/view/protocols.py
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 torchmanager_nightly-1.2b7/PKG-INFO
+-rw-r--r--   0        0        0     1318 2023-04-21 19:45:23.217167 torchmanager_nightly-1.2b8/LICENSE
+-rw-r--r--   0        0        0      659 2023-05-26 15:09:49.947121 torchmanager_nightly-1.2b8/pyproject.toml
+-rw-r--r--   0        0        0      290 2023-05-26 15:07:26.272267 torchmanager_nightly-1.2b8/torchmanager/__init__.py
+-rw-r--r--   0        0        0    10862 2023-05-26 15:07:26.273598 torchmanager_nightly-1.2b8/torchmanager/basic.py
+-rw-r--r--   0        0        0      638 2023-05-26 15:07:26.275089 torchmanager_nightly-1.2b8/torchmanager/callbacks/__init__.py
+-rw-r--r--   0        0        0     4444 2023-05-26 15:07:26.276587 torchmanager_nightly-1.2b8/torchmanager/callbacks/callback.py
+-rw-r--r--   0        0        0     4628 2023-05-26 14:55:58.693727 torchmanager_nightly-1.2b8/torchmanager/callbacks/ckpt.py
+-rw-r--r--   0        0        0     3523 2023-05-26 14:55:58.693887 torchmanager_nightly-1.2b8/torchmanager/callbacks/dynamic.py
+-rw-r--r--   0        0        0     1608 2023-05-26 14:55:58.694033 torchmanager_nightly-1.2b8/torchmanager/callbacks/early_stop.py
+-rw-r--r--   0        0        0     4642 2023-05-26 15:07:26.277845 torchmanager_nightly-1.2b8/torchmanager/callbacks/experiment.py
+-rw-r--r--   0        0        0     2224 2023-05-26 14:55:58.694400 torchmanager_nightly-1.2b8/torchmanager/callbacks/lr.py
+-rw-r--r--   0        0        0     2599 2023-05-26 15:07:26.278448 torchmanager_nightly-1.2b8/torchmanager/callbacks/tensorboard.py
+-rw-r--r--   0        0        0      964 2023-05-26 15:07:26.279144 torchmanager_nightly-1.2b8/torchmanager/compatibility.py
+-rw-r--r--   0        0        0       26 2023-05-26 15:07:26.279332 torchmanager_nightly-1.2b8/torchmanager/configs/__init__.py
+-rw-r--r--   0        0        0     3013 2023-05-26 15:07:26.280129 torchmanager_nightly-1.2b8/torchmanager/configs/basic.py
+-rw-r--r--   0        0        0       85 2023-05-26 14:55:58.695089 torchmanager_nightly-1.2b8/torchmanager/data/__init__.py
+-rw-r--r--   0        0        0     6968 2023-05-26 15:07:26.280966 torchmanager_nightly-1.2b8/torchmanager/data/dataset.py
+-rw-r--r--   0        0        0     2238 2023-05-26 15:07:26.281606 torchmanager_nightly-1.2b8/torchmanager/data/sliding.py
+-rw-r--r--   0        0        0      156 2023-05-26 15:07:26.282249 torchmanager_nightly-1.2b8/torchmanager/losses/__init__.py
+-rw-r--r--   0        0        0     5386 2023-05-26 14:55:58.695855 torchmanager_nightly-1.2b8/torchmanager/losses/cross_entropy.py
+-rw-r--r--   0        0        0     1047 2023-05-26 15:07:26.282728 torchmanager_nightly-1.2b8/torchmanager/losses/dice.py
+-rw-r--r--   0        0        0     5757 2023-05-26 15:07:26.283917 torchmanager_nightly-1.2b8/torchmanager/losses/loss.py
+-rw-r--r--   0        0        0     3117 2023-05-26 15:07:26.284752 torchmanager_nightly-1.2b8/torchmanager/losses/mse.py
+-rw-r--r--   0        0        0      362 2023-05-26 15:07:26.285400 torchmanager_nightly-1.2b8/torchmanager/metrics/__init__.py
+-rw-r--r--   0        0        0     4033 2023-05-26 15:07:26.286652 torchmanager_nightly-1.2b8/torchmanager/metrics/accuracy.py
+-rw-r--r--   0        0        0     3678 2023-05-26 15:07:26.287441 torchmanager_nightly-1.2b8/torchmanager/metrics/conf_met.py
+-rw-r--r--   0        0        0     5139 2023-05-26 15:07:26.287876 torchmanager_nightly-1.2b8/torchmanager/metrics/extractor.py
+-rw-r--r--   0        0        0     2070 2023-05-26 15:07:26.288465 torchmanager_nightly-1.2b8/torchmanager/metrics/iou.py
+-rw-r--r--   0        0        0     4003 2023-05-26 15:07:26.289542 torchmanager_nightly-1.2b8/torchmanager/metrics/metric.py
+-rw-r--r--   0        0        0     2307 2023-05-26 15:09:49.947536 torchmanager_nightly-1.2b8/torchmanager/metrics/similarity.py
+-rw-r--r--   0        0        0     9558 2023-05-26 15:07:26.290610 torchmanager_nightly-1.2b8/torchmanager/testing.py
+-rw-r--r--   0        0        0       96 2023-05-26 15:07:26.291264 torchmanager_nightly-1.2b8/torchmanager/train/__init__.py
+-rw-r--r--   0        0        0     4964 2023-05-26 14:55:58.698577 torchmanager_nightly-1.2b8/torchmanager/train/checkpoint.py
+-rw-r--r--   0        0        0      694 2023-05-26 15:07:26.291528 torchmanager_nightly-1.2b8/torchmanager/train/learning_rate.py
+-rw-r--r--   0        0        0    13808 2023-05-26 15:07:26.292056 torchmanager_nightly-1.2b8/torchmanager/training.py
+-rw-r--r--   0        0        0      459 2023-05-26 15:07:26.292957 torchmanager_nightly-1.2b8/torchmanager_core/__init__.py
+-rw-r--r--   0        0        0      109 2023-05-26 15:07:26.293236 torchmanager_nightly-1.2b8/torchmanager_core/devices/__init__.py
+-rw-r--r--   0        0        0     4879 2023-05-26 15:07:26.293903 torchmanager_nightly-1.2b8/torchmanager_core/devices/device.py
+-rw-r--r--   0        0        0      264 2023-05-26 14:55:58.701197 torchmanager_nightly-1.2b8/torchmanager_core/devices/protocols.py
+-rw-r--r--   0        0        0      153 2023-05-26 14:55:58.701398 torchmanager_nightly-1.2b8/torchmanager_core/errors/__init__.py
+-rw-r--r--   0        0        0      350 2023-05-26 14:55:58.701746 torchmanager_nightly-1.2b8/torchmanager_core/errors/runtime.py
+-rw-r--r--   0        0        0      669 2023-05-26 14:55:58.701938 torchmanager_nightly-1.2b8/torchmanager_core/errors/train.py
+-rw-r--r--   0        0        0     2772 2023-05-26 15:07:26.294864 torchmanager_nightly-1.2b8/torchmanager_core/protocols.py
+-rw-r--r--   0        0        0       44 2023-05-26 15:07:26.295205 torchmanager_nightly-1.2b8/torchmanager_core/random/__init__.py
+-rw-r--r--   0        0        0     1029 2023-05-26 15:07:26.295759 torchmanager_nightly-1.2b8/torchmanager_core/random/seed.py
+-rw-r--r--   0        0        0      204 2023-05-26 14:55:58.702551 torchmanager_nightly-1.2b8/torchmanager_core/typing.py
+-rw-r--r--   0        0        0     5260 2023-05-26 15:09:49.948122 torchmanager_nightly-1.2b8/torchmanager_core/version.py
+-rw-r--r--   0        0        0      439 2023-05-26 15:07:26.296612 torchmanager_nightly-1.2b8/torchmanager_core/view/__init__.py
+-rw-r--r--   0        0        0      313 2023-05-26 14:55:58.703314 torchmanager_nightly-1.2b8/torchmanager_core/view/protocols.py
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 torchmanager_nightly-1.2b8/PKG-INFO
```

### Comparing `torchmanager_nightly-1.2b7/LICENSE` & `torchmanager_nightly-1.2b8/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/pyproject.toml` & `torchmanager_nightly-1.2b8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "torchmanager-nightly"
-version = "1.2b7"
-description = "PyTorch Training Manager v1.2 (Beta 7)"
+version = "1.2b8"
+description = "PyTorch Training Manager v1.2 (Beta 8)"
 authors = ["Qisheng He <Qisheng.He@wayne.edu>"]
 repository = "https://github.com/kisonho/torchmanager.git"
 packages = [
     { include = "torchmanager" },
     { include = "torchmanager_core" },
 ]
```

### Comparing `torchmanager_nightly-1.2b7/torchmanager/basic.py` & `torchmanager_nightly-1.2b8/torchmanager/basic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/callbacks/__init__.py` & `torchmanager_nightly-1.2b8/torchmanager/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/callbacks/callback.py` & `torchmanager_nightly-1.2b8/torchmanager/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/callbacks/ckpt.py` & `torchmanager_nightly-1.2b8/torchmanager/callbacks/ckpt.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/callbacks/dynamic.py` & `torchmanager_nightly-1.2b8/torchmanager/callbacks/dynamic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/callbacks/early_stop.py` & `torchmanager_nightly-1.2b8/torchmanager/callbacks/early_stop.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/callbacks/experiment.py` & `torchmanager_nightly-1.2b8/torchmanager/callbacks/experiment.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/callbacks/lr.py` & `torchmanager_nightly-1.2b8/torchmanager/callbacks/lr.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/callbacks/tensorboard.py` & `torchmanager_nightly-1.2b8/torchmanager/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/compatibility.py` & `torchmanager_nightly-1.2b8/torchmanager/compatibility.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/configs/basic.py` & `torchmanager_nightly-1.2b8/torchmanager/configs/basic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/data/dataset.py` & `torchmanager_nightly-1.2b8/torchmanager/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/data/sliding.py` & `torchmanager_nightly-1.2b8/torchmanager/data/sliding.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/losses/cross_entropy.py` & `torchmanager_nightly-1.2b8/torchmanager/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/losses/dice.py` & `torchmanager_nightly-1.2b8/torchmanager/losses/dice.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/losses/loss.py` & `torchmanager_nightly-1.2b8/torchmanager/losses/loss.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/losses/mse.py` & `torchmanager_nightly-1.2b8/torchmanager/losses/mse.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/metrics/accuracy.py` & `torchmanager_nightly-1.2b8/torchmanager/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/metrics/conf_met.py` & `torchmanager_nightly-1.2b8/torchmanager/metrics/conf_met.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/metrics/extractor.py` & `torchmanager_nightly-1.2b8/torchmanager/metrics/extractor.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/metrics/iou.py` & `torchmanager_nightly-1.2b8/torchmanager/metrics/iou.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/metrics/metric.py` & `torchmanager_nightly-1.2b8/torchmanager/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/metrics/similarity.py` & `torchmanager_nightly-1.2b8/torchmanager/metrics/similarity.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,23 +35,23 @@
         window = window.unsqueeze(1)
         window = window.mm(window.t()).float().unsqueeze(0).unsqueeze(0)
         window = window.expand(channels, 1, window_size, window_size).contiguous()
         self.window = window
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         # calculate mean
-        mu1 = F.conv2d(input, self.window, padding=self.window_size // 2, groups=input.shape[1])
-        mu2 = F.conv2d(target, self.window, padding=self.window_size // 2, groups=target.shape[1])
+        mu1 = F.conv2d(input, self.window.to(input.device), padding=self.window_size // 2, groups=input.shape[1])
+        mu2 = F.conv2d(target, self.window.to(target.device), padding=self.window_size // 2, groups=target.shape[1])
         mu1_sq = mu1.pow(2)
         mu2_sq = mu2.pow(2)
         mu1_mu2 = mu1 * mu2
 
         # calculate sigma
-        sigma1_sq = F.conv2d(input * input, self.window, padding=self.window_size // 2, stride=1, groups=input.shape[1]) - mu1_sq
-        sigma2_sq = F.conv2d(target * target, self.window, padding=self.window_size // 2, stride=1, groups=target.shape[1]) - mu2_sq
-        sigma12 = F.conv2d(input * target, self.window, padding=self.window_size // 2, stride=1, groups=input.shape[1]) - mu1_mu2
+        sigma1_sq = F.conv2d(input * input, self.window.to(input.device), padding=self.window_size // 2, stride=1, groups=input.shape[1]) - mu1_sq
+        sigma2_sq = F.conv2d(target * target, self.window.to(target.device), padding=self.window_size // 2, stride=1, groups=target.shape[1]) - mu2_sq
+        sigma12 = F.conv2d(input * target, self.window.to(input.device), padding=self.window_size // 2, stride=1, groups=input.shape[1]) - mu1_mu2
 
         # calculate ssim
         C1 = (0.01 * 255) ** 2
         C2 = (0.03 * 255) ** 2
         ssim = ((2 * mu1_mu2 + C1) * (2 * sigma12 + C2)) / ((mu1_sq + mu2_sq + C1) * (sigma1_sq + sigma2_sq + C2))
         return ssim.mean()
```

### Comparing `torchmanager_nightly-1.2b7/torchmanager/testing.py` & `torchmanager_nightly-1.2b8/torchmanager/testing.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/train/checkpoint.py` & `torchmanager_nightly-1.2b8/torchmanager/train/checkpoint.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/train/learning_rate.py` & `torchmanager_nightly-1.2b8/torchmanager/train/learning_rate.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager/training.py` & `torchmanager_nightly-1.2b8/torchmanager/training.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager_core/devices/device.py` & `torchmanager_nightly-1.2b8/torchmanager_core/devices/device.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager_core/errors/train.py` & `torchmanager_nightly-1.2b8/torchmanager_core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager_core/protocols.py` & `torchmanager_nightly-1.2b8/torchmanager_core/protocols.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager_core/random/seed.py` & `torchmanager_nightly-1.2b8/torchmanager_core/random/seed.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b7/torchmanager_core/version.py` & `torchmanager_nightly-1.2b8/torchmanager_core/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,16 @@
         return self == other or self < other
 
     def __ge__(self, other: Any) -> bool:
         return self == other or self > other
 
 
 API = Version("v1.2")
-CURRENT = Version("v1.2b7")
-DESCRIPTION: str = "PyTorch Training Manager v1.2 (Beta 7)"
+CURRENT = Version("v1.2b8")
+DESCRIPTION: str = "PyTorch Training Manager v1.2 (Beta 8)"
 
 
 class VersionError(SystemError):
     def __init__(self, method_name: str, maximum_supported_version: str) -> None:
         super().__init__(f"`{method_name}` has been deprecated and removed from version {maximum_supported_version}. Current version: {CURRENT}.")
```

### Comparing `torchmanager_nightly-1.2b7/PKG-INFO` & `torchmanager_nightly-1.2b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: torchmanager-nightly
-Version: 1.2b7
-Summary: PyTorch Training Manager v1.2 (Beta 7)
+Version: 1.2b8
+Summary: PyTorch Training Manager v1.2 (Beta 8)
 Home-page: https://github.com/kisonho/torchmanager.git
 Author: Qisheng He
 Author-email: Qisheng.He@wayne.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

