# Comparing `tmp/tmasque-0.8.3.tar.gz` & `tmp/tmasque-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmasque-0.8.3.tar", last modified: Thu May 18 07:09:21 2023, max compression
+gzip compressed data, was "tmasque-0.8.4.tar", last modified: Fri May 26 01:51:11 2023, max compression
```

## Comparing `tmasque-0.8.3.tar` & `tmasque-0.8.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 07:09:21.075595 tmasque-0.8.3/
--rw-rw-rw-   0        0        0     1063 2023-01-10 22:41:04.000000 tmasque-0.8.3/LICENSE
--rw-rw-rw-   0        0        0    11884 2023-05-18 07:09:21.074588 tmasque-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0    11166 2023-05-18 06:32:24.000000 tmasque-0.8.3/README.md
--rw-rw-rw-   0        0        0     1230 2023-05-18 07:08:27.000000 tmasque-0.8.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-18 07:09:21.075595 tmasque-0.8.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-18 07:09:21.034317 tmasque-0.8.3/tmasque/
--rw-rw-rw-   0        0        0     8318 2023-05-17 06:45:28.000000 tmasque-0.8.3/tmasque/Chromatogram.py
--rw-rw-rw-   0        0        0    33669 2023-01-16 04:22:24.000000 tmasque-0.8.3/tmasque/PeakQualityControl.py
--rw-rw-rw-   0        0        0     8595 2022-11-10 17:12:56.000000 tmasque-0.8.3/tmasque/QualityEncoder.py
--rw-rw-rw-   0        0        0    29607 2022-11-07 04:58:08.000000 tmasque-0.8.3/tmasque/TargetedMSQC.py
--rw-rw-rw-   0        0        0    60247 2023-05-18 06:53:50.000000 tmasque-0.8.3/tmasque/TargetedMSQualityEncoder.py
--rw-rw-rw-   0        0        0      258 2023-05-18 07:09:03.000000 tmasque-0.8.3/tmasque/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 07:09:21.069585 tmasque-0.8.3/tmasque/encoder/
--rw-rw-rw-   0        0        0     8367 2022-11-07 04:58:30.000000 tmasque-0.8.3/tmasque/encoder/quality_encoder_type1.pickle
--rw-rw-rw-   0        0        0    11183 2022-11-07 04:58:28.000000 tmasque-0.8.3/tmasque/encoder/quality_encoder_type2.pickle
--rw-rw-rw-   0        0        0     4100 2022-11-07 04:58:30.000000 tmasque-0.8.3/tmasque/encoder/quality_encoder_type3.pickle
-drwxrwxrwx   0        0        0        0 2023-05-18 07:09:21.072584 tmasque-0.8.3/tmasque/example/
--rw-rw-rw-   0        0        0   870033 2021-10-21 01:06:31.000000 tmasque-0.8.3/tmasque/example/CPTC-EGFR-5_YSSD_2.tsv
--rw-rw-rw-   0        0        0     7139 2021-10-21 01:06:22.000000 tmasque-0.8.3/tmasque/example/PeakBoundaries.csv
--rw-rw-rw-   0        0        0     8557 2023-05-18 06:56:45.000000 tmasque-0.8.3/tmasque/tmasque_runner.py
-drwxrwxrwx   0        0        0        0 2023-05-18 07:09:21.066073 tmasque-0.8.3/tmasque.egg-info/
--rw-rw-rw-   0        0        0    11884 2023-05-18 07:09:20.000000 tmasque-0.8.3/tmasque.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      615 2023-05-18 07:09:21.000000 tmasque-0.8.3/tmasque.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 07:09:20.000000 tmasque-0.8.3/tmasque.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-18 07:09:20.000000 tmasque-0.8.3/tmasque.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       54 2023-05-18 07:09:20.000000 tmasque-0.8.3/tmasque.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 07:09:21.000000 tmasque-0.8.3/tmasque.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 01:51:11.445287 tmasque-0.8.4/
+-rw-rw-rw-   0        0        0     1063 2023-01-10 22:41:04.000000 tmasque-0.8.4/LICENSE
+-rw-rw-rw-   0        0        0    11884 2023-05-26 01:51:11.444288 tmasque-0.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11166 2023-05-18 06:32:24.000000 tmasque-0.8.4/README.md
+-rw-rw-rw-   0        0        0     1230 2023-05-18 07:08:27.000000 tmasque-0.8.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 01:51:11.445287 tmasque-0.8.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 01:51:11.399486 tmasque-0.8.4/tmasque/
+-rw-rw-rw-   0        0        0     8318 2023-05-17 06:45:28.000000 tmasque-0.8.4/tmasque/Chromatogram.py
+-rw-rw-rw-   0        0        0    33665 2023-05-25 07:46:29.000000 tmasque-0.8.4/tmasque/PeakQualityControl.py
+-rw-rw-rw-   0        0        0     8595 2022-11-10 17:12:56.000000 tmasque-0.8.4/tmasque/QualityEncoder.py
+-rw-rw-rw-   0        0        0    29613 2023-05-26 01:15:20.000000 tmasque-0.8.4/tmasque/TargetedMSQC.py
+-rw-rw-rw-   0        0        0    60786 2023-05-26 01:49:46.000000 tmasque-0.8.4/tmasque/TargetedMSQualityEncoder.py
+-rw-rw-rw-   0        0        0      258 2023-05-26 01:48:45.000000 tmasque-0.8.4/tmasque/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 01:51:11.439278 tmasque-0.8.4/tmasque/encoder/
+-rw-rw-rw-   0        0        0     8367 2022-11-07 04:58:30.000000 tmasque-0.8.4/tmasque/encoder/quality_encoder_type1.pickle
+-rw-rw-rw-   0        0        0    11183 2022-11-07 04:58:28.000000 tmasque-0.8.4/tmasque/encoder/quality_encoder_type2.pickle
+-rw-rw-rw-   0        0        0     4100 2022-11-07 04:58:30.000000 tmasque-0.8.4/tmasque/encoder/quality_encoder_type3.pickle
+drwxrwxrwx   0        0        0        0 2023-05-26 01:51:11.442286 tmasque-0.8.4/tmasque/example/
+-rw-rw-rw-   0        0        0   870033 2021-10-21 01:06:31.000000 tmasque-0.8.4/tmasque/example/CPTC-EGFR-5_YSSD_2.tsv
+-rw-rw-rw-   0        0        0     7139 2021-10-21 01:06:22.000000 tmasque-0.8.4/tmasque/example/PeakBoundaries.csv
+-rw-rw-rw-   0        0        0     8557 2023-05-18 06:56:45.000000 tmasque-0.8.4/tmasque/tmasque_runner.py
+drwxrwxrwx   0        0        0        0 2023-05-26 01:51:11.435759 tmasque-0.8.4/tmasque.egg-info/
+-rw-rw-rw-   0        0        0    11884 2023-05-26 01:51:11.000000 tmasque-0.8.4/tmasque.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2023-05-26 01:51:11.000000 tmasque-0.8.4/tmasque.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 01:51:11.000000 tmasque-0.8.4/tmasque.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-26 01:51:11.000000 tmasque-0.8.4/tmasque.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       54 2023-05-26 01:51:11.000000 tmasque-0.8.4/tmasque.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 01:51:11.000000 tmasque-0.8.4/tmasque.egg-info/top_level.txt
```

### Comparing `tmasque-0.8.3/LICENSE` & `tmasque-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tmasque-0.8.3/PKG-INFO` & `tmasque-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmasque
-Version: 0.8.3
+Version: 0.8.4
 Summary: This targeted mass spectrometry quality encoder (tmasque) evaluates peak quality systematically for targeted mass spectrometry.
 Author-email: Chi Yang <chiyang@mail.cgu.edu.tw>
 License: MIT License
 Project-URL: Homepage, https://github.com/ChiYang/tmasque
 Project-URL: Repository, https://github.com/ChiYang/tmasque
 Project-URL: Bug Tracker, https://github.com/ChiYang/tmasque/issues
 Requires-Python: >=3.8
