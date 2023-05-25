# Comparing `tmp/ORForise-1.4.0.tar.gz` & `tmp/ORForise-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ORForise-1.4.0.tar", last modified: Thu Mar 16 16:56:31 2023, max compression
+gzip compressed data, was "ORForise-1.4.1.tar", last modified: Thu May 25 23:05:55 2023, max compression
```

## Comparing `ORForise-1.4.0.tar` & `ORForise-1.4.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.135873 ORForise-1.4.0/
--rw-r--r--   0 nick      (1000) nick      (1000)    32476 2021-12-28 14:16:15.000000 ORForise-1.4.0/LICENSE
--rw-rw-r--   0 nick      (1000) nick      (1000)    36429 2023-03-16 16:56:31.135873 ORForise-1.4.0/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)    35833 2023-03-16 16:56:21.000000 ORForise-1.4.0/README.md
--rw-r--r--   0 nick      (1000) nick      (1000)      112 2022-09-29 21:49:27.000000 ORForise-1.4.0/pyproject.toml
--rw-r--r--   0 nick      (1000) nick      (1000)     1036 2023-03-16 16:56:31.135873 ORForise-1.4.0/setup.cfg
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.039871 ORForise-1.4.0/src/
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.043871 ORForise-1.4.0/src/ORForise/
--rw-r--r--   0 nick      (1000) nick      (1000)    10648 2022-11-30 01:36:06.000000 ORForise-1.4.0/src/ORForise/Aggregate_Compare.py
--rw-r--r--   0 nick      (1000) nick      (1000)    10298 2022-11-30 01:35:42.000000 ORForise-1.4.0/src/ORForise/Annotation_Compare.py
--rw-r--r--   0 nick      (1000) nick      (1000)    43921 2023-03-16 16:35:44.000000 ORForise-1.4.0/src/ORForise/Comparator.py
--rw-r--r--   0 nick      (1000) nick      (1000)    14105 2023-03-16 16:26:27.000000 ORForise-1.4.0/src/ORForise/GFF_Adder.py
--rw-r--r--   0 nick      (1000) nick      (1000)     9900 2023-02-08 06:50:14.000000 ORForise-1.4.0/src/ORForise/GFF_Intersector.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.051871 ORForise-1.4.0/src/ORForise/ORForise_Analysis/
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:15.000000 ORForise-1.4.0/src/ORForise/ORForise_Analysis/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     2643 2021-12-28 14:16:15.000000 ORForise-1.4.0/src/ORForise/ORForise_Analysis/cds_checker.py
--rw-r--r--   0 nick      (1000) nick      (1000)      939 2021-12-28 14:16:15.000000 ORForise-1.4.0/src/ORForise/ORForise_Analysis/gene_Lenghts.py
--rw-r--r--   0 nick      (1000) nick      (1000)    10085 2021-12-28 14:16:15.000000 ORForise-1.4.0/src/ORForise/ORForise_Analysis/genome_Metrics.py
--rw-r--r--   0 nick      (1000) nick      (1000)     3479 2021-12-28 14:16:15.000000 ORForise-1.4.0/src/ORForise/ORForise_Analysis/hypothetical_gene_predictions.py
--rw-r--r--   0 nick      (1000) nick      (1000)    10890 2021-12-28 14:16:15.000000 ORForise-1.4.0/src/ORForise/ORForise_Analysis/missed_Gene_Metrics.py
--rw-r--r--   0 nick      (1000) nick      (1000)     9515 2021-12-28 14:16:15.000000 ORForise-1.4.0/src/ORForise/ORForise_Analysis/parital_Match_Analysis.py
--rw-r--r--   0 nick      (1000) nick      (1000)     9886 2021-12-28 14:16:15.000000 ORForise-1.4.0/src/ORForise/ORForise_Analysis/result_File_Analysis.py
--rw-r--r--   0 nick      (1000) nick      (1000)     6114 2021-12-28 14:16:15.000000 ORForise-1.4.0/src/ORForise/ORForise_Analysis/start_Codon_Substitution.py
--rw-r--r--   0 nick      (1000) nick      (1000)     5387 2022-09-29 13:27:11.000000 ORForise-1.4.0/src/ORForise/StORForise.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.051871 ORForise-1.4.0/src/ORForise/Tools/
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.055871 ORForise-1.4.0/src/ORForise/Tools/Augustus/
--rw-r--r--   0 nick      (1000) nick      (1000)     1323 2022-05-07 14:34:26.000000 ORForise-1.4.0/src/ORForise/Tools/Augustus/Augustus.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:16.000000 ORForise-1.4.0/src/ORForise/Tools/Augustus/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.055871 ORForise-1.4.0/src/ORForise/Tools/Balrog/
--rw-r--r--   0 nick      (1000) nick      (1000)     1387 2022-05-07 14:34:26.000000 ORForise-1.4.0/src/ORForise/Tools/Balrog/Balrog.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:17.000000 ORForise-1.4.0/src/ORForise/Tools/Balrog/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.063871 ORForise-1.4.0/src/ORForise/Tools/EasyGene/
--rw-r--r--   0 nick      (1000) nick      (1000)     1323 2022-05-07 14:34:26.000000 ORForise-1.4.0/src/ORForise/Tools/EasyGene/EasyGene.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:17.000000 ORForise-1.4.0/src/ORForise/Tools/EasyGene/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.075872 ORForise-1.4.0/src/ORForise/Tools/FGENESB/
--rw-r--r--   0 nick      (1000) nick      (1000)     1480 2022-05-07 14:34:26.000000 ORForise-1.4.0/src/ORForise/Tools/FGENESB/FGENESB.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:17.000000 ORForise-1.4.0/src/ORForise/Tools/FGENESB/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.087872 ORForise-1.4.0/src/ORForise/Tools/FragGeneScan/
--rw-r--r--   0 nick      (1000) nick      (1000)     1376 2022-05-07 14:34:26.000000 ORForise-1.4.0/src/ORForise/Tools/FragGeneScan/FragGeneScan.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:17.000000 ORForise-1.4.0/src/ORForise/Tools/FragGeneScan/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.087872 ORForise-1.4.0/src/ORForise/Tools/GFF/
--rw-r--r--   0 nick      (1000) nick      (1000)     1818 2023-02-08 07:38:06.000000 ORForise-1.4.0/src/ORForise/Tools/GFF/GFF.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:17.000000 ORForise-1.4.0/src/ORForise/Tools/GFF/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.091872 ORForise-1.4.0/src/ORForise/Tools/GLIMMER_3/
--rw-r--r--   0 nick      (1000) nick      (1000)     1723 2022-05-07 14:34:26.000000 ORForise-1.4.0/src/ORForise/Tools/GLIMMER_3/GLIMMER_3.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:17.000000 ORForise-1.4.0/src/ORForise/Tools/GLIMMER_3/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.091872 ORForise-1.4.0/src/ORForise/Tools/GeneMark/
--rw-r--r--   0 nick      (1000) nick      (1000)     5374 2022-05-07 14:34:26.000000 ORForise-1.4.0/src/ORForise/Tools/GeneMark/GeneMark.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:17.000000 ORForise-1.4.0/src/ORForise/Tools/GeneMark/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.095872 ORForise-1.4.0/src/ORForise/Tools/GeneMark_HA/
--rw-r--r--   0 nick      (1000) nick      (1000)     1346 2022-05-07 14:34:26.000000 ORForise-1.4.0/src/ORForise/Tools/GeneMark_HA/GeneMark_HA.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:18.000000 ORForise-1.4.0/src/ORForise/Tools/GeneMark_HA/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.103872 ORForise-1.4.0/src/ORForise/Tools/GeneMark_HMM/
--rw-r--r--   0 nick      (1000) nick      (1000)     1359 2022-05-07 14:34:26.000000 ORForise-1.4.0/src/ORForise/Tools/GeneMark_HMM/GeneMark_HMM.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:18.000000 ORForise-1.4.0/src/ORForise/Tools/GeneMark_HMM/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.103872 ORForise-1.4.0/src/ORForise/Tools/GeneMark_S/
--rw-r--r--   0 nick      (1000) nick      (1000)     1334 2022-05-07 14:34:26.000000 ORForise-1.4.0/src/ORForise/Tools/GeneMark_S/GeneMark_S.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:18.000000 ORForise-1.4.0/src/ORForise/Tools/GeneMark_S/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.103872 ORForise-1.4.0/src/ORForise/Tools/GeneMark_S_2/
--rw-r--r--   0 nick      (1000) nick      (1000)     1468 2023-02-09 13:24:10.000000 ORForise-1.4.0/src/ORForise/Tools/GeneMark_S_2/GeneMark_S_2.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:18.000000 ORForise-1.4.0/src/ORForise/Tools/GeneMark_S_2/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.107872 ORForise-1.4.0/src/ORForise/Tools/MetaGene/
--rw-r--r--   0 nick      (1000) nick      (1000)     1334 2022-05-07 14:34:26.000000 ORForise-1.4.0/src/ORForise/Tools/MetaGene/MetaGene.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:18.000000 ORForise-1.4.0/src/ORForise/Tools/MetaGene/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.115872 ORForise-1.4.0/src/ORForise/Tools/MetaGeneAnnotator/
--rw-r--r--   0 nick      (1000) nick      (1000)     1469 2022-05-07 14:34:26.000000 ORForise-1.4.0/src/ORForise/Tools/MetaGeneAnnotator/MetaGeneAnnotator.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:18.000000 ORForise-1.4.0/src/ORForise/Tools/MetaGeneAnnotator/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.127873 ORForise-1.4.0/src/ORForise/Tools/MetaGeneMark/
--rw-r--r--   0 nick      (1000) nick      (1000)     1452 2022-05-07 14:34:26.000000 ORForise-1.4.0/src/ORForise/Tools/MetaGeneMark/MetaGeneMark.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:18.000000 ORForise-1.4.0/src/ORForise/Tools/MetaGeneMark/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.127873 ORForise-1.4.0/src/ORForise/Tools/Prodigal/
--rw-r--r--   0 nick      (1000) nick      (1000)     1427 2023-03-16 16:44:20.000000 ORForise-1.4.0/src/ORForise/Tools/Prodigal/Prodigal.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:19.000000 ORForise-1.4.0/src/ORForise/Tools/Prodigal/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.127873 ORForise-1.4.0/src/ORForise/Tools/Prokka/
--rw-r--r--   0 nick      (1000) nick      (1000)     1537 2023-02-09 12:28:57.000000 ORForise-1.4.0/src/ORForise/Tools/Prokka/Prokka.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:19.000000 ORForise-1.4.0/src/ORForise/Tools/Prokka/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.131873 ORForise-1.4.0/src/ORForise/Tools/StORF_Reporter/
--rw-r--r--   0 nick      (1000) nick      (1000)     1477 2022-10-27 20:03:26.000000 ORForise-1.4.0/src/ORForise/Tools/StORF_Reporter/StORF_Reporter.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-04-26 17:16:44.000000 ORForise-1.4.0/src/ORForise/Tools/StORF_Reporter/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.135873 ORForise-1.4.0/src/ORForise/Tools/StORF_Undetected/
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.135873 ORForise-1.4.0/src/ORForise/Tools/StORF_Undetected/Completely_Undetected/
--rw-r--r--   0 nick      (1000) nick      (1000)     1860 2021-12-28 14:16:19.000000 ORForise-1.4.0/src/ORForise/Tools/StORF_Undetected/Completely_Undetected/Completey_Undetected.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:19.000000 ORForise-1.4.0/src/ORForise/Tools/StORF_Undetected/Completely_Undetected/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1318 2021-12-28 14:16:19.000000 ORForise-1.4.0/src/ORForise/Tools/StORF_Undetected/StORF_Undetected.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:19.000000 ORForise-1.4.0/src/ORForise/Tools/StORF_Undetected/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.135873 ORForise-1.4.0/src/ORForise/Tools/StORF_Undetected/unvitiated_Genes/
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:19.000000 ORForise-1.4.0/src/ORForise/Tools/StORF_Undetected/unvitiated_Genes/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1863 2021-12-28 14:16:19.000000 ORForise-1.4.0/src/ORForise/Tools/StORF_Undetected/unvitiated_Genes/unvitiated_Missed_Genes.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.135873 ORForise-1.4.0/src/ORForise/Tools/TransDecoder/
--rw-r--r--   0 nick      (1000) nick      (1000)     1384 2022-05-07 14:34:26.000000 ORForise-1.4.0/src/ORForise/Tools/TransDecoder/TransDecoder.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:19.000000 ORForise-1.4.0/src/ORForise/Tools/TransDecoder/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:19.000000 ORForise-1.4.0/src/ORForise/Tools/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2021-12-28 14:16:19.000000 ORForise-1.4.0/src/ORForise/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1465 2023-02-09 08:36:36.000000 ORForise-1.4.0/src/ORForise/utils.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-16 16:56:31.043871 ORForise-1.4.0/src/ORForise.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)    36429 2023-03-16 16:56:31.000000 ORForise-1.4.0/src/ORForise.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     3007 2023-03-16 16:56:31.000000 ORForise-1.4.0/src/ORForise.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-03-16 16:56:31.000000 ORForise-1.4.0/src/ORForise.egg-info/dependency_links.txt
--rw-r--r--   0 nick      (1000) nick      (1000)      246 2023-03-16 16:56:31.000000 ORForise-1.4.0/src/ORForise.egg-info/entry_points.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        6 2023-03-16 16:56:31.000000 ORForise-1.4.0/src/ORForise.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-03-16 16:56:31.000000 ORForise-1.4.0/src/ORForise.egg-info/top_level.txt
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/
+-rw-r--r--   0 nick      (1000) nick      (1000)    32476 2022-12-23 17:30:27.000000 ORForise-1.4.1/LICENSE
+-rw-rw-r--   0 nick      (1000) nick      (1000)    36436 2023-05-25 23:05:55.897059 ORForise-1.4.1/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)    35840 2023-05-25 23:03:14.000000 ORForise-1.4.1/README.md
+-rw-r--r--   0 nick      (1000) nick      (1000)      112 2023-03-22 17:27:03.000000 ORForise-1.4.1/pyproject.toml
+-rw-r--r--   0 nick      (1000) nick      (1000)     1036 2023-05-25 23:05:55.901059 ORForise-1.4.1/setup.cfg
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.861058 ORForise-1.4.1/src/
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.877059 ORForise-1.4.1/src/ORForise/
+-rw-r--r--   0 nick      (1000) nick      (1000)    10648 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/Aggregate_Compare.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    10223 2023-03-23 16:23:21.000000 ORForise-1.4.1/src/ORForise/Annotation_Compare.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    44200 2023-05-25 22:49:25.000000 ORForise-1.4.1/src/ORForise/Comparator.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    14057 2023-05-25 22:18:26.000000 ORForise-1.4.1/src/ORForise/GFF_Adder.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     9900 2023-03-22 17:27:07.000000 ORForise-1.4.1/src/ORForise/GFF_Intersector.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/ORForise_Analysis/
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     2643 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/cds_checker.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      939 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/gene_Lenghts.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    10085 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/genome_Metrics.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     3479 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/hypothetical_gene_predictions.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    10890 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/missed_Gene_Metrics.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     9515 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/parital_Match_Analysis.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     9886 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/result_File_Analysis.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     6114 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/start_Codon_Substitution.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     5431 2023-04-22 15:00:10.000000 ORForise-1.4.1/src/ORForise/StORForise.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/Augustus/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1323 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/Tools/Augustus/Augustus.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:29.000000 ORForise-1.4.1/src/ORForise/Tools/Augustus/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/Balrog/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1387 2022-12-23 17:30:29.000000 ORForise-1.4.1/src/ORForise/Tools/Balrog/Balrog.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:29.000000 ORForise-1.4.1/src/ORForise/Tools/Balrog/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/EasyGene/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1323 2022-12-23 17:30:29.000000 ORForise-1.4.1/src/ORForise/Tools/EasyGene/EasyGene.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:29.000000 ORForise-1.4.1/src/ORForise/Tools/EasyGene/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/FGENESB/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1480 2022-12-23 17:30:29.000000 ORForise-1.4.1/src/ORForise/Tools/FGENESB/FGENESB.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/FGENESB/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/FragGeneScan/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1376 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/FragGeneScan/FragGeneScan.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/FragGeneScan/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/GFF/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1894 2023-05-25 22:21:03.000000 ORForise-1.4.1/src/ORForise/Tools/GFF/GFF.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/GFF/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/GLIMMER_3/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1723 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/GLIMMER_3/GLIMMER_3.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/GLIMMER_3/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/GeneMark/
+-rw-r--r--   0 nick      (1000) nick      (1000)     5374 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark/GeneMark.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/GeneMark_HA/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1346 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark_HA/GeneMark_HA.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark_HA/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/GeneMark_HMM/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1359 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark_HMM/GeneMark_HMM.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark_HMM/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/GeneMark_S/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1334 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark_S/GeneMark_S.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark_S/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/GeneMark_S_2/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1468 2023-03-22 17:27:07.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark_S_2/GeneMark_S_2.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark_S_2/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/MetaGene/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1334 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/MetaGene/MetaGene.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/MetaGene/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/MetaGeneAnnotator/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1469 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/MetaGeneAnnotator/MetaGeneAnnotator.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/MetaGeneAnnotator/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/MetaGeneMark/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1452 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/MetaGeneMark/MetaGeneMark.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/MetaGeneMark/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/Prodigal/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1427 2023-03-22 17:27:07.000000 ORForise-1.4.1/src/ORForise/Tools/Prodigal/Prodigal.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/Prodigal/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/Prokka/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1537 2023-03-22 17:27:07.000000 ORForise-1.4.1/src/ORForise/Tools/Prokka/Prokka.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-03-22 17:27:07.000000 ORForise-1.4.1/src/ORForise/Tools/Prokka/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/StORF_Reporter/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1609 2023-04-22 15:00:10.000000 ORForise-1.4.1/src/ORForise/Tools/StORF_Reporter/StORF_Reporter.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/StORF_Reporter/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/Completely_Undetected/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1860 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/Completely_Undetected/Completey_Undetected.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/Completely_Undetected/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1318 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/StORF_Undetected.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/unvitiated_Genes/
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/unvitiated_Genes/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1863 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/unvitiated_Genes/unvitiated_Missed_Genes.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/TransDecoder/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1384 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/TransDecoder/TransDecoder.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/TransDecoder/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1099 2023-05-25 23:03:14.000000 ORForise-1.4.1/src/ORForise/utils.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.877059 ORForise-1.4.1/src/ORForise.egg-info/
+-rw-r--r--   0 nick      (1000) nick      (1000)    36436 2023-05-25 23:05:55.000000 ORForise-1.4.1/src/ORForise.egg-info/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)     3007 2023-05-25 23:05:55.000000 ORForise-1.4.1/src/ORForise.egg-info/SOURCES.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        1 2023-05-25 23:05:55.000000 ORForise-1.4.1/src/ORForise.egg-info/dependency_links.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)      246 2023-05-25 23:05:55.000000 ORForise-1.4.1/src/ORForise.egg-info/entry_points.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        6 2023-05-25 23:05:55.000000 ORForise-1.4.1/src/ORForise.egg-info/requires.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        9 2023-05-25 23:05:55.000000 ORForise-1.4.1/src/ORForise.egg-info/top_level.txt
```

### Comparing `ORForise-1.4.0/LICENSE` & `ORForise-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/PKG-INFO` & `ORForise-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ORForise
-Version: 1.4.0
+Version: 1.4.1
 Summary: ORForise - Platform for analysing and comparing Prokaryote CoDing Sequence (CDS) Gene Predictions.
 Home-page: https://github.com/NickJD/ORForise
 Author: Nicholas Dimonaco
 Author-email: nicholas@dimonaco.co.uk
 Project-URL: Bug Tracker, https://github.com/NickJD/ORForise/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,15 +16,15 @@
 # ORForise - Prokaryote Genome Annotation Analysis and Comparison Platform
 ## Published in Bioinformatics :   https://academic.oup.com/bioinformatics/article/38/5/1198/6454948
 ### Platform for analysing and comparing Prokaryote CoDing Sequence (CDS) Gene Predictions. 
 ### Novel genome annotations can be compared to a provided reference annotation from Ensembl and predictions from other tools (or any given GFF annotation) .
 
 # Requirements and Installation:
 
