# Comparing `tmp/django-solo-2.0.0.tar.gz` & `tmp/django-solo-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-solo-2.0.0.tar", last modified: Mon Dec 13 07:46:38 2021, max compression
+gzip compressed data, was "django-solo-2.1.0.tar", last modified: Thu May 25 23:25:44 2023, max compression
```

## Comparing `django-solo-2.0.0.tar` & `django-solo-2.1.0.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2021-12-13 07:46:38.501114 django-solo-2.0.0/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     3230 2021-12-13 07:45:42.000000 django-solo-2.0.0/CHANGES
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      262 2021-12-13 07:45:42.000000 django-solo-2.0.0/LICENSE
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      120 2021-12-13 07:45:42.000000 django-solo-2.0.0/MANIFEST.in
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     8696 2021-12-13 07:46:38.501114 django-solo-2.0.0/PKG-INFO
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     7814 2021-12-13 07:45:42.000000 django-solo-2.0.0/README.md
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2021-12-13 07:46:38.497113 django-solo-2.0.0/django_solo.egg-info/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     8696 2021-12-13 07:46:38.000000 django-solo-2.0.0/django_solo.egg-info/PKG-INFO
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      641 2021-12-13 07:46:38.000000 django-solo-2.0.0/django_solo.egg-info/SOURCES.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        1 2021-12-13 07:46:38.000000 django-solo-2.0.0/django_solo.egg-info/dependency_links.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        1 2021-12-13 07:46:38.000000 django-solo-2.0.0/django_solo.egg-info/not-zip-safe
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       12 2021-12-13 07:46:38.000000 django-solo-2.0.0/django_solo.egg-info/requires.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        5 2021-12-13 07:46:38.000000 django-solo-2.0.0/django_solo.egg-info/top_level.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       38 2021-12-13 07:46:38.501114 django-solo-2.0.0/setup.cfg
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1674 2021-12-13 07:45:42.000000 django-solo-2.0.0/setup.py
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2021-12-13 07:46:38.497113 django-solo-2.0.0/solo/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      239 2021-12-13 07:45:42.000000 django-solo-2.0.0/solo/__init__.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     3437 2021-12-13 07:45:42.000000 django-solo-2.0.0/solo/admin.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      112 2021-12-13 07:45:42.000000 django-solo-2.0.0/solo/apps.py
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2021-12-13 07:46:38.497113 django-solo-2.0.0/solo/locale/
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2021-12-13 07:46:38.497113 django-solo-2.0.0/solo/locale/es/
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2021-12-13 07:46:38.501114 django-solo-2.0.0/solo/locale/es/LC_MESSAGES/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1048 2021-12-13 07:45:42.000000 django-solo-2.0.0/solo/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1731 2021-12-13 07:45:42.000000 django-solo-2.0.0/solo/locale/es/LC_MESSAGES/django.po
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     2090 2021-12-13 07:45:42.000000 django-solo-2.0.0/solo/models.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      489 2021-12-13 07:45:42.000000 django-solo-2.0.0/solo/settings.py
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2021-12-13 07:46:38.497113 django-solo-2.0.0/solo/templates/
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2021-12-13 07:46:38.497113 django-solo-2.0.0/solo/templates/admin/
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2021-12-13 07:46:38.501114 django-solo-2.0.0/solo/templates/admin/solo/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      726 2021-12-13 07:45:42.000000 django-solo-2.0.0/solo/templates/admin/solo/change_form.html
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      431 2021-12-13 07:45:42.000000 django-solo-2.0.0/solo/templates/admin/solo/object_history.html
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2021-12-13 07:46:38.501114 django-solo-2.0.0/solo/templatetags/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        0 2021-12-13 07:45:42.000000 django-solo-2.0.0/solo/templatetags/__init__.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1024 2021-12-13 07:45:42.000000 django-solo-2.0.0/solo/templatetags/solo_tags.py
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2021-12-13 07:46:38.501114 django-solo-2.0.0/solo/tests/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        0 2021-12-13 07:45:42.000000 django-solo-2.0.0/solo/tests/__init__.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      762 2021-12-13 07:45:42.000000 django-solo-2.0.0/solo/tests/models.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      897 2021-12-13 07:45:42.000000 django-solo-2.0.0/solo/tests/settings.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     4568 2021-12-13 07:45:42.000000 django-solo-2.0.0/solo/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:25:44.948317 django-solo-2.1.0/
+-rw-rw-rw-   0        0        0     3622 2023-05-25 23:21:47.000000 django-solo-2.1.0/CHANGES
+-rw-rw-rw-   0        0        0      271 2023-05-25 23:10:10.000000 django-solo-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0      125 2023-05-25 23:10:10.000000 django-solo-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9223 2023-05-25 23:25:44.947317 django-solo-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8297 2023-05-25 23:21:47.000000 django-solo-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 23:25:44.931320 django-solo-2.1.0/django_solo.egg-info/
+-rw-rw-rw-   0        0        0     9223 2023-05-25 23:25:44.000000 django-solo-2.1.0/django_solo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-05-25 23:25:44.000000 django-solo-2.1.0/django_solo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 23:25:44.000000 django-solo-2.1.0/django_solo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-25 23:25:44.000000 django-solo-2.1.0/django_solo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-05-25 23:25:44.000000 django-solo-2.1.0/django_solo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-25 23:25:44.000000 django-solo-2.1.0/django_solo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 23:25:44.948317 django-solo-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1769 2023-05-25 23:11:17.000000 django-solo-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:25:44.935318 django-solo-2.1.0/solo/
+-rw-rw-rw-   0        0        0      248 2023-05-25 23:25:19.000000 django-solo-2.1.0/solo/__init__.py
+-rw-rw-rw-   0        0        0     3529 2023-05-25 23:10:10.000000 django-solo-2.1.0/solo/admin.py
+-rw-rw-rw-   0        0        0      118 2023-05-25 23:10:10.000000 django-solo-2.1.0/solo/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:25:44.919317 django-solo-2.1.0/solo/locale/
+drwxrwxrwx   0        0        0        0 2023-05-25 23:25:44.918317 django-solo-2.1.0/solo/locale/de/
+drwxrwxrwx   0        0        0        0 2023-05-25 23:25:44.937317 django-solo-2.1.0/solo/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1086 2023-05-25 23:10:10.000000 django-solo-2.1.0/solo/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     1783 2023-05-25 23:10:10.000000 django-solo-2.1.0/solo/locale/de/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-05-25 23:25:44.919317 django-solo-2.1.0/solo/locale/es/
+drwxrwxrwx   0        0        0        0 2023-05-25 23:25:44.939317 django-solo-2.1.0/solo/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1048 2023-05-25 23:10:10.000000 django-solo-2.1.0/solo/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     1788 2023-05-25 23:10:10.000000 django-solo-2.1.0/solo/locale/es/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     2153 2023-05-25 23:10:10.000000 django-solo-2.1.0/solo/models.py
+-rw-rw-rw-   0        0        0      506 2023-05-25 23:10:10.000000 django-solo-2.1.0/solo/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:25:44.919317 django-solo-2.1.0/solo/templates/
+drwxrwxrwx   0        0        0        0 2023-05-25 23:25:44.919317 django-solo-2.1.0/solo/templates/admin/
+drwxrwxrwx   0        0        0        0 2023-05-25 23:25:44.941325 django-solo-2.1.0/solo/templates/admin/solo/
+-rw-rw-rw-   0        0        0      748 2023-05-25 23:10:10.000000 django-solo-2.1.0/solo/templates/admin/solo/change_form.html
+-rw-rw-rw-   0        0        0      446 2023-05-25 23:10:10.000000 django-solo-2.1.0/solo/templates/admin/solo/object_history.html
+drwxrwxrwx   0        0        0        0 2023-05-25 23:25:44.942318 django-solo-2.1.0/solo/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-05-25 23:10:10.000000 django-solo-2.1.0/solo/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     1058 2023-05-25 23:10:10.000000 django-solo-2.1.0/solo/templatetags/solo_tags.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:25:44.946318 django-solo-2.1.0/solo/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-25 23:10:10.000000 django-solo-2.1.0/solo/tests/__init__.py
+-rw-rw-rw-   0        0        0      788 2023-05-25 23:10:10.000000 django-solo-2.1.0/solo/tests/models.py
+-rw-rw-rw-   0        0        0      936 2023-05-25 23:10:10.000000 django-solo-2.1.0/solo/tests/settings.py
+-rw-rw-rw-   0        0        0     4673 2023-05-25 23:10:10.000000 django-solo-2.1.0/solo/tests/tests.py
```

### Comparing `django-solo-2.0.0/PKG-INFO` & `django-solo-2.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,544 +1,577 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 616e  : 2.1.Name: djan
-00000020: 676f 2d73 6f6c 6f0a 5665 7273 696f 6e3a  go-solo.Version:
-00000030: 2032 2e30 2e30 0a53 756d 6d61 7279 3a20   2.0.0.Summary: 
-00000040: 446a 616e 676f 2053 6f6c 6f20 6865 6c70  Django Solo help
-00000050: 7320 776f 726b 696e 6720 7769 7468 2073  s working with s
-00000060: 696e 676c 6574 6f6e 730a 486f 6d65 2d70  ingletons.Home-p
-00000070: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
-00000080: 6875 622e 636f 6d2f 6c61 7a79 6269 7264  hub.com/lazybird
-00000090: 2f64 6a61 6e67 6f2d 736f 6c6f 2f0a 4175  /django-solo/.Au
-000000a0: 7468 6f72 3a20 6c61 7a79 6269 7264 0a4c  thor: lazybird.L
-000000b0: 6963 656e 7365 3a20 4372 6561 7469 7665  icense: Creative
-000000c0: 2043 6f6d 6d6f 6e73 2041 7474 7269 6275   Commons Attribu
-000000d0: 7469 6f6e 2033 2e30 2055 6e70 6f72 7465  tion 3.0 Unporte
-000000e0: 640a 506c 6174 666f 726d 3a20 554e 4b4e  d.Platform: UNKN
-000000f0: 4f57 4e0a 436c 6173 7369 6669 6572 3a20  OWN.Classifier: 
-00000100: 4672 616d 6577 6f72 6b20 3a3a 2044 6a61  Framework :: Dja
-00000110: 6e67 6f20 3a3a 2032 2e32 0a43 6c61 7373  ngo :: 2.2.Class
-00000120: 6966 6965 723a 2046 7261 6d65 776f 726b  ifier: Framework
-00000130: 203a 3a20 446a 616e 676f 203a 3a20 332e   :: Django :: 3.
-00000140: 320a 436c 6173 7369 6669 6572 3a20 4672  2.Classifier: Fr
-00000150: 616d 6577 6f72 6b20 3a3a 2044 6a61 6e67  amework :: Djang
-00000160: 6f20 3a3a 2034 2e30 0a43 6c61 7373 6966  o :: 4.0.Classif
-00000170: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
-00000180: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
-00000190: 7065 7273 0a43 6c61 7373 6966 6965 723a  pers.Classifier:
-000001a0: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-000001b0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-000001c0: 656e 740a 436c 6173 7369 6669 6572 3a20  ent.Classifier: 
-000001d0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001e0: 7561 6765 203a 3a20 5079 7468 6f6e 0a43  uage :: Python.C
-000001f0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000200: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000210: 3a3a 2050 7974 686f 6e20 3a3a 2033 0a43  :: Python :: 3.C
-00000220: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000230: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000240: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e36  :: Python :: 3.6
-00000250: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000260: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000270: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000280: 2e37 0a43 6c61 7373 6966 6965 723a 2050  .7.Classifier: P
-00000290: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002a0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002b0: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
-000002c0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000002d0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000002e0: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
-000002f0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000300: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000310: 6e20 3a3a 2033 2e31 300a 5265 7175 6972  n :: 3.10.Requir
-00000320: 6573 2d50 7974 686f 6e3a 203e 3d33 2e36  es-Python: >=3.6
-00000330: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-00000340: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-00000350: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
-00000360: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
-00000370: 0a44 6a61 6e67 6f20 536f 6c6f 0a3d 3d3d  .Django Solo.===
-00000380: 3d3d 3d3d 3d3d 3d3d 0a0a 3c61 2068 7265  ========..<a hre
-00000390: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
-000003a0: 6f72 672f 7072 6f6a 6563 742f 646a 616e  org/project/djan
-000003b0: 676f 2d73 6f6c 6f2f 2220 616c 743d 2243  go-solo/" alt="C
-000003c0: 7572 7265 6e74 2076 6572 7369 6f6e 206f  urrent version o
-000003d0: 6e20 5079 5069 223e 3c69 6d67 2073 7263  n PyPi"><img src
-000003e0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-000003f0: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
-00000400: 646a 616e 676f 2d73 6f6c 6f2e 7376 6722  django-solo.svg"
-00000410: 202f 3e3c 2f61 3e0a 0a0a 2020 2020 2b2d   /></a>...    +-
-00000420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000430: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  ----------+.    
-00000440: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00000450: 2020 2020 2020 2020 2020 2020 7c0a 2020              |.  
-00000460: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00000470: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00000480: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00000490: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
-000004a0: 7c20 446a 616e 676f 2053 6f6c 6f20 6865  | Django Solo he
-000004b0: 6c70 7320 776f 726b 696e 6720 7769 7468  lps working with
-000004c0: 2073 696e 676c 6574 6f6e 733a 0a20 2020   singletons:.   
-000004d0: 207c 2020 2020 2020 2020 2020 2020 202f   |             /
-000004e0: 5c20 2020 2020 2020 2020 2020 207c 2064  \            | d
-000004f0: 6174 6162 6173 6520 7461 626c 6573 2074  atabase tables t
-00000500: 6861 7420 6f6e 6c79 2068 6176 6520 6f6e  hat only have on
-00000510: 6520 726f 772e 0a20 2020 207c 2020 2020  e row..    |    
-00000520: 2020 2020 2020 203e 3d29 273e 2020 2020         >=)'>    
-00000530: 2020 2020 2020 207c 2053 696e 676c 6574         | Singlet
-00000540: 6f6e 7320 6172 6520 7573 6566 756c 2066  ons are useful f
-00000550: 6f72 2074 6869 6e67 7320 6c69 6b65 2067  or things like g
-00000560: 6c6f 6261 6c0a 2020 2020 7c20 2020 2020  lobal.    |     
-00000570: 2020 2020 2020 2020 5c2f 2020 2020 2020          \/      
-00000580: 2020 2020 2020 7c20 7365 7474 696e 6773        | settings
-00000590: 2074 6861 7420 796f 7520 7761 6e74 2074   that you want t
-000005a0: 6f20 6564 6974 2066 726f 6d20 7468 6520  o edit from the 
-000005b0: 6164 6d69 6e0a 2020 2020 7c20 2020 2020  admin.    |     
-000005c0: 2020 2020 2020 2020 2f20 2020 2020 2020          /       
-000005d0: 2020 2020 2020 7c20 696e 7374 6561 6420        | instead 
-000005e0: 6f66 2068 6176 696e 6720 7468 656d 2069  of having them i
-000005f0: 6e20 446a 616e 676f 2073 6574 7469 6e67  n Django setting
-00000600: 732e 7079 2e0a 2020 2020 7c20 2020 2020  s.py..    |     
-00000610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000620: 2020 2020 2020 7c20 0a20 2020 207c 2020        | .    |  
-00000630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000640: 2020 2020 2020 2020 207c 200a 2020 2020           | .    
-00000650: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00000660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 0a0a  ------------+...
-00000670: 4665 6174 7572 6573 0a2d 2d2d 2d2d 2d2d  Features.-------
-00000680: 2d0a 0a53 6f6c 6f20 6865 6c70 7320 796f  -..Solo helps yo
-00000690: 7520 656e 666f 7263 6520 696e 7374 616e  u enforce instan
-000006a0: 7469 6174 696e 6720 6f6e 6c79 206f 6e65  tiating only one
-000006b0: 2069 6e73 7461 6e63 6520 6f66 2061 206d   instance of a m
-000006c0: 6f64 656c 2069 6e20 646a 616e 676f 2e0a  odel in django..
-000006d0: 0a2a 2059 6f75 2064 6566 696e 6520 7468  .* You define th
-000006e0: 6520 6d6f 6465 6c20 7468 6174 2077 696c  e model that wil
-000006f0: 6c20 686f 6c64 2079 6f75 7220 7369 6e67  l hold your sing
-00000700: 6c65 746f 6e20 6f62 6a65 6374 2e0a 2a20  leton object..* 
-00000710: 646a 616e 676f 2d73 6f6c 6f20 6769 7665  django-solo give
-00000720: 7320 6865 6c70 6572 2070 6172 656e 7420  s helper parent 
-00000730: 636c 6173 7320 666f 7220 796f 7572 206d  class for your m
-00000740: 6f64 656c 2061 6e64 2074 6865 2061 646d  odel and the adm
-00000750: 696e 2063 6c61 7373 6573 2e0a 2a20 596f  in classes..* Yo
-00000760: 7520 6765 7420 616e 2061 646d 696e 2069  u get an admin i
-00000770: 6e74 6572 6661 6365 2074 6861 7427 7320  nterface that's 
-00000780: 6177 6172 6520 796f 7520 6f6e 6c79 2068  aware you only h
-00000790: 6176 6520 6f6e 6520 6f62 6a65 6374 2e0a  ave one object..
-000007a0: 2a20 596f 7520 6361 6e20 7265 7472 6965  * You can retrie
-000007b0: 7665 2074 6865 206f 626a 6563 7420 6672  ve the object fr
-000007c0: 6f6d 2074 656d 706c 6174 6573 2e0a 2a20  om templates..* 
-000007d0: 4279 2065 6e61 626c 696e 6720 6361 6368  By enabling cach
-000007e0: 696e 672c 2074 6865 2064 6174 6162 6173  ing, the databas
-000007f0: 6520 6973 206e 6f74 2071 7565 7269 6564  e is not queried
-00000800: 2069 6e74 656e 7369 7665 6c79 2e0a 0a55   intensively...U
-00000810: 7365 2043 6173 6573 0a2d 2d2d 2d2d 2d2d  se Cases.-------
-00000820: 2d0a 0a44 6a61 6e67 6f20 536f 6c6f 2069  -..Django Solo i
-00000830: 7320 616c 736f 2067 7265 6174 2066 6f72  s also great for
-00000840: 2075 7365 2077 6974 6820 7369 6e67 6c65   use with single
-00000850: 746f 6e20 6f62 6a65 6374 7320 7468 6174  ton objects that
-00000860: 2068 6176 6520 6120 6f6e 6520 746f 206d   have a one to m
-00000870: 616e 7920 7265 6c61 7469 6f6e 7368 6970  any relationship
-00000880: 2e20 4c69 6b65 2074 6865 2075 7365 2063  . Like the use c
-00000890: 6173 6520 6265 6c6f 7720 7768 6572 6520  ase below where 
-000008a0: 796f 7520 6861 7665 2061 2027 486f 6d65  you have a 'Home
-000008b0: 2053 6c69 6465 7222 2074 6861 7420 6861   Slider" that ha
-000008c0: 7320 6d61 6e79 2022 536c 6964 6573 222e  s many "Slides".
-000008d0: 0a0a 2a20 476c 6f62 616c 206f 7220 6465  ..* Global or de
-000008e0: 6661 756c 7420 7365 7474 696e 6773 0a2a  fault settings.*
-000008f0: 2041 6e20 696d 6167 6520 736c 6964 6572   An image slider
-00000900: 2074 6861 7420 6861 7320 6d61 6e79 2073   that has many s
-00000910: 6c69 6465 730a 2a20 4120 7061 6765 2073  lides.* A page s
-00000920: 6563 7469 6f6e 2074 6861 7420 6861 7320  ection that has 
-00000930: 7375 622d 7365 6374 696f 6e73 0a2a 2041  sub-sections.* A
-00000940: 2074 6561 6d20 6269 6f20 7769 7468 206d   team bio with m
-00000950: 616e 7920 7465 616d 206d 656d 6265 7273  any team members
-00000960: 0a0a 5468 6572 6520 6172 6520 6d61 6e79  ..There are many
-00000970: 2063 6173 6573 2077 6865 7265 2069 7420   cases where it 
-00000980: 6d61 6b65 7320 7365 6e73 6520 666f 7220  makes sense for 
-00000990: 7468 6520 7061 7265 6e74 2069 6e20 6120  the parent in a 
-000009a0: 6f6e 6520 746f 206d 616e 7920 7265 6c61  one to many rela
-000009b0: 7469 6f6e 7368 6970 2074 6f20 6265 206c  tionship to be l
-000009c0: 696d 6974 6564 2074 6f20 6120 7369 6e67  imited to a sing
-000009d0: 6c65 2069 6e73 7461 6e63 652e 0a0a 5573  le instance...Us
-000009e0: 6167 6520 4578 616d 706c 650a 0a60 6060  age Example..```
-000009f0: 7079 7468 6f6e 0a23 206d 6f64 656c 732e  python.# models.
-00000a00: 7079 0a0a 6672 6f6d 2064 6a61 6e67 6f2e  py..from django.
-00000a10: 6462 2069 6d70 6f72 7420 6d6f 6465 6c73  db import models
-00000a20: 0a66 726f 6d20 736f 6c6f 2e6d 6f64 656c  .from solo.model
-00000a30: 7320 696d 706f 7274 2053 696e 676c 6574  s import Singlet
-00000a40: 6f6e 4d6f 6465 6c0a 0a0a 636c 6173 7320  onModel...class 
-00000a50: 5369 7465 436f 6e66 6967 7572 6174 696f  SiteConfiguratio
-00000a60: 6e28 5369 6e67 6c65 746f 6e4d 6f64 656c  n(SingletonModel
-00000a70: 293a 0a20 2020 2073 6974 655f 6e61 6d65  ):.    site_name
-00000a80: 203d 206d 6f64 656c 732e 4368 6172 4669   = models.CharFi
-00000a90: 656c 6428 6d61 785f 6c65 6e67 7468 3d32  eld(max_length=2
-00000aa0: 3535 2c20 6465 6661 756c 743d 2753 6974  55, default='Sit
-00000ab0: 6520 4e61 6d65 2729 0a20 2020 206d 6169  e Name').    mai
-00000ac0: 6e74 656e 616e 6365 5f6d 6f64 6520 3d20  ntenance_mode = 
-00000ad0: 6d6f 6465 6c73 2e42 6f6f 6c65 616e 4669  models.BooleanFi
-00000ae0: 656c 6428 6465 6661 756c 743d 4661 6c73  eld(default=Fals
-00000af0: 6529 0a0a 2020 2020 6465 6620 5f5f 7374  e)..    def __st
-00000b00: 725f 5f28 7365 6c66 293a 0a20 2020 2020  r__(self):.     
-00000b10: 2020 2072 6574 7572 6e20 2253 6974 6520     return "Site 
-00000b20: 436f 6e66 6967 7572 6174 696f 6e22 0a0a  Configuration"..
-00000b30: 2020 2020 636c 6173 7320 4d65 7461 3a0a      class Meta:.
-00000b40: 2020 2020 2020 2020 7665 7262 6f73 655f          verbose_
-00000b50: 6e61 6d65 203d 2022 5369 7465 2043 6f6e  name = "Site Con
-00000b60: 6669 6775 7261 7469 6f6e 220a 6060 600a  figuration".```.
-00000b70: 0a60 6060 7079 7468 6f6e 0a23 2061 646d  .```python.# adm
-00000b80: 696e 2e70 790a 0a66 726f 6d20 646a 616e  in.py..from djan
-00000b90: 676f 2e63 6f6e 7472 6962 2069 6d70 6f72  go.contrib impor
-00000ba0: 7420 6164 6d69 6e0a 6672 6f6d 2073 6f6c  t admin.from sol
-00000bb0: 6f2e 6164 6d69 6e20 696d 706f 7274 2053  o.admin import S
-00000bc0: 696e 676c 6574 6f6e 4d6f 6465 6c41 646d  ingletonModelAdm
-00000bd0: 696e 0a66 726f 6d20 636f 6e66 6967 2e6d  in.from config.m
-00000be0: 6f64 656c 7320 696d 706f 7274 2053 6974  odels import Sit
-00000bf0: 6543 6f6e 6669 6775 7261 7469 6f6e 0a0a  eConfiguration..
-00000c00: 0a61 646d 696e 2e73 6974 652e 7265 6769  .admin.site.regi
-00000c10: 7374 6572 2853 6974 6543 6f6e 6669 6775  ster(SiteConfigu
-00000c20: 7261 7469 6f6e 2c20 5369 6e67 6c65 746f  ration, Singleto
-00000c30: 6e4d 6f64 656c 4164 6d69 6e29 0a60 6060  nModelAdmin).```
-00000c40: 0a0a 6060 6070 7974 686f 6e0a 2320 5468  ..```python.# Th
-00000c50: 6572 6520 6973 206f 6e6c 7920 6f6e 6520  ere is only one 
-00000c60: 6974 656d 2069 6e20 7468 6520 7461 626c  item in the tabl
-00000c70: 652c 2079 6f75 2063 616e 2067 6574 2069  e, you can get i
-00000c80: 7420 7468 6973 2077 6179 3a0a 6672 6f6d  t this way:.from
-00000c90: 202e 6d6f 6465 6c73 2069 6d70 6f72 7420   .models import 
-00000ca0: 5369 7465 436f 6e66 6967 7572 6174 696f  SiteConfiguratio
-00000cb0: 6e0a 636f 6e66 6967 203d 2053 6974 6543  n.config = SiteC
-00000cc0: 6f6e 6669 6775 7261 7469 6f6e 2e6f 626a  onfiguration.obj
-00000cd0: 6563 7473 2e67 6574 2829 0a0a 2320 6765  ects.get()..# ge
-00000ce0: 745f 736f 6c6f 2077 696c 6c20 6372 6561  t_solo will crea
-00000cf0: 7465 2074 6865 2069 7465 6d20 6966 2069  te the item if i
-00000d00: 7420 646f 6573 206e 6f74 2061 6c72 6561  t does not alrea
-00000d10: 6479 2065 7869 7374 0a63 6f6e 6669 6720  dy exist.config 
-00000d20: 3d20 5369 7465 436f 6e66 6967 7572 6174  = SiteConfigurat
-00000d30: 696f 6e2e 6765 745f 736f 6c6f 2829 0a60  ion.get_solo().`
-00000d40: 6060 0a0a 496e 2079 6f75 7220 6d6f 6465  ``..In your mode
-00000d50: 6c2c 206e 6f74 6520 686f 7720 796f 7520  l, note how you 
-00000d60: 6469 6420 6e6f 7420 6861 7665 2074 6f20  did not have to 
-00000d70: 7072 6f76 6964 6520 6120 6076 6572 626f  provide a `verbo
-00000d80: 7365 5f6e 616d 655f 706c 7572 616c 6020  se_name_plural` 
-00000d90: 6669 656c 6420 2d0a 5468 6174 2773 2062  field -.That's b
-00000da0: 6563 6175 7365 2044 6a61 6e67 6f20 536f  ecause Django So
-00000db0: 6c6f 2075 7365 7320 7468 6520 6076 6572  lo uses the `ver
-00000dc0: 626f 7365 5f6e 616d 6560 2069 6e73 7465  bose_name` inste
-00000dd0: 6164 2e0a 0a49 6620 796f 7527 7265 2063  ad...If you're c
-00000de0: 6861 6e67 696e 6720 616e 2065 7869 7374  hanging an exist
-00000df0: 696e 6720 6d6f 6465 6c20 2877 6869 6368  ing model (which
-00000e00: 2061 6c72 6561 6479 2068 6173 2073 6f6d   already has som
-00000e10: 6520 6f62 6a65 6374 7320 7374 6f72 6564  e objects stored
-00000e20: 2069 6e20 7468 6520 6461 7461 6261 7365   in the database
-00000e30: 2920 746f 2061 2073 696e 676c 6574 6f6e  ) to a singleton
-00000e40: 206d 6f64 656c 2c20 796f 7520 6361 6e20   model, you can 
-00000e50: 6578 706c 6963 6974 6c79 2070 726f 7669  explicitly provi
-00000e60: 6465 2074 6865 2069 6420 6f66 2074 6865  de the id of the
-00000e70: 2072 6f77 2069 6e20 7468 6520 6461 7461   row in the data
-00000e80: 6261 7365 2066 6f72 2064 6a61 6e67 6f2d  base for django-
-00000e90: 736f 6c6f 2074 6f20 7573 652e 2054 6869  solo to use. Thi
-00000ea0: 7320 6361 6e20 6265 2064 6f6e 6520 6279  s can be done by
-00000eb0: 2073 6574 7469 6e67 2060 7369 6e67 6c65   setting `single
-00000ec0: 746f 6e5f 696e 7374 616e 6365 5f69 6460  ton_instance_id`
-00000ed0: 2070 726f 7065 7274 7920 6f6e 2074 6865   property on the
-00000ee0: 206d 6f64 656c 3a0a 0a60 6060 7079 7468   model:..```pyth
-00000ef0: 6f6e 0a63 6c61 7373 2053 6974 6543 6f6e  on.class SiteCon
-00000f00: 6669 6775 7261 7469 6f6e 2853 696e 676c  figuration(Singl
-00000f10: 6574 6f6e 4d6f 6465 6c29 3a0a 2020 2020  etonModel):.    
-00000f20: 7369 6e67 6c65 746f 6e5f 696e 7374 616e  singleton_instan
-00000f30: 6365 5f69 6420 3d20 3234 0a20 2020 2023  ce_id = 24.    #
-00000f40: 2028 2e2e 2e29 0a60 6060 0a0a 496e 7374   (...).```..Inst
-00000f50: 616c 6c61 7469 6f6e 0a2d 2d2d 2d2d 2d2d  allation.-------
-00000f60: 2d2d 2d2d 2d0a 0a54 6869 7320 6170 706c  -----..This appl
-00000f70: 6963 6174 696f 6e20 7265 7175 6972 6573  ication requires
-00000f80: 2044 6a61 6e67 6f20 322e 322c 2033 2e32   Django 2.2, 3.2
-00000f90: 2c20 6f72 2034 2e30 2e0a 0a2a 2049 6e73  , or 4.0...* Ins
-00000fa0: 7461 6c6c 2074 6865 2070 6163 6b61 6765  tall the package
-00000fb0: 2075 7369 6e67 2060 7069 7020 696e 7374   using `pip inst
-00000fc0: 616c 6c20 646a 616e 676f 2d73 6f6c 6f60  all django-solo`
-00000fd0: 0a2a 2041 6464 2060 6073 6f6c 6f60 6020  .* Add ``solo`` 
-00000fe0: 6f72 2060 6073 6f6c 6f2e 6170 7073 2e53  or ``solo.apps.S
-00000ff0: 6f6c 6f41 7070 436f 6e66 6967 6060 2074  oloAppConfig`` t
-00001000: 6f20 796f 7572 2060 6049 4e53 5441 4c4c  o your ``INSTALL
-00001010: 4544 5f41 5050 5360 6020 7365 7474 696e  ED_APPS`` settin
-00001020: 672e 0a0a 5468 6973 2069 7320 686f 7720  g...This is how 
-00001030: 796f 7520 7275 6e20 7465 7374 733a 0a0a  you run tests:..
-00001040: 2020 2020 2e2f 6d61 6e61 6765 2e70 7920      ./manage.py 
-00001050: 7465 7374 2073 6f6c 6f20 2d2d 7365 7474  test solo --sett
-00001060: 696e 6773 3d73 6f6c 6f2e 7465 7374 732e  ings=solo.tests.
-00001070: 7365 7474 696e 6773 0a0a 416e 6420 6672  settings..And fr
-00001080: 6f6d 2077 6974 6869 6e20 6074 6f78 603a  om within `tox`:
-00001090: 0a0a 6060 600a 7079 7468 6f6e 202d 6d20  ..```.python -m 
-000010a0: 7069 7020 696e 7374 616c 6c20 746f 780a  pip install tox.
-000010b0: 746f 780a 6060 600a 0a53 7570 706f 7274  tox.```..Support
-000010c0: 6564 204c 616e 6775 6167 6573 0a2d 2d2d  ed Languages.---
-000010d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000010e0: 0a0a 2d20 456e 676c 6973 680a 2d20 5370  ..- English.- Sp
-000010f0: 616e 6973 680a 0a41 646d 696e 0a2d 2d2d  anish..Admin.---
-00001100: 2d2d 0a0a 5468 6520 7374 616e 6461 7264  --..The standard
-00001110: 2044 6a61 6e67 6f20 6164 6d69 6e20 646f   Django admin do
-00001120: 6573 206e 6f74 2066 6974 2077 656c 6c20  es not fit well 
-00001130: 7768 656e 2077 6f72 6b69 6e67 2077 6974  when working wit
-00001140: 6820 7369 6e67 6c65 746f 6e2c 0a66 6f72  h singleton,.for
-00001150: 2069 6e73 7461 6e63 652c 2069 6620 796f   instance, if yo
-00001160: 7520 6e65 6564 2073 6f6d 6520 676c 6f62  u need some glob
-00001170: 616c 2073 6974 6520 7365 7474 696e 6773  al site settings
-00001180: 2074 6f20 6265 2065 6469 7465 6420 696e   to be edited in
-00001190: 2074 6865 2061 646d 696e 2e0a 446a 616e   the admin..Djan
-000011a0: 676f 2053 6f6c 6f20 7072 6f76 6964 6573  go Solo provides
-000011b0: 2061 206d 6f64 6966 6965 6420 6164 6d69   a modified admi
-000011c0: 6e20 666f 7220 7468 6174 2e0a 0a0a 215b  n for that....![
-000011d0: 646a 616e 676f 2d73 6f6c 6f20 6164 6d69  django-solo admi
-000011e0: 6e5d 2868 7474 7073 3a2f 2f72 6177 2e67  n](https://raw.g
-000011f0: 6974 6875 622e 636f 6d2f 6c61 7a79 6269  ithub.com/lazybi
-00001200: 7264 2f64 6a61 6e67 6f2d 736f 6c6f 2f6d  rd/django-solo/m
-00001210: 6173 7465 722f 646f 6373 2f69 6d61 6765  aster/docs/image
-00001220: 732f 646a 616e 676f 2d73 6f6c 6f2d 6164  s/django-solo-ad
-00001230: 6d69 6e2e 6a70 6720 2264 6a61 6e67 6f2d  min.jpg "django-
-00001240: 736f 6c6f 2061 646d 696e 2229 0a0a 0a2a  solo admin")...*
-00001250: 2049 6e20 7468 6520 6164 6d69 6e20 686f   In the admin ho
-00001260: 6d65 2070 6167 6520 7768 6572 6520 616c  me page where al
-00001270: 6c20 6170 706c 6963 6174 696f 6e73 2061  l applications a
-00001280: 7265 206c 6973 7465 642c 2077 6520 6861  re listed, we ha
-00001290: 7665 2061 2060 636f 6e66 6967 600a 2020  ve a `config`.  
-000012a0: 6170 706c 6963 6174 696f 6e20 7468 6174  application that
-000012b0: 2068 6f6c 6473 2061 2073 696e 676c 6574   holds a singlet
-000012c0: 6f6e 206d 6f64 656c 2066 6f72 2073 6974  on model for sit
-000012d0: 6520 636f 6e66 6967 7572 6174 696f 6e2e  e configuration.
-000012e0: 0a2a 2054 6865 2063 6f6e 6669 6775 7261  .* The configura
-000012f0: 7469 6f6e 206f 626a 6563 7420 6361 6e20  tion object can 
-00001300: 6f6e 6c79 2062 6520 6368 616e 6765 642c  only be changed,
-00001310: 2074 6865 7265 2773 206e 6f20 6c69 6e6b   there's no link
-00001320: 2066 6f72 2022 6164 6422 2028 3129 2e0a   for "add" (1)..
-00001330: 2a20 5468 6520 6c69 6e6b 2074 6f20 7468  * The link to th
-00001340: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
-00001350: 7061 6765 2028 3229 2064 6972 6563 746c  page (2) directl
-00001360: 7920 676f 6573 2074 6f20 7468 6520 666f  y goes to the fo
-00001370: 726d 2070 6167 6520 2d20 6e6f 0a20 206e  rm page - no.  n
-00001380: 6565 6420 666f 7220 616e 2069 6e74 6572  eed for an inter
-00001390: 6d65 6469 6172 7920 6f62 6a65 6374 206c  mediary object l
-000013a0: 6973 7420 7061 6765 2c20 7369 6e63 6520  ist page, since 
-000013b0: 7468 6572 6527 7320 6f6e 6c79 206f 6e65  there's only one
-000013c0: 206f 626a 6563 742e 0a2a 2054 6865 2065   object..* The e
-000013d0: 6469 7420 7061 6765 2068 6173 2061 206d  dit page has a m
-000013e0: 6f64 6966 6965 6420 6272 6561 6463 7275  odified breadcru
-000013f0: 6d62 2028 3329 2074 6f20 6176 6f69 6420  mb (3) to avoid 
-00001400: 6c69 6e6b 696e 6720 746f 2074 6865 0a20  linking to the. 
-00001410: 2069 6e74 6572 6d65 6469 6172 7920 6f62   intermediary ob
-00001420: 6a65 6374 206c 6973 7420 7061 6765 2e0a  ject list page..
-00001430: 2a20 4672 6f6d 2074 6865 2065 6469 7420  * From the edit 
-00001440: 7061 6765 2c20 7765 2063 616e 6e6f 7420  page, we cannot 
-00001450: 6465 6c65 7465 2074 6865 206f 626a 6563  delete the objec
-00001460: 7420 2834 2920 6e6f 7220 6361 6e20 7765  t (4) nor can we
-00001470: 2061 6464 2061 206e 6577 206f 6e65 2028   add a new one (
-00001480: 3529 2e0a 0a49 6620 796f 7520 7769 7368  5)...If you wish
-00001490: 2074 6f20 6469 7361 626c 6520 7468 6520   to disable the 
-000014a0: 736b 6970 7069 6e67 206f 6620 7468 6520  skipping of the 
-000014b0: 6f62 6a65 6374 206c 6973 7420 7061 6765  object list page
-000014c0: 2c20 616e 6420 6861 7665 2074 6865 2064  , and have the d
-000014d0: 6566 6175 6c74 0a62 7265 6164 6372 756d  efault.breadcrum
-000014e0: 6273 2c20 796f 7520 7368 6f75 6c64 2073  bs, you should s
-000014f0: 6574 2060 534f 4c4f 5f41 444d 494e 5f53  et `SOLO_ADMIN_S
-00001500: 4b49 505f 4f42 4a45 4354 5f4c 4953 545f  KIP_OBJECT_LIST_
-00001510: 5041 4745 6020 746f 2060 4661 6c73 6560  PAGE` to `False`
-00001520: 2069 6e20 796f 7572 2073 6574 7469 6e67   in your setting
-00001530: 732e 0a0a 4176 6169 6c61 6269 6c69 7479  s...Availability
-00001540: 2066 726f 6d20 7465 6d70 6c61 7465 730a   from templates.
-00001550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a54 6865  -----------..The
-00001570: 2073 696e 676c 6574 6f6e 206f 626a 6563   singleton objec
-00001580: 7420 6361 6e20 6265 2072 6574 7269 6576  t can be retriev
-00001590: 6564 2066 726f 6d20 7465 6d70 6c61 7465  ed from template
-000015a0: 2062 7920 6769 7669 6e67 2074 6865 2044   by giving the D
-000015b0: 6a61 6e67 6f20 6d6f 6465 6c0a 646f 7474  jango model.dott
-000015c0: 6564 2070 6174 683a 0a0a 6060 6064 6a61  ed path:..```dja
-000015d0: 6e67 6f0a 7b25 2067 6574 5f73 6f6c 6f20  ngo.{% get_solo 
-000015e0: 2761 7070 5f6c 6162 656c 2e4d 6f64 656c  'app_label.Model
-000015f0: 4e61 6d65 2720 6173 206d 795f 636f 6e66  Name' as my_conf
-00001600: 6967 2025 7d0a 6060 600a 0a45 7861 6d70  ig %}.```..Examp
-00001610: 6c65 3a0a 0a60 6060 646a 616e 676f 0a7b  le:..```django.{
-00001620: 2520 6c6f 6164 2073 6f6c 6f5f 7461 6773  % load solo_tags
-00001630: 2025 7d0a 7b25 2067 6574 5f73 6f6c 6f20   %}.{% get_solo 
-00001640: 2763 6f6e 6669 672e 5369 7465 436f 6e66  'config.SiteConf
-00001650: 6967 7572 6174 696f 6e27 2061 7320 7369  iguration' as si
-00001660: 7465 5f63 6f6e 6669 6720 257d 0a7b 7b20  te_config %}.{{ 
-00001670: 7369 7465 5f63 6f6e 6669 672e 7369 7465  site_config.site
-00001680: 5f6e 616d 6520 7d7d 0a7b 7b20 7369 7465  _name }}.{{ site
-00001690: 5f63 6f6e 6669 672e 6d61 696e 7465 6e61  _config.maintena
-000016a0: 6e63 655f 6d6f 6465 207d 7d0a 6060 600a  nce_mode }}.```.
-000016b0: 0a49 6620 796f 7527 7265 2065 7874 656e  .If you're exten
-000016c0: 6469 6e67 2061 2074 656d 706c 6174 652c  ding a template,
-000016d0: 2062 6520 7375 7265 2074 6f20 7573 6520   be sure to use 
-000016e0: 7468 6520 7461 6720 696e 2074 6865 2070  the tag in the p
-000016f0: 726f 7065 7220 7363 6f70 652e 0a0a 5269  roper scope...Ri
-00001700: 6768 743a 0a0a 6060 6064 6a61 6e67 6f0a  ght:..```django.
-00001710: 7b25 2065 7874 656e 6473 2022 696e 6465  {% extends "inde
-00001720: 782e 6874 6d6c 2220 257d 0a7b 2520 6c6f  x.html" %}.{% lo
-00001730: 6164 2073 6f6c 6f5f 7461 6773 2025 7d0a  ad solo_tags %}.
-00001740: 0a7b 2520 626c 6f63 6b20 636f 6e74 656e  .{% block conten
-00001750: 7420 257d 0a20 2020 207b 2520 6765 745f  t %}.    {% get_
-00001760: 736f 6c6f 2027 636f 6e66 6967 2e53 6974  solo 'config.Sit
-00001770: 6543 6f6e 6669 6775 7261 7469 6f6e 2720  eConfiguration' 
-00001780: 6173 2073 6974 655f 636f 6e66 6967 2025  as site_config %
-00001790: 7d0a 2020 2020 7b7b 2073 6974 655f 636f  }.    {{ site_co
-000017a0: 6e66 6967 2e73 6974 655f 6e61 6d65 207d  nfig.site_name }
-000017b0: 7d0a 7b25 2065 6e64 626c 6f63 6b20 636f  }.{% endblock co
-000017c0: 6e74 656e 7420 257d 0a60 6060 0a0a 5772  ntent %}.```..Wr
-000017d0: 6f6e 673a 0a0a 6060 6064 6a61 6e67 6f0a  ong:..```django.
-000017e0: 7b25 2065 7874 656e 6473 2022 696e 6465  {% extends "inde
-000017f0: 782e 6874 6d6c 2220 257d 0a7b 2520 6c6f  x.html" %}.{% lo
-00001800: 6164 2073 6f6c 6f5f 7461 6773 2025 7d0a  ad solo_tags %}.
-00001810: 7b25 2067 6574 5f73 6f6c 6f20 2763 6f6e  {% get_solo 'con
-00001820: 6669 672e 5369 7465 436f 6e66 6967 7572  fig.SiteConfigur
-00001830: 6174 696f 6e27 2061 7320 7369 7465 5f63  ation' as site_c
-00001840: 6f6e 6669 6720 257d 0a0a 7b25 2062 6c6f  onfig %}..{% blo
-00001850: 636b 2063 6f6e 7465 6e74 2025 7d0a 2020  ck content %}.  
-00001860: 2020 7b7b 2073 6974 655f 636f 6e66 6967    {{ site_config
-00001870: 2e73 6974 655f 6e61 6d65 207d 7d0a 7b25  .site_name }}.{%
-00001880: 2065 6e64 626c 6f63 6b20 636f 6e74 656e   endblock conten
-00001890: 7420 257d 0a60 6060 0a0a 0a43 6163 6869  t %}.```...Cachi
-000018a0: 6e67 0a2d 2d2d 2d2d 2d2d 0a0a 4279 2064  ng.-------..By d
-000018b0: 6566 6175 6c74 2063 6163 6869 6e67 2069  efault caching i
-000018c0: 7320 6469 7361 626c 6564 3a20 6576 6572  s disabled: ever
-000018d0: 7920 7469 6d65 2060 6765 745f 736f 6c6f  y time `get_solo
-000018e0: 6020 7265 7472 6965 7665 7320 7468 6520  ` retrieves the 
-000018f0: 7369 6e67 6c65 746f 6e0a 6f62 6a65 6374  singleton.object
-00001900: 2c20 7468 6572 6520 7769 6c6c 2062 6520  , there will be 
-00001910: 6120 6461 7461 6261 7365 2071 7565 7279  a database query
-00001920: 2e0a 0a59 6f75 2063 616e 2065 6e61 626c  ...You can enabl
-00001930: 6520 6361 6368 696e 6720 746f 206f 6e6c  e caching to onl
-00001940: 7920 7175 6572 7920 7468 6520 6461 7461  y query the data
-00001950: 6261 7365 2077 6865 6e20 696e 6974 6961  base when initia
-00001960: 6c6c 7920 7265 7472 6965 7669 6e67 2074  lly retrieving t
-00001970: 6865 0a6f 626a 6563 742e 2054 6865 2063  he.object. The c
-00001980: 6163 6865 2077 696c 6c20 616c 736f 2062  ache will also b
-00001990: 6520 7570 6461 7465 6420 7768 656e 2075  e updated when u
-000019a0: 7064 6174 6573 2061 7265 206d 6164 6520  pdates are made 
-000019b0: 6672 6f6d 2074 6865 2061 646d 696e 2e0a  from the admin..
-000019c0: 0a54 6865 2063 6163 6865 2074 696d 656f  .The cache timeo
-000019d0: 7574 2069 7320 636f 6e74 726f 6c6c 6564  ut is controlled
-000019e0: 2076 6961 2074 6865 2060 534f 4c4f 5f43   via the `SOLO_C
-000019f0: 4143 4845 5f54 494d 454f 5554 6020 7365  ACHE_TIMEOUT` se
-00001a00: 7474 696e 6773 2e0a 5468 6520 6361 6368  ttings..The cach
-00001a10: 6520 6261 636b 656e 6420 746f 2062 6520  e backend to be 
-00001a20: 7573 6564 2069 7320 636f 6e74 726f 6c6c  used is controll
-00001a30: 6564 2076 6961 2074 6865 2060 534f 4c4f  ed via the `SOLO
-00001a40: 5f43 4143 4845 6020 7365 7474 696e 6773  _CACHE` settings
-00001a50: 2e0a 0a0a 5365 7474 696e 6773 0a2d 2d2d  ....Settings.---
-00001a60: 2d2d 2d2d 2d0a 0a23 2323 2054 656d 706c  -----..### Templ
-00001a70: 6174 6520 7461 6720 6e61 6d65 0a0a 596f  ate tag name..Yo
-00001a80: 7520 6361 6e20 7265 7472 6965 7665 2079  u can retrieve y
-00001a90: 6f75 7220 7369 6e67 6c65 746f 6e20 6f62  our singleton ob
-00001aa0: 6a65 6374 2069 6e20 7465 6d70 6c61 7465  ject in template
-00001ab0: 7320 7573 696e 6720 7468 6520 6067 6574  s using the `get
-00001ac0: 5f73 6f6c 6f60 0a74 656d 706c 6174 6520  _solo`.template 
-00001ad0: 7461 672e 0a0a 596f 7520 6361 6e20 6368  tag...You can ch
-00001ae0: 616e 6765 2074 6865 206e 616d 6520 6067  ange the name `g
-00001af0: 6574 5f73 6f6c 6f60 2075 7369 6e67 2074  et_solo` using t
-00001b00: 6865 0a60 4745 545f 534f 4c4f 5f54 454d  he.`GET_SOLO_TEM
-00001b10: 504c 4154 455f 5441 475f 4e41 4d45 6020  PLATE_TAG_NAME` 
-00001b20: 7365 7474 696e 672e 0a0a 6060 6070 7974  setting...```pyt
-00001b30: 686f 6e0a 4745 545f 534f 4c4f 5f54 454d  hon.GET_SOLO_TEM
-00001b40: 504c 4154 455f 5441 475f 4e41 4d45 203d  PLATE_TAG_NAME =
-00001b50: 2027 6765 745f 636f 6e66 6967 270a 6060   'get_config'.``
-00001b60: 600a 0a23 2323 2041 646d 696e 206f 7665  `..### Admin ove
-00001b70: 7272 6964 6520 666c 6167 0a0a 4279 2064  rride flag..By d
-00001b80: 6566 6175 6c74 2c20 7468 6520 6164 6d69  efault, the admi
-00001b90: 6e20 6973 206f 7665 7272 6964 6465 6e2e  n is overridden.
-00001ba0: 2042 7574 2069 6620 796f 7520 7769 7368   But if you wish
-00001bb0: 2074 6f20 6b65 6570 2074 6865 206f 626a   to keep the obj
-00001bc0: 6563 7420 6c69 7374 0a70 6167 6520 2865  ect list.page (e
-00001bd0: 2e67 2e20 746f 2063 7573 746f 6d69 7a65  .g. to customize
-00001be0: 2061 6374 696f 6e73 292c 2079 6f75 2063   actions), you c
-00001bf0: 616e 2073 6574 2074 6865 2060 534f 4c4f  an set the `SOLO
-00001c00: 5f41 444d 494e 5f53 4b49 505f 4f42 4a45  _ADMIN_SKIP_OBJE
-00001c10: 4354 5f4c 4953 545f 5041 4745 600a 746f  CT_LIST_PAGE`.to
-00001c20: 2060 4661 6c73 6560 2e0a 0a60 6060 7079   `False`...```py
-00001c30: 7468 6f6e 0a53 4f4c 4f5f 4144 4d49 4e5f  thon.SOLO_ADMIN_
-00001c40: 534b 4950 5f4f 424a 4543 545f 4c49 5354  SKIP_OBJECT_LIST
-00001c50: 5f50 4147 4520 3d20 5472 7565 0a60 6060  _PAGE = True.```
-00001c60: 0a0a 2323 2320 4361 6368 6520 6261 636b  ..### Cache back
-00001c70: 656e 640a 0a44 6a61 6e67 6f20 7072 6f76  end..Django prov
-00001c80: 6964 6573 2061 2077 6179 2074 6f20 6465  ides a way to de
-00001c90: 6669 6e65 206d 756c 7469 706c 6520 6361  fine multiple ca
-00001ca0: 6368 6520 6261 636b 656e 6473 2077 6974  che backends wit
-00001cb0: 6820 7468 6520 6043 4143 4845 5360 0a73  h the `CACHES`.s
-00001cc0: 6574 7469 6e67 732e 2049 6620 796f 7520  ettings. If you 
-00001cd0: 7761 6e74 2074 6865 2073 696e 676c 6574  want the singlet
-00001ce0: 6f6e 206f 626a 6563 7420 746f 2062 6520  on object to be 
-00001cf0: 6361 6368 6564 2073 6570 6172 6174 656c  cached separatel
-00001d00: 792c 2079 6f75 0a63 6f75 6c64 2064 6566  y, you.could def
-00001d10: 696e 6520 7468 6520 6043 4143 4845 5360  ine the `CACHES`
-00001d20: 2061 6e64 2074 6865 2060 534f 4c4f 5f43   and the `SOLO_C
-00001d30: 4143 4845 6020 7365 7474 696e 6773 206c  ACHE` settings l
-00001d40: 696b 6520 7468 6973 3a0a 0a60 6060 7079  ike this:..```py
-00001d50: 7468 6f6e 0a43 4143 4845 5320 3d20 7b0a  thon.CACHES = {.
-00001d60: 2020 2020 2764 6566 6175 6c74 273a 207b      'default': {
-00001d70: 0a20 2020 2020 2020 2027 4241 434b 454e  .        'BACKEN
-00001d80: 4427 3a20 2764 6a61 6e67 6f2e 636f 7265  D': 'django.core
-00001d90: 2e63 6163 6865 2e62 6163 6b65 6e64 732e  .cache.backends.
-00001da0: 6d65 6d63 6163 6865 642e 4d65 6d63 6163  memcached.Memcac
-00001db0: 6865 6443 6163 6865 272c 0a20 2020 2020  hedCache',.     
-00001dc0: 2020 2027 4c4f 4341 5449 4f4e 273a 2027     'LOCATION': '
-00001dd0: 3132 372e 302e 302e 313a 3131 3231 3127  127.0.0.1:11211'
-00001de0: 2c0a 2020 2020 7d2c 0a20 2020 2027 6c6f  ,.    },.    'lo
-00001df0: 6361 6c27 3a20 7b0a 2020 2020 2020 2020  cal': {.        
-00001e00: 2742 4143 4b45 4e44 273a 2027 646a 616e  'BACKEND': 'djan
-00001e10: 676f 2e63 6f72 652e 6361 6368 652e 6261  go.core.cache.ba
-00001e20: 636b 656e 6473 2e6c 6f63 6d65 6d2e 4c6f  ckends.locmem.Lo
-00001e30: 634d 656d 4361 6368 6527 2c0a 2020 2020  cMemCache',.    
-00001e40: 7d2c 0a7d 0a0a 534f 4c4f 5f43 4143 4845  },.}..SOLO_CACHE
-00001e50: 203d 2027 6c6f 6361 6c27 0a60 6060 0a0a   = 'local'.```..
-00001e60: 4361 6368 696e 6720 7769 6c6c 2062 6520  Caching will be 
-00001e70: 6469 7361 626c 6564 2069 6620 7365 7420  disabled if set 
-00001e80: 746f 2060 4e6f 6e65 602e 0a0a 0a23 2323  to `None`....###
-00001e90: 2043 6163 6865 2074 696d 656f 7574 0a0a   Cache timeout..
-00001ea0: 5468 6520 6361 6368 6520 7469 6d65 6f75  The cache timeou
-00001eb0: 7420 696e 2073 6563 6f6e 6473 2e0a 0a60  t in seconds...`
-00001ec0: 6060 7079 7468 6f6e 0a53 4f4c 4f5f 4341  ``python.SOLO_CA
-00001ed0: 4348 455f 5449 4d45 4f55 5420 3d20 3630  CHE_TIMEOUT = 60
-00001ee0: 2a35 2020 2320 3520 6d69 6e73 0a60 6060  *5  # 5 mins.```
-00001ef0: 0a0a 2323 2320 4361 6368 6520 7072 6566  ..### Cache pref
-00001f00: 6978 0a0a 5468 6520 7072 6566 6978 2074  ix..The prefix t
-00001f10: 6f20 7573 6520 666f 7220 7468 6520 6361  o use for the ca
-00001f20: 6368 6520 6b65 792e 0a0a 6060 6070 7974  che key...```pyt
-00001f30: 686f 6e0a 534f 4c4f 5f43 4143 4845 5f50  hon.SOLO_CACHE_P
-00001f40: 5245 4649 5820 3d20 2773 6f6c 6f27 0a60  REFIX = 'solo'.`
-00001f50: 6060 0a0a 4765 7474 696e 6720 7468 6520  ``..Getting the 
-00001f60: 636f 6465 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d  code.===========
-00001f70: 3d3d 3d3d 3d0a 0a54 6865 2063 6f64 6520  =====..The code 
-00001f80: 6973 2068 6f73 7465 6420 6174 2068 7474  is hosted at htt
-00001f90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001fa0: 6c61 7a79 6269 7264 2f64 6a61 6e67 6f2d  lazybird/django-
-00001fb0: 736f 6c6f 2f0a 0a43 6865 636b 206f 7574  solo/..Check out
-00001fc0: 2074 6865 206c 6174 6573 7420 6465 7665   the latest deve
-00001fd0: 6c6f 706d 656e 7420 7665 7273 696f 6e20  lopment version 
-00001fe0: 616e 6f6e 796d 6f75 736c 7920 7769 7468  anonymously with
-00001ff0: 3a0a 0a20 2020 2024 2067 6974 2063 6c6f  :..    $ git clo
-00002000: 6e65 2067 6974 3a2f 2f67 6974 6875 622e  ne git://github.
-00002010: 636f 6d2f 6c61 7a79 6269 7264 2f64 6a61  com/lazybird/dja
-00002020: 6e67 6f2d 736f 6c6f 2e67 6974 0a0a 596f  ngo-solo.git..Yo
-00002030: 7520 6361 6e20 696e 7374 616c 6c20 7468  u can install th
-00002040: 6520 7061 636b 6167 6520 696e 2074 6865  e package in the
-00002050: 2022 6564 6974 6162 6c65 2220 6d6f 6465   "editable" mode
-00002060: 206c 696b 6520 7468 6973 3a0a 0a20 2020   like this:..   
-00002070: 2070 6970 2075 6e69 6e73 7461 6c6c 2064   pip uninstall d
-00002080: 6a61 6e67 6f2d 736f 6c6f 2020 2320 6a75  jango-solo  # ju
-00002090: 7374 2069 6e20 6361 7365 2e2e 2e0a 2020  st in case....  
-000020a0: 2020 7069 7020 696e 7374 616c 6c20 2d65    pip install -e
-000020b0: 2067 6974 2b68 7474 7073 3a2f 2f67 6974   git+https://git
-000020c0: 6875 622e 636f 6d2f 6c61 7a79 6269 7264  hub.com/lazybird
-000020d0: 2f64 6a61 6e67 6f2d 736f 6c6f 2e67 6974  /django-solo.git
-000020e0: 2365 6767 3d64 6a61 6e67 6f2d 736f 6c6f  #egg=django-solo
-000020f0: 0a0a 596f 7520 6361 6e20 616c 736f 2069  ..You can also i
-00002100: 6e73 7461 6c6c 2061 2073 7065 6369 6669  nstall a specifi
-00002110: 6320 6272 616e 6368 3a0a 0a20 2020 2070  c branch:..    p
-00002120: 6970 2069 6e73 7461 6c6c 202d 6520 6769  ip install -e gi
-00002130: 742b 6874 7470 733a 2f2f 6769 7468 7562  t+https://github
-00002140: 2e63 6f6d 2f6c 617a 7962 6972 642f 646a  .com/lazybird/dj
-00002150: 616e 676f 2d73 6f6c 6f2e 6769 7440 6d79  ango-solo.git@my
-00002160: 2d62 7261 6e63 6823 6567 673d 646a 616e  -branch#egg=djan
-00002170: 676f 2d73 6f6c 6f0a 0a54 6865 2070 6163  go-solo..The pac
-00002180: 6b61 6765 2069 7320 6e6f 7720 696e 7374  kage is now inst
-00002190: 616c 6c65 6420 696e 2079 6f75 7220 7072  alled in your pr
-000021a0: 6f6a 6563 7420 616e 6420 796f 7520 6361  oject and you ca
-000021b0: 6e20 6669 6e64 2074 6865 2063 6f64 652e  n find the code.
-000021c0: 0a0a 546f 2072 756e 2074 6865 2075 6e69  ..To run the uni
-000021d0: 7420 7465 7374 733a 0a0a 2020 2020 7069  t tests:..    pi
-000021e0: 7020 696e 7374 616c 6c20 746f 780a 2020  p install tox.  
-000021f0: 2020 746f 780a 0a0a                        tox...
+00000010: 3a20 322e 310d 0a4e 616d 653a 2064 6a61  : 2.1..Name: dja
+00000020: 6e67 6f2d 736f 6c6f 0d0a 5665 7273 696f  ngo-solo..Versio
+00000030: 6e3a 2032 2e31 2e30 0d0a 5375 6d6d 6172  n: 2.1.0..Summar
+00000040: 793a 2044 6a61 6e67 6f20 536f 6c6f 2068  y: Django Solo h
+00000050: 656c 7073 2077 6f72 6b69 6e67 2077 6974  elps working wit
+00000060: 6820 7369 6e67 6c65 746f 6e73 0d0a 486f  h singletons..Ho
+00000070: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
+00000080: 2f67 6974 6875 622e 636f 6d2f 6c61 7a79  /github.com/lazy
+00000090: 6269 7264 2f64 6a61 6e67 6f2d 736f 6c6f  bird/django-solo
+000000a0: 2f0d 0a41 7574 686f 723a 206c 617a 7962  /..Author: lazyb
+000000b0: 6972 640d 0a4c 6963 656e 7365 3a20 4372  ird..License: Cr
+000000c0: 6561 7469 7665 2043 6f6d 6d6f 6e73 2041  eative Commons A
+000000d0: 7474 7269 6275 7469 6f6e 2033 2e30 2055  ttribution 3.0 U
+000000e0: 6e70 6f72 7465 640d 0a43 6c61 7373 6966  nported..Classif
+000000f0: 6965 723a 2046 7261 6d65 776f 726b 203a  ier: Framework :
+00000100: 3a20 446a 616e 676f 203a 3a20 332e 320d  : Django :: 3.2.
+00000110: 0a43 6c61 7373 6966 6965 723a 2046 7261  .Classifier: Fra
+00000120: 6d65 776f 726b 203a 3a20 446a 616e 676f  mework :: Django
+00000130: 203a 3a20 342e 300d 0a43 6c61 7373 6966   :: 4.0..Classif
+00000140: 6965 723a 2046 7261 6d65 776f 726b 203a  ier: Framework :
+00000150: 3a20 446a 616e 676f 203a 3a20 342e 310d  : Django :: 4.1.
+00000160: 0a43 6c61 7373 6966 6965 723a 2046 7261  .Classifier: Fra
+00000170: 6d65 776f 726b 203a 3a20 446a 616e 676f  mework :: Django
+00000180: 203a 3a20 342e 320d 0a43 6c61 7373 6966   :: 4.2..Classif
+00000190: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
+000001a0: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
+000001b0: 7065 7273 0d0a 436c 6173 7369 6669 6572  pers..Classifier
+000001c0: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
+000001d0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+000001e0: 6465 6e74 0d0a 436c 6173 7369 6669 6572  dent..Classifier
+000001f0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000200: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000210: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
+00000220: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000230: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000240: 330d 0a43 6c61 7373 6966 6965 723a 2050  3..Classifier: P
+00000250: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000260: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000270: 2033 2e37 0d0a 436c 6173 7369 6669 6572   3.7..Classifier
+00000280: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000290: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000002a0: 203a 3a20 332e 380d 0a43 6c61 7373 6966   :: 3.8..Classif
+000002b0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000002c0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000002d0: 686f 6e20 3a3a 2033 2e39 0d0a 436c 6173  hon :: 3.9..Clas
+000002e0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000002f0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000300: 5079 7468 6f6e 203a 3a20 332e 3130 0d0a  Python :: 3.10..
+00000310: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000320: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000330: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000340: 3131 0d0a 5265 7175 6972 6573 2d50 7974  11..Requires-Pyt
+00000350: 686f 6e3a 203e 3d33 2e37 0d0a 4465 7363  hon: >=3.7..Desc
+00000360: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+00000370: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+00000380: 6f77 6e0d 0a4c 6963 656e 7365 2d46 696c  own..License-Fil
+00000390: 653a 204c 4943 454e 5345 0d0a 0d0a 0d0a  e: LICENSE......
+000003a0: 446a 616e 676f 2053 6f6c 6f0d 0a3d 3d3d  Django Solo..===
+000003b0: 3d3d 3d3d 3d3d 3d3d 0d0a 0d0a 3c61 2068  ========....<a h
+000003c0: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+000003d0: 692e 6f72 672f 7072 6f6a 6563 742f 646a  i.org/project/dj
+000003e0: 616e 676f 2d73 6f6c 6f2f 2220 616c 743d  ango-solo/" alt=
+000003f0: 2243 7572 7265 6e74 2076 6572 7369 6f6e  "Current version
+00000400: 206f 6e20 5079 5069 223e 3c69 6d67 2073   on PyPi"><img s
+00000410: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000420: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000430: 762f 646a 616e 676f 2d73 6f6c 6f2e 7376  v/django-solo.sv
+00000440: 6722 202f 3e3c 2f61 3e0d 0a0d 0a0d 0a20  g" /></a>...... 
+00000450: 2020 202b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     +------------
+00000460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00000470: 0d0a 2020 2020 7c20 2020 2020 2020 2020  ..    |         
+00000480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000490: 2020 7c0d 0a20 2020 207c 2020 2020 2020    |..    |      
+000004a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004b0: 2020 2020 207c 0d0a 2020 2020 7c20 2020       |..    |   
+000004c0: 2020 2020 2020 2020 2020 5c20 2020 2020            \     
+000004d0: 2020 2020 2020 2020 7c20 446a 616e 676f          | Django
+000004e0: 2053 6f6c 6f20 6865 6c70 7320 776f 726b   Solo helps work
+000004f0: 696e 6720 7769 7468 2073 696e 676c 6574  ing with singlet
+00000500: 6f6e 733a 0d0a 2020 2020 7c20 2020 2020  ons:..    |     
+00000510: 2020 2020 2020 2020 2f5c 2020 2020 2020          /\      
+00000520: 2020 2020 2020 7c20 6461 7461 6261 7365        | database
+00000530: 2074 6162 6c65 7320 7468 6174 206f 6e6c   tables that onl
+00000540: 7920 6861 7665 206f 6e65 2072 6f77 2e0d  y have one row..
+00000550: 0a20 2020 207c 2020 2020 2020 2020 2020  .    |          
+00000560: 203e 3d29 273e 2020 2020 2020 2020 2020   >=)'>          
+00000570: 207c 2053 696e 676c 6574 6f6e 7320 6172   | Singletons ar
+00000580: 6520 7573 6566 756c 2066 6f72 2074 6869  e useful for thi
+00000590: 6e67 7320 6c69 6b65 2067 6c6f 6261 6c0d  ngs like global.
+000005a0: 0a20 2020 207c 2020 2020 2020 2020 2020  .    |          
+000005b0: 2020 205c 2f20 2020 2020 2020 2020 2020     \/           
+000005c0: 207c 2073 6574 7469 6e67 7320 7468 6174   | settings that
+000005d0: 2079 6f75 2077 616e 7420 746f 2065 6469   you want to edi
+000005e0: 7420 6672 6f6d 2074 6865 2061 646d 696e  t from the admin
+000005f0: 0d0a 2020 2020 7c20 2020 2020 2020 2020  ..    |         
+00000600: 2020 2020 2f20 2020 2020 2020 2020 2020      /           
+00000610: 2020 7c20 696e 7374 6561 6420 6f66 2068    | instead of h
+00000620: 6176 696e 6720 7468 656d 2069 6e20 446a  aving them in Dj
+00000630: 616e 676f 2073 6574 7469 6e67 732e 7079  ango settings.py
+00000640: 2e0d 0a20 2020 207c 2020 2020 2020 2020  ...    |        
+00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000660: 2020 207c 200d 0a20 2020 207c 2020 2020     | ..    |    
+00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000680: 2020 2020 2020 207c 200d 0a20 2020 202b         | ..    +
+00000690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000006a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0d0a 0d0a  -----------+....
+000006b0: 0d0a 4665 6174 7572 6573 0d0a 2d2d 2d2d  ..Features..----
+000006c0: 2d2d 2d2d 0d0a 0d0a 536f 6c6f 2068 656c  ----....Solo hel
+000006d0: 7073 2079 6f75 2065 6e66 6f72 6365 2069  ps you enforce i
+000006e0: 6e73 7461 6e74 6961 7469 6e67 206f 6e6c  nstantiating onl
+000006f0: 7920 6f6e 6520 696e 7374 616e 6365 206f  y one instance o
+00000700: 6620 6120 6d6f 6465 6c20 696e 2064 6a61  f a model in dja
+00000710: 6e67 6f2e 0d0a 0d0a 2a20 596f 7520 6465  ngo.....* You de
+00000720: 6669 6e65 2074 6865 206d 6f64 656c 2074  fine the model t
+00000730: 6861 7420 7769 6c6c 2068 6f6c 6420 796f  hat will hold yo
+00000740: 7572 2073 696e 676c 6574 6f6e 206f 626a  ur singleton obj
+00000750: 6563 742e 0d0a 2a20 646a 616e 676f 2d73  ect...* django-s
+00000760: 6f6c 6f20 6769 7665 7320 6865 6c70 6572  olo gives helper
+00000770: 2070 6172 656e 7420 636c 6173 7320 666f   parent class fo
+00000780: 7220 796f 7572 206d 6f64 656c 2061 6e64  r your model and
+00000790: 2074 6865 2061 646d 696e 2063 6c61 7373   the admin class
+000007a0: 6573 2e0d 0a2a 2059 6f75 2067 6574 2061  es...* You get a
+000007b0: 6e20 6164 6d69 6e20 696e 7465 7266 6163  n admin interfac
+000007c0: 6520 7468 6174 2773 2061 7761 7265 2079  e that's aware y
+000007d0: 6f75 206f 6e6c 7920 6861 7665 206f 6e65  ou only have one
+000007e0: 206f 626a 6563 742e 0d0a 2a20 596f 7520   object...* You 
+000007f0: 6361 6e20 7265 7472 6965 7665 2074 6865  can retrieve the
+00000800: 206f 626a 6563 7420 6672 6f6d 2074 656d   object from tem
+00000810: 706c 6174 6573 2e0d 0a2a 2042 7920 656e  plates...* By en
+00000820: 6162 6c69 6e67 2063 6163 6869 6e67 2c20  abling caching, 
+00000830: 7468 6520 6461 7461 6261 7365 2069 7320  the database is 
+00000840: 6e6f 7420 7175 6572 6965 6420 696e 7465  not queried inte
+00000850: 6e73 6976 656c 792e 0d0a 0d0a 5573 6520  nsively.....Use 
+00000860: 4361 7365 730d 0a2d 2d2d 2d2d 2d2d 2d0d  Cases..--------.
+00000870: 0a0d 0a44 6a61 6e67 6f20 536f 6c6f 2069  ...Django Solo i
+00000880: 7320 616c 736f 2067 7265 6174 2066 6f72  s also great for
+00000890: 2075 7365 2077 6974 6820 7369 6e67 6c65   use with single
+000008a0: 746f 6e20 6f62 6a65 6374 7320 7468 6174  ton objects that
+000008b0: 2068 6176 6520 6120 6f6e 6520 746f 206d   have a one to m
+000008c0: 616e 7920 7265 6c61 7469 6f6e 7368 6970  any relationship
+000008d0: 2e20 4c69 6b65 2074 6865 2075 7365 2063  . Like the use c
+000008e0: 6173 6520 6265 6c6f 7720 7768 6572 6520  ase below where 
+000008f0: 796f 7520 6861 7665 2061 2027 486f 6d65  you have a 'Home
+00000900: 2053 6c69 6465 7222 2074 6861 7420 6861   Slider" that ha
+00000910: 7320 6d61 6e79 2022 536c 6964 6573 222e  s many "Slides".
+00000920: 0d0a 0d0a 2a20 476c 6f62 616c 206f 7220  ....* Global or 
+00000930: 6465 6661 756c 7420 7365 7474 696e 6773  default settings
+00000940: 0d0a 2a20 416e 2069 6d61 6765 2073 6c69  ..* An image sli
+00000950: 6465 7220 7468 6174 2068 6173 206d 616e  der that has man
+00000960: 7920 736c 6964 6573 0d0a 2a20 4120 7061  y slides..* A pa
+00000970: 6765 2073 6563 7469 6f6e 2074 6861 7420  ge section that 
+00000980: 6861 7320 7375 622d 7365 6374 696f 6e73  has sub-sections
+00000990: 0d0a 2a20 4120 7465 616d 2062 696f 2077  ..* A team bio w
+000009a0: 6974 6820 6d61 6e79 2074 6561 6d20 6d65  ith many team me
+000009b0: 6d62 6572 730d 0a0d 0a54 6865 7265 2061  mbers....There a
+000009c0: 7265 206d 616e 7920 6361 7365 7320 7768  re many cases wh
+000009d0: 6572 6520 6974 206d 616b 6573 2073 656e  ere it makes sen
+000009e0: 7365 2066 6f72 2074 6865 2070 6172 656e  se for the paren
+000009f0: 7420 696e 2061 206f 6e65 2074 6f20 6d61  t in a one to ma
+00000a00: 6e79 2072 656c 6174 696f 6e73 6869 7020  ny relationship 
+00000a10: 746f 2062 6520 6c69 6d69 7465 6420 746f  to be limited to
+00000a20: 2061 2073 696e 676c 6520 696e 7374 616e   a single instan
+00000a30: 6365 2e0d 0a0d 0a55 7361 6765 2045 7861  ce.....Usage Exa
+00000a40: 6d70 6c65 0d0a 0d0a 6060 6070 7974 686f  mple....```pytho
+00000a50: 6e0d 0a23 206d 6f64 656c 732e 7079 0d0a  n..# models.py..
+00000a60: 0d0a 6672 6f6d 2064 6a61 6e67 6f2e 6462  ..from django.db
+00000a70: 2069 6d70 6f72 7420 6d6f 6465 6c73 0d0a   import models..
+00000a80: 6672 6f6d 2073 6f6c 6f2e 6d6f 6465 6c73  from solo.models
+00000a90: 2069 6d70 6f72 7420 5369 6e67 6c65 746f   import Singleto
+00000aa0: 6e4d 6f64 656c 0d0a 0d0a 0d0a 636c 6173  nModel......clas
+00000ab0: 7320 5369 7465 436f 6e66 6967 7572 6174  s SiteConfigurat
+00000ac0: 696f 6e28 5369 6e67 6c65 746f 6e4d 6f64  ion(SingletonMod
+00000ad0: 656c 293a 0d0a 2020 2020 7369 7465 5f6e  el):..    site_n
+00000ae0: 616d 6520 3d20 6d6f 6465 6c73 2e43 6861  ame = models.Cha
+00000af0: 7246 6965 6c64 286d 6178 5f6c 656e 6774  rField(max_lengt
+00000b00: 683d 3235 352c 2064 6566 6175 6c74 3d27  h=255, default='
+00000b10: 5369 7465 204e 616d 6527 290d 0a20 2020  Site Name')..   
+00000b20: 206d 6169 6e74 656e 616e 6365 5f6d 6f64   maintenance_mod
+00000b30: 6520 3d20 6d6f 6465 6c73 2e42 6f6f 6c65  e = models.Boole
+00000b40: 616e 4669 656c 6428 6465 6661 756c 743d  anField(default=
+00000b50: 4661 6c73 6529 0d0a 0d0a 2020 2020 6465  False)....    de
+00000b60: 6620 5f5f 7374 725f 5f28 7365 6c66 293a  f __str__(self):
+00000b70: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000b80: 2022 5369 7465 2043 6f6e 6669 6775 7261   "Site Configura
+00000b90: 7469 6f6e 220d 0a0d 0a20 2020 2063 6c61  tion"....    cla
+00000ba0: 7373 204d 6574 613a 0d0a 2020 2020 2020  ss Meta:..      
+00000bb0: 2020 7665 7262 6f73 655f 6e61 6d65 203d    verbose_name =
+00000bc0: 2022 5369 7465 2043 6f6e 6669 6775 7261   "Site Configura
+00000bd0: 7469 6f6e 220d 0a60 6060 0d0a 0d0a 6060  tion"..```....``
+00000be0: 6070 7974 686f 6e0d 0a23 2061 646d 696e  `python..# admin
+00000bf0: 2e70 790d 0a0d 0a66 726f 6d20 646a 616e  .py....from djan
+00000c00: 676f 2e63 6f6e 7472 6962 2069 6d70 6f72  go.contrib impor
+00000c10: 7420 6164 6d69 6e0d 0a66 726f 6d20 736f  t admin..from so
+00000c20: 6c6f 2e61 646d 696e 2069 6d70 6f72 7420  lo.admin import 
+00000c30: 5369 6e67 6c65 746f 6e4d 6f64 656c 4164  SingletonModelAd
+00000c40: 6d69 6e0d 0a66 726f 6d20 636f 6e66 6967  min..from config
+00000c50: 2e6d 6f64 656c 7320 696d 706f 7274 2053  .models import S
+00000c60: 6974 6543 6f6e 6669 6775 7261 7469 6f6e  iteConfiguration
+00000c70: 0d0a 0d0a 0d0a 6164 6d69 6e2e 7369 7465  ......admin.site
+00000c80: 2e72 6567 6973 7465 7228 5369 7465 436f  .register(SiteCo
+00000c90: 6e66 6967 7572 6174 696f 6e2c 2053 696e  nfiguration, Sin
+00000ca0: 676c 6574 6f6e 4d6f 6465 6c41 646d 696e  gletonModelAdmin
+00000cb0: 290d 0a60 6060 0d0a 0d0a 6060 6070 7974  )..```....```pyt
+00000cc0: 686f 6e0d 0a23 2054 6865 7265 2069 7320  hon..# There is 
+00000cd0: 6f6e 6c79 206f 6e65 2069 7465 6d20 696e  only one item in
+00000ce0: 2074 6865 2074 6162 6c65 2c20 796f 7520   the table, you 
+00000cf0: 6361 6e20 6765 7420 6974 2074 6869 7320  can get it this 
+00000d00: 7761 793a 0d0a 6672 6f6d 202e 6d6f 6465  way:..from .mode
+00000d10: 6c73 2069 6d70 6f72 7420 5369 7465 436f  ls import SiteCo
+00000d20: 6e66 6967 7572 6174 696f 6e0d 0a63 6f6e  nfiguration..con
+00000d30: 6669 6720 3d20 5369 7465 436f 6e66 6967  fig = SiteConfig
+00000d40: 7572 6174 696f 6e2e 6f62 6a65 6374 732e  uration.objects.
+00000d50: 6765 7428 290d 0a0d 0a23 2067 6574 5f73  get()....# get_s
+00000d60: 6f6c 6f20 7769 6c6c 2063 7265 6174 6520  olo will create 
+00000d70: 7468 6520 6974 656d 2069 6620 6974 2064  the item if it d
+00000d80: 6f65 7320 6e6f 7420 616c 7265 6164 7920  oes not already 
+00000d90: 6578 6973 740d 0a63 6f6e 6669 6720 3d20  exist..config = 
+00000da0: 5369 7465 436f 6e66 6967 7572 6174 696f  SiteConfiguratio
+00000db0: 6e2e 6765 745f 736f 6c6f 2829 0d0a 6060  n.get_solo()..``
+00000dc0: 600d 0a0d 0a49 6e20 796f 7572 206d 6f64  `....In your mod
+00000dd0: 656c 2c20 6e6f 7465 2068 6f77 2079 6f75  el, note how you
+00000de0: 2064 6964 206e 6f74 2068 6176 6520 746f   did not have to
+00000df0: 2070 726f 7669 6465 2061 2060 7665 7262   provide a `verb
+00000e00: 6f73 655f 6e61 6d65 5f70 6c75 7261 6c60  ose_name_plural`
+00000e10: 2066 6965 6c64 202d 0d0a 5468 6174 2773   field -..That's
+00000e20: 2062 6563 6175 7365 2044 6a61 6e67 6f20   because Django 
+00000e30: 536f 6c6f 2075 7365 7320 7468 6520 6076  Solo uses the `v
+00000e40: 6572 626f 7365 5f6e 616d 6560 2069 6e73  erbose_name` ins
+00000e50: 7465 6164 2e0d 0a0d 0a49 6620 796f 7527  tead.....If you'
+00000e60: 7265 2063 6861 6e67 696e 6720 616e 2065  re changing an e
+00000e70: 7869 7374 696e 6720 6d6f 6465 6c20 2877  xisting model (w
+00000e80: 6869 6368 2061 6c72 6561 6479 2068 6173  hich already has
+00000e90: 2073 6f6d 6520 6f62 6a65 6374 7320 7374   some objects st
+00000ea0: 6f72 6564 2069 6e20 7468 6520 6461 7461  ored in the data
+00000eb0: 6261 7365 2920 746f 2061 2073 696e 676c  base) to a singl
+00000ec0: 6574 6f6e 206d 6f64 656c 2c20 796f 7520  eton model, you 
+00000ed0: 6361 6e20 6578 706c 6963 6974 6c79 2070  can explicitly p
+00000ee0: 726f 7669 6465 2074 6865 2069 6420 6f66  rovide the id of
+00000ef0: 2074 6865 2072 6f77 2069 6e20 7468 6520   the row in the 
+00000f00: 6461 7461 6261 7365 2066 6f72 2064 6a61  database for dja
+00000f10: 6e67 6f2d 736f 6c6f 2074 6f20 7573 652e  ngo-solo to use.
+00000f20: 2054 6869 7320 6361 6e20 6265 2064 6f6e   This can be don
+00000f30: 6520 6279 2073 6574 7469 6e67 2060 7369  e by setting `si
+00000f40: 6e67 6c65 746f 6e5f 696e 7374 616e 6365  ngleton_instance
+00000f50: 5f69 6460 2070 726f 7065 7274 7920 6f6e  _id` property on
+00000f60: 2074 6865 206d 6f64 656c 3a0d 0a0d 0a60   the model:....`
+00000f70: 6060 7079 7468 6f6e 0d0a 636c 6173 7320  ``python..class 
+00000f80: 5369 7465 436f 6e66 6967 7572 6174 696f  SiteConfiguratio
+00000f90: 6e28 5369 6e67 6c65 746f 6e4d 6f64 656c  n(SingletonModel
+00000fa0: 293a 0d0a 2020 2020 7369 6e67 6c65 746f  ):..    singleto
+00000fb0: 6e5f 696e 7374 616e 6365 5f69 6420 3d20  n_instance_id = 
+00000fc0: 3234 0d0a 2020 2020 2320 282e 2e2e 290d  24..    # (...).
+00000fd0: 0a60 6060 0d0a 0d0a 496e 7374 616c 6c61  .```....Installa
+00000fe0: 7469 6f6e 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d  tion..----------
+00000ff0: 2d2d 0d0a 0d0a 5468 6973 2061 7070 6c69  --....This appli
+00001000: 6361 7469 6f6e 2072 6571 7569 7265 7320  cation requires 
+00001010: 446a 616e 676f 2033 2e32 2c20 342e 302c  Django 3.2, 4.0,
+00001020: 206f 7220 342e 312e 0d0a 0d0a 2a20 496e   or 4.1.....* In
+00001030: 7374 616c 6c20 7468 6520 7061 636b 6167  stall the packag
+00001040: 6520 7573 696e 6720 6070 6970 2069 6e73  e using `pip ins
+00001050: 7461 6c6c 2064 6a61 6e67 6f2d 736f 6c6f  tall django-solo
+00001060: 600d 0a2a 2041 6464 2060 6073 6f6c 6f60  `..* Add ``solo`
+00001070: 6020 6f72 2060 6073 6f6c 6f2e 6170 7073  ` or ``solo.apps
+00001080: 2e53 6f6c 6f41 7070 436f 6e66 6967 6060  .SoloAppConfig``
+00001090: 2074 6f20 796f 7572 2060 6049 4e53 5441   to your ``INSTA
+000010a0: 4c4c 4544 5f41 5050 5360 6020 7365 7474  LLED_APPS`` sett
+000010b0: 696e 672e 0d0a 0d0a 5468 6973 2069 7320  ing.....This is 
+000010c0: 686f 7720 796f 7520 7275 6e20 7465 7374  how you run test
+000010d0: 733a 0d0a 0d0a 2020 2020 2e2f 6d61 6e61  s:....    ./mana
+000010e0: 6765 2e70 7920 7465 7374 2073 6f6c 6f20  ge.py test solo 
+000010f0: 2d2d 7365 7474 696e 6773 3d73 6f6c 6f2e  --settings=solo.
+00001100: 7465 7374 732e 7365 7474 696e 6773 0d0a  tests.settings..
+00001110: 0d0a 416e 6420 6672 6f6d 2077 6974 6869  ..And from withi
+00001120: 6e20 6074 6f78 603a 0d0a 0d0a 6060 600d  n `tox`:....```.
+00001130: 0a70 7974 686f 6e20 2d6d 2070 6970 2069  .python -m pip i
+00001140: 6e73 7461 6c6c 2074 6f78 0d0a 746f 780d  nstall tox..tox.
+00001150: 0a60 6060 0d0a 0d0a 5375 7070 6f72 7465  .```....Supporte
+00001160: 6420 4c61 6e67 7561 6765 730d 0a2d 2d2d  d Languages..---
+00001170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001180: 0d0a 0d0a 2d20 456e 676c 6973 680d 0a2d  ....- English..-
+00001190: 2053 7061 6e69 7368 0d0a 2d20 4765 726d   Spanish..- Germ
+000011a0: 616e 0d0a 0d0a 4164 6d69 6e0d 0a2d 2d2d  an....Admin..---
+000011b0: 2d2d 0d0a 0d0a 5468 6520 7374 616e 6461  --....The standa
+000011c0: 7264 2044 6a61 6e67 6f20 6164 6d69 6e20  rd Django admin 
+000011d0: 646f 6573 206e 6f74 2066 6974 2077 656c  does not fit wel
+000011e0: 6c20 7768 656e 2077 6f72 6b69 6e67 2077  l when working w
+000011f0: 6974 6820 7369 6e67 6c65 746f 6e2c 0d0a  ith singleton,..
+00001200: 666f 7220 696e 7374 616e 6365 2c20 6966  for instance, if
+00001210: 2079 6f75 206e 6565 6420 736f 6d65 2067   you need some g
+00001220: 6c6f 6261 6c20 7369 7465 2073 6574 7469  lobal site setti
+00001230: 6e67 7320 746f 2062 6520 6564 6974 6564  ngs to be edited
+00001240: 2069 6e20 7468 6520 6164 6d69 6e2e 0d0a   in the admin...
+00001250: 446a 616e 676f 2053 6f6c 6f20 7072 6f76  Django Solo prov
+00001260: 6964 6573 2061 206d 6f64 6966 6965 6420  ides a modified 
+00001270: 6164 6d69 6e20 666f 7220 7468 6174 2e0d  admin for that..
+00001280: 0a0d 0a0d 0a21 5b64 6a61 6e67 6f2d 736f  .....![django-so
+00001290: 6c6f 2061 646d 696e 5d28 6874 7470 733a  lo admin](https:
+000012a0: 2f2f 7261 772e 6769 7468 7562 2e63 6f6d  //raw.github.com
+000012b0: 2f6c 617a 7962 6972 642f 646a 616e 676f  /lazybird/django
+000012c0: 2d73 6f6c 6f2f 6d61 7374 6572 2f64 6f63  -solo/master/doc
+000012d0: 732f 696d 6167 6573 2f64 6a61 6e67 6f2d  s/images/django-
+000012e0: 736f 6c6f 2d61 646d 696e 2e6a 7067 2022  solo-admin.jpg "
+000012f0: 646a 616e 676f 2d73 6f6c 6f20 6164 6d69  django-solo admi
+00001300: 6e22 290d 0a0d 0a0d 0a2a 2049 6e20 7468  n")......* In th
+00001310: 6520 6164 6d69 6e20 686f 6d65 2070 6167  e admin home pag
+00001320: 6520 7768 6572 6520 616c 6c20 6170 706c  e where all appl
+00001330: 6963 6174 696f 6e73 2061 7265 206c 6973  ications are lis
+00001340: 7465 642c 2077 6520 6861 7665 2061 2060  ted, we have a `
+00001350: 636f 6e66 6967 600d 0a20 2061 7070 6c69  config`..  appli
+00001360: 6361 7469 6f6e 2074 6861 7420 686f 6c64  cation that hold
+00001370: 7320 6120 7369 6e67 6c65 746f 6e20 6d6f  s a singleton mo
+00001380: 6465 6c20 666f 7220 7369 7465 2063 6f6e  del for site con
+00001390: 6669 6775 7261 7469 6f6e 2e0d 0a2a 2054  figuration...* T
+000013a0: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
+000013b0: 206f 626a 6563 7420 6361 6e20 6f6e 6c79   object can only
+000013c0: 2062 6520 6368 616e 6765 642c 2074 6865   be changed, the
+000013d0: 7265 2773 206e 6f20 6c69 6e6b 2066 6f72  re's no link for
+000013e0: 2022 6164 6422 2028 3129 2e0d 0a2a 2054   "add" (1)...* T
+000013f0: 6865 206c 696e 6b20 746f 2074 6865 2063  he link to the c
+00001400: 6f6e 6669 6775 7261 7469 6f6e 2070 6167  onfiguration pag
+00001410: 6520 2832 2920 6469 7265 6374 6c79 2067  e (2) directly g
+00001420: 6f65 7320 746f 2074 6865 2066 6f72 6d20  oes to the form 
+00001430: 7061 6765 202d 206e 6f0d 0a20 206e 6565  page - no..  nee
+00001440: 6420 666f 7220 616e 2069 6e74 6572 6d65  d for an interme
+00001450: 6469 6172 7920 6f62 6a65 6374 206c 6973  diary object lis
+00001460: 7420 7061 6765 2c20 7369 6e63 6520 7468  t page, since th
+00001470: 6572 6527 7320 6f6e 6c79 206f 6e65 206f  ere's only one o
+00001480: 626a 6563 742e 0d0a 2a20 5468 6520 6564  bject...* The ed
+00001490: 6974 2070 6167 6520 6861 7320 6120 6d6f  it page has a mo
+000014a0: 6469 6669 6564 2062 7265 6164 6372 756d  dified breadcrum
+000014b0: 6220 2833 2920 746f 2061 766f 6964 206c  b (3) to avoid l
+000014c0: 696e 6b69 6e67 2074 6f20 7468 650d 0a20  inking to the.. 
+000014d0: 2069 6e74 6572 6d65 6469 6172 7920 6f62   intermediary ob
+000014e0: 6a65 6374 206c 6973 7420 7061 6765 2e0d  ject list page..
+000014f0: 0a2a 2046 726f 6d20 7468 6520 6564 6974  .* From the edit
+00001500: 2070 6167 652c 2077 6520 6361 6e6e 6f74   page, we cannot
+00001510: 2064 656c 6574 6520 7468 6520 6f62 6a65   delete the obje
+00001520: 6374 2028 3429 206e 6f72 2063 616e 2077  ct (4) nor can w
+00001530: 6520 6164 6420 6120 6e65 7720 6f6e 6520  e add a new one 
+00001540: 2835 292e 0d0a 0d0a 4966 2079 6f75 2077  (5).....If you w
+00001550: 6973 6820 746f 2064 6973 6162 6c65 2074  ish to disable t
+00001560: 6865 2073 6b69 7070 696e 6720 6f66 2074  he skipping of t
+00001570: 6865 206f 626a 6563 7420 6c69 7374 2070  he object list p
+00001580: 6167 652c 2061 6e64 2068 6176 6520 7468  age, and have th
+00001590: 6520 6465 6661 756c 740d 0a62 7265 6164  e default..bread
+000015a0: 6372 756d 6273 2c20 796f 7520 7368 6f75  crumbs, you shou
+000015b0: 6c64 2073 6574 2060 534f 4c4f 5f41 444d  ld set `SOLO_ADM
+000015c0: 494e 5f53 4b49 505f 4f42 4a45 4354 5f4c  IN_SKIP_OBJECT_L
+000015d0: 4953 545f 5041 4745 6020 746f 2060 4661  IST_PAGE` to `Fa
+000015e0: 6c73 6560 2069 6e20 796f 7572 2073 6574  lse` in your set
+000015f0: 7469 6e67 732e 0d0a 0d0a 4176 6169 6c61  tings.....Availa
+00001600: 6269 6c69 7479 2066 726f 6d20 7465 6d70  bility from temp
+00001610: 6c61 7465 730d 0a2d 2d2d 2d2d 2d2d 2d2d  lates..---------
+00001620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001630: 2d2d 0d0a 0d0a 5468 6520 7369 6e67 6c65  --....The single
+00001640: 746f 6e20 6f62 6a65 6374 2063 616e 2062  ton object can b
+00001650: 6520 7265 7472 6965 7665 6420 6672 6f6d  e retrieved from
+00001660: 2074 656d 706c 6174 6520 6279 2067 6976   template by giv
+00001670: 696e 6720 7468 6520 446a 616e 676f 206d  ing the Django m
+00001680: 6f64 656c 0d0a 646f 7474 6564 2070 6174  odel..dotted pat
+00001690: 683a 0d0a 0d0a 6060 6064 6a61 6e67 6f0d  h:....```django.
+000016a0: 0a7b 2520 6765 745f 736f 6c6f 2027 6170  .{% get_solo 'ap
+000016b0: 705f 6c61 6265 6c2e 4d6f 6465 6c4e 616d  p_label.ModelNam
+000016c0: 6527 2061 7320 6d79 5f63 6f6e 6669 6720  e' as my_config 
+000016d0: 257d 0d0a 6060 600d 0a0d 0a45 7861 6d70  %}..```....Examp
+000016e0: 6c65 3a0d 0a0d 0a60 6060 646a 616e 676f  le:....```django
+000016f0: 0d0a 7b25 206c 6f61 6420 736f 6c6f 5f74  ..{% load solo_t
+00001700: 6167 7320 257d 0d0a 7b25 2067 6574 5f73  ags %}..{% get_s
+00001710: 6f6c 6f20 2763 6f6e 6669 672e 5369 7465  olo 'config.Site
+00001720: 436f 6e66 6967 7572 6174 696f 6e27 2061  Configuration' a
+00001730: 7320 7369 7465 5f63 6f6e 6669 6720 257d  s site_config %}
+00001740: 0d0a 7b7b 2073 6974 655f 636f 6e66 6967  ..{{ site_config
+00001750: 2e73 6974 655f 6e61 6d65 207d 7d0d 0a7b  .site_name }}..{
+00001760: 7b20 7369 7465 5f63 6f6e 6669 672e 6d61  { site_config.ma
+00001770: 696e 7465 6e61 6e63 655f 6d6f 6465 207d  intenance_mode }
+00001780: 7d0d 0a60 6060 0d0a 0d0a 4966 2079 6f75  }..```....If you
+00001790: 2772 6520 6578 7465 6e64 696e 6720 6120  're extending a 
+000017a0: 7465 6d70 6c61 7465 2c20 6265 2073 7572  template, be sur
+000017b0: 6520 746f 2075 7365 2074 6865 2074 6167  e to use the tag
+000017c0: 2069 6e20 7468 6520 7072 6f70 6572 2073   in the proper s
+000017d0: 636f 7065 2e0d 0a0d 0a52 6967 6874 3a0d  cope.....Right:.
+000017e0: 0a0d 0a60 6060 646a 616e 676f 0d0a 7b25  ...```django..{%
+000017f0: 2065 7874 656e 6473 2022 696e 6465 782e   extends "index.
+00001800: 6874 6d6c 2220 257d 0d0a 7b25 206c 6f61  html" %}..{% loa
+00001810: 6420 736f 6c6f 5f74 6167 7320 257d 0d0a  d solo_tags %}..
+00001820: 0d0a 7b25 2062 6c6f 636b 2063 6f6e 7465  ..{% block conte
+00001830: 6e74 2025 7d0d 0a20 2020 207b 2520 6765  nt %}..    {% ge
+00001840: 745f 736f 6c6f 2027 636f 6e66 6967 2e53  t_solo 'config.S
+00001850: 6974 6543 6f6e 6669 6775 7261 7469 6f6e  iteConfiguration
+00001860: 2720 6173 2073 6974 655f 636f 6e66 6967  ' as site_config
+00001870: 2025 7d0d 0a20 2020 207b 7b20 7369 7465   %}..    {{ site
+00001880: 5f63 6f6e 6669 672e 7369 7465 5f6e 616d  _config.site_nam
+00001890: 6520 7d7d 0d0a 7b25 2065 6e64 626c 6f63  e }}..{% endbloc
+000018a0: 6b20 636f 6e74 656e 7420 257d 0d0a 6060  k content %}..``
+000018b0: 600d 0a0d 0a57 726f 6e67 3a0d 0a0d 0a60  `....Wrong:....`
+000018c0: 6060 646a 616e 676f 0d0a 7b25 2065 7874  ``django..{% ext
+000018d0: 656e 6473 2022 696e 6465 782e 6874 6d6c  ends "index.html
+000018e0: 2220 257d 0d0a 7b25 206c 6f61 6420 736f  " %}..{% load so
+000018f0: 6c6f 5f74 6167 7320 257d 0d0a 7b25 2067  lo_tags %}..{% g
+00001900: 6574 5f73 6f6c 6f20 2763 6f6e 6669 672e  et_solo 'config.
+00001910: 5369 7465 436f 6e66 6967 7572 6174 696f  SiteConfiguratio
+00001920: 6e27 2061 7320 7369 7465 5f63 6f6e 6669  n' as site_confi
+00001930: 6720 257d 0d0a 0d0a 7b25 2062 6c6f 636b  g %}....{% block
+00001940: 2063 6f6e 7465 6e74 2025 7d0d 0a20 2020   content %}..   
+00001950: 207b 7b20 7369 7465 5f63 6f6e 6669 672e   {{ site_config.
+00001960: 7369 7465 5f6e 616d 6520 7d7d 0d0a 7b25  site_name }}..{%
+00001970: 2065 6e64 626c 6f63 6b20 636f 6e74 656e   endblock conten
+00001980: 7420 257d 0d0a 6060 600d 0a0d 0a0d 0a43  t %}..```......C
+00001990: 6163 6869 6e67 0d0a 2d2d 2d2d 2d2d 2d0d  aching..-------.
+000019a0: 0a0d 0a42 7920 6465 6661 756c 7420 6361  ...By default ca
+000019b0: 6368 696e 6720 6973 2064 6973 6162 6c65  ching is disable
+000019c0: 643a 2065 7665 7279 2074 696d 6520 6067  d: every time `g
+000019d0: 6574 5f73 6f6c 6f60 2072 6574 7269 6576  et_solo` retriev
+000019e0: 6573 2074 6865 2073 696e 676c 6574 6f6e  es the singleton
+000019f0: 0d0a 6f62 6a65 6374 2c20 7468 6572 6520  ..object, there 
+00001a00: 7769 6c6c 2062 6520 6120 6461 7461 6261  will be a databa
+00001a10: 7365 2071 7565 7279 2e0d 0a0d 0a59 6f75  se query.....You
+00001a20: 2063 616e 2065 6e61 626c 6520 6361 6368   can enable cach
+00001a30: 696e 6720 746f 206f 6e6c 7920 7175 6572  ing to only quer
+00001a40: 7920 7468 6520 6461 7461 6261 7365 2077  y the database w
+00001a50: 6865 6e20 696e 6974 6961 6c6c 7920 7265  hen initially re
+00001a60: 7472 6965 7669 6e67 2074 6865 0d0a 6f62  trieving the..ob
+00001a70: 6a65 6374 2e20 5468 6520 6361 6368 6520  ject. The cache 
+00001a80: 7769 6c6c 2061 6c73 6f20 6265 2075 7064  will also be upd
+00001a90: 6174 6564 2077 6865 6e20 7570 6461 7465  ated when update
+00001aa0: 7320 6172 6520 6d61 6465 2066 726f 6d20  s are made from 
+00001ab0: 7468 6520 6164 6d69 6e2e 0d0a 0d0a 5468  the admin.....Th
+00001ac0: 6520 6361 6368 6520 7469 6d65 6f75 7420  e cache timeout 
+00001ad0: 6973 2063 6f6e 7472 6f6c 6c65 6420 7669  is controlled vi
+00001ae0: 6120 7468 6520 6053 4f4c 4f5f 4341 4348  a the `SOLO_CACH
+00001af0: 455f 5449 4d45 4f55 5460 2073 6574 7469  E_TIMEOUT` setti
+00001b00: 6e67 732e 0d0a 5468 6520 6361 6368 6520  ngs...The cache 
+00001b10: 6261 636b 656e 6420 746f 2062 6520 7573  backend to be us
+00001b20: 6564 2069 7320 636f 6e74 726f 6c6c 6564  ed is controlled
+00001b30: 2076 6961 2074 6865 2060 534f 4c4f 5f43   via the `SOLO_C
+00001b40: 4143 4845 6020 7365 7474 696e 6773 2e0d  ACHE` settings..
+00001b50: 0a0d 0a0d 0a53 6574 7469 6e67 730d 0a2d  .....Settings..-
+00001b60: 2d2d 2d2d 2d2d 2d0d 0a0d 0a23 2323 2054  -------....### T
+00001b70: 656d 706c 6174 6520 7461 6720 6e61 6d65  emplate tag name
+00001b80: 0d0a 0d0a 596f 7520 6361 6e20 7265 7472  ....You can retr
+00001b90: 6965 7665 2079 6f75 7220 7369 6e67 6c65  ieve your single
+00001ba0: 746f 6e20 6f62 6a65 6374 2069 6e20 7465  ton object in te
+00001bb0: 6d70 6c61 7465 7320 7573 696e 6720 7468  mplates using th
+00001bc0: 6520 6067 6574 5f73 6f6c 6f60 0d0a 7465  e `get_solo`..te
+00001bd0: 6d70 6c61 7465 2074 6167 2e0d 0a0d 0a59  mplate tag.....Y
+00001be0: 6f75 2063 616e 2063 6861 6e67 6520 7468  ou can change th
+00001bf0: 6520 6e61 6d65 2060 6765 745f 736f 6c6f  e name `get_solo
+00001c00: 6020 7573 696e 6720 7468 650d 0a60 4745  ` using the..`GE
+00001c10: 545f 534f 4c4f 5f54 454d 504c 4154 455f  T_SOLO_TEMPLATE_
+00001c20: 5441 475f 4e41 4d45 6020 7365 7474 696e  TAG_NAME` settin
+00001c30: 672e 0d0a 0d0a 6060 6070 7974 686f 6e0d  g.....```python.
+00001c40: 0a47 4554 5f53 4f4c 4f5f 5445 4d50 4c41  .GET_SOLO_TEMPLA
+00001c50: 5445 5f54 4147 5f4e 414d 4520 3d20 2767  TE_TAG_NAME = 'g
+00001c60: 6574 5f63 6f6e 6669 6727 0d0a 6060 600d  et_config'..```.
+00001c70: 0a0d 0a23 2323 2041 646d 696e 206f 7665  ...### Admin ove
+00001c80: 7272 6964 6520 666c 6167 0d0a 0d0a 4279  rride flag....By
+00001c90: 2064 6566 6175 6c74 2c20 7468 6520 6164   default, the ad
+00001ca0: 6d69 6e20 6973 206f 7665 7272 6964 6465  min is overridde
+00001cb0: 6e2e 2042 7574 2069 6620 796f 7520 7769  n. But if you wi
+00001cc0: 7368 2074 6f20 6b65 6570 2074 6865 206f  sh to keep the o
+00001cd0: 626a 6563 7420 6c69 7374 0d0a 7061 6765  bject list..page
+00001ce0: 2028 652e 672e 2074 6f20 6375 7374 6f6d   (e.g. to custom
+00001cf0: 697a 6520 6163 7469 6f6e 7329 2c20 796f  ize actions), yo
+00001d00: 7520 6361 6e20 7365 7420 7468 6520 6053  u can set the `S
+00001d10: 4f4c 4f5f 4144 4d49 4e5f 534b 4950 5f4f  OLO_ADMIN_SKIP_O
+00001d20: 424a 4543 545f 4c49 5354 5f50 4147 4560  BJECT_LIST_PAGE`
+00001d30: 0d0a 746f 2060 4661 6c73 6560 2e0d 0a0d  ..to `False`....
+00001d40: 0a60 6060 7079 7468 6f6e 0d0a 534f 4c4f  .```python..SOLO
+00001d50: 5f41 444d 494e 5f53 4b49 505f 4f42 4a45  _ADMIN_SKIP_OBJE
+00001d60: 4354 5f4c 4953 545f 5041 4745 203d 2054  CT_LIST_PAGE = T
+00001d70: 7275 650d 0a60 6060 0d0a 0d0a 2323 2320  rue..```....### 
+00001d80: 4361 6368 6520 6261 636b 656e 640d 0a0d  Cache backend...
+00001d90: 0a44 6a61 6e67 6f20 7072 6f76 6964 6573  .Django provides
+00001da0: 2061 2077 6179 2074 6f20 6465 6669 6e65   a way to define
+00001db0: 206d 756c 7469 706c 6520 6361 6368 6520   multiple cache 
+00001dc0: 6261 636b 656e 6473 2077 6974 6820 7468  backends with th
+00001dd0: 6520 6043 4143 4845 5360 0d0a 7365 7474  e `CACHES`..sett
+00001de0: 696e 6773 2e20 4966 2079 6f75 2077 616e  ings. If you wan
+00001df0: 7420 7468 6520 7369 6e67 6c65 746f 6e20  t the singleton 
+00001e00: 6f62 6a65 6374 2074 6f20 6265 2063 6163  object to be cac
+00001e10: 6865 6420 7365 7061 7261 7465 6c79 2c20  hed separately, 
+00001e20: 796f 750d 0a63 6f75 6c64 2064 6566 696e  you..could defin
+00001e30: 6520 7468 6520 6043 4143 4845 5360 2061  e the `CACHES` a
+00001e40: 6e64 2074 6865 2060 534f 4c4f 5f43 4143  nd the `SOLO_CAC
+00001e50: 4845 6020 7365 7474 696e 6773 206c 696b  HE` settings lik
+00001e60: 6520 7468 6973 3a0d 0a0d 0a60 6060 7079  e this:....```py
+00001e70: 7468 6f6e 0d0a 4341 4348 4553 203d 207b  thon..CACHES = {
+00001e80: 0d0a 2020 2020 2764 6566 6175 6c74 273a  ..    'default':
+00001e90: 207b 0d0a 2020 2020 2020 2020 2742 4143   {..        'BAC
+00001ea0: 4b45 4e44 273a 2027 646a 616e 676f 2e63  KEND': 'django.c
+00001eb0: 6f72 652e 6361 6368 652e 6261 636b 656e  ore.cache.backen
+00001ec0: 6473 2e6d 656d 6361 6368 6564 2e4d 656d  ds.memcached.Mem
+00001ed0: 6361 6368 6564 4361 6368 6527 2c0d 0a20  cachedCache',.. 
+00001ee0: 2020 2020 2020 2027 4c4f 4341 5449 4f4e         'LOCATION
+00001ef0: 273a 2027 3132 372e 302e 302e 313a 3131  ': '127.0.0.1:11
+00001f00: 3231 3127 2c0d 0a20 2020 207d 2c0d 0a20  211',..    },.. 
+00001f10: 2020 2027 6c6f 6361 6c27 3a20 7b0d 0a20     'local': {.. 
+00001f20: 2020 2020 2020 2027 4241 434b 454e 4427         'BACKEND'
+00001f30: 3a20 2764 6a61 6e67 6f2e 636f 7265 2e63  : 'django.core.c
+00001f40: 6163 6865 2e62 6163 6b65 6e64 732e 6c6f  ache.backends.lo
+00001f50: 636d 656d 2e4c 6f63 4d65 6d43 6163 6865  cmem.LocMemCache
+00001f60: 272c 0d0a 2020 2020 7d2c 0d0a 7d0d 0a0d  ',..    },..}...
+00001f70: 0a53 4f4c 4f5f 4341 4348 4520 3d20 276c  .SOLO_CACHE = 'l
+00001f80: 6f63 616c 270d 0a60 6060 0d0a 0d0a 4361  ocal'..```....Ca
+00001f90: 6368 696e 6720 7769 6c6c 2062 6520 6469  ching will be di
+00001fa0: 7361 626c 6564 2069 6620 7365 7420 746f  sabled if set to
+00001fb0: 2060 4e6f 6e65 602e 0d0a 0d0a 0d0a 2323   `None`.......##
+00001fc0: 2320 4361 6368 6520 7469 6d65 6f75 740d  # Cache timeout.
+00001fd0: 0a0d 0a54 6865 2063 6163 6865 2074 696d  ...The cache tim
+00001fe0: 656f 7574 2069 6e20 7365 636f 6e64 732e  eout in seconds.
+00001ff0: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a53  ....```python..S
+00002000: 4f4c 4f5f 4341 4348 455f 5449 4d45 4f55  OLO_CACHE_TIMEOU
+00002010: 5420 3d20 3630 2a35 2020 2320 3520 6d69  T = 60*5  # 5 mi
+00002020: 6e73 0d0a 6060 600d 0a0d 0a23 2323 2043  ns..```....### C
+00002030: 6163 6865 2070 7265 6669 780d 0a0d 0a54  ache prefix....T
+00002040: 6865 2070 7265 6669 7820 746f 2075 7365  he prefix to use
+00002050: 2066 6f72 2074 6865 2063 6163 6865 206b   for the cache k
+00002060: 6579 2e0d 0a0d 0a60 6060 7079 7468 6f6e  ey.....```python
+00002070: 0d0a 534f 4c4f 5f43 4143 4845 5f50 5245  ..SOLO_CACHE_PRE
+00002080: 4649 5820 3d20 2773 6f6c 6f27 0d0a 6060  FIX = 'solo'..``
+00002090: 600d 0a0d 0a47 6574 7469 6e67 2074 6865  `....Getting the
+000020a0: 2063 6f64 650d 0a3d 3d3d 3d3d 3d3d 3d3d   code..=========
+000020b0: 3d3d 3d3d 3d3d 3d0d 0a0d 0a54 6865 2063  =======....The c
+000020c0: 6f64 6520 6973 2068 6f73 7465 6420 6174  ode is hosted at
+000020d0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000020e0: 636f 6d2f 6c61 7a79 6269 7264 2f64 6a61  com/lazybird/dja
+000020f0: 6e67 6f2d 736f 6c6f 2f0d 0a0d 0a43 6865  ngo-solo/....Che
+00002100: 636b 206f 7574 2074 6865 206c 6174 6573  ck out the lates
+00002110: 7420 6465 7665 6c6f 706d 656e 7420 7665  t development ve
+00002120: 7273 696f 6e20 616e 6f6e 796d 6f75 736c  rsion anonymousl
+00002130: 7920 7769 7468 3a0d 0a0d 0a20 2020 2024  y with:....    $
+00002140: 2067 6974 2063 6c6f 6e65 2067 6974 3a2f   git clone git:/
+00002150: 2f67 6974 6875 622e 636f 6d2f 6c61 7a79  /github.com/lazy
+00002160: 6269 7264 2f64 6a61 6e67 6f2d 736f 6c6f  bird/django-solo
+00002170: 2e67 6974 0d0a 0d0a 596f 7520 6361 6e20  .git....You can 
+00002180: 696e 7374 616c 6c20 7468 6520 7061 636b  install the pack
+00002190: 6167 6520 696e 2074 6865 2022 6564 6974  age in the "edit
+000021a0: 6162 6c65 2220 6d6f 6465 206c 696b 6520  able" mode like 
+000021b0: 7468 6973 3a0d 0a0d 0a20 2020 2070 6970  this:....    pip
+000021c0: 2075 6e69 6e73 7461 6c6c 2064 6a61 6e67   uninstall djang
+000021d0: 6f2d 736f 6c6f 2020 2320 6a75 7374 2069  o-solo  # just i
+000021e0: 6e20 6361 7365 2e2e 2e0d 0a20 2020 2070  n case.....    p
+000021f0: 6970 2069 6e73 7461 6c6c 202d 6520 6769  ip install -e gi
+00002200: 742b 6874 7470 733a 2f2f 6769 7468 7562  t+https://github
+00002210: 2e63 6f6d 2f6c 617a 7962 6972 642f 646a  .com/lazybird/dj
+00002220: 616e 676f 2d73 6f6c 6f2e 6769 7423 6567  ango-solo.git#eg
+00002230: 673d 646a 616e 676f 2d73 6f6c 6f0d 0a0d  g=django-solo...
+00002240: 0a59 6f75 2063 616e 2061 6c73 6f20 696e  .You can also in
+00002250: 7374 616c 6c20 6120 7370 6563 6966 6963  stall a specific
+00002260: 2062 7261 6e63 683a 0d0a 0d0a 2020 2020   branch:....    
+00002270: 7069 7020 696e 7374 616c 6c20 2d65 2067  pip install -e g
+00002280: 6974 2b68 7474 7073 3a2f 2f67 6974 6875  it+https://githu
+00002290: 622e 636f 6d2f 6c61 7a79 6269 7264 2f64  b.com/lazybird/d
+000022a0: 6a61 6e67 6f2d 736f 6c6f 2e67 6974 406d  jango-solo.git@m
+000022b0: 792d 6272 616e 6368 2365 6767 3d64 6a61  y-branch#egg=dja
+000022c0: 6e67 6f2d 736f 6c6f 0d0a 0d0a 5468 6520  ngo-solo....The 
+000022d0: 7061 636b 6167 6520 6973 206e 6f77 2069  package is now i
+000022e0: 6e73 7461 6c6c 6564 2069 6e20 796f 7572  nstalled in your
+000022f0: 2070 726f 6a65 6374 2061 6e64 2079 6f75   project and you
+00002300: 2063 616e 2066 696e 6420 7468 6520 636f   can find the co
+00002310: 6465 2e0d 0a0d 0a54 6f20 7275 6e20 7468  de.....To run th
+00002320: 6520 756e 6974 2074 6573 7473 3a0d 0a0d  e unit tests:...
+00002330: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
+00002340: 2074 6f78 0d0a 2020 2020 746f 780d 0a0d   tox..    tox...
+00002350: 0a23 2323 204d 616b 696e 6720 6120 7265  .### Making a re
+00002360: 6c65 6173 650d 0a0d 0a31 2e20 5570 6461  lease....1. Upda
+00002370: 7465 205b 6073 6f6c 6f2f 5f5f 696e 6974  te [`solo/__init
+00002380: 5f5f 2e70 7960 5d28 736f 6c6f 2f5f 5f69  __.py`](solo/__i
+00002390: 6e69 745f 5f2e 7079 2920 6076 6572 7369  nit__.py) `versi
+000023a0: 6f6e 600d 0a0d 0a32 2e20 4d61 6b65 2061  on`....2. Make a
+000023b0: 206e 6577 2072 656c 6561 7365 206f 6e20   new release on 
+000023c0: 4769 7448 7562 0d0a 0d0a 6060 6073 6865  GitHub....```she
+000023d0: 6c6c 0d0a 746f 7820 2d65 2062 7569 6c64  ll..tox -e build
+000023e0: 0d0a 6060 600d 0a0d 0a60 6060 7368 656c  ..```....```shel
+000023f0: 6c0d 0a74 6f78 202d 6520 7570 6c6f 6164  l..tox -e upload
+00002400: 0d0a 6060 600d 0a                        ..```..
```

### Comparing `django-solo-2.0.0/django_solo.egg-info/PKG-INFO` & `django-solo-2.1.0/django_solo.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,544 +1,577 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 616e  : 2.1.Name: djan
-00000020: 676f 2d73 6f6c 6f0a 5665 7273 696f 6e3a  go-solo.Version:
-00000030: 2032 2e30 2e30 0a53 756d 6d61 7279 3a20   2.0.0.Summary: 
-00000040: 446a 616e 676f 2053 6f6c 6f20 6865 6c70  Django Solo help
-00000050: 7320 776f 726b 696e 6720 7769 7468 2073  s working with s
-00000060: 696e 676c 6574 6f6e 730a 486f 6d65 2d70  ingletons.Home-p
-00000070: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
-00000080: 6875 622e 636f 6d2f 6c61 7a79 6269 7264  hub.com/lazybird
-00000090: 2f64 6a61 6e67 6f2d 736f 6c6f 2f0a 4175  /django-solo/.Au
-000000a0: 7468 6f72 3a20 6c61 7a79 6269 7264 0a4c  thor: lazybird.L
-000000b0: 6963 656e 7365 3a20 4372 6561 7469 7665  icense: Creative
-000000c0: 2043 6f6d 6d6f 6e73 2041 7474 7269 6275   Commons Attribu
-000000d0: 7469 6f6e 2033 2e30 2055 6e70 6f72 7465  tion 3.0 Unporte
-000000e0: 640a 506c 6174 666f 726d 3a20 554e 4b4e  d.Platform: UNKN
-000000f0: 4f57 4e0a 436c 6173 7369 6669 6572 3a20  OWN.Classifier: 
-00000100: 4672 616d 6577 6f72 6b20 3a3a 2044 6a61  Framework :: Dja
-00000110: 6e67 6f20 3a3a 2032 2e32 0a43 6c61 7373  ngo :: 2.2.Class
-00000120: 6966 6965 723a 2046 7261 6d65 776f 726b  ifier: Framework
-00000130: 203a 3a20 446a 616e 676f 203a 3a20 332e   :: Django :: 3.
-00000140: 320a 436c 6173 7369 6669 6572 3a20 4672  2.Classifier: Fr
-00000150: 616d 6577 6f72 6b20 3a3a 2044 6a61 6e67  amework :: Djang
-00000160: 6f20 3a3a 2034 2e30 0a43 6c61 7373 6966  o :: 4.0.Classif
-00000170: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
-00000180: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
-00000190: 7065 7273 0a43 6c61 7373 6966 6965 723a  pers.Classifier:
-000001a0: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-000001b0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-000001c0: 656e 740a 436c 6173 7369 6669 6572 3a20  ent.Classifier: 
-000001d0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001e0: 7561 6765 203a 3a20 5079 7468 6f6e 0a43  uage :: Python.C
-000001f0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000200: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000210: 3a3a 2050 7974 686f 6e20 3a3a 2033 0a43  :: Python :: 3.C
-00000220: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000230: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000240: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e36  :: Python :: 3.6
-00000250: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000260: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000270: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000280: 2e37 0a43 6c61 7373 6966 6965 723a 2050  .7.Classifier: P
-00000290: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002a0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002b0: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
-000002c0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000002d0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000002e0: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
-000002f0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000300: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000310: 6e20 3a3a 2033 2e31 300a 5265 7175 6972  n :: 3.10.Requir
-00000320: 6573 2d50 7974 686f 6e3a 203e 3d33 2e36  es-Python: >=3.6
-00000330: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-00000340: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-00000350: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
-00000360: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
-00000370: 0a44 6a61 6e67 6f20 536f 6c6f 0a3d 3d3d  .Django Solo.===
-00000380: 3d3d 3d3d 3d3d 3d3d 0a0a 3c61 2068 7265  ========..<a hre
-00000390: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
-000003a0: 6f72 672f 7072 6f6a 6563 742f 646a 616e  org/project/djan
-000003b0: 676f 2d73 6f6c 6f2f 2220 616c 743d 2243  go-solo/" alt="C
-000003c0: 7572 7265 6e74 2076 6572 7369 6f6e 206f  urrent version o
-000003d0: 6e20 5079 5069 223e 3c69 6d67 2073 7263  n PyPi"><img src
-000003e0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-000003f0: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
-00000400: 646a 616e 676f 2d73 6f6c 6f2e 7376 6722  django-solo.svg"
-00000410: 202f 3e3c 2f61 3e0a 0a0a 2020 2020 2b2d   /></a>...    +-
-00000420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000430: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  ----------+.    
-00000440: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00000450: 2020 2020 2020 2020 2020 2020 7c0a 2020              |.  
-00000460: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00000470: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00000480: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00000490: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
-000004a0: 7c20 446a 616e 676f 2053 6f6c 6f20 6865  | Django Solo he
-000004b0: 6c70 7320 776f 726b 696e 6720 7769 7468  lps working with
-000004c0: 2073 696e 676c 6574 6f6e 733a 0a20 2020   singletons:.   
-000004d0: 207c 2020 2020 2020 2020 2020 2020 202f   |             /
-000004e0: 5c20 2020 2020 2020 2020 2020 207c 2064  \            | d
-000004f0: 6174 6162 6173 6520 7461 626c 6573 2074  atabase tables t
-00000500: 6861 7420 6f6e 6c79 2068 6176 6520 6f6e  hat only have on
-00000510: 6520 726f 772e 0a20 2020 207c 2020 2020  e row..    |    
-00000520: 2020 2020 2020 203e 3d29 273e 2020 2020         >=)'>    
-00000530: 2020 2020 2020 207c 2053 696e 676c 6574         | Singlet
-00000540: 6f6e 7320 6172 6520 7573 6566 756c 2066  ons are useful f
-00000550: 6f72 2074 6869 6e67 7320 6c69 6b65 2067  or things like g
-00000560: 6c6f 6261 6c0a 2020 2020 7c20 2020 2020  lobal.    |     
-00000570: 2020 2020 2020 2020 5c2f 2020 2020 2020          \/      
-00000580: 2020 2020 2020 7c20 7365 7474 696e 6773        | settings
-00000590: 2074 6861 7420 796f 7520 7761 6e74 2074   that you want t
-000005a0: 6f20 6564 6974 2066 726f 6d20 7468 6520  o edit from the 
-000005b0: 6164 6d69 6e0a 2020 2020 7c20 2020 2020  admin.    |     
-000005c0: 2020 2020 2020 2020 2f20 2020 2020 2020          /       
-000005d0: 2020 2020 2020 7c20 696e 7374 6561 6420        | instead 
-000005e0: 6f66 2068 6176 696e 6720 7468 656d 2069  of having them i
-000005f0: 6e20 446a 616e 676f 2073 6574 7469 6e67  n Django setting
-00000600: 732e 7079 2e0a 2020 2020 7c20 2020 2020  s.py..    |     
-00000610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000620: 2020 2020 2020 7c20 0a20 2020 207c 2020        | .    |  
-00000630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000640: 2020 2020 2020 2020 207c 200a 2020 2020           | .    
-00000650: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00000660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 0a0a  ------------+...
-00000670: 4665 6174 7572 6573 0a2d 2d2d 2d2d 2d2d  Features.-------
-00000680: 2d0a 0a53 6f6c 6f20 6865 6c70 7320 796f  -..Solo helps yo
-00000690: 7520 656e 666f 7263 6520 696e 7374 616e  u enforce instan
-000006a0: 7469 6174 696e 6720 6f6e 6c79 206f 6e65  tiating only one
-000006b0: 2069 6e73 7461 6e63 6520 6f66 2061 206d   instance of a m
-000006c0: 6f64 656c 2069 6e20 646a 616e 676f 2e0a  odel in django..
-000006d0: 0a2a 2059 6f75 2064 6566 696e 6520 7468  .* You define th
-000006e0: 6520 6d6f 6465 6c20 7468 6174 2077 696c  e model that wil
-000006f0: 6c20 686f 6c64 2079 6f75 7220 7369 6e67  l hold your sing
-00000700: 6c65 746f 6e20 6f62 6a65 6374 2e0a 2a20  leton object..* 
-00000710: 646a 616e 676f 2d73 6f6c 6f20 6769 7665  django-solo give
-00000720: 7320 6865 6c70 6572 2070 6172 656e 7420  s helper parent 
-00000730: 636c 6173 7320 666f 7220 796f 7572 206d  class for your m
-00000740: 6f64 656c 2061 6e64 2074 6865 2061 646d  odel and the adm
-00000750: 696e 2063 6c61 7373 6573 2e0a 2a20 596f  in classes..* Yo
-00000760: 7520 6765 7420 616e 2061 646d 696e 2069  u get an admin i
-00000770: 6e74 6572 6661 6365 2074 6861 7427 7320  nterface that's 
-00000780: 6177 6172 6520 796f 7520 6f6e 6c79 2068  aware you only h
-00000790: 6176 6520 6f6e 6520 6f62 6a65 6374 2e0a  ave one object..
-000007a0: 2a20 596f 7520 6361 6e20 7265 7472 6965  * You can retrie
-000007b0: 7665 2074 6865 206f 626a 6563 7420 6672  ve the object fr
-000007c0: 6f6d 2074 656d 706c 6174 6573 2e0a 2a20  om templates..* 
-000007d0: 4279 2065 6e61 626c 696e 6720 6361 6368  By enabling cach
-000007e0: 696e 672c 2074 6865 2064 6174 6162 6173  ing, the databas
-000007f0: 6520 6973 206e 6f74 2071 7565 7269 6564  e is not queried
-00000800: 2069 6e74 656e 7369 7665 6c79 2e0a 0a55   intensively...U
-00000810: 7365 2043 6173 6573 0a2d 2d2d 2d2d 2d2d  se Cases.-------
-00000820: 2d0a 0a44 6a61 6e67 6f20 536f 6c6f 2069  -..Django Solo i
-00000830: 7320 616c 736f 2067 7265 6174 2066 6f72  s also great for
-00000840: 2075 7365 2077 6974 6820 7369 6e67 6c65   use with single
-00000850: 746f 6e20 6f62 6a65 6374 7320 7468 6174  ton objects that
-00000860: 2068 6176 6520 6120 6f6e 6520 746f 206d   have a one to m
-00000870: 616e 7920 7265 6c61 7469 6f6e 7368 6970  any relationship
-00000880: 2e20 4c69 6b65 2074 6865 2075 7365 2063  . Like the use c
-00000890: 6173 6520 6265 6c6f 7720 7768 6572 6520  ase below where 
-000008a0: 796f 7520 6861 7665 2061 2027 486f 6d65  you have a 'Home
-000008b0: 2053 6c69 6465 7222 2074 6861 7420 6861   Slider" that ha
-000008c0: 7320 6d61 6e79 2022 536c 6964 6573 222e  s many "Slides".
-000008d0: 0a0a 2a20 476c 6f62 616c 206f 7220 6465  ..* Global or de
-000008e0: 6661 756c 7420 7365 7474 696e 6773 0a2a  fault settings.*
-000008f0: 2041 6e20 696d 6167 6520 736c 6964 6572   An image slider
-00000900: 2074 6861 7420 6861 7320 6d61 6e79 2073   that has many s
-00000910: 6c69 6465 730a 2a20 4120 7061 6765 2073  lides.* A page s
-00000920: 6563 7469 6f6e 2074 6861 7420 6861 7320  ection that has 
-00000930: 7375 622d 7365 6374 696f 6e73 0a2a 2041  sub-sections.* A
-00000940: 2074 6561 6d20 6269 6f20 7769 7468 206d   team bio with m
-00000950: 616e 7920 7465 616d 206d 656d 6265 7273  any team members
-00000960: 0a0a 5468 6572 6520 6172 6520 6d61 6e79  ..There are many
-00000970: 2063 6173 6573 2077 6865 7265 2069 7420   cases where it 
-00000980: 6d61 6b65 7320 7365 6e73 6520 666f 7220  makes sense for 
-00000990: 7468 6520 7061 7265 6e74 2069 6e20 6120  the parent in a 
-000009a0: 6f6e 6520 746f 206d 616e 7920 7265 6c61  one to many rela
-000009b0: 7469 6f6e 7368 6970 2074 6f20 6265 206c  tionship to be l
-000009c0: 696d 6974 6564 2074 6f20 6120 7369 6e67  imited to a sing
-000009d0: 6c65 2069 6e73 7461 6e63 652e 0a0a 5573  le instance...Us
-000009e0: 6167 6520 4578 616d 706c 650a 0a60 6060  age Example..```
-000009f0: 7079 7468 6f6e 0a23 206d 6f64 656c 732e  python.# models.
-00000a00: 7079 0a0a 6672 6f6d 2064 6a61 6e67 6f2e  py..from django.
-00000a10: 6462 2069 6d70 6f72 7420 6d6f 6465 6c73  db import models
-00000a20: 0a66 726f 6d20 736f 6c6f 2e6d 6f64 656c  .from solo.model
-00000a30: 7320 696d 706f 7274 2053 696e 676c 6574  s import Singlet
-00000a40: 6f6e 4d6f 6465 6c0a 0a0a 636c 6173 7320  onModel...class 
-00000a50: 5369 7465 436f 6e66 6967 7572 6174 696f  SiteConfiguratio
-00000a60: 6e28 5369 6e67 6c65 746f 6e4d 6f64 656c  n(SingletonModel
-00000a70: 293a 0a20 2020 2073 6974 655f 6e61 6d65  ):.    site_name
-00000a80: 203d 206d 6f64 656c 732e 4368 6172 4669   = models.CharFi
-00000a90: 656c 6428 6d61 785f 6c65 6e67 7468 3d32  eld(max_length=2
-00000aa0: 3535 2c20 6465 6661 756c 743d 2753 6974  55, default='Sit
-00000ab0: 6520 4e61 6d65 2729 0a20 2020 206d 6169  e Name').    mai
-00000ac0: 6e74 656e 616e 6365 5f6d 6f64 6520 3d20  ntenance_mode = 
-00000ad0: 6d6f 6465 6c73 2e42 6f6f 6c65 616e 4669  models.BooleanFi
-00000ae0: 656c 6428 6465 6661 756c 743d 4661 6c73  eld(default=Fals
-00000af0: 6529 0a0a 2020 2020 6465 6620 5f5f 7374  e)..    def __st
-00000b00: 725f 5f28 7365 6c66 293a 0a20 2020 2020  r__(self):.     
-00000b10: 2020 2072 6574 7572 6e20 2253 6974 6520     return "Site 
-00000b20: 436f 6e66 6967 7572 6174 696f 6e22 0a0a  Configuration"..
-00000b30: 2020 2020 636c 6173 7320 4d65 7461 3a0a      class Meta:.
-00000b40: 2020 2020 2020 2020 7665 7262 6f73 655f          verbose_
-00000b50: 6e61 6d65 203d 2022 5369 7465 2043 6f6e  name = "Site Con
-00000b60: 6669 6775 7261 7469 6f6e 220a 6060 600a  figuration".```.
-00000b70: 0a60 6060 7079 7468 6f6e 0a23 2061 646d  .```python.# adm
-00000b80: 696e 2e70 790a 0a66 726f 6d20 646a 616e  in.py..from djan
-00000b90: 676f 2e63 6f6e 7472 6962 2069 6d70 6f72  go.contrib impor
-00000ba0: 7420 6164 6d69 6e0a 6672 6f6d 2073 6f6c  t admin.from sol
-00000bb0: 6f2e 6164 6d69 6e20 696d 706f 7274 2053  o.admin import S
-00000bc0: 696e 676c 6574 6f6e 4d6f 6465 6c41 646d  ingletonModelAdm
-00000bd0: 696e 0a66 726f 6d20 636f 6e66 6967 2e6d  in.from config.m
-00000be0: 6f64 656c 7320 696d 706f 7274 2053 6974  odels import Sit
-00000bf0: 6543 6f6e 6669 6775 7261 7469 6f6e 0a0a  eConfiguration..
-00000c00: 0a61 646d 696e 2e73 6974 652e 7265 6769  .admin.site.regi
-00000c10: 7374 6572 2853 6974 6543 6f6e 6669 6775  ster(SiteConfigu
-00000c20: 7261 7469 6f6e 2c20 5369 6e67 6c65 746f  ration, Singleto
-00000c30: 6e4d 6f64 656c 4164 6d69 6e29 0a60 6060  nModelAdmin).```
-00000c40: 0a0a 6060 6070 7974 686f 6e0a 2320 5468  ..```python.# Th
-00000c50: 6572 6520 6973 206f 6e6c 7920 6f6e 6520  ere is only one 
-00000c60: 6974 656d 2069 6e20 7468 6520 7461 626c  item in the tabl
-00000c70: 652c 2079 6f75 2063 616e 2067 6574 2069  e, you can get i
-00000c80: 7420 7468 6973 2077 6179 3a0a 6672 6f6d  t this way:.from
-00000c90: 202e 6d6f 6465 6c73 2069 6d70 6f72 7420   .models import 
-00000ca0: 5369 7465 436f 6e66 6967 7572 6174 696f  SiteConfiguratio
-00000cb0: 6e0a 636f 6e66 6967 203d 2053 6974 6543  n.config = SiteC
-00000cc0: 6f6e 6669 6775 7261 7469 6f6e 2e6f 626a  onfiguration.obj
-00000cd0: 6563 7473 2e67 6574 2829 0a0a 2320 6765  ects.get()..# ge
-00000ce0: 745f 736f 6c6f 2077 696c 6c20 6372 6561  t_solo will crea
-00000cf0: 7465 2074 6865 2069 7465 6d20 6966 2069  te the item if i
-00000d00: 7420 646f 6573 206e 6f74 2061 6c72 6561  t does not alrea
-00000d10: 6479 2065 7869 7374 0a63 6f6e 6669 6720  dy exist.config 
-00000d20: 3d20 5369 7465 436f 6e66 6967 7572 6174  = SiteConfigurat
-00000d30: 696f 6e2e 6765 745f 736f 6c6f 2829 0a60  ion.get_solo().`
-00000d40: 6060 0a0a 496e 2079 6f75 7220 6d6f 6465  ``..In your mode
-00000d50: 6c2c 206e 6f74 6520 686f 7720 796f 7520  l, note how you 
-00000d60: 6469 6420 6e6f 7420 6861 7665 2074 6f20  did not have to 
-00000d70: 7072 6f76 6964 6520 6120 6076 6572 626f  provide a `verbo
-00000d80: 7365 5f6e 616d 655f 706c 7572 616c 6020  se_name_plural` 
-00000d90: 6669 656c 6420 2d0a 5468 6174 2773 2062  field -.That's b
-00000da0: 6563 6175 7365 2044 6a61 6e67 6f20 536f  ecause Django So
-00000db0: 6c6f 2075 7365 7320 7468 6520 6076 6572  lo uses the `ver
-00000dc0: 626f 7365 5f6e 616d 6560 2069 6e73 7465  bose_name` inste
-00000dd0: 6164 2e0a 0a49 6620 796f 7527 7265 2063  ad...If you're c
-00000de0: 6861 6e67 696e 6720 616e 2065 7869 7374  hanging an exist
-00000df0: 696e 6720 6d6f 6465 6c20 2877 6869 6368  ing model (which
-00000e00: 2061 6c72 6561 6479 2068 6173 2073 6f6d   already has som
-00000e10: 6520 6f62 6a65 6374 7320 7374 6f72 6564  e objects stored
-00000e20: 2069 6e20 7468 6520 6461 7461 6261 7365   in the database
-00000e30: 2920 746f 2061 2073 696e 676c 6574 6f6e  ) to a singleton
-00000e40: 206d 6f64 656c 2c20 796f 7520 6361 6e20   model, you can 
-00000e50: 6578 706c 6963 6974 6c79 2070 726f 7669  explicitly provi
-00000e60: 6465 2074 6865 2069 6420 6f66 2074 6865  de the id of the
-00000e70: 2072 6f77 2069 6e20 7468 6520 6461 7461   row in the data
-00000e80: 6261 7365 2066 6f72 2064 6a61 6e67 6f2d  base for django-
-00000e90: 736f 6c6f 2074 6f20 7573 652e 2054 6869  solo to use. Thi
-00000ea0: 7320 6361 6e20 6265 2064 6f6e 6520 6279  s can be done by
-00000eb0: 2073 6574 7469 6e67 2060 7369 6e67 6c65   setting `single
-00000ec0: 746f 6e5f 696e 7374 616e 6365 5f69 6460  ton_instance_id`
-00000ed0: 2070 726f 7065 7274 7920 6f6e 2074 6865   property on the
-00000ee0: 206d 6f64 656c 3a0a 0a60 6060 7079 7468   model:..```pyth
-00000ef0: 6f6e 0a63 6c61 7373 2053 6974 6543 6f6e  on.class SiteCon
-00000f00: 6669 6775 7261 7469 6f6e 2853 696e 676c  figuration(Singl
-00000f10: 6574 6f6e 4d6f 6465 6c29 3a0a 2020 2020  etonModel):.    
-00000f20: 7369 6e67 6c65 746f 6e5f 696e 7374 616e  singleton_instan
-00000f30: 6365 5f69 6420 3d20 3234 0a20 2020 2023  ce_id = 24.    #
-00000f40: 2028 2e2e 2e29 0a60 6060 0a0a 496e 7374   (...).```..Inst
-00000f50: 616c 6c61 7469 6f6e 0a2d 2d2d 2d2d 2d2d  allation.-------
-00000f60: 2d2d 2d2d 2d0a 0a54 6869 7320 6170 706c  -----..This appl
-00000f70: 6963 6174 696f 6e20 7265 7175 6972 6573  ication requires
-00000f80: 2044 6a61 6e67 6f20 322e 322c 2033 2e32   Django 2.2, 3.2
-00000f90: 2c20 6f72 2034 2e30 2e0a 0a2a 2049 6e73  , or 4.0...* Ins
-00000fa0: 7461 6c6c 2074 6865 2070 6163 6b61 6765  tall the package
-00000fb0: 2075 7369 6e67 2060 7069 7020 696e 7374   using `pip inst
-00000fc0: 616c 6c20 646a 616e 676f 2d73 6f6c 6f60  all django-solo`
-00000fd0: 0a2a 2041 6464 2060 6073 6f6c 6f60 6020  .* Add ``solo`` 
-00000fe0: 6f72 2060 6073 6f6c 6f2e 6170 7073 2e53  or ``solo.apps.S
-00000ff0: 6f6c 6f41 7070 436f 6e66 6967 6060 2074  oloAppConfig`` t
-00001000: 6f20 796f 7572 2060 6049 4e53 5441 4c4c  o your ``INSTALL
-00001010: 4544 5f41 5050 5360 6020 7365 7474 696e  ED_APPS`` settin
-00001020: 672e 0a0a 5468 6973 2069 7320 686f 7720  g...This is how 
-00001030: 796f 7520 7275 6e20 7465 7374 733a 0a0a  you run tests:..
-00001040: 2020 2020 2e2f 6d61 6e61 6765 2e70 7920      ./manage.py 
-00001050: 7465 7374 2073 6f6c 6f20 2d2d 7365 7474  test solo --sett
-00001060: 696e 6773 3d73 6f6c 6f2e 7465 7374 732e  ings=solo.tests.
-00001070: 7365 7474 696e 6773 0a0a 416e 6420 6672  settings..And fr
-00001080: 6f6d 2077 6974 6869 6e20 6074 6f78 603a  om within `tox`:
-00001090: 0a0a 6060 600a 7079 7468 6f6e 202d 6d20  ..```.python -m 
-000010a0: 7069 7020 696e 7374 616c 6c20 746f 780a  pip install tox.
-000010b0: 746f 780a 6060 600a 0a53 7570 706f 7274  tox.```..Support
-000010c0: 6564 204c 616e 6775 6167 6573 0a2d 2d2d  ed Languages.---
-000010d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000010e0: 0a0a 2d20 456e 676c 6973 680a 2d20 5370  ..- English.- Sp
-000010f0: 616e 6973 680a 0a41 646d 696e 0a2d 2d2d  anish..Admin.---
-00001100: 2d2d 0a0a 5468 6520 7374 616e 6461 7264  --..The standard
-00001110: 2044 6a61 6e67 6f20 6164 6d69 6e20 646f   Django admin do
-00001120: 6573 206e 6f74 2066 6974 2077 656c 6c20  es not fit well 
-00001130: 7768 656e 2077 6f72 6b69 6e67 2077 6974  when working wit
-00001140: 6820 7369 6e67 6c65 746f 6e2c 0a66 6f72  h singleton,.for
-00001150: 2069 6e73 7461 6e63 652c 2069 6620 796f   instance, if yo
-00001160: 7520 6e65 6564 2073 6f6d 6520 676c 6f62  u need some glob
-00001170: 616c 2073 6974 6520 7365 7474 696e 6773  al site settings
-00001180: 2074 6f20 6265 2065 6469 7465 6420 696e   to be edited in
-00001190: 2074 6865 2061 646d 696e 2e0a 446a 616e   the admin..Djan
-000011a0: 676f 2053 6f6c 6f20 7072 6f76 6964 6573  go Solo provides
-000011b0: 2061 206d 6f64 6966 6965 6420 6164 6d69   a modified admi
-000011c0: 6e20 666f 7220 7468 6174 2e0a 0a0a 215b  n for that....![
-000011d0: 646a 616e 676f 2d73 6f6c 6f20 6164 6d69  django-solo admi
-000011e0: 6e5d 2868 7474 7073 3a2f 2f72 6177 2e67  n](https://raw.g
-000011f0: 6974 6875 622e 636f 6d2f 6c61 7a79 6269  ithub.com/lazybi
-00001200: 7264 2f64 6a61 6e67 6f2d 736f 6c6f 2f6d  rd/django-solo/m
-00001210: 6173 7465 722f 646f 6373 2f69 6d61 6765  aster/docs/image
-00001220: 732f 646a 616e 676f 2d73 6f6c 6f2d 6164  s/django-solo-ad
-00001230: 6d69 6e2e 6a70 6720 2264 6a61 6e67 6f2d  min.jpg "django-
-00001240: 736f 6c6f 2061 646d 696e 2229 0a0a 0a2a  solo admin")...*
-00001250: 2049 6e20 7468 6520 6164 6d69 6e20 686f   In the admin ho
-00001260: 6d65 2070 6167 6520 7768 6572 6520 616c  me page where al
-00001270: 6c20 6170 706c 6963 6174 696f 6e73 2061  l applications a
-00001280: 7265 206c 6973 7465 642c 2077 6520 6861  re listed, we ha
-00001290: 7665 2061 2060 636f 6e66 6967 600a 2020  ve a `config`.  
-000012a0: 6170 706c 6963 6174 696f 6e20 7468 6174  application that
-000012b0: 2068 6f6c 6473 2061 2073 696e 676c 6574   holds a singlet
-000012c0: 6f6e 206d 6f64 656c 2066 6f72 2073 6974  on model for sit
-000012d0: 6520 636f 6e66 6967 7572 6174 696f 6e2e  e configuration.
-000012e0: 0a2a 2054 6865 2063 6f6e 6669 6775 7261  .* The configura
-000012f0: 7469 6f6e 206f 626a 6563 7420 6361 6e20  tion object can 
-00001300: 6f6e 6c79 2062 6520 6368 616e 6765 642c  only be changed,
-00001310: 2074 6865 7265 2773 206e 6f20 6c69 6e6b   there's no link
-00001320: 2066 6f72 2022 6164 6422 2028 3129 2e0a   for "add" (1)..
-00001330: 2a20 5468 6520 6c69 6e6b 2074 6f20 7468  * The link to th
-00001340: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
-00001350: 7061 6765 2028 3229 2064 6972 6563 746c  page (2) directl
-00001360: 7920 676f 6573 2074 6f20 7468 6520 666f  y goes to the fo
-00001370: 726d 2070 6167 6520 2d20 6e6f 0a20 206e  rm page - no.  n
-00001380: 6565 6420 666f 7220 616e 2069 6e74 6572  eed for an inter
-00001390: 6d65 6469 6172 7920 6f62 6a65 6374 206c  mediary object l
-000013a0: 6973 7420 7061 6765 2c20 7369 6e63 6520  ist page, since 
-000013b0: 7468 6572 6527 7320 6f6e 6c79 206f 6e65  there's only one
-000013c0: 206f 626a 6563 742e 0a2a 2054 6865 2065   object..* The e
-000013d0: 6469 7420 7061 6765 2068 6173 2061 206d  dit page has a m
-000013e0: 6f64 6966 6965 6420 6272 6561 6463 7275  odified breadcru
-000013f0: 6d62 2028 3329 2074 6f20 6176 6f69 6420  mb (3) to avoid 
-00001400: 6c69 6e6b 696e 6720 746f 2074 6865 0a20  linking to the. 
-00001410: 2069 6e74 6572 6d65 6469 6172 7920 6f62   intermediary ob
-00001420: 6a65 6374 206c 6973 7420 7061 6765 2e0a  ject list page..
-00001430: 2a20 4672 6f6d 2074 6865 2065 6469 7420  * From the edit 
-00001440: 7061 6765 2c20 7765 2063 616e 6e6f 7420  page, we cannot 
-00001450: 6465 6c65 7465 2074 6865 206f 626a 6563  delete the objec
-00001460: 7420 2834 2920 6e6f 7220 6361 6e20 7765  t (4) nor can we
-00001470: 2061 6464 2061 206e 6577 206f 6e65 2028   add a new one (
-00001480: 3529 2e0a 0a49 6620 796f 7520 7769 7368  5)...If you wish
-00001490: 2074 6f20 6469 7361 626c 6520 7468 6520   to disable the 
-000014a0: 736b 6970 7069 6e67 206f 6620 7468 6520  skipping of the 
-000014b0: 6f62 6a65 6374 206c 6973 7420 7061 6765  object list page
-000014c0: 2c20 616e 6420 6861 7665 2074 6865 2064  , and have the d
-000014d0: 6566 6175 6c74 0a62 7265 6164 6372 756d  efault.breadcrum
-000014e0: 6273 2c20 796f 7520 7368 6f75 6c64 2073  bs, you should s
-000014f0: 6574 2060 534f 4c4f 5f41 444d 494e 5f53  et `SOLO_ADMIN_S
-00001500: 4b49 505f 4f42 4a45 4354 5f4c 4953 545f  KIP_OBJECT_LIST_
-00001510: 5041 4745 6020 746f 2060 4661 6c73 6560  PAGE` to `False`
-00001520: 2069 6e20 796f 7572 2073 6574 7469 6e67   in your setting
-00001530: 732e 0a0a 4176 6169 6c61 6269 6c69 7479  s...Availability
-00001540: 2066 726f 6d20 7465 6d70 6c61 7465 730a   from templates.
-00001550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a54 6865  -----------..The
-00001570: 2073 696e 676c 6574 6f6e 206f 626a 6563   singleton objec
-00001580: 7420 6361 6e20 6265 2072 6574 7269 6576  t can be retriev
-00001590: 6564 2066 726f 6d20 7465 6d70 6c61 7465  ed from template
-000015a0: 2062 7920 6769 7669 6e67 2074 6865 2044   by giving the D
-000015b0: 6a61 6e67 6f20 6d6f 6465 6c0a 646f 7474  jango model.dott
-000015c0: 6564 2070 6174 683a 0a0a 6060 6064 6a61  ed path:..```dja
-000015d0: 6e67 6f0a 7b25 2067 6574 5f73 6f6c 6f20  ngo.{% get_solo 
-000015e0: 2761 7070 5f6c 6162 656c 2e4d 6f64 656c  'app_label.Model
-000015f0: 4e61 6d65 2720 6173 206d 795f 636f 6e66  Name' as my_conf
-00001600: 6967 2025 7d0a 6060 600a 0a45 7861 6d70  ig %}.```..Examp
-00001610: 6c65 3a0a 0a60 6060 646a 616e 676f 0a7b  le:..```django.{
-00001620: 2520 6c6f 6164 2073 6f6c 6f5f 7461 6773  % load solo_tags
-00001630: 2025 7d0a 7b25 2067 6574 5f73 6f6c 6f20   %}.{% get_solo 
-00001640: 2763 6f6e 6669 672e 5369 7465 436f 6e66  'config.SiteConf
-00001650: 6967 7572 6174 696f 6e27 2061 7320 7369  iguration' as si
-00001660: 7465 5f63 6f6e 6669 6720 257d 0a7b 7b20  te_config %}.{{ 
-00001670: 7369 7465 5f63 6f6e 6669 672e 7369 7465  site_config.site
-00001680: 5f6e 616d 6520 7d7d 0a7b 7b20 7369 7465  _name }}.{{ site
-00001690: 5f63 6f6e 6669 672e 6d61 696e 7465 6e61  _config.maintena
-000016a0: 6e63 655f 6d6f 6465 207d 7d0a 6060 600a  nce_mode }}.```.
-000016b0: 0a49 6620 796f 7527 7265 2065 7874 656e  .If you're exten
-000016c0: 6469 6e67 2061 2074 656d 706c 6174 652c  ding a template,
-000016d0: 2062 6520 7375 7265 2074 6f20 7573 6520   be sure to use 
-000016e0: 7468 6520 7461 6720 696e 2074 6865 2070  the tag in the p
-000016f0: 726f 7065 7220 7363 6f70 652e 0a0a 5269  roper scope...Ri
-00001700: 6768 743a 0a0a 6060 6064 6a61 6e67 6f0a  ght:..```django.
-00001710: 7b25 2065 7874 656e 6473 2022 696e 6465  {% extends "inde
-00001720: 782e 6874 6d6c 2220 257d 0a7b 2520 6c6f  x.html" %}.{% lo
-00001730: 6164 2073 6f6c 6f5f 7461 6773 2025 7d0a  ad solo_tags %}.
-00001740: 0a7b 2520 626c 6f63 6b20 636f 6e74 656e  .{% block conten
-00001750: 7420 257d 0a20 2020 207b 2520 6765 745f  t %}.    {% get_
-00001760: 736f 6c6f 2027 636f 6e66 6967 2e53 6974  solo 'config.Sit
-00001770: 6543 6f6e 6669 6775 7261 7469 6f6e 2720  eConfiguration' 
-00001780: 6173 2073 6974 655f 636f 6e66 6967 2025  as site_config %
-00001790: 7d0a 2020 2020 7b7b 2073 6974 655f 636f  }.    {{ site_co
-000017a0: 6e66 6967 2e73 6974 655f 6e61 6d65 207d  nfig.site_name }
-000017b0: 7d0a 7b25 2065 6e64 626c 6f63 6b20 636f  }.{% endblock co
-000017c0: 6e74 656e 7420 257d 0a60 6060 0a0a 5772  ntent %}.```..Wr
-000017d0: 6f6e 673a 0a0a 6060 6064 6a61 6e67 6f0a  ong:..```django.
-000017e0: 7b25 2065 7874 656e 6473 2022 696e 6465  {% extends "inde
-000017f0: 782e 6874 6d6c 2220 257d 0a7b 2520 6c6f  x.html" %}.{% lo
-00001800: 6164 2073 6f6c 6f5f 7461 6773 2025 7d0a  ad solo_tags %}.
-00001810: 7b25 2067 6574 5f73 6f6c 6f20 2763 6f6e  {% get_solo 'con
-00001820: 6669 672e 5369 7465 436f 6e66 6967 7572  fig.SiteConfigur
-00001830: 6174 696f 6e27 2061 7320 7369 7465 5f63  ation' as site_c
-00001840: 6f6e 6669 6720 257d 0a0a 7b25 2062 6c6f  onfig %}..{% blo
-00001850: 636b 2063 6f6e 7465 6e74 2025 7d0a 2020  ck content %}.  
-00001860: 2020 7b7b 2073 6974 655f 636f 6e66 6967    {{ site_config
-00001870: 2e73 6974 655f 6e61 6d65 207d 7d0a 7b25  .site_name }}.{%
-00001880: 2065 6e64 626c 6f63 6b20 636f 6e74 656e   endblock conten
-00001890: 7420 257d 0a60 6060 0a0a 0a43 6163 6869  t %}.```...Cachi
-000018a0: 6e67 0a2d 2d2d 2d2d 2d2d 0a0a 4279 2064  ng.-------..By d
-000018b0: 6566 6175 6c74 2063 6163 6869 6e67 2069  efault caching i
-000018c0: 7320 6469 7361 626c 6564 3a20 6576 6572  s disabled: ever
-000018d0: 7920 7469 6d65 2060 6765 745f 736f 6c6f  y time `get_solo
-000018e0: 6020 7265 7472 6965 7665 7320 7468 6520  ` retrieves the 
-000018f0: 7369 6e67 6c65 746f 6e0a 6f62 6a65 6374  singleton.object
-00001900: 2c20 7468 6572 6520 7769 6c6c 2062 6520  , there will be 
-00001910: 6120 6461 7461 6261 7365 2071 7565 7279  a database query
-00001920: 2e0a 0a59 6f75 2063 616e 2065 6e61 626c  ...You can enabl
-00001930: 6520 6361 6368 696e 6720 746f 206f 6e6c  e caching to onl
-00001940: 7920 7175 6572 7920 7468 6520 6461 7461  y query the data
-00001950: 6261 7365 2077 6865 6e20 696e 6974 6961  base when initia
-00001960: 6c6c 7920 7265 7472 6965 7669 6e67 2074  lly retrieving t
-00001970: 6865 0a6f 626a 6563 742e 2054 6865 2063  he.object. The c
-00001980: 6163 6865 2077 696c 6c20 616c 736f 2062  ache will also b
-00001990: 6520 7570 6461 7465 6420 7768 656e 2075  e updated when u
-000019a0: 7064 6174 6573 2061 7265 206d 6164 6520  pdates are made 
-000019b0: 6672 6f6d 2074 6865 2061 646d 696e 2e0a  from the admin..
-000019c0: 0a54 6865 2063 6163 6865 2074 696d 656f  .The cache timeo
-000019d0: 7574 2069 7320 636f 6e74 726f 6c6c 6564  ut is controlled
-000019e0: 2076 6961 2074 6865 2060 534f 4c4f 5f43   via the `SOLO_C
-000019f0: 4143 4845 5f54 494d 454f 5554 6020 7365  ACHE_TIMEOUT` se
-00001a00: 7474 696e 6773 2e0a 5468 6520 6361 6368  ttings..The cach
-00001a10: 6520 6261 636b 656e 6420 746f 2062 6520  e backend to be 
-00001a20: 7573 6564 2069 7320 636f 6e74 726f 6c6c  used is controll
-00001a30: 6564 2076 6961 2074 6865 2060 534f 4c4f  ed via the `SOLO
-00001a40: 5f43 4143 4845 6020 7365 7474 696e 6773  _CACHE` settings
-00001a50: 2e0a 0a0a 5365 7474 696e 6773 0a2d 2d2d  ....Settings.---
-00001a60: 2d2d 2d2d 2d0a 0a23 2323 2054 656d 706c  -----..### Templ
-00001a70: 6174 6520 7461 6720 6e61 6d65 0a0a 596f  ate tag name..Yo
-00001a80: 7520 6361 6e20 7265 7472 6965 7665 2079  u can retrieve y
-00001a90: 6f75 7220 7369 6e67 6c65 746f 6e20 6f62  our singleton ob
-00001aa0: 6a65 6374 2069 6e20 7465 6d70 6c61 7465  ject in template
-00001ab0: 7320 7573 696e 6720 7468 6520 6067 6574  s using the `get
-00001ac0: 5f73 6f6c 6f60 0a74 656d 706c 6174 6520  _solo`.template 
-00001ad0: 7461 672e 0a0a 596f 7520 6361 6e20 6368  tag...You can ch
-00001ae0: 616e 6765 2074 6865 206e 616d 6520 6067  ange the name `g
-00001af0: 6574 5f73 6f6c 6f60 2075 7369 6e67 2074  et_solo` using t
-00001b00: 6865 0a60 4745 545f 534f 4c4f 5f54 454d  he.`GET_SOLO_TEM
-00001b10: 504c 4154 455f 5441 475f 4e41 4d45 6020  PLATE_TAG_NAME` 
-00001b20: 7365 7474 696e 672e 0a0a 6060 6070 7974  setting...```pyt
-00001b30: 686f 6e0a 4745 545f 534f 4c4f 5f54 454d  hon.GET_SOLO_TEM
-00001b40: 504c 4154 455f 5441 475f 4e41 4d45 203d  PLATE_TAG_NAME =
-00001b50: 2027 6765 745f 636f 6e66 6967 270a 6060   'get_config'.``
-00001b60: 600a 0a23 2323 2041 646d 696e 206f 7665  `..### Admin ove
-00001b70: 7272 6964 6520 666c 6167 0a0a 4279 2064  rride flag..By d
-00001b80: 6566 6175 6c74 2c20 7468 6520 6164 6d69  efault, the admi
-00001b90: 6e20 6973 206f 7665 7272 6964 6465 6e2e  n is overridden.
-00001ba0: 2042 7574 2069 6620 796f 7520 7769 7368   But if you wish
-00001bb0: 2074 6f20 6b65 6570 2074 6865 206f 626a   to keep the obj
-00001bc0: 6563 7420 6c69 7374 0a70 6167 6520 2865  ect list.page (e
-00001bd0: 2e67 2e20 746f 2063 7573 746f 6d69 7a65  .g. to customize
-00001be0: 2061 6374 696f 6e73 292c 2079 6f75 2063   actions), you c
-00001bf0: 616e 2073 6574 2074 6865 2060 534f 4c4f  an set the `SOLO
-00001c00: 5f41 444d 494e 5f53 4b49 505f 4f42 4a45  _ADMIN_SKIP_OBJE
-00001c10: 4354 5f4c 4953 545f 5041 4745 600a 746f  CT_LIST_PAGE`.to
-00001c20: 2060 4661 6c73 6560 2e0a 0a60 6060 7079   `False`...```py
-00001c30: 7468 6f6e 0a53 4f4c 4f5f 4144 4d49 4e5f  thon.SOLO_ADMIN_
-00001c40: 534b 4950 5f4f 424a 4543 545f 4c49 5354  SKIP_OBJECT_LIST
-00001c50: 5f50 4147 4520 3d20 5472 7565 0a60 6060  _PAGE = True.```
-00001c60: 0a0a 2323 2320 4361 6368 6520 6261 636b  ..### Cache back
-00001c70: 656e 640a 0a44 6a61 6e67 6f20 7072 6f76  end..Django prov
-00001c80: 6964 6573 2061 2077 6179 2074 6f20 6465  ides a way to de
-00001c90: 6669 6e65 206d 756c 7469 706c 6520 6361  fine multiple ca
-00001ca0: 6368 6520 6261 636b 656e 6473 2077 6974  che backends wit
-00001cb0: 6820 7468 6520 6043 4143 4845 5360 0a73  h the `CACHES`.s
-00001cc0: 6574 7469 6e67 732e 2049 6620 796f 7520  ettings. If you 
-00001cd0: 7761 6e74 2074 6865 2073 696e 676c 6574  want the singlet
-00001ce0: 6f6e 206f 626a 6563 7420 746f 2062 6520  on object to be 
-00001cf0: 6361 6368 6564 2073 6570 6172 6174 656c  cached separatel
-00001d00: 792c 2079 6f75 0a63 6f75 6c64 2064 6566  y, you.could def
-00001d10: 696e 6520 7468 6520 6043 4143 4845 5360  ine the `CACHES`
-00001d20: 2061 6e64 2074 6865 2060 534f 4c4f 5f43   and the `SOLO_C
-00001d30: 4143 4845 6020 7365 7474 696e 6773 206c  ACHE` settings l
-00001d40: 696b 6520 7468 6973 3a0a 0a60 6060 7079  ike this:..```py
-00001d50: 7468 6f6e 0a43 4143 4845 5320 3d20 7b0a  thon.CACHES = {.
-00001d60: 2020 2020 2764 6566 6175 6c74 273a 207b      'default': {
-00001d70: 0a20 2020 2020 2020 2027 4241 434b 454e  .        'BACKEN
-00001d80: 4427 3a20 2764 6a61 6e67 6f2e 636f 7265  D': 'django.core
-00001d90: 2e63 6163 6865 2e62 6163 6b65 6e64 732e  .cache.backends.
-00001da0: 6d65 6d63 6163 6865 642e 4d65 6d63 6163  memcached.Memcac
-00001db0: 6865 6443 6163 6865 272c 0a20 2020 2020  hedCache',.     
-00001dc0: 2020 2027 4c4f 4341 5449 4f4e 273a 2027     'LOCATION': '
-00001dd0: 3132 372e 302e 302e 313a 3131 3231 3127  127.0.0.1:11211'
-00001de0: 2c0a 2020 2020 7d2c 0a20 2020 2027 6c6f  ,.    },.    'lo
-00001df0: 6361 6c27 3a20 7b0a 2020 2020 2020 2020  cal': {.        
-00001e00: 2742 4143 4b45 4e44 273a 2027 646a 616e  'BACKEND': 'djan
-00001e10: 676f 2e63 6f72 652e 6361 6368 652e 6261  go.core.cache.ba
-00001e20: 636b 656e 6473 2e6c 6f63 6d65 6d2e 4c6f  ckends.locmem.Lo
-00001e30: 634d 656d 4361 6368 6527 2c0a 2020 2020  cMemCache',.    
-00001e40: 7d2c 0a7d 0a0a 534f 4c4f 5f43 4143 4845  },.}..SOLO_CACHE
-00001e50: 203d 2027 6c6f 6361 6c27 0a60 6060 0a0a   = 'local'.```..
-00001e60: 4361 6368 696e 6720 7769 6c6c 2062 6520  Caching will be 
-00001e70: 6469 7361 626c 6564 2069 6620 7365 7420  disabled if set 
-00001e80: 746f 2060 4e6f 6e65 602e 0a0a 0a23 2323  to `None`....###
-00001e90: 2043 6163 6865 2074 696d 656f 7574 0a0a   Cache timeout..
-00001ea0: 5468 6520 6361 6368 6520 7469 6d65 6f75  The cache timeou
-00001eb0: 7420 696e 2073 6563 6f6e 6473 2e0a 0a60  t in seconds...`
-00001ec0: 6060 7079 7468 6f6e 0a53 4f4c 4f5f 4341  ``python.SOLO_CA
-00001ed0: 4348 455f 5449 4d45 4f55 5420 3d20 3630  CHE_TIMEOUT = 60
-00001ee0: 2a35 2020 2320 3520 6d69 6e73 0a60 6060  *5  # 5 mins.```
-00001ef0: 0a0a 2323 2320 4361 6368 6520 7072 6566  ..### Cache pref
-00001f00: 6978 0a0a 5468 6520 7072 6566 6978 2074  ix..The prefix t
-00001f10: 6f20 7573 6520 666f 7220 7468 6520 6361  o use for the ca
-00001f20: 6368 6520 6b65 792e 0a0a 6060 6070 7974  che key...```pyt
-00001f30: 686f 6e0a 534f 4c4f 5f43 4143 4845 5f50  hon.SOLO_CACHE_P
-00001f40: 5245 4649 5820 3d20 2773 6f6c 6f27 0a60  REFIX = 'solo'.`
-00001f50: 6060 0a0a 4765 7474 696e 6720 7468 6520  ``..Getting the 
-00001f60: 636f 6465 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d  code.===========
-00001f70: 3d3d 3d3d 3d0a 0a54 6865 2063 6f64 6520  =====..The code 
-00001f80: 6973 2068 6f73 7465 6420 6174 2068 7474  is hosted at htt
-00001f90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001fa0: 6c61 7a79 6269 7264 2f64 6a61 6e67 6f2d  lazybird/django-
-00001fb0: 736f 6c6f 2f0a 0a43 6865 636b 206f 7574  solo/..Check out
-00001fc0: 2074 6865 206c 6174 6573 7420 6465 7665   the latest deve
-00001fd0: 6c6f 706d 656e 7420 7665 7273 696f 6e20  lopment version 
-00001fe0: 616e 6f6e 796d 6f75 736c 7920 7769 7468  anonymously with
-00001ff0: 3a0a 0a20 2020 2024 2067 6974 2063 6c6f  :..    $ git clo
-00002000: 6e65 2067 6974 3a2f 2f67 6974 6875 622e  ne git://github.
-00002010: 636f 6d2f 6c61 7a79 6269 7264 2f64 6a61  com/lazybird/dja
-00002020: 6e67 6f2d 736f 6c6f 2e67 6974 0a0a 596f  ngo-solo.git..Yo
-00002030: 7520 6361 6e20 696e 7374 616c 6c20 7468  u can install th
-00002040: 6520 7061 636b 6167 6520 696e 2074 6865  e package in the
-00002050: 2022 6564 6974 6162 6c65 2220 6d6f 6465   "editable" mode
-00002060: 206c 696b 6520 7468 6973 3a0a 0a20 2020   like this:..   
-00002070: 2070 6970 2075 6e69 6e73 7461 6c6c 2064   pip uninstall d
-00002080: 6a61 6e67 6f2d 736f 6c6f 2020 2320 6a75  jango-solo  # ju
-00002090: 7374 2069 6e20 6361 7365 2e2e 2e0a 2020  st in case....  
-000020a0: 2020 7069 7020 696e 7374 616c 6c20 2d65    pip install -e
-000020b0: 2067 6974 2b68 7474 7073 3a2f 2f67 6974   git+https://git
-000020c0: 6875 622e 636f 6d2f 6c61 7a79 6269 7264  hub.com/lazybird
-000020d0: 2f64 6a61 6e67 6f2d 736f 6c6f 2e67 6974  /django-solo.git
-000020e0: 2365 6767 3d64 6a61 6e67 6f2d 736f 6c6f  #egg=django-solo
-000020f0: 0a0a 596f 7520 6361 6e20 616c 736f 2069  ..You can also i
-00002100: 6e73 7461 6c6c 2061 2073 7065 6369 6669  nstall a specifi
-00002110: 6320 6272 616e 6368 3a0a 0a20 2020 2070  c branch:..    p
-00002120: 6970 2069 6e73 7461 6c6c 202d 6520 6769  ip install -e gi
-00002130: 742b 6874 7470 733a 2f2f 6769 7468 7562  t+https://github
-00002140: 2e63 6f6d 2f6c 617a 7962 6972 642f 646a  .com/lazybird/dj
-00002150: 616e 676f 2d73 6f6c 6f2e 6769 7440 6d79  ango-solo.git@my
-00002160: 2d62 7261 6e63 6823 6567 673d 646a 616e  -branch#egg=djan
-00002170: 676f 2d73 6f6c 6f0a 0a54 6865 2070 6163  go-solo..The pac
-00002180: 6b61 6765 2069 7320 6e6f 7720 696e 7374  kage is now inst
-00002190: 616c 6c65 6420 696e 2079 6f75 7220 7072  alled in your pr
-000021a0: 6f6a 6563 7420 616e 6420 796f 7520 6361  oject and you ca
-000021b0: 6e20 6669 6e64 2074 6865 2063 6f64 652e  n find the code.
-000021c0: 0a0a 546f 2072 756e 2074 6865 2075 6e69  ..To run the uni
-000021d0: 7420 7465 7374 733a 0a0a 2020 2020 7069  t tests:..    pi
-000021e0: 7020 696e 7374 616c 6c20 746f 780a 2020  p install tox.  
-000021f0: 2020 746f 780a 0a0a                        tox...
+00000010: 3a20 322e 310d 0a4e 616d 653a 2064 6a61  : 2.1..Name: dja
+00000020: 6e67 6f2d 736f 6c6f 0d0a 5665 7273 696f  ngo-solo..Versio
+00000030: 6e3a 2032 2e31 2e30 0d0a 5375 6d6d 6172  n: 2.1.0..Summar
+00000040: 793a 2044 6a61 6e67 6f20 536f 6c6f 2068  y: Django Solo h
+00000050: 656c 7073 2077 6f72 6b69 6e67 2077 6974  elps working wit
+00000060: 6820 7369 6e67 6c65 746f 6e73 0d0a 486f  h singletons..Ho
+00000070: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
+00000080: 2f67 6974 6875 622e 636f 6d2f 6c61 7a79  /github.com/lazy
+00000090: 6269 7264 2f64 6a61 6e67 6f2d 736f 6c6f  bird/django-solo
+000000a0: 2f0d 0a41 7574 686f 723a 206c 617a 7962  /..Author: lazyb
+000000b0: 6972 640d 0a4c 6963 656e 7365 3a20 4372  ird..License: Cr
+000000c0: 6561 7469 7665 2043 6f6d 6d6f 6e73 2041  eative Commons A
+000000d0: 7474 7269 6275 7469 6f6e 2033 2e30 2055  ttribution 3.0 U
+000000e0: 6e70 6f72 7465 640d 0a43 6c61 7373 6966  nported..Classif
+000000f0: 6965 723a 2046 7261 6d65 776f 726b 203a  ier: Framework :
+00000100: 3a20 446a 616e 676f 203a 3a20 332e 320d  : Django :: 3.2.
+00000110: 0a43 6c61 7373 6966 6965 723a 2046 7261  .Classifier: Fra
+00000120: 6d65 776f 726b 203a 3a20 446a 616e 676f  mework :: Django
+00000130: 203a 3a20 342e 300d 0a43 6c61 7373 6966   :: 4.0..Classif
+00000140: 6965 723a 2046 7261 6d65 776f 726b 203a  ier: Framework :
+00000150: 3a20 446a 616e 676f 203a 3a20 342e 310d  : Django :: 4.1.
+00000160: 0a43 6c61 7373 6966 6965 723a 2046 7261  .Classifier: Fra
+00000170: 6d65 776f 726b 203a 3a20 446a 616e 676f  mework :: Django
+00000180: 203a 3a20 342e 320d 0a43 6c61 7373 6966   :: 4.2..Classif
+00000190: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
+000001a0: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
+000001b0: 7065 7273 0d0a 436c 6173 7369 6669 6572  pers..Classifier
+000001c0: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
+000001d0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+000001e0: 6465 6e74 0d0a 436c 6173 7369 6669 6572  dent..Classifier
+000001f0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000200: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000210: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
+00000220: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000230: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000240: 330d 0a43 6c61 7373 6966 6965 723a 2050  3..Classifier: P
+00000250: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000260: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000270: 2033 2e37 0d0a 436c 6173 7369 6669 6572   3.7..Classifier
+00000280: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000290: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000002a0: 203a 3a20 332e 380d 0a43 6c61 7373 6966   :: 3.8..Classif
+000002b0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000002c0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000002d0: 686f 6e20 3a3a 2033 2e39 0d0a 436c 6173  hon :: 3.9..Clas
+000002e0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000002f0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000300: 5079 7468 6f6e 203a 3a20 332e 3130 0d0a  Python :: 3.10..
+00000310: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000320: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000330: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000340: 3131 0d0a 5265 7175 6972 6573 2d50 7974  11..Requires-Pyt
+00000350: 686f 6e3a 203e 3d33 2e37 0d0a 4465 7363  hon: >=3.7..Desc
+00000360: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+00000370: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+00000380: 6f77 6e0d 0a4c 6963 656e 7365 2d46 696c  own..License-Fil
+00000390: 653a 204c 4943 454e 5345 0d0a 0d0a 0d0a  e: LICENSE......
+000003a0: 446a 616e 676f 2053 6f6c 6f0d 0a3d 3d3d  Django Solo..===
+000003b0: 3d3d 3d3d 3d3d 3d3d 0d0a 0d0a 3c61 2068  ========....<a h
+000003c0: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+000003d0: 692e 6f72 672f 7072 6f6a 6563 742f 646a  i.org/project/dj
+000003e0: 616e 676f 2d73 6f6c 6f2f 2220 616c 743d  ango-solo/" alt=
+000003f0: 2243 7572 7265 6e74 2076 6572 7369 6f6e  "Current version
+00000400: 206f 6e20 5079 5069 223e 3c69 6d67 2073   on PyPi"><img s
+00000410: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000420: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000430: 762f 646a 616e 676f 2d73 6f6c 6f2e 7376  v/django-solo.sv
+00000440: 6722 202f 3e3c 2f61 3e0d 0a0d 0a0d 0a20  g" /></a>...... 
+00000450: 2020 202b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     +------------
+00000460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00000470: 0d0a 2020 2020 7c20 2020 2020 2020 2020  ..    |         
+00000480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000490: 2020 7c0d 0a20 2020 207c 2020 2020 2020    |..    |      
+000004a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004b0: 2020 2020 207c 0d0a 2020 2020 7c20 2020       |..    |   
+000004c0: 2020 2020 2020 2020 2020 5c20 2020 2020            \     
+000004d0: 2020 2020 2020 2020 7c20 446a 616e 676f          | Django
+000004e0: 2053 6f6c 6f20 6865 6c70 7320 776f 726b   Solo helps work
+000004f0: 696e 6720 7769 7468 2073 696e 676c 6574  ing with singlet
+00000500: 6f6e 733a 0d0a 2020 2020 7c20 2020 2020  ons:..    |     
+00000510: 2020 2020 2020 2020 2f5c 2020 2020 2020          /\      
+00000520: 2020 2020 2020 7c20 6461 7461 6261 7365        | database
+00000530: 2074 6162 6c65 7320 7468 6174 206f 6e6c   tables that onl
+00000540: 7920 6861 7665 206f 6e65 2072 6f77 2e0d  y have one row..
+00000550: 0a20 2020 207c 2020 2020 2020 2020 2020  .    |          
+00000560: 203e 3d29 273e 2020 2020 2020 2020 2020   >=)'>          
+00000570: 207c 2053 696e 676c 6574 6f6e 7320 6172   | Singletons ar
+00000580: 6520 7573 6566 756c 2066 6f72 2074 6869  e useful for thi
+00000590: 6e67 7320 6c69 6b65 2067 6c6f 6261 6c0d  ngs like global.
+000005a0: 0a20 2020 207c 2020 2020 2020 2020 2020  .    |          
+000005b0: 2020 205c 2f20 2020 2020 2020 2020 2020     \/           
+000005c0: 207c 2073 6574 7469 6e67 7320 7468 6174   | settings that
+000005d0: 2079 6f75 2077 616e 7420 746f 2065 6469   you want to edi
+000005e0: 7420 6672 6f6d 2074 6865 2061 646d 696e  t from the admin
+000005f0: 0d0a 2020 2020 7c20 2020 2020 2020 2020  ..    |         
+00000600: 2020 2020 2f20 2020 2020 2020 2020 2020      /           
+00000610: 2020 7c20 696e 7374 6561 6420 6f66 2068    | instead of h
+00000620: 6176 696e 6720 7468 656d 2069 6e20 446a  aving them in Dj
+00000630: 616e 676f 2073 6574 7469 6e67 732e 7079  ango settings.py
+00000640: 2e0d 0a20 2020 207c 2020 2020 2020 2020  ...    |        
+00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000660: 2020 207c 200d 0a20 2020 207c 2020 2020     | ..    |    
+00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000680: 2020 2020 2020 207c 200d 0a20 2020 202b         | ..    +
+00000690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000006a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0d0a 0d0a  -----------+....
+000006b0: 0d0a 4665 6174 7572 6573 0d0a 2d2d 2d2d  ..Features..----
+000006c0: 2d2d 2d2d 0d0a 0d0a 536f 6c6f 2068 656c  ----....Solo hel
+000006d0: 7073 2079 6f75 2065 6e66 6f72 6365 2069  ps you enforce i
+000006e0: 6e73 7461 6e74 6961 7469 6e67 206f 6e6c  nstantiating onl
+000006f0: 7920 6f6e 6520 696e 7374 616e 6365 206f  y one instance o
+00000700: 6620 6120 6d6f 6465 6c20 696e 2064 6a61  f a model in dja
+00000710: 6e67 6f2e 0d0a 0d0a 2a20 596f 7520 6465  ngo.....* You de
+00000720: 6669 6e65 2074 6865 206d 6f64 656c 2074  fine the model t
+00000730: 6861 7420 7769 6c6c 2068 6f6c 6420 796f  hat will hold yo
+00000740: 7572 2073 696e 676c 6574 6f6e 206f 626a  ur singleton obj
+00000750: 6563 742e 0d0a 2a20 646a 616e 676f 2d73  ect...* django-s
+00000760: 6f6c 6f20 6769 7665 7320 6865 6c70 6572  olo gives helper
+00000770: 2070 6172 656e 7420 636c 6173 7320 666f   parent class fo
+00000780: 7220 796f 7572 206d 6f64 656c 2061 6e64  r your model and
+00000790: 2074 6865 2061 646d 696e 2063 6c61 7373   the admin class
+000007a0: 6573 2e0d 0a2a 2059 6f75 2067 6574 2061  es...* You get a
+000007b0: 6e20 6164 6d69 6e20 696e 7465 7266 6163  n admin interfac
+000007c0: 6520 7468 6174 2773 2061 7761 7265 2079  e that's aware y
+000007d0: 6f75 206f 6e6c 7920 6861 7665 206f 6e65  ou only have one
+000007e0: 206f 626a 6563 742e 0d0a 2a20 596f 7520   object...* You 
+000007f0: 6361 6e20 7265 7472 6965 7665 2074 6865  can retrieve the
+00000800: 206f 626a 6563 7420 6672 6f6d 2074 656d   object from tem
+00000810: 706c 6174 6573 2e0d 0a2a 2042 7920 656e  plates...* By en
+00000820: 6162 6c69 6e67 2063 6163 6869 6e67 2c20  abling caching, 
+00000830: 7468 6520 6461 7461 6261 7365 2069 7320  the database is 
+00000840: 6e6f 7420 7175 6572 6965 6420 696e 7465  not queried inte
+00000850: 6e73 6976 656c 792e 0d0a 0d0a 5573 6520  nsively.....Use 
+00000860: 4361 7365 730d 0a2d 2d2d 2d2d 2d2d 2d0d  Cases..--------.
+00000870: 0a0d 0a44 6a61 6e67 6f20 536f 6c6f 2069  ...Django Solo i
+00000880: 7320 616c 736f 2067 7265 6174 2066 6f72  s also great for
+00000890: 2075 7365 2077 6974 6820 7369 6e67 6c65   use with single
+000008a0: 746f 6e20 6f62 6a65 6374 7320 7468 6174  ton objects that
+000008b0: 2068 6176 6520 6120 6f6e 6520 746f 206d   have a one to m
+000008c0: 616e 7920 7265 6c61 7469 6f6e 7368 6970  any relationship
+000008d0: 2e20 4c69 6b65 2074 6865 2075 7365 2063  . Like the use c
+000008e0: 6173 6520 6265 6c6f 7720 7768 6572 6520  ase below where 
+000008f0: 796f 7520 6861 7665 2061 2027 486f 6d65  you have a 'Home
+00000900: 2053 6c69 6465 7222 2074 6861 7420 6861   Slider" that ha
+00000910: 7320 6d61 6e79 2022 536c 6964 6573 222e  s many "Slides".
+00000920: 0d0a 0d0a 2a20 476c 6f62 616c 206f 7220  ....* Global or 
+00000930: 6465 6661 756c 7420 7365 7474 696e 6773  default settings
+00000940: 0d0a 2a20 416e 2069 6d61 6765 2073 6c69  ..* An image sli
+00000950: 6465 7220 7468 6174 2068 6173 206d 616e  der that has man
+00000960: 7920 736c 6964 6573 0d0a 2a20 4120 7061  y slides..* A pa
+00000970: 6765 2073 6563 7469 6f6e 2074 6861 7420  ge section that 
+00000980: 6861 7320 7375 622d 7365 6374 696f 6e73  has sub-sections
+00000990: 0d0a 2a20 4120 7465 616d 2062 696f 2077  ..* A team bio w
+000009a0: 6974 6820 6d61 6e79 2074 6561 6d20 6d65  ith many team me
+000009b0: 6d62 6572 730d 0a0d 0a54 6865 7265 2061  mbers....There a
+000009c0: 7265 206d 616e 7920 6361 7365 7320 7768  re many cases wh
+000009d0: 6572 6520 6974 206d 616b 6573 2073 656e  ere it makes sen
+000009e0: 7365 2066 6f72 2074 6865 2070 6172 656e  se for the paren
+000009f0: 7420 696e 2061 206f 6e65 2074 6f20 6d61  t in a one to ma
+00000a00: 6e79 2072 656c 6174 696f 6e73 6869 7020  ny relationship 
+00000a10: 746f 2062 6520 6c69 6d69 7465 6420 746f  to be limited to
+00000a20: 2061 2073 696e 676c 6520 696e 7374 616e   a single instan
+00000a30: 6365 2e0d 0a0d 0a55 7361 6765 2045 7861  ce.....Usage Exa
+00000a40: 6d70 6c65 0d0a 0d0a 6060 6070 7974 686f  mple....```pytho
+00000a50: 6e0d 0a23 206d 6f64 656c 732e 7079 0d0a  n..# models.py..
+00000a60: 0d0a 6672 6f6d 2064 6a61 6e67 6f2e 6462  ..from django.db
+00000a70: 2069 6d70 6f72 7420 6d6f 6465 6c73 0d0a   import models..
+00000a80: 6672 6f6d 2073 6f6c 6f2e 6d6f 6465 6c73  from solo.models
+00000a90: 2069 6d70 6f72 7420 5369 6e67 6c65 746f   import Singleto
+00000aa0: 6e4d 6f64 656c 0d0a 0d0a 0d0a 636c 6173  nModel......clas
+00000ab0: 7320 5369 7465 436f 6e66 6967 7572 6174  s SiteConfigurat
+00000ac0: 696f 6e28 5369 6e67 6c65 746f 6e4d 6f64  ion(SingletonMod
+00000ad0: 656c 293a 0d0a 2020 2020 7369 7465 5f6e  el):..    site_n
+00000ae0: 616d 6520 3d20 6d6f 6465 6c73 2e43 6861  ame = models.Cha
+00000af0: 7246 6965 6c64 286d 6178 5f6c 656e 6774  rField(max_lengt
+00000b00: 683d 3235 352c 2064 6566 6175 6c74 3d27  h=255, default='
+00000b10: 5369 7465 204e 616d 6527 290d 0a20 2020  Site Name')..   
+00000b20: 206d 6169 6e74 656e 616e 6365 5f6d 6f64   maintenance_mod
+00000b30: 6520 3d20 6d6f 6465 6c73 2e42 6f6f 6c65  e = models.Boole
+00000b40: 616e 4669 656c 6428 6465 6661 756c 743d  anField(default=
+00000b50: 4661 6c73 6529 0d0a 0d0a 2020 2020 6465  False)....    de
+00000b60: 6620 5f5f 7374 725f 5f28 7365 6c66 293a  f __str__(self):
+00000b70: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000b80: 2022 5369 7465 2043 6f6e 6669 6775 7261   "Site Configura
+00000b90: 7469 6f6e 220d 0a0d 0a20 2020 2063 6c61  tion"....    cla
+00000ba0: 7373 204d 6574 613a 0d0a 2020 2020 2020  ss Meta:..      
+00000bb0: 2020 7665 7262 6f73 655f 6e61 6d65 203d    verbose_name =
+00000bc0: 2022 5369 7465 2043 6f6e 6669 6775 7261   "Site Configura
+00000bd0: 7469 6f6e 220d 0a60 6060 0d0a 0d0a 6060  tion"..```....``
+00000be0: 6070 7974 686f 6e0d 0a23 2061 646d 696e  `python..# admin
+00000bf0: 2e70 790d 0a0d 0a66 726f 6d20 646a 616e  .py....from djan
+00000c00: 676f 2e63 6f6e 7472 6962 2069 6d70 6f72  go.contrib impor
+00000c10: 7420 6164 6d69 6e0d 0a66 726f 6d20 736f  t admin..from so
+00000c20: 6c6f 2e61 646d 696e 2069 6d70 6f72 7420  lo.admin import 
+00000c30: 5369 6e67 6c65 746f 6e4d 6f64 656c 4164  SingletonModelAd
+00000c40: 6d69 6e0d 0a66 726f 6d20 636f 6e66 6967  min..from config
+00000c50: 2e6d 6f64 656c 7320 696d 706f 7274 2053  .models import S
+00000c60: 6974 6543 6f6e 6669 6775 7261 7469 6f6e  iteConfiguration
+00000c70: 0d0a 0d0a 0d0a 6164 6d69 6e2e 7369 7465  ......admin.site
+00000c80: 2e72 6567 6973 7465 7228 5369 7465 436f  .register(SiteCo
+00000c90: 6e66 6967 7572 6174 696f 6e2c 2053 696e  nfiguration, Sin
+00000ca0: 676c 6574 6f6e 4d6f 6465 6c41 646d 696e  gletonModelAdmin
+00000cb0: 290d 0a60 6060 0d0a 0d0a 6060 6070 7974  )..```....```pyt
+00000cc0: 686f 6e0d 0a23 2054 6865 7265 2069 7320  hon..# There is 
+00000cd0: 6f6e 6c79 206f 6e65 2069 7465 6d20 696e  only one item in
+00000ce0: 2074 6865 2074 6162 6c65 2c20 796f 7520   the table, you 
+00000cf0: 6361 6e20 6765 7420 6974 2074 6869 7320  can get it this 
+00000d00: 7761 793a 0d0a 6672 6f6d 202e 6d6f 6465  way:..from .mode
+00000d10: 6c73 2069 6d70 6f72 7420 5369 7465 436f  ls import SiteCo
+00000d20: 6e66 6967 7572 6174 696f 6e0d 0a63 6f6e  nfiguration..con
+00000d30: 6669 6720 3d20 5369 7465 436f 6e66 6967  fig = SiteConfig
+00000d40: 7572 6174 696f 6e2e 6f62 6a65 6374 732e  uration.objects.
+00000d50: 6765 7428 290d 0a0d 0a23 2067 6574 5f73  get()....# get_s
+00000d60: 6f6c 6f20 7769 6c6c 2063 7265 6174 6520  olo will create 
+00000d70: 7468 6520 6974 656d 2069 6620 6974 2064  the item if it d
+00000d80: 6f65 7320 6e6f 7420 616c 7265 6164 7920  oes not already 
+00000d90: 6578 6973 740d 0a63 6f6e 6669 6720 3d20  exist..config = 
+00000da0: 5369 7465 436f 6e66 6967 7572 6174 696f  SiteConfiguratio
+00000db0: 6e2e 6765 745f 736f 6c6f 2829 0d0a 6060  n.get_solo()..``
+00000dc0: 600d 0a0d 0a49 6e20 796f 7572 206d 6f64  `....In your mod
+00000dd0: 656c 2c20 6e6f 7465 2068 6f77 2079 6f75  el, note how you
+00000de0: 2064 6964 206e 6f74 2068 6176 6520 746f   did not have to
+00000df0: 2070 726f 7669 6465 2061 2060 7665 7262   provide a `verb
+00000e00: 6f73 655f 6e61 6d65 5f70 6c75 7261 6c60  ose_name_plural`
+00000e10: 2066 6965 6c64 202d 0d0a 5468 6174 2773   field -..That's
+00000e20: 2062 6563 6175 7365 2044 6a61 6e67 6f20   because Django 
+00000e30: 536f 6c6f 2075 7365 7320 7468 6520 6076  Solo uses the `v
+00000e40: 6572 626f 7365 5f6e 616d 6560 2069 6e73  erbose_name` ins
+00000e50: 7465 6164 2e0d 0a0d 0a49 6620 796f 7527  tead.....If you'
+00000e60: 7265 2063 6861 6e67 696e 6720 616e 2065  re changing an e
+00000e70: 7869 7374 696e 6720 6d6f 6465 6c20 2877  xisting model (w
+00000e80: 6869 6368 2061 6c72 6561 6479 2068 6173  hich already has
+00000e90: 2073 6f6d 6520 6f62 6a65 6374 7320 7374   some objects st
+00000ea0: 6f72 6564 2069 6e20 7468 6520 6461 7461  ored in the data
+00000eb0: 6261 7365 2920 746f 2061 2073 696e 676c  base) to a singl
+00000ec0: 6574 6f6e 206d 6f64 656c 2c20 796f 7520  eton model, you 
+00000ed0: 6361 6e20 6578 706c 6963 6974 6c79 2070  can explicitly p
+00000ee0: 726f 7669 6465 2074 6865 2069 6420 6f66  rovide the id of
+00000ef0: 2074 6865 2072 6f77 2069 6e20 7468 6520   the row in the 
+00000f00: 6461 7461 6261 7365 2066 6f72 2064 6a61  database for dja
+00000f10: 6e67 6f2d 736f 6c6f 2074 6f20 7573 652e  ngo-solo to use.
+00000f20: 2054 6869 7320 6361 6e20 6265 2064 6f6e   This can be don
+00000f30: 6520 6279 2073 6574 7469 6e67 2060 7369  e by setting `si
+00000f40: 6e67 6c65 746f 6e5f 696e 7374 616e 6365  ngleton_instance
+00000f50: 5f69 6460 2070 726f 7065 7274 7920 6f6e  _id` property on
+00000f60: 2074 6865 206d 6f64 656c 3a0d 0a0d 0a60   the model:....`
+00000f70: 6060 7079 7468 6f6e 0d0a 636c 6173 7320  ``python..class 
+00000f80: 5369 7465 436f 6e66 6967 7572 6174 696f  SiteConfiguratio
+00000f90: 6e28 5369 6e67 6c65 746f 6e4d 6f64 656c  n(SingletonModel
+00000fa0: 293a 0d0a 2020 2020 7369 6e67 6c65 746f  ):..    singleto
+00000fb0: 6e5f 696e 7374 616e 6365 5f69 6420 3d20  n_instance_id = 
+00000fc0: 3234 0d0a 2020 2020 2320 282e 2e2e 290d  24..    # (...).
+00000fd0: 0a60 6060 0d0a 0d0a 496e 7374 616c 6c61  .```....Installa
+00000fe0: 7469 6f6e 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d  tion..----------
+00000ff0: 2d2d 0d0a 0d0a 5468 6973 2061 7070 6c69  --....This appli
+00001000: 6361 7469 6f6e 2072 6571 7569 7265 7320  cation requires 
+00001010: 446a 616e 676f 2033 2e32 2c20 342e 302c  Django 3.2, 4.0,
+00001020: 206f 7220 342e 312e 0d0a 0d0a 2a20 496e   or 4.1.....* In
+00001030: 7374 616c 6c20 7468 6520 7061 636b 6167  stall the packag
+00001040: 6520 7573 696e 6720 6070 6970 2069 6e73  e using `pip ins
+00001050: 7461 6c6c 2064 6a61 6e67 6f2d 736f 6c6f  tall django-solo
+00001060: 600d 0a2a 2041 6464 2060 6073 6f6c 6f60  `..* Add ``solo`
+00001070: 6020 6f72 2060 6073 6f6c 6f2e 6170 7073  ` or ``solo.apps
+00001080: 2e53 6f6c 6f41 7070 436f 6e66 6967 6060  .SoloAppConfig``
+00001090: 2074 6f20 796f 7572 2060 6049 4e53 5441   to your ``INSTA
+000010a0: 4c4c 4544 5f41 5050 5360 6020 7365 7474  LLED_APPS`` sett
+000010b0: 696e 672e 0d0a 0d0a 5468 6973 2069 7320  ing.....This is 
+000010c0: 686f 7720 796f 7520 7275 6e20 7465 7374  how you run test
+000010d0: 733a 0d0a 0d0a 2020 2020 2e2f 6d61 6e61  s:....    ./mana
+000010e0: 6765 2e70 7920 7465 7374 2073 6f6c 6f20  ge.py test solo 
+000010f0: 2d2d 7365 7474 696e 6773 3d73 6f6c 6f2e  --settings=solo.
+00001100: 7465 7374 732e 7365 7474 696e 6773 0d0a  tests.settings..
+00001110: 0d0a 416e 6420 6672 6f6d 2077 6974 6869  ..And from withi
+00001120: 6e20 6074 6f78 603a 0d0a 0d0a 6060 600d  n `tox`:....```.
+00001130: 0a70 7974 686f 6e20 2d6d 2070 6970 2069  .python -m pip i
+00001140: 6e73 7461 6c6c 2074 6f78 0d0a 746f 780d  nstall tox..tox.
+00001150: 0a60 6060 0d0a 0d0a 5375 7070 6f72 7465  .```....Supporte
+00001160: 6420 4c61 6e67 7561 6765 730d 0a2d 2d2d  d Languages..---
+00001170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001180: 0d0a 0d0a 2d20 456e 676c 6973 680d 0a2d  ....- English..-
+00001190: 2053 7061 6e69 7368 0d0a 2d20 4765 726d   Spanish..- Germ
+000011a0: 616e 0d0a 0d0a 4164 6d69 6e0d 0a2d 2d2d  an....Admin..---
+000011b0: 2d2d 0d0a 0d0a 5468 6520 7374 616e 6461  --....The standa
+000011c0: 7264 2044 6a61 6e67 6f20 6164 6d69 6e20  rd Django admin 
+000011d0: 646f 6573 206e 6f74 2066 6974 2077 656c  does not fit wel
+000011e0: 6c20 7768 656e 2077 6f72 6b69 6e67 2077  l when working w
+000011f0: 6974 6820 7369 6e67 6c65 746f 6e2c 0d0a  ith singleton,..
+00001200: 666f 7220 696e 7374 616e 6365 2c20 6966  for instance, if
+00001210: 2079 6f75 206e 6565 6420 736f 6d65 2067   you need some g
+00001220: 6c6f 6261 6c20 7369 7465 2073 6574 7469  lobal site setti
+00001230: 6e67 7320 746f 2062 6520 6564 6974 6564  ngs to be edited
+00001240: 2069 6e20 7468 6520 6164 6d69 6e2e 0d0a   in the admin...
+00001250: 446a 616e 676f 2053 6f6c 6f20 7072 6f76  Django Solo prov
+00001260: 6964 6573 2061 206d 6f64 6966 6965 6420  ides a modified 
+00001270: 6164 6d69 6e20 666f 7220 7468 6174 2e0d  admin for that..
+00001280: 0a0d 0a0d 0a21 5b64 6a61 6e67 6f2d 736f  .....![django-so
+00001290: 6c6f 2061 646d 696e 5d28 6874 7470 733a  lo admin](https:
+000012a0: 2f2f 7261 772e 6769 7468 7562 2e63 6f6d  //raw.github.com
+000012b0: 2f6c 617a 7962 6972 642f 646a 616e 676f  /lazybird/django
+000012c0: 2d73 6f6c 6f2f 6d61 7374 6572 2f64 6f63  -solo/master/doc
+000012d0: 732f 696d 6167 6573 2f64 6a61 6e67 6f2d  s/images/django-
+000012e0: 736f 6c6f 2d61 646d 696e 2e6a 7067 2022  solo-admin.jpg "
+000012f0: 646a 616e 676f 2d73 6f6c 6f20 6164 6d69  django-solo admi
+00001300: 6e22 290d 0a0d 0a0d 0a2a 2049 6e20 7468  n")......* In th
+00001310: 6520 6164 6d69 6e20 686f 6d65 2070 6167  e admin home pag
+00001320: 6520 7768 6572 6520 616c 6c20 6170 706c  e where all appl
+00001330: 6963 6174 696f 6e73 2061 7265 206c 6973  ications are lis
+00001340: 7465 642c 2077 6520 6861 7665 2061 2060  ted, we have a `
+00001350: 636f 6e66 6967 600d 0a20 2061 7070 6c69  config`..  appli
+00001360: 6361 7469 6f6e 2074 6861 7420 686f 6c64  cation that hold
+00001370: 7320 6120 7369 6e67 6c65 746f 6e20 6d6f  s a singleton mo
+00001380: 6465 6c20 666f 7220 7369 7465 2063 6f6e  del for site con
+00001390: 6669 6775 7261 7469 6f6e 2e0d 0a2a 2054  figuration...* T
+000013a0: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
+000013b0: 206f 626a 6563 7420 6361 6e20 6f6e 6c79   object can only
+000013c0: 2062 6520 6368 616e 6765 642c 2074 6865   be changed, the
+000013d0: 7265 2773 206e 6f20 6c69 6e6b 2066 6f72  re's no link for
+000013e0: 2022 6164 6422 2028 3129 2e0d 0a2a 2054   "add" (1)...* T
+000013f0: 6865 206c 696e 6b20 746f 2074 6865 2063  he link to the c
+00001400: 6f6e 6669 6775 7261 7469 6f6e 2070 6167  onfiguration pag
+00001410: 6520 2832 2920 6469 7265 6374 6c79 2067  e (2) directly g
+00001420: 6f65 7320 746f 2074 6865 2066 6f72 6d20  oes to the form 
+00001430: 7061 6765 202d 206e 6f0d 0a20 206e 6565  page - no..  nee
+00001440: 6420 666f 7220 616e 2069 6e74 6572 6d65  d for an interme
+00001450: 6469 6172 7920 6f62 6a65 6374 206c 6973  diary object lis
+00001460: 7420 7061 6765 2c20 7369 6e63 6520 7468  t page, since th
+00001470: 6572 6527 7320 6f6e 6c79 206f 6e65 206f  ere's only one o
+00001480: 626a 6563 742e 0d0a 2a20 5468 6520 6564  bject...* The ed
+00001490: 6974 2070 6167 6520 6861 7320 6120 6d6f  it page has a mo
+000014a0: 6469 6669 6564 2062 7265 6164 6372 756d  dified breadcrum
+000014b0: 6220 2833 2920 746f 2061 766f 6964 206c  b (3) to avoid l
+000014c0: 696e 6b69 6e67 2074 6f20 7468 650d 0a20  inking to the.. 
+000014d0: 2069 6e74 6572 6d65 6469 6172 7920 6f62   intermediary ob
+000014e0: 6a65 6374 206c 6973 7420 7061 6765 2e0d  ject list page..
+000014f0: 0a2a 2046 726f 6d20 7468 6520 6564 6974  .* From the edit
+00001500: 2070 6167 652c 2077 6520 6361 6e6e 6f74   page, we cannot
+00001510: 2064 656c 6574 6520 7468 6520 6f62 6a65   delete the obje
+00001520: 6374 2028 3429 206e 6f72 2063 616e 2077  ct (4) nor can w
+00001530: 6520 6164 6420 6120 6e65 7720 6f6e 6520  e add a new one 
+00001540: 2835 292e 0d0a 0d0a 4966 2079 6f75 2077  (5).....If you w
+00001550: 6973 6820 746f 2064 6973 6162 6c65 2074  ish to disable t
+00001560: 6865 2073 6b69 7070 696e 6720 6f66 2074  he skipping of t
+00001570: 6865 206f 626a 6563 7420 6c69 7374 2070  he object list p
+00001580: 6167 652c 2061 6e64 2068 6176 6520 7468  age, and have th
+00001590: 6520 6465 6661 756c 740d 0a62 7265 6164  e default..bread
+000015a0: 6372 756d 6273 2c20 796f 7520 7368 6f75  crumbs, you shou
+000015b0: 6c64 2073 6574 2060 534f 4c4f 5f41 444d  ld set `SOLO_ADM
+000015c0: 494e 5f53 4b49 505f 4f42 4a45 4354 5f4c  IN_SKIP_OBJECT_L
+000015d0: 4953 545f 5041 4745 6020 746f 2060 4661  IST_PAGE` to `Fa
+000015e0: 6c73 6560 2069 6e20 796f 7572 2073 6574  lse` in your set
+000015f0: 7469 6e67 732e 0d0a 0d0a 4176 6169 6c61  tings.....Availa
+00001600: 6269 6c69 7479 2066 726f 6d20 7465 6d70  bility from temp
+00001610: 6c61 7465 730d 0a2d 2d2d 2d2d 2d2d 2d2d  lates..---------
+00001620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001630: 2d2d 0d0a 0d0a 5468 6520 7369 6e67 6c65  --....The single
+00001640: 746f 6e20 6f62 6a65 6374 2063 616e 2062  ton object can b
+00001650: 6520 7265 7472 6965 7665 6420 6672 6f6d  e retrieved from
+00001660: 2074 656d 706c 6174 6520 6279 2067 6976   template by giv
+00001670: 696e 6720 7468 6520 446a 616e 676f 206d  ing the Django m
+00001680: 6f64 656c 0d0a 646f 7474 6564 2070 6174  odel..dotted pat
+00001690: 683a 0d0a 0d0a 6060 6064 6a61 6e67 6f0d  h:....```django.
+000016a0: 0a7b 2520 6765 745f 736f 6c6f 2027 6170  .{% get_solo 'ap
+000016b0: 705f 6c61 6265 6c2e 4d6f 6465 6c4e 616d  p_label.ModelNam
+000016c0: 6527 2061 7320 6d79 5f63 6f6e 6669 6720  e' as my_config 
+000016d0: 257d 0d0a 6060 600d 0a0d 0a45 7861 6d70  %}..```....Examp
+000016e0: 6c65 3a0d 0a0d 0a60 6060 646a 616e 676f  le:....```django
+000016f0: 0d0a 7b25 206c 6f61 6420 736f 6c6f 5f74  ..{% load solo_t
+00001700: 6167 7320 257d 0d0a 7b25 2067 6574 5f73  ags %}..{% get_s
+00001710: 6f6c 6f20 2763 6f6e 6669 672e 5369 7465  olo 'config.Site
+00001720: 436f 6e66 6967 7572 6174 696f 6e27 2061  Configuration' a
+00001730: 7320 7369 7465 5f63 6f6e 6669 6720 257d  s site_config %}
+00001740: 0d0a 7b7b 2073 6974 655f 636f 6e66 6967  ..{{ site_config
+00001750: 2e73 6974 655f 6e61 6d65 207d 7d0d 0a7b  .site_name }}..{
+00001760: 7b20 7369 7465 5f63 6f6e 6669 672e 6d61  { site_config.ma
+00001770: 696e 7465 6e61 6e63 655f 6d6f 6465 207d  intenance_mode }
+00001780: 7d0d 0a60 6060 0d0a 0d0a 4966 2079 6f75  }..```....If you
+00001790: 2772 6520 6578 7465 6e64 696e 6720 6120  're extending a 
+000017a0: 7465 6d70 6c61 7465 2c20 6265 2073 7572  template, be sur
+000017b0: 6520 746f 2075 7365 2074 6865 2074 6167  e to use the tag
+000017c0: 2069 6e20 7468 6520 7072 6f70 6572 2073   in the proper s
+000017d0: 636f 7065 2e0d 0a0d 0a52 6967 6874 3a0d  cope.....Right:.
+000017e0: 0a0d 0a60 6060 646a 616e 676f 0d0a 7b25  ...```django..{%
+000017f0: 2065 7874 656e 6473 2022 696e 6465 782e   extends "index.
+00001800: 6874 6d6c 2220 257d 0d0a 7b25 206c 6f61  html" %}..{% loa
+00001810: 6420 736f 6c6f 5f74 6167 7320 257d 0d0a  d solo_tags %}..
+00001820: 0d0a 7b25 2062 6c6f 636b 2063 6f6e 7465  ..{% block conte
+00001830: 6e74 2025 7d0d 0a20 2020 207b 2520 6765  nt %}..    {% ge
+00001840: 745f 736f 6c6f 2027 636f 6e66 6967 2e53  t_solo 'config.S
+00001850: 6974 6543 6f6e 6669 6775 7261 7469 6f6e  iteConfiguration
+00001860: 2720 6173 2073 6974 655f 636f 6e66 6967  ' as site_config
+00001870: 2025 7d0d 0a20 2020 207b 7b20 7369 7465   %}..    {{ site
+00001880: 5f63 6f6e 6669 672e 7369 7465 5f6e 616d  _config.site_nam
+00001890: 6520 7d7d 0d0a 7b25 2065 6e64 626c 6f63  e }}..{% endbloc
+000018a0: 6b20 636f 6e74 656e 7420 257d 0d0a 6060  k content %}..``
+000018b0: 600d 0a0d 0a57 726f 6e67 3a0d 0a0d 0a60  `....Wrong:....`
+000018c0: 6060 646a 616e 676f 0d0a 7b25 2065 7874  ``django..{% ext
+000018d0: 656e 6473 2022 696e 6465 782e 6874 6d6c  ends "index.html
+000018e0: 2220 257d 0d0a 7b25 206c 6f61 6420 736f  " %}..{% load so
+000018f0: 6c6f 5f74 6167 7320 257d 0d0a 7b25 2067  lo_tags %}..{% g
+00001900: 6574 5f73 6f6c 6f20 2763 6f6e 6669 672e  et_solo 'config.
+00001910: 5369 7465 436f 6e66 6967 7572 6174 696f  SiteConfiguratio
+00001920: 6e27 2061 7320 7369 7465 5f63 6f6e 6669  n' as site_confi
+00001930: 6720 257d 0d0a 0d0a 7b25 2062 6c6f 636b  g %}....{% block
+00001940: 2063 6f6e 7465 6e74 2025 7d0d 0a20 2020   content %}..   
+00001950: 207b 7b20 7369 7465 5f63 6f6e 6669 672e   {{ site_config.
+00001960: 7369 7465 5f6e 616d 6520 7d7d 0d0a 7b25  site_name }}..{%
+00001970: 2065 6e64 626c 6f63 6b20 636f 6e74 656e   endblock conten
+00001980: 7420 257d 0d0a 6060 600d 0a0d 0a0d 0a43  t %}..```......C
+00001990: 6163 6869 6e67 0d0a 2d2d 2d2d 2d2d 2d0d  aching..-------.
+000019a0: 0a0d 0a42 7920 6465 6661 756c 7420 6361  ...By default ca
+000019b0: 6368 696e 6720 6973 2064 6973 6162 6c65  ching is disable
+000019c0: 643a 2065 7665 7279 2074 696d 6520 6067  d: every time `g
+000019d0: 6574 5f73 6f6c 6f60 2072 6574 7269 6576  et_solo` retriev
+000019e0: 6573 2074 6865 2073 696e 676c 6574 6f6e  es the singleton
+000019f0: 0d0a 6f62 6a65 6374 2c20 7468 6572 6520  ..object, there 
+00001a00: 7769 6c6c 2062 6520 6120 6461 7461 6261  will be a databa
+00001a10: 7365 2071 7565 7279 2e0d 0a0d 0a59 6f75  se query.....You
+00001a20: 2063 616e 2065 6e61 626c 6520 6361 6368   can enable cach
+00001a30: 696e 6720 746f 206f 6e6c 7920 7175 6572  ing to only quer
+00001a40: 7920 7468 6520 6461 7461 6261 7365 2077  y the database w
+00001a50: 6865 6e20 696e 6974 6961 6c6c 7920 7265  hen initially re
+00001a60: 7472 6965 7669 6e67 2074 6865 0d0a 6f62  trieving the..ob
+00001a70: 6a65 6374 2e20 5468 6520 6361 6368 6520  ject. The cache 
+00001a80: 7769 6c6c 2061 6c73 6f20 6265 2075 7064  will also be upd
+00001a90: 6174 6564 2077 6865 6e20 7570 6461 7465  ated when update
+00001aa0: 7320 6172 6520 6d61 6465 2066 726f 6d20  s are made from 
+00001ab0: 7468 6520 6164 6d69 6e2e 0d0a 0d0a 5468  the admin.....Th
+00001ac0: 6520 6361 6368 6520 7469 6d65 6f75 7420  e cache timeout 
+00001ad0: 6973 2063 6f6e 7472 6f6c 6c65 6420 7669  is controlled vi
+00001ae0: 6120 7468 6520 6053 4f4c 4f5f 4341 4348  a the `SOLO_CACH
+00001af0: 455f 5449 4d45 4f55 5460 2073 6574 7469  E_TIMEOUT` setti
+00001b00: 6e67 732e 0d0a 5468 6520 6361 6368 6520  ngs...The cache 
+00001b10: 6261 636b 656e 6420 746f 2062 6520 7573  backend to be us
+00001b20: 6564 2069 7320 636f 6e74 726f 6c6c 6564  ed is controlled
+00001b30: 2076 6961 2074 6865 2060 534f 4c4f 5f43   via the `SOLO_C
+00001b40: 4143 4845 6020 7365 7474 696e 6773 2e0d  ACHE` settings..
+00001b50: 0a0d 0a0d 0a53 6574 7469 6e67 730d 0a2d  .....Settings..-
+00001b60: 2d2d 2d2d 2d2d 2d0d 0a0d 0a23 2323 2054  -------....### T
+00001b70: 656d 706c 6174 6520 7461 6720 6e61 6d65  emplate tag name
+00001b80: 0d0a 0d0a 596f 7520 6361 6e20 7265 7472  ....You can retr
+00001b90: 6965 7665 2079 6f75 7220 7369 6e67 6c65  ieve your single
+00001ba0: 746f 6e20 6f62 6a65 6374 2069 6e20 7465  ton object in te
+00001bb0: 6d70 6c61 7465 7320 7573 696e 6720 7468  mplates using th
+00001bc0: 6520 6067 6574 5f73 6f6c 6f60 0d0a 7465  e `get_solo`..te
+00001bd0: 6d70 6c61 7465 2074 6167 2e0d 0a0d 0a59  mplate tag.....Y
+00001be0: 6f75 2063 616e 2063 6861 6e67 6520 7468  ou can change th
+00001bf0: 6520 6e61 6d65 2060 6765 745f 736f 6c6f  e name `get_solo
+00001c00: 6020 7573 696e 6720 7468 650d 0a60 4745  ` using the..`GE
+00001c10: 545f 534f 4c4f 5f54 454d 504c 4154 455f  T_SOLO_TEMPLATE_
+00001c20: 5441 475f 4e41 4d45 6020 7365 7474 696e  TAG_NAME` settin
+00001c30: 672e 0d0a 0d0a 6060 6070 7974 686f 6e0d  g.....```python.
+00001c40: 0a47 4554 5f53 4f4c 4f5f 5445 4d50 4c41  .GET_SOLO_TEMPLA
+00001c50: 5445 5f54 4147 5f4e 414d 4520 3d20 2767  TE_TAG_NAME = 'g
+00001c60: 6574 5f63 6f6e 6669 6727 0d0a 6060 600d  et_config'..```.
+00001c70: 0a0d 0a23 2323 2041 646d 696e 206f 7665  ...### Admin ove
+00001c80: 7272 6964 6520 666c 6167 0d0a 0d0a 4279  rride flag....By
+00001c90: 2064 6566 6175 6c74 2c20 7468 6520 6164   default, the ad
+00001ca0: 6d69 6e20 6973 206f 7665 7272 6964 6465  min is overridde
+00001cb0: 6e2e 2042 7574 2069 6620 796f 7520 7769  n. But if you wi
+00001cc0: 7368 2074 6f20 6b65 6570 2074 6865 206f  sh to keep the o
+00001cd0: 626a 6563 7420 6c69 7374 0d0a 7061 6765  bject list..page
+00001ce0: 2028 652e 672e 2074 6f20 6375 7374 6f6d   (e.g. to custom
+00001cf0: 697a 6520 6163 7469 6f6e 7329 2c20 796f  ize actions), yo
+00001d00: 7520 6361 6e20 7365 7420 7468 6520 6053  u can set the `S
+00001d10: 4f4c 4f5f 4144 4d49 4e5f 534b 4950 5f4f  OLO_ADMIN_SKIP_O
+00001d20: 424a 4543 545f 4c49 5354 5f50 4147 4560  BJECT_LIST_PAGE`
+00001d30: 0d0a 746f 2060 4661 6c73 6560 2e0d 0a0d  ..to `False`....
+00001d40: 0a60 6060 7079 7468 6f6e 0d0a 534f 4c4f  .```python..SOLO
+00001d50: 5f41 444d 494e 5f53 4b49 505f 4f42 4a45  _ADMIN_SKIP_OBJE
+00001d60: 4354 5f4c 4953 545f 5041 4745 203d 2054  CT_LIST_PAGE = T
+00001d70: 7275 650d 0a60 6060 0d0a 0d0a 2323 2320  rue..```....### 
+00001d80: 4361 6368 6520 6261 636b 656e 640d 0a0d  Cache backend...
+00001d90: 0a44 6a61 6e67 6f20 7072 6f76 6964 6573  .Django provides
+00001da0: 2061 2077 6179 2074 6f20 6465 6669 6e65   a way to define
+00001db0: 206d 756c 7469 706c 6520 6361 6368 6520   multiple cache 
+00001dc0: 6261 636b 656e 6473 2077 6974 6820 7468  backends with th
+00001dd0: 6520 6043 4143 4845 5360 0d0a 7365 7474  e `CACHES`..sett
+00001de0: 696e 6773 2e20 4966 2079 6f75 2077 616e  ings. If you wan
+00001df0: 7420 7468 6520 7369 6e67 6c65 746f 6e20  t the singleton 
+00001e00: 6f62 6a65 6374 2074 6f20 6265 2063 6163  object to be cac
+00001e10: 6865 6420 7365 7061 7261 7465 6c79 2c20  hed separately, 
+00001e20: 796f 750d 0a63 6f75 6c64 2064 6566 696e  you..could defin
+00001e30: 6520 7468 6520 6043 4143 4845 5360 2061  e the `CACHES` a
+00001e40: 6e64 2074 6865 2060 534f 4c4f 5f43 4143  nd the `SOLO_CAC
+00001e50: 4845 6020 7365 7474 696e 6773 206c 696b  HE` settings lik
+00001e60: 6520 7468 6973 3a0d 0a0d 0a60 6060 7079  e this:....```py
+00001e70: 7468 6f6e 0d0a 4341 4348 4553 203d 207b  thon..CACHES = {
+00001e80: 0d0a 2020 2020 2764 6566 6175 6c74 273a  ..    'default':
+00001e90: 207b 0d0a 2020 2020 2020 2020 2742 4143   {..        'BAC
+00001ea0: 4b45 4e44 273a 2027 646a 616e 676f 2e63  KEND': 'django.c
+00001eb0: 6f72 652e 6361 6368 652e 6261 636b 656e  ore.cache.backen
+00001ec0: 6473 2e6d 656d 6361 6368 6564 2e4d 656d  ds.memcached.Mem
+00001ed0: 6361 6368 6564 4361 6368 6527 2c0d 0a20  cachedCache',.. 
+00001ee0: 2020 2020 2020 2027 4c4f 4341 5449 4f4e         'LOCATION
+00001ef0: 273a 2027 3132 372e 302e 302e 313a 3131  ': '127.0.0.1:11
+00001f00: 3231 3127 2c0d 0a20 2020 207d 2c0d 0a20  211',..    },.. 
+00001f10: 2020 2027 6c6f 6361 6c27 3a20 7b0d 0a20     'local': {.. 
+00001f20: 2020 2020 2020 2027 4241 434b 454e 4427         'BACKEND'
+00001f30: 3a20 2764 6a61 6e67 6f2e 636f 7265 2e63  : 'django.core.c
+00001f40: 6163 6865 2e62 6163 6b65 6e64 732e 6c6f  ache.backends.lo
+00001f50: 636d 656d 2e4c 6f63 4d65 6d43 6163 6865  cmem.LocMemCache
+00001f60: 272c 0d0a 2020 2020 7d2c 0d0a 7d0d 0a0d  ',..    },..}...
+00001f70: 0a53 4f4c 4f5f 4341 4348 4520 3d20 276c  .SOLO_CACHE = 'l
+00001f80: 6f63 616c 270d 0a60 6060 0d0a 0d0a 4361  ocal'..```....Ca
+00001f90: 6368 696e 6720 7769 6c6c 2062 6520 6469  ching will be di
+00001fa0: 7361 626c 6564 2069 6620 7365 7420 746f  sabled if set to
+00001fb0: 2060 4e6f 6e65 602e 0d0a 0d0a 0d0a 2323   `None`.......##
+00001fc0: 2320 4361 6368 6520 7469 6d65 6f75 740d  # Cache timeout.
+00001fd0: 0a0d 0a54 6865 2063 6163 6865 2074 696d  ...The cache tim
+00001fe0: 656f 7574 2069 6e20 7365 636f 6e64 732e  eout in seconds.
+00001ff0: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a53  ....```python..S
+00002000: 4f4c 4f5f 4341 4348 455f 5449 4d45 4f55  OLO_CACHE_TIMEOU
+00002010: 5420 3d20 3630 2a35 2020 2320 3520 6d69  T = 60*5  # 5 mi
+00002020: 6e73 0d0a 6060 600d 0a0d 0a23 2323 2043  ns..```....### C
+00002030: 6163 6865 2070 7265 6669 780d 0a0d 0a54  ache prefix....T
+00002040: 6865 2070 7265 6669 7820 746f 2075 7365  he prefix to use
+00002050: 2066 6f72 2074 6865 2063 6163 6865 206b   for the cache k
+00002060: 6579 2e0d 0a0d 0a60 6060 7079 7468 6f6e  ey.....```python
+00002070: 0d0a 534f 4c4f 5f43 4143 4845 5f50 5245  ..SOLO_CACHE_PRE
+00002080: 4649 5820 3d20 2773 6f6c 6f27 0d0a 6060  FIX = 'solo'..``
+00002090: 600d 0a0d 0a47 6574 7469 6e67 2074 6865  `....Getting the
+000020a0: 2063 6f64 650d 0a3d 3d3d 3d3d 3d3d 3d3d   code..=========
+000020b0: 3d3d 3d3d 3d3d 3d0d 0a0d 0a54 6865 2063  =======....The c
+000020c0: 6f64 6520 6973 2068 6f73 7465 6420 6174  ode is hosted at
+000020d0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000020e0: 636f 6d2f 6c61 7a79 6269 7264 2f64 6a61  com/lazybird/dja
+000020f0: 6e67 6f2d 736f 6c6f 2f0d 0a0d 0a43 6865  ngo-solo/....Che
+00002100: 636b 206f 7574 2074 6865 206c 6174 6573  ck out the lates
+00002110: 7420 6465 7665 6c6f 706d 656e 7420 7665  t development ve
+00002120: 7273 696f 6e20 616e 6f6e 796d 6f75 736c  rsion anonymousl
+00002130: 7920 7769 7468 3a0d 0a0d 0a20 2020 2024  y with:....    $
+00002140: 2067 6974 2063 6c6f 6e65 2067 6974 3a2f   git clone git:/
+00002150: 2f67 6974 6875 622e 636f 6d2f 6c61 7a79  /github.com/lazy
+00002160: 6269 7264 2f64 6a61 6e67 6f2d 736f 6c6f  bird/django-solo
+00002170: 2e67 6974 0d0a 0d0a 596f 7520 6361 6e20  .git....You can 
+00002180: 696e 7374 616c 6c20 7468 6520 7061 636b  install the pack
+00002190: 6167 6520 696e 2074 6865 2022 6564 6974  age in the "edit
+000021a0: 6162 6c65 2220 6d6f 6465 206c 696b 6520  able" mode like 
+000021b0: 7468 6973 3a0d 0a0d 0a20 2020 2070 6970  this:....    pip
+000021c0: 2075 6e69 6e73 7461 6c6c 2064 6a61 6e67   uninstall djang
+000021d0: 6f2d 736f 6c6f 2020 2320 6a75 7374 2069  o-solo  # just i
+000021e0: 6e20 6361 7365 2e2e 2e0d 0a20 2020 2070  n case.....    p
+000021f0: 6970 2069 6e73 7461 6c6c 202d 6520 6769  ip install -e gi
+00002200: 742b 6874 7470 733a 2f2f 6769 7468 7562  t+https://github
+00002210: 2e63 6f6d 2f6c 617a 7962 6972 642f 646a  .com/lazybird/dj
+00002220: 616e 676f 2d73 6f6c 6f2e 6769 7423 6567  ango-solo.git#eg
+00002230: 673d 646a 616e 676f 2d73 6f6c 6f0d 0a0d  g=django-solo...
+00002240: 0a59 6f75 2063 616e 2061 6c73 6f20 696e  .You can also in
+00002250: 7374 616c 6c20 6120 7370 6563 6966 6963  stall a specific
+00002260: 2062 7261 6e63 683a 0d0a 0d0a 2020 2020   branch:....    
+00002270: 7069 7020 696e 7374 616c 6c20 2d65 2067  pip install -e g
+00002280: 6974 2b68 7474 7073 3a2f 2f67 6974 6875  it+https://githu
+00002290: 622e 636f 6d2f 6c61 7a79 6269 7264 2f64  b.com/lazybird/d
+000022a0: 6a61 6e67 6f2d 736f 6c6f 2e67 6974 406d  jango-solo.git@m
+000022b0: 792d 6272 616e 6368 2365 6767 3d64 6a61  y-branch#egg=dja
+000022c0: 6e67 6f2d 736f 6c6f 0d0a 0d0a 5468 6520  ngo-solo....The 
+000022d0: 7061 636b 6167 6520 6973 206e 6f77 2069  package is now i
+000022e0: 6e73 7461 6c6c 6564 2069 6e20 796f 7572  nstalled in your
+000022f0: 2070 726f 6a65 6374 2061 6e64 2079 6f75   project and you
+00002300: 2063 616e 2066 696e 6420 7468 6520 636f   can find the co
+00002310: 6465 2e0d 0a0d 0a54 6f20 7275 6e20 7468  de.....To run th
+00002320: 6520 756e 6974 2074 6573 7473 3a0d 0a0d  e unit tests:...
+00002330: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
+00002340: 2074 6f78 0d0a 2020 2020 746f 780d 0a0d   tox..    tox...
+00002350: 0a23 2323 204d 616b 696e 6720 6120 7265  .### Making a re
+00002360: 6c65 6173 650d 0a0d 0a31 2e20 5570 6461  lease....1. Upda
+00002370: 7465 205b 6073 6f6c 6f2f 5f5f 696e 6974  te [`solo/__init
+00002380: 5f5f 2e70 7960 5d28 736f 6c6f 2f5f 5f69  __.py`](solo/__i
+00002390: 6e69 745f 5f2e 7079 2920 6076 6572 7369  nit__.py) `versi
+000023a0: 6f6e 600d 0a0d 0a32 2e20 4d61 6b65 2061  on`....2. Make a
+000023b0: 206e 6577 2072 656c 6561 7365 206f 6e20   new release on 
+000023c0: 4769 7448 7562 0d0a 0d0a 6060 6073 6865  GitHub....```she
+000023d0: 6c6c 0d0a 746f 7820 2d65 2062 7569 6c64  ll..tox -e build
+000023e0: 0d0a 6060 600d 0a0d 0a60 6060 7368 656c  ..```....```shel
+000023f0: 6c0d 0a74 6f78 202d 6520 7570 6c6f 6164  l..tox -e upload
+00002400: 0d0a 6060 600d 0a                        ..```..
```

### Comparing `django-solo-2.0.0/django_solo.egg-info/SOURCES.txt` & `django-solo-2.1.0/django_solo.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 django_solo.egg-info/requires.txt
 django_solo.egg-info/top_level.txt
 solo/__init__.py
 solo/admin.py
 solo/apps.py
 solo/models.py
 solo/settings.py
+solo/locale/de/LC_MESSAGES/django.mo
+solo/locale/de/LC_MESSAGES/django.po
 solo/locale/es/LC_MESSAGES/django.mo
 solo/locale/es/LC_MESSAGES/django.po
 solo/templates/admin/solo/change_form.html
 solo/templates/admin/solo/object_history.html
 solo/templatetags/__init__.py
 solo/templatetags/solo_tags.py
 solo/tests/__init__.py
```

### Comparing `django-solo-2.0.0/setup.py` & `django-solo-2.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,56 @@
-import os
-import re
-
-from setuptools import setup, find_packages
-
-README = os.path.join(os.path.dirname(__file__), 'README.md')
-
-# When running tests using tox, README.md is not found
-try:
-    with open(README) as file:
-        long_description = file.read()
-except Exception:
-    long_description = ''
-
-
-def get_version(package):
-    """
-    Return package version as listed in `__version__` in `__init__.py`.
-    """
-    with open(os.path.join(package, '__init__.py')) as file:
-        init_py = file.read()
-    return re.search("__version__ = ['\"]([^'\"]+)['\"]", init_py).group(1)
-
-
-version = get_version('solo')
-
-setup(
-    name='django-solo',
-    version=version,
-    description='Django Solo helps working with singletons',
-    python_requires='>=3.6',
-    install_requires=['django>=2.2'],
-    packages=find_packages(),
-    url='https://github.com/lazybird/django-solo/',
-    author='lazybird',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    include_package_data=True,
-    zip_safe=False,
-    license='Creative Commons Attribution 3.0 Unported',
-    classifiers=[
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
-        'Intended Audience :: Developers',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-    ]
-)
+import os
+import re
+
+from setuptools import setup, find_packages
+
+README = os.path.join(os.path.dirname(__file__), 'README.md')
+
+# When running tests using tox, README.md is not found
+try:
+    with open(README) as file:
+        long_description = file.read()
+except Exception:
+    long_description = ''
+
+
+def get_version(package):
+    """
+    Return package version as listed in `__version__` in `__init__.py`.
+    """
+    with open(os.path.join(package, '__init__.py')) as file:
+        init_py = file.read()
+    return re.search("__version__ = ['\"]([^'\"]+)['\"]", init_py).group(1)
+
+
+version = get_version('solo')
+
+setup(
+    name='django-solo',
+    version=version,
+    description='Django Solo helps working with singletons',
+    python_requires='>=3.7',
+    install_requires=['django>=3.2'],
+    packages=find_packages(),
+    url='https://github.com/lazybird/django-solo/',
+    author='lazybird',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
+    include_package_data=True,
+    zip_safe=False,
+    license='Creative Commons Attribution 3.0 Unported',
+    classifiers=[
+        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
+        'Intended Audience :: Developers',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+    ]
+)
```

### Comparing `django-solo-2.0.0/solo/admin.py` & `django-solo-2.1.0/solo/admin.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-from django.urls import re_path
-from django.contrib import admin
-from django.http import HttpResponseRedirect
-from django.utils.encoding import force_str
-from django.utils.translation import gettext as _
-
-from solo.models import DEFAULT_SINGLETON_INSTANCE_ID
-from solo import settings as solo_settings
-
-
-class SingletonModelAdmin(admin.ModelAdmin):
-    object_history_template = "admin/solo/object_history.html"
-    change_form_template = "admin/solo/change_form.html"
-
-    def has_add_permission(self, request):
-        return False
-
-    def has_delete_permission(self, request, obj=None):
-        return False
-
-    def get_urls(self):
-        urls = super(SingletonModelAdmin, self).get_urls()
-
-        if not solo_settings.SOLO_ADMIN_SKIP_OBJECT_LIST_PAGE:
-            return urls
-
-        # _meta.model_name only exists on Django>=1.6 -
-        # on earlier versions, use module_name.lower()
-        try:
-            model_name = self.model._meta.model_name
-        except AttributeError:
-            model_name = self.model._meta.module_name.lower()
-
-        self.model._meta.verbose_name_plural = self.model._meta.verbose_name
-        url_name_prefix = '%(app_name)s_%(model_name)s' % {
-            'app_name': self.model._meta.app_label,
-            'model_name': model_name,
-        }
-        custom_urls = [
-            re_path(r'^history/$',
-                    self.admin_site.admin_view(self.history_view),
-                    {'object_id': str(self.singleton_instance_id)},
-                    name='%s_history' % url_name_prefix),
-            re_path(r'^$',
-                    self.admin_site.admin_view(self.change_view),
-                    {'object_id': str(self.singleton_instance_id)},
-                    name='%s_change' % url_name_prefix),
-        ]
-
-        # By inserting the custom URLs first, we overwrite the standard URLs.
-        return custom_urls + urls
-
-    def response_change(self, request, obj):
-        msg = _('%(obj)s was changed successfully.') % {
-            'obj': force_str(obj)}
-        if '_continue' in request.POST:
-            self.message_user(request, msg + ' ' +
-                              _('You may edit it again below.'))
-            return HttpResponseRedirect(request.path)
-        else:
-            self.message_user(request, msg)
-            return HttpResponseRedirect("../../")
-
-    def change_view(self, request, object_id, form_url='', extra_context=None):
-        if object_id == str(self.singleton_instance_id):
-            self.model.objects.get_or_create(pk=self.singleton_instance_id)
-
-        if not extra_context:
-            extra_context = dict()
-        extra_context['skip_object_list_page'] = solo_settings.SOLO_ADMIN_SKIP_OBJECT_LIST_PAGE
-
-        return super(SingletonModelAdmin, self).change_view(
-            request,
-            object_id,
-            form_url=form_url,
-            extra_context=extra_context,
-        )
-
-    def history_view(self, request, object_id, extra_context=None):
-        if not extra_context:
-            extra_context = dict()
-        extra_context['skip_object_list_page'] = solo_settings.SOLO_ADMIN_SKIP_OBJECT_LIST_PAGE
-
-        return super(SingletonModelAdmin, self).history_view(
-            request,
-            object_id,
-            extra_context=extra_context,
-        )
-
-    @property
-    def singleton_instance_id(self):
-        return getattr(self.model, 'singleton_instance_id', DEFAULT_SINGLETON_INSTANCE_ID)
+from django.urls import re_path
+from django.contrib import admin
+from django.http import HttpResponseRedirect
+from django.utils.encoding import force_str
+from django.utils.translation import gettext as _
+
+from solo.models import DEFAULT_SINGLETON_INSTANCE_ID
+from solo import settings as solo_settings
+
+
+class SingletonModelAdmin(admin.ModelAdmin):
+    object_history_template = "admin/solo/object_history.html"
+    change_form_template = "admin/solo/change_form.html"
+
+    def has_add_permission(self, request):
+        return False
+
+    def has_delete_permission(self, request, obj=None):
+        return False
+
+    def get_urls(self):
+        urls = super(SingletonModelAdmin, self).get_urls()
+
+        if not solo_settings.SOLO_ADMIN_SKIP_OBJECT_LIST_PAGE:
+            return urls
+
+        # _meta.model_name only exists on Django>=1.6 -
+        # on earlier versions, use module_name.lower()
+        try:
+            model_name = self.model._meta.model_name
+        except AttributeError:
+            model_name = self.model._meta.module_name.lower()
+
+        self.model._meta.verbose_name_plural = self.model._meta.verbose_name
+        url_name_prefix = '%(app_name)s_%(model_name)s' % {
+            'app_name': self.model._meta.app_label,
+            'model_name': model_name,
+        }
+        custom_urls = [
+            re_path(r'^history/$',
+                    self.admin_site.admin_view(self.history_view),
+                    {'object_id': str(self.singleton_instance_id)},
+                    name='%s_history' % url_name_prefix),
+            re_path(r'^$',
+                    self.admin_site.admin_view(self.change_view),
+                    {'object_id': str(self.singleton_instance_id)},
+                    name='%s_change' % url_name_prefix),
+        ]
+
+        # By inserting the custom URLs first, we overwrite the standard URLs.
+        return custom_urls + urls
+
+    def response_change(self, request, obj):
+        msg = _('%(obj)s was changed successfully.') % {
+            'obj': force_str(obj)}
+        if '_continue' in request.POST:
+            self.message_user(request, msg + ' ' +
+                              _('You may edit it again below.'))
+            return HttpResponseRedirect(request.path)
+        else:
+            self.message_user(request, msg)
+            return HttpResponseRedirect("../../")
+
+    def change_view(self, request, object_id, form_url='', extra_context=None):
+        if object_id == str(self.singleton_instance_id):
+            self.model.objects.get_or_create(pk=self.singleton_instance_id)
+
+        if not extra_context:
+            extra_context = dict()
+        extra_context['skip_object_list_page'] = solo_settings.SOLO_ADMIN_SKIP_OBJECT_LIST_PAGE
+
+        return super(SingletonModelAdmin, self).change_view(
+            request,
+            object_id,
+            form_url=form_url,
+            extra_context=extra_context,
+        )
+
+    def history_view(self, request, object_id, extra_context=None):
+        if not extra_context:
+            extra_context = dict()
+        extra_context['skip_object_list_page'] = solo_settings.SOLO_ADMIN_SKIP_OBJECT_LIST_PAGE
+
+        return super(SingletonModelAdmin, self).history_view(
+            request,
+            object_id,
+            extra_context=extra_context,
+        )
+
+    @property
+    def singleton_instance_id(self):
+        return getattr(self.model, 'singleton_instance_id', DEFAULT_SINGLETON_INSTANCE_ID)
```

### Comparing `django-solo-2.0.0/solo/locale/es/LC_MESSAGES/django.mo` & `django-solo-2.1.0/solo/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-solo-2.0.0/solo/locale/es/LC_MESSAGES/django.po` & `django-solo-2.1.0/solo/locale/es/LC_MESSAGES/django.po`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-# Spanish translation for django-solo.
-# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
-# This file is distributed under the same license as the django-solo package.
-# Álvaro Mondéjar <mondejar1994@gmail.com>, 2020.
-#
-msgid ""
-msgstr ""
-"Project-Id-Version: \n"
-"Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-04-13 16:13+0200\n"
-"PO-Revision-Date: 2008-11-30 12:12\n"
-"Last-Translator: <mondejar1994@gmail.com>\n"
-"Language-Team: es\n"
-"Language: es\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"X-Translated-Using: django-rosetta 0.9.3\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-
-#: solo/admin.py:53
-#, python-format
-msgid "%(obj)s was changed successfully."
-msgstr "%(obj)s fue editado correctamente."
-
-#: solo/admin.py:55
-msgid "You may edit it again below."
-msgstr "Puede volverlo a editar otra vez a continuación."
-
-#: solo/templates/admin/solo/change_form.html:7
-#: solo/templates/admin/solo/object_history.html:6
-msgid "Home"
-msgstr "Inicio"
-
-#: solo/templates/admin/solo/change_form.html:14
-#: solo/templates/admin/solo/object_history.html:9
-msgid "History"
-msgstr "Historial"
-
-#: solo/templates/admin/solo/change_form.html:15
-msgid "View on site"
-msgstr "Ver en el sitio"
-
-#: solo/templatetags/solo_tags.py:22
-#, python-format
-msgid ""
-"Templatetag requires the model dotted path: 'app_label.ModelName'. Received "
-"'%s'."
-msgstr "Templatetag requiere el path del modelo punteado. Recibido '%s'."
-
-#: solo/templatetags/solo_tags.py:28
-#, python-format
-msgid ""
-"Could not get the model name '%(model)s' from the application named '%(app)s'"
-msgstr ""
-"No se pudo obtener el nombre del modelo '%(model)s' de la aplicación llamada "
-"'%(app)s'"
+# Spanish translation for django-solo.
+# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
+# This file is distributed under the same license as the django-solo package.
+# Álvaro Mondéjar <mondejar1994@gmail.com>, 2020.
+#
+msgid ""
+msgstr ""
+"Project-Id-Version: \n"
+"Report-Msgid-Bugs-To: \n"
+"POT-Creation-Date: 2020-04-13 16:13+0200\n"
+"PO-Revision-Date: 2008-11-30 12:12\n"
+"Last-Translator: <mondejar1994@gmail.com>\n"
+"Language-Team: es\n"
+"Language: es\n"
+"MIME-Version: 1.0\n"
+"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Transfer-Encoding: 8bit\n"
+"X-Translated-Using: django-rosetta 0.9.3\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: solo/admin.py:53
+#, python-format
+msgid "%(obj)s was changed successfully."
+msgstr "%(obj)s fue editado correctamente."
+
+#: solo/admin.py:55
+msgid "You may edit it again below."
+msgstr "Puede volverlo a editar otra vez a continuación."
+
+#: solo/templates/admin/solo/change_form.html:7
+#: solo/templates/admin/solo/object_history.html:6
+msgid "Home"
+msgstr "Inicio"
+
+#: solo/templates/admin/solo/change_form.html:14
+#: solo/templates/admin/solo/object_history.html:9
+msgid "History"
+msgstr "Historial"
+
+#: solo/templates/admin/solo/change_form.html:15
+msgid "View on site"
+msgstr "Ver en el sitio"
+
+#: solo/templatetags/solo_tags.py:22
+#, python-format
+msgid ""
+"Templatetag requires the model dotted path: 'app_label.ModelName'. Received "
+"'%s'."
+msgstr "Templatetag requiere el path del modelo punteado. Recibido '%s'."
+
+#: solo/templatetags/solo_tags.py:28
+#, python-format
+msgid ""
+"Could not get the model name '%(model)s' from the application named '%(app)s'"
+msgstr ""
+"No se pudo obtener el nombre del modelo '%(model)s' de la aplicación llamada "
+"'%(app)s'"
```

### Comparing `django-solo-2.0.0/solo/models.py` & `django-solo-2.1.0/solo/models.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from django.conf import settings
-from django.db import models
-
-try:
-    from django.core.cache import caches
-    get_cache = lambda cache_name: caches[cache_name]
-except ImportError:
-    from django.core.cache import get_cache
-
-from solo import settings as solo_settings
-
-DEFAULT_SINGLETON_INSTANCE_ID = 1
-
-class SingletonModel(models.Model):
-    singleton_instance_id = DEFAULT_SINGLETON_INSTANCE_ID
-
-    class Meta:
-        abstract = True
-
-    def save(self, *args, **kwargs):
-        self.pk = self.singleton_instance_id
-        super(SingletonModel, self).save(*args, **kwargs)
-        self.set_to_cache()
-
-    def delete(self, *args, **kwargs):
-        self.clear_cache()
-        super(SingletonModel, self).delete(*args, **kwargs)
-
-    @classmethod
-    def clear_cache(cls):
-        cache_name = getattr(settings, 'SOLO_CACHE', solo_settings.SOLO_CACHE)
-        if cache_name:
-            cache = get_cache(cache_name)
-            cache_key = cls.get_cache_key()
-            cache.delete(cache_key)
-
-    def set_to_cache(self):
-        cache_name = getattr(settings, 'SOLO_CACHE', solo_settings.SOLO_CACHE)
-        if not cache_name:
-            return None
-        cache = get_cache(cache_name)
-        cache_key = self.get_cache_key()
-        timeout = getattr(settings, 'SOLO_CACHE_TIMEOUT', solo_settings.SOLO_CACHE_TIMEOUT)
-        cache.set(cache_key, self, timeout)
-
-    @classmethod
-    def get_cache_key(cls):
-        prefix = getattr(settings, 'SOLO_CACHE_PREFIX', solo_settings.SOLO_CACHE_PREFIX)
-        return '%s:%s' % (prefix, cls.__name__.lower())
-
-    @classmethod
-    def get_solo(cls):
-        cache_name = getattr(settings, 'SOLO_CACHE', solo_settings.SOLO_CACHE)
-        if not cache_name:
-            obj, created = cls.objects.get_or_create(pk=cls.singleton_instance_id)
-            return obj
-        cache = get_cache(cache_name)
-        cache_key = cls.get_cache_key()
-        obj = cache.get(cache_key)
-        if not obj:
-            obj, created = cls.objects.get_or_create(pk=cls.singleton_instance_id)
-            obj.set_to_cache()
-        return obj
+from django.conf import settings
+from django.db import models
+
+try:
+    from django.core.cache import caches
+    get_cache = lambda cache_name: caches[cache_name]
+except ImportError:
+    from django.core.cache import get_cache
+
+from solo import settings as solo_settings
+
+DEFAULT_SINGLETON_INSTANCE_ID = 1
+
+class SingletonModel(models.Model):
+    singleton_instance_id = DEFAULT_SINGLETON_INSTANCE_ID
+
+    class Meta:
+        abstract = True
+
+    def save(self, *args, **kwargs):
+        self.pk = self.singleton_instance_id
+        super(SingletonModel, self).save(*args, **kwargs)
+        self.set_to_cache()
+
+    def delete(self, *args, **kwargs):
+        self.clear_cache()
+        super(SingletonModel, self).delete(*args, **kwargs)
+
+    @classmethod
+    def clear_cache(cls):
+        cache_name = getattr(settings, 'SOLO_CACHE', solo_settings.SOLO_CACHE)
+        if cache_name:
+            cache = get_cache(cache_name)
+            cache_key = cls.get_cache_key()
+            cache.delete(cache_key)
+
+    def set_to_cache(self):
+        cache_name = getattr(settings, 'SOLO_CACHE', solo_settings.SOLO_CACHE)
+        if not cache_name:
+            return None
+        cache = get_cache(cache_name)
+        cache_key = self.get_cache_key()
+        timeout = getattr(settings, 'SOLO_CACHE_TIMEOUT', solo_settings.SOLO_CACHE_TIMEOUT)
+        cache.set(cache_key, self, timeout)
+
+    @classmethod
+    def get_cache_key(cls):
+        prefix = getattr(settings, 'SOLO_CACHE_PREFIX', solo_settings.SOLO_CACHE_PREFIX)
+        return '%s:%s' % (prefix, cls.__name__.lower())
+
+    @classmethod
+    def get_solo(cls):
+        cache_name = getattr(settings, 'SOLO_CACHE', solo_settings.SOLO_CACHE)
+        if not cache_name:
+            obj, created = cls.objects.get_or_create(pk=cls.singleton_instance_id)
+            return obj
+        cache = get_cache(cache_name)
+        cache_key = cls.get_cache_key()
+        obj = cache.get(cache_key)
+        if not obj:
+            obj, created = cls.objects.get_or_create(pk=cls.singleton_instance_id)
+            obj.set_to_cache()
+        return obj
```

### Comparing `django-solo-2.0.0/solo/tests/models.py` & `django-solo-2.1.0/solo/tests/models.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from django.core.files.uploadedfile import SimpleUploadedFile
-from django.db import models
-
-from solo.models import SingletonModel
-
-
-class SiteConfiguration(SingletonModel):
-    site_name = models.CharField(max_length=255, default='Default Config')
-    file = models.FileField(upload_to='files', default=SimpleUploadedFile("default-file.pdf", None))
-
-    def __str__(self):
-        return "Site Configuration"
-
-    class Meta:
-        verbose_name = "Site Configuration"
-
-
-class SiteConfigurationWithExplicitlyGivenId(SingletonModel):
-    singleton_instance_id = 24
-    site_name = models.CharField(max_length=255, default='Default Config')
-
-    def __str__(self):
-        return "Site Configuration"
-
-    class Meta:
-        verbose_name = "Site Configuration"
+from django.core.files.uploadedfile import SimpleUploadedFile
+from django.db import models
+
+from solo.models import SingletonModel
+
+
+class SiteConfiguration(SingletonModel):
+    site_name = models.CharField(max_length=255, default='Default Config')
+    file = models.FileField(upload_to='files', default=SimpleUploadedFile("default-file.pdf", None))
+
+    def __str__(self):
+        return "Site Configuration"
+
+    class Meta:
+        verbose_name = "Site Configuration"
+
+
+class SiteConfigurationWithExplicitlyGivenId(SingletonModel):
+    singleton_instance_id = 24
+    site_name = models.CharField(max_length=255, default='Default Config')
+
+    def __str__(self):
+        return "Site Configuration"
+
+    class Meta:
+        verbose_name = "Site Configuration"
```

### Comparing `django-solo-2.0.0/solo/tests/settings.py` & `django-solo-2.1.0/solo/tests/settings.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-MIDDLEWARE_CLASSES = (
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.middleware.locale.LocaleMiddleware',
-    'django.middleware.common.CommonMiddleware',
-    'django.middleware.csrf.CsrfViewMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',
-)
-
-DATABASES = {
-    'default': {
-        'ENGINE': 'django.db.backends.sqlite3',
-        'NAME': 'solo-tests.db',
-    }
-}
-
-INSTALLED_APPS = (
-    'solo',
-    'solo.tests',
-)
-
-SECRET_KEY = 'any-key'
-
-CACHES = {
-    'default': {
-        'BACKEND': 'django.core.cache.backends.locmem.LocMemCache',
-        'LOCATION': '127.0.0.1:11211',
-    },
-}
-
-SOLO_CACHE = 'default'
-
-TEMPLATES = [
-    {
-        'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'APP_DIRS': True,
-    },
-]
-DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
+MIDDLEWARE_CLASSES = (
+    'django.contrib.sessions.middleware.SessionMiddleware',
+    'django.middleware.locale.LocaleMiddleware',
+    'django.middleware.common.CommonMiddleware',
+    'django.middleware.csrf.CsrfViewMiddleware',
+    'django.contrib.auth.middleware.AuthenticationMiddleware',
+    'django.contrib.messages.middleware.MessageMiddleware',
+)
+
+DATABASES = {
+    'default': {
+        'ENGINE': 'django.db.backends.sqlite3',
+        'NAME': 'solo-tests.db',
+    }
+}
+
+INSTALLED_APPS = (
+    'solo',
+    'solo.tests',
+)
+
+SECRET_KEY = 'any-key'
+
+CACHES = {
+    'default': {
+        'BACKEND': 'django.core.cache.backends.locmem.LocMemCache',
+        'LOCATION': '127.0.0.1:11211',
+    },
+}
+
+SOLO_CACHE = 'default'
+
+TEMPLATES = [
+    {
+        'BACKEND': 'django.template.backends.django.DjangoTemplates',
+        'APP_DIRS': True,
+    },
+]
+DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
```

### Comparing `django-solo-2.0.0/solo/tests/tests.py` & `django-solo-2.1.0/solo/tests/tests.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-from django.core.files.uploadedfile import SimpleUploadedFile
-from django.template import Template, Context
-from django.test import TestCase
-
-from django.test.utils import override_settings
-from solo.models import get_cache
-from solo.tests.models import SiteConfiguration, SiteConfigurationWithExplicitlyGivenId
-
-
-class SingletonTest(TestCase):
-
-    def setUp(self):
-        self.template = Template(
-            '{% load solo_tags %}'
-            '{% get_solo "tests.SiteConfiguration" as site_config  %}'
-            '{{ site_config.site_name }}'
-            '{{ site_config.file.url }}'
-        )
-        self.cache = get_cache('default')
-        self.cache_key = SiteConfiguration.get_cache_key()
-        self.cache.clear()
-        SiteConfiguration.objects.all().delete()
-
-    def test_template_tag_renders_default_site_config(self):
-        SiteConfiguration.objects.all().delete()
-        # At this point, there is no configuration object and we expect a
-        # one to be created automatically with the default name value as
-        # defined in models.
-        output = self.template.render(Context())
-        self.assertIn('Default Config', output)
-
-    def test_template_tag_renders_site_config(self):
-        SiteConfiguration.objects.create(site_name='Test Config')
-        output = self.template.render(Context())
-        self.assertIn('Test Config', output)
-
-    @override_settings(SOLO_CACHE='default')
-    def test_template_tag_uses_cache_if_enabled(self):
-        SiteConfiguration.objects.create(site_name='Config In Database')
-        fake_configuration = {'site_name': 'Config In Cache'}
-        self.cache.set(self.cache_key, fake_configuration, 10)
-        output = self.template.render(Context())
-        self.assertNotIn('Config In Database', output)
-        self.assertNotIn('Default Config', output)
-        self.assertIn('Config In Cache', output)
-
-    @override_settings(SOLO_CACHE=None)
-    def test_template_tag_uses_database_if_cache_disabled(self):
-        SiteConfiguration.objects.create(site_name='Config In Database')
-        fake_configuration = {'site_name': 'Config In Cache'}
-        self.cache.set(self.cache_key, fake_configuration, 10)
-        output = self.template.render(Context())
-        self.assertNotIn('Config In Cache', output)
-        self.assertNotIn('Default Config', output)
-        self.assertIn('Config In Database', output)
-
-    @override_settings(SOLO_CACHE='default')
-    def test_delete_if_cache_enabled(self):
-        self.assertEqual(SiteConfiguration.objects.count(), 0)
-        self.assertIsNone(self.cache.get(self.cache_key))
-
-        one_cfg = SiteConfiguration.get_solo()
-        one_cfg.site_name = 'TEST SITE PLEASE IGNORE'
-        one_cfg.save()
-        self.assertEqual(SiteConfiguration.objects.count(), 1)
-        self.assertIsNotNone(self.cache.get(self.cache_key))
-
-        one_cfg.delete()
-        self.assertEqual(SiteConfiguration.objects.count(), 0)
-        self.assertIsNone(self.cache.get(self.cache_key))
-        self.assertEqual(SiteConfiguration.get_solo().site_name, 'Default Config')
-
-    @override_settings(SOLO_CACHE=None)
-    def test_delete_if_cache_disabled(self):
-        # As above, but without the cache checks
-        self.assertEqual(SiteConfiguration.objects.count(), 0)
-        one_cfg = SiteConfiguration.get_solo()
-        one_cfg.site_name = 'TEST (uncached) SITE PLEASE IGNORE'
-        one_cfg.save()
-        self.assertEqual(SiteConfiguration.objects.count(), 1)
-        one_cfg.delete()
-        self.assertEqual(SiteConfiguration.objects.count(), 0)
-        self.assertEqual(SiteConfiguration.get_solo().site_name, 'Default Config')
-
-    @override_settings(SOLO_CACHE='default')
-    def test_file_upload_if_cache_enabled(self):
-        cfg = SiteConfiguration.objects.create(site_name='Test Config', file=SimpleUploadedFile("file.pdf", None))
-        output = self.template.render(Context())
-        self.assertIn(cfg.file.url, output)
-
-    @override_settings(SOLO_CACHE_PREFIX='other')
-    def test_cache_prefix_overriding(self):
-        key = SiteConfiguration.get_cache_key()
-        prefix = key.partition(':')[0]
-        self.assertEqual(prefix, 'other')
-
-
-class SingletonWithExplicitIdTest(TestCase):
-
-    def setUp(self):
-        SiteConfigurationWithExplicitlyGivenId.objects.all().delete()
-
-    def test_when_singleton_instance_id_is_given_created_item_will_have_given_instance_id(self):
-        item = SiteConfigurationWithExplicitlyGivenId.get_solo()
-        self.assertEqual(item.pk, SiteConfigurationWithExplicitlyGivenId.singleton_instance_id)
+from django.core.files.uploadedfile import SimpleUploadedFile
+from django.template import Template, Context
+from django.test import TestCase
+
+from django.test.utils import override_settings
+from solo.models import get_cache
+from solo.tests.models import SiteConfiguration, SiteConfigurationWithExplicitlyGivenId
+
+
+class SingletonTest(TestCase):
+
+    def setUp(self):
+        self.template = Template(
+            '{% load solo_tags %}'
+            '{% get_solo "tests.SiteConfiguration" as site_config  %}'
+            '{{ site_config.site_name }}'
+            '{{ site_config.file.url }}'
+        )
+        self.cache = get_cache('default')
+        self.cache_key = SiteConfiguration.get_cache_key()
+        self.cache.clear()
+        SiteConfiguration.objects.all().delete()
+
+    def test_template_tag_renders_default_site_config(self):
+        SiteConfiguration.objects.all().delete()
+        # At this point, there is no configuration object and we expect a
+        # one to be created automatically with the default name value as
+        # defined in models.
+        output = self.template.render(Context())
+        self.assertIn('Default Config', output)
+
+    def test_template_tag_renders_site_config(self):
+        SiteConfiguration.objects.create(site_name='Test Config')
+        output = self.template.render(Context())
+        self.assertIn('Test Config', output)
+
+    @override_settings(SOLO_CACHE='default')
+    def test_template_tag_uses_cache_if_enabled(self):
+        SiteConfiguration.objects.create(site_name='Config In Database')
+        fake_configuration = {'site_name': 'Config In Cache'}
+        self.cache.set(self.cache_key, fake_configuration, 10)
+        output = self.template.render(Context())
+        self.assertNotIn('Config In Database', output)
+        self.assertNotIn('Default Config', output)
+        self.assertIn('Config In Cache', output)
+
+    @override_settings(SOLO_CACHE=None)
+    def test_template_tag_uses_database_if_cache_disabled(self):
+        SiteConfiguration.objects.create(site_name='Config In Database')
+        fake_configuration = {'site_name': 'Config In Cache'}
+        self.cache.set(self.cache_key, fake_configuration, 10)
+        output = self.template.render(Context())
+        self.assertNotIn('Config In Cache', output)
+        self.assertNotIn('Default Config', output)
+        self.assertIn('Config In Database', output)
+
+    @override_settings(SOLO_CACHE='default')
+    def test_delete_if_cache_enabled(self):
+        self.assertEqual(SiteConfiguration.objects.count(), 0)
+        self.assertIsNone(self.cache.get(self.cache_key))
+
+        one_cfg = SiteConfiguration.get_solo()
+        one_cfg.site_name = 'TEST SITE PLEASE IGNORE'
+        one_cfg.save()
+        self.assertEqual(SiteConfiguration.objects.count(), 1)
+        self.assertIsNotNone(self.cache.get(self.cache_key))
+
+        one_cfg.delete()
+        self.assertEqual(SiteConfiguration.objects.count(), 0)
+        self.assertIsNone(self.cache.get(self.cache_key))
+        self.assertEqual(SiteConfiguration.get_solo().site_name, 'Default Config')
+
+    @override_settings(SOLO_CACHE=None)
+    def test_delete_if_cache_disabled(self):
+        # As above, but without the cache checks
+        self.assertEqual(SiteConfiguration.objects.count(), 0)
+        one_cfg = SiteConfiguration.get_solo()
+        one_cfg.site_name = 'TEST (uncached) SITE PLEASE IGNORE'
+        one_cfg.save()
+        self.assertEqual(SiteConfiguration.objects.count(), 1)
+        one_cfg.delete()
+        self.assertEqual(SiteConfiguration.objects.count(), 0)
+        self.assertEqual(SiteConfiguration.get_solo().site_name, 'Default Config')
+
+    @override_settings(SOLO_CACHE='default')
+    def test_file_upload_if_cache_enabled(self):
+        cfg = SiteConfiguration.objects.create(site_name='Test Config', file=SimpleUploadedFile("file.pdf", None))
+        output = self.template.render(Context())
+        self.assertIn(cfg.file.url, output)
+
+    @override_settings(SOLO_CACHE_PREFIX='other')
+    def test_cache_prefix_overriding(self):
+        key = SiteConfiguration.get_cache_key()
+        prefix = key.partition(':')[0]
+        self.assertEqual(prefix, 'other')
+
+
+class SingletonWithExplicitIdTest(TestCase):
+
+    def setUp(self):
+        SiteConfigurationWithExplicitlyGivenId.objects.all().delete()
+
+    def test_when_singleton_instance_id_is_given_created_item_will_have_given_instance_id(self):
+        item = SiteConfigurationWithExplicitlyGivenId.get_solo()
+        self.assertEqual(item.pk, SiteConfigurationWithExplicitlyGivenId.singleton_instance_id)
```

