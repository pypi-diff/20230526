# Comparing `tmp/microarch-0.0.8.tar.gz` & `tmp/microarch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microarch-0.0.8.tar", last modified: Mon Sep  5 09:00:01 2022, max compression
+gzip compressed data, was "microarch-0.0.9.tar", last modified: Mon Jan  9 17:38:59 2023, max compression
```

## Comparing `microarch-0.0.8.tar` & `microarch-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 09:00:01.395744 microarch-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-05 08:59:42.000000 microarch-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-09-05 09:00:01.395744 microarch-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-05 08:59:42.000000 microarch-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 09:00:01.395744 microarch-0.0.8/microarch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-09-05 09:00:01.000000 microarch-0.0.8/microarch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-09-05 09:00:01.000000 microarch-0.0.8/microarch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-05 09:00:01.000000 microarch-0.0.8/microarch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-05 09:00:01.000000 microarch-0.0.8/microarch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-05 09:00:01.000000 microarch-0.0.8/microarch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    92739 2022-09-05 08:59:42.000000 microarch-0.0.8/microarch.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-05 09:00:01.395744 microarch-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2587 2022-09-05 08:59:42.000000 microarch-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 17:38:59.830041 microarch-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-01-09 17:38:42.000000 microarch-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-01-09 17:38:59.830041 microarch-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-01-09 17:38:42.000000 microarch-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 17:38:59.830041 microarch-0.0.9/microarch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-01-09 17:38:59.000000 microarch-0.0.9/microarch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-01-09 17:38:59.000000 microarch-0.0.9/microarch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-01-09 17:38:59.000000 microarch-0.0.9/microarch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-01-09 17:38:59.000000 microarch-0.0.9/microarch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-01-09 17:38:59.000000 microarch-0.0.9/microarch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    97922 2023-01-09 17:38:42.000000 microarch-0.0.9/microarch.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-09 17:38:59.830041 microarch-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2587 2023-01-09 17:38:42.000000 microarch-0.0.9/setup.py
```

### Comparing `microarch-0.0.8/LICENSE` & `microarch-0.0.9/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Knuth Project
+Copyright (c) 2022-2023 Knuth Project
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `microarch-0.0.8/PKG-INFO` & `microarch-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microarch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Knuth Microarchitecture Management (CPUID)
 Home-page: https://github.com/k-nuth/microarch
 Author: Fernando Pelliccioni
 Author-email: fpelliccioni@gmail.com
 License: MIT
 Keywords: knuth kth crypto bitcoin btc bch cash build tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `microarch-0.0.8/microarch.egg-info/PKG-INFO` & `microarch-0.0.9/microarch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microarch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Knuth Microarchitecture Management (CPUID)
 Home-page: https://github.com/k-nuth/microarch
 Author: Fernando Pelliccioni
 Author-email: fpelliccioni@gmail.com
 License: MIT
 Keywords: knuth kth crypto bitcoin btc bch cash build tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `microarch-0.0.8/microarch.py` & `microarch-0.0.9/microarch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 #
-# Copyright (c) 2019-2022 Knuth Project
+# Copyright (c) 2019-2023 Knuth Project
 #
 
 from enum import Enum
 import cpuid
 import importlib
 from collections import deque
 
@@ -1111,14 +1111,154 @@
     "SGX_LC",
     "MCOMMIT",
     "RDPRU",
     "INVPCID",
     "SEV_SNP",
 ]
 
+extensions_kth_defines = [
+    None,       # Version Bit 1
+    None,       # Version Bit 0
+    None,       # Version Bit 1
+    None,       # Version Bit 0
+    None,       # Version Bit 1
+    None,       # Version Bit 0
+    None,       # Version Bit 1
+    None,       # Version Bit 0
+
+    None,       # Version Bit 1
+    None,       # Version Bit 0
+    None,       # Version Bit 1
+    None,       # Version Bit 0
+    None,       # Version Bit 1
+    None,       # Version Bit 0
+    None,       # Version Bit 1
+    None,       # Version Bit 0
+
+# 16:
+    "-DKTH_EXT_64_BITS",
+
+# Level 1 (baseline)
+# 17:
+    "-DKTH_EXT_CMOV",
+    "-DKTH_EXT_CX8",
+    "-DKTH_EXT_FPU",
+    "-DKTH_EXT_FXSR",
+    "-DKTH_EXT_MMX",
+    # "-DKTH_EXT_OSFXSR",            # Operating System check.
+    "-DKTH_EXT_SCE",                 # System-Call Extension (SCE) Bit           (some part could be related to OS check)
+    "-DKTH_EXT_SSE",
+    "-DKTH_EXT_SSE2",
+
+# Level 2 - x86-64-v2
+    "-DKTH_EXT_CX16",            # CMPXCHG16B
+    "-DKTH_EXT_LAHF_SAHF",
+    "-DKTH_EXT_POPCNT",
+    "-DKTH_EXT_SSE3",
+    "-DKTH_EXT_SSE4_1",
+    "-DKTH_EXT_SSE4_2",
+    "-DKTH_EXT_SSSE3",
+
+    # Level 3 - x86-64-v3
+    "-DKTH_EXT_AVX",
+    "-DKTH_EXT_AVX2",
+    "-DKTH_EXT_BMI1",
+    "-DKTH_EXT_BMI2",
+    "-DKTH_EXT_F16C",
+    "-DKTH_EXT_FMA",
+    "-DKTH_EXT_LZCNT -DKTH_EXT_ABM",
+    "-DKTH_EXT_MOVBE",
+    "-DKTH_EXT_XSAVE",             # OSXSAVE     # TODO(fernando): según el spec de Levels, acá tenemos que chequear OSXSAVE,
+                                            # pero nosotros solo podemos chequear XSAVE a nivel procesador
+                                            # el chequeo de soporte de features del sistema operativo lo debería hacer
+                                            # el nodo en runtime (o quizás no)
+
+    # Level 4 - x86-64-v4
+    "-DKTH_EXT_AVX512F",
+    "-DKTH_EXT_AVX512BW",
+    "-DKTH_EXT_AVX512CD",
+    "-DKTH_EXT_AVX512DQ",
+    "-DKTH_EXT_AVX512VL",
+
+    # Other Features ------------------------------------------
+    "-DKTH_EXT_SSE4A",
+    "-DKTH_EXT_PKU",
+    "-DKTH_EXT_PCLMUL",
+    "-DKTH_EXT_FSGSBASE",
+    "-DKTH_EXT_RDRND",
+    "-DKTH_EXT_FMA4",
+    "-DKTH_EXT_XOP",
+    "-DKTH_EXT_TBM",
+    "-DKTH_EXT_RDSEED",
+    "-DKTH_EXT_ADX",
+    "-DKTH_EXT_3DNOW",
+    "-DKTH_EXT_3DNOWEXT",
+    "-DKTH_EXT_PREFETCHW",
+    "-DKTH_EXT_PREFETCHWT1",
+    "-DKTH_EXT_CLFLUSHOPT",
+    "-DKTH_EXT_XSAVEOPT",
+    "-DKTH_EXT_XSAVEC",
+    "-DKTH_EXT_XSAVES",
+    "-DKTH_EXT_CLWB",
+    "-DKTH_EXT_PTWRITE",
+    "-DKTH_EXT_RDPID",
+    "-DKTH_EXT_SGX",
+    "-DKTH_EXT_GFNI",
+    "-DKTH_EXT_VPCLMULQDQ",
+    "-DKTH_EXT_PCONFIG",
+    "-DKTH_EXT_WBNOINVD",
+    "-DKTH_EXT_MOVDIRI",
+    "-DKTH_EXT_MOVDIR64B",
+    "-DKTH_EXT_LWP",
+    "-DKTH_EXT_MWAITX",
+    "-DKTH_EXT_CLZERO",
+    "-DKTH_EXT_INVLPGB_TLBSYNC",
+    "-DKTH_EXT_CET_SS",
+    "-DKTH_EXT_AVXVNNI",
+    "-DKTH_EXT_TSXRTM",
+    "-DKTH_EXT_TSXHLE",
+    "-DKTH_EXT_WAITPKG",
+    "-DKTH_EXT_ENQCMD",
+    "-DKTH_EXT_UINTR",
+    "-DKTH_EXT_TSXLDTRK",
+    "-DKTH_EXT_CLDEMOTE",
+    "-DKTH_EXT_SERIALIZE",
+    "-DKTH_EXT_HRESET",
+    "-DKTH_EXT_AES",
+    "-DKTH_EXT_VAES",
+    "-DKTH_EXT_SHA",
+    "-DKTH_EXT_KL",
+    "-DKTH_EXT_WIDEKL",
+    "-DKTH_EXT_AVX512FP16",
+    "-DKTH_EXT_AVX512PF",
+    "-DKTH_EXT_AVX512ER",
+    "-DKTH_EXT_AVX5124VNNIW",
+    "-DKTH_EXT_AVX5124FMAPS",
+    "-DKTH_EXT_AVX512VBMI",
+    "-DKTH_EXT_AVX512IFMA",
+    "-DKTH_EXT_AVX512VBMI2",
+    "-DKTH_EXT_AVX512VPOPCNTDQ",
+    "-DKTH_EXT_AVX512BITALG",
+    "-DKTH_EXT_AVX512VNNI",
+    "-DKTH_EXT_AVX512BF16",
+    "-DKTH_EXT_AVX512VP2INTERSECT",
+    "-DKTH_EXT_AMXBF16",
+    "-DKTH_EXT_AMXTILE",
+    "-DKTH_EXT_AMXINT8",
+    "-DKTH_EXT_MMXEXT",
+    "-DKTH_EXT_XGETBV_ECX1",
+    "-DKTH_EXT_UMIP",
+    "-DKTH_EXT_SGX_LC",
+    "-DKTH_EXT_MCOMMIT",
+    "-DKTH_EXT_RDPRU",
+    "-DKTH_EXT_INVPCID",
+    "-DKTH_EXT_SEV_SNP",
+]
+
+
 extensions_flags = {
     'gcc':         None,
     'apple-clang': None,
     'clang':       None,
     'msvc':        None,
     'mingw':       None
 }
@@ -1732,14 +1872,28 @@
         if i >= len(extensions_names):
             continue
 
         if (exts[i] == 1):
             res.append(extensions_names[i])
     return res
 
+def extensions_to_kth_defines(exts, comp):
+    res = []
+    for i in range(MIN_EXTENSION, len(exts)):
+        if i >= len(extensions_kth_defines):
+            continue
+
+        if (exts[i] == 1):
+            res.append(extensions_kth_defines[i])
+
+    if comp == 'msvc':
+        res = [x.replace('-D', '/D') for x in res]
+
+    return res
+
 # ----------------------------------------------------------------------
 
 class Vendor(Enum):
     Other = 0,
     Intel = 1,
     AMD = 2,
     VIA = 3,
@@ -2029,38 +2183,45 @@
     exts += [0] * (KTH_EXTENSIONS_MAX - len(exts))
     return exts
 
 def get_all_data(os, comp, comp_ver):
     cpu_exts = get_available_extensions()
     cpu_marchid = encode_extensions(cpu_exts)
     cpu_names = extensions_to_names(cpu_exts)
+    cpu_kth_defs = extensions_to_kth_defines(cpu_exts, comp)
+
 
     comp_exts = filter_extensions(cpu_exts, os, comp, comp_ver)
     comp_marchid = encode_extensions(comp_exts)
     comp_names = extensions_to_names(comp_exts)
+    comp_kth_defs = extensions_to_kth_defines(comp_exts, comp)
     comp_flags = get_compiler_flags(comp_exts, os, comp, comp_ver)
 
     level3_exts = level3_on()
     level3_marchid = encode_extensions(level3_exts)
     level3_names = extensions_to_names(level3_exts)
+    level3_kth_defs = extensions_to_kth_defines(level3_exts, comp)
     level3_flags = get_compiler_flags(level3_exts, os, comp, comp_ver)
 
     return {
         'cpu_exts': cpu_exts,
         'cpu_marchid': cpu_marchid,
         'cpu_names': cpu_names,
+        'cpu_kth_defs': cpu_kth_defs,
 
         'comp_exts': comp_exts,
         'comp_marchid': comp_marchid,
         'comp_names': comp_names,
+        'comp_kth_defs': comp_kth_defs,
         'comp_flags': comp_flags,
 
         'level3_exts': level3_exts,
         'level3_marchid': level3_marchid,
         'level3_names': level3_names,
+        'level3_kth_defs': level3_kth_defs,
         'level3_flags': level3_flags,
     }
 
 def get_all_data_from_marchid(marchid, os, comp, comp_ver):
     user_exts = decode_extensions(marchid)
     user_names = None
     user_flags = None
@@ -2071,53 +2232,61 @@
     if user_exts is not None:
         version_bits = get_version_bits()
         exts_version = user_exts[:len(version_bits)]
 
         if version_bits == exts_version:
             user_marchid_valid = True
             user_names = extensions_to_names(user_exts)
+            user_kth_defs = extensions_to_kth_defines(user_exts, comp)
             user_flags = get_compiler_flags(user_exts, os, comp, comp_ver)
             user_exts_filtered = filter_extensions(user_exts, os, comp, comp_ver)
             user_exts_compiler_compatible = user_exts == user_exts_filtered
 
     cpu_exts = get_available_extensions()
     cpu_marchid = encode_extensions(cpu_exts)
     cpu_names = extensions_to_names(cpu_exts)
+    cpu_kth_defs = extensions_to_kth_defines(cpu_exts, comp)
 
     comp_exts = filter_extensions(cpu_exts, os, comp, comp_ver)
     comp_marchid = encode_extensions(comp_exts)
     comp_names = extensions_to_names(comp_exts)
+    comp_kth_defs = extensions_to_kth_defines(comp_exts, comp)
     comp_flags = get_compiler_flags(comp_exts, os, comp, comp_ver)
 
     level3_exts = level3_on()
     level3_marchid = encode_extensions(level3_exts)
     level3_names = extensions_to_names(level3_exts)
+    level3_kth_defs = extensions_to_kth_defines(level3_exts, comp)
     level3_flags = get_compiler_flags(level3_exts, os, comp, comp_ver)
 
     return {
         'user_marchid_valid': user_marchid_valid,
         'user_exts': user_exts,
         'user_exts_filtered': user_exts_filtered,
         'user_marchid': marchid,
         'user_names': user_names,
+        'user_kth_defs': user_kth_defs,
         'user_flags': user_flags,
         'user_exts_compiler_compatible': user_exts_compiler_compatible,
 
         'cpu_exts': cpu_exts,
         'cpu_marchid': cpu_marchid,
+        'cpu_kth_defs': cpu_kth_defs,
         'cpu_names': cpu_names,
 
         'comp_exts': comp_exts,
         'comp_marchid': comp_marchid,
         'comp_names': comp_names,
+        'comp_kth_defs': comp_kth_defs,
         'comp_flags': comp_flags,
 
         'level3_exts': level3_exts,
         'level3_marchid': level3_marchid,
         'level3_names': level3_names,
+        'level3_kth_defs': level3_kth_defs,
         'level3_flags': level3_flags,
     }
 
 def several_tests(os, comp, comp_ver):
 
     exts = level0_on()
     marchid = encode_extensions(exts)
@@ -2192,38 +2361,45 @@
 #         print("Level3 extensions: ", names)
 
 #         level3_flags = get_compiler_flags(level3_exts, os, comp, comp_ver)
 #         print("Level3 compiler flags: ", level3_flags)
 
 
 def main():
-    # print(support_level1_features())
-    # print(support_level2_features())
-    # print(support_level3_features())
-    # print(support_level4_features())
-
-    os = 'Linux'
-    comp = 'gcc'
-    comp_ver = 12
-
-    # os = 'Macos'
-    # comp = 'apple-clang'
-    # comp_ver = 13
+    # # print(support_level1_features())
+    # # print(support_level2_features())
+    # # print(support_level3_features())
+    # # print(support_level4_features())
 
     # os = 'Linux'
-    # comp = 'clang'
-    # comp_ver = 6
+    # comp = 'gcc'
+    # comp_ver = 12
+
+    # # os = 'Macos'
+    # # comp = 'apple-clang'
+    # # comp_ver = 13
+
+    # # os = 'Linux'
+    # # comp = 'clang'
+    # # comp_ver = 6
+
+    # several_tests(os, comp, comp_ver)
+
+    # # comp_flags2 = get_compiler_flags_arch_id(archid, os, comp, comp_ver)
+    # # print(comp_flags2)
+
+    # # for i in range(len(filtered)):
+    # #     print(filtered[i])
+
+
 
-    several_tests(os, comp, comp_ver)
+    xxx = decode_extensions('ZLm9Pjh')
+    print(xxx)
 
-    # comp_flags2 = get_compiler_flags_arch_id(archid, os, comp, comp_ver)
-    # print(comp_flags2)
 
-    # for i in range(len(filtered)):
-    #     print(filtered[i])
 
 if __name__ == "__main__":
     main()
```

### Comparing `microarch-0.0.8/setup.py` & `microarch-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 #
-# Copyright (c) 2019-2022 Knuth Project
+# Copyright (c) 2019-2023 Knuth Project
 #
 
 from setuptools import setup
 from setuptools.command.install import install
 import subprocess
 import os
 
 __title__ = "microarch"
 __summary__ = "Knuth Microarchitecture Management (CPUID)"
 __uri__ = "https://github.com/k-nuth/microarch"
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 __author__ = "Fernando Pelliccioni"
 __email__ = "fpelliccioni@gmail.com"
 __license__ = "MIT"
-__copyright__ = "Copyright (c) 2019-2022 Knuth Project"
+__copyright__ = "Copyright (c) 2019-2023 Knuth Project"
 
 
 install_requires = [
     "cpuid >= 0.0.9",
 ]
 
 class PostInstallCommand(install):
```

