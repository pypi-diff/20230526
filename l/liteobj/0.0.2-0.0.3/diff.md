# Comparing `tmp/liteobj-0.0.2.tar.gz` & `tmp/liteobj-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteobj-0.0.2.tar", last modified: Thu Feb 23 01:58:01 2023, max compression
+gzip compressed data, was "liteobj-0.0.3.tar", last modified: Thu May 25 22:18:58 2023, max compression
```

## Comparing `liteobj-0.0.2.tar` & `liteobj-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-02-23 01:58:01.506604 liteobj-0.0.2/
--rwxr-xr-x   0 user      (1000) user      (1000)     1069 2023-02-23 01:10:34.000000 liteobj-0.0.2/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      255 2023-02-23 01:58:01.506604 liteobj-0.0.2/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1455 2023-02-23 01:48:38.000000 liteobj-0.0.2/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-02-23 01:58:01.506604 liteobj-0.0.2/liteobj/
--rw-r--r--   0 user      (1000) user      (1000)       66 2023-02-23 01:11:59.000000 liteobj-0.0.2/liteobj/__init__.py
--rwxr-xr-x   0 user      (1000) user      (1000)     3460 2023-02-23 01:12:16.000000 liteobj-0.0.2/liteobj/lite.py
--rw-r--r--   0 user      (1000) user      (1000)       14 2023-02-23 01:12:26.000000 liteobj-0.0.2/liteobj/requirements.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-02-23 01:58:01.506604 liteobj-0.0.2/liteobj.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      255 2023-02-23 01:58:01.000000 liteobj-0.0.2/liteobj.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      275 2023-02-23 01:58:01.000000 liteobj-0.0.2/liteobj.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-02-23 01:58:01.000000 liteobj-0.0.2/liteobj.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-02-23 01:58:01.000000 liteobj-0.0.2/liteobj.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       15 2023-02-23 01:58:01.000000 liteobj-0.0.2/liteobj.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-02-23 01:58:01.000000 liteobj-0.0.2/liteobj.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-02-23 01:58:01.506604 liteobj-0.0.2/setup.cfg
--rwxr-xr-x   0 user      (1000) user      (1000)      706 2023-02-23 01:56:33.000000 liteobj-0.0.2/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 22:18:58.542070 liteobj-0.0.3/
+-rwxr-xr-x   0 user      (1000) user      (1000)    11538 2023-05-25 22:18:19.000000 liteobj-0.0.3/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      255 2023-05-25 22:18:58.542070 liteobj-0.0.3/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1349 2023-05-25 22:11:37.000000 liteobj-0.0.3/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 22:18:58.532070 liteobj-0.0.3/liteobj/
+-rw-r--r--   0 user      (1000) user      (1000)       20 2023-05-25 22:02:13.000000 liteobj-0.0.3/liteobj/__init__.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     3541 2023-05-25 22:12:29.000000 liteobj-0.0.3/liteobj/lite.py
+-rw-r--r--   0 user      (1000) user      (1000)       28 2023-05-25 21:59:58.000000 liteobj-0.0.3/liteobj/requirements.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 22:18:58.542070 liteobj-0.0.3/liteobj.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      255 2023-05-25 22:18:58.000000 liteobj-0.0.3/liteobj.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      275 2023-05-25 22:18:58.000000 liteobj-0.0.3/liteobj.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-25 22:18:58.000000 liteobj-0.0.3/liteobj.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-25 22:18:58.000000 liteobj-0.0.3/liteobj.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)       29 2023-05-25 22:18:58.000000 liteobj-0.0.3/liteobj.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-25 22:18:58.000000 liteobj-0.0.3/liteobj.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-25 22:18:58.542070 liteobj-0.0.3/setup.cfg
+-rwxr-xr-x   0 user      (1000) user      (1000)      706 2023-05-25 22:15:21.000000 liteobj-0.0.3/setup.py
```

### Comparing `liteobj-0.0.2/README.md` & `liteobj-0.0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,85 @@
-00000000: 2320 4c69 7465 6f62 6a0a 0a0a 3c61 2068  # Liteobj...<a h
-00000010: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00000020: 6875 622e 636f 6d2f 316c 696e 742f 6c69  hub.com/1lint/li
-00000030: 7465 6c61 622f 626c 6f62 2f6d 6173 7465  telab/blob/maste
-00000040: 722f 4c49 4345 4e53 4522 3e3c 696d 6720  r/LICENSE"><img 
-00000050: 616c 743d 224d 4954 204c 6963 656e 7365  alt="MIT License
-00000060: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-00000070: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000080: 6467 652f 4c69 6365 6e73 652d 4d49 542d  dge/License-MIT-
-00000090: 7965 6c6c 6f77 6772 6565 6e22 202f 3e3c  yellowgreen" /><
-000000a0: 2f61 3e0a 0a4c 6974 656f 626a 2069 7320  /a>..Liteobj is 
-000000b0: 6120 636f 6e76 656e 6965 6e63 6520 746f  a convenience to
-000000c0: 6f6c 2066 6f72 2063 6f6e 6669 6775 7269  ol for configuri
-000000d0: 6e67 206c 6172 6765 206f 626a 6563 7473  ng large objects
-000000e0: 2069 6e20 5079 7468 6f6e 2e0a 4d4c 2065   in Python..ML e
-000000f0: 7870 6572 696d 656e 7473 206f 6674 656e  xperiments often
-00000100: 2069 6e76 6f6c 7665 2069 6e73 7461 6e74   involve instant
-00000110: 6961 7469 6e67 206d 756c 7469 706c 6520  iating multiple 
-00000120: 6c61 7965 7273 206f 6620 6e65 7374 6564  layers of nested
-00000130: 206f 626a 6563 7473 2c20 6c65 6164 696e   objects, leadin
-00000140: 6720 746f 2063 756d 6265 7273 6f6d 6520  g to cumbersome 
-00000150: 696e 7374 616e 7469 6174 696f 6e20 6c6f  instantiation lo
-00000160: 6769 6320 616e 6420 636f 6e66 6967 7572  gic and configur
-00000170: 6174 696f 6e20 6669 6c65 2066 6f72 6d61  ation file forma
-00000180: 7473 2073 7065 6369 6669 6320 746f 2065  ts specific to e
-00000190: 6163 6820 7072 6f6a 6563 7427 7320 636f  ach project's co
-000001a0: 6465 2e20 5468 726f 7567 6820 736f 6d65  de. Through some
-000001b0: 2072 6563 7572 7369 6f6e 2c20 6c69 7465   recursion, lite
-000001c0: 6f62 6a20 656e 6162 6c65 7320 6120 7369  obj enables a si
-000001d0: 6d70 6c69 6669 6564 206f 626a 6563 7420  mplified object 
-000001e0: 636f 6e66 6967 7572 6174 696f 6e20 666f  configuration fo
-000001f0: 726d 6174 2063 616e 2062 6520 6d6f 7265  rmat can be more
-00000200: 2064 6972 6563 746c 7920 636f 6d70 696c   directly compil
-00000210: 6564 2069 6e74 6f20 7468 6520 7370 6563  ed into the spec
-00000220: 6966 6965 6420 6f62 6a65 6374 2e20 0a0a  ified object. ..
-00000230: 506c 6561 7365 2073 6565 205b 7475 746f  Please see [tuto
-00000240: 7269 616c 2e69 7079 6e62 5d28 6874 7470  rial.ipynb](http
-00000250: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f31  s://github.com/1
-00000260: 6c69 6e74 2f6c 6974 656f 626a 2f62 6c6f  lint/liteobj/blo
-00000270: 622f 6d61 7374 6572 2f74 7574 6f72 6961  b/master/tutoria
-00000280: 6c2e 6970 796e 6229 2066 6f72 2061 6e20  l.ipynb) for an 
-00000290: 6578 706c 616e 6174 696f 6e20 616e 6420  explanation and 
-000002a0: 6465 6d6f 6e73 7472 6174 696f 6e20 6f66  demonstration of
-000002b0: 2060 6c69 7465 6f62 6a60 2e20 0a0a 2323   `liteobj`. ..##
-000002c0: 2049 6e73 7461 6c6c 0a0a 496e 7374 616c   Install..Instal
-000002d0: 6c20 6672 6f6d 2070 6970 0a60 6060 0a70  l from pip.```.p
-000002e0: 6970 2069 6e73 7461 6c6c 206c 6974 656f  ip install liteo
-000002f0: 626a 0a60 6060 0a0a 4173 2061 2062 6173  bj.```..As a bas
-00000300: 6963 2065 7861 6d70 6c65 2c20 7275 6e20  ic example, run 
-00000310: 7468 6520 5079 746f 7263 6820 4c69 6768  the Pytorch Ligh
-00000320: 746e 696e 6720 4261 7369 6320 4741 4e20  tning Basic GAN 
-00000330: 7475 746f 7269 616c 2066 726f 6d20 6874  tutorial from ht
-00000340: 7470 733a 2f2f 7079 746f 7263 682d 6c69  tps://pytorch-li
-00000350: 6768 746e 696e 672e 7265 6164 7468 6564  ghtning.readthed
-00000360: 6f63 732e 696f 2f65 6e2f 7374 6162 6c65  ocs.io/en/stable
-00000370: 2f6e 6f74 6562 6f6f 6b73 2f6c 6967 6874  /notebooks/light
-00000380: 6e69 6e67 5f65 7861 6d70 6c65 732f 6261  ning_examples/ba
-00000390: 7369 632d 6761 6e2e 6874 6d6c 0a60 6060  sic-gan.html.```
-000003a0: 0a67 6974 2063 6c6f 6e65 2068 7474 7073  .git clone https
-000003b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 316c  ://github.com/1l
-000003c0: 696e 742f 6c69 7465 6f62 6a0a 6364 206c  int/liteobj.cd l
-000003d0: 6974 656f 626a 0a70 7974 686f 6e20 2d6d  iteobj.python -m
-000003e0: 2070 6970 2069 6e73 7461 6c6c 202d 7220   pip install -r 
-000003f0: 7265 7175 6972 656d 656e 7473 2e74 7874  requirements.txt
-00000400: 0a70 7974 686f 6e20 6c69 7465 2e70 7920  .python lite.py 
-00000410: 6c61 622e 7961 6d6c 2066 6974 0a60 6060  lab.yaml fit.```
-00000420: 0a0a 546f 2072 756e 206c 6974 652e 7079  ..To run lite.py
-00000430: 2069 6e20 6f74 6865 7220 6469 7265 6374   in other direct
-00000440: 6f72 6965 732c 2069 6e73 7461 6c6c 2074  ories, install t
-00000450: 6865 2070 6970 2070 6163 6b61 6765 2e20  he pip package. 
-00000460: 5468 656e 2072 756e 2063 6f6e 6669 6775  Then run configu
-00000470: 7261 7469 6f6e 7320 7769 7468 2074 6865  rations with the
-00000480: 2060 6c69 7465 6020 636f 6e73 6f6c 6520   `lite` console 
-00000490: 7363 7269 7074 200a 6060 600a 7079 7468  script .```.pyth
-000004a0: 6f6e 202d 6d20 7069 7020 696e 7374 616c  on -m pip instal
-000004b0: 6c20 2e0a 6c69 7465 2063 6f6e 6669 6773  l ..lite configs
-000004c0: 2f6c 6162 2e79 616d 6c20 6669 740a 6060  /lab.yaml fit.``
-000004d0: 600a 0a53 796e 7461 7820 6973 200a 6060  `..Syntax is .``
-000004e0: 600a 6c69 7465 207b 636f 6e66 6967 5f70  `.lite {config_p
-000004f0: 6174 687d 207b 6f62 6a65 6374 5f6d 6574  ath} {object_met
-00000500: 686f 647d 0a60 6060 0a57 6865 7265 2060  hod}.```.Where `
-00000510: 636f 6e66 6967 5f70 6174 6860 2069 7320  config_path` is 
-00000520: 7061 7468 2074 6f20 7468 6520 7961 6d6c  path to the yaml
-00000530: 2066 696c 6520 746f 2069 6e73 7461 6e74   file to instant
-00000540: 6961 7465 2c20 616e 6420 606f 626a 6563  iate, and `objec
-00000550: 745f 6d65 7468 6f64 6020 6973 2074 6865  t_method` is the
-00000560: 206e 616d 6520 6f66 2074 6865 206f 626a   name of the obj
-00000570: 6563 7420 6d65 7468 6f64 2074 6f20 696e  ect method to in
-00000580: 766f 6b65 206f 6e63 6520 7468 6520 6f62  voke once the ob
-00000590: 6a65 6374 2069 7320 696e 7374 616e 7469  ject is instanti
-000005a0: 6174 6564 2e20 0a0a 0a0a 0a0a 0a0a 0a    ated. .........
+00000000: 2320 4c69 7465 6f62 6a0a 0a4c 6974 6577  # Liteobj..Litew
+00000010: 6569 6768 7420 636f 6e66 6967 7572 6174  eight configurat
+00000020: 696f 6e20 666f 726d 6174 2066 6f72 2064  ion format for d
+00000030: 6566 696e 696e 6720 616e 6420 7265 6375  efining and recu
+00000040: 7273 6976 656c 7920 696e 7374 616e 7469  rsively instanti
+00000050: 6174 696e 6720 7079 7468 6f6e 206f 626a  ating python obj
+00000060: 6563 7473 2063 6f6d 706f 7365 6420 6f66  ects composed of
+00000070: 206e 6573 7465 6420 6f62 6a65 6374 2070   nested object p
+00000080: 6172 616d 6574 6572 730a 0a53 6565 205b  arameters..See [
+00000090: 7475 746f 7269 616c 2e69 7079 6e62 5d28  tutorial.ipynb](
+000000a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000000b0: 6f6d 2f31 6c69 6e74 2f6c 6974 656f 626a  om/1lint/liteobj
+000000c0: 2f62 6c6f 622f 6d61 7374 6572 2f74 7574  /blob/master/tut
+000000d0: 6f72 6961 6c2e 6970 796e 6229 2065 7861  orial.ipynb) exa
+000000e0: 6d70 6c65 2075 7365 206f 6620 606c 6974  mple use of `lit
+000000f0: 656f 626a 6020 2874 7574 6f72 6961 6c20  eobj` (tutorial 
+00000100: 666f 7220 7072 6576 696f 7573 2076 6572  for previous ver
+00000110: 7369 6f6e 2c20 6375 7272 656e 746c 7920  sion, currently 
+00000120: 6f75 7420 6f66 2064 6174 652c 2077 696c  out of date, wil
+00000130: 6c20 6265 2066 6978 6564 2073 6f6f 6e29  l be fixed soon)
+00000140: 0a0a 2323 2049 6e73 7461 6c6c 0a0a 496e  ..## Install..In
+00000150: 7374 616c 6c20 6672 6f6d 2070 6970 0a60  stall from pip.`
+00000160: 6060 0a70 6970 2069 6e73 7461 6c6c 206c  ``.pip install l
+00000170: 6974 656f 626a 0a60 6060 0a0a 2323 2051  iteobj.```..## Q
+00000180: 7569 636b 7374 6172 7420 4578 616d 706c  uickstart Exampl
+00000190: 650a 4173 2061 2062 6173 6963 2065 7861  e.As a basic exa
+000001a0: 6d70 6c65 2c20 7275 6e20 7468 6520 5079  mple, run the Py
+000001b0: 746f 7263 6820 4c69 6768 746e 696e 6720  torch Lightning 
+000001c0: 4261 7369 6320 4741 4e20 7475 746f 7269  Basic GAN tutori
+000001d0: 616c 2066 726f 6d20 6874 7470 733a 2f2f  al from https://
+000001e0: 7079 746f 7263 682d 6c69 6768 746e 696e  pytorch-lightnin
+000001f0: 672e 7265 6164 7468 6564 6f63 732e 696f  g.readthedocs.io
+00000200: 2f65 6e2f 7374 6162 6c65 2f6e 6f74 6562  /en/stable/noteb
+00000210: 6f6f 6b73 2f6c 6967 6874 6e69 6e67 5f65  ooks/lightning_e
+00000220: 7861 6d70 6c65 732f 6261 7369 632d 6761  xamples/basic-ga
+00000230: 6e2e 6874 6d6c 0a60 6060 0a67 6974 2063  n.html.```.git c
+00000240: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
+00000250: 6875 622e 636f 6d2f 316c 696e 742f 6c69  hub.com/1lint/li
+00000260: 7465 6f62 6a0a 6364 206c 6974 656f 626a  teobj.cd liteobj
+00000270: 0a70 7974 686f 6e20 2d6d 2070 6970 2069  .python -m pip i
+00000280: 6e73 7461 6c6c 202d 7220 6261 7369 635f  nstall -r basic_
+00000290: 6761 6e2f 7265 7175 6972 656d 656e 7473  gan/requirements
+000002a0: 2e74 7874 0a70 7974 686f 6e20 6c69 7465  .txt.python lite
+000002b0: 2e70 7920 6261 7369 635f 6761 6e2f 6c61  .py basic_gan/la
+000002c0: 622e 7961 6d6c 2066 6974 0a60 6060 0a0a  b.yaml fit.```..
+000002d0: 546f 2072 756e 206c 6974 652e 7079 2069  To run lite.py i
+000002e0: 6e20 6f74 6865 7220 6469 7265 6374 6f72  n other director
+000002f0: 6965 732c 2069 6e73 7461 6c6c 2074 6865  ies, install the
+00000300: 2070 6970 2070 6163 6b61 6765 2e20 5468   pip package. Th
+00000310: 656e 2072 756e 2063 6f6e 6669 6775 7261  en run configura
+00000320: 7469 6f6e 7320 7769 7468 2074 6865 2060  tions with the `
+00000330: 6c69 7465 6020 636f 6e73 6f6c 6520 7363  lite` console sc
+00000340: 7269 7074 200a 6060 600a 7079 7468 6f6e  ript .```.python
+00000350: 202d 6d20 7069 7020 696e 7374 616c 6c20   -m pip install 
+00000360: 2e0a 6c69 7465 2062 6173 6963 5f67 616e  ..lite basic_gan
+00000370: 2f6c 6162 2e79 616d 6c20 6669 740a 6060  /lab.yaml fit.``
+00000380: 600a 0a43 4c49 2073 796e 7461 7820 6973  `..CLI syntax is
+00000390: 200a 6060 600a 6c69 7465 207b 636f 6e66   .```.lite {conf
+000003a0: 6967 5f70 6174 687d 207b 6f62 6a65 6374  ig_path} {object
+000003b0: 5f6d 6574 686f 647d 207b 6d65 7468 6f64  _method} {method
+000003c0: 5f61 7267 737d 207b 6d65 7468 6f64 5f6b  _args} {method_k
+000003d0: 7761 7267 737d 0a60 6060 0a60 636f 6e66  wargs}.```.`conf
+000003e0: 6967 5f70 6174 6860 2069 7320 7061 7468  ig_path` is path
+000003f0: 2074 6f20 7468 6520 7961 6d6c 2066 696c   to the yaml fil
+00000400: 6520 746f 2069 6e73 7461 6e74 6961 7465  e to instantiate
+00000410: 2c20 616e 6420 6973 2074 6865 206f 6e6c  , and is the onl
+00000420: 7920 7265 7175 6972 6564 2070 6172 616d  y required param
+00000430: 6574 6572 2e20 5265 7475 726e 7320 7468  eter. Returns th
+00000440: 6520 696e 7374 616e 7469 6174 6564 206f  e instantiated o
+00000450: 626a 6563 7420 696e 7374 616e 6365 0a60  bject instance.`
+00000460: 6f62 6a65 6374 5f6d 6574 686f 6460 2069  object_method` i
+00000470: 7320 7468 6520 6e61 6d65 206f 6620 7468  s the name of th
+00000480: 6520 6f62 6a65 6374 206d 6574 686f 6420  e object method 
+00000490: 746f 2069 6e76 6f6b 6520 6f6e 6365 2074  to invoke once t
+000004a0: 6865 206f 626a 6563 7420 6973 2069 6e73  he object is ins
+000004b0: 7461 6e74 6961 7465 642e 2049 6620 7061  tantiated. If pa
+000004c0: 7373 6564 2c20 7265 7475 726e 7320 7468  ssed, returns th
+000004d0: 6520 6f75 7470 7574 206f 6620 7468 6520  e output of the 
+000004e0: 6f62 6a65 6374 206d 6574 686f 640a 606d  object method.`m
+000004f0: 6574 686f 645f 6172 6773 6020 616e 6420  ethod_args` and 
+00000500: 606d 6574 686f 645f 6b77 6172 6773 6020  `method_kwargs` 
+00000510: 6172 6520 7061 7373 6564 2064 6972 6563  are passed direc
+00000520: 746c 7920 696e 746f 2074 6865 206f 626a  tly into the obj
+00000530: 6563 7420 6d65 7468 6f64 2e20 0a0a 0a0a  ect method. ....
+00000540: 0a0a 0a0a 0a                             .....
```

### Comparing `liteobj-0.0.2/liteobj/lite.py` & `liteobj-0.0.3/liteobj/lite.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,115 @@
-from importlib import import_module, reload
+from importlib import import_module
 from fire import Fire
 from omegaconf import OmegaConf, DictConfig
 from typing import Any
 import sys
 import os
