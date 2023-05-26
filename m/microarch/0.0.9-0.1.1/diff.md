# Comparing `tmp/microarch-0.0.9.tar.gz` & `tmp/microarch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microarch-0.0.9.tar", last modified: Mon Jan  9 17:38:59 2023, max compression
+gzip compressed data, was "microarch-0.1.1.tar", last modified: Fri May 26 14:13:37 2023, max compression
```

## Comparing `microarch-0.0.9.tar` & `microarch-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 17:38:59.830041 microarch-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-01-09 17:38:42.000000 microarch-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-01-09 17:38:59.830041 microarch-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-01-09 17:38:42.000000 microarch-0.0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 17:38:59.830041 microarch-0.0.9/microarch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-01-09 17:38:59.000000 microarch-0.0.9/microarch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-01-09 17:38:59.000000 microarch-0.0.9/microarch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-01-09 17:38:59.000000 microarch-0.0.9/microarch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-01-09 17:38:59.000000 microarch-0.0.9/microarch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-01-09 17:38:59.000000 microarch-0.0.9/microarch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    97922 2023-01-09 17:38:42.000000 microarch-0.0.9/microarch.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-09 17:38:59.830041 microarch-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2587 2023-01-09 17:38:42.000000 microarch-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:13:37.253763 microarch-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-05-26 14:13:18.000000 microarch-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-05-26 14:13:37.253763 microarch-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-05-26 14:13:18.000000 microarch-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:13:37.253763 microarch-0.1.1/microarch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-05-26 14:13:37.000000 microarch-0.1.1/microarch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-26 14:13:37.000000 microarch-0.1.1/microarch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-26 14:13:37.000000 microarch-0.1.1/microarch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-26 14:13:37.000000 microarch-0.1.1/microarch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-26 14:13:37.000000 microarch-0.1.1/microarch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)   102971 2023-05-26 14:13:18.000000 microarch-0.1.1/microarch.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-26 14:13:37.253763 microarch-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2587 2023-05-26 14:13:18.000000 microarch-0.1.1/setup.py
```

### Comparing `microarch-0.0.9/LICENSE` & `microarch-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `microarch-0.0.9/PKG-INFO` & `microarch-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microarch
-Version: 0.0.9
+Version: 0.1.1
 Summary: Knuth Microarchitecture Management (CPUID)
 Home-page: https://github.com/k-nuth/microarch
 Author: Fernando Pelliccioni
 Author-email: fpelliccioni@gmail.com
 License: MIT
 Keywords: knuth kth crypto bitcoin btc bch cash build tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `microarch-0.0.9/microarch.egg-info/PKG-INFO` & `microarch-0.1.1/microarch.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microarch
-Version: 0.0.9
+Version: 0.1.1
 Summary: Knuth Microarchitecture Management (CPUID)
 Home-page: https://github.com/k-nuth/microarch
 Author: Fernando Pelliccioni
 Author-email: fpelliccioni@gmail.com
 License: MIT
 Keywords: knuth kth crypto bitcoin btc bch cash build tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `microarch-0.0.9/microarch.py` & `microarch-0.1.1/microarch.py`

 * *Files 2% similar despite different names*

