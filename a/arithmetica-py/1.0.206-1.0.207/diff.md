# Comparing `tmp/arithmetica-py-1.0.206.tar.gz` & `tmp/arithmetica-py-1.0.207.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arithmetica-py-1.0.206.tar", last modified: Sun May 14 18:33:13 2023, max compression
+gzip compressed data, was "arithmetica-py-1.0.207.tar", last modified: Fri May 26 21:08:32 2023, max compression
```

## Comparing `arithmetica-py-1.0.206.tar` & `arithmetica-py-1.0.207.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:33:13.879999 arithmetica-py-1.0.206/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-14 18:32:46.000000 arithmetica-py-1.0.206/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 18:33:13.879999 arithmetica-py-1.0.206/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-05-14 18:32:46.000000 arithmetica-py-1.0.206/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:33:13.879999 arithmetica-py-1.0.206/arithmetica_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 18:33:13.000000 arithmetica-py-1.0.206/arithmetica_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-14 18:33:13.000000 arithmetica-py-1.0.206/arithmetica_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:33:13.000000 arithmetica-py-1.0.206/arithmetica_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-14 18:33:13.000000 arithmetica-py-1.0.206/arithmetica_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 18:33:13.879999 arithmetica-py-1.0.206/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-14 18:32:46.000000 arithmetica-py-1.0.206/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:33:13.875999 arithmetica-py-1.0.206/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:33:13.879999 arithmetica-py-1.0.206/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)   184894 2023-05-14 18:33:13.000000 arithmetica-py-1.0.206/src/python-module/libarithmetica.a
--rw-r--r--   0 runner    (1001) docker     (123)    75112 2023-05-14 18:33:13.000000 arithmetica-py-1.0.206/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-05-14 18:32:46.000000 arithmetica-py-1.0.206/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-14 18:33:13.000000 arithmetica-py-1.0.206/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:08:32.248847 arithmetica-py-1.0.207/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-26 21:08:13.000000 arithmetica-py-1.0.207/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 21:08:32.248847 arithmetica-py-1.0.207/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-05-26 21:08:13.000000 arithmetica-py-1.0.207/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:08:32.248847 arithmetica-py-1.0.207/arithmetica_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 21:08:32.000000 arithmetica-py-1.0.207/arithmetica_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-26 21:08:32.000000 arithmetica-py-1.0.207/arithmetica_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:08:32.000000 arithmetica-py-1.0.207/arithmetica_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 21:08:32.000000 arithmetica-py-1.0.207/arithmetica_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:08:32.248847 arithmetica-py-1.0.207/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-26 21:08:13.000000 arithmetica-py-1.0.207/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:08:32.248847 arithmetica-py-1.0.207/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:08:32.248847 arithmetica-py-1.0.207/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)   185158 2023-05-26 21:08:32.000000 arithmetica-py-1.0.207/src/python-module/libarithmetica.a
+-rw-r--r--   0 runner    (1001) docker     (123)    75112 2023-05-26 21:08:32.000000 arithmetica-py-1.0.207/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-05-26 21:08:13.000000 arithmetica-py-1.0.207/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 21:08:32.000000 arithmetica-py-1.0.207/src/python-module/version.txt
```

### Comparing `arithmetica-py-1.0.206/LICENSE` & `arithmetica-py-1.0.207/LICENSE`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.206/README.md` & `arithmetica-py-1.0.207/README.md`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.206/setup.py` & `arithmetica-py-1.0.207/setup.py`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.206/src/python-module/libarithmetica.a` & `arithmetica-py-1.0.207/src/python-module/libarithmetica.a`

 * *Files 1% similar despite different names*

#### nm -s {}

```diff
@@ -514,19 +514,20 @@
                  U malloc
                  U memcpy
                  U memmove
                  U strlen
 0000000000000000 T terminating_decimal_to_fraction
 
 Fraction.cpp.o:
-0000000000000017 r .LC12
-000000000000001a r .LC13
+0000000000000019 r .LC13
+000000000000001c r .LC14
 0000000000000000 r .LC4
 0000000000000000 r .LC5
-0000000000000015 r .LC6
+0000000000000002 r .LC6
+0000000000000017 r .LC7
 0000000000000000 V DW.ref.__gxx_personality_v0
                  U _Unwind_Resume
 00000000000002a0 T _ZN11arithmetica8Fraction9to_stringB5cxx11Ev
 00000000000000d0 t _ZN11arithmetica8Fraction9to_stringB5cxx11Ev.cold
 0000000000000150 T _ZN11arithmetica8FractionC1EPKc
 0000000000000200 T _ZN11arithmetica8FractionC1ERK8fraction
 00000000000000a0 T _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
@@ -540,34 +541,35 @@
 0000000000000034 t _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE.cold
 0000000000000030 T _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_
 0000000000000000 t _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_.cold
 0000000000000000 T _ZN11arithmetica8FractionC2Ev
 0000000000000000 W _ZN11arithmetica8FractionD1Ev
 0000000000000000 W _ZN11arithmetica8FractionD2Ev
 0000000000000000 n _ZN11arithmetica8FractionD5Ev
-0000000000000da0 T _ZN11arithmetica8FractiondvERKS0_
-00000000000001bc t _ZN11arithmetica8FractiondvERKS0_.cold
-00000000000010b0 T _ZN11arithmetica8FractioneqERKS0_
-0000000000000780 T _ZN11arithmetica8FractionmiERKS0_
-0000000000000134 t _ZN11arithmetica8FractionmiERKS0_.cold
-0000000000000a90 T _ZN11arithmetica8FractionmlERKS0_
-0000000000000178 t _ZN11arithmetica8FractionmlERKS0_.cold
-0000000000000470 T _ZN11arithmetica8FractionplERKS0_
-00000000000000f0 t _ZN11arithmetica8FractionplERKS0_.cold
+0000000000000db0 T _ZN11arithmetica8FractiondvERKS0_
+00000000000001d4 t _ZN11arithmetica8FractiondvERKS0_.cold
+00000000000010c0 T _ZN11arithmetica8FractioneqERKS0_
+0000000000000790 T _ZN11arithmetica8FractionmiERKS0_
+000000000000014c t _ZN11arithmetica8FractionmiERKS0_.cold
+0000000000000aa0 T _ZN11arithmetica8FractionmlERKS0_
+0000000000000190 t _ZN11arithmetica8FractionmlERKS0_.cold
+0000000000000480 T _ZN11arithmetica8FractionplERKS0_
+0000000000000108 t _ZN11arithmetica8FractionplERKS0_.cold
                  U _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc
                  U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm
+                 U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7reserveEm
                  U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm
                  U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_
                  U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm
                  U _ZSt19__throw_logic_errorPKc
                  U _ZSt20__throw_length_errorPKc
                  U _ZdlPvm
-0000000000001180 T _ZeqRKN11arithmetica8FractionES2_
-0000000000001250 T _ZltRKN11arithmetica8FractionES2_
-0000000000000200 t _ZltRKN11arithmetica8FractionES2_.cold
+0000000000001190 T _ZeqRKN11arithmetica8FractionES2_
+0000000000001260 T _ZltRKN11arithmetica8FractionES2_
+0000000000000218 t _ZltRKN11arithmetica8FractionES2_.cold
                  U __gxx_personality_v0
                  U __stack_chk_fail
                  U add_fraction
                  U calloc
                  U delete_fraction
                  U memcmp
                  U memcpy
```

#### file list

```diff
@@ -18,15 +18,15 @@
 ?rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 power_integer.c.o
 ?rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 repeating_decimal_to_fraction.c.o
 ?rw-r--r--   0        0        0    18192 1970-01-01 00:00:00.000000 simplify_arithmetic_expression.c.o
 ?rw-r--r--   0        0        0     4712 1970-01-01 00:00:00.000000 sine.c.o
 ?rw-r--r--   0        0        0     4736 1970-01-01 00:00:00.000000 square_root.c.o
 ?rw-r--r--   0        0        0     1808 1970-01-01 00:00:00.000000 tangent.c.o
 ?rw-r--r--   0        0        0     2856 1970-01-01 00:00:00.000000 terminating_decimal_to_fraction.c.o
-?rw-r--r--   0        0        0    19760 1970-01-01 00:00:00.000000 Fraction.cpp.o
+?rw-r--r--   0        0        0    20024 1970-01-01 00:00:00.000000 Fraction.cpp.o
 ?rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 fraction.c.o
 ?rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 add_fraction.c.o
 ?rw-r--r--   0        0        0     1944 1970-01-01 00:00:00.000000 multiply_fraction.c.o
 ?rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 parse_fraction.c.o
 ?rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 power_fraction.c.o
 ?rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 simplify_parsed_fraction.c.o
 ?rw-r--r--   0        0        0     2336 1970-01-01 00:00:00.000000 subtract_fraction.c.o
```

#### Fraction.cpp.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          18224 (bytes into file)
+  Start of section headers:          18488 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         24
   Section header string table index: 23
```

##### readelf --wide --sections {}

```diff
@@ -1,33 +1,33 @@
-There are 24 section headers, starting at offset 0x4730:
+There are 24 section headers, starting at offset 0x4838:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .group            GROUP           0000000000000000 000040 00000c 04     21  21  4
-  [ 2] .group            GROUP           0000000000000000 00004c 00000c 04     21  25  4
-  [ 3] .text             PROGBITS        0000000000000000 000060 0014cf 00  AX  0   0 16
-  [ 4] .rela.text        RELA            0000000000000000 002d40 001128 18   I 21   3  8
-  [ 5] .data             PROGBITS        0000000000000000 00152f 000000 00  WA  0   0  1
-  [ 6] .bss              NOBITS          0000000000000000 00152f 000000 00  WA  0   0  1
-  [ 7] .text.unlikely    PROGBITS        0000000000000000 001530 000230 00  AX  0   0  2
-  [ 8] .rela.text.unlikely RELA            0000000000000000 003e68 000330 18   I 21   7  8
-  [ 9] .gcc_except_table PROGBITS        0000000000000000 001760 00015a 00   A  0   0  1
-  [10] .rodata.str1.8    PROGBITS        0000000000000000 0018c0 00002a 01 AMS  0   0  8
-  [11] .rodata.str1.1    PROGBITS        0000000000000000 0018ea 00001c 01 AMS  0   0  1
-  [12] .text._ZN11arithmetica8FractionD2Ev PROGBITS        0000000000000000 001910 000042 00 AXG  0   0 16
-  [13] .rela.text._ZN11arithmetica8FractionD2Ev RELA            0000000000000000 004198 000030 18  IG 21  12  8
-  [14] .data.rel.local.DW.ref.__gxx_personality_v0 PROGBITS        0000000000000000 001958 000008 00 WAG  0   0  8
-  [15] .rela.data.rel.local.DW.ref.__gxx_personality_v0 RELA            0000000000000000 0041c8 000018 18  IG 21  14  8
-  [16] .comment          PROGBITS        0000000000000000 001960 00002c 01  MS  0   0  1
-  [17] .note.GNU-stack   PROGBITS        0000000000000000 00198c 000000 00      0   0  1
-  [18] .note.gnu.property NOTE            0000000000000000 001990 000020 00   A  0   0  8
-  [19] .eh_frame         PROGBITS        0000000000000000 0019b0 000588 00   A  0   0  8
-  [20] .rela.eh_frame    RELA            0000000000000000 0041e0 000438 18   I 21  19  8
-  [21] .symtab           SYMTAB          0000000000000000 001f38 000600 18     22  22  8
-  [22] .strtab           STRTAB          0000000000000000 002538 000803 00      0   0  1
-  [23] .shstrtab         STRTAB          0000000000000000 004618 000111 00      0   0  1
+  [ 1] .group            GROUP           0000000000000000 000040 00000c 04     21  22  4
+  [ 2] .group            GROUP           0000000000000000 00004c 00000c 04     21  26  4
+  [ 3] .text             PROGBITS        0000000000000000 000060 0014df 00  AX  0   0 16
+  [ 4] .rela.text        RELA            0000000000000000 002dd0 001188 18   I 21   3  8
+  [ 5] .data             PROGBITS        0000000000000000 00153f 000000 00  WA  0   0  1
+  [ 6] .bss              NOBITS          0000000000000000 00153f 000000 00  WA  0   0  1
+  [ 7] .text.unlikely    PROGBITS        0000000000000000 001540 000248 00  AX  0   0  2
+  [ 8] .rela.text.unlikely RELA            0000000000000000 003f58 000348 18   I 21   7  8
+  [ 9] .gcc_except_table PROGBITS        0000000000000000 001788 00015f 00   A  0   0  1
+  [10] .rodata.str1.8    PROGBITS        0000000000000000 0018e8 00002a 01 AMS  0   0  8
+  [11] .rodata.str1.1    PROGBITS        0000000000000000 001912 00001e 01 AMS  0   0  1
+  [12] .text._ZN11arithmetica8FractionD2Ev PROGBITS        0000000000000000 001930 000042 00 AXG  0   0 16
+  [13] .rela.text._ZN11arithmetica8FractionD2Ev RELA            0000000000000000 0042a0 000030 18  IG 21  12  8
+  [14] .data.rel.local.DW.ref.__gxx_personality_v0 PROGBITS        0000000000000000 001978 000008 00 WAG  0   0  8
+  [15] .rela.data.rel.local.DW.ref.__gxx_personality_v0 RELA            0000000000000000 0042d0 000018 18  IG 21  14  8
+  [16] .comment          PROGBITS        0000000000000000 001980 00002c 01  MS  0   0  1
+  [17] .note.GNU-stack   PROGBITS        0000000000000000 0019ac 000000 00      0   0  1
+  [18] .note.gnu.property NOTE            0000000000000000 0019b0 000020 00   A  0   0  8
+  [19] .eh_frame         PROGBITS        0000000000000000 0019d0 000588 00   A  0   0  8
+  [20] .rela.eh_frame    RELA            0000000000000000 0042e8 000438 18   I 21  19  8
+  [21] .symtab           SYMTAB          0000000000000000 001f58 000630 18     22  23  8
+  [22] .strtab           STRTAB          0000000000000000 002588 000848 00      0   0  1
+  [23] .shstrtab         STRTAB          0000000000000000 004720 000111 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,67 +1,69 @@
 
-Symbol table '.symtab' contains 64 entries:
+Symbol table '.symtab' contains 66 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS Fraction.cpp
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    3 .text
      3: 0000000000000000     0 SECTION LOCAL  DEFAULT    7 .text.unlikely
      4: 0000000000000000     0 SECTION LOCAL  DEFAULT    9 .gcc_except_table
      5: 0000000000000000    51 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_.cold
      6: 0000000000000034    51 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE.cold
      7: 0000000000000068    51 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionC2EPKc.cold
      8: 000000000000009c    51 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionC2ERK8fraction.cold
-     9: 00000000000000d0    32 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8Fraction9to_stringB5cxx11Ev.cold
+     9: 00000000000000d0    55 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8Fraction9to_stringB5cxx11Ev.cold
     10: 0000000000000000     0 SECTION LOCAL  DEFAULT   12 .text._ZN11arithmetica8FractionD2Ev
