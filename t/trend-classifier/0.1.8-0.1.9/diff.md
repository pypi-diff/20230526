# Comparing `tmp/trend_classifier-0.1.8.tar.gz` & `tmp/trend_classifier-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trend_classifier-0.1.8.tar", max compression
+gzip compressed data, was "trend_classifier-0.1.9.tar", max compression
```

## Comparing `trend_classifier-0.1.8.tar` & `trend_classifier-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1088 2022-09-07 08:15:06.671955 trend_classifier-0.1.8/LICENSE
--rw-r--r--   0        0        0     3504 2022-09-09 16:47:19.460957 trend_classifier-0.1.8/README.md
--rw-r--r--   0        0        0     1643 2023-02-01 19:45:19.718759 trend_classifier-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      379 2022-09-09 12:12:57.092322 trend_classifier-0.1.8/trend_classifier/__init__.py
--rw-r--r--   0        0        0     1331 2023-02-01 19:44:57.539293 trend_classifier-0.1.8/trend_classifier/configuration.py
--rw-r--r--   0        0        0      270 2022-09-08 21:29:53.596745 trend_classifier-0.1.8/trend_classifier/models.py
--rw-r--r--   0        0        0     4022 2022-09-13 07:33:04.087718 trend_classifier-0.1.8/trend_classifier/segment.py
--rw-r--r--   0        0        0    12840 2023-02-01 19:44:57.539918 trend_classifier-0.1.8/trend_classifier/segmentation.py
--rw-r--r--   0        0        0       80 2022-09-08 18:24:27.521352 trend_classifier-0.1.8/trend_classifier/types.py
--rw-r--r--   0        0        0     4042 2023-02-01 19:44:57.540415 trend_classifier-0.1.8/trend_classifier/visuals.py
--rw-r--r--   0        0        0     4365 1970-01-01 00:00:00.000000 trend_classifier-0.1.8/setup.py
--rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 trend_classifier-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1088 2022-09-07 08:15:06.671955 trend_classifier-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3560 2023-02-02 04:55:39.702100 trend_classifier-0.1.9/README.md
+-rw-r--r--   0        0        0     1667 2023-05-26 08:46:44.757029 trend_classifier-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      379 2022-09-09 12:12:57.092322 trend_classifier-0.1.9/trend_classifier/__init__.py
+-rw-r--r--   0        0        0     1331 2023-02-01 19:44:57.539293 trend_classifier-0.1.9/trend_classifier/configuration.py
+-rw-r--r--   0        0        0      270 2022-09-08 21:29:53.596745 trend_classifier-0.1.9/trend_classifier/models.py
+-rw-r--r--   0        0        0     4022 2022-09-13 07:33:04.087718 trend_classifier-0.1.9/trend_classifier/segment.py
+-rw-r--r--   0        0        0    12840 2023-02-01 19:44:57.539918 trend_classifier-0.1.9/trend_classifier/segmentation.py
+-rw-r--r--   0        0        0       80 2022-09-08 18:24:27.521352 trend_classifier-0.1.9/trend_classifier/types.py
+-rw-r--r--   0        0        0     4042 2023-02-01 19:44:57.540415 trend_classifier-0.1.9/trend_classifier/visuals.py
+-rw-r--r--   0        0        0     4752 1970-01-01 00:00:00.000000 trend_classifier-0.1.9/PKG-INFO
```

### Comparing `trend_classifier-0.1.8/LICENSE` & `trend_classifier-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trend_classifier-0.1.8/README.md` & `trend_classifier-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -78,12 +78,13 @@
     )
 ```
 export results to tabular format (pandas DataFrame):
 ```python
 seg.segments.to_dataframe()
 ```
 ![](https://github.com/izikeros/trend_classifier/blob/main/img/to_dataframe.jpg?raw=true)
-(not all columns are shown)
+
+(**NOTE:** for clarity reasons, not all columns are shown in the screenshot above)
 
 ## License
 
 [MIT](LICENSE) © [Krystian Safjan](https://safjan.com/).
```