```

### Comparing `tmasque-0.8.3/README.md` & `tmasque-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `tmasque-0.8.3/pyproject.toml` & `tmasque-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tmasque-0.8.3/tmasque/Chromatogram.py` & `tmasque-0.8.4/tmasque/Chromatogram.py`

 * *Files identical despite different names*

### Comparing `tmasque-0.8.3/tmasque/PeakQualityControl.py` & `tmasque-0.8.4/tmasque/PeakQualityControl.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
   def _saveQualityMetrics(self, fn, ps, level, qualityMetricValues, isotope, transition):
     if fn not in self.quality_indexes:
       self.quality_indexes[fn] = dict()
     if ps not in self.quality_indexes[fn]:
       self.quality_indexes[fn][ps] = dict()
     if level not in self.quality_indexes[fn][ps]:
-      self.quality_indexes[fn][ps][level] = dict()    
+      self.quality_indexes[fn][ps][level] = dict()
     if level == 'transition_level':
       if isotope not in self.quality_indexes[fn][ps][level]:
         self.quality_indexes[fn][ps][level][isotope] = dict()
       self.quality_indexes[fn][ps]['transition_level'][isotope][transition] = qualityMetricValues
     elif level == 'transition_pair_level':
       self.quality_indexes[fn][ps]['transition_pair_level'][transition] = qualityMetricValues
     elif level == 'isotope_level':