-### The ORForise platform is written in Python3.8 and only requires the NumPy library (should be installed automatically by pip when installing ORForise) which is standard in most base installations of Python3.
+### The ORForise platform is written in Python (3.6-3.9) and only requires the NumPy library (should be installed automatically by pip when installing ORForise) which is standard in most base installations of Python3.
 
 ## Intallation:
 
 ### The ORForise platform is available via the pip Python package manager ```pip3 install ORForise```. 
 ### Consider using '--no-cache-dir' with pip to ensure the download of the newest version of the package.
 
 ## Required Files:
@@ -57,15 +57,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: Annotation_Compare.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -t TOOL -tp TOOL_PREDICTION
                              [-rt REFERENCE_TOOL] [-o OUTNAME] [-v {True,False}]
 
-ORForise v1.4.0: Annotatione-Compare Run Parameters.
+ORForise v1.4.1: Annotatione-Compare Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -t TOOL               Which tool to analyse? (Prodigal)
   -tp TOOL_PREDICTION   Tool genome prediction file (.gff) - Different Tool Parameters are compared individually via
@@ -107,15 +107,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: Aggregate_Compare.py [-h] -dna GENOME_DNA -t TOOLS -tp TOOL_PREDICTIONS -ref REFERENCE_ANNOTATION
                             [-rt REFERENCE_TOOL] [-o OUTNAME] [-v {True,False}]
 