-    11: 00000000000000f0    68 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionplERKS0_.cold
-    12: 0000000000000134    68 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionmiERKS0_.cold
-    13: 0000000000000178    68 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionmlERKS0_.cold
-    14: 00000000000001bc    68 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractiondvERKS0_.cold
-    15: 0000000000000200    48 FUNC    LOCAL  DEFAULT    7 _ZltRKN11arithmetica8FractionES2_.cold
-    16: 0000000000000015     0 NOTYPE  LOCAL  DEFAULT   11 .LC6
-    17: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT   10 .LC4
-    18: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT   11 .LC5
-    19: 0000000000000017     0 NOTYPE  LOCAL  DEFAULT   11 .LC12
-    20: 000000000000001a     0 NOTYPE  LOCAL  DEFAULT   11 .LC13
-    21: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT    1 _ZN11arithmetica8FractionD5Ev
-    22: 0000000000000000    44 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2Ev
-    23: 0000000000000000    44 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1Ev
-    24: 0000000000000030    98 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_
-    25: 0000000000000000     8 OBJECT  WEAK   HIDDEN    14 DW.ref.__gxx_personality_v0
-    26: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_
-    27: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND __gxx_personality_v0
-    28: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZdlPvm
-    29: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Unwind_Resume
-    30: 0000000000000030    98 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_
-    31: 00000000000000a0   172 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
-    32: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND parse_fraction
-    33: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen
-    34: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm
-    35: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND delete_fraction
-    36: 00000000000000a0   172 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
-    37: 0000000000000150   172 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2EPKc
-    38: 0000000000000150   172 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1EPKc
-    39: 0000000000000200   155 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2ERK8fraction
-    40: 0000000000000200   155 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1ERK8fraction
-    41: 00000000000002a0   458 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8Fraction9to_stringB5cxx11Ev
-    42: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm
-    43: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm
-    44: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcpy
-    45: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZSt19__throw_logic_errorPKc
-    46: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZSt20__throw_length_errorPKc
-    47: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND __stack_chk_fail
-    48: 0000000000000000    66 FUNC    WEAK   DEFAULT   12 _ZN11arithmetica8FractionD2Ev
-    49: 0000000000000000    66 FUNC    WEAK   DEFAULT   12 _ZN11arithmetica8FractionD1Ev
-    50: 0000000000000470   780 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionplERKS0_
-    51: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND calloc
-    52: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strcpy
-    53: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND add_fraction
-    54: 0000000000000780   780 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionmiERKS0_
-    55: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND subtract_fraction
-    56: 0000000000000a90   780 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionmlERKS0_
-    57: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND multiply_fraction
-    58: 0000000000000da0   780 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractiondvERKS0_
-    59: 00000000000010b0   207 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractioneqERKS0_
-    60: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc
-    61: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcmp
-    62: 0000000000001180   207 FUNC    GLOBAL DEFAULT    3 _ZeqRKN11arithmetica8FractionES2_
-    63: 0000000000001250   639 FUNC    GLOBAL DEFAULT    3 _ZltRKN11arithmetica8FractionES2_
+    11: 0000000000000108    68 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionplERKS0_.cold
+    12: 000000000000014c    68 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionmiERKS0_.cold
+    13: 0000000000000190    68 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionmlERKS0_.cold
+    14: 00000000000001d4    68 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractiondvERKS0_.cold
+    15: 0000000000000218    48 FUNC    LOCAL  DEFAULT    7 _ZltRKN11arithmetica8FractionES2_.cold
+    16: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT   11 .LC5
+    17: 0000000000000017     0 NOTYPE  LOCAL  DEFAULT   11 .LC7
+    18: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT   10 .LC4
+    19: 0000000000000002     0 NOTYPE  LOCAL  DEFAULT   11 .LC6
+    20: 0000000000000019     0 NOTYPE  LOCAL  DEFAULT   11 .LC13
+    21: 000000000000001c     0 NOTYPE  LOCAL  DEFAULT   11 .LC14
+    22: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT    1 _ZN11arithmetica8FractionD5Ev
+    23: 0000000000000000    44 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2Ev
+    24: 0000000000000000    44 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1Ev
+    25: 0000000000000030    98 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_
+    26: 0000000000000000     8 OBJECT  WEAK   HIDDEN    14 DW.ref.__gxx_personality_v0
+    27: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_
+    28: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND __gxx_personality_v0
+    29: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZdlPvm
+    30: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Unwind_Resume
+    31: 0000000000000030    98 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_
+    32: 00000000000000a0   172 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
+    33: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND parse_fraction
+    34: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen
+    35: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm
+    36: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND delete_fraction
+    37: 00000000000000a0   172 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
+    38: 0000000000000150   172 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2EPKc
+    39: 0000000000000150   172 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1EPKc
+    40: 0000000000000200   155 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2ERK8fraction
+    41: 0000000000000200   155 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1ERK8fraction
+    42: 00000000000002a0   466 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8Fraction9to_stringB5cxx11Ev
+    43: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc
+    44: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm
+    45: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcpy
+    46: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7reserveEm
+    47: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm
+    48: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZSt19__throw_logic_errorPKc
+    49: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND __stack_chk_fail
+    50: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZSt20__throw_length_errorPKc
+    51: 0000000000000000    66 FUNC    WEAK   DEFAULT   12 _ZN11arithmetica8FractionD2Ev
+    52: 0000000000000000    66 FUNC    WEAK   DEFAULT   12 _ZN11arithmetica8FractionD1Ev
+    53: 0000000000000480   780 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionplERKS0_
+    54: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND calloc
+    55: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strcpy
+    56: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND add_fraction
+    57: 0000000000000790   780 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionmiERKS0_
+    58: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND subtract_fraction
+    59: 0000000000000aa0   780 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionmlERKS0_
+    60: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND multiply_fraction
+    61: 0000000000000db0   780 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractiondvERKS0_
+    62: 00000000000010c0   207 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractioneqERKS0_
+    63: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcmp
+    64: 0000000000001190   207 FUNC    GLOBAL DEFAULT    3 _ZeqRKN11arithmetica8FractionES2_
+    65: 0000000000001260   639 FUNC    GLOBAL DEFAULT    3 _ZltRKN11arithmetica8FractionES2_
```

##### readelf --wide --relocs {}

```diff
@@ -1,244 +1,249 @@
 
-Relocation section '.rela.text' at offset 0x2d40 contains 183 entries:
+Relocation section '.rela.text' at offset 0x2dd0 contains 187 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-000000000000006a  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_ - 4
-0000000000000079  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_ - 4
-00000000000000e0  0000002000000004 R_X86_64_PLT32         0000000000000000 parse_fraction - 4
-00000000000000ee  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000102  0000002200000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
-000000000000010e  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000122  0000002200000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
-000000000000012d  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000190  0000002000000004 R_X86_64_PLT32         0000000000000000 parse_fraction - 4
-000000000000019e  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000001b2  0000002200000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
-00000000000001be  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000001d2  0000002200000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
-00000000000001dd  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000246  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000258  0000002200000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
-0000000000000268  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-000000000000027c  0000002200000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
-0000000000000338  0000001000000002 R_X86_64_PC32          0000000000000015 .LC6 - 4
-0000000000000340  0000002a00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm - 4
-0000000000000350  0000002a00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm - 4
-00000000000003a6  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000003ed  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-000000000000040a  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000433  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-0000000000000438  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-000000000000043f  0000001200000002 R_X86_64_PC32          0000000000000000 .LC5 - 4
-0000000000000444  0000002e00000004 R_X86_64_PLT32         0000000000000000 _ZSt20__throw_length_errorPKc - 4
-0000000000000449  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-00000000000004ac  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000004c1  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000004d6  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000004eb  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000004fa  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000506  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000511  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000520  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000548  0000003500000004 R_X86_64_PLT32         0000000000000000 add_fraction - 4
-0000000000000559  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000569  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000584  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000005ce  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-00000000000005d3  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-00000000000005f4  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000637  0000001e00000004 R_X86_64_PLT32         0000000000000030 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ - 4
-000000000000064f  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000667  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000672  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-00000000000006cb  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-00000000000006e8  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000070b  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-000000000000072a  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000073e  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-0000000000000745  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-000000000000074a  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-00000000000007bc  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000007d1  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000007e6  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000007fb  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-000000000000080a  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000816  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000821  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000830  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000858  0000003700000004 R_X86_64_PLT32         0000000000000000 subtract_fraction - 4
-0000000000000869  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000879  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000894  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000008de  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-00000000000008e3  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000000904  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000947  0000001e00000004 R_X86_64_PLT32         0000000000000030 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ - 4
-000000000000095f  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000977  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000982  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-00000000000009db  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-00000000000009f8  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000a1b  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000a3a  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000a4e  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-0000000000000a55  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-0000000000000a5a  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000000acc  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000ae1  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000af6  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000b0b  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000b1a  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000b26  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000b31  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000b40  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000b68  0000003900000004 R_X86_64_PLT32         0000000000000000 multiply_fraction - 4
-0000000000000b79  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000b89  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000ba4  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000bee  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-0000000000000bf3  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000000c14  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000c57  0000001e00000004 R_X86_64_PLT32         0000000000000030 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ - 4
-0000000000000c6f  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000c87  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000c92  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000ceb  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000d08  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000d2b  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000d4a  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000d5e  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-0000000000000d65  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-0000000000000d6a  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000000ddc  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000df1  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000e06  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000e1b  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000e2a  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000e36  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000e42  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000e50  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000e78  0000003900000004 R_X86_64_PLT32         0000000000000000 multiply_fraction - 4
-0000000000000e89  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000e99  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000eb4  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000efe  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-0000000000000f03  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000000f24  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000f67  0000001e00000004 R_X86_64_PLT32         0000000000000030 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ - 4
-0000000000000f7f  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000f97  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000fa2  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000ffb  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000001018  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000103b  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-000000000000105a  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000106e  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-0000000000001075  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-000000000000107a  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-00000000000010b9  0000001300000002 R_X86_64_PC32          0000000000000017 .LC12 - 4
-00000000000010c2  0000001400000002 R_X86_64_PC32          000000000000001a .LC13 - 4
-00000000000010d6  0000003c00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
-00000000000010e5  0000003c00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
-00000000000010f8  0000003c00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
-000000000000112d  0000003d00000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
-0000000000001155  0000003d00000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
-0000000000001167  0000003c00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
-0000000000001189  0000001300000002 R_X86_64_PC32          0000000000000017 .LC12 - 4
-0000000000001192  0000001400000002 R_X86_64_PC32          000000000000001a .LC13 - 4
-00000000000011a6  0000003c00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
-00000000000011b5  0000003c00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
-00000000000011c8  0000003c00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
-00000000000011fd  0000003d00000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
-0000000000001225  0000003d00000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
-0000000000001237  0000003c00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
-0000000000001330  0000003600000004 R_X86_64_PLT32         0000000000000780 _ZN11arithmetica8FractionmiERKS0_ - 4
-0000000000001362  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000137f  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000001397  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000013af  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000141d  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-000000000000143a  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000145d  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-000000000000147a  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000001490  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-0000000000001495  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-000000000000149a  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-00000000000014a1  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-00000000000014a6  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+000000000000006a  0000001b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_ - 4
+0000000000000079  0000001b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_ - 4
+00000000000000e0  0000002100000004 R_X86_64_PLT32         0000000000000000 parse_fraction - 4
+00000000000000ee  0000002200000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000102  0000002300000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
+000000000000010e  0000002200000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000122  0000002300000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
+000000000000012d  0000002400000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000190  0000002100000004 R_X86_64_PLT32         0000000000000000 parse_fraction - 4
+000000000000019e  0000002200000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000001b2  0000002300000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
+00000000000001be  0000002200000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000001d2  0000002300000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
+00000000000001dd  0000002400000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000246  0000002200000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000258  0000002300000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
+0000000000000268  0000002200000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+000000000000027c  0000002300000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
+000000000000030e  0000001000000002 R_X86_64_PC32          0000000000000000 .LC5 - 4
+0000000000000318  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+000000000000036b  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000000387  0000002d00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000003c9  0000002e00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7reserveEm - 4
+00000000000003e6  0000001100000002 R_X86_64_PC32          0000000000000017 .LC7 - 4
+00000000000003ee  0000002f00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm - 4
+00000000000003fe  0000002f00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm - 4
+0000000000000410  0000002f00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm - 4
+000000000000042c  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000438  0000001200000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+000000000000043d  0000003000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000000442  0000003100000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+0000000000000449  0000001300000002 R_X86_64_PC32          0000000000000002 .LC6 - 4
+000000000000044e  0000003200000004 R_X86_64_PLT32         0000000000000000 _ZSt20__throw_length_errorPKc - 4
+00000000000004bc  0000003600000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000004d1  0000003600000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000004e6  0000003600000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000004fb  0000003600000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+000000000000050a  0000003700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000516  0000003700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000521  0000003700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000530  0000003700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000558  0000003800000004 R_X86_64_PLT32         0000000000000000 add_fraction - 4
+0000000000000569  0000002400000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000579  0000002400000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000594  0000002200000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000005de  0000001200000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+00000000000005e3  0000003000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000000604  0000002200000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000647  0000001f00000004 R_X86_64_PLT32         0000000000000030 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ - 4
+000000000000065f  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000677  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000682  0000002400000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+00000000000006db  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+00000000000006f8  0000002d00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000071b  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+000000000000073a  0000002d00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000074e  0000003100000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+0000000000000755  0000001200000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+000000000000075a  0000003000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+00000000000007cc  0000003600000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000007e1  0000003600000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000007f6  0000003600000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+000000000000080b  0000003600000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+000000000000081a  0000003700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000826  0000003700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000831  0000003700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000840  0000003700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000868  0000003a00000004 R_X86_64_PLT32         0000000000000000 subtract_fraction - 4
+0000000000000879  0000002400000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000889  0000002400000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+00000000000008a4  0000002200000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000008ee  0000001200000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+00000000000008f3  0000003000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000000914  0000002200000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000957  0000001f00000004 R_X86_64_PLT32         0000000000000030 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ - 4
+000000000000096f  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000987  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000992  0000002400000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+00000000000009eb  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000000a08  0000002d00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000a2b  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000000a4a  0000002d00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000a5e  0000003100000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+0000000000000a65  0000001200000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+0000000000000a6a  0000003000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000000adc  0000003600000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000af1  0000003600000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000b06  0000003600000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000b1b  0000003600000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000b2a  0000003700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000b36  0000003700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000b41  0000003700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000b50  0000003700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000b78  0000003c00000004 R_X86_64_PLT32         0000000000000000 multiply_fraction - 4
+0000000000000b89  0000002400000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000b99  0000002400000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000bb4  0000002200000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000bfe  0000001200000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+0000000000000c03  0000003000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000000c24  0000002200000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000c67  0000001f00000004 R_X86_64_PLT32         0000000000000030 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ - 4
+0000000000000c7f  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000c97  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000ca2  0000002400000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000cfb  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000000d18  0000002d00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000d3b  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000000d5a  0000002d00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000d6e  0000003100000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+0000000000000d75  0000001200000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+0000000000000d7a  0000003000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000000dec  0000003600000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000e01  0000003600000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000e16  0000003600000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000e2b  0000003600000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000e3a  0000003700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000e46  0000003700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000e52  0000003700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000e60  0000003700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000e88  0000003c00000004 R_X86_64_PLT32         0000000000000000 multiply_fraction - 4
+0000000000000e99  0000002400000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000ea9  0000002400000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000ec4  0000002200000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000f0e  0000001200000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+0000000000000f13  0000003000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000000f34  0000002200000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000f77  0000001f00000004 R_X86_64_PLT32         0000000000000030 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ - 4
+0000000000000f8f  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000fa7  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000fb2  0000002400000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+000000000000100b  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000001028  0000002d00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000104b  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+000000000000106a  0000002d00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000107e  0000003100000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+0000000000001085  0000001200000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+000000000000108a  0000003000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+00000000000010c9  0000001400000002 R_X86_64_PC32          0000000000000019 .LC13 - 4
+00000000000010d2  0000001500000002 R_X86_64_PC32          000000000000001c .LC14 - 4
+00000000000010e6  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+00000000000010f5  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+0000000000001108  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+000000000000113d  0000003f00000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
+0000000000001165  0000003f00000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
+0000000000001177  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+0000000000001199  0000001400000002 R_X86_64_PC32          0000000000000019 .LC13 - 4
+00000000000011a2  0000001500000002 R_X86_64_PC32          000000000000001c .LC14 - 4
+00000000000011b6  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+00000000000011c5  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+00000000000011d8  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+000000000000120d  0000003f00000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
+0000000000001235  0000003f00000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
+0000000000001247  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+0000000000001340  0000003900000004 R_X86_64_PLT32         0000000000000790 _ZN11arithmetica8FractionmiERKS0_ - 4
+0000000000001372  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000138f  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000013a7  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000013bf  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000142d  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+000000000000144a  0000002d00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000146d  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+000000000000148a  0000002d00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000014a0  0000001200000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+00000000000014a5  0000003000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+00000000000014aa  0000003100000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+00000000000014b1  0000001200000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+00000000000014b6  0000003000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
 000000000000008e  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely - 4
 0000000000000148  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 30
 00000000000001f8  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 64
 0000000000000297  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 98
-000000000000045a  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + cc
-0000000000000466  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + cc
-0000000000000760  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 104
-000000000000076c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + ec
-0000000000000778  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 11e
-0000000000000a70  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 148
-0000000000000a7c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 130
-0000000000000a88  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 162
-0000000000000d80  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 18c
-0000000000000d8c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 174
-0000000000000d98  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1a6
-0000000000001090  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1d0
-000000000000109c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1b8
-00000000000010a8  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1ea
-00000000000014bf  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1fc
-00000000000014cb  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 21c
+0000000000000462  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + cc
+000000000000046e  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + cc
+0000000000000770  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 11c
+000000000000077c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 104
+0000000000000788  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 136
+0000000000000a80  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 160
+0000000000000a8c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 148
+0000000000000a98  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 17a
+0000000000000d90  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1a4
+0000000000000d9c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 18c
+0000000000000da8  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1be
+00000000000010a0  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1e8
+00000000000010ac  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1d0
+00000000000010b8  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 202
+00000000000014cf  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 214
+00000000000014db  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 234
 
-Relocation section '.rela.text.unlikely' at offset 0x3e68 contains 34 entries:
+Relocation section '.rela.text.unlikely' at offset 0x3f58 contains 35 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000000012  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000027  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000002f  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-0000000000000046  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000005b  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000063  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-000000000000007a  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000008f  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000097  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-00000000000000ae  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000000c3  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000000cb  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-00000000000000e4  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000000ec  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-0000000000000104  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000011c  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000128  0000003100000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
-0000000000000130  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-0000000000000148  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000160  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000016c  0000003100000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
-0000000000000174  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-000000000000018c  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000001a4  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000001b0  0000003100000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
-00000000000001b8  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-00000000000001d0  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000001e8  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000001f4  0000003100000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
-00000000000001fc  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-0000000000000214  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000021c  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-0000000000000224  0000003100000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
-000000000000022c  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+0000000000000012  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000027  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000002f  0000001e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+0000000000000046  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000005b  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000063  0000001e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+000000000000007a  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000008f  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000097  0000001e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+00000000000000ae  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000000c3  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000000cb  0000001e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+00000000000000e4  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000000fb  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000103  0000001e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+000000000000011c  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000134  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000140  0000003400000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
+0000000000000148  0000001e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+0000000000000160  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000178  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000184  0000003400000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
+000000000000018c  0000001e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+00000000000001a4  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000001bc  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000001c8  0000003400000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
+00000000000001d0  0000001e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+00000000000001e8  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000200  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000020c  0000003400000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
+0000000000000214  0000001e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+000000000000022c  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000234  0000001e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+000000000000023c  0000003400000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
+0000000000000244  0000001e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
 
-Relocation section '.rela.text._ZN11arithmetica8FractionD2Ev' at offset 0x4198 contains 2 entries:
+Relocation section '.rela.text._ZN11arithmetica8FractionD2Ev' at offset 0x42a0 contains 2 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-000000000000001e  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000038  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000001e  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000038  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
 
-Relocation section '.rela.data.rel.local.DW.ref.__gxx_personality_v0' at offset 0x41c8 contains 1 entry:
+Relocation section '.rela.data.rel.local.DW.ref.__gxx_personality_v0' at offset 0x42d0 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000000000  0000001b00000001 R_X86_64_64            0000000000000000 __gxx_personality_v0 + 0
+0000000000000000  0000001c00000001 R_X86_64_64            0000000000000000 __gxx_personality_v0 + 0
 
