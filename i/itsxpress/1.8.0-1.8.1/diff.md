# Comparing `tmp/itsxpress-1.8.0.tar.gz` & `tmp/itsxpress-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/itsxpress-1.8.0.tar", last modified: Mon Dec  9 21:50:33 2019, max compression
+gzip compressed data, was "itsxpress-1.8.1.tar", last modified: Thu May 25 19:03:34 2023, max compression
```

## Comparing `itsxpress-1.8.0.tar` & `itsxpress-1.8.1.tar`

### file list

```diff
@@ -1,61 +1,59 @@
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-09 21:50:33.000000 itsxpress-1.8.0/
--rw-r--r--   0 rivers     (501) staff       (20)     9726 2019-12-09 21:50:33.000000 itsxpress-1.8.0/PKG-INFO
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-09 21:50:33.000000 itsxpress-1.8.0/itsxpress/
--rw-r--r--   0 rivers     (501) staff       (20)     1519 2019-12-09 21:35:37.000000 itsxpress-1.8.0/itsxpress/definitions.py
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-09 21:50:33.000000 itsxpress-1.8.0/itsxpress/ITSx_db/
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-09 21:50:33.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/
--rw-r--r--   0 rivers     (501) staff       (20)   487925 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/G.hmm
--rw-r--r--   0 rivers     (501) staff       (20)    85766 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/P.hmm
--rw-r--r--   0 rivers     (501) staff       (20)    60046 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/Q.hmm
--rw-r--r--   0 rivers     (501) staff       (20)  4615535 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/F.hmm
--rw-r--r--   0 rivers     (501) staff       (20)   214397 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/D.hmm
--rw-r--r--   0 rivers     (501) staff       (20)    68619 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/S.hmm
--rw-r--r--   0 rivers     (501) staff       (20)   351565 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/R.hmm
--rw-r--r--   0 rivers     (501) staff       (20)   120052 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/E.hmm
--rw-r--r--   0 rivers     (501) staff       (20)   754700 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/A.hmm
--rw-r--r--   0 rivers     (501) staff       (20)    34311 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/U.hmm
--rw-r--r--   0 rivers     (501) staff       (20)   128601 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/B.hmm
--rw-r--r--   0 rivers     (501) staff       (20)   171599 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/C.hmm
--rw-r--r--   0 rivers     (501) staff       (20)  1922155 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/T.hmm
--rw-r--r--   0 rivers     (501) staff       (20)   608925 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/O.hmm
--rw-r--r--   0 rivers     (501) staff       (20)  3035909 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/M.hmm
--rw-r--r--   0 rivers     (501) staff       (20)   334620 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/L.hmm
--rw-r--r--   0 rivers     (501) staff       (20)   205812 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/H.hmm
--rw-r--r--   0 rivers     (501) staff       (20)    42875 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/I.hmm
--rw-r--r--   0 rivers     (501) staff       (20) 13243412 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/all.hmm
--rw-r--r--   0 rivers     (501) staff       (20)       85 2018-07-06 13:27:29.000000 itsxpress-1.8.0/itsxpress/__init__.py
--rwxr-xr-x   0 rivers     (501) staff       (20)    33518 2019-12-09 21:35:37.000000 itsxpress-1.8.0/itsxpress/main.py
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-09 21:50:33.000000 itsxpress-1.8.0/itsxpress.egg-info/
--rw-r--r--   0 rivers     (501) staff       (20)     9726 2019-12-09 21:50:32.000000 itsxpress-1.8.0/itsxpress.egg-info/PKG-INFO
--rw-r--r--   0 rivers     (501) staff       (20)        1 2018-07-06 13:28:09.000000 itsxpress-1.8.0/itsxpress.egg-info/not-zip-safe
--rw-r--r--   0 rivers     (501) staff       (20)     1518 2019-12-09 21:50:32.000000 itsxpress-1.8.0/itsxpress.egg-info/SOURCES.txt
--rw-r--r--   0 rivers     (501) staff       (20)       51 2019-12-09 21:50:32.000000 itsxpress-1.8.0/itsxpress.egg-info/entry_points.txt
--rw-r--r--   0 rivers     (501) staff       (20)       16 2019-12-09 21:50:32.000000 itsxpress-1.8.0/itsxpress.egg-info/requires.txt
--rw-r--r--   0 rivers     (501) staff       (20)       10 2019-12-09 21:50:32.000000 itsxpress-1.8.0/itsxpress.egg-info/top_level.txt
--rw-r--r--   0 rivers     (501) staff       (20)        1 2019-12-09 21:50:32.000000 itsxpress-1.8.0/itsxpress.egg-info/dependency_links.txt
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-09 21:50:33.000000 itsxpress-1.8.0/tests/
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-09 21:50:33.000000 itsxpress-1.8.0/tests/test_data/
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-09 21:50:33.000000 itsxpress-1.8.0/tests/test_data/ex_tmpdir/
--rw-r--r--   0 rivers     (501) staff       (20)    58647 2018-07-06 13:27:29.000000 itsxpress-1.8.0/tests/test_data/ex_tmpdir/rep.fa
--rw-r--r--   0 rivers     (501) staff       (20)    27444 2018-07-06 13:27:29.000000 itsxpress-1.8.0/tests/test_data/ex_tmpdir/uc.txt
--rw-r--r--   0 rivers     (501) staff       (20)    54890 2019-12-09 21:35:37.000000 itsxpress-1.8.0/tests/test_data/ex_tmpdir/rep-rc.fa
--rw-r--r--   0 rivers     (501) staff       (20)    22268 2018-07-06 13:27:29.000000 itsxpress-1.8.0/tests/test_data/ex_tmpdir/seq.fq.gz
--rw-r--r--   0 rivers     (501) staff       (20)  5383207 2018-07-06 13:27:29.000000 itsxpress-1.8.0/tests/test_data/ex_tmpdir/domtbl.txt
--rw-r--r--   0 rivers     (501) staff       (20)      357 2018-10-24 16:36:50.000000 itsxpress-1.8.0/tests/test_data/ITSxpress.log
--rw-r--r--   0 rivers     (501) staff       (20)    68703 2019-12-09 21:35:37.000000 itsxpress-1.8.0/tests/test_data/t2_r1.fq
--rw-r--r--   0 rivers     (501) staff       (20)     6148 2018-12-12 01:21:24.000000 itsxpress-1.8.0/tests/test_data/.DS_Store
--rw-r--r--   0 rivers     (501) staff       (20)      869 2018-07-06 13:27:29.000000 itsxpress-1.8.0/tests/test_data/broken.fastq
--rw-r--r--   0 rivers     (501) staff       (20)    99019 2018-07-06 13:27:29.000000 itsxpress-1.8.0/tests/test_data/testout.fastq
--rw-r--r--   0 rivers     (501) staff       (20)    21098 2018-07-25 18:27:16.000000 itsxpress-1.8.0/tests/test_data/4774-1-MSITS3_R1.fastq.gz
--rw-r--r--   0 rivers     (501) staff       (20)   139915 2018-09-10 14:55:58.000000 itsxpress-1.8.0/tests/test_data/4774-1-MSITS3_R1.fastq
--rw-r--r--   0 rivers     (501) staff       (20)   184296 2018-07-06 13:27:29.000000 itsxpress-1.8.0/tests/test_data/4774-1-MSITS3_merged.fastq
--rw-r--r--   0 rivers     (501) staff       (20)   279956 2018-07-06 13:27:29.000000 itsxpress-1.8.0/tests/test_data/4774-1-MSITS3_interleaved.fastq
--rw-r--r--   0 rivers     (501) staff       (20)      374 2018-07-25 18:28:33.000000 itsxpress-1.8.0/tests/test_data/broken.fastq.gz
--rw-r--r--   0 rivers     (501) staff       (20)   140041 2018-09-10 14:56:06.000000 itsxpress-1.8.0/tests/test_data/4774-1-MSITS3_R2.fastq
--rw-r--r--   0 rivers     (501) staff       (20)    99471 2019-07-30 20:52:23.000000 itsxpress-1.8.0/tests/test_data/t2_r2.fq
--rw-r--r--   0 rivers     (501) staff       (20)    29912 2018-07-25 18:27:23.000000 itsxpress-1.8.0/tests/test_data/4774-1-MSITS3_R2.fastq.gz
--rw-r--r--   0 rivers     (501) staff       (20)      115 2019-12-09 21:28:44.000000 itsxpress-1.8.0/MANIFEST.in
--rw-r--r--   0 rivers     (501) staff       (20)     1057 2019-12-09 21:35:37.000000 itsxpress-1.8.0/setup.py
--rw-r--r--   0 rivers     (501) staff       (20)       38 2019-12-09 21:50:33.000000 itsxpress-1.8.0/setup.cfg
--rw-r--r--   0 rivers     (501) staff       (20)     7573 2019-12-09 21:49:56.000000 itsxpress-1.8.0/README.rst
--rw-r--r--   0 rivers     (501) staff       (20)     6909 2018-08-31 16:40:22.000000 itsxpress-1.8.0/LICENSE.txt
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-05-25 19:03:34.410313 itsxpress-1.8.1/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     6909 2023-02-17 17:30:32.000000 itsxpress-1.8.1/LICENSE.txt
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      115 2023-02-17 17:30:32.000000 itsxpress-1.8.1/MANIFEST.in
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    20650 2023-05-25 19:03:34.410313 itsxpress-1.8.1/PKG-INFO
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    12166 2023-05-25 18:48:44.000000 itsxpress-1.8.1/README.rst
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-05-25 19:03:34.342312 itsxpress-1.8.1/itsxpress/
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-05-25 19:03:34.342312 itsxpress-1.8.1/itsxpress/ITSx_db/
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-05-25 19:03:34.374313 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)   754700 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/A.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)   128601 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/B.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)   171599 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/C.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)   214397 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/D.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)   120052 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/E.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)  4615535 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/F.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)   487925 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/G.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)   205812 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/H.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    42875 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/I.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)   334620 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/L.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)  3035909 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/M.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)   608925 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/O.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    85766 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/P.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    60046 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/Q.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)   351565 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/R.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    68619 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/S.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)  1922155 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/T.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    34311 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/U.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000) 13243412 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/all.hmm
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       85 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/__init__.py
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     1519 2023-02-17 17:30:32.000000 itsxpress-1.8.1/itsxpress/definitions.py
+-rwxrwxr-x   0 sveinn    (1000) sveinn    (1000)    34694 2023-04-05 15:02:23.000000 itsxpress-1.8.1/itsxpress/main.py
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-05-25 19:03:34.342312 itsxpress-1.8.1/itsxpress.egg-info/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    20650 2023-05-25 19:03:34.000000 itsxpress-1.8.1/itsxpress.egg-info/PKG-INFO
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     1455 2023-05-25 19:03:34.000000 itsxpress-1.8.1/itsxpress.egg-info/SOURCES.txt
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)        1 2023-05-25 19:03:34.000000 itsxpress-1.8.1/itsxpress.egg-info/dependency_links.txt
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       50 2023-05-25 19:03:34.000000 itsxpress-1.8.1/itsxpress.egg-info/entry_points.txt
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       47 2023-05-25 19:03:34.000000 itsxpress-1.8.1/itsxpress.egg-info/requires.txt
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       10 2023-05-25 19:03:34.000000 itsxpress-1.8.1/itsxpress.egg-info/top_level.txt
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     1102 2023-03-02 02:49:33.000000 itsxpress-1.8.1/pyproject.toml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       38 2023-05-25 19:03:34.410313 itsxpress-1.8.1/setup.cfg
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-05-25 19:03:34.394313 itsxpress-1.8.1/tests/
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-05-25 19:03:34.398313 itsxpress-1.8.1/tests/test_data/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)   139915 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_data/4774-1-MSITS3_R1.fastq
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    21098 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_data/4774-1-MSITS3_R1.fastq.gz
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)   140041 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_data/4774-1-MSITS3_R2.fastq
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    29912 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_data/4774-1-MSITS3_R2.fastq.gz
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)   279956 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_data/4774-1-MSITS3_interleaved.fastq
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)   184296 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_data/4774-1-MSITS3_merged.fastq
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      869 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_data/broken.fastq
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      374 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_data/broken.fastq.gz
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-05-25 19:03:34.410313 itsxpress-1.8.1/tests/test_data/ex_tmpdir/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)  5383207 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_data/ex_tmpdir/domtbl.txt
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    54890 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_data/ex_tmpdir/rep-rc.fa
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    58647 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_data/ex_tmpdir/rep.fa
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    22268 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_data/ex_tmpdir/seq.fq.gz
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    27444 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_data/ex_tmpdir/uc.txt
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    68703 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_data/t2_r1.fq
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    99471 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_data/t2_r2.fq
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    99019 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_data/testout.fastq
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    10459 2023-02-17 17:30:32.000000 itsxpress-1.8.1/tests/test_main.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `itsxpress-1.8.0/itsxpress/definitions.py` & `itsxpress-1.8.1/itsxpress/definitions.py`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/G.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/G.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/P.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/P.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/Q.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/Q.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/F.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/F.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/D.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/D.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/S.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/S.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/R.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/R.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/E.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/E.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/A.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/A.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/U.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/U.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/B.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/B.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/C.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/C.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/T.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/T.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/O.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/O.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/M.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/M.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/L.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/L.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/H.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/H.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/I.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/I.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/ITSx_db/HMMs/all.hmm` & `itsxpress-1.8.1/itsxpress/ITSx_db/HMMs/all.hmm`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/itsxpress/main.py` & `itsxpress-1.8.1/itsxpress/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #!/usr/bin/env python
-"""ITSxpress: A python module to rapidly trim ITS amplicon sequences from FASTQ files.
+"""##### This is the end of life version 1 of q2_itsxpress and the command line version of ITSxpress.
+The new version 2 of ITSxpress, has the Qiime2 plugin built in with command line version of ITSxpress. #####
 
-Authors: Adam Rivers, Kyle weber, USDA Agricultural Research Service
+ITSxpress: A python module to rapidly trim ITS amplicon sequences from FASTQ files.
+
+Authors: Adam Rivers, Kyle weber, Sveinn Einarsson, USDA Agricultural Research Service
 
 The internally transcribed spacer region is a region between the highly conserved small
 subunit (SSU) of rRNA and the large subunit (LSU) of the rRNA. The eukaryotic ITS contains
 the 5.8s gene and two variable length spacer regions. In amplicon sequencing studies it is
 common practice to trim off the conserved (SSU, 5,8S or LSU) regions. Bengtsson-Palme
 et al. (2013) published software the software package ITSx to do this.
 
@@ -120,15 +123,14 @@
             self.ddict[sequence][stype]["to_pos"] = to_pos
             self.ddict[sequence][stype]["from_pos"] = from_pos
             self.ddict[sequence]["tlen"] = tlen
 
 
     def parse(self):
         """Parses dom table from HMMsearch.
-
         The dom table is parsed and the start and stop position from the top scoring
         hmm math is saved. The start and stop positions of reach sequence are added to the ddict attribute.
 
         """
         try:
             with open(self.domtable, 'r') as f:
                 for num, line in enumerate(f):
@@ -497,20 +499,19 @@
             threads (int or str):the number of processor threads to use
 
         """
         try:
             self.uc_file=os.path.join(self.tempdir, 'uc.txt')
             self.rep_file=os.path.join(self.tempdir,'rep.fa')
             parameters = ["vsearch",
-                          "--derep_fulllength",
+                          "--fastx_uniques",
                           self.seq_file,
-                          "--output", self.rep_file,
+                          "--fastaout", self.rep_file,
                           "--uc", self.uc_file,
-                          "--strand", "both",
-                          "--threads", str(threads)]
+                          "--strand", "both"]
             p2 = subprocess.run(parameters, stderr=subprocess.PIPE)
             logging.info(p2.stderr.decode('utf-8'))
             p2.check_returncode()
         except subprocess.CalledProcessError as e:
             logging.exception("Could not perform dereplication with Vsearch. Error from Vsearch was:\n {}".format(p2.stderr.decode('utf-8')))
             raise e
         except FileNotFoundError as f:
@@ -744,14 +745,36 @@
             logging.error("There appears to be an issue reading the input file {}.".format(file))
             raise g
 
     core(fastq)
     if fastq2:
         core(fastq2)
 
+def _check_total_reads(file, file2 = None):
+    """Check the total number of reads in the input file(s).
+    """
+    #Count every fourth line in fastq file.
+    def core(file):
+        if file.endswith('.gz'):
+            f = gzip.open(file, 'rt')
+        else:
+            f = open(file, 'r')
+        n = 0
+        for i, line in enumerate(f):
+            if i % 4 == 0:
+                n += 1
+        f.close()
+        return n
+    
+    reads = core(file)
+    logging.info("Total number of reads in file {} is {}.".format(file, reads))
+    if file2:
+        reads = core(file2)
+        logging.info("Total number of reads in file {} is {}.".format(file2, reads))
+
 # workflow
 
 def main(args=None):
     """Run Complete ITS trimming workflow.
 
     """
     # Set up logging
@@ -803,14 +826,24 @@
             else:
                 dedup_obj.create_paired_trimmed_seqs(args.outfile, args.outfile2, gzipped=False, itspos=its_pos)
         else:
             if args.outfile.split('.')[-1] =='gz':
                 dedup_obj.create_trimmed_seqs(args.outfile, gzipped=True, itspos=its_pos)
             else:
                 dedup_obj.create_trimmed_seqs(args.outfile, gzipped=False, itspos=its_pos)
+
+        # Count reads after trimming
+        logging.info("Counting reads after trimming.")
+        if args.outfile2:
+            _check_total_reads(args.fastq, args.fastq2)
+            _check_total_reads(args.outfile, args.outfile2)
+        else:
+            _check_total_reads(args.fastq)
+            _check_total_reads(args.outfile)
+
         t1 = time.time()
         fmttime = time.strftime("%H:%M:%S", time.gmtime(t1-t0))
         logging.info("ITSxpress ran in {}".format(fmttime))
     except Exception as e:
         logging.error("ITSxpress terminated with errors. See the log file for details.")
         logging.error(e)
         raise SystemExit(1)
```

