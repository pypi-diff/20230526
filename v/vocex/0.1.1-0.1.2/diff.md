# Comparing `tmp/vocex-0.1.1.tar.gz` & `tmp/vocex-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocex-0.1.1.tar", last modified: Wed May 24 10:47:03 2023, max compression
+gzip compressed data, was "vocex-0.1.2.tar", last modified: Thu May 25 22:34:00 2023, max compression
```

## Comparing `vocex-0.1.1.tar` & `vocex-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,11 @@
--rw-r--r--   0        0        0        8 2023-05-08 02:42:27.826184 vocex-0.1.1/README.md
--rw-r--r--   0        0        0      398 2023-05-24 10:47:03.325288 vocex-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 21:58:56.410903 vocex-0.1.1/training/__init__.py
--rw-r--r--   0        0        0     1292 2023-05-24 00:56:28.799940 vocex-0.1.1/training/arguments.py
--rw-r--r--   0        0        0      934 2023-05-14 19:16:02.031062 vocex-0.1.1/training/data/phone2idx.json
--rw-r--r--   0        0        0    32624 2023-05-14 19:16:48.039523 vocex-0.1.1/training/data/speaker2idx.json
--rw-r--r--   0        0        0       34 2023-05-07 15:52:27.868453 vocex-0.1.1/vocex/__init__.py
--rw-r--r--   0        0        0     2025 2023-05-07 15:53:39.423391 vocex-0.1.1/vocex/conformer_layer.py
--rw-r--r--   0        0        0     6729 2023-05-24 00:42:33.325126 vocex-0.1.1/vocex/conformer_model.py
--rw-r--r--   0        0        0     4209 2023-05-16 09:01:55.015467 vocex-0.1.1/vocex/scaler.py
--rw-r--r--   0        0        0     3845 2023-05-08 13:55:39.298893 vocex-0.1.1/vocex/tpu_metrics_delta.py
--rw-r--r--   0        0        0     2460 2023-05-07 15:45:50.981971 vocex-0.1.1/vocex/transformer.py
--rw-r--r--   0        0        0     1756 2023-05-09 04:48:57.299991 vocex-0.1.1/vocex/utils.py
--rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 vocex-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        8 2023-05-08 02:42:27.826184 vocex-0.1.2/README.md
+-rw-r--r--   0        0        0      398 2023-05-25 22:34:00.644389 vocex-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-07 15:52:27.868453 vocex-0.1.2/vocex/__init__.py
+-rw-r--r--   0        0        0     2025 2023-05-07 15:53:39.423391 vocex-0.1.2/vocex/conformer_layer.py
+-rw-r--r--   0        0        0     8798 2023-05-25 17:38:23.728729 vocex-0.1.2/vocex/conformer_model.py
+-rw-r--r--   0        0        0     4209 2023-05-24 16:42:44.629275 vocex-0.1.2/vocex/scaler.py
+-rw-r--r--   0        0        0     3830 2023-05-24 18:47:16.895683 vocex-0.1.2/vocex/softdtw.py
+-rw-r--r--   0        0        0     3845 2023-05-08 13:55:39.298893 vocex-0.1.2/vocex/tpu_metrics_delta.py
+-rw-r--r--   0        0        0     2460 2023-05-07 15:45:50.981971 vocex-0.1.2/vocex/transformer.py
+-rw-r--r--   0        0        0     1756 2023-05-09 04:48:57.299991 vocex-0.1.2/vocex/utils.py
+-rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 vocex-0.1.2/PKG-INFO
```

### Comparing `vocex-0.1.1/vocex/conformer_layer.py` & `vocex-0.1.2/vocex/conformer_layer.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.1/vocex/conformer_model.py` & `vocex-0.1.2/vocex/conformer_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from torch import nn
 from tqdm.auto import tqdm
 from .transformer import TransformerEncoder, PositionalEncoding
 from .conformer_layer import ConformerLayer
 from .scaler import GaussianMinMaxScaler
 from .utils import Transpose, NoamLR
 from .tpu_metrics_delta import MetricsDelta
