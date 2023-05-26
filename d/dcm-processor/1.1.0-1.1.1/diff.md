# Comparing `tmp/dcm-processor-1.1.0.tar.gz` & `tmp/dcm-processor-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcm-processor-1.1.0.tar", last modified: Wed May 17 12:42:37 2023, max compression
+gzip compressed data, was "dcm-processor-1.1.1.tar", last modified: Fri May 26 12:24:31 2023, max compression
```

## Comparing `dcm-processor-1.1.0.tar` & `dcm-processor-1.1.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:37.149464 dcm-processor-1.1.0/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1074 2021-05-11 10:55:48.000000 dcm-processor-1.1.0/LICENSE
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-05-17 12:42:37.150014 dcm-processor-1.1.0/PKG-INFO
--rwxr-xr-x   0 giles     (1000) giles     (1000)     5834 2023-04-17 10:06:58.000000 dcm-processor-1.1.0/README.md
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.720272 dcm-processor-1.1.0/dcm_processor/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       61 2021-10-17 14:30:50.000000 dcm-processor-1.1.0/dcm_processor/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    15407 2023-04-15 09:02:58.000000 dcm-processor-1.1.0/dcm_processor/argparser.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    33214 2023-05-17 11:54:45.000000 dcm-processor-1.1.0/dcm_processor/files.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    46033 2023-04-19 12:36:49.000000 dcm-processor-1.1.0/dcm_processor/script.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.683831 dcm-processor-1.1.0/dcm_processor/services/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.681816 dcm-processor-1.1.0/dcm_processor/services/base/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.758424 dcm-processor-1.1.0/dcm_processor/services/base/module/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.966491 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/
--rwxr-xr-x   0 giles     (1000) giles     (1000)   642195 2021-10-17 16:16:14.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)    17869 2021-10-17 16:16:15.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)      526 2023-04-06 14:13:53.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1590 2023-05-12 10:21:10.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    69564 2021-10-17 16:16:15.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.976669 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/config/
--rwxr-xr-x   0 giles     (1000) giles     (1000)    59797 2023-05-17 12:00:32.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script
--rwxr-xr-x   0 giles     (1000) giles     (1000)      248 2021-10-17 16:16:15.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/config/hash_table.csv
--rwxr-xr-x   0 giles     (1000) giles     (1000)       86 2021-10-17 16:16:15.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/config/psudonyms.csv
--rwxr-xr-x   0 giles     (1000) giles     (1000)    10424 2021-10-17 16:16:15.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   863881 2021-10-17 16:16:16.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)     3471 2023-03-31 12:35:15.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)  1172845 2021-10-17 16:16:18.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   391834 2021-10-17 16:16:19.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)    28241 2021-10-17 16:16:19.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   338969 2021-10-17 16:16:20.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/util.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1777 2023-03-31 20:09:03.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/utils.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)       26 2021-10-17 16:16:20.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/requirements.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       72 2021-10-17 16:16:20.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/script.sh
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.991698 dcm-processor-1.1.0/dcm_processor/services/base/module/storageManager/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/storageManager/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)       95 2023-05-11 22:55:55.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/storageManager/header_codes.json
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6218 2023-01-31 18:15:24.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/storageManager/lib.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    10622 2023-05-11 22:55:44.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/storageManager/main.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:37.014549 dcm-processor-1.1.0/dcm_processor/services/base/module/systemcleaner/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/systemcleaner/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     3908 2023-04-28 08:48:28.000000 dcm-processor-1.1.0/dcm_processor/services/base/module/systemcleaner/main.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:37.019802 dcm-processor-1.1.0/dcm_processor/services/base/registry/
--rwxr-xr-x   0 giles     (1000) giles     (1000)      491 2023-04-28 08:35:17.000000 dcm-processor-1.1.0/dcm_processor/services/base/registry/__init__.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.686497 dcm-processor-1.1.0/dcm_processor/services/dcm2nii/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:37.124060 dcm-processor-1.1.0/dcm_processor/services/dcm2nii/module/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     4030 2023-04-14 14:47:11.000000 dcm-processor-1.1.0/dcm_processor/services/dcm2nii/module/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)  1948128 2023-03-02 19:03:11.000000 dcm-processor-1.1.0/dcm_processor/services/dcm2nii/module/dcm2niix
--rwxr-xr-x   0 giles     (1000) giles     (1000)      406 2023-03-24 20:50:04.000000 dcm-processor-1.1.0/dcm_processor/services/dcm2nii/module/lib.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:37.145108 dcm-processor-1.1.0/dcm_processor/services/dcm2nii/registry/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1013 2023-04-14 12:17:35.000000 dcm-processor-1.1.0/dcm_processor/services/dcm2nii/registry/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)      288 2023-04-18 12:25:35.000000 dcm-processor-1.1.0/dcm_processor/services/dcm2nii/registry/settings.json
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6682 2023-04-21 16:23:38.000000 dcm-processor-1.1.0/dcm_processor/worker.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-17 12:42:36.745532 dcm-processor-1.1.0/dcm_processor.egg-info/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-05-17 12:42:35.000000 dcm-processor-1.1.0/dcm_processor.egg-info/PKG-INFO
--rwxr-xr-x   0 giles     (1000) giles     (1000)     2368 2023-05-17 12:42:36.000000 dcm-processor-1.1.0/dcm_processor.egg-info/SOURCES.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)        1 2023-05-17 12:42:35.000000 dcm-processor-1.1.0/dcm_processor.egg-info/dependency_links.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       53 2023-05-17 12:42:35.000000 dcm-processor-1.1.0/dcm_processor.egg-info/entry_points.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       76 2023-05-17 12:42:35.000000 dcm-processor-1.1.0/dcm_processor.egg-info/requires.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       14 2023-05-17 12:42:35.000000 dcm-processor-1.1.0/dcm_processor.egg-info/top_level.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       89 2021-10-17 14:23:09.000000 dcm-processor-1.1.0/pyproject.toml
--rwxr-xr-x   0 giles     (1000) giles     (1000)      980 2023-05-17 12:42:37.152834 dcm-processor-1.1.0/setup.cfg
--rwxr-xr-x   0 giles     (1000) giles     (1000)      109 2021-10-17 19:37:23.000000 dcm-processor-1.1.0/setup.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-26 12:24:31.723501 dcm-processor-1.1.1/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1074 2021-05-11 10:55:48.000000 dcm-processor-1.1.1/LICENSE
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-05-26 12:24:31.723805 dcm-processor-1.1.1/PKG-INFO
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     5834 2023-04-17 10:06:58.000000 dcm-processor-1.1.1/README.md
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-26 12:24:31.462371 dcm-processor-1.1.1/dcm_processor/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       61 2021-10-17 14:30:50.000000 dcm-processor-1.1.1/dcm_processor/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    15407 2023-05-17 16:40:44.000000 dcm-processor-1.1.1/dcm_processor/argparser.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    33214 2023-05-17 11:54:45.000000 dcm-processor-1.1.1/dcm_processor/files.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    46033 2023-04-19 12:36:49.000000 dcm-processor-1.1.1/dcm_processor/script.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-26 12:24:31.417605 dcm-processor-1.1.1/dcm_processor/services/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-26 12:24:31.416294 dcm-processor-1.1.1/dcm_processor/services/base/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-26 12:24:31.480746 dcm-processor-1.1.1/dcm_processor/services/base/module/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-26 12:24:31.578553 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   642195 2021-10-17 16:16:14.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    17869 2021-10-17 16:16:15.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      526 2023-04-06 14:13:53.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1590 2023-05-12 10:21:10.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    69564 2021-10-17 16:16:15.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-26 12:24:31.594864 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/config/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    59867 2023-05-26 12:21:12.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      248 2021-10-17 16:16:15.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/config/hash_table.csv
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       86 2021-10-17 16:16:15.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/config/psudonyms.csv
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    10424 2021-10-17 16:16:15.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   863881 2021-10-17 16:16:16.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     3479 2023-05-26 10:55:08.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)  1172845 2021-10-17 16:16:18.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   391834 2021-10-17 16:16:19.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    28241 2021-10-17 16:16:19.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   338969 2021-10-17 16:16:20.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/util.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1777 2023-03-31 20:09:03.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/utils.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       26 2021-10-17 16:16:20.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/requirements.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       72 2021-10-17 16:16:20.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/script.sh
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-26 12:24:31.660654 dcm-processor-1.1.1/dcm_processor/services/base/module/storageManager/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/storageManager/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       95 2023-05-11 22:55:55.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/storageManager/header_codes.json
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6218 2023-01-31 18:15:24.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/storageManager/lib.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    10622 2023-05-11 22:55:44.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/storageManager/main.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-26 12:24:31.668830 dcm-processor-1.1.1/dcm_processor/services/base/module/systemcleaner/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/systemcleaner/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     3908 2023-04-28 08:48:28.000000 dcm-processor-1.1.1/dcm_processor/services/base/module/systemcleaner/main.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-26 12:24:31.676817 dcm-processor-1.1.1/dcm_processor/services/base/registry/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      491 2023-04-28 08:35:17.000000 dcm-processor-1.1.1/dcm_processor/services/base/registry/__init__.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-26 12:24:31.419661 dcm-processor-1.1.1/dcm_processor/services/dcm2nii/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-26 12:24:31.718377 dcm-processor-1.1.1/dcm_processor/services/dcm2nii/module/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     4030 2023-04-14 14:47:11.000000 dcm-processor-1.1.1/dcm_processor/services/dcm2nii/module/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)  1948128 2023-03-02 19:03:11.000000 dcm-processor-1.1.1/dcm_processor/services/dcm2nii/module/dcm2niix
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      406 2023-03-24 20:50:04.000000 dcm-processor-1.1.1/dcm_processor/services/dcm2nii/module/lib.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-26 12:24:31.722356 dcm-processor-1.1.1/dcm_processor/services/dcm2nii/registry/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1013 2023-04-14 12:17:35.000000 dcm-processor-1.1.1/dcm_processor/services/dcm2nii/registry/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      288 2023-04-18 12:25:35.000000 dcm-processor-1.1.1/dcm_processor/services/dcm2nii/registry/settings.json
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6682 2023-04-21 16:23:38.000000 dcm-processor-1.1.1/dcm_processor/worker.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-05-26 12:24:31.475846 dcm-processor-1.1.1/dcm_processor.egg-info/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-05-26 12:24:30.000000 dcm-processor-1.1.1/dcm_processor.egg-info/PKG-INFO
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     2368 2023-05-26 12:24:31.000000 dcm-processor-1.1.1/dcm_processor.egg-info/SOURCES.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)        1 2023-05-26 12:24:30.000000 dcm-processor-1.1.1/dcm_processor.egg-info/dependency_links.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       53 2023-05-26 12:24:30.000000 dcm-processor-1.1.1/dcm_processor.egg-info/entry_points.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       76 2023-05-26 12:24:30.000000 dcm-processor-1.1.1/dcm_processor.egg-info/requires.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       14 2023-05-26 12:24:30.000000 dcm-processor-1.1.1/dcm_processor.egg-info/top_level.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       89 2021-10-17 14:23:09.000000 dcm-processor-1.1.1/pyproject.toml
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      980 2023-05-26 12:24:31.739998 dcm-processor-1.1.1/setup.cfg
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      109 2021-10-17 19:37:23.000000 dcm-processor-1.1.1/setup.py
```

### Comparing `dcm-processor-1.1.0/LICENSE` & `dcm-processor-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/PKG-INFO` & `dcm-processor-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcm-processor
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Command line tool for the dicom processor library
 Home-page: https://github.com/giesekow/dcm-processor-cli
 Author: Giles Tetteh
 Author-email: giles.tetteh@tum.de
 Keywords: orthanc,dicom,worker,processor,translation,medical
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dcm-processor-1.1.0/README.md` & `dcm-processor-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/argparser.py` & `dcm-processor-1.1.1/dcm_processor/argparser.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/files.py` & `dcm-processor-1.1.1/dcm_processor/files.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/script.py` & `dcm-processor-1.1.1/dcm_processor/script.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar` & `dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar` & `dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py` & `dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py` & `dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar` & `dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script` & `dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
  <e en="T" t="00080016" n="SOPClassUID">@keep()</e>
  <e en="T" t="00080018" n="SOPInstanceUID">@hashuid(@UIDROOT,this)</e>
  <e en="T" t="00080020" n="StudyDate">@keep()</e>
  <e en="T" t="00080021" n="SeriesDate">@modifydate(this,*,*,1)</e>
  <e en="T" t="00080022" n="AcquisitionDate">@modifydate(this,*,*,1)</e>
  <e en="T" t="00080023" n="ContentDate">@modifydate(this,*,1,1)</e>
  <e en="T" t="00080024" n="OverlayDate">@remove()</e>