-ORForise v1.4.0: Aggregate-Compare Run Parameters.
+ORForise v1.4.1: Aggregate-Compare Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -t TOOLS              Which tools to analyse? (Prodigal,GeneMarkS)
   -tp TOOL_PREDICTIONS  Tool genome prediction file (.gff) - Providefile locations for each tool comma separated
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
@@ -261,15 +261,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: GFF_Adder.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -at ADDITIONAL_TOOL -add ADDITIONAL_ANNOTATION -o
                     OUTPUT_FILE [-rt REFERENCE_TOOL] [-gi GENE_IDENT] [-gene_ident GENE_IDENT] [-olap OVERLAP]
 
-ORForise v1.4.0: GFF-Adder Run Parameters.
+ORForise v1.4.1: GFF-Adder Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -at ADDITIONAL_TOOL   Which format to use for additional annotation?
   -add ADDITIONAL_ANNOTATION
@@ -323,15 +323,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: GFF_Intersector.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -at ADDITIONAL_TOOL -add
                           ADDITIONAL_ANNOTATION -o OUTPUT_FILE [-rt REFERENCE_TOOL] [-gi GENE_IDENT] [-cov COVERAGE]
 
-ORForise v1.4.0: GFF-Intersector Run Parameters.
+ORForise v1.4.1: GFF-Intersector Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -at ADDITIONAL_TOOL   Which format to use for additional annotation?
   -add ADDITIONAL_ANNOTATION