-
-# originally inspired by object instantiation code found in https://github.com/CompVis/taming-transformers. 
-# added logic to recursively instantiate objects used as parameters, and recursively load omegaconfigs from yaml files to support superconfigs
+from time import time
+from pathlib import Path
 
 SUPER_CONFIG_KEY = 'super'
+CLASS_STRING = 'class_string' 
 
-OBJECT_PARAM_KEY = 'object_params'
-CLASS_NAME_KEY = 'target' 
-PARAM_KEY = 'params'
+KWARGS = 'kwargs'
+ARGS = 'args'
 METHOD_KEY = 'method'
 
-CONFIG_PATH_KEY = '_source_config_path'
+METADATA_KEY = 'lite_metadata'
+
 
+# compile function source and assign object to target_name
+def compile_callable(source, target_name=None):
 
-# load omegaconfig from string filepath to yaml file
-# if omegaconfig has SUPER_CONFIG_KEY key, recursively load omegaconfigs from corresponding value, which should be list of yaml filepaths to superconfigs
+    ldict = {}
+    exec(source, globals(), ldict)
+
+    if target_name:
+        return ldict[target_name]
+    else:
+        for v in ldict.values():
+            if callable(v):
+                return v
+
+# pack args and kwargs into a list
+def listify(*args, **kwargs):
+    return [*args, *kwargs.values()]
+
+# computes class_string for class object
+def get_class_string(_class):
+    return f'{_class.__module__}.{_class.__name__}'
+
+# recursively load config with superconfigs
 def load_config(yaml_file: str) -> DictConfig:
 
     config = OmegaConf.load(yaml_file)
 
     if SUPER_CONFIG_KEY in config:
         super_configs = []
         for super_config in config[SUPER_CONFIG_KEY]:
             super_configs.append(load_config(super_config))
         config = OmegaConf.unsafe_merge(*super_configs, config)
         
     return config
 
