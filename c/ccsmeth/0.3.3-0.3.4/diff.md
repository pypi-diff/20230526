# Comparing `tmp/ccsmeth-0.3.3.tar.gz` & `tmp/ccsmeth-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccsmeth-0.3.3.tar", last modified: Mon May 15 11:32:43 2023, max compression
+gzip compressed data, was "ccsmeth-0.3.4.tar", last modified: Fri May 26 03:04:43 2023, max compression
```

## Comparing `ccsmeth-0.3.3.tar` & `ccsmeth-0.3.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 11:32:43.705074 ccsmeth-0.3.3/
--rw-rw-rw-   0        0        0     1683 2023-03-22 03:41:13.000000 ccsmeth-0.3.3/LICENSE
--rw-rw-rw-   0        0        0       84 2023-03-22 03:41:13.000000 ccsmeth-0.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2219 2023-05-15 11:32:43.705074 ccsmeth-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     1418 2023-05-10 16:47:48.000000 ccsmeth-0.3.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-15 11:32:43.481213 ccsmeth-0.3.3/ccsmeth/
--rw-rw-rw-   0        0        0        0 2022-05-16 12:12:40.000000 ccsmeth-0.3.3/ccsmeth/__init__.py
--rw-rw-rw-   0        0        0    15200 2023-03-22 03:41:13.000000 ccsmeth-0.3.3/ccsmeth/_bam2modbam.py
--rw-rw-rw-   0        0        0       18 2023-05-15 09:50:50.000000 ccsmeth-0.3.3/ccsmeth/_version.py
--rw-rw-rw-   0        0        0     9878 2023-03-22 03:41:13.000000 ccsmeth-0.3.3/ccsmeth/align_hifi_reads.py
--rw-rw-rw-   0        0        0     6040 2023-03-22 03:41:13.000000 ccsmeth-0.3.3/ccsmeth/call_hifi_reads.py
--rw-rw-rw-   0        0        0    30718 2023-05-09 07:02:54.000000 ccsmeth-0.3.3/ccsmeth/call_modifications.py
--rw-rw-rw-   0        0        0    37939 2023-05-09 07:03:05.000000 ccsmeth-0.3.3/ccsmeth/call_mods_freq_bam.py
--rw-rw-rw-   0        0        0    18444 2023-03-22 03:41:14.000000 ccsmeth-0.3.3/ccsmeth/call_mods_freq_txt.py
--rw-rw-rw-   0        0        0    54823 2023-05-09 07:02:13.000000 ccsmeth-0.3.3/ccsmeth/ccsmeth.py
--rw-rw-rw-   0        0        0     6908 2023-03-22 03:41:14.000000 ccsmeth-0.3.3/ccsmeth/dataloader.py
--rw-rw-rw-   0        0        0    31829 2023-05-09 07:02:43.000000 ccsmeth-0.3.3/ccsmeth/extract_features.py
--rw-rw-rw-   0        0        0    10097 2023-04-26 02:27:23.000000 ccsmeth-0.3.3/ccsmeth/models.py
--rw-rw-rw-   0        0        0    20305 2023-03-22 03:41:14.000000 ccsmeth-0.3.3/ccsmeth/train.py
--rw-rw-rw-   0        0        0    25193 2023-04-23 13:09:00.000000 ccsmeth-0.3.3/ccsmeth/train_multigpu.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:32:43.690083 ccsmeth-0.3.3/ccsmeth/utils/
--rw-rw-rw-   0        0        0        0 2022-05-21 04:53:39.000000 ccsmeth-0.3.3/ccsmeth/utils/__init__.py
--rw-rw-rw-   0        0        0     2801 2023-03-22 03:41:14.000000 ccsmeth-0.3.3/ccsmeth/utils/attention.py
--rw-rw-rw-   0        0        0      756 2023-03-22 03:41:14.000000 ccsmeth-0.3.3/ccsmeth/utils/constants_torch.py
--rw-rw-rw-   0        0        0     4077 2023-03-22 03:41:14.000000 ccsmeth-0.3.3/ccsmeth/utils/lookahead.py
--rw-rw-rw-   0        0        0    13974 2023-03-22 03:41:15.000000 ccsmeth-0.3.3/ccsmeth/utils/process_utils.py
--rw-rw-rw-   0        0        0     9051 2022-05-16 12:12:41.000000 ccsmeth-0.3.3/ccsmeth/utils/ranger2020.py
--rw-rw-rw-   0        0        0     2789 2022-05-16 12:12:41.000000 ccsmeth-0.3.3/ccsmeth/utils/ref_reader.py
--rw-rw-rw-   0        0        0      963 2023-03-22 03:41:15.000000 ccsmeth-0.3.3/ccsmeth/utils/sam2fastq_std.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:32:43.592144 ccsmeth-0.3.3/ccsmeth.egg-info/
--rw-rw-rw-   0        0        0     2219 2023-05-15 11:32:42.000000 ccsmeth-0.3.3/ccsmeth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      853 2023-05-15 11:32:43.000000 ccsmeth-0.3.3/ccsmeth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 11:32:42.000000 ccsmeth-0.3.3/ccsmeth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-15 11:32:42.000000 ccsmeth-0.3.3/ccsmeth.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 11:32:42.000000 ccsmeth-0.3.3/ccsmeth.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      134 2023-05-15 11:32:42.000000 ccsmeth-0.3.3/ccsmeth.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-15 11:32:42.000000 ccsmeth-0.3.3/ccsmeth.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      152 2023-03-22 03:41:16.000000 ccsmeth-0.3.3/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-05-15 11:32:43.718069 ccsmeth-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     2017 2023-03-22 03:41:17.000000 ccsmeth-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 03:04:43.336925 ccsmeth-0.3.4/
+-rw-rw-rw-   0        0        0     1683 2023-03-22 03:41:13.000000 ccsmeth-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0       84 2023-03-22 03:41:13.000000 ccsmeth-0.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2319 2023-05-26 03:04:43.336925 ccsmeth-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1513 2023-05-26 02:48:04.000000 ccsmeth-0.3.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-26 03:04:43.187017 ccsmeth-0.3.4/ccsmeth/
+-rw-rw-rw-   0        0        0        0 2022-05-16 12:12:40.000000 ccsmeth-0.3.4/ccsmeth/__init__.py
+-rw-rw-rw-   0        0        0    15200 2023-03-22 03:41:13.000000 ccsmeth-0.3.4/ccsmeth/_bam2modbam.py
+-rw-rw-rw-   0        0        0       18 2023-05-26 03:01:01.000000 ccsmeth-0.3.4/ccsmeth/_version.py
+-rw-rw-rw-   0        0        0     9878 2023-03-22 03:41:13.000000 ccsmeth-0.3.4/ccsmeth/align_hifi_reads.py
+-rw-rw-rw-   0        0        0     6040 2023-03-22 03:41:13.000000 ccsmeth-0.3.4/ccsmeth/call_hifi_reads.py
+-rw-rw-rw-   0        0        0    30718 2023-05-09 07:02:54.000000 ccsmeth-0.3.4/ccsmeth/call_modifications.py
+-rw-rw-rw-   0        0        0    37939 2023-05-09 07:03:05.000000 ccsmeth-0.3.4/ccsmeth/call_mods_freq_bam.py
+-rw-rw-rw-   0        0        0    18444 2023-03-22 03:41:14.000000 ccsmeth-0.3.4/ccsmeth/call_mods_freq_txt.py
+-rw-rw-rw-   0        0        0    54823 2023-05-09 07:02:13.000000 ccsmeth-0.3.4/ccsmeth/ccsmeth.py
+-rw-rw-rw-   0        0        0     6872 2023-05-26 02:33:38.000000 ccsmeth-0.3.4/ccsmeth/dataloader.py
+-rw-rw-rw-   0        0        0    31796 2023-05-26 02:33:21.000000 ccsmeth-0.3.4/ccsmeth/extract_features.py
+-rw-rw-rw-   0        0        0    10097 2023-04-26 02:27:23.000000 ccsmeth-0.3.4/ccsmeth/models.py
+-rw-rw-rw-   0        0        0    20305 2023-03-22 03:41:14.000000 ccsmeth-0.3.4/ccsmeth/train.py
+-rw-rw-rw-   0        0        0    25193 2023-04-23 13:09:00.000000 ccsmeth-0.3.4/ccsmeth/train_multigpu.py
+drwxrwxrwx   0        0        0        0 2023-05-26 03:04:43.329932 ccsmeth-0.3.4/ccsmeth/utils/
+-rw-rw-rw-   0        0        0        0 2022-05-21 04:53:39.000000 ccsmeth-0.3.4/ccsmeth/utils/__init__.py
+-rw-rw-rw-   0        0        0     2801 2023-03-22 03:41:14.000000 ccsmeth-0.3.4/ccsmeth/utils/attention.py
+-rw-rw-rw-   0        0        0      756 2023-03-22 03:41:14.000000 ccsmeth-0.3.4/ccsmeth/utils/constants_torch.py
+-rw-rw-rw-   0        0        0     4077 2023-03-22 03:41:14.000000 ccsmeth-0.3.4/ccsmeth/utils/lookahead.py
+-rw-rw-rw-   0        0        0    13974 2023-03-22 03:41:15.000000 ccsmeth-0.3.4/ccsmeth/utils/process_utils.py
+-rw-rw-rw-   0        0        0     9051 2022-05-16 12:12:41.000000 ccsmeth-0.3.4/ccsmeth/utils/ranger2020.py
+-rw-rw-rw-   0        0        0     2789 2022-05-16 12:12:41.000000 ccsmeth-0.3.4/ccsmeth/utils/ref_reader.py
+-rw-rw-rw-   0        0        0      963 2023-03-22 03:41:15.000000 ccsmeth-0.3.4/ccsmeth/utils/sam2fastq_std.py
+drwxrwxrwx   0        0        0        0 2023-05-26 03:04:43.252976 ccsmeth-0.3.4/ccsmeth.egg-info/
+-rw-rw-rw-   0        0        0     2319 2023-05-26 03:04:41.000000 ccsmeth-0.3.4/ccsmeth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2023-05-26 03:04:41.000000 ccsmeth-0.3.4/ccsmeth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 03:04:41.000000 ccsmeth-0.3.4/ccsmeth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-26 03:04:41.000000 ccsmeth-0.3.4/ccsmeth.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 11:32:42.000000 ccsmeth-0.3.4/ccsmeth.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      134 2023-05-26 03:04:41.000000 ccsmeth-0.3.4/ccsmeth.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 03:04:41.000000 ccsmeth-0.3.4/ccsmeth.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      152 2023-03-22 03:41:16.000000 ccsmeth-0.3.4/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-05-26 03:04:43.344920 ccsmeth-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     2017 2023-03-22 03:41:17.000000 ccsmeth-0.3.4/setup.py
```

### Comparing `ccsmeth-0.3.3/LICENSE` & `ccsmeth-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/PKG-INFO` & `ccsmeth-0.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ccsmeth
-Version: 0.3.3
+Version: 0.3.4
 Summary: Detecting DNA methylation from PacBio CCS reads
 Home-page: https://github.com/PengNi/ccsmeth