-Relocation section '.rela.eh_frame' at offset 0x41e0 contains 45 entries:
+Relocation section '.rela.eh_frame' at offset 0x42e8 contains 45 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
-000000000000003f  0000001900000002 R_X86_64_PC32          0000000000000000 DW.ref.__gxx_personality_v0 + 0
+000000000000003f  0000001a00000002 R_X86_64_PC32          0000000000000000 DW.ref.__gxx_personality_v0 + 0
 0000000000000054  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 30
 000000000000005d  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 0
 0000000000000094  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 0
 000000000000009d  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 8
 00000000000000b8  0000000200000002 R_X86_64_PC32          0000000000000000 .text + a0
 00000000000000c1  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 10
 0000000000000108  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 34
@@ -250,31 +255,31 @@
 00000000000001a0  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 200
 00000000000001a9  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 32
 00000000000001f0  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 9c
 00000000000001f9  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 3b
 0000000000000214  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 2a0
 000000000000021d  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 43
 000000000000025c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + d0
-0000000000000265  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 5e
+0000000000000265  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 63
 0000000000000280  0000000a00000002 R_X86_64_PC32          0000000000000000 .text._ZN11arithmetica8FractionD2Ev + 0
-00000000000002a0  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 470
-00000000000002a9  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 66
-00000000000002f4  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + f0
-00000000000002fd  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 91
-0000000000000318  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 780
-0000000000000321  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 99
-000000000000036c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 134
-0000000000000375  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + c4
-0000000000000390  0000000200000002 R_X86_64_PC32          0000000000000000 .text + a90
-0000000000000399  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + cc
-00000000000003e4  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 178
-00000000000003ed  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + f7
-0000000000000408  0000000200000002 R_X86_64_PC32          0000000000000000 .text + da0
-0000000000000411  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + ff
-000000000000045c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1bc
-0000000000000465  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 12a
-0000000000000480  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 10b0
-00000000000004cc  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 1180
-0000000000000518  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 1250
-0000000000000521  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 132
-000000000000056c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 200
-0000000000000575  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 152
+00000000000002a0  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 480
+00000000000002a9  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 6b
+00000000000002f4  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 108
+00000000000002fd  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 96
+0000000000000318  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 790
+0000000000000321  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 9e
+000000000000036c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 14c
+0000000000000375  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + c9
+0000000000000390  0000000200000002 R_X86_64_PC32          0000000000000000 .text + aa0
+0000000000000399  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + d1
+00000000000003e4  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 190
+00000000000003ed  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + fc
+0000000000000408  0000000200000002 R_X86_64_PC32          0000000000000000 .text + db0
+0000000000000411  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 104
+000000000000045c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1d4
+0000000000000465  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 12f
+0000000000000480  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 10c0
+00000000000004cc  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 1190
+0000000000000518  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 1260
+0000000000000521  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 137
+000000000000056c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 218
+0000000000000575  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 157
```

##### readelf --wide --debug-dump=frames {}

```diff
@@ -225,51 +225,52 @@
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
   DW_CFA_nop
 
-0000020c 0000000000000044 000001e4 FDE cie=0000002c pc=00000000000002a0..000000000000046a
+0000020c 0000000000000044 000001e4 FDE cie=0000002c pc=00000000000002a0..0000000000000472
   Augmentation data:     26 fe ff ff
   DW_CFA_advance_loc: 6 to 00000000000002a6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 2 to 00000000000002a8
+  DW_CFA_advance_loc: 6 to 00000000000002ac
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 2 to 00000000000002aa
+  DW_CFA_advance_loc: 2 to 00000000000002ae
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 4 to 00000000000002ae
+  DW_CFA_advance_loc: 4 to 00000000000002b2
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 1 to 00000000000002af
+  DW_CFA_advance_loc: 1 to 00000000000002b3
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc: 7 to 00000000000002b6
+  DW_CFA_advance_loc: 7 to 00000000000002ba
   DW_CFA_def_cfa_offset: 112
-  DW_CFA_advance_loc2: 268 to 00000000000003c2
+  DW_CFA_advance_loc1: 130 to 000000000000033c
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 4 to 00000000000003c6
+  DW_CFA_advance_loc: 4 to 0000000000000340
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 00000000000003c7
+  DW_CFA_advance_loc: 1 to 0000000000000341
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000003c9
+  DW_CFA_advance_loc: 2 to 0000000000000343
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000003cb
+  DW_CFA_advance_loc: 2 to 0000000000000345
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000003cd
+  DW_CFA_advance_loc: 2 to 0000000000000347
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 3 to 00000000000003d0
+  DW_CFA_advance_loc: 9 to 0000000000000350
   DW_CFA_restore_state
+  DW_CFA_nop
 
-00000254 0000000000000020 0000022c FDE cie=0000002c pc=00000000000000d0..00000000000000f0
-  Augmentation data:     f9 fd ff ff
+00000254 0000000000000020 0000022c FDE cie=0000002c pc=00000000000000d0..0000000000000107
+  Augmentation data:     fe fd ff ff
   DW_CFA_def_cfa_offset: 112
   DW_CFA_offset: r3 (rbx) at cfa-48
   DW_CFA_offset: r6 (rbp) at cfa-40
   DW_CFA_offset: r12 (r12) at cfa-32
   DW_CFA_offset: r13 (r13) at cfa-24
   DW_CFA_offset: r14 (r14) at cfa-16
   DW_CFA_nop
@@ -285,353 +286,353 @@
   DW_CFA_def_cfa_offset: 8
   DW_CFA_advance_loc: 13 to 0000000000000040
   DW_CFA_restore_state
   DW_CFA_advance_loc: 1 to 0000000000000041
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
 
-00000298 0000000000000050 00000270 FDE cie=0000002c pc=0000000000000470..000000000000077c
-  Augmentation data:     bd fd ff ff
-  DW_CFA_advance_loc: 6 to 0000000000000476
+00000298 0000000000000050 00000270 FDE cie=0000002c pc=0000000000000480..000000000000078c
+  Augmentation data:     c2 fd ff ff
+  DW_CFA_advance_loc: 6 to 0000000000000486
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000000478
+  DW_CFA_advance_loc: 2 to 0000000000000488
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 000000000000047a
+  DW_CFA_advance_loc: 2 to 000000000000048a
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 000000000000047c
+  DW_CFA_advance_loc: 2 to 000000000000048c
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000000047d
+  DW_CFA_advance_loc: 1 to 000000000000048d
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 0000000000000481
+  DW_CFA_advance_loc: 4 to 0000000000000491
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 10 to 000000000000048b
+  DW_CFA_advance_loc: 10 to 000000000000049b
   DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc2: 523 to 0000000000000696
+  DW_CFA_advance_loc2: 523 to 00000000000006a6
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000000697
+  DW_CFA_advance_loc: 1 to 00000000000006a7
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000000698
+  DW_CFA_advance_loc: 1 to 00000000000006a8
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000069a
+  DW_CFA_advance_loc: 2 to 00000000000006aa
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000069c
+  DW_CFA_advance_loc: 2 to 00000000000006ac
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000069e
+  DW_CFA_advance_loc: 2 to 00000000000006ae
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000006a0
+  DW_CFA_advance_loc: 2 to 00000000000006b0
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 00000000000006a8
+  DW_CFA_advance_loc: 8 to 00000000000006b8
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000002ec 0000000000000020 000002c4 FDE cie=0000002c pc=00000000000000f0..0000000000000134
-  Augmentation data:     94 fd ff ff
+000002ec 0000000000000020 000002c4 FDE cie=0000002c pc=0000000000000108..000000000000014c
+  Augmentation data:     99 fd ff ff
   DW_CFA_def_cfa_offset: 192
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
 
-00000310 0000000000000050 000002e8 FDE cie=0000002c pc=0000000000000780..0000000000000a8c
-  Augmentation data:     78 fd ff ff
-  DW_CFA_advance_loc: 6 to 0000000000000786
+00000310 0000000000000050 000002e8 FDE cie=0000002c pc=0000000000000790..0000000000000a9c
+  Augmentation data:     7d fd ff ff
+  DW_CFA_advance_loc: 6 to 0000000000000796
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000000788
+  DW_CFA_advance_loc: 2 to 0000000000000798
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 000000000000078a
+  DW_CFA_advance_loc: 2 to 000000000000079a
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 000000000000078c
+  DW_CFA_advance_loc: 2 to 000000000000079c
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000000078d
+  DW_CFA_advance_loc: 1 to 000000000000079d
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 0000000000000791
+  DW_CFA_advance_loc: 4 to 00000000000007a1
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 10 to 000000000000079b
+  DW_CFA_advance_loc: 10 to 00000000000007ab
   DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc2: 523 to 00000000000009a6
+  DW_CFA_advance_loc2: 523 to 00000000000009b6
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 00000000000009a7
+  DW_CFA_advance_loc: 1 to 00000000000009b7
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000009a8
+  DW_CFA_advance_loc: 1 to 00000000000009b8
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000009aa
+  DW_CFA_advance_loc: 2 to 00000000000009ba
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000009ac
+  DW_CFA_advance_loc: 2 to 00000000000009bc
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000009ae
+  DW_CFA_advance_loc: 2 to 00000000000009be
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000009b0
+  DW_CFA_advance_loc: 2 to 00000000000009c0
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 00000000000009b8
+  DW_CFA_advance_loc: 8 to 00000000000009c8
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000364 0000000000000020 0000033c FDE cie=0000002c pc=0000000000000134..0000000000000178
-  Augmentation data:     4f fd ff ff
+00000364 0000000000000020 0000033c FDE cie=0000002c pc=000000000000014c..0000000000000190
+  Augmentation data:     54 fd ff ff
   DW_CFA_def_cfa_offset: 192
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
 
-00000388 0000000000000050 00000360 FDE cie=0000002c pc=0000000000000a90..0000000000000d9c
-  Augmentation data:     33 fd ff ff
-  DW_CFA_advance_loc: 6 to 0000000000000a96
+00000388 0000000000000050 00000360 FDE cie=0000002c pc=0000000000000aa0..0000000000000dac
+  Augmentation data:     38 fd ff ff
+  DW_CFA_advance_loc: 6 to 0000000000000aa6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000000a98
+  DW_CFA_advance_loc: 2 to 0000000000000aa8
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000000a9a
+  DW_CFA_advance_loc: 2 to 0000000000000aaa
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 0000000000000a9c
+  DW_CFA_advance_loc: 2 to 0000000000000aac
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000000a9d
+  DW_CFA_advance_loc: 1 to 0000000000000aad
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 0000000000000aa1
+  DW_CFA_advance_loc: 4 to 0000000000000ab1
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 10 to 0000000000000aab
+  DW_CFA_advance_loc: 10 to 0000000000000abb
   DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc2: 523 to 0000000000000cb6
+  DW_CFA_advance_loc2: 523 to 0000000000000cc6
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000000cb7
+  DW_CFA_advance_loc: 1 to 0000000000000cc7
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000000cb8
+  DW_CFA_advance_loc: 1 to 0000000000000cc8
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000000cba
+  DW_CFA_advance_loc: 2 to 0000000000000cca
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000000cbc
+  DW_CFA_advance_loc: 2 to 0000000000000ccc
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000000cbe
+  DW_CFA_advance_loc: 2 to 0000000000000cce
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000000cc0
+  DW_CFA_advance_loc: 2 to 0000000000000cd0
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 0000000000000cc8
+  DW_CFA_advance_loc: 8 to 0000000000000cd8
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000003dc 0000000000000020 000003b4 FDE cie=0000002c pc=0000000000000178..00000000000001bc
-  Augmentation data:     0a fd ff ff
+000003dc 0000000000000020 000003b4 FDE cie=0000002c pc=0000000000000190..00000000000001d4
+  Augmentation data:     0f fd ff ff
   DW_CFA_def_cfa_offset: 192
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
 
-00000400 0000000000000050 000003d8 FDE cie=0000002c pc=0000000000000da0..00000000000010ac
-  Augmentation data:     ee fc ff ff
-  DW_CFA_advance_loc: 6 to 0000000000000da6
+00000400 0000000000000050 000003d8 FDE cie=0000002c pc=0000000000000db0..00000000000010bc
+  Augmentation data:     f3 fc ff ff
+  DW_CFA_advance_loc: 6 to 0000000000000db6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000000da8
+  DW_CFA_advance_loc: 2 to 0000000000000db8
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000000daa
+  DW_CFA_advance_loc: 2 to 0000000000000dba
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 0000000000000dac
+  DW_CFA_advance_loc: 2 to 0000000000000dbc
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000000dad
+  DW_CFA_advance_loc: 1 to 0000000000000dbd
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 0000000000000db1
+  DW_CFA_advance_loc: 4 to 0000000000000dc1
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 10 to 0000000000000dbb
+  DW_CFA_advance_loc: 10 to 0000000000000dcb
   DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc2: 523 to 0000000000000fc6
+  DW_CFA_advance_loc2: 523 to 0000000000000fd6
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000000fc7
+  DW_CFA_advance_loc: 1 to 0000000000000fd7
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000000fc8
+  DW_CFA_advance_loc: 1 to 0000000000000fd8
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000000fca
+  DW_CFA_advance_loc: 2 to 0000000000000fda
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000000fcc
+  DW_CFA_advance_loc: 2 to 0000000000000fdc
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000000fce
+  DW_CFA_advance_loc: 2 to 0000000000000fde
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000000fd0
+  DW_CFA_advance_loc: 2 to 0000000000000fe0
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 0000000000000fd8
+  DW_CFA_advance_loc: 8 to 0000000000000fe8
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000454 0000000000000020 0000042c FDE cie=0000002c pc=00000000000001bc..0000000000000200
-  Augmentation data:     c5 fc ff ff
+00000454 0000000000000020 0000042c FDE cie=0000002c pc=00000000000001d4..0000000000000218
+  Augmentation data:     ca fc ff ff
   DW_CFA_def_cfa_offset: 192
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
 
-00000478 0000000000000048 0000047c FDE cie=00000000 pc=00000000000010b0..000000000000117f
-  DW_CFA_advance_loc: 6 to 00000000000010b6
+00000478 0000000000000048 0000047c FDE cie=00000000 pc=00000000000010c0..000000000000118f
+  DW_CFA_advance_loc: 6 to 00000000000010c6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r13 (r13) at cfa-16
-  DW_CFA_advance_loc: 9 to 00000000000010bf
+  DW_CFA_advance_loc: 9 to 00000000000010cf
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r12 (r12) at cfa-24
-  DW_CFA_advance_loc: 8 to 00000000000010c7
+  DW_CFA_advance_loc: 8 to 00000000000010d7
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r6 (rbp) at cfa-32
-  DW_CFA_advance_loc: 7 to 00000000000010ce
+  DW_CFA_advance_loc: 7 to 00000000000010de
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r3 (rbx) at cfa-40
-  DW_CFA_advance_loc: 7 to 00000000000010d5
+  DW_CFA_advance_loc: 7 to 00000000000010e5
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 59 to 0000000000001110
+  DW_CFA_advance_loc: 59 to 0000000000001120
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 0000000000001111
+  DW_CFA_advance_loc: 1 to 0000000000001121
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 0000000000001112
+  DW_CFA_advance_loc: 1 to 0000000000001122
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000001114
+  DW_CFA_advance_loc: 2 to 0000000000001124
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001116
+  DW_CFA_advance_loc: 2 to 0000000000001126
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 10 to 0000000000001120
+  DW_CFA_advance_loc: 10 to 0000000000001130
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 83 to 0000000000001173
+  DW_CFA_advance_loc1: 83 to 0000000000001183
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 6 to 0000000000001179
+  DW_CFA_advance_loc: 6 to 0000000000001189
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 000000000000117a
+  DW_CFA_advance_loc: 1 to 000000000000118a
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000117c
+  DW_CFA_advance_loc: 2 to 000000000000118c
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000117e
+  DW_CFA_advance_loc: 2 to 000000000000118e
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
 
-000004c4 0000000000000048 000004c8 FDE cie=00000000 pc=0000000000001180..000000000000124f
-  DW_CFA_advance_loc: 6 to 0000000000001186
+000004c4 0000000000000048 000004c8 FDE cie=00000000 pc=0000000000001190..000000000000125f
+  DW_CFA_advance_loc: 6 to 0000000000001196
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r13 (r13) at cfa-16
-  DW_CFA_advance_loc: 9 to 000000000000118f
+  DW_CFA_advance_loc: 9 to 000000000000119f
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r12 (r12) at cfa-24
-  DW_CFA_advance_loc: 8 to 0000000000001197
+  DW_CFA_advance_loc: 8 to 00000000000011a7
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r6 (rbp) at cfa-32
-  DW_CFA_advance_loc: 7 to 000000000000119e
+  DW_CFA_advance_loc: 7 to 00000000000011ae
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r3 (rbx) at cfa-40
-  DW_CFA_advance_loc: 7 to 00000000000011a5
+  DW_CFA_advance_loc: 7 to 00000000000011b5
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 59 to 00000000000011e0
+  DW_CFA_advance_loc: 59 to 00000000000011f0
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 00000000000011e1
+  DW_CFA_advance_loc: 1 to 00000000000011f1
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 00000000000011e2
+  DW_CFA_advance_loc: 1 to 00000000000011f2
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000011e4
+  DW_CFA_advance_loc: 2 to 00000000000011f4
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000011e6
+  DW_CFA_advance_loc: 2 to 00000000000011f6
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 10 to 00000000000011f0
+  DW_CFA_advance_loc: 10 to 0000000000001200
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 83 to 0000000000001243
+  DW_CFA_advance_loc1: 83 to 0000000000001253
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 6 to 0000000000001249
+  DW_CFA_advance_loc: 6 to 0000000000001259
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 000000000000124a
+  DW_CFA_advance_loc: 1 to 000000000000125a
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000124c
+  DW_CFA_advance_loc: 2 to 000000000000125c
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000124e
+  DW_CFA_advance_loc: 2 to 000000000000125e
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000510 0000000000000050 000004e8 FDE cie=0000002c pc=0000000000001250..00000000000014cf
-  Augmentation data:     11 fc ff ff
-  DW_CFA_advance_loc: 6 to 0000000000001256
+00000510 0000000000000050 000004e8 FDE cie=0000002c pc=0000000000001260..00000000000014df
+  Augmentation data:     16 fc ff ff
+  DW_CFA_advance_loc: 6 to 0000000000001266
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000001258
+  DW_CFA_advance_loc: 2 to 0000000000001268
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 000000000000125a
+  DW_CFA_advance_loc: 2 to 000000000000126a
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 5 to 000000000000125f
+  DW_CFA_advance_loc: 5 to 000000000000126f
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000001260
+  DW_CFA_advance_loc: 1 to 0000000000001270
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 0000000000001261
+  DW_CFA_advance_loc: 1 to 0000000000001271
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 10 to 000000000000126b
+  DW_CFA_advance_loc: 10 to 000000000000127b
   DW_CFA_def_cfa_offset: 224