```

### Comparing `tmasque-0.8.3/tmasque/QualityEncoder.py` & `tmasque-0.8.4/tmasque/QualityEncoder.py`

 * *Files identical despite different names*

### Comparing `tmasque-0.8.3/tmasque/TargetedMSQC.py` & `tmasque-0.8.4/tmasque/TargetedMSQC.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,15 +505,15 @@
     else:
       corr = np.corrcoef(Area2SumRatio[light_col].loc[0], Area2SumRatio[heavy_col].loc[0])[0][1]
     if np.isnan(corr):
       return 0
     else:
       return corr
 
-  def _calculatePairRatioConsistency(self, chromatogram_data): #4(sum補0) #Level 1
+  def calculateEachPairRatioConsistency(self, chromatogram_data): #4(sum補0) #Level 1
     Area2SumRatio = chromatogram_data['Area2SumRatio']
     cols = list(set(['.'.join(i.split('.')[:-1]) for i in Area2SumRatio.columns]))
     PairRatioConsistency = []
     for c in cols:
       if Area2SumRatio[c+'.heavy'][0] == 0:
         PairRatioConsistency.append(5)
       else:
@@ -526,15 +526,15 @@
 
   def calculatePairRatioConsistency(self, chrom_data_list):
     rownames = []
     PairRatioConsistency = pd.DataFrame([])
     for chrom_data in chrom_data_list:
       if chrom_data is None:
         continue
-      PairRatioConsistency = pd.concat([PairRatioConsistency, self._calculatePairRatioConsistency(chrom_data)])
+      PairRatioConsistency = pd.concat([PairRatioConsistency, self.calculateEachPairRatioConsistency(chrom_data)])
       rownames.append(chrom_data['fileName'])
     PairRatioConsistency.index = rownames
     return PairRatioConsistency
 
 
   def calculateMeanIsotopeRatioConsistency(self, chrom_data_list): #8(sum補0) #Level 3, each File has its own value
     rownames = []
```

### Comparing `tmasque-0.8.3/tmasque/TargetedMSQualityEncoder.py` & `tmasque-0.8.4/tmasque/TargetedMSQualityEncoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   page_items = options['page_items']
   score_tables = options['score_tables']
   nrow = options['nrow']
   ncol = options['ncol']
   plt.rcParams['figure.dpi'] = options['dpi']
   plt.rcParams['figure.figsize'] = (options['fig_w'], options['fig_h'])
   plt.rcParams.update({'font.size': 10})
-  
+  switchLightHeavy = True if options['switchLightHeavy'] else False
   fig, axs = plt.subplots(nrow*2, ncol, layout="constrained")
   item_idx = 0
   if page_items[0] is not None:
     if options['mol_separation']:
       fig.suptitle(page_items[0]['peptideModifiedSequence'] + ' (Page ' + str(options['page_num']) + ' of ' + str(options['total_page']) + ')', fontsize=14, fontweight='bold', ha='left', x=0.01)
     else:
       fig.suptitle('Page ' + str(options['page_num']) + ' of ' + str(options['total_page']), fontsize=10, ha='right', x=0.98)