-Download-URL: https://github.com/PengNi/ccsmeth/archive/refs/tags/0.3.3.tar.gz
+Download-URL: https://github.com/PengNi/ccsmeth/archive/refs/tags/0.3.4.tar.gz
 Author: Peng Ni
 Author-email: 543943952@qq.com
 License: BSD-3-Clause-Clear license
 Keywords: methylation,pacbio,neural network
 Platform: Linux
 Platform: MacOS
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,19 @@
 
 ccsmeth
 ========
 
 
 Documentation
 -------------
+v0.3.4
+----------
+replace 'numpy.float' by 'float" in extract_features and call_mods modules
+
+
 v0.3.3
 ----------
 more robust operation for MM/ML tags
 
 update the call_mods model (v1 to v2), use shared params for both rnn and attention
 
 update aggregate model (v2 to v2p)
```

### Comparing `ccsmeth-0.3.3/README.rst` & `ccsmeth-0.3.4/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 ccsmeth
 ========
 
 
 Documentation
 -------------
+v0.3.4
+----------
+replace 'numpy.float' by 'float" in extract_features and call_mods modules
+
+
 v0.3.3
 ----------
 more robust operation for MM/ML tags
 
 update the call_mods model (v1 to v2), use shared params for both rnn and attention
 
 update aggregate model (v2 to v2p)