+# recursively instantiate objects that have objects as parameters
+def instantiate(config: OmegaConf) -> Any:
 
-# instantiate object(s) specified by omegaconfig 
-# if omegaconfig contains OBJECT_PARAM_KEY key, recursively instantiate objects from corresponding value, which should also be an omegaconfig
-def instantiate_from_config(config: OmegaConf) -> Any:
-
-    object_params = {}
-    if OBJECT_PARAM_KEY in config:
-        for object_name, object_config in config[OBJECT_PARAM_KEY].items():
-            object_params[object_name] = instantiate_from_config(object_config)
-
-    module_string, class_string = config[CLASS_NAME_KEY].rsplit(".", 1)
-    if module_string in sys.modules:
-        module = reload(sys.modules[module_string])
-    else:
-        module = import_module(module_string)
-    module_class = getattr(module, class_string)
+    class_string = config.get(CLASS_STRING, None)
+    if class_string is None:
+        raise ValueError(f"Cannot instantiate object without '{CLASS_STRING}' key")
+    
+    module_name, class_name = class_string.rsplit(".", 1)
+    module = import_module(module_name)
+    module_class = getattr(module, class_name)
+
+    kwargs = {}
+    if KWARGS in config:
+        for k, v in config[KWARGS].items():
+            kwargs[k] = instantiate(v) if isinstance(config[KWARGS][k], DictConfig) else v
+ 
+    args = []
+    if ARGS in config:
+        for item in config[ARGS]:
+            args.append(instantiate(item)) if isinstance(item, DictConfig) else args.append(item)
 
