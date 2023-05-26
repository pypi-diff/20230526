# Comparing `tmp/dwiqc-0.2.0-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.2.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 22467 bytes, number of entries: 21
+Zip file size: 22654 bytes, number of entries: 21
 -rw-r--r--  2.0 unx      225 b- defN 23-May-19 16:11 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-May-25 19:10 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-May-26 11:38 dwiqc/__version__.py
 -rw-r--r--  2.0 unx      283 b- defN 23-May-25 14:54 dwiqc/browser/__init__.py
 -rw-r--r--  2.0 unx       62 b- defN 23-May-19 16:11 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6651 b- defN 23-May-25 14:45 dwiqc/cli/get.py
 -rw-r--r--  2.0 unx     5805 b- defN 23-May-25 14:56 dwiqc/cli/process.py
 -rw-r--r--  2.0 unx      160 b- defN 23-May-19 16:11 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-May-19 16:11 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-May-19 16:11 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-May-19 16:11 dwiqc/tasks/__init__.py
 -rw-r--r--  2.0 unx     8664 b- defN 23-May-23 14:22 dwiqc/tasks/prequal.py
 -rw-r--r--  2.0 unx     4209 b- defN 23-May-22 17:12 dwiqc/tasks/prequal_EQ.py
 -rw-r--r--  2.0 unx     6193 b- defN 23-May-23 11:24 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3782 b- defN 23-May-19 16:11 dwiqc/tasks/qsiprep_EQ.py
--rw-r--r--  2.0 unx    14029 b- defN 23-May-25 14:46 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     3889 b- defN 23-May-25 19:12 dwiqc-0.2.0.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-May-25 19:12 dwiqc-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      457 b- defN 23-May-25 19:12 dwiqc-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-25 19:12 dwiqc-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-25 19:12 dwiqc-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1640 b- defN 23-May-25 19:12 dwiqc-0.2.0.dist-info/RECORD
-21 files, 60217 bytes uncompressed, 19829 bytes compressed:  67.1%
+-rw-r--r--  2.0 unx    16212 b- defN 23-May-26 11:38 dwiqc/xnat/__init__.py
+-rwxr-xr-x  2.0 unx     3889 b- defN 23-May-26 11:42 dwiqc-0.2.1.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-May-26 11:42 dwiqc-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      457 b- defN 23-May-26 11:42 dwiqc-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-26 11:42 dwiqc-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-26 11:42 dwiqc-0.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1640 b- defN 23-May-26 11:42 dwiqc-0.2.1.dist-info/RECORD
+21 files, 62400 bytes uncompressed, 20016 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -39,26 +39,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.2.0.data/scripts/dwiQC.py
+Filename: dwiqc-0.2.1.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.2.0.dist-info/LICENSE
+Filename: dwiqc-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.2.0.dist-info/METADATA
+Filename: dwiqc-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.2.0.dist-info/WHEEL
+Filename: dwiqc-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.2.0.dist-info/top_level.txt
+Filename: dwiqc-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.2.0.dist-info/RECORD
+Filename: dwiqc-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/xnat/__init__.py

```diff
@@ -131,14 +131,18 @@
                 'source': os.path.join(self.dirs['prequal'], 'OUTPUTS', 'EDDY', 'eddy_results.qc', 'avg_b3000.png'),
                 'dest': os.path.join('b3000_avg', '{0}_preprocessed_b3000.png'.format(aid))
             },
             {
                 'source': os.path.join(self.dirs['prequal'], 'OUTPUTS', 'EDDY', 'eddy_results.qc', 'qc.pdf'),
                 'dest': os.path.join('eddy_pdf', '{0}_eddy_quad_qc.pdf'.format(aid))
             },
+            {
+                'source': os.path.join(self.dirs['prequal'], 'OUTPUTS', 'EDDY', 'motion_plot.png'),
+                'dest': os.path.join('motion-plot', '{0}_motion_plot.png'.format(aid))
+            },
 
             # pull images from prequal output
             {
                 'source': os.path.join(self.dirs['prequal'], 'OUTPUTS', 'PDF', 'png', 'FA.png'),
                 'dest': os.path.join('FA_map', '{0}_FA.png'.format(aid))
             },
             {
@@ -165,28 +169,52 @@
                 'source': os.path.join(self.dirs['prequal'], 'OUTPUTS', 'PDF', 'dtiQA.pdf'),
                 'dest': os.path.join('prequal_pdf', '{0}_prequal_qc.pdf'.format(aid))
             },
 
             # pull files from qsiprep output
 
             {
-                'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  'qsiprep.pdf'),
-                'dest': os.path.join('qsiprep-pdf', '{0}_qsiprep.pdf'.format(aid))
-            },
-            {
                 'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub + '.html'),
                 'dest': os.path.join('qsiprep-html', '{0}_qsiprep.html'.format(aid))
             },
             {
                 'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub, 'figures', self.sub + '_ses-' + self.ses + '_run-' + self.run + '_carpetplot.svg'),
                 'dest': os.path.join('carpet-plot', '{0}_carpetplot.svg'.format(aid))
             },
             {
                 'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub, 'figures', self.sub + '_t1_2_mni.svg'),
                 'dest': os.path.join('t1-registration', '{0}_t1_registration.svg'.format(aid))
+            },
+            {
+                'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub, 'figures', self.sub + '_seg_brainmask.svg'),
+                'dest': os.path.join('seg-brainmask', '{0}_seg_brainmask.svg'.format(aid))
+            },
+            {
+                'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub, 'figures', self.sub + '_ses-' + self.ses + '_run-' + self.run + '_dwi_denoise_ses_' + self.ses + '_run-' + self.run + '_dwi_wf_denoising.svg'),
+                'dest': os.path.join('denoise', '{0}_denoise.svg'.format(aid))
+            },
+            {
+                'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub, 'figures', self.sub + '_ses-' + self.ses + '_run-' + self.run + '_dwi_denoise_ses_' + self.ses + '_run-' + self.run + '_dwi_wf_biascorr.svg'),
+                'dest': os.path.join('bias-corr', '{0}_bias_correction.svg'.format(aid))
+            },
+            {
+                'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub, 'figures', self.sub + '_ses-' + self.ses + '_run-' + self.run + '_desc-resampled_b0ref.svg'),
+                'dest': os.path.join('b0-ref', '{0}_b0_reference.svg'.format(aid))
+            },
+            {
+                'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub, 'figures', self.sub + '_ses-' + self.ses + '_run-' + self.run + '_sampling_scheme.gif'),
+                'dest': os.path.join('sampling-scheme', '{0}_sampling_scheme.gif'.format(aid))
+            },
+            {
+                'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub, 'figures', self.sub + '_ses-' + self.ses + '_run-' + self.run + '_desc-sdc_b0.svg'),
+                'dest': os.path.join('distortion', '{0}_distortion.svg'.format(aid))
+            },
+            {
+                'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub, 'figures', self.sub + '_ses-' + self.ses + '_run-' + self.run + '_coreg.svg'),
+                'dest': os.path.join('coreg', '{0}_coreg.svg'.format(aid))
             }
         ]
         # start building XML
         xnatns = '{%s}' % ns['xnat']
         etree.SubElement(root, xnatns + 'imageSession_ID').text = DWI_ds['experiment_id']
         etree.SubElement(root, 'PA_fmap_scan_id').text = PA_ds['scan']
         etree.SubElement(root, 'AP_fmap_scan_id').text = AP_ds['scan']
```

