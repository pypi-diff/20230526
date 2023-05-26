# Comparing `tmp/bkw_python-0.0.3.tar.gz` & `tmp/bkw_python-0.0.4.tar.gz`

## Comparing `bkw_python-0.0.3.tar` & `bkw_python-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bkw_python-0.0.3/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bkw_python-0.0.3/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bkw_python-0.0.3/.pytest_cache/README.md
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 bkw_python-0.0.3/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 bkw_python-0.0.3/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 bkw_python-0.0.3/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 bkw_python-0.0.3/src/bkw_python/__init__.py
--rw-r--r--   0        0        0     9351 2020-02-02 00:00:00.000000 bkw_python-0.0.3/src/bkw_python/data_models.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 bkw_python-0.0.3/src/bkw_python/exceptions.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 bkw_python-0.0.3/src/bkw_python/operation_helpers.py
--rw-r--r--   0        0        0    11055 2020-02-02 00:00:00.000000 bkw_python-0.0.3/src/bkw_python/operation_models.py
--rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 bkw_python-0.0.3/src/bkw_python/rest_adapter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bkw_python-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 bkw_python-0.0.3/tests/test_parse_document.py
--rw-r--r--   0        0        0    14260 2020-02-02 00:00:00.000000 bkw_python-0.0.3/tests/test_run_claims_register.py
--rw-r--r--   0        0        0    41437 2020-02-02 00:00:00.000000 bkw_python-0.0.3/tests/test_search_cases.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 bkw_python-0.0.3/tests/test_search_parties.py
--rw-r--r--   0        0        0    66377 2020-02-02 00:00:00.000000 bkw_python-0.0.3/tests/document_parsing_responses/18_42694_secured_claims.json
--rw-r--r--   0        0        0    26212 2020-02-02 00:00:00.000000 bkw_python-0.0.3/tests/document_parsing_responses/22_24902_no_secured_claims.json
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 bkw_python-0.0.3/LICENSE
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bkw_python-0.0.3/README.md
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 bkw_python-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 bkw_python-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bkw_python-0.0.4/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bkw_python-0.0.4/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bkw_python-0.0.4/.pytest_cache/README.md
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bkw_python-0.0.4/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 bkw_python-0.0.4/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 bkw_python-0.0.4/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 bkw_python-0.0.4/src/bkw_python/__init__.py
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 bkw_python-0.0.4/src/bkw_python/data_models.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 bkw_python-0.0.4/src/bkw_python/exceptions.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 bkw_python-0.0.4/src/bkw_python/operation_helpers.py
+-rw-r--r--   0        0        0    11055 2020-02-02 00:00:00.000000 bkw_python-0.0.4/src/bkw_python/operation_models.py
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 bkw_python-0.0.4/src/bkw_python/rest_adapter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bkw_python-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 bkw_python-0.0.4/tests/test_parse_document.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 bkw_python-0.0.4/tests/test_parse_document_schedule_i.py
+-rw-r--r--   0        0        0    14260 2020-02-02 00:00:00.000000 bkw_python-0.0.4/tests/test_run_claims_register.py
+-rw-r--r--   0        0        0    41437 2020-02-02 00:00:00.000000 bkw_python-0.0.4/tests/test_search_cases.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 bkw_python-0.0.4/tests/test_search_parties.py
+-rw-r--r--   0        0        0    66377 2020-02-02 00:00:00.000000 bkw_python-0.0.4/tests/document_parsing_responses/18_42694_secured_claims.json
+-rw-r--r--   0        0        0    29900 2020-02-02 00:00:00.000000 bkw_python-0.0.4/tests/document_parsing_responses/20-40596-schedule-i.json
+-rw-r--r--   0        0        0    14491 2020-02-02 00:00:00.000000 bkw_python-0.0.4/tests/document_parsing_responses/22-20465-schedule-i.json
+-rw-r--r--   0        0        0    26212 2020-02-02 00:00:00.000000 bkw_python-0.0.4/tests/document_parsing_responses/22_24902_no_secured_claims.json
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 bkw_python-0.0.4/LICENSE
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bkw_python-0.0.4/README.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 bkw_python-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 bkw_python-0.0.4/PKG-INFO
```

### Comparing `bkw_python-0.0.3/.pytest_cache/v/cache/nodeids` & `bkw_python-0.0.4/.pytest_cache/v/cache/nodeids`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8421052631578947%*

 * *Differences: {'insert': '[(3, '*

 * *           "'tests/test_parse_document_schedule_i.py::test_run_parse_document_no_secured_claims'), "*

 * *           '(4, '*

 * *           "'tests/test_parse_document_schedule_i.py::test_run_parse_document_schedule_i_basic'), "*

 * *           '(5, '*

 * *           "'tests/test_parse_document_schedule_i.py::test_run_parse_document_schedule_i_basic_2'), "*

 * *           '(6, '*

 * *           "'tests/test_parse_document_schedule_i.py::test_run_parse_document_schedule_i_basic_single_income'), "*

 * *           '(7, '*

 * *     […]*

```diff
@@ -1,11 +1,17 @@
 [
     "tests/test_parse_document.py::test_run_parse_document_basic",
     "tests/test_parse_document.py::test_run_parse_document_no_secured_claims",
     "tests/test_parse_document.py::test_run_parse_document_secured_claims",
+    "tests/test_parse_document_schedule_i.py::test_run_parse_document_no_secured_claims",
+    "tests/test_parse_document_schedule_i.py::test_run_parse_document_schedule_i_basic",
+    "tests/test_parse_document_schedule_i.py::test_run_parse_document_schedule_i_basic_2",
+    "tests/test_parse_document_schedule_i.py::test_run_parse_document_schedule_i_basic_single_income",
+    "tests/test_parse_document_schedule_i.py::test_run_parse_document_schedule_i_multiple_income",
+    "tests/test_parse_document_schedule_i.py::test_run_parse_document_secured_claims",
     "tests/test_run_claims_register.py::test_run_claims_register_basic",
     "tests/test_run_claims_register.py::test_run_claims_register_cache",
     "tests/test_run_claims_register.py::test_run_claims_register_invalid_case",
     "tests/test_run_claims_register.py::test_run_claims_register_invalid_case_format",
     "tests/test_run_claims_register.py::test_run_claims_register_no_cache",
     "tests/test_search_cases.py::test_case_schema_parsing_multiple",
     "tests/test_search_cases.py::test_case_schema_parsing_single",
```

### Comparing `bkw_python-0.0.3/src/bkw_python/data_models.py` & `bkw_python-0.0.4/src/bkw_python/data_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -224,17 +224,70 @@
     @validator("dateAdded", "dateTerminated", pre=True)
     def parse_date(cls, value):
         return datetime.strptime(
             value,
             "%Y-%m-%d"
         )
 
-
 class Bkml(BaseModel):
     form106D: Optional[Form106D]
+    formIm: Optional[Union[FormIm, List[FormIm]]]
+
+class FormIm(BaseModel):
+    document: Optional[str]
+    page: Optional[str]
+    data: Optional[FormImData]
+
+class FormImData(BaseModel):
+    maritalStatus: Optional[str]
+    employment: Optional[FormImEmployment]
+    income: Optional[FormImIncome]
+
+class FormImEmployment(BaseModel):
+    debtor1: Optional[FormImDebtorEmployment]
+    debtor2: Optional[FormImDebtorEmployment]
+
+class FormImIncome(BaseModel):
+    line2: Optional[FormImDebtorIncome]
+    line3: Optional[FormImDebtorIncome]
+    line4: Optional[FormImDebtorIncome]
+    line5a: Optional[FormImDebtorIncome]
+    line5b: Optional[FormImDebtorIncome]
+    line5c: Optional[FormImDebtorIncome]
+    line5d: Optional[FormImDebtorIncome]
+    line5e: Optional[FormImDebtorIncome]
+    line5f: Optional[FormImDebtorIncome]
+    line5g: Optional[FormImDebtorIncome]
+    line5h: Optional[Dict]
+    line6: Optional[FormImDebtorIncome]
+    line7: Optional[FormImDebtorIncome]
+    line8a: Optional[FormImDebtorIncome]
+    line8b: Optional[FormImDebtorIncome]
+    line8c: Optional[FormImDebtorIncome]
+    line8d: Optional[FormImDebtorIncome]
+    line8e: Optional[FormImDebtorIncome]
+    line8f: Optional[Dict]
+    line8g: Optional[FormImDebtorIncome]
+    line8h: Optional[Dict]
+    line9: Optional[FormImDebtorIncome]
+    line10: Optional[FormImDebtorIncome]
+    line11: Optional[Dict]
+    line12: Optional[str]
+    line13: Optional[Dict]
+
+class FormImDebtorIncome(BaseModel):
+    debtor1: Optional[str]
+    debtor2: Optional[str]
+    total: Optional[str] # only happens in line 10 that I know of
+
+class FormImDebtorEmployment(BaseModel):
+    occupation: Optional[str]
+    employerName: Optional[str]
+    employerAddress: Optional[str]
+    howLongEmployed: Optional[str]
 
 class Form106D(BaseModel):
     document: Optional[str]
     page: Optional[str]
     data: Optional[Form106DData] = None
 
     def get_secured_claims(self) -> List[Form106DSecuredClaim]:
@@ -282,11 +335,17 @@
 Claim.update_forward_refs()
 Creditor.update_forward_refs()
 Document.update_forward_refs()
 Filing.update_forward_refs()
 Party.update_forward_refs()
 
 Bkml.update_forward_refs()
+FormIm.update_forward_refs()
+FormImData.update_forward_refs()
+FormImEmployment.update_forward_refs()
+FormImDebtorEmployment.update_forward_refs()
+FormImIncome.update_forward_refs()
+FormImDebtorIncome.update_forward_refs()
 Form106D.update_forward_refs()
 Form106DData.update_forward_refs()
 Form106DDataPart1.update_forward_refs()
 Form106DSecuredClaim.update_forward_refs()
```

### Comparing `bkw_python-0.0.3/src/bkw_python/operation_models.py` & `bkw_python-0.0.4/src/bkw_python/operation_models.py`

 * *Files identical despite different names*

### Comparing `bkw_python-0.0.3/src/bkw_python/rest_adapter.py` & `bkw_python-0.0.4/src/bkw_python/rest_adapter.py`

 * *Files identical despite different names*

### Comparing `bkw_python-0.0.3/tests/test_parse_document.py` & `bkw_python-0.0.4/tests/test_parse_document.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -34,8 +34,8 @@
     assert bkml.form106D
     assert bkml.form106D.get_secured_claims()
     assert bkml.form106D.get_secured_claims()[0].amount == "12540.00"
     assert bkml.form106D.get_secured_claims()[0].collateral == "12900.00"
     assert bkml.form106D.get_secured_claims()[1].amount == "215009.37"
     assert bkml.form106D.get_secured_claims()[1].collateral == "607000.00"
     assert bkml.form106D.get_secured_claims()[2].amount == "21368.42"
-    assert bkml.form106D.get_secured_claims()[2].collateral == "21368.42"
+    assert bkml.form106D.get_secured_claims()[2].collateral == "21368.42"
```

### Comparing `bkw_python-0.0.3/tests/test_run_claims_register.py` & `bkw_python-0.0.4/tests/test_run_claims_register.py`

 * *Files identical despite different names*

### Comparing `bkw_python-0.0.3/tests/test_search_cases.py` & `bkw_python-0.0.4/tests/test_search_cases.py`

 * *Files identical despite different names*

### Comparing `bkw_python-0.0.3/tests/test_search_parties.py` & `bkw_python-0.0.4/tests/test_search_parties.py`

 * *Files identical despite different names*

### Comparing `bkw_python-0.0.3/tests/document_parsing_responses/18_42694_secured_claims.json` & `bkw_python-0.0.4/tests/document_parsing_responses/18_42694_secured_claims.json`

 * *Files identical despite different names*

### Comparing `bkw_python-0.0.3/tests/document_parsing_responses/22_24902_no_secured_claims.json` & `bkw_python-0.0.4/tests/document_parsing_responses/22_24902_no_secured_claims.json`

 * *Files identical despite different names*

### Comparing `bkw_python-0.0.3/LICENSE` & `bkw_python-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bkw_python-0.0.3/README.md` & `bkw_python-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bkw_python-0.0.3/pyproject.toml` & `bkw_python-0.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bkw-python"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Ryan Stone", email="ryan@bankruptcywatch.com" },
 ]
 description = "A limited Python client for the BankruptcyWatch API."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `bkw_python-0.0.3/PKG-INFO` & `bkw_python-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bkw-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: A limited Python client for the BankruptcyWatch API.
 Project-URL: Homepage, https://github.com/ryangustaf/bkw-python
 Project-URL: Bug Tracker, https://github.com/ryangustaf/bkw-python/issues
 Author-email: Ryan Stone <ryan@bankruptcywatch.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