-  DW_CFA_advance_loc2: 358 to 00000000000013d1
+  DW_CFA_advance_loc2: 358 to 00000000000013e1
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 00000000000013d5
+  DW_CFA_advance_loc: 4 to 00000000000013e5
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000013d6
+  DW_CFA_advance_loc: 1 to 00000000000013e6
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000013d8
+  DW_CFA_advance_loc: 2 to 00000000000013e8
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000013da
+  DW_CFA_advance_loc: 2 to 00000000000013ea
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000013dc
+  DW_CFA_advance_loc: 2 to 00000000000013ec
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000013de
+  DW_CFA_advance_loc: 2 to 00000000000013ee
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 2 to 00000000000013e0
+  DW_CFA_advance_loc: 2 to 00000000000013f0
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000564 0000000000000020 0000053c FDE cie=0000002c pc=0000000000000200..0000000000000230
-  Augmentation data:     dd fb ff ff
+00000564 0000000000000020 0000053c FDE cie=0000002c pc=0000000000000218..0000000000000248
+  Augmentation data:     e2 fb ff ff
   DW_CFA_def_cfa_offset: 224
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
```

##### strings --all --bytes=8 {}

```diff
@@ -41,30 +41,31 @@
 delete_fraction
 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
 _ZN11arithmetica8FractionC2EPKc
 _ZN11arithmetica8FractionC1EPKc
 _ZN11arithmetica8FractionC2ERK8fraction
 _ZN11arithmetica8FractionC1ERK8fraction
 _ZN11arithmetica8Fraction9to_stringB5cxx11Ev
-_ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm
+_ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc
 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm
+_ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7reserveEm
+_ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm
 _ZSt19__throw_logic_errorPKc
-_ZSt20__throw_length_errorPKc
 __stack_chk_fail
+_ZSt20__throw_length_errorPKc
 _ZN11arithmetica8FractionD2Ev
 _ZN11arithmetica8FractionD1Ev
 _ZN11arithmetica8FractionplERKS0_
 add_fraction
 _ZN11arithmetica8FractionmiERKS0_
 subtract_fraction
 _ZN11arithmetica8FractionmlERKS0_
 multiply_fraction
 _ZN11arithmetica8FractiondvERKS0_
 _ZN11arithmetica8FractioneqERKS0_
-_ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc
 _ZeqRKN11arithmetica8FractionES2_
 _ZltRKN11arithmetica8FractionES2_
 .shstrtab
 .rela.text
 .rela.text.unlikely
 .gcc_except_table
 .rodata.str1.8
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -239,139 +239,145 @@
 	nop
 	nopl   0x0(%rax)
 
 00000000000002a0 <arithmetica::Fraction::to_string[abi:cxx11]()>:
 arithmetica::Fraction::to_string[abi:cxx11]():
 	endbr64
 	push   %r14
+	lea    0x10(%rdi),%r14
 	push   %r13
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	push   %rbx
 	mov    %rsi,%rbx
 	sub    $0x40,%rsp
-	mov    (%rsi),%r14
 	mov    0x8(%rsi),%r13
 	mov    %fs:0x28,%rax
 	mov    %rax,0x38(%rsp)
 	xor    %eax,%eax
-	lea    0x20(%rsp),%rbp
-	mov    %r14,%rax
-	mov    %rbp,0x10(%rsp)
+	mov    %r14,(%rdi)
+	mov    (%rsi),%rbp
+	mov    %rbp,%rax
 	add    %r13,%rax
-	je     2e8 <arithmetica::Fraction::to_string[abi:cxx11]()+0x48>
-	test   %r14,%r14
-	je     430 <arithmetica::Fraction::to_string[abi:cxx11]()+0x190>
+	je     2e5 <arithmetica::Fraction::to_string[abi:cxx11]()+0x45>
+	test   %rbp,%rbp
+	je     435 <arithmetica::Fraction::to_string[abi:cxx11]()+0x195>
 	mov    %r13,0x8(%rsp)
 	cmp    $0xf,%r13
-	ja     3e0 <arithmetica::Fraction::to_string[abi:cxx11]()+0x140>
+	ja     360 <arithmetica::Fraction::to_string[abi:cxx11]()+0xc0>
 	cmp    $0x1,%r13
-	jne    3d0 <arithmetica::Fraction::to_string[abi:cxx11]()+0x130>
-	movzbl (%r14),%eax
-	mov    %al,0x20(%rsp)
-	mov    %rbp,%rax
-	mov    %r13,0x18(%rsp)
-	movb   $0x0,(%rax,%r13,1)
-	movabs $0x3fffffffffffffff,%rax
-	cmp    %rax,0x18(%rsp)
-	je     43c <arithmetica::Fraction::to_string[abi:cxx11]()+0x19c>
-	lea    0x10(%rsp),%r13
-	mov    $0x1,%edx
+	jne    350 <arithmetica::Fraction::to_string[abi:cxx11]()+0xb0>
+	movzbl 0x0(%rbp),%eax
+	mov    %al,0x10(%r12)
+	mov    %r14,%rax
+	mov    %r13,0x8(%r12)
+	lea    0x20(%rbx),%rdi
 	lea    0x0(%rip),%rsi        
- R_X86_64_PC32	.LC6-0x4
-	mov    %r13,%rdi
-	call   344 <arithmetica::Fraction::to_string[abi:cxx11]()+0xa4>
- R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_append(char const*, unsigned long)-0x4
-	mov    0x28(%rbx),%rdx
-	mov    0x20(%rbx),%rsi
-	mov    %r13,%rdi
-	call   354 <arithmetica::Fraction::to_string[abi:cxx11]()+0xb4>
- R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_append(char const*, unsigned long)-0x4
-	lea    0x10(%r12),%rdx
-	mov    %rdx,(%r12)
-	mov    (%rax),%rcx
-	lea    0x10(%rax),%rdx
-	cmp    %rdx,%rcx
-	je     420 <arithmetica::Fraction::to_string[abi:cxx11]()+0x180>
-	mov    %rcx,(%r12)
-	mov    0x10(%rax),%rcx
-	mov    %rcx,0x10(%r12)
-	mov    0x8(%rax),%rcx
-	mov    %rdx,(%rax)
-	mov    0x10(%rsp),%rdi
-	movq   $0x0,0x8(%rax)
-	mov    %rcx,0x8(%r12)
-	movb   $0x0,0x10(%rax)
-	cmp    %rbp,%rdi
-	je     3aa <arithmetica::Fraction::to_string[abi:cxx11]()+0x10a>
-	mov    0x20(%rsp),%rax
-	lea    0x1(%rax),%rsi
-	call   3aa <arithmetica::Fraction::to_string[abi:cxx11]()+0x10a>
- R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
+ R_X86_64_PC32	.LC5-0x4
+	movb   $0x0,(%rax,%r13,1)
+	call   31c <arithmetica::Fraction::to_string[abi:cxx11]()+0x7c>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
+	test   %eax,%eax
+	jne    3a0 <arithmetica::Fraction::to_string[abi:cxx11]()+0x100>
 	mov    0x38(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    448 <arithmetica::Fraction::to_string[abi:cxx11]()+0x1a8>
+	jne    441 <arithmetica::Fraction::to_string[abi:cxx11]()+0x1a1>
 	add    $0x40,%rsp
 	mov    %r12,%rax
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
-	xchg   %ax,%ax
+	nopl   0x0(%rax,%rax,1)
 	test   %r13,%r13
-	jne    44d <arithmetica::Fraction::to_string[abi:cxx11]()+0x1ad>
-	mov    %rbp,%rax
-	jmp    30c <arithmetica::Fraction::to_string[abi:cxx11]()+0x6c>
-	nopl   (%rax)
-	lea    0x10(%rsp),%rdi
+	jne    452 <arithmetica::Fraction::to_string[abi:cxx11]()+0x1b2>
+	mov    %r14,%rax
+	jmp    302 <arithmetica::Fraction::to_string[abi:cxx11]()+0x62>
+	xchg   %ax,%ax
+	mov    %r12,%rdi
 	lea    0x8(%rsp),%rsi
 	xor    %edx,%edx
-	call   3f1 <arithmetica::Fraction::to_string[abi:cxx11]()+0x151>
+	call   36f <arithmetica::Fraction::to_string[abi:cxx11]()+0xcf>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
-	mov    %rax,0x10(%rsp)
+	mov    %rax,(%r12)
 	mov    %rax,%rdi
 	mov    0x8(%rsp),%rax
-	mov    %rax,0x20(%rsp)
+	mov    %rax,0x10(%r12)
 	mov    %r13,%rdx
-	mov    %r14,%rsi
-	call   40e <arithmetica::Fraction::to_string[abi:cxx11]()+0x16e>
+	mov    %rbp,%rsi
+	call   38b <arithmetica::Fraction::to_string[abi:cxx11]()+0xeb>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x8(%rsp),%r13
-	mov    0x10(%rsp),%rax
-	jmp    30c <arithmetica::Fraction::to_string[abi:cxx11]()+0x6c>
-	nopl   (%rax)
-	movdqu 0x10(%rax),%xmm0
-	movups %xmm0,0x10(%r12)
-	jmp    37a <arithmetica::Fraction::to_string[abi:cxx11]()+0xda>
+	mov    (%r12),%rax
+	jmp    302 <arithmetica::Fraction::to_string[abi:cxx11]()+0x62>
+	nopl   0x0(%rax)
+	mov    0x28(%rbx),%rax
+	lea    0x10(%rsp),%rbp
+	lea    0x20(%rsp),%r13
+	movq   $0x0,0x18(%rsp)
+	mov    %rbp,%rdi
+	mov    %r13,0x10(%rsp)
+	lea    0x1(%rax),%rsi
+	movb   $0x0,0x20(%rsp)
+	call   3cd <arithmetica::Fraction::to_string[abi:cxx11]()+0x12d>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::reserve(unsigned long)-0x4
+	movabs $0x3fffffffffffffff,%rax
+	cmp    %rax,0x18(%rsp)
+	je     446 <arithmetica::Fraction::to_string[abi:cxx11]()+0x1a6>
+	mov    $0x1,%edx
+	lea    0x0(%rip),%rsi        
+ R_X86_64_PC32	.LC7-0x4
+	mov    %rbp,%rdi
+	call   3f2 <arithmetica::Fraction::to_string[abi:cxx11]()+0x152>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_append(char const*, unsigned long)-0x4
+	mov    0x28(%rbx),%rdx
+	mov    0x20(%rbx),%rsi
+	mov    %rbp,%rdi
+	call   402 <arithmetica::Fraction::to_string[abi:cxx11]()+0x162>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_append(char const*, unsigned long)-0x4
+	mov    0x18(%rsp),%rdx
+	mov    0x10(%rsp),%rsi
+	mov    %r12,%rdi
+	call   414 <arithmetica::Fraction::to_string[abi:cxx11]()+0x174>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_append(char const*, unsigned long)-0x4
+	mov    0x10(%rsp),%rdi
+	cmp    %r13,%rdi
+	je     324 <arithmetica::Fraction::to_string[abi:cxx11]()+0x84>
+	mov    0x20(%rsp),%rax
+	lea    0x1(%rax),%rsi
+	call   430 <arithmetica::Fraction::to_string[abi:cxx11]()+0x190>
+ R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
+	jmp    324 <arithmetica::Fraction::to_string[abi:cxx11]()+0x84>
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   43c <arithmetica::Fraction::to_string[abi:cxx11]()+0x19c>
+	call   441 <arithmetica::Fraction::to_string[abi:cxx11]()+0x1a1>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
+	call   446 <arithmetica::Fraction::to_string[abi:cxx11]()+0x1a6>
+ R_X86_64_PLT32	__stack_chk_fail-0x4
 	lea    0x0(%rip),%rdi        
- R_X86_64_PC32	.LC5-0x4
-	call   448 <arithmetica::Fraction::to_string[abi:cxx11]()+0x1a8>
+ R_X86_64_PC32	.LC6-0x4
+	call   452 <arithmetica::Fraction::to_string[abi:cxx11]()+0x1b2>
  R_X86_64_PLT32	std::__throw_length_error(char const*)-0x4
-	call   44d <arithmetica::Fraction::to_string[abi:cxx11]()+0x1ad>
- R_X86_64_PLT32	__stack_chk_fail-0x4
-	mov    %rbp,%rdi
-	jmp    403 <arithmetica::Fraction::to_string[abi:cxx11]()+0x163>
+	mov    %r14,%rdi
+	jmp    380 <arithmetica::Fraction::to_string[abi:cxx11]()+0xe0>
 	endbr64
-	mov    %rax,%r12
-	jmp    45e <arithmetica::Fraction::to_string[abi:cxx11]()+0x1be>
+	mov    %rax,%rbp
+	jmp    466 <arithmetica::Fraction::to_string[abi:cxx11]()+0x1c6>
  R_X86_64_PC32	.text.unlikely+0xcc
 	endbr64
-	mov    %rax,%r12
-	jmp    46a <arithmetica::Fraction::to_string[abi:cxx11]()+0x1ca>
+	mov    %rax,%rbp
+	jmp    472 <arithmetica::Fraction::to_string[abi:cxx11]()+0x1d2>
  R_X86_64_PC32	.text.unlikely+0xcc
-	nopw   0x0(%rax,%rax,1)
+	data16 cs nopw 0x0(%rax,%rax,1)
+	nopl   (%rax)
 
-0000000000000470 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)>:
+0000000000000480 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)>:
 arithmetica::Fraction::operator+(arithmetica::Fraction const&):
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
@@ -381,220 +387,220 @@
 	sub    $0x88,%rsp
 	mov    %rdi,0x8(%rsp)
 	mov    %fs:0x28,%rax
 	mov    %rax,0x78(%rsp)
 	mov    0x8(%rsi),%rax
 	mov    $0x1,%esi
 	lea    0x1(%rax),%rdi
-	call   4b0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x40>
+	call   4c0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x40>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r13
 	mov    0x28(%rbp),%rax
 	lea    0x1(%rax),%rdi
-	call   4c5 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x55>
+	call   4d5 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x55>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r14
 	mov    0x8(%rbx),%rax
 	lea    0x1(%rax),%rdi
-	call   4da <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x6a>
+	call   4ea <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x6a>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r15
 	mov    0x28(%rbx),%rax
 	lea    0x1(%rax),%rdi
-	call   4ef <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x7f>
+	call   4ff <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x7f>
  R_X86_64_PLT32	calloc-0x4
 	mov    0x0(%rbp),%rsi
 	mov    %r13,%rdi
 	mov    %rax,%r12
-	call   4fe <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x8e>
+	call   50e <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x8e>
  R_X86_64_PLT32	strcpy-0x4
 	mov    0x20(%rbp),%rsi
 	mov    %r14,%rdi
-	call   50a <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x9a>
+	call   51a <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x9a>
  R_X86_64_PLT32	strcpy-0x4
 	mov    (%rbx),%rsi
 	mov    %r15,%rdi
-	call   515 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xa5>
+	call   525 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xa5>
  R_X86_64_PLT32	strcpy-0x4
 	mov    0x20(%rbx),%rsi
 	mov    %r12,%rdi
 	mov    %r12,%rbx
-	call   524 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xb4>
+	call   534 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xb4>
  R_X86_64_PLT32	strcpy-0x4
 	movq   %r12,%xmm1
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	movq   %r15,%xmm0
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x10(%rsp)
 	mov    0x18(%rsp),%rcx
 	mov    0x10(%rsp),%rdx
-	call   54c <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xdc>
+	call   55c <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xdc>
  R_X86_64_PLT32	add_fraction-0x4
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	mov    %rax,%r12
 	mov    %rdx,%rbp
-	call   55d <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xed>
+	call   56d <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xed>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbx,%rsi
 	mov    %r15,%rdi
 	lea    0x60(%rsp),%rbx
-	call   56d <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xfd>
+	call   57d <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xfd>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbx,0x50(%rsp)
 	test   %rbp,%rbp
-	je     742 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2d2>
+	je     752 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2d2>
 	mov    %rbp,%rdi
 	lea    0x50(%rsp),%r15
-	call   588 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x118>
+	call   598 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x118>
  R_X86_64_PLT32	strlen-0x4
 	mov    %rax,0x28(%rsp)
 	mov    %rax,%r14
 	cmp    $0xf,%rax
-	ja     6c0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x250>
+	ja     6d0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x250>
 	cmp    $0x1,%rax
-	jne    5e0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x170>
+	jne    5f0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x170>
 	movzbl 0x0(%rbp),%edx
 	mov    %dl,0x60(%rsp)
 	mov    %rbx,%rdx
 	mov    %rax,0x58(%rsp)
 	lea    0x40(%rsp),%r14
 	movb   $0x0,(%rdx,%rax,1)
 	lea    0x30(%rsp),%rax
 	mov    %r14,0x30(%rsp)
 	mov    %rax,%r13
 	test   %r12,%r12
-	jne    5f0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x180>
+	jne    600 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x180>
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   5d7 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x167>
+	call   5e7 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x167>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	nopw   0x0(%rax,%rax,1)
 	test   %rax,%rax
-	jne    753 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2e3>
+	jne    763 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2e3>
 	mov    %rbx,%rdx
-	jmp    5ab <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x13b>
+	jmp    5bb <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x13b>
 	xchg   %ax,%ax
 	mov    %r12,%rdi