-    # allow instantiation options like huggingface from_pretrained, instead of standard __init__
-    # method should not use super(), see https://stackoverflow.com/questions/12047847/super-object-not-calling-getattr
-    method_string = config.get(METHOD_KEY, '__init__') 
+
+    # allow custom instantiation method
+    method_string = config.get(METHOD_KEY, '__init__')
     if method_string is None:
         return module_class
-    elif method_string == '__init__':
-        return module_class(**config.get(PARAM_KEY, dict()), **object_params)
-    method = getattr(module_class, method_string)
-    return method(**config.get(PARAM_KEY, dict()), **object_params)
-
-# instantiate object from yaml file, then run object method specified in method_string. 
-# convenience function to run pytorch-lightning trainer methods from terminal
-# i.e. to train, run "">> python lite.py path/to/omegaconfig.yaml fit"
-def run(yaml_file: str, method_string: str=None, *args, **kwargs) -> Any:
 
-    # add current directory to path for importing local modules
+    # have to invoke __init__ method as special case due to nuances of python compiler
+    if method_string == '__init__':
+        return module_class(*args, **kwargs)
+    else:
+        method = getattr(module_class, method_string)
+        return method(*args, **kwargs)
+
+# convenience method for running object from yaml
+def run(yaml_file: str, method_string: str=None, *args, **kwargs) -> Any:
     sys.path.append(os.getcwd()) 
 
     config = load_config(yaml_file)