## Comparing `dwiqc-0.2.0.data/scripts/dwiQC.py` & `dwiqc-0.2.1.data/scripts/dwiQC.py`

 * *Files identical despite different names*

## Comparing `dwiqc-0.2.0.dist-info/LICENSE` & `dwiqc-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.2.0.dist-info/RECORD` & `dwiqc-0.2.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=1KRq0DVFDxk2iSmDfpBZnQA7Rttv4X1YZA8dflf7aSc,247
+dwiqc/__version__.py,sha256=Sgnrt606IOFHQvDt3B-tbrw3bBwq7FFpW8OP__0X9LE,247
 dwiqc/browser/__init__.py,sha256=MlUOz0v7bA_dtQyXX27WF0dzyGGo4xkEEt2PT2B0_aQ,283
 dwiqc/cli/__init__.py,sha256=zGIm7lrjh3wA191D-VjQBZNjSlspFUx148VwDNQGaTk,62
 dwiqc/cli/get.py,sha256=6ixaBdwEgY_GXh8L-_3QDY4MEsNqSJgXle_mxW99mlk,6651
 dwiqc/cli/process.py,sha256=bRZ4tOIyJM3xLB1XVN5035YdkQRma_1NcZ4nDIxzZMs,5805
 dwiqc/config/__init__.py,sha256=k_w5JzoJN_7R7eI_sIJxHA4FQQHs0_KGf-6jsbG4Xs8,160
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
 dwiqc/tasks/prequal.py,sha256=GagoXzYhHaWV2uEfcadsc-85ij71hxP3YnZDANMO2UY,8664
 dwiqc/tasks/prequal_EQ.py,sha256=PWmlo8u_D5qM1lyXdmT7iq865JL6xoPM0JHGEwzRnes,4209
 dwiqc/tasks/qsiprep.py,sha256=2HAmLSSXyKRUuYmok9EEmoPaSo8_7LoCAU-JGfudeiY,6193
 dwiqc/tasks/qsiprep_EQ.py,sha256=JWildptHsuyJVj7ZYMFlWWYvsAIszJpWk1a0m05JM-Q,3782
-dwiqc/xnat/__init__.py,sha256=oPnIkNNM5Tw7Q677VioA8sSU2_Qa6FH-ckjxTQakFdc,14029
-dwiqc-0.2.0.data/scripts/dwiQC.py,sha256=D6ZRhtwJAl0gYODeWhrT4fl7tZtnul0iXrMRyrHxIfE,3889
-dwiqc-0.2.0.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.2.0.dist-info/METADATA,sha256=W_VJDbRBkOIr85VtRTzuPZEyyX7Gz41enYGWuZn4bW8,457
-dwiqc-0.2.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-dwiqc-0.2.0.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.2.0.dist-info/RECORD,,
+dwiqc/xnat/__init__.py,sha256=4-tJIvDSzSiek-aNwRwvKTQ19_xhEwsF-7ty9czWwec,16212
+dwiqc-0.2.1.data/scripts/dwiQC.py,sha256=D6ZRhtwJAl0gYODeWhrT4fl7tZtnul0iXrMRyrHxIfE,3889
+dwiqc-0.2.1.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.2.1.dist-info/METADATA,sha256=NUBxWlJeEXYsyAnhAmYA9ZDDJJHkcx21VlKIe6TXYqc,457
+dwiqc-0.2.1.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+dwiqc-0.2.1.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.2.1.dist-info/RECORD,,
```

