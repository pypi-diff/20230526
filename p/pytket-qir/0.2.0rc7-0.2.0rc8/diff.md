# Comparing `tmp/pytket_qir-0.2.0rc7-py3-none-any.whl.zip` & `tmp/pytket_qir-0.2.0rc8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17967 bytes, number of entries: 12
--rw-r--r--  2.0 unx      858 b- defN 23-May-25 11:19 pytket/qir/__init__.py
--rw-r--r--  2.0 unx       69 b- defN 23-May-25 11:19 pytket/qir/_metadata.py
--rw-r--r--  2.0 unx      711 b- defN 23-May-25 11:19 pytket/qir/conversion/__init__.py
--rw-r--r--  2.0 unx     3352 b- defN 23-May-25 11:19 pytket/qir/conversion/api.py
--rw-r--r--  2.0 unx    28971 b- defN 23-May-25 11:19 pytket/qir/conversion/conversion.py
--rw-r--r--  2.0 unx     4082 b- defN 23-May-25 11:19 pytket/qir/conversion/gatesets.py
--rw-r--r--  2.0 unx     1481 b- defN 23-May-25 11:19 pytket/qir/conversion/module.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-25 11:19 pytket_qir-0.2.0rc7.dist-info/LICENSE
--rw-r--r--  2.0 unx     4183 b- defN 23-May-25 11:19 pytket_qir-0.2.0rc7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-25 11:19 pytket_qir-0.2.0rc7.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-25 11:19 pytket_qir-0.2.0rc7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1017 b- defN 23-May-25 11:19 pytket_qir-0.2.0rc7.dist-info/RECORD
-12 files, 56180 bytes uncompressed, 16245 bytes compressed:  71.1%
+Zip file size: 18119 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      858 b- defN 23-May-26 14:26 pytket/qir/__init__.py
+-rw-r--r--  2.0 unx       69 b- defN 23-May-26 14:27 pytket/qir/_metadata.py
+-rw-r--r--  2.0 unx      711 b- defN 23-May-26 14:26 pytket/qir/conversion/__init__.py
+-rw-r--r--  2.0 unx     3352 b- defN 23-May-26 14:26 pytket/qir/conversion/api.py
+-rw-r--r--  2.0 unx    30282 b- defN 23-May-26 14:26 pytket/qir/conversion/conversion.py
+-rw-r--r--  2.0 unx     4082 b- defN 23-May-26 14:26 pytket/qir/conversion/gatesets.py
+-rw-r--r--  2.0 unx     1481 b- defN 23-May-26 14:26 pytket/qir/conversion/module.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-26 14:27 pytket_qir-0.2.0rc8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4183 b- defN 23-May-26 14:27 pytket_qir-0.2.0rc8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 14:27 pytket_qir-0.2.0rc8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-26 14:27 pytket_qir-0.2.0rc8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1017 b- defN 23-May-26 14:27 pytket_qir-0.2.0rc8.dist-info/RECORD
+12 files, 57491 bytes uncompressed, 16397 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: pytket/qir/conversion/gatesets.py
 Comment: 
 
 Filename: pytket/qir/conversion/module.py
 Comment: 
 
-Filename: pytket_qir-0.2.0rc7.dist-info/LICENSE
+Filename: pytket_qir-0.2.0rc8.dist-info/LICENSE
 Comment: 
 
-Filename: pytket_qir-0.2.0rc7.dist-info/METADATA
+Filename: pytket_qir-0.2.0rc8.dist-info/METADATA
 Comment: 
 
-Filename: pytket_qir-0.2.0rc7.dist-info/WHEEL
+Filename: pytket_qir-0.2.0rc8.dist-info/WHEEL
 Comment: 
 
-Filename: pytket_qir-0.2.0rc7.dist-info/top_level.txt
+Filename: pytket_qir-0.2.0rc8.dist-info/top_level.txt
 Comment: 
 
-Filename: pytket_qir-0.2.0rc7.dist-info/RECORD
+Filename: pytket_qir-0.2.0rc8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytket/qir/_metadata.py

```diff
@@ -1,2 +1,2 @@
-__extension_version__ = "0.2.0rc7"
+__extension_version__ = "0.2.0rc8"
 __extension_name__ = "pytket-qir"
```

## pytket/qir/conversion/conversion.py