@@ -50,19 +50,19 @@
       fn = chrom_data['fileName']
       ps = chrom_data['peptideModifiedSequence']
       #score_table = pd.DataFrame(self.cache_store[ps][fn]).T
       try:
         score_table = score_tables[ps][fn]
       except:
         score_table = None
-      _sub_chrom_plot(chrom_data, score_table, axs[2*row_idx, col_idx], axs[2*row_idx + 1, col_idx], options = options, mol_separation = options['mol_separation'])
+      _sub_chrom_plot(chrom_data, score_table, axs[2*row_idx, col_idx], axs[2*row_idx + 1, col_idx], options = options, mol_separation = options['mol_separation'], switchLightHeavy=switchLightHeavy)
       item_idx += 1
   return fig
 
-def _sub_chrom_plot(chrom_data, store_table, ax1, ax2, options=None, mol_separation=True):
+def _sub_chrom_plot(chrom_data, store_table, ax1, ax2, options=None, mol_separation=True, switchLightHeavy=False):
   fn = chrom_data['fileName']
   ps = chrom_data['peptideModifiedSequence']
   time = chrom_data['time']
   light_global_max_intensity = chrom_data['intensity'][chrom_data['endogenous_cols']].max().max()
   heavy_global_max_intensity = chrom_data['intensity'][chrom_data['standard_cols']].max().max()
   light_exp = len(str(int(light_global_max_intensity))) - 2
   heavy_exp = len(str(int(heavy_global_max_intensity))) - 2
@@ -96,16 +96,20 @@
     type3_max = options['type3_max']
 
   if light_exp < 0 :
       light_exp = 0
   if heavy_exp < 0:
       heavy_exp = 0
   for fragment in chrom_data['transitions']:
-      ax1.plot(time, [intensity/(10**light_exp) for intensity in chrom_data['intensity'][fragment + '.light']],  linewidth=1, label=fragment + '.light')
-      ax2.plot(time, [intensity/(10**heavy_exp) for intensity in chrom_data['intensity'][fragment + '.heavy']],  linewidth=1, label=fragment + '.heavy')
+      if switchLightHeavy:
+        ax1.plot(time, [intensity/(10**light_exp) for intensity in chrom_data['intensity'][fragment + '.light']],  linewidth=1, label=fragment + '.heavy')
+        ax2.plot(time, [intensity/(10**heavy_exp) for intensity in chrom_data['intensity'][fragment + '.heavy']],  linewidth=1, label=fragment + '.light')
+      else:
+        ax1.plot(time, [intensity/(10**light_exp) for intensity in chrom_data['intensity'][fragment + '.light']],  linewidth=1, label=fragment + '.light')
+        ax2.plot(time, [intensity/(10**heavy_exp) for intensity in chrom_data['intensity'][fragment + '.heavy']],  linewidth=1, label=fragment + '.heavy')
       if not mol_separation:
         ax1.set_title(ps + '\n', fontsize=12, fontweight='bold')
       ax1.annotate(fn, xy=(0.5, 1.02), xycoords='axes fraction', ha='center', va='bottom', fontsize=10, fontweight='normal')
       ax1.set_ylabel('Intensity(10^%s)'%light_exp, fontsize=10)
       ax1.set_xlabel('Retention Time', fontsize = 10)
       if chrom_data['start'] is not None:
         ax1.axvline(chrom_data['start'], linestyle= '--', linewidth=1,color='black')
@@ -195,22 +199,23 @@
         ax1.set_facecolor('mistyrose')
         ax2.set_facecolor('mistyrose')
   else:
     ax1.set_facecolor('lightgray')
     ax2.set_facecolor('lightgray')
 
 class TargetedMSQualityEncoder():
-  def __init__(self, chromatogram_tsv, peak_boundary_csv, core_num=20, switchLightHeavy=False, device='auto', summarize_type='meidan'):
+  def __init__(self, chromatogram_tsv, peak_boundary_csv, core_num=20, switchLightHeavy=False, device='auto'):
     self.core_num = core_num
     self.peak_qc = PeakQualityControl(chromatogram_tsv, peak_boundary_csv, core_num=self.core_num, switchLightHeavy=switchLightHeavy)
     self.device = device
     self.cache_store = {}
     self._sample_df = None
     self._transition_df = None
     self.no_boundary_set = dict()
