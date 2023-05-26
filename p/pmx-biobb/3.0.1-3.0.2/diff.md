# Comparing `tmp/pmx_biobb-3.0.1.tar.gz` & `tmp/pmx_biobb-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pmx_biobb-3.0.1.tar", last modified: Fri May 26 09:02:36 2023, max compression
+gzip compressed data, was "dist/pmx_biobb-3.0.2.tar", last modified: Fri May 26 09:59:53 2023, max compression
```

## Comparing `pmx_biobb-3.0.1.tar` & `pmx_biobb-3.0.2.tar`

### file list

```diff
@@ -1,318 +1,318 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:36.000000 pmx_biobb-3.0.1/
--rw-r--r--   0 pau        (501) staff       (20)     7651 2023-04-25 13:43:32.000000 pmx_biobb-3.0.1/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)       95 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/MANIFEST.in
--rw-r--r--   0 pau        (501) staff       (20)     2860 2023-05-26 09:02:36.000000 pmx_biobb-3.0.1/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     2255 2023-04-25 14:02:40.000000 pmx_biobb-3.0.1/README.rst
--rw-r--r--   0 pau        (501) staff       (20)      194 2023-05-26 09:02:36.000000 pmx_biobb-3.0.1/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     2159 2023-05-26 09:00:14.000000 pmx_biobb-3.0.1/setup.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:35.000000 pmx_biobb-3.0.1/src/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:36.000000 pmx_biobb-3.0.1/src/pmx/
--rw-r--r--   0 pau        (501) staff       (20)     2261 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)      459 2023-05-26 09:02:36.000000 pmx_biobb-3.0.1/src/pmx/_version.py
--rw-r--r--   0 pau        (501) staff       (20)    80750 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/alchemy.py
--rw-r--r--   0 pau        (501) staff       (20)    13155 2023-05-25 09:43:30.000000 pmx_biobb-3.0.1/src/pmx/analysis.py
--rw-r--r--   0 pau        (501) staff       (20)    15992 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/atom.py
--rw-r--r--   0 pau        (501) staff       (20)    14221 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/atomselection.py
--rw-r--r--   0 pau        (501) staff       (20)    13429 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/builder.py
--rw-r--r--   0 pau        (501) staff       (20)    34519 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/chain.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:35.000000 pmx_biobb-3.0.1/src/pmx/data/
--rw-r--r--   0 pau        (501) staff       (20)   233765 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/aminoacids.pkl
--rw-r--r--   0 pau        (501) staff       (20) 17363760 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/bbdep.pkl
--rw-r--r--   0 pau        (501) staff       (20)     1786 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/blosum62_new.mat
--rw-r--r--   0 pau        (501) staff       (20)   144604 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/bp.pkl
--rw-r--r--   0 pau        (501) staff       (20)   149219 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/bp_amber.pkl
--rw-r--r--   0 pau        (501) staff       (20)   148935 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/bp_charmm.pkl
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:35.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:35.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/
--rw-r--r--   0 pau        (501) staff       (20)      661 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/Makefile.am
--rw-r--r--   0 pau        (501) staff       (20)    12694 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/Makefile.in
--rw-r--r--   0 pau        (501) staff       (20)     9997 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     8884 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      849 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)    80500 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5207 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     5339 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    66560 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     8192 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)       79 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      947 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1948 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3882 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)  3071584 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1260735 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:35.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)    21524 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)     2589 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9412 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      903 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)   101863 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5207 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     5335 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    36227 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp
--rw-r--r--   0 pau        (501) staff       (20)  1202088 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres
--rw-r--r--   0 pau        (501) staff       (20)    36132 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      130 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    10830 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp
--rw-r--r--   0 pau        (501) staff       (20)    45478 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     7972 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      722 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      974 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1949 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3886 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)  2805564 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1181333 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)   300774 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp
--rw-r--r--   0 pau        (501) staff       (20)   129919 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    16346 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp
--rw-r--r--   0 pau        (501) staff       (20)    18595 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:35.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)     2589 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9412 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      903 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)   101863 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5207 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     4978 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    36227 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_ffbonded_for_ildn_test.itp
--rw-r--r--   0 pau        (501) staff       (20)  1202088 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_mutres
--rw-r--r--   0 pau        (501) staff       (20)    36132 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/correct_ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    10830 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffberger.itp
--rw-r--r--   0 pau        (501) staff       (20)    36132 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     7476 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      709 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      974 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1949 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3886 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)  2805564 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1181333 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)   300774 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.mtp
--rw-r--r--   0 pau        (501) staff       (20)   129937 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    16346 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer.itp
--rw-r--r--   0 pau        (501) staff       (20)    18595 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer_posre.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:35.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)     9997 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9416 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      903 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)   104467 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5207 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     4652 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    36127 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     6772 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      704 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      951 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1948 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3886 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)  3290968 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1389335 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/watermodels.dat
--rw-r--r--   0 pau        (501) staff       (20)     3873 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/atommass.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:35.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)       84 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)     2060 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     8026 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)     1519 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      181 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)    44420 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     6253 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)    13027 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    37937 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/cmap.itp
--rw-r--r--   0 pau        (501) staff       (20)      244 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)      261 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/dna.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     1660 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      265 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/dna.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9612 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    88617 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)    74128 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ffnabonded.itp
--rw-r--r--   0 pau        (501) staff       (20)    47717 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ffnanonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)   144554 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     2792 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)     1208 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     2882 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/gb.itp
--rw-r--r--   0 pau        (501) staff       (20)     1767 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)        0 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/lipids.hdb
--rw-r--r--   0 pau        (501) staff       (20)    48593 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/lipids.rtp
--rw-r--r--   0 pau        (501) staff       (20)       70 2023-04-25 13:50:06.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/mutres.arn
--rw-r--r--   0 pau        (501) staff       (20)  2828420 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1165390 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)      164 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)      261 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/rna.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     1884 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      265 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/rna.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      126 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)     9712 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      910 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      916 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)     1369 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1419 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1576 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     2237 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)      915 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tips3p.itp
--rw-r--r--   0 pau        (501) staff       (20)      306 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:36.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)    24002 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    82367 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/cmap.itp
--rw-r--r--   0 pau        (501) staff       (20)  1123865 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)  1614095 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     7941 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      435 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     2734 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/gb.itp
--rw-r--r--   0 pau        (501) staff       (20)     2079 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)       92 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.arn
--rw-r--r--   0 pau        (501) staff       (20)     1134 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     8979 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.hdb
--rw-r--r--   0 pau        (501) staff       (20)     1397 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      198 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.r2b
--rw-r--r--   0 pau        (501) staff       (20)  1133668 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5220 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.vsd
--rw-r--r--   0 pau        (501) staff       (20)       92 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres.arn
--rw-r--r--   0 pau        (501) staff       (20)  3015999 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1267062 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)   283035 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.mtp
--rw-r--r--   0 pau        (501) staff       (20)   123173 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)     1339 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/nbfix.itp
--rw-r--r--   0 pau        (501) staff       (20)      619 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      625 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)     1026 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1242 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)      221 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/watermodels.dat
--rw-r--r--   0 pau        (501) staff       (20)     3940 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/elements.dat
--rw-r--r--   0 pau        (501) staff       (20)    10624 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/residuetypes.dat
--rw-r--r--   0 pau        (501) staff       (20)    29266 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/spc216.gro
--rw-r--r--   0 pau        (501) staff       (20)      343 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/specbond.dat
--rw-r--r--   0 pau        (501) staff       (20)      848 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/vdwradii.dat
--rw-r--r--   0 pau        (501) staff       (20)      447 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/mutff/xlateat.dat
--rw-r--r--   0 pau        (501) staff       (20)    70529 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/data/rna.pkl
--rw-r--r--   0 pau        (501) staff       (20)    36875 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/estimators.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:35.000000 pmx_biobb-3.0.1/src/pmx/extensions/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:36.000000 pmx_biobb-3.0.1/src/pmx/extensions/pmx/
--rw-r--r--   0 pau        (501) staff       (20)    13896 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/extensions/pmx/Energy.c
--rw-r--r--   0 pau        (501) staff       (20)    15145 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/extensions/pmx/Geometry.c
--rw-r--r--   0 pau        (501) staff       (20)    20514 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/extensions/pmx/Geometry.h
--rw-r--r--   0 pau        (501) staff       (20)     2086 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/extensions/pmx/cpp_test.cpp
--rw-r--r--   0 pau        (501) staff       (20)     3939 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/extensions/pmx/init.c
--rw-r--r--   0 pau        (501) staff       (20)     4662 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/extensions/pmx/pmx.h
--rw-r--r--   0 pau        (501) staff       (20)    17556 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/extensions/pmx/wrap_Geometry.c
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:36.000000 pmx_biobb-3.0.1/src/pmx/extensions/xdr/
--rw-r--r--   0 pau        (501) staff       (20)     8847 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/extensions/xdr/trr2xtc.c
--rw-r--r--   0 pau        (501) staff       (20)    64408 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/extensions/xdr/xdrfile.c
--rw-r--r--   0 pau        (501) staff       (20)    23730 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/extensions/xdr/xdrfile.h
--rw-r--r--   0 pau        (501) staff       (20)    13474 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/extensions/xdr/xdrfile_c_test.c
--rw-r--r--   0 pau        (501) staff       (20)    14744 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/extensions/xdr/xdrfile_trr.c
--rw-r--r--   0 pau        (501) staff       (20)     2364 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/extensions/xdr/xdrfile_trr.h
--rw-r--r--   0 pau        (501) staff       (20)     3629 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/extensions/xdr/xdrfile_xtc.c
--rw-r--r--   0 pau        (501) staff       (20)     2255 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/extensions/xdr/xdrfile_xtc.h
--rw-r--r--   0 pau        (501) staff       (20)    29075 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/ffparser.py
--rw-r--r--   0 pau        (501) staff       (20)    97348 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/forcefield.py
--rw-r--r--   0 pau        (501) staff       (20)     7685 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/geometry.py
--rw-r--r--   0 pau        (501) staff       (20)     8707 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/gmx.py
--rw-r--r--   0 pau        (501) staff       (20)     6179 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/jobscript.py
--rw-r--r--   0 pau        (501) staff       (20)   123096 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/library.py
--rw-r--r--   0 pau        (501) staff       (20)   117960 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/ligand_alchemy.py
--rw-r--r--   0 pau        (501) staff       (20)    46038 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/model.py
--rw-r--r--   0 pau        (501) staff       (20)    28167 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/molecule.py
--rw-r--r--   0 pau        (501) staff       (20)     7345 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/mutdb.py
--rw-r--r--   0 pau        (501) staff       (20)     8874 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/ndx.py
--rw-r--r--   0 pau        (501) staff       (20)    16599 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/options.py
--rw-r--r--   0 pau        (501) staff       (20)     5036 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/parser.py
--rw-r--r--   0 pau        (501) staff       (20)    21628 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/rosetta.py
--rw-r--r--   0 pau        (501) staff       (20)    15211 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/rosetta_analyze.py
--rw-r--r--   0 pau        (501) staff       (20)    11783 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/rotamer.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:36.000000 pmx_biobb-3.0.1/src/pmx/scripts/
--rw-r--r--   0 pau        (501) staff       (20)        0 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/scripts/__init__.py
--rwxr-xr-x   0 pau        (501) staff       (20)    32259 2023-05-25 09:45:33.000000 pmx_biobb-3.0.1/src/pmx/scripts/analyze_dhdl.py
--rwxr-xr-x   0 pau        (501) staff       (20)    19768 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/scripts/atomMapping.py
--rwxr-xr-x   0 pau        (501) staff       (20)    11939 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/scripts/build_cyclic_top.py
--rwxr-xr-x   0 pau        (501) staff       (20)     2988 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/scripts/cli.py
--rwxr-xr-x   0 pau        (501) staff       (20)    73999 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/scripts/generate_hybrid_residue.py
--rwxr-xr-x   0 pau        (501) staff       (20)     6989 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/scripts/generate_hybrid_topology.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:36.000000 pmx_biobb-3.0.1/src/pmx/scripts/icolos_entrypoints/
--rw-r--r--   0 pau        (501) staff       (20)        0 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/scripts/icolos_entrypoints/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)     7137 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/scripts/icolos_entrypoints/assemble_systems.py
--rwxr-xr-x   0 pau        (501) staff       (20)    12867 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/scripts/ligandHybrid.py
--rwxr-xr-x   0 pau        (501) staff       (20)     2705 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/scripts/make_double_box.py
--rw-r--r--   0 pau        (501) staff       (20)    19698 2023-05-12 10:00:20.000000 pmx_biobb-3.0.1/src/pmx/scripts/md_setup.py
--rwxr-xr-x   0 pau        (501) staff       (20)    23029 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/scripts/mutate.py
--rw-r--r--   0 pau        (501) staff       (20)     7795 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/scripts/prepare_crooks_runs.py
--rwxr-xr-x   0 pau        (501) staff       (20)     1475 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/scripts/set_gmxlib.py
--rw-r--r--   0 pau        (501) staff       (20)    17636 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/scripts/setup_abfe.py
--rw-r--r--   0 pau        (501) staff       (20)    15258 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/utils.py
--rw-r--r--   0 pau        (501) staff       (20)    11331 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/xdrfile.py
--rw-r--r--   0 pau        (501) staff       (20)     1784 2023-04-25 13:50:07.000000 pmx_biobb-3.0.1/src/pmx/xtc.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:02:36.000000 pmx_biobb-3.0.1/src/pmx_biobb.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     2860 2023-05-26 09:02:35.000000 pmx_biobb-3.0.1/src/pmx_biobb.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)    14242 2023-05-26 09:02:35.000000 pmx_biobb-3.0.1/src/pmx_biobb.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-05-26 09:02:35.000000 pmx_biobb-3.0.1/src/pmx_biobb.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)       53 2023-05-26 09:02:35.000000 pmx_biobb-3.0.1/src/pmx_biobb.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-04-26 11:15:51.000000 pmx_biobb-3.0.1/src/pmx_biobb.egg-info/not-zip-safe
--rw-r--r--   0 pau        (501) staff       (20)       12 2023-05-26 09:02:35.000000 pmx_biobb-3.0.1/src/pmx_biobb.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)        4 2023-05-26 09:02:35.000000 pmx_biobb-3.0.1/src/pmx_biobb.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)    65955 2023-05-26 09:00:14.000000 pmx_biobb-3.0.1/versioneer.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/
+-rw-r--r--   0 pau        (501) staff       (20)     7651 2023-04-25 13:43:32.000000 pmx_biobb-3.0.2/LICENSE
+-rw-r--r--   0 pau        (501) staff       (20)       95 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/MANIFEST.in
+-rw-r--r--   0 pau        (501) staff       (20)     2860 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     2255 2023-04-25 14:02:40.000000 pmx_biobb-3.0.2/README.rst
+-rw-r--r--   0 pau        (501) staff       (20)      194 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     2159 2023-05-26 09:53:14.000000 pmx_biobb-3.0.2/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx/
+-rw-r--r--   0 pau        (501) staff       (20)     2261 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)      459 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx/_version.py
+-rw-r--r--   0 pau        (501) staff       (20)    80750 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/alchemy.py
+-rw-r--r--   0 pau        (501) staff       (20)    13155 2023-05-25 09:43:30.000000 pmx_biobb-3.0.2/src/pmx/analysis.py
+-rw-r--r--   0 pau        (501) staff       (20)    15992 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/atom.py
+-rw-r--r--   0 pau        (501) staff       (20)    14221 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/atomselection.py
+-rw-r--r--   0 pau        (501) staff       (20)    13429 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/builder.py
+-rw-r--r--   0 pau        (501) staff       (20)    34519 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/chain.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx/data/
+-rw-r--r--   0 pau        (501) staff       (20)   233765 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/aminoacids.pkl
+-rw-r--r--   0 pau        (501) staff       (20) 17363760 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/bbdep.pkl
+-rw-r--r--   0 pau        (501) staff       (20)     1786 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/blosum62_new.mat
+-rw-r--r--   0 pau        (501) staff       (20)   144604 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/bp.pkl
+-rw-r--r--   0 pau        (501) staff       (20)   149219 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/bp_amber.pkl
+-rw-r--r--   0 pau        (501) staff       (20)   148935 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/bp_charmm.pkl
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)      661 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/Makefile.am
+-rw-r--r--   0 pau        (501) staff       (20)    12694 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/Makefile.in
+-rw-r--r--   0 pau        (501) staff       (20)     9997 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.arn
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     8884 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      849 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    80500 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     5207 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.vsd
+-rw-r--r--   0 pau        (501) staff       (20)     5339 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/atomtypes.atp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/dna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     3104 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/dna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/dna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    29892 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    66560 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)     8192 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/ffnonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)       79 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/forcefield.doc
+-rw-r--r--   0 pau        (501) staff       (20)      947 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1948 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/gbsa.itp
+-rw-r--r--   0 pau        (501) staff       (20)     3882 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)  3071584 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/mutres.mtp
+-rw-r--r--   0 pau        (501) staff       (20)  1260735 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/mutres.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/rna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     4104 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/rna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/rna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    30277 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/rna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)      802 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1261 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1317 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/tip4pew.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1870 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/tip5p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1250 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/urea.itp
+-rw-r--r--   0 pau        (501) staff       (20)      214 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)    21524 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn
+-rw-r--r--   0 pau        (501) staff       (20)     2589 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     9412 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      903 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b
+-rw-r--r--   0 pau        (501) staff       (20)   101863 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     5207 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd
+-rw-r--r--   0 pau        (501) staff       (20)     5335 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp
+-rw-r--r--   0 pau        (501) staff       (20)    36227 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp
+-rw-r--r--   0 pau        (501) staff       (20)  1202088 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres
+-rw-r--r--   0 pau        (501) staff       (20)    36132 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)      130 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     3104 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    29892 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    10830 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp
+-rw-r--r--   0 pau        (501) staff       (20)    45478 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)     7972 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)      722 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.doc
+-rw-r--r--   0 pau        (501) staff       (20)      974 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1949 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp
+-rw-r--r--   0 pau        (501) staff       (20)     3886 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)  2805564 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp
+-rw-r--r--   0 pau        (501) staff       (20)  1181333 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp
+-rw-r--r--   0 pau        (501) staff       (20)   300774 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp
+-rw-r--r--   0 pau        (501) staff       (20)   129919 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    16346 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp
+-rw-r--r--   0 pau        (501) staff       (20)    18595 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     4104 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    30277 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)      802 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1261 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1317 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1870 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1250 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/urea.itp
+-rw-r--r--   0 pau        (501) staff       (20)      214 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)     2589 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.arn
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     9412 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      903 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.r2b
+-rw-r--r--   0 pau        (501) staff       (20)   101863 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     5207 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.vsd
+-rw-r--r--   0 pau        (501) staff       (20)     4978 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/atomtypes.atp
+-rw-r--r--   0 pau        (501) staff       (20)    36227 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_ffbonded_for_ildn_test.itp
+-rw-r--r--   0 pau        (501) staff       (20)  1202088 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_mutres
+-rw-r--r--   0 pau        (501) staff       (20)    36132 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/correct_ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     3104 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    29892 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    10830 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffberger.itp
+-rw-r--r--   0 pau        (501) staff       (20)    36132 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)     7476 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffnonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)      709 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.doc
+-rw-r--r--   0 pau        (501) staff       (20)      974 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1949 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/gbsa.itp
+-rw-r--r--   0 pau        (501) staff       (20)     3886 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)  2805564 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.mtp
+-rw-r--r--   0 pau        (501) staff       (20)  1181333 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.rtp
+-rw-r--r--   0 pau        (501) staff       (20)   300774 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.mtp
+-rw-r--r--   0 pau        (501) staff       (20)   129937 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    16346 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer.itp
+-rw-r--r--   0 pau        (501) staff       (20)    18595 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer_posre.itp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     4104 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    30277 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)      802 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1261 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1317 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4pew.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1870 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip5p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1250 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/urea.itp
+-rw-r--r--   0 pau        (501) staff       (20)      214 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)     9997 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.arn
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     9416 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      903 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.r2b
+-rw-r--r--   0 pau        (501) staff       (20)   104467 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     5207 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.vsd
+-rw-r--r--   0 pau        (501) staff       (20)     4652 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/atomtypes.atp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     3104 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    29892 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    36127 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)     6772 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffnonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)      704 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.doc
+-rw-r--r--   0 pau        (501) staff       (20)      951 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1948 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/gbsa.itp
+-rw-r--r--   0 pau        (501) staff       (20)     3886 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)  3290968 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.mtp
+-rw-r--r--   0 pau        (501) staff       (20)  1389335 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     4104 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    30277 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)      802 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1261 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1317 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4pew.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1870 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip5p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1250 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/urea.itp
+-rw-r--r--   0 pau        (501) staff       (20)      214 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/watermodels.dat
+-rw-r--r--   0 pau        (501) staff       (20)     3873 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/atommass.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)       84 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.arn
+-rw-r--r--   0 pau        (501) staff       (20)     2060 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     8026 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)     1519 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      181 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    44420 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     6253 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.vsd
+-rw-r--r--   0 pau        (501) staff       (20)    13027 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/atomtypes.atp
+-rw-r--r--   0 pau        (501) staff       (20)    37937 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/cmap.itp
+-rw-r--r--   0 pau        (501) staff       (20)      244 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.arn
+-rw-r--r--   0 pau        (501) staff       (20)      261 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     1660 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      265 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     9612 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    88617 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)    74128 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/ffnabonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)    47717 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/ffnanonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)   144554 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/ffnonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)     2792 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.doc
+-rw-r--r--   0 pau        (501) staff       (20)     1208 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     2882 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/gb.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1767 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)        0 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/lipids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)    48593 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/lipids.rtp
+-rw-r--r--   0 pau        (501) staff       (20)       70 2023-04-25 13:50:06.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/mutres.arn
+-rw-r--r--   0 pau        (501) staff       (20)  2828420 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/mutres.mtp
+-rw-r--r--   0 pau        (501) staff       (20)  1165390 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/mutres.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      164 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.arn
+-rw-r--r--   0 pau        (501) staff       (20)      261 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     1884 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      265 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      126 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)     9712 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      910 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      916 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1369 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1419 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1576 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/tip4pew.itp
+-rw-r--r--   0 pau        (501) staff       (20)     2237 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/tip5p.itp
+-rw-r--r--   0 pau        (501) staff       (20)      915 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/tips3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)      306 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)    24002 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/atomtypes.atp
+-rw-r--r--   0 pau        (501) staff       (20)    82367 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/cmap.itp
+-rw-r--r--   0 pau        (501) staff       (20)  1123865 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)  1614095 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/ffnonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)     7941 2023-05-26 09:58:36.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.doc
+-rw-r--r--   0 pau        (501) staff       (20)      435 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     2734 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/gb.itp
+-rw-r--r--   0 pau        (501) staff       (20)     2079 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)       92 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.arn
+-rw-r--r--   0 pau        (501) staff       (20)     1134 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     8979 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.hdb
+-rw-r--r--   0 pau        (501) staff       (20)     1397 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      198 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.r2b
+-rw-r--r--   0 pau        (501) staff       (20)  1133668 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     5220 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.vsd
+-rw-r--r--   0 pau        (501) staff       (20)       92 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres.arn
+-rw-r--r--   0 pau        (501) staff       (20)  3015999 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres.mtp
+-rw-r--r--   0 pau        (501) staff       (20)  1267062 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres.rtp
+-rw-r--r--   0 pau        (501) staff       (20)   283035 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.mtp
+-rw-r--r--   0 pau        (501) staff       (20)   123173 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     1339 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/nbfix.itp
+-rw-r--r--   0 pau        (501) staff       (20)      619 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      625 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1026 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1242 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)      221 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/watermodels.dat
+-rw-r--r--   0 pau        (501) staff       (20)     3940 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/elements.dat
+-rw-r--r--   0 pau        (501) staff       (20)    10624 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/residuetypes.dat
+-rw-r--r--   0 pau        (501) staff       (20)    29266 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/spc216.gro
+-rw-r--r--   0 pau        (501) staff       (20)      343 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/specbond.dat
+-rw-r--r--   0 pau        (501) staff       (20)      848 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/vdwradii.dat
+-rw-r--r--   0 pau        (501) staff       (20)      447 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/mutff/xlateat.dat
+-rw-r--r--   0 pau        (501) staff       (20)    70529 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/data/rna.pkl
+-rw-r--r--   0 pau        (501) staff       (20)    36875 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/estimators.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx/extensions/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx/extensions/pmx/
+-rw-r--r--   0 pau        (501) staff       (20)    13896 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/extensions/pmx/Energy.c
+-rw-r--r--   0 pau        (501) staff       (20)    15145 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/extensions/pmx/Geometry.c
+-rw-r--r--   0 pau        (501) staff       (20)    20514 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/extensions/pmx/Geometry.h
+-rw-r--r--   0 pau        (501) staff       (20)     2086 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/extensions/pmx/cpp_test.cpp
+-rw-r--r--   0 pau        (501) staff       (20)     3939 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/extensions/pmx/init.c
+-rw-r--r--   0 pau        (501) staff       (20)     4662 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/extensions/pmx/pmx.h
+-rw-r--r--   0 pau        (501) staff       (20)    17556 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/extensions/pmx/wrap_Geometry.c
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx/extensions/xdr/
+-rw-r--r--   0 pau        (501) staff       (20)     8847 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/extensions/xdr/trr2xtc.c
+-rw-r--r--   0 pau        (501) staff       (20)    64408 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/extensions/xdr/xdrfile.c
+-rw-r--r--   0 pau        (501) staff       (20)    23730 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/extensions/xdr/xdrfile.h
+-rw-r--r--   0 pau        (501) staff       (20)    13474 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/extensions/xdr/xdrfile_c_test.c
+-rw-r--r--   0 pau        (501) staff       (20)    14744 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/extensions/xdr/xdrfile_trr.c
+-rw-r--r--   0 pau        (501) staff       (20)     2364 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/extensions/xdr/xdrfile_trr.h
+-rw-r--r--   0 pau        (501) staff       (20)     3629 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/extensions/xdr/xdrfile_xtc.c
+-rw-r--r--   0 pau        (501) staff       (20)     2255 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/extensions/xdr/xdrfile_xtc.h
+-rw-r--r--   0 pau        (501) staff       (20)    29075 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/ffparser.py
+-rw-r--r--   0 pau        (501) staff       (20)    97348 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/forcefield.py
+-rw-r--r--   0 pau        (501) staff       (20)     7685 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/geometry.py
+-rw-r--r--   0 pau        (501) staff       (20)     8707 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/gmx.py
+-rw-r--r--   0 pau        (501) staff       (20)     6179 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/jobscript.py
+-rw-r--r--   0 pau        (501) staff       (20)   123096 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/library.py
+-rw-r--r--   0 pau        (501) staff       (20)   117960 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/ligand_alchemy.py
+-rw-r--r--   0 pau        (501) staff       (20)    46038 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/model.py
+-rw-r--r--   0 pau        (501) staff       (20)    28167 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/molecule.py
+-rw-r--r--   0 pau        (501) staff       (20)     7345 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/mutdb.py
+-rw-r--r--   0 pau        (501) staff       (20)     8874 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/ndx.py
+-rw-r--r--   0 pau        (501) staff       (20)    16599 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/options.py
+-rw-r--r--   0 pau        (501) staff       (20)     5036 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/parser.py
+-rw-r--r--   0 pau        (501) staff       (20)    21628 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/rosetta.py
+-rw-r--r--   0 pau        (501) staff       (20)    15211 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/rosetta_analyze.py
+-rw-r--r--   0 pau        (501) staff       (20)    11783 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/rotamer.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx/scripts/
+-rw-r--r--   0 pau        (501) staff       (20)        0 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/scripts/__init__.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    32259 2023-05-25 09:45:33.000000 pmx_biobb-3.0.2/src/pmx/scripts/analyze_dhdl.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    19768 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/scripts/atomMapping.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    11939 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/scripts/build_cyclic_top.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     2988 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/scripts/cli.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    73999 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/scripts/generate_hybrid_residue.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     6989 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/scripts/generate_hybrid_topology.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx/scripts/icolos_entrypoints/
+-rw-r--r--   0 pau        (501) staff       (20)        0 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/scripts/icolos_entrypoints/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)     7137 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/scripts/icolos_entrypoints/assemble_systems.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    12867 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/scripts/ligandHybrid.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     2705 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/scripts/make_double_box.py
+-rw-r--r--   0 pau        (501) staff       (20)    19712 2023-05-26 09:42:02.000000 pmx_biobb-3.0.2/src/pmx/scripts/md_setup.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    23029 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/scripts/mutate.py
+-rw-r--r--   0 pau        (501) staff       (20)     7807 2023-05-26 09:44:23.000000 pmx_biobb-3.0.2/src/pmx/scripts/prepare_crooks_runs.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     1475 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/scripts/set_gmxlib.py
+-rw-r--r--   0 pau        (501) staff       (20)    17636 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/scripts/setup_abfe.py
+-rw-r--r--   0 pau        (501) staff       (20)    15258 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/utils.py
+-rw-r--r--   0 pau        (501) staff       (20)    11331 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/xdrfile.py
+-rw-r--r--   0 pau        (501) staff       (20)     1784 2023-04-25 13:50:07.000000 pmx_biobb-3.0.2/src/pmx/xtc.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx_biobb.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     2860 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx_biobb.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)    14242 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx_biobb.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx_biobb.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)       53 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx_biobb.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-04-26 11:15:51.000000 pmx_biobb-3.0.2/src/pmx_biobb.egg-info/not-zip-safe
+-rw-r--r--   0 pau        (501) staff       (20)       12 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx_biobb.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)        4 2023-05-26 09:59:53.000000 pmx_biobb-3.0.2/src/pmx_biobb.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)    65955 2023-05-26 09:58:36.000000 pmx_biobb-3.0.2/versioneer.py
```

### Comparing `pmx_biobb-3.0.1/LICENSE` & `pmx_biobb-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/PKG-INFO` & `pmx_biobb-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmx_biobb
-Version: 3.0.1
+Version: 3.0.2
 Summary: Toolkit for free-energy calculation setup/analysis and biomolecular structure handling
 Home-page: https://github.com/deGrootLab/pmx/tree/develop
 Author: Daniel Seeliger
 Author-email: seeliger.biosoft@gmail.de
 License: GPL 3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pmx_biobb-3.0.1/README.rst` & `pmx_biobb-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/setup.py` & `pmx_biobb-3.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                   )
 extensions = [pmx, xdrio]
 
 # -----
 # Setup
 # -----
 setup(name='pmx_biobb',
-      version='3.0.1',
+      version='3.0.2',
       cmdclass=versioneer.get_cmdclass(),
       description='Toolkit for free-energy calculation setup/analysis '
                   'and biomolecular structure handling',
       long_description=readme(),
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: GNU General Public License (GPL)',
```

### Comparing `pmx_biobb-3.0.1/src/pmx/__init__.py` & `pmx_biobb-3.0.2/src/pmx/__init__.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/alchemy.py` & `pmx_biobb-3.0.2/src/pmx/alchemy.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/analysis.py` & `pmx_biobb-3.0.2/src/pmx/analysis.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/atom.py` & `pmx_biobb-3.0.2/src/pmx/atom.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/atomselection.py` & `pmx_biobb-3.0.2/src/pmx/atomselection.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/builder.py` & `pmx_biobb-3.0.2/src/pmx/builder.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/chain.py` & `pmx_biobb-3.0.2/src/pmx/chain.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/aminoacids.pkl` & `pmx_biobb-3.0.2/src/pmx/data/aminoacids.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/bbdep.pkl` & `pmx_biobb-3.0.2/src/pmx/data/bbdep.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/blosum62_new.mat` & `pmx_biobb-3.0.2/src/pmx/data/blosum62_new.mat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/bp.pkl` & `pmx_biobb-3.0.2/src/pmx/data/bp.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/bp_amber.pkl` & `pmx_biobb-3.0.2/src/pmx/data/bp_amber.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/bp_charmm.pkl` & `pmx_biobb-3.0.2/src/pmx/data/bp_charmm.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/Makefile.am` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/Makefile.am`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/Makefile.in` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/Makefile.in`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.arn` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.arn`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.hdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.r2b` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.vsd` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/atomtypes.atp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/dna.hdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/dna.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/ffbonded.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/ffnonbonded.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/forcefield.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/gbsa.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/ions.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/mutres.mtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/mutres.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/rna.hdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/rna.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/spc.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/spce.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/tip3p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/tip4p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/tip4pew.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/tip5p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber14sbmut.ff/urea.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber14sbmut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.doc` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.doc`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ions.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spc.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spce.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/urea.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.arn` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.arn`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.hdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.r2b` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.vsd` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/atomtypes.atp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_ffbonded_for_ildn_test.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_ffbonded_for_ildn_test.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_mutres` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_mutres`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/correct_ffbonded.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/correct_ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.hdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffberger.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffberger.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffbonded.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffnonbonded.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.doc` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.doc`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/gbsa.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ions.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.mtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.mtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer_posre.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer_posre.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.hdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spc.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spce.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip3p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4pew.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip5p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/urea.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.arn` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.arn`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.hdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.r2b` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.vsd` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/atomtypes.atp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.hdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffbonded.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffnonbonded.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.doc` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.doc`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/gbsa.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ions.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.mtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.hdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spc.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spce.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip3p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4pew.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip5p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/urea.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/atommass.dat` & `pmx_biobb-3.0.2/src/pmx/data/mutff/atommass.dat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.c.tdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.c.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.hdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.n.tdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.n.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.vsd` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/atomtypes.atp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/cmap.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/cmap.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/dna.hdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/dna.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ffbonded.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ffnabonded.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/ffnabonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ffnanonbonded.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/ffnanonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ffnonbonded.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.doc` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.doc`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/gb.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/gb.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ions.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/lipids.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/lipids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/mutres.mtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/mutres.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/rna.hdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/rna.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/spc.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/spce.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tip3p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tip4p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tip4pew.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tip5p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tips3p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm22star-mut.ff/tips3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/atomtypes.atp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/cmap.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/cmap.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/ffbonded.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/ffnonbonded.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.doc` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.doc`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 *                    CHARMM36 port writted by                                 *
 *                    E. Prabhu Raman, Justin A. Lemkul, Robert Best           *
 *                    and Alexander D. MacKerell, Jr.                          *
 *                    CHARMM force field homepage:                             *
 *                    www.mackerell.umaryland.edu/CHARMM_ff_params.html        *
 *******************************************************************************
 
-Parameters taken from CHARMM36 and CGenFF 3.0.1
+Parameters taken from CHARMM36 and CGenFF 3.0.2
   Included are topologies and parameters from
     top_all36_prot.rtf          par_all36m_prot.prm
     top_all36_na.rtf            par_all36_na.prm
     top_all36_lipid.rtf         par_all36_lipid.prm
     top_all36_carb.rtf          par_all36_carb.prm
     top_all36_cgenff.rtf        par_all36_cgenff.prm
     top_all35_ethers.rtf        par_all35_ethers.prm
```

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/gb.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/gb.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/ions.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.c.tdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.c.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.hdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.n.tdb` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.n.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.vsd` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres.mtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.mtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.rtp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/nbfix.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/nbfix.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/spc.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/spce.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/tip3p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/charmm36m-mut.ff/tip4p.itp` & `pmx_biobb-3.0.2/src/pmx/data/mutff/charmm36m-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/elements.dat` & `pmx_biobb-3.0.2/src/pmx/data/mutff/elements.dat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/residuetypes.dat` & `pmx_biobb-3.0.2/src/pmx/data/mutff/residuetypes.dat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/spc216.gro` & `pmx_biobb-3.0.2/src/pmx/data/mutff/spc216.gro`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/mutff/vdwradii.dat` & `pmx_biobb-3.0.2/src/pmx/data/mutff/vdwradii.dat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/data/rna.pkl` & `pmx_biobb-3.0.2/src/pmx/data/rna.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/estimators.py` & `pmx_biobb-3.0.2/src/pmx/estimators.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/extensions/pmx/Energy.c` & `pmx_biobb-3.0.2/src/pmx/extensions/pmx/Energy.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/extensions/pmx/Geometry.c` & `pmx_biobb-3.0.2/src/pmx/extensions/pmx/Geometry.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/extensions/pmx/Geometry.h` & `pmx_biobb-3.0.2/src/pmx/extensions/pmx/Geometry.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/extensions/pmx/cpp_test.cpp` & `pmx_biobb-3.0.2/src/pmx/extensions/pmx/cpp_test.cpp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/extensions/pmx/init.c` & `pmx_biobb-3.0.2/src/pmx/extensions/pmx/init.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/extensions/pmx/pmx.h` & `pmx_biobb-3.0.2/src/pmx/extensions/pmx/pmx.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/extensions/pmx/wrap_Geometry.c` & `pmx_biobb-3.0.2/src/pmx/extensions/pmx/wrap_Geometry.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/extensions/xdr/trr2xtc.c` & `pmx_biobb-3.0.2/src/pmx/extensions/xdr/trr2xtc.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/extensions/xdr/xdrfile.c` & `pmx_biobb-3.0.2/src/pmx/extensions/xdr/xdrfile.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/extensions/xdr/xdrfile.h` & `pmx_biobb-3.0.2/src/pmx/extensions/xdr/xdrfile.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/extensions/xdr/xdrfile_c_test.c` & `pmx_biobb-3.0.2/src/pmx/extensions/xdr/xdrfile_c_test.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/extensions/xdr/xdrfile_trr.c` & `pmx_biobb-3.0.2/src/pmx/extensions/xdr/xdrfile_trr.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/extensions/xdr/xdrfile_trr.h` & `pmx_biobb-3.0.2/src/pmx/extensions/xdr/xdrfile_trr.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/extensions/xdr/xdrfile_xtc.c` & `pmx_biobb-3.0.2/src/pmx/extensions/xdr/xdrfile_xtc.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/extensions/xdr/xdrfile_xtc.h` & `pmx_biobb-3.0.2/src/pmx/extensions/xdr/xdrfile_xtc.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/ffparser.py` & `pmx_biobb-3.0.2/src/pmx/ffparser.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/forcefield.py` & `pmx_biobb-3.0.2/src/pmx/forcefield.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/geometry.py` & `pmx_biobb-3.0.2/src/pmx/geometry.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/gmx.py` & `pmx_biobb-3.0.2/src/pmx/gmx.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/jobscript.py` & `pmx_biobb-3.0.2/src/pmx/jobscript.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/library.py` & `pmx_biobb-3.0.2/src/pmx/library.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/ligand_alchemy.py` & `pmx_biobb-3.0.2/src/pmx/ligand_alchemy.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/model.py` & `pmx_biobb-3.0.2/src/pmx/model.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/molecule.py` & `pmx_biobb-3.0.2/src/pmx/molecule.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/mutdb.py` & `pmx_biobb-3.0.2/src/pmx/mutdb.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/ndx.py` & `pmx_biobb-3.0.2/src/pmx/ndx.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/options.py` & `pmx_biobb-3.0.2/src/pmx/options.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/parser.py` & `pmx_biobb-3.0.2/src/pmx/parser.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/rosetta.py` & `pmx_biobb-3.0.2/src/pmx/rosetta.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/rosetta_analyze.py` & `pmx_biobb-3.0.2/src/pmx/rosetta_analyze.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/rotamer.py` & `pmx_biobb-3.0.2/src/pmx/rotamer.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/scripts/analyze_dhdl.py` & `pmx_biobb-3.0.2/src/pmx/scripts/analyze_dhdl.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/scripts/atomMapping.py` & `pmx_biobb-3.0.2/src/pmx/scripts/atomMapping.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/scripts/build_cyclic_top.py` & `pmx_biobb-3.0.2/src/pmx/scripts/build_cyclic_top.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/scripts/cli.py` & `pmx_biobb-3.0.2/src/pmx/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/scripts/generate_hybrid_residue.py` & `pmx_biobb-3.0.2/src/pmx/scripts/generate_hybrid_residue.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/scripts/generate_hybrid_topology.py` & `pmx_biobb-3.0.2/src/pmx/scripts/generate_hybrid_topology.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/scripts/icolos_entrypoints/assemble_systems.py` & `pmx_biobb-3.0.2/src/pmx/scripts/icolos_entrypoints/assemble_systems.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/scripts/ligandHybrid.py` & `pmx_biobb-3.0.2/src/pmx/scripts/ligandHybrid.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/scripts/make_double_box.py` & `pmx_biobb-3.0.2/src/pmx/scripts/make_double_box.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/scripts/md_setup.py` & `pmx_biobb-3.0.2/src/pmx/scripts/md_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,28 +187,28 @@
         self.mutations = []
         if self.mutation_tags:
             self.mutations_from_tags()
         self.runs = []
         self.is_single_chain = False
 
     def read_mutation_file(self, mut_file ):
-        print '\n\t\t\tReading mutation file: %s\n' % mut_file
+        print()'\n\t\t\tReading mutation file: %s\n' % mut_file)
         l = open(mut_file).readlines()
         count = 1
         for line in l:
             entr = line.strip()
             if entr:
-                print '\t\t\t (%d) ->  %s' % (count, entr)
+                print('\t\t\t (%d) ->  %s' % (count, entr))
                 self.mutation_tags.append( entr )
                 count+=1
 
 
     def setup(self):
         self.read_pdb()
-        print '\n\n'
+        print('\n\n')
         for m in self.mutations:
             self.setup_mutation_run(m)
 
     def read_pdb( self ):
         self.model = Model(self.md_in_conf)
         if len(self.model.chains) == 1:
             self.is_single_chain = True
@@ -234,25 +234,25 @@
             if chain not in affected_chains:
                 affected_chains.append( chain )
         name = '-'.join(muts)
         if str(self.__class__).split('.')[1] == 'DiscreteTI':
             name+='.dti'
         elif str(self.__class__).split('.')[1] == 'CrooksMD':
             name+='.crooks'
-        print '\n\t\t\tPreparing mutation run -> %s \n' % name
+        print('\n\t\t\tPreparing mutation run -> %s \n' % name)
         if os.path.isdir( name ):
             shutil.rmtree(name)
         os.mkdir(name)
         self.runs.append( name )
         shutil.copy(self.md_in_conf, name)
         script_file = os.path.join(name,'mutations.txt')
         fp = open(script_file,'w')
         for m in mutation:
             resid, resn, chain = m
-            print >>fp, resid, resn
+            print>>fp, resid, resn
         fp.close()
         self.make_mutation(name, affected_chains)
 
 
     def make_mutation(self, path, affected_chains ):
         os.chdir(path)
         run = '~/software/pmx/scripts/mutate_beta45.py -f %s -script mutations.txt -o mut.pdb' % self.md_in_conf
@@ -262,15 +262,15 @@
             itp_file = 'topol_Protein.itp'
             run = '~/software/pmx/scripts/make_bstate_beta45.py -itp %s' % itp_file
             run_command( self.make_mutation, run )
             shutil.move(itp_file, itp_file+'.save')
             shutil.move('newtop.itp', itp_file)
         else:
             for chain in affected_chains:
-                print 'Applying changes to topology of chain %s' % chain
+                print('Applying changes to topology of chain %s' % chain)
                 itp_file = 'topol_Protein_chain_%s.itp' % chain
                 run = '~/software/pmx/scripts/make_bstate_beta45.py -itp %s' % itp_file
                 run_command( self.make_mutation, run )
                 shutil.move(itp_file, itp_file+'.save')
                 shutil.move('newtop.itp', itp_file)
         os.chdir('..')
 
@@ -285,30 +285,30 @@
 
     def do_crooks( self, mdp_file, min_mdp_file, time, nruns ):
         mdp = MDP().read( mdp_file)
         min_mdp = MDP().read( min_mdp_file)
         self.prepare_min_mdp_files(min_mdp, time )
         self.prepare_eq_mdp_files(mdp, time )
         for r in self.runs:
-            print '\n\t\t\tSetting up Crooks run -> %s\n' % r
+            print('\n\t\t\tSetting up Crooks run -> %s\n' % r)
 
             self.minimize_states( r )
             self.setup_equilibration_runs( r, nruns )
 
     def minimize_states( self, path ):
 
         os.chdir(path)
         run = 'grompp -f ../crooks_minA.mdp -c gmx.pdb -o minA.tpr'
         run_command( self.minimize_states, run )
         run = 'grompp -f ../crooks_minB.mdp -c gmx.pdb -o minB.tpr'
         run_command( self.minimize_states, run )
-        print '\n\t\t\tRunning energy minimization on %s ( state A ) \n' % ( path )
+        print('\n\t\t\tRunning energy minimization on %s ( state A ) \n' % ( path ))
         run = 'mdrun -v -c emA.pdb -s minA.tpr'
         run_command( self.minimize_states, run )
-        print '\n\t\t\tRunning energy minimization on %s ( state B ) \n' % ( path )
+        print('\n\t\t\tRunning energy minimization on %s ( state B ) \n' % ( path ))
         run = 'mdrun -v -c emB.pdb -s minB.tpr'
         run_command( self.minimize_states, run )
         os.chdir('..')
 
     def prepare_eq_mdp_files( self, mdp, time ):
         nsteps = 1000*time/.002
         mdp['nsteps'] = nsteps
@@ -331,15 +331,15 @@
         print >>fp, mdp
         fp.close()
 
 
     def setup_equilibration_runs( self, path, nruns ):
         os.chdir(path)
         for i in range(nruns):
-            print '\n\t\t\tPreparing run input file for  %s ( run %d ) \n' % ( path, i )
+            print('\n\t\t\tPreparing run input file for  %s ( run %d ) \n' % ( path, i ))
             os.mkdir('runA.%d' % i)
             os.mkdir('runB.%d' % i)
             run = 'grompp -f ../crooks_eqA.mdp -c emA.pdb -o runA.%d/topol.tpr' % i
             run_command( self.setup_equilibration_runs, run )
             run = 'grompp -f ../crooks_eqB.mdp -c emB.pdb -o runB.%d/topol.tpr' % i
             run_command( self.setup_equilibration_runs, run )
             self.clean_backups()
@@ -382,32 +382,32 @@
     def setup_runs( self, path ):
         os.chdir( path )
         for lda in self.lambda_steps:
             min_mdp = 'dti_min_%4.3f.mdp' % round(lda,3)
             run_mdp = 'dti_%4.3f.mdp' % round(lda,3)
             run_dir = 'run_%4.3f' % round(lda,3)
             os.mkdir( run_dir )
-            print '\n\t\t\tRunning energy minimization on %s/%s \n' % ( path, run_dir )
+            print('\n\t\t\tRunning energy minimization on %s/%s \n' % ( path, run_dir ))
             run = 'grompp -f ../%s -c gmx.pdb -o %s/em.tpr' % (min_mdp, run_dir )
             run_command( self.setup_runs, run )
             os.chdir( run_dir )
             run = 'mdrun -v -c em.pdb -s em.tpr'
             run_command( self.setup_runs, run )
             os.chdir('..')
-            print '\n\t\t\tPreparing run input file for  %s/%s \n' % ( path, run_dir )
+            print('\n\t\t\tPreparing run input file for  %s/%s \n' % ( path, run_dir ))
             run = 'grompp -f ../%s -c %s/em.pdb -o %s/topol.tpr' % (run_mdp, run_dir, run_dir )
             run_command( self.setup_runs, run )
             self.clean_backups()
         os.chdir( '..')
 
     def do_dti( self, mdp, min_mdp, time ):
         self.prepare_dti_min_mdp_files( min_mdp)
         self.prepare_dti_mdp_files( mdp, time)
         for r in self.runs:
-            print '\n\t\t\tSetting up Discrete TI run -> %s\n' % r
+            print('\n\t\t\tSetting up Discrete TI run -> %s\n' % r)
             self.setup_runs( r )
 
 
 
 def main(argv):
 
     version = "1.0"
@@ -480,15 +480,15 @@
 
     if not cmdl['-skip_md_setup']:
         md = MD( pdb_in = pdb_in, water = water, conc = conc, box_type = box_type, box_size = box_size )
         md.setup()
         free_energy_start_pdb = md.md_in_conf
     else:
         if not bFreeEnergy:
-            print 'Nothing to do........... (no MD, no Free Energy)'
+            print('Nothing to do........... (no MD, no Free Energy)')
             sys.exit()
     if bFreeEnergy:
         if not free_energy_start_pdb:
             free_energy_start_pdb = pdb_in
         if cmdl['-fe.crooks']:
             crooksMD = CrooksMD( mutation_file, md_in_conf = free_energy_start_pdb)
             crooksMD.setup()
@@ -497,15 +497,15 @@
         if cmdl['-fe.dti']:
             dti = DiscreteTI( mutation_file, md_in_conf = free_energy_start_pdb )
             dti.setup()
             dti.read_lambda_steps( cmdl['-lambda_steps'] )
             dti.do_dti(cmdl['-dti_mdp'], cmdl['-min_mdp'], cmdl['-dti_run_time'] )
 
 
-    print '\n\t\t\t ....... DONE .......... \n'
+    print('\n\t\t\t ....... DONE .......... \n')
 
 
 
 ##     n_crooks_runs = cmdl['-n_crooks_runs']
 ##     if cmdl.opt['-m'].is_set:
 ##         mut_file  = cmdl['-m']
 ##     else:
```

### Comparing `pmx_biobb-3.0.1/src/pmx/scripts/mutate.py` & `pmx_biobb-3.0.2/src/pmx/scripts/mutate.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/scripts/prepare_crooks_runs.py` & `pmx_biobb-3.0.2/src/pmx/scripts/prepare_crooks_runs.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,23 +47,23 @@
         print >>sys.stderr, 'Output written to %s' % err_file
         fp = open(err_file, 'w')
         print >>fp, s
         print >>fp, out
         fp.close()
         sys.exit(1)
     else:
-        print "%-90s" % s, ': ok'
+        print("%-90s" % s, ': ok')
 
 
 def make_dir_tree(skip=4):
 
     # catch all run?.? dirs
     dirs = glob('run?.?')
     for d in dirs:
-        print '\tPreparing run %s' % d
+        print('\tPreparing run %s' % d)
         os.chdir(d)
         os.mkdir('morphes')
         cmd = 'echo 0| trjconv -f traj.trr -s topol.tpr -skip %d -b 2001 -sep -o morphes/frame.gro' % skip
         run_command(make_dir_tree, cmd)
         os.chdir('morphes')
 
         # put each file into single directory
@@ -105,15 +105,15 @@
     fp.close()
 
 
 def make_run_input_files():
 
     dirs = glob('run?.?')
     for d in dirs:
-        print '\n\tPreparing run input files %s' % d
+        print('\n\tPreparing run input files %s' % d)
         mdp_file = None
         if d.split('.')[0][-1] == 'A':  # 0->1
             mdp_file = 'crooks_TI_runA.mdp'
         elif d.split('.')[0][-1] == 'B':  # 1->0
             mdp_file = 'crooks_TI_runB.mdp'
         dir_list = glob(os.path.join(d, 'morphes')+'/frame*')
         for f in dir_list:
@@ -189,32 +189,32 @@
 
     run_dir = args.dir
     mdp_file = args.mdp
     sw_time = args.sw_time
     sc_alpha = args.sc_alpha
     sc_sigma = args.sc_sigma
 
-    print '\n\t Preparing FGTI runs in directory..: %s' % run_dir
-    print '\t Template mdp file to use............: %s' % mdp_file
-    print '\t Switching time to use...............: %8d ps' % int(sw_time)
-    print '\t Soft-core alpha to use..............: %8.3f' % sc_alpha
-    print '\t Soft-core sigma to use..............: %8.3f' % sc_sigma
-    print '\n'
+    print('\n\t Preparing FGTI runs in directory..: %s' % run_dir)
+    print('\t Template mdp file to use............: %s' % mdp_file)
+    print('\t Switching time to use...............: %8d ps' % int(sw_time))
+    print('\t Soft-core alpha to use..............: %8.3f' % sc_alpha)
+    print('\t Soft-core sigma to use..............: %8.3f' % sc_sigma)
+    print('\n')
 
 
     os.chdir(run_dir)
 
-    print '\t Preparing mdp input files........... '
+    print('\t Preparing mdp input files........... ')
 
     prepare_mdp_files(mdp_file, sw_time, sc_alpha, sc_sigma)
 
 
-    print '\t Preparing directory tree............ '
+    print('\t Preparing directory tree............ ')
     make_dir_tree(skip=args.skip)
     make_run_input_files()
     os.chdir(here)
-    print '\n\t............... DONE .................\n'
+    print('\n\t............... DONE .................\n')
 
 
 if __name__ == '__main__':
     args = parse_options()
     main(args)
```

### Comparing `pmx_biobb-3.0.1/src/pmx/scripts/set_gmxlib.py` & `pmx_biobb-3.0.2/src/pmx/scripts/set_gmxlib.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/scripts/setup_abfe.py` & `pmx_biobb-3.0.2/src/pmx/scripts/setup_abfe.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/utils.py` & `pmx_biobb-3.0.2/src/pmx/utils.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/xdrfile.py` & `pmx_biobb-3.0.2/src/pmx/xdrfile.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx/xtc.py` & `pmx_biobb-3.0.2/src/pmx/xtc.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/src/pmx_biobb.egg-info/PKG-INFO` & `pmx_biobb-3.0.2/src/pmx_biobb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmx-biobb
-Version: 3.0.1
+Version: 3.0.2
 Summary: Toolkit for free-energy calculation setup/analysis and biomolecular structure handling
 Home-page: https://github.com/deGrootLab/pmx/tree/develop
 Author: Daniel Seeliger
 Author-email: seeliger.biosoft@gmail.de
 License: GPL 3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pmx_biobb-3.0.1/src/pmx_biobb.egg-info/SOURCES.txt` & `pmx_biobb-3.0.2/src/pmx_biobb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pmx_biobb-3.0.1/versioneer.py` & `pmx_biobb-3.0.2/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -734,25 +734,25 @@
 def render_pep440(pieces):
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
-    1: no tags. git_describe was just HEX. 3.0.1
+    1: no tags. git_describe was just HEX. 3.0.2
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "3.0.1" %% (pieces["distance"],
+        rendered = "3.0.2" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_pre(pieces):
@@ -1234,26 +1234,26 @@
 def render_pep440(pieces):
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
-    1: no tags. git_describe was just HEX. 3.0.1
+    1: no tags. git_describe was just HEX. 3.0.2
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "3.0.1"
+        rendered = "3.0.2"
 
     return rendered
 
 
 def render_pep440_pre(pieces):
     """TAG[.post.devDISTANCE] -- No -dirty.
 
@@ -1394,15 +1394,15 @@
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
     """Get the project version from whatever source is available."""
 
-    return {"version": "3.0.1", "full-revisionid": None,
+    return {"version": "3.0.2", "full-revisionid": None,
             "dirty": None, "error": "unable to compute version",
             "date": None}
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
```