```

### Comparing `ORForise-1.4.0/README.md` & `ORForise-1.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ORForise - Prokaryote Genome Annotation Analysis and Comparison Platform
 ## Published in Bioinformatics :   https://academic.oup.com/bioinformatics/article/38/5/1198/6454948
 ### Platform for analysing and comparing Prokaryote CoDing Sequence (CDS) Gene Predictions. 
 ### Novel genome annotations can be compared to a provided reference annotation from Ensembl and predictions from other tools (or any given GFF annotation) .
 
 # Requirements and Installation:
 
-### The ORForise platform is written in Python3.8 and only requires the NumPy library (should be installed automatically by pip when installing ORForise) which is standard in most base installations of Python3.
+### The ORForise platform is written in Python (3.6-3.9) and only requires the NumPy library (should be installed automatically by pip when installing ORForise) which is standard in most base installations of Python3.
 
 ## Intallation:
 
 ### The ORForise platform is available via the pip Python package manager ```pip3 install ORForise```. 
 ### Consider using '--no-cache-dir' with pip to ensure the download of the newest version of the package.
 
 ## Required Files:
@@ -42,15 +42,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: Annotation_Compare.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -t TOOL -tp TOOL_PREDICTION
                              [-rt REFERENCE_TOOL] [-o OUTNAME] [-v {True,False}]
 
-ORForise v1.4.0: Annotatione-Compare Run Parameters.
+ORForise v1.4.1: Annotatione-Compare Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -t TOOL               Which tool to analyse? (Prodigal)
   -tp TOOL_PREDICTION   Tool genome prediction file (.gff) - Different Tool Parameters are compared individually via
@@ -92,15 +92,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: Aggregate_Compare.py [-h] -dna GENOME_DNA -t TOOLS -tp TOOL_PREDICTIONS -ref REFERENCE_ANNOTATION
                             [-rt REFERENCE_TOOL] [-o OUTNAME] [-v {True,False}]
 
-ORForise v1.4.0: Aggregate-Compare Run Parameters.
+ORForise v1.4.1: Aggregate-Compare Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -t TOOLS              Which tools to analyse? (Prodigal,GeneMarkS)
   -tp TOOL_PREDICTIONS  Tool genome prediction file (.gff) - Providefile locations for each tool comma separated
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
@@ -246,15 +246,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: GFF_Adder.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -at ADDITIONAL_TOOL -add ADDITIONAL_ANNOTATION -o
                     OUTPUT_FILE [-rt REFERENCE_TOOL] [-gi GENE_IDENT] [-gene_ident GENE_IDENT] [-olap OVERLAP]
 
-ORForise v1.4.0: GFF-Adder Run Parameters.
+ORForise v1.4.1: GFF-Adder Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -at ADDITIONAL_TOOL   Which format to use for additional annotation?
   -add ADDITIONAL_ANNOTATION
@@ -308,15 +308,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: GFF_Intersector.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -at ADDITIONAL_TOOL -add
                           ADDITIONAL_ANNOTATION -o OUTPUT_FILE [-rt REFERENCE_TOOL] [-gi GENE_IDENT] [-cov COVERAGE]
 
-ORForise v1.4.0: GFF-Intersector Run Parameters.
+ORForise v1.4.1: GFF-Intersector Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -at ADDITIONAL_TOOL   Which format to use for additional annotation?
   -add ADDITIONAL_ANNOTATION
```

### Comparing `ORForise-1.4.0/setup.cfg` & `ORForise-1.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ORForise
-version = 1.4.0
+version = 1.4.1
 author = Nicholas Dimonaco
 author_email = nicholas@dimonaco.co.uk
 description = ORForise - Platform for analysing and comparing Prokaryote CoDing Sequence (CDS) Gene Predictions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/NickJD/ORForise
 project_urls =
```

### Comparing `ORForise-1.4.0/src/ORForise/Aggregate_Compare.py` & `ORForise-1.4.1/src/ORForise/Aggregate_Compare.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Annotation_Compare.py` & `ORForise-1.4.1/src/ORForise/Annotation_Compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,16 @@
     from utils import *
 except ImportError:
     from ORForise.utils import *
 
 ##########################
 
 def comparator(options):
-    genome_Seq = ""
-    with open(options.genome_DNA, 'r') as genome:
-        for line in genome:
-            line = line.replace("\n", "")
-            if not line.startswith('>'):
-                genome_Seq += str(line)
+    with open(options.genome_DNA, mode='r') as genome:
+        genome_Seq = "".join(line.rstrip() for line in genome if not line.startswith('>'))
     ##############################################
     if not options.reference_tool:  # IF using Ensembl for comparison
         ref_genes = collections.OrderedDict()  # Order is important
         count = 0
         with open(options.reference_annotation, 'r') as genome_gff:
             for line in genome_gff:
                 line = line.split('\t')
```

### Comparing `ORForise-1.4.0/src/ORForise/Comparator.py` & `ORForise-1.4.1/src/ORForise/Comparator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-
 try:
     from utils import *
 except ImportError:
     from ORForise.utils import *
 
 
 class comparator:  # Class to hold global-type variables
@@ -42,15 +41,16 @@
 #         else:
 #             to_return = dictionary[newkey].split(',')
 #             to_return = to_return[0]+'_'+to_return[1]+'_'+to_return[2]
 #             return to_return
 #     else:
 #         print ('Key not found')
 
-
+def is_double_range(range1, range2):
+    return len(range1) >= 2 * len(range2)
 def nuc_Count(start, stop, strand):  # Gets correct seq then returns GC
     if strand == '-':
         r_Start = comp.genome_Size - stop
         r_Stop = comp.genome_Size - start
         seq = (comp.genome_Seq_Rev[r_Start:r_Stop + 1])
     elif strand == '+':
         seq = (comp.genome_Seq[start - 1:stop])
@@ -259,53 +259,57 @@
         comp.partial_Hits.update({partial: [genSeq, orfSeq]})
 
 
 def tool_comparison(ref_genes, orfs, genome, verbose):
     comp.genome_Seq = genome
     comp.genome_Seq_Rev = revCompIterative(genome)
     comp.genome_Size = len(genome)