+    self.switchLightHeavy = switchLightHeavy
     self.quality_warn_range_config = dict(
       # Type 1 quality
       TransitionJaggedness_light = dict(min=0, max=0.3, direction=-1),
       TransitionSymmetry_light=dict(min=0, max=1, direction=1),
       TransitionModality_light=dict(min=0, max=0.3, direction=-1),
       TransitionShift_light=dict(min=0, max=0.3, direction=-1),
       TransitionFWHM_light=dict(min=0.05, max=1, direction=-1),
@@ -919,15 +924,15 @@
             score_tables[ps] = dict()
           if ps in self.cache_store and fn in self.cache_store[ps]:
             score_tables[ps][fn] = pd.DataFrame(self.cache_store[ps][fn]).T
           else:
             score_tables[ps][fn] = None
         page_input_options.append({'page_items': page_items, 'nrow': nrow, 'ncol': ncol, 'score_tables': score_tables,
                                     'dpi': dpi, 'fig_w': fig_w, 'fig_h': fig_h, 'page_num': page_idx + 1, 'total_page': total_page,
-                                    'mol_separation': mol_separation, 'type1_min': type1_min, 'type1_max': type1_max, 
+                                    'mol_separation': mol_separation, 'type1_min': type1_min, 'type1_max': type1_max, 'switchLightHeavy': self.switchLightHeavy,
                                     'type2_min':type2_min, 'type2_max': type2_max, 'type3_min': type3_min, 'type3_max': type3_max
                                   })
     print('Generating figures ...')
     page_num = 1
     if threads >= 2:
       pool = Pool(threads)
       figs = pool.map(_chrom_plot_page, page_input_options)
```

### Comparing `tmasque-0.8.3/tmasque/encoder/quality_encoder_type1.pickle` & `tmasque-0.8.4/tmasque/encoder/quality_encoder_type1.pickle`

 * *Files identical despite different names*

### Comparing `tmasque-0.8.3/tmasque/encoder/quality_encoder_type2.pickle` & `tmasque-0.8.4/tmasque/encoder/quality_encoder_type2.pickle`

 * *Files identical despite different names*

### Comparing `tmasque-0.8.3/tmasque/encoder/quality_encoder_type3.pickle` & `tmasque-0.8.4/tmasque/encoder/quality_encoder_type3.pickle`

 * *Files identical despite different names*

### Comparing `tmasque-0.8.3/tmasque/example/CPTC-EGFR-5_YSSD_2.tsv` & `tmasque-0.8.4/tmasque/example/CPTC-EGFR-5_YSSD_2.tsv`

 * *Files identical despite different names*

### Comparing `tmasque-0.8.3/tmasque/example/PeakBoundaries.csv` & `tmasque-0.8.4/tmasque/example/PeakBoundaries.csv`

 * *Files identical despite different names*

### Comparing `tmasque-0.8.3/tmasque/tmasque_runner.py` & `tmasque-0.8.4/tmasque/tmasque_runner.py`

 * *Files identical despite different names*

### Comparing `tmasque-0.8.3/tmasque.egg-info/PKG-INFO` & `tmasque-0.8.4/tmasque.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmasque
-Version: 0.8.3
+Version: 0.8.4
 Summary: This targeted mass spectrometry quality encoder (tmasque) evaluates peak quality systematically for targeted mass spectrometry.
 Author-email: Chi Yang <chiyang@mail.cgu.edu.tw>
 License: MIT License
 Project-URL: Homepage, https://github.com/ChiYang/tmasque
 Project-URL: Repository, https://github.com/ChiYang/tmasque
 Project-URL: Bug Tracker, https://github.com/ChiYang/tmasque/issues
 Requires-Python: >=3.8
```

### Comparing `tmasque-0.8.3/tmasque.egg-info/SOURCES.txt` & `tmasque-0.8.4/tmasque.egg-info/SOURCES.txt`

 * *Files identical despite different names*

