# Comparing `tmp/mathslib-2.8.0.tar.gz` & `tmp/mathslib-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathslib-2.8.0.tar", last modified: Sun May 14 10:16:15 2023, max compression
+gzip compressed data, was "mathslib-2.9.0.tar", last modified: Fri May 26 11:05:05 2023, max compression
```

## Comparing `mathslib-2.8.0.tar` & `mathslib-2.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 10:16:15.927414 mathslib-2.8.0/
--rw-rw-rw-   0        0        0     1211 2022-05-22 14:55:29.000000 mathslib-2.8.0/LICENSE.txt
--rw-rw-rw-   0        0        0     6734 2023-05-14 10:16:15.927414 mathslib-2.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     5813 2023-05-14 10:10:16.000000 mathslib-2.8.0/README.rst
--rw-rw-rw-   0        0        0       85 2022-05-22 15:02:53.000000 mathslib-2.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-05-14 10:16:15.930702 mathslib-2.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1560 2023-05-14 10:15:05.000000 mathslib-2.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 10:16:15.830026 mathslib-2.8.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 10:16:15.880789 mathslib-2.8.0/src/mathslib/
--rw-rw-rw-   0        0        0     1543 2022-06-10 07:50:59.000000 mathslib-2.8.0/src/mathslib/__init__.py
--rw-rw-rw-   0        0        0    15906 2023-05-14 09:39:13.000000 mathslib-2.8.0/src/mathslib/algorithms.py
--rw-rw-rw-   0        0        0     3314 2023-05-14 09:50:54.000000 mathslib-2.8.0/src/mathslib/fib.py
--rw-rw-rw-   0        0        0     9961 2023-05-14 09:49:26.000000 mathslib-2.8.0/src/mathslib/linalg.py
--rw-rw-rw-   0        0        0    19925 2023-05-14 09:50:13.000000 mathslib-2.8.0/src/mathslib/numtheory.py
--rw-rw-rw-   0        0        0    13999 2023-05-14 10:01:31.000000 mathslib-2.8.0/src/mathslib/primes.py
--rw-rw-rw-   0        0        0     5272 2023-05-14 09:45:48.000000 mathslib-2.8.0/src/mathslib/simple.py
-drwxrwxrwx   0        0        0        0 2023-05-14 10:16:15.924443 mathslib-2.8.0/src/mathslib.egg-info/
--rw-rw-rw-   0        0        0     6734 2023-05-14 10:16:15.000000 mathslib-2.8.0/src/mathslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-05-14 10:16:15.000000 mathslib-2.8.0/src/mathslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 10:16:15.000000 mathslib-2.8.0/src/mathslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-14 10:16:15.000000 mathslib-2.8.0/src/mathslib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 10:16:15.000000 mathslib-2.8.0/src/mathslib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 11:05:05.681615 mathslib-2.9.0/
+-rw-rw-rw-   0        0        0     1211 2022-05-22 14:55:29.000000 mathslib-2.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     6815 2023-05-26 11:05:05.681615 mathslib-2.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5893 2023-05-26 11:03:53.000000 mathslib-2.9.0/README.rst
+-rw-rw-rw-   0        0        0       85 2022-05-22 15:02:53.000000 mathslib-2.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-05-26 11:05:05.689993 mathslib-2.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1560 2023-05-26 11:04:09.000000 mathslib-2.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:05:05.578900 mathslib-2.9.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 11:05:05.638984 mathslib-2.9.0/src/mathslib/
+-rw-rw-rw-   0        0        0     1543 2022-06-10 07:50:59.000000 mathslib-2.9.0/src/mathslib/__init__.py
+-rw-rw-rw-   0        0        0    15906 2023-05-14 09:39:13.000000 mathslib-2.9.0/src/mathslib/algorithms.py
+-rw-rw-rw-   0        0        0     3314 2023-05-14 09:50:54.000000 mathslib-2.9.0/src/mathslib/fib.py
+-rw-rw-rw-   0        0        0     9961 2023-05-14 09:49:26.000000 mathslib-2.9.0/src/mathslib/linalg.py
+-rw-rw-rw-   0        0        0    21385 2023-05-26 11:01:11.000000 mathslib-2.9.0/src/mathslib/numtheory.py
+-rw-rw-rw-   0        0        0    13999 2023-05-14 10:01:31.000000 mathslib-2.9.0/src/mathslib/primes.py
+-rw-rw-rw-   0        0        0     5272 2023-05-14 09:45:48.000000 mathslib-2.9.0/src/mathslib/simple.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:05:05.679357 mathslib-2.9.0/src/mathslib.egg-info/
+-rw-rw-rw-   0        0        0     6815 2023-05-26 11:05:05.000000 mathslib-2.9.0/src/mathslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-05-26 11:05:05.000000 mathslib-2.9.0/src/mathslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 11:05:05.000000 mathslib-2.9.0/src/mathslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-26 11:05:05.000000 mathslib-2.9.0/src/mathslib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 11:05:05.000000 mathslib-2.9.0/src/mathslib.egg-info/top_level.txt
```

### Comparing `mathslib-2.8.0/LICENSE.txt` & `mathslib-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mathslib-2.8.0/PKG-INFO` & `mathslib-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathslib
-Version: 2.8.0
+Version: 2.9.0
 Summary: Library of Mathematical functions and Algorithms
 Home-page: https://github.com/igorvanloo/mathslib
 Author: Igor van Loo
 Author-email: igorvanloo@gmail.com
 Project-URL: Bug Reports, https://github.com/igorvanloo/mathslib/issues
 Project-URL: Source, https://github.com/igorvanloo/mathslib
 Keywords: numbertheory,maths,algorithms