+
+    better_pos_orfs_items = [[(int(pos.split(',')[0]), int(pos.split(',')[1])), orf_Details] for pos, orf_Details in orfs.items()] #TODO: turn pos into tuple instead of string everywhere
+
     for gene_num, gene_details in ref_genes.items():  # Loop through each gene to compare against predicted ORFs
         g_Start = int(gene_details[0])
         g_Stop = int(gene_details[1])
         g_Strand = gene_details[2]
         g_pos = str(g_Start) + ',' + str(g_Stop)
         gene_Set = set(range(g_Start,
                              g_Stop + 1))  # Used to check Overlap of ORFs and pick best match - slow but confirms best match
         overlapping_ORFs = collections.OrderedDict()
         perfect_Match = False
         out_Frame = False
-        for pos, orf_Details in orfs.items():  # Check if perfect match, if not check if match covers at least 75% of gene - Loop through ALL ORFs - SLOW
-            o_Start = int(pos.split(',')[0])
-            o_Stop = int(pos.split(',')[1])
+        for pos, orf_Details in better_pos_orfs_items:  # Check if perfect match, if not check if match covers at least 75% of gene - Loop through ALL ORFs - SLOW
+            o_Start,o_Stop = pos
             o_Strand = orf_Details[0]
             #orf_Set = set(range(o_Start, o_Stop + 1)) Removed for optimisation
             if o_Stop <= g_Start or o_Start >= g_Stop:  # Not caught up yet
                 continue
             elif o_Start == g_Start and o_Stop == g_Stop:  # If perfect match, break and skip the rest of the ORFs
                 perfect_Match = True
                 break
+            elif is_double_range(range(o_Start, o_Stop), range(g_Start,g_Stop)):  # If ORF is double or more than the length of the gene, we do not count as found.
+                continue
             elif g_Start <= o_Start < g_Stop or g_Start < o_Stop < g_Stop:  # If ORF Start or Stop is between gene Start or Stop
                 #overlap = len(gene_Set.intersection(orf_Set)) # Replaced for optimisation
                 overlap = max(min(o_Stop, g_Stop) - max(o_Start, g_Start), -1) + 1
                 coverage = 100 * float(overlap) / float(len(gene_Set))
                 orf_Details.append(coverage)
                 if abs(o_Stop - g_Stop) % 3 == 0 and o_Strand == g_Strand and coverage >= MIN_COVERAGE:  # Only continue if ORF covers at least 75% of the gene and is in frame
-                    overlapping_ORFs.update({pos: orf_Details})
+                    overlapping_ORFs.update({f'{o_Start},{o_Stop}': orf_Details})
                 elif coverage >= MIN_COVERAGE:  # Not in frame / on same strand
-                    comp.out_Of_Frame_ORFs.update({pos: orf_Details})
+                    comp.out_Of_Frame_ORFs.update({f'{o_Start},{o_Stop}': orf_Details})
                     out_Frame = True
             elif o_Start <= g_Start and o_Stop >= g_Stop:  # If ORF extends one or both ends of the gene
                 #overlap = len(gene_Set.intersection(orf_Set)) # Replaced for optimisation
                 overlap = max(min(o_Stop, g_Stop) - max(o_Start, g_Start), -1) + 1
                 coverage = 100 * float(overlap) / float(len(gene_Set))
                 orf_Details.append(coverage)
                 if abs(o_Stop - g_Stop) % 3 == 0 and o_Strand == g_Strand and coverage >= MIN_COVERAGE:  # Only continue if ORF covers at least 75% of the gene and is in frame
-                    overlapping_ORFs.update({pos: orf_Details})
+                    overlapping_ORFs.update({f'{o_Start},{o_Stop}': orf_Details})
                 elif coverage >= MIN_COVERAGE:
-                    comp.out_Of_Frame_ORFs.update({pos: orf_Details})
+                    comp.out_Of_Frame_ORFs.update({f'{o_Start},{o_Stop}': orf_Details})
                     out_Frame = True
             else:
                 if verbose == True:
                     print("Unexpected Error Finding Predicted CDSs")  # Should not happen
         # Now Check that we select the best ORF
         ### Multi_Match_ORFs Should contain All genes found by a specific ORF
         if perfect_Match == True:  # Check if the ORF is a perfect match to the Gene
@@ -387,27 +391,28 @@
     else:
         median_Stop_Difference = 'N/A'
 
     # Get Start and Stop Codon Usage
     atg_P, gtg_P, ttg_P, att_P, ctg_P, other_Start_P, other_Starts = start_Codon_Count(orfs)
     tag_P, taa_P, tga_P, other_Stop_P, other_Stops = stop_Codon_Count(orfs)
     # Count nucleotides found from ALL ORFs
-    gene_Nuc_Array = np.zeros((comp.genome_Size), dtype=np.int)
-    orf_Nuc_Array = np.zeros((comp.genome_Size), dtype=np.int)
-    matched_ORF_Nuc_Array = np.zeros((comp.genome_Size), dtype=np.int)
+    gene_Nuc_Array = np.zeros((comp.genome_Size), dtype=np.bool)
+    orf_Nuc_Array = np.zeros((comp.genome_Size), dtype=np.bool)
+    matched_ORF_Nuc_Array = np.zeros((comp.genome_Size), dtype=np.bool)
 
     prev_Gene_Stop = 0
     prev_Gene_Overlapped = False
     for gene_Num, gene_details in ref_genes.items():  # Loop through each gene to compare against predicted ORFs
         g_Start = int(gene_details[0])
         g_Stop = int(gene_details[1])
         g_Strand = gene_details[2]
-        gene_Length = (g_Stop - g_Start)
+        gene_Length = (g_Stop - g_Start) +1
+        if gene_Length == 0: print(g_Start, g_Stop, "!!!!!!!!!!!!!!!!!!!!!!!!")
         comp.gene_Lengths.append(gene_Length)
-        gene_Nuc_Array[g_Start - 1:g_Stop] = [1]  # Changing all between the two positions to 1's
+        gene_Nuc_Array[g_Start - 1:g_Stop] = True  # Changing all between the two positions to 1's
         comp.gene_GC.append(nuc_Count(g_Start, g_Stop, g_Strand))
         if gene_Length <= SHORT_ORF_LENGTH:  # .utils
             comp.gene_Short.append(gene_Length)
         ### Calculate overlapping Genes -
         if prev_Gene_Stop > g_Start:
             if '+' in g_Strand:
                 comp.gene_Pos_Olap.append(prev_Gene_Stop - g_Start)
@@ -441,17 +446,17 @@
         if o_Positions not in list(comp.matched_ORFs.keys()):
             orf_Unmatched(o_Start, o_Stop, o_Strand)
         # Get ORF Strand metrics:
         if o_Strand == "+":  # Get number of Positive and Negative strand ORFs
             comp.pos_Strand += 1
         elif o_Strand == "-":
             comp.neg_Strand += 1
-        orf_Length = (o_Stop - o_Start)
+        orf_Length = (o_Stop - o_Start) +1
         comp.orf_Lengths.append(orf_Length)