-	call   5f8 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x188>
+	call   608 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x188>
  R_X86_64_PLT32	strlen-0x4
 	mov    %rax,0x10(%rsp)
 	mov    %rax,0x28(%rsp)
 	cmp    $0xf,%rax
-	ja     700 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x290>
+	ja     710 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x290>
 	cmp    $0x1,%rax
-	jne    6a8 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x238>
+	jne    6b8 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x238>
 	movzbl (%r12),%edx
 	mov    %dl,0x40(%rsp)
 	mov    %r14,%rdx
 	mov    %rax,0x38(%rsp)
 	mov    0x8(%rsp),%rdi
 	mov    %r13,%rsi
 	movb   $0x0,(%rdx,%rax,1)
 	mov    %r15,%rdx
-	call   63b <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1cb>
+	call   64b <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1cb>
  R_X86_64_PLT32	arithmetica::Fraction::Fraction(std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&, std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&)-0x4
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     653 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1e3>
+	je     663 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1e3>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   653 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1e3>
+	call   663 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1e3>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	cmp    %rbx,%rdi
-	je     66b <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1fb>
+	je     67b <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1fb>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   66b <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1fb>
+	call   67b <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1fb>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    %r12,%rdi
 	mov    %rbp,%rsi
-	call   676 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x206>
+	call   686 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x206>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    0x78(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    73d <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2cd>
+	jne    74d <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2cd>
 	mov    0x8(%rsp),%rax
 	add    $0x88,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopl   0x0(%rax)
 	cmpq   $0x0,0x10(%rsp)
-	jne    74e <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2de>
+	jne    75e <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2de>
 	mov    %r14,%rdx
-	jmp    622 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1b2>
+	jmp    632 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1b2>
 	nopl   0x0(%rax)
 	mov    %r15,%rdi
 	lea    0x28(%rsp),%rsi
 	xor    %edx,%edx
-	call   6cf <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x25f>
+	call   6df <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x25f>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x50(%rsp)
 	mov    %rax,%rdi
 	mov    0x28(%rsp),%rax
 	mov    %rax,0x60(%rsp)
 	mov    %r14,%rdx
 	mov    %rbp,%rsi
-	call   6ec <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x27c>
+	call   6fc <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x27c>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rax
 	mov    0x50(%rsp),%rdx
-	jmp    5ab <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x13b>
+	jmp    5bb <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x13b>
 	nopl   0x0(%rax,%rax,1)
 	lea    0x28(%rsp),%rsi
 	xor    %edx,%edx
 	mov    %r13,%rdi
-	call   70f <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x29f>
+	call   71f <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x29f>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x30(%rsp)
 	mov    %rax,%rdi
 	mov    0x28(%rsp),%rax
 	mov    %rax,0x40(%rsp)
 	mov    0x10(%rsp),%rdx
 	mov    %r12,%rsi
-	call   72e <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2be>
+	call   73e <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2be>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rax
 	mov    0x30(%rsp),%rdx
-	jmp    622 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1b2>
-	call   742 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2d2>
+	jmp    632 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1b2>
+	call   752 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2d2>
  R_X86_64_PLT32	__stack_chk_fail-0x4
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   74e <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2de>
+	call   75e <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2de>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	mov    %r14,%rdi
-	jmp    721 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2b1>
+	jmp    731 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2b1>
 	mov    %rbx,%rdi
-	jmp    6e1 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x271>
+	jmp    6f1 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x271>
 	endbr64
 	mov    %rax,%rbp
-	jmp    764 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2f4>
- R_X86_64_PC32	.text.unlikely+0x104
+	jmp    774 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2f4>
+ R_X86_64_PC32	.text.unlikely+0x11c
 	endbr64
 	mov    %rax,%rbp
-	jmp    770 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x300>
- R_X86_64_PC32	.text.unlikely+0xec
+	jmp    780 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x300>
+ R_X86_64_PC32	.text.unlikely+0x104
 	endbr64
 	mov    %rax,%rbp
-	jmp    77c <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x30c>
- R_X86_64_PC32	.text.unlikely+0x11e
+	jmp    78c <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x30c>
+ R_X86_64_PC32	.text.unlikely+0x136
 	nopl   0x0(%rax)
 
-0000000000000780 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)>:
+0000000000000790 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)>:
 arithmetica::Fraction::operator-(arithmetica::Fraction const&):
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
@@ -604,220 +610,220 @@
 	sub    $0x88,%rsp
 	mov    %rdi,0x8(%rsp)
 	mov    %fs:0x28,%rax
 	mov    %rax,0x78(%rsp)
 	mov    0x8(%rsi),%rax
 	mov    $0x1,%esi
 	lea    0x1(%rax),%rdi
-	call   7c0 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x40>
+	call   7d0 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x40>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r13
 	mov    0x28(%rbp),%rax
 	lea    0x1(%rax),%rdi
-	call   7d5 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x55>
+	call   7e5 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x55>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r14
 	mov    0x8(%rbx),%rax
 	lea    0x1(%rax),%rdi
-	call   7ea <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x6a>
+	call   7fa <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x6a>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r15
 	mov    0x28(%rbx),%rax
 	lea    0x1(%rax),%rdi
-	call   7ff <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x7f>
+	call   80f <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x7f>
  R_X86_64_PLT32	calloc-0x4
 	mov    0x0(%rbp),%rsi
 	mov    %r13,%rdi
 	mov    %rax,%r12
-	call   80e <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x8e>
+	call   81e <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x8e>
  R_X86_64_PLT32	strcpy-0x4
 	mov    0x20(%rbp),%rsi
 	mov    %r14,%rdi
-	call   81a <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x9a>
+	call   82a <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x9a>
  R_X86_64_PLT32	strcpy-0x4
 	mov    (%rbx),%rsi
 	mov    %r15,%rdi
-	call   825 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xa5>
+	call   835 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xa5>
  R_X86_64_PLT32	strcpy-0x4
 	mov    0x20(%rbx),%rsi
 	mov    %r12,%rdi
 	mov    %r12,%rbx
-	call   834 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xb4>
+	call   844 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xb4>
  R_X86_64_PLT32	strcpy-0x4
 	movq   %r12,%xmm1
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	movq   %r15,%xmm0
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x10(%rsp)
 	mov    0x18(%rsp),%rcx
 	mov    0x10(%rsp),%rdx
-	call   85c <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xdc>
+	call   86c <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xdc>
  R_X86_64_PLT32	subtract_fraction-0x4
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	mov    %rax,%r12
 	mov    %rdx,%rbp
-	call   86d <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xed>
+	call   87d <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xed>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbx,%rsi
 	mov    %r15,%rdi
 	lea    0x60(%rsp),%rbx
-	call   87d <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xfd>
+	call   88d <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xfd>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbx,0x50(%rsp)
 	test   %rbp,%rbp
-	je     a52 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2d2>
+	je     a62 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2d2>
 	mov    %rbp,%rdi
 	lea    0x50(%rsp),%r15
-	call   898 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x118>
+	call   8a8 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x118>
  R_X86_64_PLT32	strlen-0x4
 	mov    %rax,0x28(%rsp)
 	mov    %rax,%r14
 	cmp    $0xf,%rax
-	ja     9d0 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x250>
+	ja     9e0 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x250>
 	cmp    $0x1,%rax
-	jne    8f0 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x170>
+	jne    900 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x170>
 	movzbl 0x0(%rbp),%edx
 	mov    %dl,0x60(%rsp)
 	mov    %rbx,%rdx
 	mov    %rax,0x58(%rsp)
 	lea    0x40(%rsp),%r14
 	movb   $0x0,(%rdx,%rax,1)
 	lea    0x30(%rsp),%rax
 	mov    %r14,0x30(%rsp)
 	mov    %rax,%r13
 	test   %r12,%r12
-	jne    900 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x180>
+	jne    910 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x180>
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   8e7 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x167>
+	call   8f7 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x167>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	nopw   0x0(%rax,%rax,1)
 	test   %rax,%rax
-	jne    a63 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2e3>
+	jne    a73 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2e3>
 	mov    %rbx,%rdx
-	jmp    8bb <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x13b>
+	jmp    8cb <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x13b>
 	xchg   %ax,%ax
 	mov    %r12,%rdi
-	call   908 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x188>
+	call   918 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x188>
  R_X86_64_PLT32	strlen-0x4
 	mov    %rax,0x10(%rsp)
 	mov    %rax,0x28(%rsp)
 	cmp    $0xf,%rax
-	ja     a10 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x290>
+	ja     a20 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x290>
 	cmp    $0x1,%rax
-	jne    9b8 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x238>
+	jne    9c8 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x238>
 	movzbl (%r12),%edx
 	mov    %dl,0x40(%rsp)
 	mov    %r14,%rdx
 	mov    %rax,0x38(%rsp)
 	mov    0x8(%rsp),%rdi
 	mov    %r13,%rsi
 	movb   $0x0,(%rdx,%rax,1)
 	mov    %r15,%rdx
-	call   94b <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1cb>
+	call   95b <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1cb>
  R_X86_64_PLT32	arithmetica::Fraction::Fraction(std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&, std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&)-0x4
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     963 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1e3>
+	je     973 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1e3>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   963 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1e3>
+	call   973 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1e3>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	cmp    %rbx,%rdi
-	je     97b <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1fb>
+	je     98b <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1fb>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   97b <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1fb>
+	call   98b <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1fb>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    %r12,%rdi
 	mov    %rbp,%rsi
-	call   986 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x206>
+	call   996 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x206>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    0x78(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    a4d <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2cd>
+	jne    a5d <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2cd>
 	mov    0x8(%rsp),%rax
 	add    $0x88,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopl   0x0(%rax)
 	cmpq   $0x0,0x10(%rsp)
-	jne    a5e <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2de>
+	jne    a6e <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2de>
 	mov    %r14,%rdx
-	jmp    932 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1b2>
+	jmp    942 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1b2>
 	nopl   0x0(%rax)
 	mov    %r15,%rdi
 	lea    0x28(%rsp),%rsi
 	xor    %edx,%edx
-	call   9df <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x25f>
+	call   9ef <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x25f>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x50(%rsp)
 	mov    %rax,%rdi
 	mov    0x28(%rsp),%rax
 	mov    %rax,0x60(%rsp)
 	mov    %r14,%rdx
 	mov    %rbp,%rsi
-	call   9fc <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x27c>
+	call   a0c <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x27c>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rax
 	mov    0x50(%rsp),%rdx
-	jmp    8bb <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x13b>
+	jmp    8cb <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x13b>
 	nopl   0x0(%rax,%rax,1)
 	lea    0x28(%rsp),%rsi
 	xor    %edx,%edx
 	mov    %r13,%rdi
-	call   a1f <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x29f>
+	call   a2f <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x29f>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x30(%rsp)
 	mov    %rax,%rdi
 	mov    0x28(%rsp),%rax
 	mov    %rax,0x40(%rsp)
 	mov    0x10(%rsp),%rdx
 	mov    %r12,%rsi
-	call   a3e <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2be>
+	call   a4e <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2be>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rax
 	mov    0x30(%rsp),%rdx
-	jmp    932 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1b2>
-	call   a52 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2d2>
+	jmp    942 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1b2>
+	call   a62 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2d2>
  R_X86_64_PLT32	__stack_chk_fail-0x4
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   a5e <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2de>
+	call   a6e <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2de>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	mov    %r14,%rdi
-	jmp    a31 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2b1>
+	jmp    a41 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2b1>
 	mov    %rbx,%rdi
-	jmp    9f1 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x271>
+	jmp    a01 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x271>
 	endbr64
 	mov    %rax,%rbp
-	jmp    a74 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2f4>
- R_X86_64_PC32	.text.unlikely+0x148
+	jmp    a84 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2f4>
+ R_X86_64_PC32	.text.unlikely+0x160
 	endbr64
 	mov    %rax,%rbp
-	jmp    a80 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x300>
- R_X86_64_PC32	.text.unlikely+0x130
+	jmp    a90 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x300>
+ R_X86_64_PC32	.text.unlikely+0x148
 	endbr64
 	mov    %rax,%rbp
-	jmp    a8c <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x30c>
- R_X86_64_PC32	.text.unlikely+0x162
+	jmp    a9c <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x30c>
+ R_X86_64_PC32	.text.unlikely+0x17a
 	nopl   0x0(%rax)
 
-0000000000000a90 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)>:
+0000000000000aa0 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)>:
 arithmetica::Fraction::operator*(arithmetica::Fraction const&):
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
@@ -827,220 +833,220 @@
 	sub    $0x88,%rsp
 	mov    %rdi,0x8(%rsp)
 	mov    %fs:0x28,%rax
 	mov    %rax,0x78(%rsp)
 	mov    0x8(%rsi),%rax
 	mov    $0x1,%esi
 	lea    0x1(%rax),%rdi
-	call   ad0 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x40>
+	call   ae0 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x40>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r13
 	mov    0x28(%rbp),%rax
 	lea    0x1(%rax),%rdi
-	call   ae5 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x55>
+	call   af5 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x55>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r14
 	mov    0x8(%rbx),%rax
 	lea    0x1(%rax),%rdi
-	call   afa <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x6a>
+	call   b0a <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x6a>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r15
 	mov    0x28(%rbx),%rax
 	lea    0x1(%rax),%rdi
-	call   b0f <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x7f>
+	call   b1f <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x7f>
  R_X86_64_PLT32	calloc-0x4
 	mov    0x0(%rbp),%rsi
 	mov    %r13,%rdi
 	mov    %rax,%r12
-	call   b1e <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x8e>
+	call   b2e <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x8e>
  R_X86_64_PLT32	strcpy-0x4
 	mov    0x20(%rbp),%rsi
 	mov    %r14,%rdi
-	call   b2a <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x9a>
+	call   b3a <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x9a>
  R_X86_64_PLT32	strcpy-0x4
 	mov    (%rbx),%rsi
 	mov    %r15,%rdi
-	call   b35 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xa5>
+	call   b45 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xa5>
  R_X86_64_PLT32	strcpy-0x4
 	mov    0x20(%rbx),%rsi
 	mov    %r12,%rdi
 	mov    %r12,%rbx
-	call   b44 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xb4>
+	call   b54 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xb4>
  R_X86_64_PLT32	strcpy-0x4
 	movq   %r12,%xmm1
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	movq   %r15,%xmm0
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x10(%rsp)
 	mov    0x18(%rsp),%rcx
 	mov    0x10(%rsp),%rdx
-	call   b6c <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xdc>
+	call   b7c <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xdc>
  R_X86_64_PLT32	multiply_fraction-0x4
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	mov    %rax,%r12
 	mov    %rdx,%rbp
-	call   b7d <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xed>
+	call   b8d <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xed>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbx,%rsi
 	mov    %r15,%rdi
 	lea    0x60(%rsp),%rbx
-	call   b8d <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xfd>
+	call   b9d <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xfd>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbx,0x50(%rsp)
 	test   %rbp,%rbp
-	je     d62 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2d2>
+	je     d72 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2d2>
 	mov    %rbp,%rdi
 	lea    0x50(%rsp),%r15
-	call   ba8 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x118>
+	call   bb8 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x118>
  R_X86_64_PLT32	strlen-0x4
 	mov    %rax,0x28(%rsp)
 	mov    %rax,%r14
 	cmp    $0xf,%rax
-	ja     ce0 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x250>
+	ja     cf0 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x250>
 	cmp    $0x1,%rax
-	jne    c00 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x170>
+	jne    c10 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x170>
 	movzbl 0x0(%rbp),%edx
 	mov    %dl,0x60(%rsp)
 	mov    %rbx,%rdx
 	mov    %rax,0x58(%rsp)
 	lea    0x40(%rsp),%r14
 	movb   $0x0,(%rdx,%rax,1)
 	lea    0x30(%rsp),%rax
 	mov    %r14,0x30(%rsp)
 	mov    %rax,%r13
 	test   %r12,%r12
-	jne    c10 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x180>
+	jne    c20 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x180>
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   bf7 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x167>
+	call   c07 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x167>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	nopw   0x0(%rax,%rax,1)
 	test   %rax,%rax
-	jne    d73 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2e3>
+	jne    d83 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2e3>
 	mov    %rbx,%rdx
-	jmp    bcb <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x13b>
+	jmp    bdb <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x13b>
 	xchg   %ax,%ax
 	mov    %r12,%rdi
-	call   c18 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x188>
+	call   c28 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x188>
  R_X86_64_PLT32	strlen-0x4
 	mov    %rax,0x10(%rsp)
 	mov    %rax,0x28(%rsp)
 	cmp    $0xf,%rax
-	ja     d20 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x290>
+	ja     d30 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x290>
 	cmp    $0x1,%rax
-	jne    cc8 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x238>
+	jne    cd8 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x238>
 	movzbl (%r12),%edx
 	mov    %dl,0x40(%rsp)
 	mov    %r14,%rdx
 	mov    %rax,0x38(%rsp)
 	mov    0x8(%rsp),%rdi
 	mov    %r13,%rsi
 	movb   $0x0,(%rdx,%rax,1)
 	mov    %r15,%rdx
-	call   c5b <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1cb>
+	call   c6b <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1cb>
  R_X86_64_PLT32	arithmetica::Fraction::Fraction(std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&, std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&)-0x4
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     c73 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1e3>
+	je     c83 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1e3>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   c73 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1e3>
+	call   c83 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1e3>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	cmp    %rbx,%rdi
-	je     c8b <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1fb>
+	je     c9b <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1fb>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   c8b <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1fb>
+	call   c9b <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1fb>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    %r12,%rdi
 	mov    %rbp,%rsi