@@ -44,14 +44,15 @@
 +----------------+------------------------------------------------------------+
 |numtheory.py    | * divisors_of(x, include_x)                                |
 |                | * divisors(x, n)                                           |
 |                | * continued_fraction(x)                                    |
 |                | * overall_fraction(x)                                      |
 |                | * phi(x)                                                   |
 |                | * phi_sieve(x)                                             |
+|                | * phi_sum(x)                                               |
 |                | * mobius(x)                                                |
 |                | * mobius_k_sieve(limit, k)                                 |
 |                | * count_k_free(n, k)                                       |
 |                | * ppt(limit, non_primitive)                                |
 |                | * k_smooth_numbers(max_prime, limit)                       |
 |                | * k_powerful(k, limit, count)                              |
 |                | * legendre_factorial(x)                                    |
```

### Comparing `mathslib-2.8.0/README.rst` & `mathslib-2.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 +----------------+------------------------------------------------------------+
 |numtheory.py    | * divisors_of(x, include_x)                                |
 |                | * divisors(x, n)                                           |
 |                | * continued_fraction(x)                                    |
 |                | * overall_fraction(x)                                      |
 |                | * phi(x)                                                   |
 |                | * phi_sieve(x)                                             |
+|                | * phi_sum(x)                                               |
 |                | * mobius(x)                                                |
 |                | * mobius_k_sieve(limit, k)                                 |
 |                | * count_k_free(n, k)                                       |
 |                | * ppt(limit, non_primitive)                                |
 |                | * k_smooth_numbers(max_prime, limit)                       |
 |                | * k_powerful(k, limit, count)                              |
 |                | * legendre_factorial(x)                                    |