### Comparing `itsxpress-1.8.0/itsxpress.egg-info/SOURCES.txt` & `itsxpress-1.8.1/itsxpress.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
-setup.py
+pyproject.toml
 itsxpress/__init__.py
 itsxpress/definitions.py
 itsxpress/main.py
 itsxpress.egg-info/PKG-INFO
 itsxpress.egg-info/SOURCES.txt
 itsxpress.egg-info/dependency_links.txt
 itsxpress.egg-info/entry_points.txt
-itsxpress.egg-info/not-zip-safe
 itsxpress.egg-info/requires.txt
 itsxpress.egg-info/top_level.txt
 itsxpress/ITSx_db/HMMs/A.hmm
 itsxpress/ITSx_db/HMMs/B.hmm
 itsxpress/ITSx_db/HMMs/C.hmm
 itsxpress/ITSx_db/HMMs/D.hmm
 itsxpress/ITSx_db/HMMs/E.hmm
@@ -27,22 +26,21 @@
 itsxpress/ITSx_db/HMMs/P.hmm
 itsxpress/ITSx_db/HMMs/Q.hmm
 itsxpress/ITSx_db/HMMs/R.hmm
 itsxpress/ITSx_db/HMMs/S.hmm
 itsxpress/ITSx_db/HMMs/T.hmm
 itsxpress/ITSx_db/HMMs/U.hmm
 itsxpress/ITSx_db/HMMs/all.hmm
