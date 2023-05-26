# Comparing `tmp/polysort-0.0.2.tar.gz` & `tmp/polysort-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polysort-0.0.2.tar", last modified: Fri May 26 17:39:07 2023, max compression
+gzip compressed data, was "polysort-0.0.3.tar", last modified: Fri May 26 17:40:47 2023, max compression
```

## Comparing `polysort-0.0.2.tar` & `polysort-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 17:39:07.740801 polysort-0.0.2/
--rw-rw-rw-   0        0        0      848 2023-05-26 17:39:07.740801 polysort-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 17:39:07.728798 polysort-0.0.2/polysort/
--rw-rw-rw-   0        0        0        0 2023-04-18 14:21:18.000000 polysort-0.0.2/polysort/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:39:07.739801 polysort-0.0.2/polysort.egg-info/
--rw-rw-rw-   0        0        0      848 2023-05-26 17:39:07.000000 polysort-0.0.2/polysort.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-05-26 17:39:07.000000 polysort-0.0.2/polysort.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 17:39:07.000000 polysort-0.0.2/polysort.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-26 17:39:07.000000 polysort-0.0.2/polysort.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      959 2023-05-26 17:39:07.741802 polysort-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0       85 2023-05-26 17:39:04.000000 polysort-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:40:47.301790 polysort-0.0.3/
+-rw-rw-rw-   0        0        0      837 2023-05-26 17:40:47.302791 polysort-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 17:40:47.291789 polysort-0.0.3/polysort/
+-rw-rw-rw-   0        0        0        0 2023-04-18 14:21:18.000000 polysort-0.0.3/polysort/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:40:47.300792 polysort-0.0.3/polysort.egg-info/
+-rw-rw-rw-   0        0        0      837 2023-05-26 17:40:47.000000 polysort-0.0.3/polysort.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-05-26 17:40:47.000000 polysort-0.0.3/polysort.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 17:40:47.000000 polysort-0.0.3/polysort.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 17:40:47.000000 polysort-0.0.3/polysort.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      948 2023-05-26 17:40:47.303791 polysort-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       85 2023-05-26 17:40:45.000000 polysort-0.0.3/setup.py
```

### Comparing `polysort-0.0.2/PKG-INFO` & `polysort-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: polysort
-Version: 0.0.2
-Summary: A collection of state space search algorithms
+Version: 0.0.3
+Summary: A collection of sorting algorithms
 Home-page: https://github.com/chaseburton/polysort
 Author: Chase Burton Taylor
 Author-email: ctaylor@citycollege.sheffield.eu
 License: MIT
 Project-URL: Documentation, http://polysort.readthedocs.org
 Project-URL: Source Code, https://github.com/chaseburton/polysort
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `polysort-0.0.2/polysort.egg-info/PKG-INFO` & `polysort-0.0.3/polysort.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: polysort
-Version: 0.0.2
-Summary: A collection of state space search algorithms
+Version: 0.0.3
+Summary: A collection of sorting algorithms
 Home-page: https://github.com/chaseburton/polysort
 Author: Chase Burton Taylor
 Author-email: ctaylor@citycollege.sheffield.eu
 License: MIT
 Project-URL: Documentation, http://polysort.readthedocs.org
 Project-URL: Source Code, https://github.com/chaseburton/polysort
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `polysort-0.0.2/setup.cfg` & `polysort-0.0.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -2,59 +2,59 @@
 00000010: 203d 2070 6f6c 7973 6f72 740d 0a61 7574   = polysort..aut
 00000020: 686f 7220 3d20 4368 6173 6520 4275 7274  hor = Chase Burt
 00000030: 6f6e 2054 6179 6c6f 720d 0a61 7574 686f  on Taylor..autho
 00000040: 722d 656d 6169 6c20 3d20 6374 6179 6c6f  r-email = ctaylo
 00000050: 7240 6369 7479 636f 6c6c 6567 652e 7368  r@citycollege.sh
 00000060: 6566 6669 656c 642e 6575 0d0a 7375 6d6d  effield.eu..summ
 00000070: 6172 7920 3d20 4120 636f 6c6c 6563 7469  ary = A collecti
