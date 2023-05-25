# Comparing `tmp/isqrt-1.0.2.tar.gz` & `tmp/isqrt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isqrt-1.0.2.tar", last modified: Sun Jul 31 19:05:35 2022, max compression
+gzip compressed data, was "isqrt-1.1.0.tar", last modified: Thu May 25 21:58:53 2023, max compression
```

## Comparing `isqrt-1.0.2.tar` & `isqrt-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-07-31 19:05:35.865306 isqrt-1.0.2/
--rw-rw-rw-   0        0        0     1091 2022-06-13 22:32:37.000000 isqrt-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     5612 2022-07-31 19:05:35.865040 isqrt-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5171 2022-07-24 03:56:27.000000 isqrt-1.0.2/README.rst
--rw-rw-rw-   0        0        0      788 2022-07-30 19:52:51.000000 isqrt-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-07-31 19:05:35.865503 isqrt-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-07-31 19:05:35.851111 isqrt-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2022-07-31 19:05:35.856475 isqrt-1.0.2/src/isqrt/
--rw-rw-rw-   0        0        0       81 2022-06-13 22:32:37.000000 isqrt-1.0.2/src/isqrt/__init__.py
--rw-rw-rw-   0        0        0     4770 2022-07-31 18:04:49.000000 isqrt-1.0.2/src/isqrt/isqrt.py
-drwxrwxrwx   0        0        0        0 2022-07-31 19:05:35.864952 isqrt-1.0.2/src/isqrt.egg-info/
--rw-rw-rw-   0        0        0     5612 2022-07-31 19:05:35.000000 isqrt-1.0.2/src/isqrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2022-07-31 19:05:35.000000 isqrt-1.0.2/src/isqrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-31 19:05:35.000000 isqrt-1.0.2/src/isqrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2022-07-31 19:05:35.000000 isqrt-1.0.2/src/isqrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-07-31 19:05:35.000000 isqrt-1.0.2/src/isqrt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 21:58:53.341580 isqrt-1.1.0/
+-rw-rw-rw-   0        0        0     1091 2022-06-13 22:32:37.000000 isqrt-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5874 2023-05-25 21:58:53.341580 isqrt-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5433 2023-05-25 21:56:47.000000 isqrt-1.1.0/README.rst
+-rw-rw-rw-   0        0        0      789 2023-05-05 03:50:09.000000 isqrt-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 21:58:53.341580 isqrt-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 21:58:53.327574 isqrt-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 21:58:53.332077 isqrt-1.1.0/src/isqrt/
+-rw-rw-rw-   0        0        0       81 2022-06-13 22:32:37.000000 isqrt-1.1.0/src/isqrt/__init__.py
+-rw-rw-rw-   0        0        0     4786 2022-08-20 07:16:43.000000 isqrt-1.1.0/src/isqrt/isqrt.py
+drwxrwxrwx   0        0        0        0 2023-05-25 21:58:53.341580 isqrt-1.1.0/src/isqrt.egg-info/
+-rw-rw-rw-   0        0        0     5874 2023-05-25 21:58:53.000000 isqrt-1.1.0/src/isqrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-05-25 21:58:53.000000 isqrt-1.1.0/src/isqrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 21:58:53.000000 isqrt-1.1.0/src/isqrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-05-25 21:58:53.000000 isqrt-1.1.0/src/isqrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-25 21:58:53.000000 isqrt-1.1.0/src/isqrt.egg-info/top_level.txt
```

### Comparing `isqrt-1.0.2/LICENSE` & `isqrt-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isqrt-1.0.2/PKG-INFO` & `isqrt-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isqrt
-Version: 1.0.2
+Version: 1.1.0
 Summary: Efficient pure-Python implementation of the integer square root function.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/lapets/isqrt
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -40,57 +40,71 @@
 
 .. |math_isqrt| replace:: ``math.isqrt``
 .. _math_isqrt: https://docs.python.org/3/library/math.html#math.isqrt
 
 .. |math_sqrt| replace:: ``math.sqrt``
 .. _math_sqrt: https://docs.python.org/3/library/math.html#math.sqrt
 