-tests/test_data/.DS_Store
+tests/test_main.py
 tests/test_data/4774-1-MSITS3_R1.fastq
 tests/test_data/4774-1-MSITS3_R1.fastq.gz
 tests/test_data/4774-1-MSITS3_R2.fastq
 tests/test_data/4774-1-MSITS3_R2.fastq.gz
 tests/test_data/4774-1-MSITS3_interleaved.fastq
 tests/test_data/4774-1-MSITS3_merged.fastq
-tests/test_data/ITSxpress.log
 tests/test_data/broken.fastq
 tests/test_data/broken.fastq.gz
 tests/test_data/t2_r1.fq
 tests/test_data/t2_r2.fq
 tests/test_data/testout.fastq
 tests/test_data/ex_tmpdir/domtbl.txt
 tests/test_data/ex_tmpdir/rep-rc.fa
```

### Comparing `itsxpress-1.8.0/tests/test_data/ex_tmpdir/rep.fa` & `itsxpress-1.8.1/tests/test_data/ex_tmpdir/rep.fa`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/tests/test_data/ex_tmpdir/uc.txt` & `itsxpress-1.8.1/tests/test_data/ex_tmpdir/uc.txt`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/tests/test_data/ex_tmpdir/rep-rc.fa` & `itsxpress-1.8.1/tests/test_data/ex_tmpdir/rep-rc.fa`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/tests/test_data/ex_tmpdir/seq.fq.gz` & `itsxpress-1.8.1/tests/test_data/ex_tmpdir/seq.fq.gz`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/tests/test_data/ex_tmpdir/domtbl.txt` & `itsxpress-1.8.1/tests/test_data/ex_tmpdir/domtbl.txt`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/tests/test_data/t2_r1.fq` & `itsxpress-1.8.1/tests/test_data/t2_r1.fq`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/tests/test_data/broken.fastq` & `itsxpress-1.8.1/tests/test_data/broken.fastq`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/tests/test_data/testout.fastq` & `itsxpress-1.8.1/tests/test_data/testout.fastq`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/tests/test_data/4774-1-MSITS3_R1.fastq.gz` & `itsxpress-1.8.1/tests/test_data/4774-1-MSITS3_R1.fastq.gz`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/tests/test_data/4774-1-MSITS3_R1.fastq` & `itsxpress-1.8.1/tests/test_data/4774-1-MSITS3_R1.fastq`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/tests/test_data/4774-1-MSITS3_merged.fastq` & `itsxpress-1.8.1/tests/test_data/4774-1-MSITS3_merged.fastq`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/tests/test_data/4774-1-MSITS3_interleaved.fastq` & `itsxpress-1.8.1/tests/test_data/4774-1-MSITS3_interleaved.fastq`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/tests/test_data/4774-1-MSITS3_R2.fastq` & `itsxpress-1.8.1/tests/test_data/4774-1-MSITS3_R2.fastq`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/tests/test_data/t2_r2.fq` & `itsxpress-1.8.1/tests/test_data/t2_r2.fq`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/tests/test_data/4774-1-MSITS3_R2.fastq.gz` & `itsxpress-1.8.1/tests/test_data/4774-1-MSITS3_R2.fastq.gz`

 * *Files identical despite different names*

### Comparing `itsxpress-1.8.0/LICENSE.txt` & `itsxpress-1.8.1/LICENSE.txt`

 * *Files identical despite different names*