```

### Comparing `ccsmeth-0.3.3/ccsmeth/_bam2modbam.py` & `ccsmeth-0.3.4/ccsmeth/_bam2modbam.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth/align_hifi_reads.py` & `ccsmeth-0.3.4/ccsmeth/align_hifi_reads.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth/call_hifi_reads.py` & `ccsmeth-0.3.4/ccsmeth/call_hifi_reads.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth/call_modifications.py` & `ccsmeth-0.3.4/ccsmeth/call_modifications.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth/call_mods_freq_bam.py` & `ccsmeth-0.3.4/ccsmeth/call_mods_freq_bam.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth/call_mods_freq_txt.py` & `ccsmeth-0.3.4/ccsmeth/call_mods_freq_txt.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth/ccsmeth.py` & `ccsmeth-0.3.4/ccsmeth/ccsmeth.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth/dataloader.py` & `ccsmeth-0.3.4/ccsmeth/dataloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,29 +21,29 @@
     #     methy_label
     words = line.strip().split("\t")
 
     sampleinfo = "\t".join(words[0:5])
 
     fkmer = np.array([base2code_dna[x] for x in words[5]])
     fpass = np.array([int(words[6])] * len(fkmer))
-    fipdm = np.array([float(x) for x in words[7].split(",")], dtype=np.float)
-    fipdsd = np.array([float(x) for x in words[8].split(",")], dtype=np.float) if words[8] != "." else 0
-    fpwm = np.array([float(x) for x in words[9].split(",")], dtype=np.float)
-    fpwsd = np.array([float(x) for x in words[10].split(",")], dtype=np.float) if words[10] != "." else 0
-    fqual = np.array([float(x) for x in words[11].split(",")], dtype=np.float)
-    fmap = np.array([float(x) for x in words[12].split(",")], dtype=np.float) if words[12] != "." else 0
+    fipdm = np.array([float(x) for x in words[7].split(",")], dtype=float)
+    fipdsd = np.array([float(x) for x in words[8].split(",")], dtype=float) if words[8] != "." else 0
+    fpwm = np.array([float(x) for x in words[9].split(",")], dtype=float)
+    fpwsd = np.array([float(x) for x in words[10].split(",")], dtype=float) if words[10] != "." else 0
+    fqual = np.array([float(x) for x in words[11].split(",")], dtype=float)
+    fmap = np.array([float(x) for x in words[12].split(",")], dtype=float) if words[12] != "." else 0
 
     rkmer = np.array([base2code_dna[x] for x in words[13]])
     rpass = np.array([int(words[14])] * len(rkmer))