-	call   c96 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x206>
+	call   ca6 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x206>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    0x78(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    d5d <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2cd>
+	jne    d6d <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2cd>
 	mov    0x8(%rsp),%rax
 	add    $0x88,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopl   0x0(%rax)
 	cmpq   $0x0,0x10(%rsp)
-	jne    d6e <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2de>
+	jne    d7e <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2de>
 	mov    %r14,%rdx
-	jmp    c42 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1b2>
+	jmp    c52 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1b2>
 	nopl   0x0(%rax)
 	mov    %r15,%rdi
 	lea    0x28(%rsp),%rsi
 	xor    %edx,%edx
-	call   cef <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x25f>
+	call   cff <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x25f>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x50(%rsp)
 	mov    %rax,%rdi
 	mov    0x28(%rsp),%rax
 	mov    %rax,0x60(%rsp)
 	mov    %r14,%rdx
 	mov    %rbp,%rsi
-	call   d0c <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x27c>
+	call   d1c <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x27c>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rax
 	mov    0x50(%rsp),%rdx
-	jmp    bcb <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x13b>
+	jmp    bdb <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x13b>
 	nopl   0x0(%rax,%rax,1)
 	lea    0x28(%rsp),%rsi
 	xor    %edx,%edx
 	mov    %r13,%rdi
-	call   d2f <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x29f>
+	call   d3f <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x29f>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x30(%rsp)
 	mov    %rax,%rdi
 	mov    0x28(%rsp),%rax
 	mov    %rax,0x40(%rsp)
 	mov    0x10(%rsp),%rdx
 	mov    %r12,%rsi
-	call   d4e <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2be>
+	call   d5e <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2be>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rax
 	mov    0x30(%rsp),%rdx
-	jmp    c42 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1b2>
-	call   d62 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2d2>
+	jmp    c52 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1b2>
+	call   d72 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2d2>
  R_X86_64_PLT32	__stack_chk_fail-0x4
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   d6e <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2de>
+	call   d7e <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2de>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	mov    %r14,%rdi
-	jmp    d41 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2b1>
+	jmp    d51 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2b1>
 	mov    %rbx,%rdi
-	jmp    d01 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x271>
+	jmp    d11 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x271>
 	endbr64
 	mov    %rax,%rbp
-	jmp    d84 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2f4>
- R_X86_64_PC32	.text.unlikely+0x18c
+	jmp    d94 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2f4>
+ R_X86_64_PC32	.text.unlikely+0x1a4
 	endbr64
 	mov    %rax,%rbp
-	jmp    d90 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x300>
- R_X86_64_PC32	.text.unlikely+0x174
+	jmp    da0 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x300>
+ R_X86_64_PC32	.text.unlikely+0x18c
 	endbr64
 	mov    %rax,%rbp
-	jmp    d9c <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x30c>
- R_X86_64_PC32	.text.unlikely+0x1a6
+	jmp    dac <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x30c>
+ R_X86_64_PC32	.text.unlikely+0x1be
 	nopl   0x0(%rax)
 
-0000000000000da0 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)>:
+0000000000000db0 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)>:
 arithmetica::Fraction::operator/(arithmetica::Fraction const&):
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
@@ -1050,380 +1056,380 @@
 	sub    $0x88,%rsp
 	mov    %rdi,0x8(%rsp)
 	mov    %fs:0x28,%rax
 	mov    %rax,0x78(%rsp)
 	mov    0x8(%rsi),%rax
 	mov    $0x1,%esi
 	lea    0x1(%rax),%rdi
-	call   de0 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x40>
+	call   df0 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x40>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r13
 	mov    0x28(%rbp),%rax
 	lea    0x1(%rax),%rdi
-	call   df5 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x55>
+	call   e05 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x55>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r14
 	mov    0x28(%rbx),%rax
 	lea    0x1(%rax),%rdi
-	call   e0a <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x6a>
+	call   e1a <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x6a>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r15
 	mov    0x8(%rbx),%rax
 	lea    0x1(%rax),%rdi
-	call   e1f <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x7f>
+	call   e2f <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x7f>
  R_X86_64_PLT32	calloc-0x4
 	mov    0x0(%rbp),%rsi
 	mov    %r13,%rdi
 	mov    %rax,%r12
-	call   e2e <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x8e>
+	call   e3e <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x8e>
  R_X86_64_PLT32	strcpy-0x4
 	mov    0x20(%rbp),%rsi
 	mov    %r14,%rdi
-	call   e3a <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x9a>
+	call   e4a <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x9a>
  R_X86_64_PLT32	strcpy-0x4
 	mov    0x20(%rbx),%rsi
 	mov    %r15,%rdi
-	call   e46 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xa6>
+	call   e56 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xa6>
  R_X86_64_PLT32	strcpy-0x4
 	mov    (%rbx),%rsi
 	mov    %r12,%rdi
 	mov    %r12,%rbx
-	call   e54 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xb4>
+	call   e64 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xb4>
  R_X86_64_PLT32	strcpy-0x4
 	movq   %r12,%xmm1
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	movq   %r15,%xmm0
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x10(%rsp)
 	mov    0x18(%rsp),%rcx
 	mov    0x10(%rsp),%rdx
-	call   e7c <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xdc>
+	call   e8c <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xdc>
  R_X86_64_PLT32	multiply_fraction-0x4
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	mov    %rax,%r12
 	mov    %rdx,%rbp
-	call   e8d <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xed>
+	call   e9d <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xed>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbx,%rsi
 	mov    %r15,%rdi
 	lea    0x60(%rsp),%rbx
-	call   e9d <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xfd>
+	call   ead <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xfd>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbx,0x50(%rsp)
 	test   %rbp,%rbp
-	je     1072 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2d2>
+	je     1082 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2d2>
 	mov    %rbp,%rdi
 	lea    0x50(%rsp),%r15
-	call   eb8 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x118>
+	call   ec8 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x118>
  R_X86_64_PLT32	strlen-0x4
 	mov    %rax,0x28(%rsp)
 	mov    %rax,%r14
 	cmp    $0xf,%rax
-	ja     ff0 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x250>
+	ja     1000 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x250>
 	cmp    $0x1,%rax
-	jne    f10 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x170>
+	jne    f20 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x170>
 	movzbl 0x0(%rbp),%edx
 	mov    %dl,0x60(%rsp)
 	mov    %rbx,%rdx
 	mov    %rax,0x58(%rsp)
 	lea    0x40(%rsp),%r14
 	movb   $0x0,(%rdx,%rax,1)
 	lea    0x30(%rsp),%rax
 	mov    %r14,0x30(%rsp)
 	mov    %rax,%r13
 	test   %r12,%r12
-	jne    f20 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x180>
+	jne    f30 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x180>
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   f07 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x167>
+	call   f17 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x167>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	nopw   0x0(%rax,%rax,1)
 	test   %rax,%rax
-	jne    1083 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2e3>
+	jne    1093 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2e3>
 	mov    %rbx,%rdx
-	jmp    edb <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x13b>
+	jmp    eeb <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x13b>
 	xchg   %ax,%ax
 	mov    %r12,%rdi
-	call   f28 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x188>
+	call   f38 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x188>
  R_X86_64_PLT32	strlen-0x4
 	mov    %rax,0x10(%rsp)
 	mov    %rax,0x28(%rsp)
 	cmp    $0xf,%rax
-	ja     1030 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x290>
+	ja     1040 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x290>
 	cmp    $0x1,%rax
-	jne    fd8 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x238>
+	jne    fe8 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x238>
 	movzbl (%r12),%edx
 	mov    %dl,0x40(%rsp)
 	mov    %r14,%rdx
 	mov    %rax,0x38(%rsp)
 	mov    0x8(%rsp),%rdi
 	mov    %r13,%rsi
 	movb   $0x0,(%rdx,%rax,1)
 	mov    %r15,%rdx
-	call   f6b <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1cb>
+	call   f7b <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1cb>
  R_X86_64_PLT32	arithmetica::Fraction::Fraction(std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&, std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&)-0x4
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     f83 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1e3>
+	je     f93 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1e3>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   f83 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1e3>
+	call   f93 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1e3>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	cmp    %rbx,%rdi
-	je     f9b <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1fb>
+	je     fab <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1fb>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   f9b <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1fb>
+	call   fab <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1fb>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    %r12,%rdi
 	mov    %rbp,%rsi
-	call   fa6 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x206>
+	call   fb6 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x206>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    0x78(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    106d <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2cd>
+	jne    107d <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2cd>
 	mov    0x8(%rsp),%rax
 	add    $0x88,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopl   0x0(%rax)
 	cmpq   $0x0,0x10(%rsp)
-	jne    107e <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2de>
+	jne    108e <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2de>
 	mov    %r14,%rdx
-	jmp    f52 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1b2>
+	jmp    f62 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1b2>
 	nopl   0x0(%rax)
 	mov    %r15,%rdi
 	lea    0x28(%rsp),%rsi
 	xor    %edx,%edx
-	call   fff <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x25f>
+	call   100f <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x25f>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x50(%rsp)
 	mov    %rax,%rdi
 	mov    0x28(%rsp),%rax
 	mov    %rax,0x60(%rsp)
 	mov    %r14,%rdx
 	mov    %rbp,%rsi
-	call   101c <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x27c>
+	call   102c <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x27c>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rax
 	mov    0x50(%rsp),%rdx
-	jmp    edb <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x13b>
+	jmp    eeb <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x13b>
 	nopl   0x0(%rax,%rax,1)
 	lea    0x28(%rsp),%rsi
 	xor    %edx,%edx
 	mov    %r13,%rdi
-	call   103f <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x29f>
+	call   104f <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x29f>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x30(%rsp)
 	mov    %rax,%rdi
 	mov    0x28(%rsp),%rax
 	mov    %rax,0x40(%rsp)
 	mov    0x10(%rsp),%rdx
 	mov    %r12,%rsi
-	call   105e <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2be>
+	call   106e <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2be>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rax
 	mov    0x30(%rsp),%rdx
-	jmp    f52 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1b2>
-	call   1072 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2d2>
+	jmp    f62 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1b2>
+	call   1082 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2d2>
  R_X86_64_PLT32	__stack_chk_fail-0x4
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   107e <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2de>
+	call   108e <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2de>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	mov    %r14,%rdi
-	jmp    1051 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2b1>
+	jmp    1061 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2b1>
 	mov    %rbx,%rdi
-	jmp    1011 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x271>
+	jmp    1021 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x271>
 	endbr64
 	mov    %rax,%rbp
-	jmp    1094 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2f4>
- R_X86_64_PC32	.text.unlikely+0x1d0
+	jmp    10a4 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2f4>
+ R_X86_64_PC32	.text.unlikely+0x1e8
 	endbr64
 	mov    %rax,%rbp
-	jmp    10a0 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x300>
- R_X86_64_PC32	.text.unlikely+0x1b8
+	jmp    10b0 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x300>
+ R_X86_64_PC32	.text.unlikely+0x1d0
 	endbr64
 	mov    %rax,%rbp
-	jmp    10ac <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x30c>
- R_X86_64_PC32	.text.unlikely+0x1ea
+	jmp    10bc <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x30c>
+ R_X86_64_PC32	.text.unlikely+0x202
 	nopl   0x0(%rax)
 
-00000000000010b0 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)>:
+00000000000010c0 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)>:
 arithmetica::Fraction::operator==(arithmetica::Fraction const&):
 	endbr64
 	push   %r13
 	lea    0x0(%rip),%r13        
- R_X86_64_PC32	.LC12-0x4
+ R_X86_64_PC32	.LC13-0x4
 	push   %r12
 	lea    0x0(%rip),%r12        
- R_X86_64_PC32	.LC13-0x4
+ R_X86_64_PC32	.LC14-0x4
 	push   %rbp
 	mov    %rsi,%rbp
 	mov    %r13,%rsi
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x8,%rsp
-	call   10da <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x2a>
+	call   10ea <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x2a>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
 	test   %eax,%eax
-	jne    10f1 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x41>
+	jne    1101 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x41>
 	mov    %r12,%rsi
 	mov    %rbp,%rdi
-	call   10e9 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x39>
+	call   10f9 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x39>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
 	test   %eax,%eax
-	je     116f <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xbf>
+	je     117f <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xbf>
 	mov    %r12,%rsi
 	mov    %rbx,%rdi
-	call   10fc <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x4c>
+	call   110c <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x4c>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
 	test   %eax,%eax
-	je     1160 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xb0>
+	je     1170 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xb0>
 	mov    0x8(%rbx),%rdx
 	xor    %eax,%eax
 	cmp    0x8(%rbp),%rdx
-	je     1120 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x70>
+	je     1130 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x70>
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	nopw   0x0(%rax,%rax,1)
 	mov    (%rbx),%rdi
 	mov    0x0(%rbp),%rsi
 	test   %rdx,%rdx
-	je     113b <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x8b>
-	call   1131 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x81>
+	je     114b <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x8b>
+	call   1141 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x81>
  R_X86_64_PLT32	memcmp-0x4
 	mov    %eax,%r8d
 	xor    %eax,%eax
 	test   %r8d,%r8d
-	jne    110c <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x5c>
+	jne    111c <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x5c>
 	mov    0x28(%rbx),%rdx
 	xor    %eax,%eax
 	cmp    0x28(%rbp),%rdx
-	jne    110c <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x5c>
+	jne    111c <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x5c>
 	mov    0x20(%rbx),%rdi
 	mov    0x20(%rbp),%rsi
 	test   %rdx,%rdx
-	je     116f <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xbf>
-	call   1159 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xa9>
+	je     117f <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xbf>
+	call   1169 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xa9>
  R_X86_64_PLT32	memcmp-0x4
 	test   %eax,%eax
 	sete   %al
-	jmp    110c <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x5c>
+	jmp    111c <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x5c>
 	mov    %r13,%rsi
 	mov    %rbp,%rdi
-	call   116b <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xbb>
+	call   117b <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xbb>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
 	test   %eax,%eax
-	jne    1100 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x50>
+	jne    1110 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x50>
 	add    $0x8,%rsp
 	mov    $0x1,%eax
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	nop
 
-0000000000001180 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)>:
+0000000000001190 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)>:
 operator==(arithmetica::Fraction const&, arithmetica::Fraction const&):
 	endbr64
 	push   %r13
 	lea    0x0(%rip),%r13        
- R_X86_64_PC32	.LC12-0x4
+ R_X86_64_PC32	.LC13-0x4
 	push   %r12
 	lea    0x0(%rip),%r12        
- R_X86_64_PC32	.LC13-0x4
+ R_X86_64_PC32	.LC14-0x4
 	push   %rbp
 	mov    %rsi,%rbp
 	mov    %r13,%rsi
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x8,%rsp
-	call   11aa <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x2a>
+	call   11ba <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x2a>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
 	test   %eax,%eax
-	jne    11c1 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x41>
+	jne    11d1 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x41>
 	mov    %r12,%rsi
 	mov    %rbp,%rdi
-	call   11b9 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x39>
+	call   11c9 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x39>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
 	test   %eax,%eax
-	je     123f <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xbf>
+	je     124f <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xbf>
 	mov    %r12,%rsi
 	mov    %rbx,%rdi
-	call   11cc <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x4c>
+	call   11dc <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x4c>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
 	test   %eax,%eax
-	je     1230 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xb0>
+	je     1240 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xb0>
 	mov    0x8(%rbx),%rdx
 	xor    %eax,%eax
 	cmp    0x8(%rbp),%rdx
-	je     11f0 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x70>
+	je     1200 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x70>
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	nopw   0x0(%rax,%rax,1)
 	mov    (%rbx),%rdi
 	mov    0x0(%rbp),%rsi
 	test   %rdx,%rdx
-	je     120b <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x8b>
-	call   1201 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x81>
+	je     121b <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x8b>
+	call   1211 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x81>
  R_X86_64_PLT32	memcmp-0x4
 	mov    %eax,%r8d
 	xor    %eax,%eax
 	test   %r8d,%r8d
-	jne    11dc <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x5c>
+	jne    11ec <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x5c>
 	mov    0x28(%rbx),%rdx
 	xor    %eax,%eax
 	cmp    0x28(%rbp),%rdx
-	jne    11dc <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x5c>
+	jne    11ec <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x5c>
 	mov    0x20(%rbx),%rdi
 	mov    0x20(%rbp),%rsi
 	test   %rdx,%rdx
-	je     123f <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xbf>
-	call   1229 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xa9>
+	je     124f <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xbf>
+	call   1239 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xa9>
  R_X86_64_PLT32	memcmp-0x4
 	test   %eax,%eax
 	sete   %al
-	jmp    11dc <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x5c>
+	jmp    11ec <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x5c>
 	mov    %r13,%rsi
 	mov    %rbp,%rdi
-	call   123b <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xbb>
+	call   124b <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xbb>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
 	test   %eax,%eax
-	jne    11d0 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x50>
+	jne    11e0 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x50>
 	add    $0x8,%rsp
 	mov    $0x1,%eax
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	nop
 
-0000000000001250 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)>:
+0000000000001260 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)>:
 operator<(arithmetica::Fraction const&, arithmetica::Fraction const&):
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	mov    %rsi,%r13
 	push   %r12
@@ -1436,157 +1442,157 @@
 	mov    %fs:0x28,%rax
 	mov    %rax,0x98(%rsp)
 	xor    %eax,%eax
 	lea    0x20(%rsp),%rbp
 	mov    %r14,%rax
 	mov    %rbp,0x10(%rsp)
 	add    %r12,%rax
-	je     12a0 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x50>
+	je     12b0 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x50>
 	test   %r14,%r14
-	je     148d <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x23d>
+	je     149d <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x23d>
 	mov    %r12,0x8(%rsp)
 	cmp    $0xf,%r12
-	ja     1410 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1c0>
+	ja     1420 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1c0>
 	cmp    $0x1,%r12
-	jne    13e0 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x190>
+	jne    13f0 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x190>
 	movzbl (%r14),%eax
 	mov    %al,0x20(%rsp)
 	mov    %rbp,%rax
 	mov    %r12,0x18(%rsp)
 	lea    0x40(%rsp),%r14
 	movb   $0x0,(%rax,%r12,1)
 	mov    0x20(%rbx),%r15
 	mov    0x28(%rbx),%r12
 	mov    %r14,0x30(%rsp)
 	mov    %r15,%rax
 	add    %r12,%rax
-	je     12f1 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xa1>
+	je     1301 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xa1>
 	test   %r15,%r15
-	je     149e <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x24e>
+	je     14ae <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x24e>
 	mov    %r12,0x8(%rsp)
 	cmp    $0xf,%r12
-	ja     1450 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x200>
+	ja     1460 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x200>
 	cmp    $0x1,%r12