+from .softdtw import SoftDTW
 
 class Vocex(nn.Module):
 
     def __init__(
         self,
         measures=["energy", "pitch", "srmr", "snr"],
         in_channels=80,
@@ -17,14 +18,16 @@
         kernel_size=3,
         dropout=0.1,
         depthwise=True,
         measure_nlayers=4,
         dvector_dim=256,
         dvector_nlayers=2,
         noise_factor=0.1,
+        use_softdtw=False,
+        softdtw_gamma=1.0,
     ):
         super().__init__()
         self.measures = measures
         self.noise_factor = noise_factor
         in_channels = in_channels
         filter_size = filter_size
         kernel_size = kernel_size
@@ -56,14 +59,17 @@
             nn.Linear(filter_size, 1024),
             nn.ReLU(),
             nn.Linear(1024, 1024),
             nn.ReLU(),
             nn.Linear(1024, num_outputs),
         )
         
+        self.dvector_conv_in_layer = nn.Linear(filter_size, filter_size)
+        self.dvector_x_in_layer = nn.Linear(in_channels, filter_size)
+
         self.dvector_layers = TransformerEncoder(
             ConformerLayer(
                 filter_size,
                 2,
                 conv_in=filter_size,
                 conv_filter_size=filter_size,
                 conv_kernel=(kernel_size, 1),
@@ -82,18 +88,24 @@
             nn.Linear(1024, 1024),
             nn.ReLU(),
             nn.Linear(1024, dvector_dim),
         )
 
         self.scaler_dict = {
             k: GaussianMinMaxScaler(10) for k in self.measures
+            if not k.endswith("_binary")
         }
         self.scaler_dict["mel"] = GaussianMinMaxScaler(10)
         self.scaler_dict["dvector"] = GaussianMinMaxScaler(10)
         self.scaler_dict = nn.ModuleDict(self.scaler_dict)
+        self.use_softdtw = use_softdtw
+        if self.use_softdtw:
+            self.softdtw = SoftDTW(gamma=softdtw_gamma)
+
+        self.verbose = False
 
         self.apply(self._init_weights)
 
     @property
     def scalers(self):
         return self.scaler_dict
 
@@ -109,66 +121,94 @@
     def fit_scalers(self, dataloader, n_batches=1000):
         # reset scalers
         for k in self.scalers:
             self.scalers[k].is_fit = False
         for i, batch in tqdm(enumerate(dataloader), desc="Fitting scalers", total=n_batches):
             self.scalers["mel"].partial_fit(batch["mel"])
             for k in self.measures:
-                self.scalers[k].partial_fit(batch["measures"][k])
+                if not k.endswith("_binary"):
+                    self.scalers[k].partial_fit(batch["measures"][k])
             self.scalers["dvector"].partial_fit(batch["dvector"])
             if i >= n_batches:
                 break
         for k in self.scalers:
             self.scalers[k].is_fit = True
 
     def forward(self, mel, dvector=None, measures=None, inference=False):
+        mel_padding_mask = mel.sum(dim=-1) != 0
+        mel_padding_mask = mel_padding_mask.to(torch.float32)
         if not self.scalers["mel"].is_fit:
             self.scalers["mel"].partial_fit(mel)
         x = self.scalers["mel"].transform(mel)
         x = x + (torch.randn_like(x) * x.std() + x.mean()) * self.noise_factor
-        x = self.in_layer(x)
-        x = self.positional_encoding(x)
-        out_conv = self.layers(x)
+        out = self.in_layer(x)
+        if self.verbose:
+            print(out.mean(), "1")
+        out = self.positional_encoding(out)
+        if self.verbose:
+            print(out.mean(), "2")
+        out_conv = self.layers(out, src_key_padding_mask=mel_padding_mask)
+        if self.verbose:
+            print(out_conv.mean(), "3")
         out = self.linear(out_conv)
+        if self.verbose:
+            print(out.mean(), "4")
         out = out.transpose(1, 2)
         measure_results = {}
         measure_true = {}
         loss_dict = {}
+        for i, measure in enumerate(self.measures):
+            measure_out = out[:, i]
+            if not measure.endswith("_binary") and not self.scalers[measure].is_fit:
+                self.scalers[measure].partial_fit(measures[measure])
+            measure_results[measure] = measure_out
         if measures is not None:
             loss_dict = {}
-            for i, measure in enumerate(self.measures):
-                measure_out = out[:, i]
-                if not self.scalers[measure].is_fit:
-                    self.scalers[measure].partial_fit(measures[measure])
-                measure_results[measure] = measure_out
-                measure_true[measure] = self.scalers[measure].transform(measures[measure])
+            for measure in self.measures:
+                if not measure.endswith("_binary"):
+                    measure_true[measure] = self.scalers[measure].transform(measures[measure])
+                else:
+                    measure_true[measure] = measures[measure]
             measures_losses = []
             for measure in self.measures:
-                m_loss = nn.MSELoss()(measure_results[measure], measure_true[measure])
+                if measure.endswith("_binary"):
+                    m_loss = nn.BCEWithLogitsLoss()(measure_results[measure]*mel_padding_mask, measure_true[measure]*mel_padding_mask)
+                else:
+                    if not self.use_softdtw:
+                        m_loss = nn.MSELoss()(measure_results[measure]*mel_padding_mask, measure_true[measure]*mel_padding_mask)
+                    else:
+                        if self.verbose:
+                            print(measure_results[measure], measure_true[measure])
+                        m_loss = self.softdtw(
+                            measure_results[measure]*mel_padding_mask,
+                            measure_true[measure]*mel_padding_mask,
+                        ) / 1000
                 loss_dict[measure] = m_loss
                 measures_losses.append(m_loss)
             loss = sum(measures_losses) / len(self.measures)
         else:
             loss = None
         ### d-vector
         # predict d-vector using global average and max pooling as input
-        out_dvec = self.dvector_layers(x)
+        out_conv_dvec = self.dvector_conv_in_layer(out_conv)
+        x = self.dvector_x_in_layer(x)
+        out_dvec = self.dvector_layers(out_conv_dvec + x, src_key_padding_mask=mel_padding_mask)
         dvector_input = torch.cat(
             [
                 torch.mean(out_dvec, dim=1),
                 torch.max(out_dvec, dim=1)[0],
             ],
             dim=1,
         )
         dvector_pred = self.dvector_linear(dvector_input)
         if dvector is not None:
             if not self.scalers["dvector"].is_fit:
                 self.scalers["dvector"].partial_fit(dvector)
             true_dvector = self.scalers["dvector"].transform(dvector)
-            dvector_loss = nn.MSELoss()(dvector_pred, true_dvector)
+            dvector_loss = nn.L1Loss()(dvector_pred, true_dvector)
             loss_dict["dvector"] = dvector_loss
             if loss is not None:
                 loss += dvector_loss
                 loss /= 2
             else:
                 loss = dvector_loss
         if not inference:
@@ -176,17 +216,20 @@
                 "loss": loss,
                 "compound_losses": loss_dict,
             }
             return results
         else:
             # transform back to original scale
             for measure in self.measures:
-                measure_results[measure] = self.scalers[measure].inverse_transform(
-                    measure_results[measure]
-                )
+                if not measure.endswith("_binary"):
+                    measure_results[measure] = self.scalers[measure].inverse_transform(
+                        measure_results[measure]
+                    )
+                else:
+                    measure_results[measure] = torch.sigmoid(measure_results[measure]).detach()
             dvector_pred = self.scalers["dvector"].inverse_transform(dvector_pred)
             results = {
                 "loss": loss,
                 "compound_losses": loss_dict,
                 "measures": measure_results,
                 "dvector": dvector_pred,
             }
```

### Comparing `vocex-0.1.1/vocex/scaler.py` & `vocex-0.1.2/vocex/scaler.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.1/vocex/tpu_metrics_delta.py` & `vocex-0.1.2/vocex/tpu_metrics_delta.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.1/vocex/transformer.py` & `vocex-0.1.2/vocex/transformer.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.1/vocex/utils.py` & `vocex-0.1.2/vocex/utils.py`

 * *Files identical despite different names*

