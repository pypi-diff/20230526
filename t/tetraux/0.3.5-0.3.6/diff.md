# Comparing `tmp/tetraux-0.3.5-cp39-cp39-win_amd64.whl.zip` & `tmp/tetraux-0.3.6-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 413753 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat   225280 b- defN 23-Apr-01 12:30 tetraux.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat       95 b- defN 23-Apr-01 12:30 tetraux-0.3.5.data/platlib/.load-order-tetraux-0.3.5
--rw-rw-rw-  2.0 fat   306688 b- defN 23-Apr-01 12:30 tetraux-0.3.5.data/platlib/concrt140-ee6441d54902364ca4e9860bce396cc7.dll
--rw-rw-rw-  2.0 fat   611328 b- defN 23-Apr-01 12:30 tetraux-0.3.5.data/platlib/msvcp140-22eeac616fa56c2d2c96c1251d58388a.dll
--rw-rw-rw-  2.0 fat      448 b- defN 23-Apr-01 12:30 tetraux-0.3.5.dist-info/DELVEWHEEL
--rw-rw-rw-  2.0 fat      493 b- defN 23-Apr-01 12:30 tetraux-0.3.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      842 b- defN 23-Apr-01 12:30 tetraux-0.3.5.dist-info/RECORD
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-01 12:30 tetraux-0.3.5.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-01 12:30 tetraux-0.3.5.dist-info/WHEEL
-9 files, 1145282 bytes uncompressed, 412277 bytes compressed:  64.0%
+Zip file size: 414147 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat   225792 b- defN 23-May-26 16:50 tetraux.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat       93 b- defN 23-May-26 16:50 tetraux-0.3.6.data/platlib/.load-order-tetraux-0.3.6
+-rw-rw-rw-  2.0 fat   306688 b- defN 23-May-26 16:50 tetraux-0.3.6.data/platlib/concrt140-ee6441d54902364ca4e9860bce396cc7.dll
+-rw-rw-rw-  2.0 fat   611328 b- defN 23-May-26 16:50 tetraux-0.3.6.data/platlib/msvcp140-41f8deb5d6517c32be84db89c4f92b0f.dll
+-rw-rw-rw-  2.0 fat      448 b- defN 23-May-26 16:50 tetraux-0.3.6.dist-info/DELVEWHEEL
+-rw-rw-rw-  2.0 fat      493 b- defN 23-May-26 16:50 tetraux-0.3.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      842 b- defN 23-May-26 16:50 tetraux-0.3.6.dist-info/RECORD
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-26 16:50 tetraux-0.3.6.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-26 16:50 tetraux-0.3.6.dist-info/WHEEL
+9 files, 1145792 bytes uncompressed, 412671 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: tetraux.cp39-win_amd64.pyd
 Comment: 
 
-Filename: tetraux-0.3.5.data/platlib/.load-order-tetraux-0.3.5
+Filename: tetraux-0.3.6.data/platlib/.load-order-tetraux-0.3.6
 Comment: 
 
-Filename: tetraux-0.3.5.data/platlib/concrt140-ee6441d54902364ca4e9860bce396cc7.dll
+Filename: tetraux-0.3.6.data/platlib/concrt140-ee6441d54902364ca4e9860bce396cc7.dll
 Comment: 
 
-Filename: tetraux-0.3.5.data/platlib/msvcp140-22eeac616fa56c2d2c96c1251d58388a.dll
+Filename: tetraux-0.3.6.data/platlib/msvcp140-41f8deb5d6517c32be84db89c4f92b0f.dll
 Comment: 
 
-Filename: tetraux-0.3.5.dist-info/DELVEWHEEL
+Filename: tetraux-0.3.6.dist-info/DELVEWHEEL
 Comment: 
 
-Filename: tetraux-0.3.5.dist-info/METADATA
+Filename: tetraux-0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: tetraux-0.3.5.dist-info/RECORD
+Filename: tetraux-0.3.6.dist-info/RECORD
 Comment: 
 
-Filename: tetraux-0.3.5.dist-info/top_level.txt
+Filename: tetraux-0.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: tetraux-0.3.5.dist-info/WHEEL
+Filename: tetraux-0.3.6.dist-info/WHEEL
 Comment: 
 
 Zip file comment:
```

## Comparing `tetraux-0.3.5.data/platlib/concrt140-ee6441d54902364ca4e9860bce396cc7.dll` & `tetraux-0.3.6.data/platlib/concrt140-ee6441d54902364ca4e9860bce396cc7.dll`

 * *Files 0% similar despite different names*

### objdump

```diff
@@ -25,15 +25,15 @@
 MajorImageVersion	10
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		0004e000
 SizeOfHeaders		00000400
-CheckSum		0005077e
+CheckSum		0004cd26
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00004160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 					GUARD_CF
 SizeOfStackReserve	0000000000100000