-	jne    13f8 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1a8>
+	jne    1408 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1a8>
 	movzbl (%r15),%eax
 	mov    %al,0x40(%rsp)
 	mov    %r14,%rax
 	mov    %r12,0x38(%rsp)
 	lea    0x50(%rsp),%rdi
 	mov    %r13,%rdx
 	movb   $0x0,(%rax,%r12,1)
 	lea    0x10(%rsp),%r12
 	mov    %r12,%rsi
-	call   1334 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xe4>
+	call   1344 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xe4>
  R_X86_64_PLT32	arithmetica::Fraction::operator-(arithmetica::Fraction const&)-0x4
 	mov    0x50(%rsp),%rdi
 	mov    0x70(%rsp),%r8
 	lea    0x80(%rsp),%rax
 	cmpb   $0x2d,(%rdi)
 	sete   %r12b
 	cmp    %rax,%r8
-	je     136b <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x11b>
+	je     137b <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x11b>
 	mov    0x80(%rsp),%rax
 	mov    %r8,%rdi
 	lea    0x1(%rax),%rsi
-	call   1366 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x116>
+	call   1376 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x116>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	lea    0x60(%rsp),%rax
 	cmp    %rax,%rdi
-	je     1383 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x133>
+	je     1393 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x133>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   1383 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x133>
+	call   1393 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x133>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     139b <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x14b>
+	je     13ab <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x14b>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   139b <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x14b>
+	call   13ab <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x14b>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x10(%rsp),%rdi
 	cmp    %rbp,%rdi