-00000080: 6f6e 206f 6620 7374 6174 6520 7370 6163  on of state spac
-00000090: 6520 7365 6172 6368 2061 6c67 6f72 6974  e search algorit
-000000a0: 686d 730d 0a64 6573 6372 6970 7469 6f6e  hms..description
-000000b0: 2d66 696c 6520 3d20 5245 4144 4d45 2e6d  -file = README.m
-000000c0: 640d 0a64 6573 6372 6970 7469 6f6e 2d63  d..description-c
-000000d0: 6f6e 7465 6e74 2d74 7970 6520 3d20 7465  ontent-type = te
-000000e0: 7874 2f78 2d6d 643b 2063 6861 7273 6574  xt/x-md; charset
-000000f0: 3d55 5446 2d38 0d0a 686f 6d65 2d70 6167  =UTF-8..home-pag
-00000100: 6520 3d20 6874 7470 733a 2f2f 6769 7468  e = https://gith
-00000110: 7562 2e63 6f6d 2f63 6861 7365 6275 7274  ub.com/chaseburt
-00000120: 6f6e 2f70 6f6c 7973 6f72 740d 0a70 726f  on/polysort..pro
-00000130: 6a65 6374 5f75 726c 7320 3d20 0d0a 0944  ject_urls = ...D
-00000140: 6f63 756d 656e 7461 7469 6f6e 203d 2068  ocumentation = h
-00000150: 7474 703a 2f2f 706f 6c79 736f 7274 2e72  ttp://polysort.r
-00000160: 6561 6474 6865 646f 6373 2e6f 7267 0d0a  eadthedocs.org..
-00000170: 0953 6f75 7263 6520 436f 6465 203d 2068  .Source Code = h
-00000180: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000190: 6d2f 6368 6173 6562 7572 746f 6e2f 706f  m/chaseburton/po
-000001a0: 6c79 736f 7274 0d0a 6c69 6365 6e73 6520  lysort..license 
-000001b0: 3d20 4d49 540d 0a6c 6963 656e 7365 5f66  = MIT..license_f
-000001c0: 696c 6520 3d20 4c49 4345 4e53 452e 7478  ile = LICENSE.tx
-000001d0: 740d 0a63 6c61 7373 6966 6965 7220 3d20  t..classifier = 
-000001e0: 0d0a 0944 6576 656c 6f70 6d65 6e74 2053  ...Development S
-000001f0: 7461 7475 7320 3a3a 2033 202d 2041 6c70  tatus :: 3 - Alp
-00000200: 6861 0d0a 0949 6e74 656e 6465 6420 4175  ha...Intended Au
-00000210: 6469 656e 6365 203a 3a20 5363 6965 6e63  dience :: Scienc
-00000220: 652f 5265 7365 6172 6368 0d0a 0954 6f70  e/Research...Top
-00000230: 6963 203a 3a20 5363 6965 6e74 6966 6963  ic :: Scientific
-00000240: 2f45 6e67 696e 6565 7269 6e67 203a 3a20  /Engineering :: 
-00000250: 4172 7469 6669 6369 616c 2049 6e74 656c  Artificial Intel
-00000260: 6c69 6765 6e63 650d 0a09 4c69 6365 6e73  ligence...Licens
-00000270: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000280: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-00000290: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-000002a0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000002b0: 6e0d 0a09 5072 6f67 7261 6d6d 696e 6720  n...Programming 
-000002c0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002d0: 6f6e 203a 3a20 330d 0a09 5072 6f67 7261  on :: 3...Progra
-000002e0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000002f0: 3a20 5079 7468 6f6e 203a 3a20 332e 370d  : Python :: 3.7.
-00000300: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000310: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000320: 203a 3a20 332e 380d 0a09 5072 6f67 7261   :: 3.8...Progra
-00000330: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000340: 3a20 5079 7468 6f6e 203a 3a20 332e 390d  : Python :: 3.9.
-00000350: 0a0d 0a5b 6669 6c65 735d 0d0a 7061 636b  ...[files]..pack
-00000360: 6167 6520 3d20 0d0a 0970 6f6c 7973 6f72  age = ...polysor
-00000370: 740d 0a0d 0a5b 6264 6973 745f 7768 6565  t....[bdist_whee
-00000380: 6c5d 0d0a 756e 6976 6572 7361 6c20 3d20  l]..universal = 
-00000390: 310d 0a0d 0a5b 6567 675f 696e 666f 5d0d  1....[egg_info].
-000003a0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-000003b0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000080: 6f6e 206f 6620 736f 7274 696e 6720 616c  on of sorting al
+00000090: 676f 7269 7468 6d73 0d0a 6465 7363 7269  gorithms..descri
+000000a0: 7074 696f 6e2d 6669 6c65 203d 2052 4541  ption-file = REA
+000000b0: 444d 452e 6d64 0d0a 6465 7363 7269 7074  DME.md..descript
+000000c0: 696f 6e2d 636f 6e74 656e 742d 7479 7065  ion-content-type
+000000d0: 203d 2074 6578 742f 782d 6d64 3b20 6368   = text/x-md; ch
+000000e0: 6172 7365 743d 5554 462d 380d 0a68 6f6d  arset=UTF-8..hom
+000000f0: 652d 7061 6765 203d 2068 7474 7073 3a2f  e-page = https:/
+00000100: 2f67 6974 6875 622e 636f 6d2f 6368 6173  /github.com/chas
+00000110: 6562 7572 746f 6e2f 706f 6c79 736f 7274  eburton/polysort
+00000120: 0d0a 7072 6f6a 6563 745f 7572 6c73 203d  ..project_urls =
+00000130: 200d 0a09 446f 6375 6d65 6e74 6174 696f   ...Documentatio
+00000140: 6e20 3d20 6874 7470 3a2f 2f70 6f6c 7973  n = http://polys
+00000150: 6f72 742e 7265 6164 7468 6564 6f63 732e  ort.readthedocs.
+00000160: 6f72 670d 0a09 536f 7572 6365 2043 6f64  org...Source Cod
+00000170: 6520 3d20 6874 7470 733a 2f2f 6769 7468  e = https://gith
+00000180: 7562 2e63 6f6d 2f63 6861 7365 6275 7274  ub.com/chaseburt
+00000190: 6f6e 2f70 6f6c 7973 6f72 740d 0a6c 6963  on/polysort..lic
+000001a0: 656e 7365 203d 204d 4954 0d0a 6c69 6365  ense = MIT..lice
+000001b0: 6e73 655f 6669 6c65 203d 204c 4943 454e  nse_file = LICEN
+000001c0: 5345 2e74 7874 0d0a 636c 6173 7369 6669  SE.txt..classifi
+000001d0: 6572 203d 200d 0a09 4465 7665 6c6f 706d  er = ...Developm
+000001e0: 656e 7420 5374 6174 7573 203a 3a20 3320  ent Status :: 3 
+000001f0: 2d20 416c 7068 610d 0a09 496e 7465 6e64  - Alpha...Intend
+00000200: 6564 2041 7564 6965 6e63 6520 3a3a 2053  ed Audience :: S
+00000210: 6369 656e 6365 2f52 6573 6561 7263 680d  cience/Research.
+00000220: 0a09 546f 7069 6320 3a3a 2053 6369 656e  ..Topic :: Scien
+00000230: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
+00000240: 6720 3a3a 2041 7274 6966 6963 6961 6c20  g :: Artificial 
+00000250: 496e 7465 6c6c 6967 656e 6365 0d0a 094c  Intelligence...L
+00000260: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000270: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+00000280: 6365 6e73 650d 0a09 5072 6f67 7261 6d6d  cense...Programm
+00000290: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002a0: 5079 7468 6f6e 0d0a 0950 726f 6772 616d  Python...Program
+000002b0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002c0: 2050 7974 686f 6e20 3a3a 2033 0d0a 0950   Python :: 3...P
+000002d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000002e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000002f0: 2033 2e37 0d0a 0950 726f 6772 616d 6d69   3.7...Programmi
+00000300: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000310: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
+00000320: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000330: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000340: 2033 2e39 0d0a 0d0a 5b66 696c 6573 5d0d   3.9....[files].
+00000350: 0a70 6163 6b61 6765 203d 200d 0a09 706f  .package = ...po
+00000360: 6c79 736f 7274 0d0a 0d0a 5b62 6469 7374  lysort....[bdist
+00000370: 5f77 6865 656c 5d0d 0a75 6e69 7665 7273  _wheel]..univers
+00000380: 616c 203d 2031 0d0a 0d0a 5b65 6767 5f69  al = 1....[egg_i
+00000390: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+000003a0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+000003b0: 0d0a 0d0a                                ....
```