-        orf_Nuc_Array[o_Start - 1:o_Stop] = [1]  # Changing all between the two positions to 1's
+        orf_Nuc_Array[o_Start - 1:o_Stop] = True  # Changing all between the two positions to 1's
         comp.orf_GC.append(nuc_Count(o_Start, o_Stop, o_Strand))
         if orf_Length <= SHORT_ORF_LENGTH:  # .utils
             comp.orf_Short.append(orf_Length)
         ### Calculate overlapping ORFs -
         if prev_ORF_Stop > o_Start:
             if '+' in o_Strand:
                 comp.orf_Pos_Olap.append(prev_ORF_Stop - o_Start)
@@ -476,15 +481,15 @@
     matched_Prev_ORF_Stop = 0
     matched_Prev_ORF_Overlapped = False
     for mo_Positions, m_ORF_Details in comp.matched_ORFs.items():
         mo_Start = int(mo_Positions.split(',')[0])
         mo_Stop = int(mo_Positions.split(',')[1])
         mo_Strand = m_ORF_Details[0]
         mo_Length = (mo_Stop - mo_Start)
-        matched_ORF_Nuc_Array[mo_Start - 1:mo_Stop] = [1]  # This is the complete matched orf not the matched orf bits
+        matched_ORF_Nuc_Array[mo_Start - 1:mo_Stop] = True  # This is the complete matched orf not the matched orf bits
 
         comp.m_ORF_GC.append(nuc_Count(mo_Start, mo_Stop, mo_Strand))
         if mo_Length <= SHORT_ORF_LENGTH:  # .utils
             comp.m_ORF_Short.append(mo_Length)
         ### Calculate overlapping Matched ORFs -
         if matched_Prev_ORF_Stop > mo_Start:
             if '+' in mo_Strand:
@@ -502,38 +507,36 @@
         matched_Prev_ORF_Stop = mo_Stop
     if matched_Prev_ORF_Overlapped == True:  # If last has a prev overlap, count it
         if '+' in mo_Strand:
             comp.m_ORF_Pos_Olap.append(0)
         elif '-' in mo_Strand:
             comp.m_ORF_Neg_Olap.append(0)
     ####