@@ -64,15 +64,15 @@
 There is an import table in .rdata at 0x180042bbc
 
 The Import Tables (interpreted .rdata section contents)
  vma:            Hint    Time      Forward  DLL       First
                  Table   Stamp     Chain    Name      Thunk
  00042bbc	00042f20 00000000 00000000 00043dc6 0002f298
 
-	DLL Name: msvcp140-22eeac616fa56c2d2c96c1251d58388a.dll
+	DLL Name: msvcp140-41f8deb5d6517c32be84db89c4f92b0f.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	43118	  652  ?_Xbad_function_call@std@@YAXXZ
 	4313a	  398  ?GetCurrentThreadId@platform@details@Concurrency@@YAJXZ
 	43174	 1412  _Mtx_init_in_situ
 	43188	 1409  _Mtx_destroy_in_situ
 	431a0	 1413  _Mtx_lock
 	431ac	 1417  _Mtx_unlock
@@ -10857,17 +10857,17 @@
 	  69c0: 51 75 65 72 79 50 65 72 66 6f 72 6d 61 6e 63 65
 	  69d0: 43 6f 75 6e 74 65 72 00 2b 02 47 65 74 43 75 72
 	  69e0: 72 65 6e 74 50 72 6f 63 65 73 73 49 64 00 01 03
 	  69f0: 47 65 74 53 79 73 74 65 6d 54 69 6d 65 41 73 46
 	  6a00: 69 6c 65 54 69 6d 65 00 2c 01 44 69 73 61 62 6c
 	  6a10: 65 54 68 72 65 61 64 4c 69 62 72 61 72 79 43 61
 	  6a20: 6c 6c 73 00 4b 45 52 4e 45 4c 33 32 2e 64 6c 6c
-	  6a30: 00 00 6d 73 76 63 70 31 34 30 2d 32 32 65 65 61
-	  6a40: 63 36 31 36 66 61 35 36 63 32 64 32 63 39 36 63
-	  6a50: 31 32 35 31 64 35 38 33 38 38 61 2e 64 6c 6c 00
+	  6a30: 00 00 6d 73 76 63 70 31 34 30 2d 34 31 66 38 64
+	  6a40: 65 62 35 64 36 35 31 37 63 33 32 62 65 38 34 64
+	  6a50: 62 38 39 63 34 66 39 32 62 30 66 2e 64 6c 6c 00
  0000000180039cec (rva: 00039cec): 000000018002d480 - 000000018002d4a3
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
  0000000180039cec also used for function at 000000018002d4c8
  0000000180039cc8 (rva: 00039cc8): 000000018002d4ec - 000000018002d528
 	Version: 1, Flags: none
@@ -99901,25 +99901,26 @@
    180043dc0:	cs fs insb (%dx),%es:(%rdi)
    180043dc3:	insb   (%dx),%es:(%rdi)
    180043dc4:	add    %al,(%rax)
    180043dc6:	insl   (%dx),%es:(%rdi)
    180043dc7:	jae    0x180043e3f
    180043dc9:	movsxd 0x31(%rax),%esi
    180043dcc:	xor    $0x30,%al
-   180043dce:	sub    $0x65653232,%eax
+   180043dce:	sub    $0x38663134,%eax
    180043dd3:	(bad)
-   180043dd4:	movsxd (%rsi),%esi
-   180043dd6:	xor    %esi,(%rsi)
-   180043dd8:	data16 (bad)
-   180043dda:	xor    $0x64326336,%eax
-   180043ddf:	xor    0x39(%rbx),%ah
-   180043de2:	ss movsxd (%rcx),%esi
-   180043de5:	xor    0x38356431(%rip),%dh        # 0x1b839a21c
-   180043deb:	xor    (%rax),%edi
-   180043ded:	cmp    %ah,0x2e(%rcx)
+   180043dda:	xor    %esi,(%rdi)
+   180043ddc:	movsxd (%rbx),%esi
+   180043dde:	xor    0x65(%rdx),%ah
+   180043de1:	cmp    %dh,(%rsp,%riz,2)
+   180043de4:	(bad)
+   180043de5:	cmp    %bh,(%rcx)
+   180043de7:	movsxd (%rsi,%riz,2),%esi
+   180043dea:	cmp    %esi,(%rdx)
+   180043dec:	(bad)
+   180043ded:	xor    %ah,0x2e(%rsi)
    180043df0:	fs insb (%dx),%es:(%rdi)
    180043df2:	insb   (%dx),%es:(%rdi)
 	...
 
 Disassembly of section .data:
 
 0000000180044000 <.data>:
```

## Comparing `tetraux-0.3.5.data/platlib/msvcp140-22eeac616fa56c2d2c96c1251d58388a.dll` & `tetraux-0.3.6.data/platlib/msvcp140-41f8deb5d6517c32be84db89c4f92b0f.dll`

 * *Files identical despite different names*