-    ripdm = np.array([float(x) for x in words[15].split(",")], dtype=np.float)
-    ripdsd = np.array([float(x) for x in words[16].split(",")], dtype=np.float) if words[16] != "." else 0
-    rpwm = np.array([float(x) for x in words[17].split(",")], dtype=np.float)
-    rpwsd = np.array([float(x) for x in words[18].split(",")], dtype=np.float) if words[18] != "." else 0
-    rqual = np.array([float(x) for x in words[19].split(",")], dtype=np.float)
-    rmap = np.array([float(x) for x in words[20].split(",")], dtype=np.float) if words[20] != "." else 0
+    ripdm = np.array([float(x) for x in words[15].split(",")], dtype=float)
+    ripdsd = np.array([float(x) for x in words[16].split(",")], dtype=float) if words[16] != "." else 0
+    rpwm = np.array([float(x) for x in words[17].split(",")], dtype=float)
+    rpwsd = np.array([float(x) for x in words[18].split(",")], dtype=float) if words[18] != "." else 0
+    rqual = np.array([float(x) for x in words[19].split(",")], dtype=float)
+    rmap = np.array([float(x) for x in words[20].split(",")], dtype=float) if words[20] != "." else 0
 
     label = int(words[21])
 
     return sampleinfo, fkmer, fpass, fipdm, fipdsd, fpwm, fpwsd, fqual, fmap, \
         rkmer, rpass, ripdm, ripdsd, rpwm, rpwsd, rqual, rmap, label