-    object = instantiate_from_config(config)
 
-    # attach source config path to object, avoid invoking unpredictable __setattr__ logic
-    vars(object).update({CONFIG_PATH_KEY: yaml_file}) 
+    metadata = dict(config.get(METADATA_KEY, {}))
+    metadata["config_path"] = str(Path(yaml_file).resolve())
+    metadata["time"] = time()
+
+    object = instantiate(config)
+    # this bypasses setattr checks against assigning object attributes
+    vars(object).update(metadata) 
     
+    #config[METADATA_KEY] = metadata
+    #OmegaConf.save(config=config, f=yaml_file)
+
     if method_string is None:
         return object
+    
+    # if method string is defined, run instantiated object method with args and kwargs
     try:
         method = getattr(object, method_string)
         return object, method(*args, **kwargs)
     except KeyboardInterrupt:
         return object, None
 
 def main():
```

### Comparing `liteobj-0.0.2/setup.py` & `liteobj-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 00000060: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
 00000070: 6d65 6e74 7320 3d20 6f70 656e 2866 227b  ments = open(f"{
 00000080: 7265 706f 5f6e 616d 657d 2f7b 7265 7175  repo_name}/{requ
 00000090: 6972 656d 656e 7473 5f66 6e7d 2229 2e72  irements_fn}").r
 000000a0: 6561 6428 292e 7370 6c69 7428 290d 0a0d  ead().split()...
 000000b0: 0a73 6574 7570 286e 616d 653d 7265 706f  .setup(name=repo
 000000c0: 5f6e 616d 652c 0d0a 2020 2020 2020 7665  _name,..      ve
-000000d0: 7273 696f 6e3d 2730 2e30 2e32 272c 0d0a  rsion='0.0.2',..
+000000d0: 7273 696f 6e3d 2730 2e30 2e33 272c 0d0a  rsion='0.0.3',..
 000000e0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
 000000f0: 6e3d 2743 7265 6174 6520 6c69 6768 7477  n='Create lightw
 00000100: 6569 6768 7420 636f 6e66 6967 7320 666f  eight configs fo
 00000110: 7220 696e 7374 616e 7469 6174 696e 6720  r instantiating 
 00000120: 4d4c 2065 7870 6572 696d 656e 7473 272c  ML experiments',
 00000130: 0d0a 2020 2020 2020 6175 7468 6f72 3d27  ..      author='
 00000140: 316c 696e 7427 2c0d 0a20 2020 2020 2061  1lint',..      a
```