+ <e en="T" t="04000561" n="OriginalAttributesSequence">@remove()</e>
  <e en="T" t="00080025" n="CurveDate">@remove()</e>
  <e en="T" t="0008002a" n="AcquisitionDatetime">@modifydate(this,*,1,1)</e>
  <e en="T" t="00080030" n="StudyTime">@remove()</e>
  <e en="T" t="00080031" n="SeriesTime">@keep()</e>
  <e en="T" t="00080032" n="AcquisitionTime">@keep()</e>
  <e en="T" t="00080033" n="ContentTime">@keep()</e>
  <e en="T" t="00080034" n="OverlayTime">@keep()</e>
```

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar` & `dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar` & `dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py` & `dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
   
   interface_url = config_dict.get('interface_url')
   auth_server_url = config_dict.get('auth_server_url')
   client_id = config_dict.get('client_id')
   client_secret = config_dict.get('client_secret')
   identifier_system = config_dict.get('identifier_system')
 
-  if (interface_url is None) or (auth_server_url is None) or (client_id is None) or (client_secret) or (identifier_system is None):
+  if (interface_url is None) or (auth_server_url is None) or (client_id is None) or (client_secret is None) or (identifier_system is None):
     return None
   
   pat_entry = create_fhir_entry("Patient", identifier_system, ptid)
   
   bundle = create_fhir_bundle([pat_entry,])
   
   try:
```

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar` & `dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar` & `dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar` & `dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/util.jar` & `dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/util.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/DicomAnonymizerService/utils.py` & `dcm-processor-1.1.1/dcm_processor/services/base/module/DicomAnonymizerService/utils.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/storageManager/lib.py` & `dcm-processor-1.1.1/dcm_processor/services/base/module/storageManager/lib.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/storageManager/main.py` & `dcm-processor-1.1.1/dcm_processor/services/base/module/storageManager/main.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/base/module/systemcleaner/main.py` & `dcm-processor-1.1.1/dcm_processor/services/base/module/systemcleaner/main.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/dcm2nii/module/__init__.py` & `dcm-processor-1.1.1/dcm_processor/services/dcm2nii/module/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/dcm2nii/module/dcm2niix` & `dcm-processor-1.1.1/dcm_processor/services/dcm2nii/module/dcm2niix`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/services/dcm2nii/registry/__init__.py` & `dcm-processor-1.1.1/dcm_processor/services/dcm2nii/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor/worker.py` & `dcm-processor-1.1.1/dcm_processor/worker.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/dcm_processor.egg-info/PKG-INFO` & `dcm-processor-1.1.1/dcm_processor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcm-processor
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Command line tool for the dicom processor library
 Home-page: https://github.com/giesekow/dcm-processor-cli
 Author: Giles Tetteh
 Author-email: giles.tetteh@tum.de
 Keywords: orthanc,dicom,worker,processor,translation,medical
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dcm-processor-1.1.0/dcm_processor.egg-info/SOURCES.txt` & `dcm-processor-1.1.1/dcm_processor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.0/setup.cfg` & `dcm-processor-1.1.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dcm-processor
-version = 1.1.0
+version = 1.1.1
 author = Giles Tetteh
 author_email = giles.tetteh@tum.de
 description = A Command line tool for the dicom processor library
 url = https://github.com/giesekow/dcm-processor-cli
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE
```