```

### Comparing `ccsmeth-0.3.3/ccsmeth/extract_features.py` & `ccsmeth-0.3.4/ccsmeth/extract_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
     if normalize_method == 'zscore':
         sshift, sscale = np.mean(signals), np.std(signals)
     elif normalize_method == 'min-max':
         sshift, sscale = np.min(signals), np.max(signals) - np.min(signals)
     elif normalize_method == 'min-mean':
         sshift, sscale = np.min(signals), np.mean(signals)
     elif normalize_method == 'mad':
-        sshift, sscale = np.median(signals), np.float(robust.mad(signals))
+        sshift, sscale = np.median(signals), float(robust.scale.mad(signals))
     else:
         raise ValueError("")
     if sscale == 0.0:
         norm_signals = [0.] * len(signals)
     else:
         norm_signals = (signals - sshift) / sscale
     return np.around(norm_signals, decimals=6)
@@ -473,29 +473,29 @@
             kmer_seq2, kmer_pass2, kmer_ipdm2, kmer_ipds2, kmer_pwm2, kmer_pws2, kmer_qual2, kmer_map2, \
             label = featureline
 
         sampleinfo.append("\t".join(list(map(str, [chrom, abs_loc, strand, holeid, loc]))))
 
         fkmers.append(np.array([base2code_dna[x] for x in kmer_seq]))
         fpasss.append(np.array([kmer_pass] * len(kmer_seq)))
-        fipdms.append(np.array(kmer_ipdm, dtype=np.float))
-        fipdsds.append(np.array(kmer_ipds, dtype=np.float) if type(kmer_ipds) is not str else 0)
-        fpwms.append(np.array(kmer_pwm, dtype=np.float))
-        fpwsds.append(np.array(kmer_pws, dtype=np.float) if type(kmer_pws) is not str else 0)
-        fquals.append(np.array(kmer_qual, dtype=np.float))
-        fmaps.append(np.array(kmer_map, dtype=np.float) if type(kmer_map) is not str else 0)
+        fipdms.append(np.array(kmer_ipdm, dtype=float))
+        fipdsds.append(np.array(kmer_ipds, dtype=float) if type(kmer_ipds) is not str else 0)
+        fpwms.append(np.array(kmer_pwm, dtype=float))
+        fpwsds.append(np.array(kmer_pws, dtype=float) if type(kmer_pws) is not str else 0)
+        fquals.append(np.array(kmer_qual, dtype=float))
+        fmaps.append(np.array(kmer_map, dtype=float) if type(kmer_map) is not str else 0)
 
         rkmers.append(np.array([base2code_dna[x] for x in kmer_seq2]))
         rpasss.append(np.array([kmer_pass2] * len(kmer_seq2)))