-**The built-in** |math_isqrt|_ **function was introduced in Python 3.8 and should normally be used instead of the function defined in this library.** To provide the best performance possible while retaining backwards-compatible behavior for this library, the implementation in this library invokes |math_isqrt|_ when it is available. If |math_isqrt|_ is not available, this library attempts to use |math_sqrt|_ and then (if |math_sqrt|_ does not produce the correct result or the input is outside the range supported by |math_sqrt|_) defaults to a pure Python implementation in which the number of executed Python arithmetic operations is linear in the bit length of the input integer.
+**The built-in** |math_isqrt|_ **function was introduced in Python 3.8 and should normally be used instead of the function defined in this library.** To provide the best performance possible while retaining backwards-compatible behavior for this library, the implementation in this library invokes |math_isqrt|_ when it is available. If |math_isqrt|_ is not available, this library attempts to use |math_sqrt|_ and then (if |math_sqrt|_ does not produce the correct result or the input is outside the range supported by |math_sqrt|_) defaults to a pure-Python implementation in which the number of executed Python arithmetic operations is linear in the bit length of the input integer.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/isqrt>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/isqrt>`__:
+
+.. code-block:: bash
 
     python -m pip install isqrt
 
-The library can be imported in the usual way::
+The library can be imported in the usual way:
+
+.. code-block:: python
 
     from isqrt import isqrt
 
 Examples
 ^^^^^^^^
-The exported function ``isqrt`` provides a pure-Python implementation of the `integer square root <https://en.wikipedia.org/wiki/Integer_square_root>`__ algorithm::
+The exported function ``isqrt`` provides a pure-Python implementation of the `integer square root <https://en.wikipedia.org/wiki/Integer_square_root>`__ algorithm:
+
+.. code-block:: python
 
     >>> isqrt(4)
     2
     >>> isqrt(16)
     4
     >>> list(map(isqrt, range(16, 26)))
     [4, 4, 4, 4, 4, 4, 4, 4, 4, 5]
     >>> isqrt(2**30000) == 2**15000
     True
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``test``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``test``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[test,lint]
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/isqrt/isqrt.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/isqrt
 
 Acknowledgments
 ^^^^^^^^^^^^^^^
 The initial version of this function was `posted <http://stackoverflow.com/a/23279113/2738025>`__ on Stack Overflow. A `more efficient version <https://gist.github.com/castle-bravo/e841684d6bad8e0598e31862a7afcfc7>`__ was implemented by Alexander Gosselin. The implementation in this package is adapted directly from these previous implementations.
@@ -101,24 +115,32 @@
 
 Versioning
 ^^^^^^^^^^
 Beginning with version 0.10.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/isqrt>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/isqrt>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in the ``pyproject.toml`` file. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in the ``pyproject.toml`` file. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

### Comparing `isqrt-1.0.2/README.rst` & `isqrt-1.1.0/src/isqrt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: isqrt
+Version: 1.1.0
+Summary: Efficient pure-Python implementation of the integer square root function.
+Author: Andrei Lapets
+Author-email: a@lapets.io
+License: MIT
+Project-URL: Repository, https://github.com/lapets/isqrt
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: coveralls
+Provides-Extra: publish
+License-File: LICENSE
+
 =====
 isqrt
 =====
 
 Efficient pure-Python implementation of the integer square root function.
 
 |pypi| |actions| |coveralls|
@@ -24,57 +40,71 @@
 
 .. |math_isqrt| replace:: ``math.isqrt``
 .. _math_isqrt: https://docs.python.org/3/library/math.html#math.isqrt
 
 .. |math_sqrt| replace:: ``math.sqrt``
 .. _math_sqrt: https://docs.python.org/3/library/math.html#math.sqrt
 