```

### Comparing `mathslib-2.8.0/setup.py` & `mathslib-2.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (here / "README.rst").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name = "mathslib",  # Required
-    version="2.8.0",  # Required
+    version="2.9.0",  # Required
     description="Library of Mathematical functions and Algorithms",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/x-rst",  # Optional
     url="https://github.com/igorvanloo/mathslib",  # Optional
     author="Igor van Loo",  # Optional
     author_email="igorvanloo@gmail.com",  # Optional
     classifiers=[  # Optional
```

### Comparing `mathslib-2.8.0/src/mathslib/__init__.py` & `mathslib-2.9.0/src/mathslib/__init__.py`

 * *Files identical despite different names*

### Comparing `mathslib-2.8.0/src/mathslib/algorithms.py` & `mathslib-2.9.0/src/mathslib/algorithms.py`

 * *Files identical despite different names*

### Comparing `mathslib-2.8.0/src/mathslib/fib.py` & `mathslib-2.9.0/src/mathslib/fib.py`

 * *Files identical despite different names*

### Comparing `mathslib-2.8.0/src/mathslib/linalg.py` & `mathslib-2.9.0/src/mathslib/linalg.py`

 * *Files identical despite different names*

### Comparing `mathslib-2.8.0/src/mathslib/numtheory.py` & `mathslib-2.9.0/src/mathslib/numtheory.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,26 +190,77 @@
 
     :param n: An integer
 
     :returns: An array, where array[x] = phi(x)
     
     .. code-block:: python
     
-        print(phi(10)) #[0, 1, 1, 2, 2, 4, 2, 6, 4, 6, 4]
-        print(phi(20)[11:]) #[10, 4, 12, 6, 8, 8, 16, 6, 18, 8]
+        print(phi_sieve(10)) #[0, 1, 1, 2, 2, 4, 2, 6, 4, 6, 4]
+        print(phi_sieve(20)[11:]) #[10, 4, 12, 6, 8, 8, 16, 6, 18, 8]
         
     '''
     phi = [i for i in range(n + 1)]
     for p in range(2, n + 1):
         if phi[p] == p:
             phi[p] -= 1
             for i in range(2*p, n + 1, p):
                 phi[i] -= (phi[i] // p)
     return phi
 
+def phi_sum(n):
+    '''
+    Computes the `Totient Summatory Function
+    <https://en.wikipedia.org/wiki/Totient_summatory_function>`_
+    
+    The algorithm is based on `Overview of Project Euler Problem 351 <https://projecteuler.net/overview=0351>`_
+    specifically, this is an implementation of Algorithm 6, which you may view after Solving Problem 351
+
+    :param n: An integer
+
+    :returns: sum of phi(x) where x goes from 1 to n
+    
+    .. code-block:: python
+    
+        print(phi_sum(10**4)) #30397486
+        print(sum(phi(i) for i in range(1, 10**4))) #30397486
+        print(sum(phi_sieve(10**4))) #30397486
+        
+    '''
+    L = int(math.sqrt(n))
+    v = [0]*(L + 1)
+    bigV = [0]*(n//L + 1)
+    
+    for x in range(1, L + 1):
+        res = (x*(x + 1))//2
+        for g in range(2, int(math.sqrt(x)) + 1):
+            res -= v[x//g]
+        
+        for z in range(1, int(math.sqrt(x)) + 1):
+            if x//z != z:
+                res -= (x//z - x//(z + 1))*v[z]
+        
+        v[x] = res
+    
+    for x in range(n//L, 0, -1):
+        k = n//x
+        res = (k*(k + 1))//2
+        
+        for g in range(2, int(math.sqrt(k)) + 1):
+            if k//g <= L:
+                res -= v[k//g]
+            else:
+                res -= bigV[x*g]
+        
+        for z in range(1, int(math.sqrt(k)) + 1):
+            if z != k//z:
+                res -= (k//z - k//(z + 1))*v[z]
+        bigV[x] = res
+        
+    return bigV[1]
+
 def mobius(n):
     '''
     Implementation of the `Mobius function
     <https://en.wikipedia.org/wiki/M%C3%B6bius_function>`_ of n
 
     :param n: An integer
```

### Comparing `mathslib-2.8.0/src/mathslib/primes.py` & `mathslib-2.9.0/src/mathslib/primes.py`

 * *Files identical despite different names*

### Comparing `mathslib-2.8.0/src/mathslib/simple.py` & `mathslib-2.9.0/src/mathslib/simple.py`

 * *Files identical despite different names*

### Comparing `mathslib-2.8.0/src/mathslib.egg-info/PKG-INFO` & `mathslib-2.9.0/src/mathslib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathslib
-Version: 2.8.0
+Version: 2.9.0
 Summary: Library of Mathematical functions and Algorithms
 Home-page: https://github.com/igorvanloo/mathslib
 Author: Igor van Loo
 Author-email: igorvanloo@gmail.com
 Project-URL: Bug Reports, https://github.com/igorvanloo/mathslib/issues
 Project-URL: Source, https://github.com/igorvanloo/mathslib
 Keywords: numbertheory,maths,algorithms
@@ -44,14 +44,15 @@
 +----------------+------------------------------------------------------------+
 |numtheory.py    | * divisors_of(x, include_x)                                |
 |                | * divisors(x, n)                                           |
 |                | * continued_fraction(x)                                    |
 |                | * overall_fraction(x)                                      |
 |                | * phi(x)                                                   |
 |                | * phi_sieve(x)                                             |
+|                | * phi_sum(x)                                               |
 |                | * mobius(x)                                                |
 |                | * mobius_k_sieve(limit, k)                                 |
 |                | * count_k_free(n, k)                                       |
 |                | * ppt(limit, non_primitive)                                |
 |                | * k_smooth_numbers(max_prime, limit)                       |
 |                | * k_powerful(k, limit, count)                              |
 |                | * legendre_factorial(x)                                    |
```