-        ripdms.append(np.array(kmer_ipdm2, dtype=np.float))
-        ripdsds.append(np.array(kmer_ipds2, dtype=np.float) if type(kmer_ipds2) is not str else 0)
-        rpwms.append(np.array(kmer_pwm2, dtype=np.float))
-        rpwsds.append(np.array(kmer_pws2, dtype=np.float) if type(kmer_pws2) is not str else 0)
-        rquals.append(np.array(kmer_qual2, dtype=np.float))
-        rmaps.append(np.array(kmer_map2, dtype=np.float) if type(kmer_map2) is not str else 0)
+        ripdms.append(np.array(kmer_ipdm2, dtype=float))
+        ripdsds.append(np.array(kmer_ipds2, dtype=float) if type(kmer_ipds2) is not str else 0)
+        rpwms.append(np.array(kmer_pwm2, dtype=float))
+        rpwsds.append(np.array(kmer_pws2, dtype=float) if type(kmer_pws2) is not str else 0)
+        rquals.append(np.array(kmer_qual2, dtype=float))
+        rmaps.append(np.array(kmer_map2, dtype=float) if type(kmer_map2) is not str else 0)
 
         labels.append(label)
     return sampleinfo, fkmers, fpasss, fipdms, fipdsds, fpwms, fpwsds, fquals, fmaps, \
         rkmers, rpasss, ripdms, ripdsds, rpwms, rpwsds, rquals, rmaps, labels
 
 
 def worker_extract_features_from_holebatches(holebatch_q, features_q,
```

### Comparing `ccsmeth-0.3.3/ccsmeth/models.py` & `ccsmeth-0.3.4/ccsmeth/models.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth/train.py` & `ccsmeth-0.3.4/ccsmeth/train.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth/train_multigpu.py` & `ccsmeth-0.3.4/ccsmeth/train_multigpu.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth/utils/attention.py` & `ccsmeth-0.3.4/ccsmeth/utils/attention.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth/utils/constants_torch.py` & `ccsmeth-0.3.4/ccsmeth/utils/constants_torch.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth/utils/lookahead.py` & `ccsmeth-0.3.4/ccsmeth/utils/lookahead.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth/utils/process_utils.py` & `ccsmeth-0.3.4/ccsmeth/utils/process_utils.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth/utils/ranger2020.py` & `ccsmeth-0.3.4/ccsmeth/utils/ranger2020.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth/utils/ref_reader.py` & `ccsmeth-0.3.4/ccsmeth/utils/ref_reader.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth/utils/sam2fastq_std.py` & `ccsmeth-0.3.4/ccsmeth/utils/sam2fastq_std.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/ccsmeth.egg-info/PKG-INFO` & `ccsmeth-0.3.4/ccsmeth.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ccsmeth
-Version: 0.3.3
+Version: 0.3.4
 Summary: Detecting DNA methylation from PacBio CCS reads
 Home-page: https://github.com/PengNi/ccsmeth
-Download-URL: https://github.com/PengNi/ccsmeth/archive/refs/tags/0.3.3.tar.gz
+Download-URL: https://github.com/PengNi/ccsmeth/archive/refs/tags/0.3.4.tar.gz
 Author: Peng Ni
 Author-email: 543943952@qq.com
 License: BSD-3-Clause-Clear license
 Keywords: methylation,pacbio,neural network
 Platform: Linux
 Platform: MacOS
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,19 @@
 
 ccsmeth
 ========
 
 
 Documentation
 -------------
+v0.3.4
+----------
+replace 'numpy.float' by 'float" in extract_features and call_mods modules
+
+
 v0.3.3
 ----------
 more robust operation for MM/ML tags
 
 update the call_mods model (v1 to v2), use shared params for both rnn and attention
 
 update aggregate model (v2 to v2p)
```

### Comparing `ccsmeth-0.3.3/ccsmeth.egg-info/SOURCES.txt` & `ccsmeth-0.3.4/ccsmeth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.3/setup.py` & `ccsmeth-0.3.4/setup.py`

 * *Files identical despite different names*