```diff
@@ -826,14 +826,75 @@
 # AMX: Tile computation on 8-bit integers
 def support_amxint8_cpu():
     if max_function_id() < 0x00000007: return False
     _, _, _, d = cpuid.cpuid_count(0x00000007, 0)
     return (d & (1 << 25)) != 0
 
 # -----------------------------------------------------------------
+# Supported in GCC13
+# -----------------------------------------------------------------
+
+# Intel AVX-IFMA: AVX Integer Fused Multiply-Add Instructions
+# Packed Multiply of Unsigned 52-Bit Integers and Add the High 52-Bit Products to Qword Accumulators.
+# Introduced in Sierra Forest and Grand Ridge.
+def support_avxifma_cpu():
+    if max_function_id() < 0x00000007: return False
+    a, _, _, _ = cpuid.cpuid_count(0x00000007, 1)
+    return (a & (1 << 23)) != 0
+
+# Intel AVX-VNNI-INT8. AVX Vector Neural Network Instructions (VEX encoded).
+# Multiply and Add Unsigned and Signed Bytes With and Without Saturation
+# Introduced in Sierra Forest and Grand Ridge.
+def support_avxvnniint8_cpu():
+    if max_function_id() < 0x00000007: return False
+    _, _, _, d = cpuid.cpuid_count(0x00000007, 1)
+    return (d & (1 << 4)) != 0
+
+# Intel AVX-NE-CONVERT. Load BF16 Element and Convert to FP32 Element With Broadcast.
+# Introduced in Sierra Forest and Grand Ridge.
+def support_avxneconvert_cpu():
+    if max_function_id() < 0x00000007: return False
+    _, _, _, d = cpuid.cpuid_count(0x00000007, 1)
+    return (d & (1 << 5)) != 0
+
+# Intel CMPccXADD: Compare and Add if Condition is Met.
+# Introduced in Sierra Forest and Grand Ridge.
+def support_cmpccxadd_cpu():
+    if max_function_id() < 0x00000007: return False
+    a, _, _, _ = cpuid.cpuid_count(0x00000007, 1)
+    return (a & (1 << 7)) != 0
+
+# Intel AMX-FP16: Matrix multiply FP16 elements. Tile computational operations on FP16 numbers.
+# Introduced in  Granite Rapids.
+def support_amx_fp16_cpu():
+    if max_function_id() < 0x00000007: return False
+    a, _, _, _ = cpuid.cpuid_count(0x00000007, 1)
+    return (a & (1 << 21)) != 0
+
+# Intel prefetchi: Prefetch Code Into Caches
+def support_prefetchi_cpu():
+    if max_function_id() < 0x00000007: return False
+    _, _, _, d = cpuid.cpuid_count(0x00000007, 1)
+    return (d & (1 << 14)) != 0
+
+# Intel RAO-INT: New atomic instructions: AADD, AAND, AOR, AXOR.
+# Introduced in Grand Ridge.
+def support_raoint_cpu():
+    if max_function_id() < 0x00000007: return False
+    a, _, _, _ = cpuid.cpuid_count(0x00000007, 1)
+    return (a & (1 << 3)) != 0
+
+# Intel AMX-COMPLEX: Advanced Matrix Extensions for Complex numbers.
+# Introduced in Granite Rapids.
+def support_amx_complex_cpu():
+    if max_function_id() < 0x00000007: return False
+    _, _, _, d = cpuid.cpuid_count(0x00000007, 1)
+    return (d & (1 << 8)) != 0
+
+# -----------------------------------------------------------------
 
 def version_bit(i):
     global KTH_MARCH_BUILD_VERSION_BITS
     return lambda: KTH_MARCH_BUILD_VERSION_BITS[i]
 
 
 extensions_map = [
@@ -970,14 +1031,23 @@
     support_xgetbv_ecx1_cpu,
     support_umip,
     support_sgx_lc,
     support_mcommit,
     support_rdpru,
     support_invpcid,
     support_sev_snp,
+
+    support_avxifma_cpu,
+    support_avxvnniint8_cpu,
+    support_avxneconvert_cpu,
+    support_cmpccxadd_cpu,
+    support_amx_fp16_cpu,
+    support_prefetchi_cpu,
+    support_raoint_cpu,
+    support_amx_complex_cpu,
 ]
 
 extensions_names = [
     None,       # Version Bit 1
     None,       # Version Bit 0
     None,       # Version Bit 1
     None,       # Version Bit 0
@@ -1109,14 +1179,23 @@
     "XGETBV_ECX1",
     "UMIP",
     "SGX_LC",
     "MCOMMIT",
     "RDPRU",
     "INVPCID",
     "SEV_SNP",
+
+    "AVX-IFMA",
+    "AVX-VNNI-INT8",
+    "AVX-NE-CONVERT",
+    "CMPCCXADD",
+    "AMX-FP16",
+    "PREFETCHI",
+    "RAO-INT",
+    "AMX-COMPLEX",
 ]
 
 extensions_kth_defines = [
     None,       # Version Bit 1
     None,       # Version Bit 0
     None,       # Version Bit 1
     None,       # Version Bit 0
@@ -1248,14 +1327,23 @@
     "-DKTH_EXT_XGETBV_ECX1",
     "-DKTH_EXT_UMIP",
     "-DKTH_EXT_SGX_LC",
     "-DKTH_EXT_MCOMMIT",
     "-DKTH_EXT_RDPRU",
     "-DKTH_EXT_INVPCID",
     "-DKTH_EXT_SEV_SNP",
+
+    "-DKTH_EXT_AVX_IFMA",
+    "-DKTH_EXT_AVX_VNNI_INT8",
+    "-DKTH_EXT_AVX_NE_CONVERT",
+    "-DKTH_EXT_CMPCCXADD",
+    "-DKTH_EXT_AMX_FP16",
+    "-DKTH_EXT_PREFETCHI",
+    "-DKTH_EXT_RAO_INT",
+    "-DKTH_EXT_AMX_COMPLEX",
 ]
 
 
 extensions_flags = {
     'gcc':         None,
     'apple-clang': None,
     'clang':       None,
@@ -1397,14 +1485,23 @@
     None,                      # "xgetbv_ecx1"
     None,                      # "umip"
     None,                      # "sgx_lc"
     None,                      # "mcommit"
     None,                      # "rdpru"
     None,                      # "invpcid"
     None,                      # "sev_snp"
+
+    {'min_version': 13, 'flags': "-mavxifma"},
+    {'min_version': 13, 'flags': "-mavxvnniint8"},
+    {'min_version': 13, 'flags': "-mavxneconvert"},
+    {'min_version': 13, 'flags': "-mcmpccxadd"},
+    {'min_version': 13, 'flags': "-mamx-fp16"},
+    {'min_version': 13, 'flags': "-mprefetchi"},
+    {'min_version': 13, 'flags': "-mraoint"},
+    {'min_version': 13, 'flags': "-mamx-complex"},
 ]
 
 extensions_flags['clang'] = [
     None,                        # Version Bit 1
     None,                        # Version Bit 0
     None,                        # Version Bit 1
     None,                        # Version Bit 0
@@ -1534,14 +1631,23 @@
     None,                      # "xgetbv_ecx1"
     None,                      # "umip"
     None,                      # "sgx_lc"
     None,                      # "mcommit"
     None,                      # "rdpru"
     None,                      # "invpcid"
     None,                      # "sev_snp"
+
+    None,                      # "-mavxifma"
+    None,                      # "-mavxvnniint8"
+    None,                      # "-mavxneconvert"
+    None,                      # "-mcmpccxadd"
+    None,                      # "-mamx-fp16"
+    None,                      # "-mprefetchi"
+    None,                      # "-mraoint"
+    None,                      # "-mamx-complex"
 ]
 
 extensions_flags['apple-clang'] = [
     None,                        # Version Bit 1
     None,                        # Version Bit 0
     None,                        # Version Bit 1
     None,                        # Version Bit 0
@@ -1671,14 +1777,23 @@
     None,                      # "xgetbv_ecx1"
     None,                      # "umip"
     None,                      # "sgx_lc"
     None,                      # "mcommit"
     None,                      # "rdpru"
     None,                      # "invpcid"
     None,                      # "sev_snp"
+
+    None,                      # "-mavxifma"
+    None,                      # "-mavxvnniint8"
+    None,                      # "-mavxneconvert"
+    None,                      # "-mcmpccxadd"
+    None,                      # "-mamx-fp16"
+    None,                      # "-mprefetchi"
+    None,                      # "-mraoint"
+    None,                      # "-mamx-complex"
 ]
 
 # https://docs.microsoft.com/en-us/cpp/build/reference/arch-x64?view=msvc-170
 extensions_flags['msvc'] = [
     None,                        # Version Bit 1
     None,                        # Version Bit 0
     None,                        # Version Bit 1
@@ -1809,14 +1924,23 @@
     None,                                                    # xgetbv_ecx1
     None,                                                    # umip
     None,                                                    # sgx_lc
     None,                                                    # mcommit
     None,                                                    # rdpru
     None,                                                    # invpcid
     None,                                                    # sev_snp
+
+    None,                                                    # "-mavxifma"
+    None,                                                    # "-mavxvnniint8"
+    None,                                                    # "-mavxneconvert"
+    None,                                                    # "-mcmpccxadd"
+    None,                                                    # "-mamx-fp16"
+    None,                                                    # "-mprefetchi"
+    None,                                                    # "-mraoint"
+    None,                                                    # "-mamx-complex"
 ]
 
 def get_available_extensions():
     data = []
     for f in extensions_map:
         data.append(int(f()))
 
@@ -2224,14 +2348,15 @@
 def get_all_data_from_marchid(marchid, os, comp, comp_ver):
     user_exts = decode_extensions(marchid)
     user_names = None
     user_flags = None
     user_exts_filtered = None
     user_marchid_valid = False
     user_exts_compiler_compatible = None
+    user_kth_defs = None
 
     if user_exts is not None:
         version_bits = get_version_bits()
         exts_version = user_exts[:len(version_bits)]
 
         if version_bits == exts_version:
             user_marchid_valid = True
@@ -2452,14 +2577,15 @@
 # https://gcc.gnu.org/onlinedocs/gcc-6.5.0/gcc/x86-Options.html#x86-Options
 # https://gcc.gnu.org/onlinedocs/gcc-7.5.0/gcc/x86-Options.html#x86-Options
 # https://gcc.gnu.org/onlinedocs/gcc-8.5.0/gcc/x86-Options.html#x86-Options
 # https://gcc.gnu.org/onlinedocs/gcc-9.5.0/gcc/x86-Options.html#x86-Options
 # https://gcc.gnu.org/onlinedocs/gcc-10.4.0/gcc/x86-Options.html#x86-Options
 # https://gcc.gnu.org/onlinedocs/gcc-11.3.0/gcc/x86-Options.html#x86-Options
 # https://gcc.gnu.org/onlinedocs/gcc-12.1.0/gcc/x86-Options.html#x86-Options
+# https://gcc.gnu.org/onlinedocs/gcc-13.1.0/gcc/x86-Options.html
 
 # ------------------------------------------------------------------------------------------------
 
 # https://github.com/pixelb/scripts/blob/master/scripts/gcccpuopt
```

### Comparing `microarch-0.0.9/setup.py` & `microarch-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 from setuptools.command.install import install
 import subprocess
 import os
 
 __title__ = "microarch"
 __summary__ = "Knuth Microarchitecture Management (CPUID)"
 __uri__ = "https://github.com/k-nuth/microarch"
-__version__ = "0.0.9"
+__version__ = "0.1.1"
 __author__ = "Fernando Pelliccioni"
 __email__ = "fpelliccioni@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2019-2023 Knuth Project"
 
 
 install_requires = [
-    "cpuid >= 0.0.9",
+    "cpuid >= 0.0.1",
 ]
 
 class PostInstallCommand(install):
     """Override Install
     """
     def run(self):
         install.run(self)
```