### Comparing `trend_classifier-0.1.8/pyproject.toml` & `trend_classifier-0.1.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "trend-classifier"
-version = "0.1.8"
+version = "0.1.9"
 description = "Package for automated signal segmentation, trend classification and analysis."
 authors = ["Krystian Safjan <ksafjan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["trend", "timeseries", "classification", "segmentation", "analysis", "algotrading", "finance"]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -18,15 +18,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
     'Topic :: Utilities',
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<=3.12"
 matplotlib = "^3.5.3"
 pydantic = "^1.10.1"
 numpy = "^1.23.2"
 pandas = "^1.4.4"
 
 [tool.poetry.group.dev.dependencies]
 tox = "^3.25.1"
@@ -42,14 +42,15 @@
 devtools = "^0.9.0"
 plotly = "^5.10.0"
 yfinance = "^0.1.74"
 pandas = "^1.4.3"
 pip-upgrader = "^1.4.15"
 pytest-sugar = "^0.9.5"
 pytest-cov = "^3.0.0"
+pip-upgrade = "^0.0.6"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.2"
 pytest-icdiff = "^0.6"
 pytest-clarity = "^1.0.1"
 
 [tool.scriv]
```

### Comparing `trend_classifier-0.1.8/trend_classifier/configuration.py` & `trend_classifier-0.1.9/trend_classifier/configuration.py`

 * *Files identical despite different names*

### Comparing `trend_classifier-0.1.8/trend_classifier/segment.py` & `trend_classifier-0.1.9/trend_classifier/segment.py`

 * *Files identical despite different names*

### Comparing `trend_classifier-0.1.8/trend_classifier/segmentation.py` & `trend_classifier-0.1.9/trend_classifier/segmentation.py`

 * *Files identical despite different names*

### Comparing `trend_classifier-0.1.8/trend_classifier/visuals.py` & `trend_classifier-0.1.9/trend_classifier/visuals.py`

 * *Files identical despite different names*

### Comparing `trend_classifier-0.1.8/setup.py` & `trend_classifier-0.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,119 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: trend-classifier
+Version: 0.1.9
+Summary: Package for automated signal segmentation, trend classification and analysis.
+License: MIT
+Keywords: trend,timeseries,classification,segmentation,analysis,algotrading,finance
+Author: Krystian Safjan
+Author-email: ksafjan@gmail.com
+Requires-Python: >=3.8,<=3.12
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
+Requires-Dist: numpy (>=1.23.2,<2.0.0)
+Requires-Dist: pandas (>=1.4.4,<2.0.0)
+Requires-Dist: pydantic (>=1.10.1,<2.0.0)
+Description-Content-Type: text/markdown
+
+# Trend classifier
+![](https://img.shields.io/pypi/v/trend-classifier.svg)
+![](https://img.shields.io/pypi/pyversions/trend-classifier.svg)
+![](https://img.shields.io/pypi/l/trend-classifier.svg)
+![](https://img.shields.io/pypi/dm/trend-classifier.svg)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/izikeros/trend_classifier/main.svg)](https://results.pre-commit.ci/latest/github/izikeros/trend_classifier/main)
+[![Black formatter](https://github.com/izikeros/trend_classifier/actions/workflows/black.yml/badge.svg)](https://github.com/izikeros/trend_classifier/actions/workflows/black.yml)
+[![flake8](https://github.com/izikeros/trend_classifier/actions/workflows/flake8.yml/badge.svg)](https://github.com/izikeros/trend_classifier/actions/workflows/flake8.yml)
+[![pytest](https://github.com/izikeros/trend_classifier/actions/workflows/pytest.yml/badge.svg)](https://github.com/izikeros/trend_classifier/actions/workflows/pytest.yml)
+[![Maintainability](https://api.codeclimate.com/v1/badges/081a20bb8a5201cd8faf/maintainability)](https://codeclimate.com/github/izikeros/trend_classifier/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/081a20bb8a5201cd8faf/test_coverage)](https://codeclimate.com/github/izikeros/trend_classifier/test_coverage)
+
+Library for automated signal segmentation, trend classification and analysis.
+
+## Installation
+
+1. The package is pip-installable. To install it, run:
+
+   ```sh
+   pip3 install trend-classifier
+   ```
+
+## Usage
+### Pandas DataFrame Input
+usage:
+```python
+import yfinance as yf
+from trend_classifier import Segmenter
+
+# download data from yahoo finance
+df = yf.download("AAPL", start="2018-09-15", end="2022-09-05", interval="1d", progress=False)
+
+x_in = list(range(0, len(df.index.tolist()), 1))
+y_in = df["Adj Close"].tolist()
+
+seg = Segmenter(x_in, y_in, n=20)
+seg.calculate_segments()
+```
+
+For graphical output use `Segmenter.plot_segments()`:
+```python
+seg.plot_segments()
+```
+
+![Segmentation example](https://github.com/izikeros/trend_classifier/blob/main/img/screenshoot_1.jpg?raw=true)
+
+After calling method `Segmenter.calculate_segments()` segments are identified and information is stored in `Segmenter.segments` as list of Segment objects. Each Segment object. Each Segment object has attributes such as 'start', 'stop' - range of indices for the extracted segment, slope and many more attributes that might be helpful for further analysis.
+
+Exemplary info on one segment:
+```python
+from devtools import debug
+debug(seg.segments[3])
+```
+and you should see something like this:
+```
+    seg.segments[3]: Segment(
+        start=154,
+        stop=177,
+        slope=-0.37934038908585044,
+        offset=109.54630934894907,
+        slopes=[
+            -0.45173184100846725,
+            -0.22564684358754555,
+            0.15555037018051593,
+            0.34801127785130714,
+        ],
+        offsets=[
+            121.65628807526804,
+            83.56079272220015,
+            17.32660986821478,
+            -17.86417581658647,
+        ],
+        slopes_std=0.31334199799377654,
+        offsets_std=54.60900279722876,
+        std=0.933497081795997,
+        span=82.0,
+        reason_for_new_segment='offset',
+    )
+```
+export results to tabular format (pandas DataFrame):
+```python
+seg.segments.to_dataframe()
+```
+![](https://github.com/izikeros/trend_classifier/blob/main/img/to_dataframe.jpg?raw=true)
 
-packages = \
-['trend_classifier']
+(**NOTE:** for clarity reasons, not all columns are shown in the screenshot above)
 
-package_data = \
-{'': ['*']}
+## License
 
-install_requires = \
-['matplotlib>=3.5.3,<4.0.0',
- 'numpy>=1.23.2,<2.0.0',
- 'pandas>=1.4.4,<2.0.0',
- 'pydantic>=1.10.1,<2.0.0']
-
-setup_kwargs = {
-    'name': 'trend-classifier',
-    'version': '0.1.8',
-    'description': 'Package for automated signal segmentation, trend classification and analysis.',
-    'long_description': '# Trend classifier\n![](https://img.shields.io/pypi/v/trend-classifier.svg)\n![](https://img.shields.io/pypi/pyversions/trend-classifier.svg)\n![](https://img.shields.io/pypi/l/trend-classifier.svg)\n![](https://img.shields.io/pypi/dm/trend-classifier.svg)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/izikeros/trend_classifier/main.svg)](https://results.pre-commit.ci/latest/github/izikeros/trend_classifier/main)\n[![Black formatter](https://github.com/izikeros/trend_classifier/actions/workflows/black.yml/badge.svg)](https://github.com/izikeros/trend_classifier/actions/workflows/black.yml)\n[![flake8](https://github.com/izikeros/trend_classifier/actions/workflows/flake8.yml/badge.svg)](https://github.com/izikeros/trend_classifier/actions/workflows/flake8.yml)\n[![pytest](https://github.com/izikeros/trend_classifier/actions/workflows/pytest.yml/badge.svg)](https://github.com/izikeros/trend_classifier/actions/workflows/pytest.yml)\n[![Maintainability](https://api.codeclimate.com/v1/badges/081a20bb8a5201cd8faf/maintainability)](https://codeclimate.com/github/izikeros/trend_classifier/maintainability)\n[![Test Coverage](https://api.codeclimate.com/v1/badges/081a20bb8a5201cd8faf/test_coverage)](https://codeclimate.com/github/izikeros/trend_classifier/test_coverage)\n\nLibrary for automated signal segmentation, trend classification and analysis.\n\n## Installation\n\n1. The package is pip-installable. To install it, run:\n\n   ```sh\n   pip3 install trend-classifier\n   ```\n\n## Usage\n### Pandas DataFrame Input\nusage:\n```python\nimport yfinance as yf\nfrom trend_classifier import Segmenter\n\n# download data from yahoo finance\ndf = yf.download("AAPL", start="2018-09-15", end="2022-09-05", interval="1d", progress=False)\n\nx_in = list(range(0, len(df.index.tolist()), 1))\ny_in = df["Adj Close"].tolist()\n\nseg = Segmenter(x_in, y_in, n=20)\nseg.calculate_segments()\n```\n\nFor graphical output use `Segmenter.plot_segments()`:\n```python\nseg.plot_segments()\n```\n\n![Segmentation example](https://github.com/izikeros/trend_classifier/blob/main/img/screenshoot_1.jpg?raw=true)\n\nAfter calling method `Segmenter.calculate_segments()` segments are identified and information is stored in `Segmenter.segments` as list of Segment objects. Each Segment object. Each Segment object has attributes such as \'start\', \'stop\' - range of indices for the extracted segment, slope and many more attributes that might be helpful for further analysis.\n\nExemplary info on one segment:\n```python\nfrom devtools import debug\ndebug(seg.segments[3])\n```\nand you should see something like this:\n```\n    seg.segments[3]: Segment(\n        start=154,\n        stop=177,\n        slope=-0.37934038908585044,\n        offset=109.54630934894907,\n        slopes=[\n            -0.45173184100846725,\n            -0.22564684358754555,\n            0.15555037018051593,\n            0.34801127785130714,\n        ],\n        offsets=[\n            121.65628807526804,\n            83.56079272220015,\n            17.32660986821478,\n            -17.86417581658647,\n        ],\n        slopes_std=0.31334199799377654,\n        offsets_std=54.60900279722876,\n        std=0.933497081795997,\n        span=82.0,\n        reason_for_new_segment=\'offset\',\n    )\n```\nexport results to tabular format (pandas DataFrame):\n```python\nseg.segments.to_dataframe()\n```\n![](https://github.com/izikeros/trend_classifier/blob/main/img/to_dataframe.jpg?raw=true)\n(not all columns are shown)\n\n## License\n\n[MIT](LICENSE) © [Krystian Safjan](https://safjan.com/).\n',
-    'author': 'Krystian Safjan',
-    'author_email': 'ksafjan@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
+[MIT](LICENSE) © [Krystian Safjan](https://safjan.com/).
 
-
-setup(**setup_kwargs)
```