-    gene_Coverage_Genome = format(100 * np.count_nonzero(gene_Nuc_Array) / comp.genome_Size, '.2f')
-    orf_Coverage_Genome = format(100 * np.count_nonzero(orf_Nuc_Array) / comp.genome_Size, '.2f')
-    matched_ORF_Coverage_Genome = format(100 * np.count_nonzero(matched_ORF_Nuc_Array) / comp.genome_Size,
+    gene_Coverage_Genome = format(100 * np.sum(gene_Nuc_Array) / comp.genome_Size, '.2f')
+    orf_Coverage_Genome = format(100 * np.sum(orf_Nuc_Array) / comp.genome_Size, '.2f')
+    matched_ORF_Coverage_Genome = format(100 * np.sum(matched_ORF_Nuc_Array) / comp.genome_Size,
                                          '.2f')  # This gets the nts which are in matched ORFs - Check below
     # matched_ORF_Nuc_AND_Gene = np.logical_and(matched_ORF_Nuc_Array,gene_Nuc_Array) + [0 for i in range(len(gene_Nuc_Array))] # This gets the nts which are in both matched ORFs and detected genes
     # matched_ORF_Coverage_Genome = format(100 * np.count_nonzero(matched_ORF_Nuc_AND_Gene) / comp.genome_Size,'.2f')
 
     # gene and orf nucleotide Intersection
-    gene_ORF_Nuc_Intersection = np.count_nonzero(gene_Nuc_Array & orf_Nuc_Array)
+    gene_ORF_Nuc_Intersection = np.sum(gene_Nuc_Array & orf_Nuc_Array)
     # not gene but orf nucleotides
-    not_Gene_Nuc_Array = np.logical_not(gene_Nuc_Array) + [0 for i in range(
-        len(gene_Nuc_Array))]  # End part to keep array as 1,0 not T,F
-    not_Gene_Nuc_And_ORF_Count = np.count_nonzero(not_Gene_Nuc_Array & orf_Nuc_Array)
+    not_Gene_Nuc_Array = np.logical_not(gene_Nuc_Array)
+    not_Gene_Nuc_And_ORF_Count = np.sum(not_Gene_Nuc_Array & orf_Nuc_Array)
     # not orf nucleotides but gene
-    not_ORF_Nuc_Array = np.logical_not(orf_Nuc_Array) + [0 for i in range(
-        len(orf_Nuc_Array))]  # End part to keep array as 1,0 not T,F
-    not_ORF_Nuc_And_Gene_Count = np.count_nonzero(not_ORF_Nuc_Array & gene_Nuc_Array)
+    not_ORF_Nuc_Array = np.logical_not(orf_Nuc_Array)
+    not_ORF_Nuc_And_Gene_Count = np.sum(not_ORF_Nuc_Array & gene_Nuc_Array)
     # not gene or orf nucleotides
-    not_Gene_Nuc_Not_ORF_Nuc_Count = np.count_nonzero(not_Gene_Nuc_Array & not_ORF_Nuc_Array)
+    not_Gene_Nuc_Not_ORF_Nuc_Count = np.sum(not_Gene_Nuc_Array & not_ORF_Nuc_Array)
     # Nucleotide 'accuracy' - Normalised by number of nucelotides annotated by a gene
-    NT_TP = format(gene_ORF_Nuc_Intersection / np.count_nonzero(gene_Nuc_Array), '.2f')
-    NT_FP = format(not_Gene_Nuc_And_ORF_Count / np.count_nonzero(not_Gene_Nuc_Array), '.2f')
-    NT_FN = format(not_ORF_Nuc_And_Gene_Count / np.count_nonzero(gene_Nuc_Array), '.2f')
-    NT_TN = format(not_Gene_Nuc_Not_ORF_Nuc_Count / np.count_nonzero(not_Gene_Nuc_Array), '.2f')
+    NT_TP = format(gene_ORF_Nuc_Intersection / np.sum(gene_Nuc_Array), '.2f')
+    NT_FP = format(not_Gene_Nuc_And_ORF_Count / np.sum(not_Gene_Nuc_Array), '.2f')
+    NT_FN = format(not_ORF_Nuc_And_Gene_Count / np.sum(gene_Nuc_Array), '.2f')
+    NT_TN = format(not_Gene_Nuc_Not_ORF_Nuc_Count / np.sum(not_Gene_Nuc_Array), '.2f')
     NT_Precision = format(gene_ORF_Nuc_Intersection / (gene_ORF_Nuc_Intersection + not_Gene_Nuc_And_ORF_Count), '.2f')
     NT_Recall = format(gene_ORF_Nuc_Intersection / (gene_ORF_Nuc_Intersection + not_ORF_Nuc_And_Gene_Count), '.2f')
     NT_False_Discovery_Rate = format(
         not_Gene_Nuc_And_ORF_Count / (not_Gene_Nuc_And_ORF_Count + gene_ORF_Nuc_Intersection), '.2f')
     ################################# Precision and Recall of whole ORFs and Genes
     TP = format(len(comp.genes_Detected) / len(ref_genes), '.2f')
     FP = format(len(comp.unmatched_ORFs) / len(ref_genes), '.2f')
```

### Comparing `ORForise-1.4.0/src/ORForise/GFF_Adder.py` & `ORForise-1.4.1/src/ORForise/GFF_Adder.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,14 @@
     Ref_Only = 0
     Ref_Combined = collections.defaultdict(int)
     Non_Ref_Combined = collections.defaultdict(int)
 
 
     for pos, data in combined_ORFs.items():
         pos_ = pos.split(',')
-        if '15040' in pos:
-            print(2)
         start = pos_[0]
         stop = pos_[-1]
         strand = data[0]
         length = int(stop) - int(start)
         additional_annotation_info = ''
         tools = additional_tool.split(',')
         matched_tools = ''
```

### Comparing `ORForise-1.4.0/src/ORForise/GFF_Intersector.py` & `ORForise-1.4.1/src/ORForise/GFF_Intersector.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/ORForise_Analysis/cds_checker.py` & `ORForise-1.4.1/src/ORForise/ORForise_Analysis/cds_checker.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/ORForise_Analysis/gene_Lenghts.py` & `ORForise-1.4.1/src/ORForise/ORForise_Analysis/gene_Lenghts.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/ORForise_Analysis/genome_Metrics.py` & `ORForise-1.4.1/src/ORForise/ORForise_Analysis/genome_Metrics.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/ORForise_Analysis/hypothetical_gene_predictions.py` & `ORForise-1.4.1/src/ORForise/ORForise_Analysis/hypothetical_gene_predictions.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/ORForise_Analysis/missed_Gene_Metrics.py` & `ORForise-1.4.1/src/ORForise/ORForise_Analysis/missed_Gene_Metrics.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/ORForise_Analysis/parital_Match_Analysis.py` & `ORForise-1.4.1/src/ORForise/ORForise_Analysis/parital_Match_Analysis.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/ORForise_Analysis/result_File_Analysis.py` & `ORForise-1.4.1/src/ORForise/ORForise_Analysis/result_File_Analysis.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/ORForise_Analysis/start_Codon_Substitution.py` & `ORForise-1.4.1/src/ORForise/ORForise_Analysis/start_Codon_Substitution.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/StORForise.py` & `ORForise-1.4.1/src/ORForise/StORForise.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,39 +7,39 @@
 from Comparator import tool_comparison
 
 ###################
 
 
 def comparator(tool, input_to_analyse, storfs_to_find_missing, genome_to_compare):
     genome_Seq = ""
-    with open('Genomes/' + genome_to_compare + '.fa', 'r') as genome:
+    with open(genome_to_compare, 'r') as genome:
         for line in genome:
             line = line.replace("\n", "")
             if ">" not in line:
                 genome_Seq += str(line)
     ##############################################
     genes = collections.OrderedDict()
     count = 0
-    with open('Tools/StORF_Undetected/' + input_to_analyse, 'r') as genome_gff:  # Get list of missed genes
+    with open(input_to_analyse, 'r') as genome_gff:  # Get list of missed genes
         for line in genome_gff:
             if ">" in line:
                 line = line.strip()
-                Start = int(line.split('_')[1])
-                Stop = int(line.split('_')[2])
-                Strand = line.split('_')[3]
-                Gene = str(Start) + ',' + str(Stop) + ',' + Strand
-                genes.update({count: Gene})
+                start = int(line.split('_')[1])
+                stop = int(line.split('_')[2])
+                strand = line.split('_')[3]
+                gene_details = [start,stop,strand]
+                genes.update({count: gene_details})
                 count += 1
     ##################################
     tool_predictions = import_module('Tools.' + tool + '.' + tool)
     tool_predictions = getattr(tool_predictions, tool)
     orfs = tool_predictions(storfs_to_find_missing, genome_Seq)
-    all_Metrics, all_rep_Metrics, start_precision, stop_precision, other_starts, other_stops, missed_genes, unmatched_orfs, undetected_gene_metrics, unmatched_orf_metrics, gene_coverage_genome, multi_Matched_ORFs, partial_Hits = tool_comparison(
-        genes, orfs, genome_Seq)
-    outname = tool + '_' + genome_to_compare
+    all_Metrics, all_rep_Metrics, start_precision, stop_precision, other_starts, other_stops, perfect_Matches, missed_genes, unmatched_orfs, undetected_gene_metrics, unmatched_orf_metrics, orf_Coverage_Genome, matched_ORF_Coverage_Genome, gene_coverage_genome, multi_Matched_ORFs, partial_Hits = tool_comparison(
+        genes, orfs, genome_Seq,True)
+    outname = tool + '_' + genome_to_compare.split('/')[-1].split('.')[0]
     metric_description = list(all_Metrics.keys())
     metrics = list(all_Metrics.values())
     rep_metric_description = list(all_rep_Metrics.keys())
     rep_metrics = list(all_rep_Metrics.values())
     with open("Tools/" + tool + '/' + outname + '.csv', 'w', newline='\n',
               encoding='utf-8') as out_file:  # Clear write out of report
         tool_out = csv.writer(out_file, quoting=csv.QUOTE_NONE, escapechar=" ")
```

### Comparing `ORForise-1.4.0/src/ORForise/Tools/Augustus/Augustus.py` & `ORForise-1.4.1/src/ORForise/Tools/Augustus/Augustus.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/Balrog/Balrog.py` & `ORForise-1.4.1/src/ORForise/Tools/Balrog/Balrog.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/EasyGene/EasyGene.py` & `ORForise-1.4.1/src/ORForise/Tools/EasyGene/EasyGene.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/FGENESB/FGENESB.py` & `ORForise-1.4.1/src/ORForise/Tools/FGENESB/FGENESB.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/FragGeneScan/FragGeneScan.py` & `ORForise-1.4.1/src/ORForise/Tools/FragGeneScan/FragGeneScan.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/GFF/GFF.py` & `ORForise-1.4.1/src/ORForise/Tools/GFF/GFF.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,24 +7,25 @@
     from ORForise.utils import revCompIterative
     from ORForise.utils import sortORFs
 
 
 def GFF(*args):
     tool_pred = args[0]
     genome = args[1]
-    types = args[2]
+    #types = args[2]
     GFF_ORFs = collections.OrderedDict()
     genome_size = len(genome)
     genome_rev = revCompIterative(genome)
     with open(tool_pred, 'r') as gff_input:
         for line in gff_input:
             if '#' not in line:
                 line = line.split('\t')
-                gene_types = types.split(',')
-                if any(gene_type == line[2] for gene_type in gene_types)and len(line) == 9:  # line[2] for normalrun
+                #gene_types = types.split(',') - Temporary fix
+                #if any(gene_type == line[2] for gene_type in gene_types) and len(line) == 9:  # line[2] for normalrun
+                if 'CDS' in line[2] and len(line) == 9:
                     start = int(line[3])
                     stop = int(line[4])
                     strand = line[6]
                     info = line[8]
                     #name = line[8].split('Name=')[1].split(';')[0] # Issue with multiple records for each gene.
                     if '-' in strand:  # Reverse Compliment starts and stops adjusted
                         r_start = genome_size - stop
```

### Comparing `ORForise-1.4.0/src/ORForise/Tools/GLIMMER_3/GLIMMER_3.py` & `ORForise-1.4.1/src/ORForise/Tools/GLIMMER_3/GLIMMER_3.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/GeneMark/GeneMark.py` & `ORForise-1.4.1/src/ORForise/Tools/GeneMark/GeneMark.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/GeneMark_HA/GeneMark_HA.py` & `ORForise-1.4.1/src/ORForise/Tools/GeneMark_HA/GeneMark_HA.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/GeneMark_HMM/GeneMark_HMM.py` & `ORForise-1.4.1/src/ORForise/Tools/GeneMark_HMM/GeneMark_HMM.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/GeneMark_S/GeneMark_S.py` & `ORForise-1.4.1/src/ORForise/Tools/GeneMark_S/GeneMark_S.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/GeneMark_S_2/GeneMark_S_2.py` & `ORForise-1.4.1/src/ORForise/Tools/GeneMark_S_2/GeneMark_S_2.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/MetaGene/MetaGene.py` & `ORForise-1.4.1/src/ORForise/Tools/MetaGene/MetaGene.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/MetaGeneAnnotator/MetaGeneAnnotator.py` & `ORForise-1.4.1/src/ORForise/Tools/MetaGeneAnnotator/MetaGeneAnnotator.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/MetaGeneMark/MetaGeneMark.py` & `ORForise-1.4.1/src/ORForise/Tools/MetaGeneMark/MetaGeneMark.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/Prodigal/Prodigal.py` & `ORForise-1.4.1/src/ORForise/Tools/Prodigal/Prodigal.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/Prokka/Prokka.py` & `ORForise-1.4.1/src/ORForise/Tools/Prokka/Prokka.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/StORF_Reporter/StORF_Reporter.py` & `ORForise-1.4.1/src/ORForise/Tools/StORF_Reporter/StORF_Reporter.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,27 +10,28 @@
 
 def StORF_Reporter(tool_pred, genome):
     storf_orfs = collections.OrderedDict()
     genome_size = len(genome)
     genome_rev = revCompIterative(genome)
     with open(tool_pred, 'r') as storf_input:
         for line in storf_input:
-            if '#' not in line:
+            if not line.startswith('#') and not line.startswith('\n'):
                 line = line.split()
-                if 'StORF_Reporter' in line[1] or 'StoRF_Reporter' in line[1]: # need to harmonise this.
+                if 'StORF_Reporter' in line[1] or 'StoRF_Reporter' in line[1]  or 'StORF' in line[1] or 'StORF-Reporter' in line[1]: # need to harmonise this.
                     start = int(line[3])
                     stop = int(line[4])
                     strand = line[6]
+                    info = line[8]
                     if '-' in strand:  # Reverse Compliment starts and stops adjusted
                         r_start = genome_size - stop
                         r_stop = genome_size - start
                         startCodon = genome_rev[r_start:r_start + 3]
                         stopCodon = genome_rev[r_stop - 2:r_stop + 1]
                     elif '+' in strand:
                         startCodon = genome[start:start + 3]
                         stopCodon = genome[stop - 3:stop]
                     po = str(start) + ',' + str(stop)
-                    orf = [strand, startCodon, stopCodon, line[2]] # StORF/Con-StORF or CDS??
+                    orf = [strand, startCodon, stopCodon, 'CDS', info] # StORF/Con-StORF or CDS??
                     storf_orfs.update({po: orf})
 
     storf_orfs = sortORFs(storf_orfs)
     return storf_orfs
```

### Comparing `ORForise-1.4.0/src/ORForise/Tools/StORF_Undetected/Completely_Undetected/Completey_Undetected.py` & `ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/Completely_Undetected/Completey_Undetected.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/StORF_Undetected/StORF_Undetected.py` & `ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/StORF_Undetected.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/StORF_Undetected/unvitiated_Genes/unvitiated_Missed_Genes.py` & `ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/unvitiated_Genes/unvitiated_Missed_Genes.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise/Tools/TransDecoder/TransDecoder.py` & `ORForise-1.4.1/src/ORForise/Tools/TransDecoder/TransDecoder.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.0/src/ORForise.egg-info/PKG-INFO` & `ORForise-1.4.1/src/ORForise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ORForise
-Version: 1.4.0
+Version: 1.4.1
 Summary: ORForise - Platform for analysing and comparing Prokaryote CoDing Sequence (CDS) Gene Predictions.
 Home-page: https://github.com/NickJD/ORForise
 Author: Nicholas Dimonaco
 Author-email: nicholas@dimonaco.co.uk
 Project-URL: Bug Tracker, https://github.com/NickJD/ORForise/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,15 +16,15 @@
 # ORForise - Prokaryote Genome Annotation Analysis and Comparison Platform
 ## Published in Bioinformatics :   https://academic.oup.com/bioinformatics/article/38/5/1198/6454948
 ### Platform for analysing and comparing Prokaryote CoDing Sequence (CDS) Gene Predictions. 
 ### Novel genome annotations can be compared to a provided reference annotation from Ensembl and predictions from other tools (or any given GFF annotation) .
 
 # Requirements and Installation:
 
-### The ORForise platform is written in Python3.8 and only requires the NumPy library (should be installed automatically by pip when installing ORForise) which is standard in most base installations of Python3.
+### The ORForise platform is written in Python (3.6-3.9) and only requires the NumPy library (should be installed automatically by pip when installing ORForise) which is standard in most base installations of Python3.
 
 ## Intallation:
 
 ### The ORForise platform is available via the pip Python package manager ```pip3 install ORForise```. 
 ### Consider using '--no-cache-dir' with pip to ensure the download of the newest version of the package.
 
 ## Required Files:
@@ -57,15 +57,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: Annotation_Compare.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -t TOOL -tp TOOL_PREDICTION
                              [-rt REFERENCE_TOOL] [-o OUTNAME] [-v {True,False}]
 
-ORForise v1.4.0: Annotatione-Compare Run Parameters.
+ORForise v1.4.1: Annotatione-Compare Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -t TOOL               Which tool to analyse? (Prodigal)
   -tp TOOL_PREDICTION   Tool genome prediction file (.gff) - Different Tool Parameters are compared individually via
@@ -107,15 +107,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: Aggregate_Compare.py [-h] -dna GENOME_DNA -t TOOLS -tp TOOL_PREDICTIONS -ref REFERENCE_ANNOTATION
                             [-rt REFERENCE_TOOL] [-o OUTNAME] [-v {True,False}]
 
-ORForise v1.4.0: Aggregate-Compare Run Parameters.
+ORForise v1.4.1: Aggregate-Compare Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -t TOOLS              Which tools to analyse? (Prodigal,GeneMarkS)
   -tp TOOL_PREDICTIONS  Tool genome prediction file (.gff) - Providefile locations for each tool comma separated
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
@@ -261,15 +261,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: GFF_Adder.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -at ADDITIONAL_TOOL -add ADDITIONAL_ANNOTATION -o
                     OUTPUT_FILE [-rt REFERENCE_TOOL] [-gi GENE_IDENT] [-gene_ident GENE_IDENT] [-olap OVERLAP]
 
-ORForise v1.4.0: GFF-Adder Run Parameters.
+ORForise v1.4.1: GFF-Adder Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -at ADDITIONAL_TOOL   Which format to use for additional annotation?
   -add ADDITIONAL_ANNOTATION
@@ -323,15 +323,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: GFF_Intersector.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -at ADDITIONAL_TOOL -add
                           ADDITIONAL_ANNOTATION -o OUTPUT_FILE [-rt REFERENCE_TOOL] [-gi GENE_IDENT] [-cov COVERAGE]
 
-ORForise v1.4.0: GFF-Intersector Run Parameters.
+ORForise v1.4.1: GFF-Intersector Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -at ADDITIONAL_TOOL   Which format to use for additional annotation?
   -add ADDITIONAL_ANNOTATION
```

### Comparing `ORForise-1.4.0/src/ORForise.egg-info/SOURCES.txt` & `ORForise-1.4.1/src/ORForise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

