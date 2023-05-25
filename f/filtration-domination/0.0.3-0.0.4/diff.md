# Comparing `tmp/filtration_domination-0.0.3.tar.gz` & `tmp/filtration_domination-0.0.4.tar.gz`

## Comparing `filtration_domination-0.0.3.tar` & `filtration_domination-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      377 1970-01-01 00:00:00.000000 filtration_domination-0.0.3/Cargo.toml
--rw-r--r--   0      501       20      685 2022-12-19 15:41:56.000000 filtration_domination-0.0.3/.gitignore
--rw-r--r--   0      501       20      329 2022-12-19 15:41:56.000000 filtration_domination-0.0.3/pyproject.toml
--rw-r--r--   0      501       20     2652 2022-12-19 15:41:56.000000 filtration_domination-0.0.3/src/lib.rs
--rw-r--r--   0      501       20      653 2022-12-19 15:41:56.000000 filtration_domination-0.0.3/test.py
--rw-r--r--   0      501       20    12484 2022-12-19 15:41:56.000000 filtration_domination-0.0.3/Cargo.lock
--rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 filtration_domination-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      377 1970-01-01 00:00:00.000000 filtration_domination-0.0.4/Cargo.toml
+-rw-r--r--   0      501       20      685 2022-12-19 16:29:26.000000 filtration_domination-0.0.4/.gitignore
+-rw-r--r--   0      501       20      329 2022-12-19 16:29:26.000000 filtration_domination-0.0.4/pyproject.toml
+-rw-r--r--   0      501       20     2656 2022-12-19 16:29:26.000000 filtration_domination-0.0.4/src/lib.rs
+-rw-r--r--   0      501       20      653 2022-12-19 16:29:26.000000 filtration_domination-0.0.4/test.py
+-rw-r--r--   0      501       20    12484 2022-12-19 16:29:51.000000 filtration_domination-0.0.4/Cargo.lock
+-rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 filtration_domination-0.0.4/PKG-INFO
```

### Comparing `filtration_domination-0.0.3/.gitignore` & `filtration_domination-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `filtration_domination-0.0.3/src/lib.rs` & `filtration_domination-0.0.4/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,14 @@
     let estimator = DensityEstimator::Gaussian(bandwidth);
     Ok(estimator.estimate(&dist_matrix))
 }
 
 #[pymodule]
 fn filtration_domination(_py: Python, m: &PyModule) -> PyResult<()> {
     let utils = PyModule::new(_py, "utils")?;
-    m.add_function(wrap_pyfunction!(gaussian_density_estimation, m)?)?;
+    utils.add_function(wrap_pyfunction!(gaussian_density_estimation, m)?)?;
     m.add_submodule(utils)?;
 
     m.add_function(wrap_pyfunction!(remove_strongly_filtration_dominated, m)?)?;
     m.add_function(wrap_pyfunction!(remove_filtration_dominated, m)?)?;
     Ok(())
 }
```

### Comparing `filtration_domination-0.0.3/test.py` & `filtration_domination-0.0.4/test.py`

 * *Files identical despite different names*

### Comparing `filtration_domination-0.0.3/Cargo.lock` & `filtration_domination-0.0.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
  "rustc-hash",
  "sorted-iter",
  "thiserror",
 ]
 
 [[package]]
 name = "filtration-domination-python"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
  "filtration-domination",
  "ordered-float 3.3.0",
  "pyo3",
 ]
 
 [[package]]
```