-	je     13b3 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x163>
+	je     13c3 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x163>
 	mov    0x20(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   13b3 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x163>
+	call   13c3 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x163>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x98(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    1499 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x249>
+	jne    14a9 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x249>
 	add    $0xa8,%rsp
 	mov    %r12d,%eax
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nop
 	test   %r12,%r12
-	jne    14af <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x25f>
+	jne    14bf <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x25f>
 	mov    %rbp,%rax
-	jmp    12c4 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x74>
+	jmp    12d4 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x74>
 	nopl   0x0(%rax)
 	test   %r12,%r12
-	jne    14aa <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x25a>
+	jne    14ba <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x25a>
 	mov    %r14,%rax
-	jmp    1315 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xc5>
+	jmp    1325 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xc5>
 	nopl   0x0(%rax)
 	lea    0x10(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
 	xor    %edx,%edx
-	call   1421 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1d1>
+	call   1431 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1d1>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x10(%rsp)
 	mov    %rax,%rdi
 	mov    0x8(%rsp),%rax
 	mov    %rax,0x20(%rsp)
 	mov    %r12,%rdx
 	mov    %r14,%rsi
-	call   143e <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1ee>
+	call   144e <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1ee>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x8(%rsp),%r12
 	mov    0x10(%rsp),%rax
-	jmp    12c4 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x74>
+	jmp    12d4 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x74>
 	nopl   (%rax)
 	lea    0x8(%rsp),%rsi
 	lea    0x30(%rsp),%rdi
 	xor    %edx,%edx
-	call   1461 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x211>
+	call   1471 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x211>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x30(%rsp)
 	mov    %rax,%rdi
 	mov    0x8(%rsp),%rax
 	mov    %rax,0x40(%rsp)
 	mov    %r12,%rdx
 	mov    %r15,%rsi
-	call   147e <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x22e>
+	call   148e <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x22e>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x8(%rsp),%r12
 	mov    0x30(%rsp),%rax
-	jmp    1315 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xc5>
+	jmp    1325 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xc5>
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   1499 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x249>
+	call   14a9 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x249>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
-	call   149e <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x24e>
+	call   14ae <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x24e>
  R_X86_64_PLT32	__stack_chk_fail-0x4
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   14aa <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x25a>
+	call   14ba <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x25a>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	mov    %r14,%rdi
-	jmp    1473 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x223>
+	jmp    1483 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x223>
 	mov    %rbp,%rdi
-	jmp    1433 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1e3>
+	jmp    1443 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1e3>
 	endbr64
 	mov    %rax,%r12
-	jmp    14c3 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x273>
- R_X86_64_PC32	.text.unlikely+0x1fc
+	jmp    14d3 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x273>
+ R_X86_64_PC32	.text.unlikely+0x214
 	endbr64
 	mov    %rax,%rbp
-	jmp    14cf <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x27f>
- R_X86_64_PC32	.text.unlikely+0x21c
+	jmp    14df <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x27f>
+ R_X86_64_PC32	.text.unlikely+0x234
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text.unlikely {}

```diff
@@ -86,131 +86,139 @@
 	call   cf <arithmetica::Fraction::Fraction(fraction const&) [clone .cold]+0x33>
  R_X86_64_PLT32	_Unwind_Resume-0x4
 	nop
 
 00000000000000d0 <arithmetica::Fraction::to_string[abi:cxx11]() [clone .cold]>:
 arithmetica::Fraction::to_string[abi:cxx11]() [clone .cold]:
 	mov    0x10(%rsp),%rdi
-	cmp    %rbp,%rdi
+	cmp    %r13,%rdi
 	je     e8 <arithmetica::Fraction::to_string[abi:cxx11]() [clone .cold]+0x18>
 	mov    0x20(%rsp),%rax
 	lea    0x1(%rax),%rsi
 	call   e8 <arithmetica::Fraction::to_string[abi:cxx11]() [clone .cold]+0x18>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
-	mov    %r12,%rdi
-	call   f0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]>
+	mov    (%r12),%rdi
+	cmp    %rdi,%r14
+	je     ff <arithmetica::Fraction::to_string[abi:cxx11]() [clone .cold]+0x2f>
+	mov    0x10(%r12),%rsi
+	add    $0x1,%rsi
+	call   ff <arithmetica::Fraction::to_string[abi:cxx11]() [clone .cold]+0x2f>
+ R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
+	mov    %rbp,%rdi
+	call   107 <arithmetica::Fraction::to_string[abi:cxx11]() [clone .cold]+0x37>
  R_X86_64_PLT32	_Unwind_Resume-0x4
+	nop
 
-00000000000000f0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]>:
+0000000000000108 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]>:
 arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]:
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     108 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x18>
+	je     120 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x18>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   108 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x18>
+	call   120 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x18>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	cmp    %rbx,%rdi
-	je     12c <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	je     144 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x3c>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   120 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x30>
+	call   138 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x30>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
-	jmp    12c <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	jmp    144 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x3c>
 	mov    0x8(%rsp),%rdi
-	call   12c <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	call   144 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x3c>
  R_X86_64_PLT32	arithmetica::Fraction::~Fraction()-0x4
 	mov    %rbp,%rdi
-	call   134 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]>
+	call   14c <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]>
  R_X86_64_PLT32	_Unwind_Resume-0x4
 
-0000000000000134 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]>:
+000000000000014c <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]>:
 arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]:
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     14c <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x18>
+	je     164 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x18>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   14c <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x18>
+	call   164 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x18>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	cmp    %rbx,%rdi
-	je     170 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	je     188 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x3c>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   164 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x30>
+	call   17c <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x30>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
-	jmp    170 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	jmp    188 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x3c>
 	mov    0x8(%rsp),%rdi
-	call   170 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	call   188 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x3c>
  R_X86_64_PLT32	arithmetica::Fraction::~Fraction()-0x4
 	mov    %rbp,%rdi
-	call   178 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]>
+	call   190 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]>
  R_X86_64_PLT32	_Unwind_Resume-0x4
 
-0000000000000178 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]>:
+0000000000000190 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]>:
 arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]:
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     190 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x18>
+	je     1a8 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x18>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   190 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x18>
+	call   1a8 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x18>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	cmp    %rbx,%rdi
-	je     1b4 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	je     1cc <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x3c>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   1a8 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x30>
+	call   1c0 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x30>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
-	jmp    1b4 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	jmp    1cc <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x3c>
 	mov    0x8(%rsp),%rdi
-	call   1b4 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	call   1cc <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x3c>
  R_X86_64_PLT32	arithmetica::Fraction::~Fraction()-0x4
 	mov    %rbp,%rdi
-	call   1bc <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]>
+	call   1d4 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]>
  R_X86_64_PLT32	_Unwind_Resume-0x4
 
-00000000000001bc <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]>:
+00000000000001d4 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]>:
 arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]:
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     1d4 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x18>
+	je     1ec <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x18>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   1d4 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x18>
+	call   1ec <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x18>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	cmp    %rbx,%rdi
-	je     1f8 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	je     210 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x3c>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   1ec <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x30>
+	call   204 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x30>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
-	jmp    1f8 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	jmp    210 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x3c>
 	mov    0x8(%rsp),%rdi
-	call   1f8 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	call   210 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x3c>
  R_X86_64_PLT32	arithmetica::Fraction::~Fraction()-0x4
 	mov    %rbp,%rdi
-	call   200 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]>
+	call   218 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]>
  R_X86_64_PLT32	_Unwind_Resume-0x4
 
-0000000000000200 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]>:
+0000000000000218 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]>:
 operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]:
 	mov    0x10(%rsp),%rdi
 	cmp    %rbp,%rdi
-	je     218 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x18>
+	je     230 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x18>
 	mov    0x20(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   218 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x18>
+	call   230 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x18>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    %r12,%rdi
-	call   220 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x20>
+	call   238 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x20>
  R_X86_64_PLT32	_Unwind_Resume-0x4
 	mov    %r12,%rdi
-	call   228 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x28>
+	call   240 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x28>
  R_X86_64_PLT32	arithmetica::Fraction::~Fraction()-0x4
 	mov    %rbp,%rdi
-	call   230 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x30>
+	call   248 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x30>
  R_X86_64_PLT32	_Unwind_Resume-0x4
```

##### readelf --wide --decompress --hex-dump=.gcc_except_table {}

```diff
@@ -1,25 +1,25 @@
 
 Hex dump of section '.gcc_except_table':
   0x00000000 ffff0104 39145600 ffff0104 2e050000 ....9.V.........
   0x00000010 ffff0105 3f52a001 00ffff01 042e0500 ....?R..........
   0x00000020 00ffff01 053f52a0 0100ffff 01042e05 .....?R.........
   0x00000030 0000ffff 01055729 8f0100ff ff01042e ......W)........
-  0x00000040 050000ff ff01179f 0105be03 00af0105 ................
-  0x00000050 b20300cc 02500000 a30305be 0300ffff .....P..........
-  0x00000060 01041b05 0000ffff 0127d701 260000e2 .........'..&...
-  0x00000070 0205e805 00c60305 f4050081 04058006 ................
-  0x00000080 00da0405 00009a05 05e80500 d9050500 ................
-  0x00000090 00ffff01 043f0500 00ffff01 27d70126 .....?......'..&
-  0x000000a0 0000e202 05e80500 c60305f4 05008104 ................
-  0x000000b0 05800600 da040500 009a0505 e80500d9 ................
-  0x000000c0 05050000 ffff0104 3f050000 ffff0127 ........?......'
-  0x000000d0 d7012600 00e20205 e80500c6 0305f405 ..&.............
-  0x000000e0 00810405 800600da 04050000 9a0505e8 ................
-  0x000000f0 0500d905 050000ff ff01043f 050000ff ...........?....
-  0x00000100 ff0127d7 01260000 e20205e8 0500c603 ..'..&..........
-  0x00000110 05f40500 81040580 0600da04 0500009a ................
-  0x00000120 0505e805 00d90505 0000ffff 01043f05 ..............?.
-  0x00000130 0000ffff 011cdf01 05f30400 cc030500 ................
-  0x00000140 008c0405 e70400c4 04050000 d50405e7 ................
-  0x00000150 0400ffff 01041b15 0000              ..........
+  0x00000040 050000ff ff011cca 01050000 a8023aba ..............:.
+  0x00000050 0300ef02 05c60300 9c030500 00ad0305 ................
+  0x00000060 ba0300ff ff010432 050000ff ff0127d7 .......2......'.
+  0x00000070 01260000 e20205e8 0500c603 05f40500 .&..............
+  0x00000080 81040580 0600da04 0500009a 0505e805 ................
+  0x00000090 00d90505 0000ffff 01043f05 0000ffff ..........?.....
+  0x000000a0 0127d701 260000e2 0205e805 00c60305 .'..&...........
+  0x000000b0 f4050081 04058006 00da0405 00009a05 ................
+  0x000000c0 05e80500 d9050500 00ffff01 043f0500 .............?..
+  0x000000d0 00ffff01 27d70126 0000e202 05e80500 ....'..&........
+  0x000000e0 c60305f4 05008104 05800600 da040500 ................
+  0x000000f0 009a0505 e80500d9 05050000 ffff0104 ................
+  0x00000100 3f050000 ffff0127 d7012600 00e20205 ?......'..&.....
+  0x00000110 e80500c6 0305f405 00810405 800600da ................
+  0x00000120 04050000 9a0505e8 0500d905 050000ff ................
+  0x00000130 ff01043f 050000ff ff011cdf 0105f304 ...?............
+  0x00000140 00cc0305 00008c04 05e70400 c4040500 ................
+  0x00000150 00d50405 e70400ff ff01041b 150000   ...............
```

##### readelf --wide --decompress --string-dump=.rodata.str1.1 {}

```diff
@@ -1,7 +1,8 @@
 
 String dump of section '.rodata.str1.1':
-  [     0]  basic_string::append
-  [    15]  /
-  [    17]  -0
-  [    1a]  0
+  [     0]  1
+  [     2]  basic_string::append
+  [    17]  /
+  [    19]  -0
+  [    1c]  0
```

##### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -30,20 +30,20 @@
   0x000001a0 00000000 9b000000 04000000 00460e10 .............F..
   0x000001b0 8f02420e 188e0346 0e208d04 460e288c ..B....F. ..F.(.
   0x000001c0 05410e30 8606440e 38830747 0e400264 .A.0..D.8..G.@.d
   0x000001d0 0a0e3841 0e30410e 28420e20 420e1842 ..8A.0A.(B. B..B
   0x000001e0 0e10420e 08410b00 20000000 c0010000 ..B..A.. .......
   0x000001f0 00000000 33000000 04000000 000e4083 ....3.........@.
   0x00000200 0786068c 058d048e 038f0200 44000000 ............D...
-  0x00000210 e4010000 00000000 ca010000 04000000 ................
-  0x00000220 00460e10 8e02420e 188d0342 0e208c04 .F....B....B. ..
-  0x00000230 440e2886 05410e30 8306470e 70030c01 D.(..A.0..G.p...
-  0x00000240 0a0e3044 0e28410e 20420e18 420e1042 ..0D.(A. B..B..B
-  0x00000250 0e08430b 20000000 2c020000 00000000 ..C. ...,.......
-  0x00000260 20000000 04000000 000e7083 0686058c  .........p.....
+  0x00000210 e4010000 00000000 d2010000 04000000 ................
+  0x00000220 00460e10 8e02460e 188d0342 0e208c04 .F....F....B. ..
+  0x00000230 440e2886 05410e30 8306470e 7002820a D.(..A.0..G.p...
+  0x00000240 0e30440e 28410e20 420e1842 0e10420e .0D.(A. B..B..B.
+  0x00000250 08490b00 20000000 2c020000 00000000 .I.. ...,.......
+  0x00000260 37000000 04000000 000e7083 0686058c 7.........p.....
   0x00000270 048d038e 02000000 1c000000 7c020000 ............|...
   0x00000280 00000000 42000000 00450e10 83026e0a ....B....E....n.
   0x00000290 0e084d0b 410e0800 50000000 70020000 ..M.A...P...p...
   0x000002a0 00000000 0c030000 04000000 00460e10 .............F..
   0x000002b0 8f02420e 188e0342 0e208d04 420e288c ..B....B. ..B.(.
   0x000002c0 05410e30 8606440e 3883074a 0ec00103 .A.0..D.8..J....
   0x000002d0 0b020a0e 38410e30 410e2842 0e20420e ....8A.0A.(B. B.
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -28,105 +28,109 @@
   0x00000190 6c64005f 5a4e3131 61726974 686d6574 ld._ZN11arithmet
   0x000001a0 69636138 46726163 74696f6e 6d6c4552 ica8FractionmlER
   0x000001b0 4b53305f 2e636f6c 64005f5a 4e313161 KS0_.cold._ZN11a
   0x000001c0 72697468 6d657469 63613846 72616374 rithmetica8Fract
   0x000001d0 696f6e64 7645524b 53305f2e 636f6c64 iondvERKS0_.cold
   0x000001e0 005f5a6c 74524b4e 31316172 6974686d ._ZltRKN11arithm
   0x000001f0 65746963 61384672 61637469 6f6e4553 etica8FractionES
-  0x00000200 325f2e63 6f6c6400 2e4c4336 002e4c43 2_.cold..LC6..LC
-  0x00000210 34002e4c 4335002e 4c433132 002e4c43 4..LC5..LC12..LC
-  0x00000220 3133005f 5a4e3131 61726974 686d6574 13._ZN11arithmet
-  0x00000230 69636138 46726163 74696f6e 44354576 ica8FractionD5Ev
-  0x00000240 005f5a4e 31316172 6974686d 65746963 ._ZN11arithmetic
-  0x00000250 61384672 61637469 6f6e4332 4576005f a8FractionC2Ev._
-  0x00000260 5a4e3131 61726974 686d6574 69636138 ZN11arithmetica8
-  0x00000270 46726163 74696f6e 43314576 005f5a4e FractionC1Ev._ZN
-  0x00000280 31316172 6974686d 65746963 61384672 11arithmetica8Fr
-  0x00000290 61637469 6f6e4332 45524b4e 5374375f actionC2ERKNSt7_
-  0x000002a0 5f637878 31313132 62617369 635f7374 _cxx1112basic_st
-  0x000002b0 72696e67 49635374 31316368 61725f74 ringIcSt11char_t
-  0x000002c0 72616974 73496345 53614963 45454553 raitsIcESaIcEEES
-  0x000002d0 385f0044 572e7265 662e5f5f 6778785f 8_.DW.ref.__gxx_
-  0x000002e0 70657273 6f6e616c 6974795f 7630005f personality_v0._
-  0x000002f0 5a4e5374 375f5f63 78783131 31326261 ZNSt7__cxx1112ba
-  0x00000300 7369635f 73747269 6e674963 53743131 sic_stringIcSt11
-  0x00000310 63686172 5f747261 69747349 63455361 char_traitsIcESa
-  0x00000320 49634545 395f4d5f 61737369 676e4552 IcEE9_M_assignER
-  0x00000330 4b53345f 005f5a64 6c50766d 005f556e KS4_._ZdlPvm._Un
-  0x00000340 77696e64 5f526573 756d6500 5f5a4e31 wind_Resume._ZN1
-  0x00000350 31617269 74686d65 74696361 38467261 1arithmetica8Fra
-  0x00000360 6374696f 6e433145 524b4e53 74375f5f ctionC1ERKNSt7__
-  0x00000370 63787831 31313262 61736963 5f737472 cxx1112basic_str
-  0x00000380 696e6749 63537431 31636861 725f7472 ingIcSt11char_tr
-  0x00000390 61697473 49634553 61496345 45455338 aitsIcESaIcEEES8
-  0x000003a0 5f005f5a 4e313161 72697468 6d657469 _._ZN11arithmeti
-  0x000003b0 63613846 72616374 696f6e43 3245524b ca8FractionC2ERK
-  0x000003c0 4e537437 5f5f6378 78313131 32626173 NSt7__cxx1112bas
-  0x000003d0 69635f73 7472696e 67496353 74313163 ic_stringIcSt11c
-  0x000003e0 6861725f 74726169 74734963 45536149 har_traitsIcESaI
-  0x000003f0 63454545 00706172 73655f66 72616374 cEEE.parse_fract
-  0x00000400 696f6e00 7374726c 656e005f 5a4e5374 ion.strlen._ZNSt
-  0x00000410 375f5f63 78783131 31326261 7369635f 7__cxx1112basic_
-  0x00000420 73747269 6e674963 53743131 63686172 stringIcSt11char
-  0x00000430 5f747261 69747349 63455361 49634545 _traitsIcESaIcEE
-  0x00000440 31305f4d 5f726570 6c616365 456d6d50 10_M_replaceEmmP
-  0x00000450 4b636d00 64656c65 74655f66 72616374 Kcm.delete_fract
-  0x00000460 696f6e00 5f5a4e31 31617269 74686d65 ion._ZN11arithme
-  0x00000470 74696361 38467261 6374696f 6e433145 tica8FractionC1E
-  0x00000480 524b4e53 74375f5f 63787831 31313262 RKNSt7__cxx1112b
-  0x00000490 61736963 5f737472 696e6749 63537431 asic_stringIcSt1
-  0x000004a0 31636861 725f7472 61697473 49634553 1char_traitsIcES
-  0x000004b0 61496345 4545005f 5a4e3131 61726974 aIcEEE._ZN11arit
-  0x000004c0 686d6574 69636138 46726163 74696f6e hmetica8Fraction
-  0x000004d0 43324550 4b63005f 5a4e3131 61726974 C2EPKc._ZN11arit
-  0x000004e0 686d6574 69636138 46726163 74696f6e hmetica8Fraction
-  0x000004f0 43314550 4b63005f 5a4e3131 61726974 C1EPKc._ZN11arit
-  0x00000500 686d6574 69636138 46726163 74696f6e hmetica8Fraction
-  0x00000510 43324552 4b386672 61637469 6f6e005f C2ERK8fraction._
-  0x00000520 5a4e3131 61726974 686d6574 69636138 ZN11arithmetica8
-  0x00000530 46726163 74696f6e 43314552 4b386672 FractionC1ERK8fr
-  0x00000540 61637469 6f6e005f 5a4e3131 61726974 action._ZN11arit
-  0x00000550 686d6574 69636138 46726163 74696f6e hmetica8Fraction
-  0x00000560 39746f5f 73747269 6e674235 63787831 9to_stringB5cxx1
-  0x00000570 31457600 5f5a4e53 74375f5f 63787831 1Ev._ZNSt7__cxx1
-  0x00000580 31313262 61736963 5f737472 696e6749 112basic_stringI
-  0x00000590 63537431 31636861 725f7472 61697473 cSt11char_traits
-  0x000005a0 49634553 61496345 45395f4d 5f617070 IcESaIcEE9_M_app
-  0x000005b0 656e6445 504b636d 005f5a4e 5374375f endEPKcm._ZNSt7_
-  0x000005c0 5f637878 31313132 62617369 635f7374 _cxx1112basic_st
-  0x000005d0 72696e67 49635374 31316368 61725f74 ringIcSt11char_t
-  0x000005e0 72616974 73496345 53614963 4545395f raitsIcESaIcEE9_
-  0x000005f0 4d5f6372 65617465 45526d6d 006d656d M_createERmm.mem
-  0x00000600 63707900 5f5a5374 31395f5f 7468726f cpy._ZSt19__thro
-  0x00000610 775f6c6f 6769635f 6572726f 72504b63 w_logic_errorPKc
-  0x00000620 005f5a53 7432305f 5f746872 6f775f6c ._ZSt20__throw_l
-  0x00000630 656e6774 685f6572 726f7250 4b63005f ength_errorPKc._
-  0x00000640 5f737461 636b5f63 686b5f66 61696c00 _stack_chk_fail.
-  0x00000650 5f5a4e31 31617269 74686d65 74696361 _ZN11arithmetica
-  0x00000660 38467261 6374696f 6e443245 76005f5a 8FractionD2Ev._Z
-  0x00000670 4e313161 72697468 6d657469 63613846 N11arithmetica8F
-  0x00000680 72616374 696f6e44 31457600 5f5a4e31 ractionD1Ev._ZN1
-  0x00000690 31617269 74686d65 74696361 38467261 1arithmetica8Fra
-  0x000006a0 6374696f 6e706c45 524b5330 5f006361 ctionplERKS0_.ca
-  0x000006b0 6c6c6f63 00737472 63707900 6164645f lloc.strcpy.add_
-  0x000006c0 66726163 74696f6e 005f5a4e 31316172 fraction._ZN11ar
-  0x000006d0 6974686d 65746963 61384672 61637469 ithmetica8Fracti
-  0x000006e0 6f6e6d69 45524b53 305f0073 75627472 onmiERKS0_.subtr
-  0x000006f0 6163745f 66726163 74696f6e 005f5a4e act_fraction._ZN
-  0x00000700 31316172 6974686d 65746963 61384672 11arithmetica8Fr
-  0x00000710 61637469 6f6e6d6c 45524b53 305f006d actionmlERKS0_.m
-  0x00000720 756c7469 706c795f 66726163 74696f6e ultiply_fraction
-  0x00000730 005f5a4e 31316172 6974686d 65746963 ._ZN11arithmetic
-  0x00000740 61384672 61637469 6f6e6476 45524b53 a8FractiondvERKS
-  0x00000750 305f005f 5a4e3131 61726974 686d6574 0_._ZN11arithmet
-  0x00000760 69636138 46726163 74696f6e 65714552 ica8FractioneqER
-  0x00000770 4b53305f 005f5a4e 4b537437 5f5f6378 KS0_._ZNKSt7__cx
-  0x00000780 78313131 32626173 69635f73 7472696e x1112basic_strin
-  0x00000790 67496353 74313163 6861725f 74726169 gIcSt11char_trai
-  0x000007a0 74734963 45536149 63454537 636f6d70 tsIcESaIcEE7comp
-  0x000007b0 61726545 504b6300 6d656d63 6d70005f areEPKc.memcmp._
-  0x000007c0 5a657152 4b4e3131 61726974 686d6574 ZeqRKN11arithmet
-  0x000007d0 69636138 46726163 74696f6e 4553325f ica8FractionES2_
-  0x000007e0 005f5a6c 74524b4e 31316172 6974686d ._ZltRKN11arithm
-  0x000007f0 65746963 61384672 61637469 6f6e4553 etica8FractionES
-  0x00000800 325f00                              2_.
+  0x00000200 325f2e63 6f6c6400 2e4c4335 002e4c43 2_.cold..LC5..LC
+  0x00000210 37002e4c 4334002e 4c433600 2e4c4331 7..LC4..LC6..LC1
+  0x00000220 33002e4c 43313400 5f5a4e31 31617269 3..LC14._ZN11ari
+  0x00000230 74686d65 74696361 38467261 6374696f thmetica8Fractio
+  0x00000240 6e443545 76005f5a 4e313161 72697468 nD5Ev._ZN11arith
+  0x00000250 6d657469 63613846 72616374 696f6e43 metica8FractionC
+  0x00000260 32457600 5f5a4e31 31617269 74686d65 2Ev._ZN11arithme
+  0x00000270 74696361 38467261 6374696f 6e433145 tica8FractionC1E
+  0x00000280 76005f5a 4e313161 72697468 6d657469 v._ZN11arithmeti
+  0x00000290 63613846 72616374 696f6e43 3245524b ca8FractionC2ERK
+  0x000002a0 4e537437 5f5f6378 78313131 32626173 NSt7__cxx1112bas
+  0x000002b0 69635f73 7472696e 67496353 74313163 ic_stringIcSt11c
+  0x000002c0 6861725f 74726169 74734963 45536149 har_traitsIcESaI
+  0x000002d0 63454545 53385f00 44572e72 65662e5f cEEES8_.DW.ref._
+  0x000002e0 5f677878 5f706572 736f6e61 6c697479 _gxx_personality
+  0x000002f0 5f763000 5f5a4e53 74375f5f 63787831 _v0._ZNSt7__cxx1
+  0x00000300 31313262 61736963 5f737472 696e6749 112basic_stringI
+  0x00000310 63537431 31636861 725f7472 61697473 cSt11char_traits
+  0x00000320 49634553 61496345 45395f4d 5f617373 IcESaIcEE9_M_ass
+  0x00000330 69676e45 524b5334 5f005f5a 646c5076 ignERKS4_._ZdlPv
+  0x00000340 6d005f55 6e77696e 645f5265 73756d65 m._Unwind_Resume
+  0x00000350 005f5a4e 31316172 6974686d 65746963 ._ZN11arithmetic
+  0x00000360 61384672 61637469 6f6e4331 45524b4e a8FractionC1ERKN
+  0x00000370 5374375f 5f637878 31313132 62617369 St7__cxx1112basi
+  0x00000380 635f7374 72696e67 49635374 31316368 c_stringIcSt11ch
+  0x00000390 61725f74 72616974 73496345 53614963 ar_traitsIcESaIc
+  0x000003a0 45454553 385f005f 5a4e3131 61726974 EEES8_._ZN11arit
+  0x000003b0 686d6574 69636138 46726163 74696f6e hmetica8Fraction
+  0x000003c0 43324552 4b4e5374 375f5f63 78783131 C2ERKNSt7__cxx11
+  0x000003d0 31326261 7369635f 73747269 6e674963 12basic_stringIc
+  0x000003e0 53743131 63686172 5f747261 69747349 St11char_traitsI
+  0x000003f0 63455361 49634545 45007061 7273655f cESaIcEEE.parse_
+  0x00000400 66726163 74696f6e 00737472 6c656e00 fraction.strlen.
+  0x00000410 5f5a4e53 74375f5f 63787831 31313262 _ZNSt7__cxx1112b
+  0x00000420 61736963 5f737472 696e6749 63537431 asic_stringIcSt1
+  0x00000430 31636861 725f7472 61697473 49634553 1char_traitsIcES
+  0x00000440 61496345 4531305f 4d5f7265 706c6163 aIcEE10_M_replac
+  0x00000450 65456d6d 504b636d 0064656c 6574655f eEmmPKcm.delete_
+  0x00000460 66726163 74696f6e 005f5a4e 31316172 fraction._ZN11ar
+  0x00000470 6974686d 65746963 61384672 61637469 ithmetica8Fracti
+  0x00000480 6f6e4331 45524b4e 5374375f 5f637878 onC1ERKNSt7__cxx
+  0x00000490 31313132 62617369 635f7374 72696e67 1112basic_string
+  0x000004a0 49635374 31316368 61725f74 72616974 IcSt11char_trait
+  0x000004b0 73496345 53614963 45454500 5f5a4e31 sIcESaIcEEE._ZN1
+  0x000004c0 31617269 74686d65 74696361 38467261 1arithmetica8Fra
+  0x000004d0 6374696f 6e433245 504b6300 5f5a4e31 ctionC2EPKc._ZN1
+  0x000004e0 31617269 74686d65 74696361 38467261 1arithmetica8Fra
+  0x000004f0 6374696f 6e433145 504b6300 5f5a4e31 ctionC1EPKc._ZN1
+  0x00000500 31617269 74686d65 74696361 38467261 1arithmetica8Fra
+  0x00000510 6374696f 6e433245 524b3866 72616374 ctionC2ERK8fract
+  0x00000520 696f6e00 5f5a4e31 31617269 74686d65 ion._ZN11arithme
+  0x00000530 74696361 38467261 6374696f 6e433145 tica8FractionC1E
+  0x00000540 524b3866 72616374 696f6e00 5f5a4e31 RK8fraction._ZN1
+  0x00000550 31617269 74686d65 74696361 38467261 1arithmetica8Fra
+  0x00000560 6374696f 6e39746f 5f737472 696e6742 ction9to_stringB
+  0x00000570 35637878 31314576 005f5a4e 4b537437 5cxx11Ev._ZNKSt7
+  0x00000580 5f5f6378 78313131 32626173 69635f73 __cxx1112basic_s
+  0x00000590 7472696e 67496353 74313163 6861725f tringIcSt11char_
+  0x000005a0 74726169 74734963 45536149 63454537 traitsIcESaIcEE7
+  0x000005b0 636f6d70 61726545 504b6300 5f5a4e53 compareEPKc._ZNS
+  0x000005c0 74375f5f 63787831 31313262 61736963 t7__cxx1112basic
+  0x000005d0 5f737472 696e6749 63537431 31636861 _stringIcSt11cha
+  0x000005e0 725f7472 61697473 49634553 61496345 r_traitsIcESaIcE
+  0x000005f0 45395f4d 5f637265 61746545 526d6d00 E9_M_createERmm.
+  0x00000600 6d656d63 7079005f 5a4e5374 375f5f63 memcpy._ZNSt7__c
+  0x00000610 78783131 31326261 7369635f 73747269 xx1112basic_stri
+  0x00000620 6e674963 53743131 63686172 5f747261 ngIcSt11char_tra
+  0x00000630 69747349 63455361 49634545 37726573 itsIcESaIcEE7res
+  0x00000640 65727665 456d005f 5a4e5374 375f5f63 erveEm._ZNSt7__c
+  0x00000650 78783131 31326261 7369635f 73747269 xx1112basic_stri
+  0x00000660 6e674963 53743131 63686172 5f747261 ngIcSt11char_tra
+  0x00000670 69747349 63455361 49634545 395f4d5f itsIcESaIcEE9_M_
+  0x00000680 61707065 6e644550 4b636d00 5f5a5374 appendEPKcm._ZSt
+  0x00000690 31395f5f 7468726f 775f6c6f 6769635f 19__throw_logic_
+  0x000006a0 6572726f 72504b63 005f5f73 7461636b errorPKc.__stack
+  0x000006b0 5f63686b 5f666169 6c005f5a 53743230 _chk_fail._ZSt20
+  0x000006c0 5f5f7468 726f775f 6c656e67 74685f65 __throw_length_e
+  0x000006d0 72726f72 504b6300 5f5a4e31 31617269 rrorPKc._ZN11ari
+  0x000006e0 74686d65 74696361 38467261 6374696f thmetica8Fractio
+  0x000006f0 6e443245 76005f5a 4e313161 72697468 nD2Ev._ZN11arith
+  0x00000700 6d657469 63613846 72616374 696f6e44 metica8FractionD
+  0x00000710 31457600 5f5a4e31 31617269 74686d65 1Ev._ZN11arithme
+  0x00000720 74696361 38467261 6374696f 6e706c45 tica8FractionplE
+  0x00000730 524b5330 5f006361 6c6c6f63 00737472 RKS0_.calloc.str
+  0x00000740 63707900 6164645f 66726163 74696f6e cpy.add_fraction
+  0x00000750 005f5a4e 31316172 6974686d 65746963 ._ZN11arithmetic
+  0x00000760 61384672 61637469 6f6e6d69 45524b53 a8FractionmiERKS
+  0x00000770 305f0073 75627472 6163745f 66726163 0_.subtract_frac
+  0x00000780 74696f6e 005f5a4e 31316172 6974686d tion._ZN11arithm
+  0x00000790 65746963 61384672 61637469 6f6e6d6c etica8Fractionml
+  0x000007a0 45524b53 305f006d 756c7469 706c795f ERKS0_.multiply_
+  0x000007b0 66726163 74696f6e 005f5a4e 31316172 fraction._ZN11ar
+  0x000007c0 6974686d 65746963 61384672 61637469 ithmetica8Fracti
+  0x000007d0 6f6e6476 45524b53 305f005f 5a4e3131 ondvERKS0_._ZN11
+  0x000007e0 61726974 686d6574 69636138 46726163 arithmetica8Frac
+  0x000007f0 74696f6e 65714552 4b53305f 006d656d tioneqERKS0_.mem
+  0x00000800 636d7000 5f5a6571 524b4e31 31617269 cmp._ZeqRKN11ari
+  0x00000810 74686d65 74696361 38467261 6374696f thmetica8Fractio
+  0x00000820 6e455332 5f005f5a 6c74524b 4e313161 nES2_._ZltRKN11a
+  0x00000830 72697468 6d657469 63613846 72616374 rithmetica8Fract
+  0x00000840 696f6e45 53325f00                   ionES2_.
```

### Comparing `arithmetica-py-1.0.206/src/python-module/libbasic_math_operations.a` & `arithmetica-py-1.0.207/src/python-module/libbasic_math_operations.a`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.206/src/python-module/module.c` & `arithmetica-py-1.0.207/src/python-module/module.c`

 * *Files identical despite different names*