-**The built-in** |math_isqrt|_ **function was introduced in Python 3.8 and should normally be used instead of the function defined in this library.** To provide the best performance possible while retaining backwards-compatible behavior for this library, the implementation in this library invokes |math_isqrt|_ when it is available. If |math_isqrt|_ is not available, this library attempts to use |math_sqrt|_ and then (if |math_sqrt|_ does not produce the correct result or the input is outside the range supported by |math_sqrt|_) defaults to a pure Python implementation in which the number of executed Python arithmetic operations is linear in the bit length of the input integer.
+**The built-in** |math_isqrt|_ **function was introduced in Python 3.8 and should normally be used instead of the function defined in this library.** To provide the best performance possible while retaining backwards-compatible behavior for this library, the implementation in this library invokes |math_isqrt|_ when it is available. If |math_isqrt|_ is not available, this library attempts to use |math_sqrt|_ and then (if |math_sqrt|_ does not produce the correct result or the input is outside the range supported by |math_sqrt|_) defaults to a pure-Python implementation in which the number of executed Python arithmetic operations is linear in the bit length of the input integer.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/isqrt>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/isqrt>`__:
+
+.. code-block:: bash
 
     python -m pip install isqrt
 
-The library can be imported in the usual way::
+The library can be imported in the usual way:
+
+.. code-block:: python
 
     from isqrt import isqrt
 
 Examples
 ^^^^^^^^
-The exported function ``isqrt`` provides a pure-Python implementation of the `integer square root <https://en.wikipedia.org/wiki/Integer_square_root>`__ algorithm::
+The exported function ``isqrt`` provides a pure-Python implementation of the `integer square root <https://en.wikipedia.org/wiki/Integer_square_root>`__ algorithm:
+
+.. code-block:: python
 
     >>> isqrt(4)
     2
     >>> isqrt(16)
     4
     >>> list(map(isqrt, range(16, 26)))
     [4, 4, 4, 4, 4, 4, 4, 4, 4, 5]
     >>> isqrt(2**30000) == 2**15000
     True
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``test``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``test``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[test,lint]
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/isqrt/isqrt.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/isqrt
 
 Acknowledgments
 ^^^^^^^^^^^^^^^
 The initial version of this function was `posted <http://stackoverflow.com/a/23279113/2738025>`__ on Stack Overflow. A `more efficient version <https://gist.github.com/castle-bravo/e841684d6bad8e0598e31862a7afcfc7>`__ was implemented by Alexander Gosselin. The implementation in this package is adapted directly from these previous implementations.
@@ -85,24 +115,32 @@
 
 Versioning
 ^^^^^^^^^^
 Beginning with version 0.10.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/isqrt>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/isqrt>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in the ``pyproject.toml`` file. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in the ``pyproject.toml`` file. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

### Comparing `isqrt-1.0.2/pyproject.toml` & `isqrt-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [project]
 name = "isqrt"