```diff
@@ -174,20 +174,49 @@
             "reg2var",
             pyqir.FunctionType(
                 pyqir.IntType(self.module.module.context, qir_int_type),
                 [pyqir.IntType(self.module.module.context, 1)] * qir_int_type,
             ),
         )
 
-        # void __quantum__rt__int_record_output(i64)
-        self.record_output = self.module.module.add_external_function(
+        self.reg_const = {}
+
+        for creg in self.circuit.c_registers:
+            reg_name = creg[0].reg_name
+            self.reg_const[reg_name] = self.module.module.add_byte_string(
+                str.encode(reg_name)
+            )
+
+            # void __quantum__rt__int_record_output(i64)
+        self.record_output_i64 = self.module.module.add_external_function(
             "__quantum__rt__int_record_output",
             pyqir.FunctionType(
                 pyqir.Type.void(self.module.module.context),
-                [pyqir.IntType(self.module.module.context, qir_int_type)],
+                [
+                    pyqir.IntType(self.module.module.context, qir_int_type),
+                    pyqir.PointerType(pyqir.IntType(self.module.module.context, 8)),
+                ],
+            ),
+        )
+
+        # void __quantum__rt__tuple_start_record_output()
+        self.record_output_start = self.module.module.add_external_function(
+            "__quantum__rt__tuple_start_record_output",
+            pyqir.FunctionType(
+                pyqir.Type.void(self.module.module.context),
+                [],
+            ),
+        )
+
+        # void __quantum__rt__tuple_end_record_output()
+        self.record_output_end = self.module.module.add_external_function(
+            "__quantum__rt__tuple_end_record_output",
+            pyqir.FunctionType(
+                pyqir.Type.void(self.module.module.context),
+                [],
             ),
         )
 
         self.barrier: List[Optional[pyqir.Function]] = [None] * (
             self.circuit.n_qubits + 1
         )
         self.order: List[Optional[pyqir.Function]] = [None] * (
@@ -743,17 +772,29 @@
                     elif params:
                         get_gate(*params, *qubits)
                     elif results:
                         get_gate(*qubits, results)
                     else:
                         get_gate(*qubits)
         if record_output:
+
+            self.module.builder.call(
+                self.record_output_start,
+                [],
+            )
+
             for creg in self.circuit.c_registers:
                 reg_name = creg[0].reg_name
                 self.module.builder.call(
-                    self.record_output,
+                    self.record_output_i64,
                     [
                         self.ssa_vars[reg_name],
+                        self.reg_const[reg_name],
                     ],
                 )
 
+            self.module.builder.call(
+                self.record_output_end,
+                [],
+            )
+
         return module
```

## Comparing `pytket_qir-0.2.0rc7.dist-info/LICENSE` & `pytket_qir-0.2.0rc8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytket_qir-0.2.0rc7.dist-info/METADATA` & `pytket_qir-0.2.0rc8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-qir
-Version: 0.2.0rc7
+Version: 0.2.0rc8
 Summary: Extension for pytket, providing functions for conversion into to qir
 Author: TKET development team
 Author-email: tket-support@cambridgequantum.com
 License: Apache 2
 Project-URL: Documentation, https://cqcl.github.io/pytket-qir/api/index.html
 Project-URL: Source, https://github.com/CQCL/pytket-qir
 Project-URL: Tracker, https://github.com/CQCL/pytket-qir/issues
```

## Comparing `pytket_qir-0.2.0rc7.dist-info/RECORD` & `pytket_qir-0.2.0rc8.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pytket/qir/__init__.py,sha256=3AXz2dN6Yg20zM3YYtMAPf6ZCidAG-opHomVhmU93w4,858
-pytket/qir/_metadata.py,sha256=Q72S2KNuOD41_lqKXljKX1mo5gC5O05w_ibxpNJ3AN4,69
+pytket/qir/_metadata.py,sha256=_eC4ecZVUur4-IjCTiB0CUgH_SvFq5CM9ICJsUbdxDg,69
 pytket/qir/conversion/__init__.py,sha256=kKuV2wCn6cMf_iVQhlsu28cH8K4dDCUqwUXlHF_FpUg,711
 pytket/qir/conversion/api.py,sha256=FznzHIsaAJCAbhQxc3iudc173sWYI9bz1i8dJJtl9L0,3352
-pytket/qir/conversion/conversion.py,sha256=ppjPAhsBEfBtnAe-8u-izrW4zpG5O_11X6rt7rbTekc,28971
+pytket/qir/conversion/conversion.py,sha256=c8xtnC7zNntqiiPuEE1EjO9ApxS7IaXnesjJVL6YL60,30282
 pytket/qir/conversion/gatesets.py,sha256=Ix1KkLlFoyE1LkoUs0J7wFikZXT9w5jYs8mnTQnZURM,4082
 pytket/qir/conversion/module.py,sha256=fj8iHNh27_-wbjKkO9JdnKkExiRAhMWXTzjVP9kCwtA,1481
-pytket_qir-0.2.0rc7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pytket_qir-0.2.0rc7.dist-info/METADATA,sha256=_qbFKZ4Y-huQLdPB_A9e1EOCjcPfOotglGJgrg5G6X4,4183
-pytket_qir-0.2.0rc7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pytket_qir-0.2.0rc7.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
-pytket_qir-0.2.0rc7.dist-info/RECORD,,
+pytket_qir-0.2.0rc8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pytket_qir-0.2.0rc8.dist-info/METADATA,sha256=3nyE2s3mXKqknbnOLBUL0Uj9EtZw_SwZDrefD0iKJr4,4183
+pytket_qir-0.2.0rc8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pytket_qir-0.2.0rc8.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
+pytket_qir-0.2.0rc8.dist-info/RECORD,,
```