-version = "1.0.2"
+version = "1.1.0"
 description = "Efficient pure-Python implementation of the integer square root function."
 license = {text = "MIT"}
 authors = [
     {name = "Andrei Lapets"},
     {email = "a@lapets.io"}
 ]
 readme = "README.rst"
 requires-python = ">=3.7"
 
 [project.urls]
 Repository = "https://github.com/lapets/isqrt"
 
 [project.optional-dependencies]
 test = [
-    "pytest~=7.0",
-    "pytest-cov~=3.0"
+    "pytest~=7.2",
+    "pytest-cov~=4.0"
 ]
 lint = [
-    "pylint~=2.14.0"
+    "pylint~=2.17.0"
 ]
 coveralls = [
     "coveralls~=3.3.1"
 ]
 publish = [
-    "build~=0.8",
+    "build~=0.10",
     "twine~=4.0"
 ]
 
 [build-system]
 requires = [
-    "setuptools~=62.0"
+    "setuptools~=67.6"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --ignore=docs --cov=isqrt --cov-report term-missing"
```

### Comparing `isqrt-1.0.2/src/isqrt/isqrt.py` & `isqrt-1.1.0/src/isqrt/isqrt.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     # pylint: disable=line-too-long # Accommodate long link URLs on docstring.
     """
     Returns the largest root such that ``root**2 <= n (root + 1)**2 > n``.
     When using Python 3.8 or later, this function acts as a wrapper for the
     built-in :obj:`math.isqrt` function.
 
     For all other supported versions of Python, this function reverts to a
-    pure Python algorithm that is adapted from an
+    pure-Python algorithm that is adapted from an
     `implementation by Alexander Gosselin <https://gist.github.com/castle-bravo/e841684d6bad8e0598e31862a7afcfc7>`__,
     which is based on a `Stack Overflow answer by Tobin Fricke <http://stackoverflow.com/a/23279113/2738025>`__.
 
     >>> isqrt(4)
     2
     >>> isqrt(16)
     4
@@ -96,19 +96,19 @@
     if n is None or (not isinstance(n, int)):
         raise TypeError('input must be an integer') # pragma: no cover
 
     if n < 0:
         raise ValueError('input must be a non-negative integer') # pragma: no cover
 
     root = 0 # Running result.
-    rmdr = 0 # Running remainder n - root**2.
-    for s in reversed(range(0, n.bit_length(), 2)): # Shift n by s bits.
-        bits = n >> s & 3 # The next two most significant bits of n.
+    rmdr = 0 # Running remainder ``n - root**2``.
+    for s in reversed(range(0, n.bit_length(), 2)): # Shift ``n`` by ``s`` bits.
+        bits = n >> s & 3 # The next two most significant bits of ``n``.
         rmdr = rmdr << 2 | bits # Increase the remainder.
         cand = root << 2 | 1 # Shifted candidate root value to try.
         bit_next = int(rmdr >= cand) # The next bit in the remainder.
         root = root << 1 | bit_next # Add next bit to running result.
         rmdr -= cand * bit_next # Reduce the remainder if bit was added.
     return root
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     doctest.testmod() # pragma: no cover
```

### Comparing `isqrt-1.0.2/src/isqrt.egg-info/PKG-INFO` & `isqrt-1.1.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: isqrt
-Version: 1.0.2
-Summary: Efficient pure-Python implementation of the integer square root function.
-Author: Andrei Lapets
-Author-email: a@lapets.io
-License: MIT
-Project-URL: Repository, https://github.com/lapets/isqrt
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
 =====
 isqrt
 =====
 
 Efficient pure-Python implementation of the integer square root function.
 
 |pypi| |actions| |coveralls|
@@ -40,57 +24,71 @@
 
 .. |math_isqrt| replace:: ``math.isqrt``
 .. _math_isqrt: https://docs.python.org/3/library/math.html#math.isqrt
 
 .. |math_sqrt| replace:: ``math.sqrt``
 .. _math_sqrt: https://docs.python.org/3/library/math.html#math.sqrt
 
-**The built-in** |math_isqrt|_ **function was introduced in Python 3.8 and should normally be used instead of the function defined in this library.** To provide the best performance possible while retaining backwards-compatible behavior for this library, the implementation in this library invokes |math_isqrt|_ when it is available. If |math_isqrt|_ is not available, this library attempts to use |math_sqrt|_ and then (if |math_sqrt|_ does not produce the correct result or the input is outside the range supported by |math_sqrt|_) defaults to a pure Python implementation in which the number of executed Python arithmetic operations is linear in the bit length of the input integer.
+**The built-in** |math_isqrt|_ **function was introduced in Python 3.8 and should normally be used instead of the function defined in this library.** To provide the best performance possible while retaining backwards-compatible behavior for this library, the implementation in this library invokes |math_isqrt|_ when it is available. If |math_isqrt|_ is not available, this library attempts to use |math_sqrt|_ and then (if |math_sqrt|_ does not produce the correct result or the input is outside the range supported by |math_sqrt|_) defaults to a pure-Python implementation in which the number of executed Python arithmetic operations is linear in the bit length of the input integer.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/isqrt>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/isqrt>`__:
+
+.. code-block:: bash
 
     python -m pip install isqrt
 
-The library can be imported in the usual way::
+The library can be imported in the usual way:
+
+.. code-block:: python
 
     from isqrt import isqrt
 
 Examples
 ^^^^^^^^
-The exported function ``isqrt`` provides a pure-Python implementation of the `integer square root <https://en.wikipedia.org/wiki/Integer_square_root>`__ algorithm::
+The exported function ``isqrt`` provides a pure-Python implementation of the `integer square root <https://en.wikipedia.org/wiki/Integer_square_root>`__ algorithm:
+
+.. code-block:: python
 
     >>> isqrt(4)
     2
     >>> isqrt(16)
     4
     >>> list(map(isqrt, range(16, 26)))
     [4, 4, 4, 4, 4, 4, 4, 4, 4, 5]
     >>> isqrt(2**30000) == 2**15000
     True
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``test``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``test``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[test,lint]
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/isqrt/isqrt.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/isqrt
 
 Acknowledgments
 ^^^^^^^^^^^^^^^
 The initial version of this function was `posted <http://stackoverflow.com/a/23279113/2738025>`__ on Stack Overflow. A `more efficient version <https://gist.github.com/castle-bravo/e841684d6bad8e0598e31862a7afcfc7>`__ was implemented by Alexander Gosselin. The implementation in this package is adapted directly from these previous implementations.
@@ -101,24 +99,32 @@
 
 Versioning
 ^^^^^^^^^^
 Beginning with version 0.10.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/isqrt>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/isqrt>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in the ``pyproject.toml`` file. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in the ``pyproject.toml`` file. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

