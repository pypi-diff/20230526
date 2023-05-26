# Comparing `tmp/stocktracer-0.2.0.tar.gz` & `tmp/stocktracer-0.3.0.tar.gz`

## Comparing `stocktracer-0.2.0.tar` & `stocktracer-0.3.0.tar`

### file list

```diff
@@ -1,70 +1,73 @@
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 stocktracer-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 stocktracer-0.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 stocktracer-0.2.0/Makefile
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 stocktracer-0.2.0/Pipfile
--rw-r--r--   0        0        0   120246 2020-02-02 00:00:00.000000 stocktracer-0.2.0/Pipfile.lock
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 stocktracer-0.2.0/SECURITY.md
--rwxr-xr-x   0        0        0      571 2020-02-02 00:00:00.000000 stocktracer-0.2.0/auto-format.sh
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 stocktracer-0.2.0/conftest.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 stocktracer-0.2.0/mkdocs.yml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 stocktracer-0.2.0/pydocktest.json
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 stocktracer-0.2.0/requirements.txt
--rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 stocktracer-0.2.0/smoke-test.sh
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 stocktracer-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 stocktracer-0.2.0/.github/pull_request_template.md
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 stocktracer-0.2.0/.github/release.yml
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 stocktracer-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 stocktracer-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 stocktracer-0.2.0/.github/workflows/cleanup.yml
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 stocktracer-0.2.0/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 stocktracer-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 stocktracer-0.2.0/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 stocktracer-0.2.0/.github/workflows/python.yml
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 stocktracer-0.2.0/.github/workflows/release-test.yml
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 stocktracer-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/getting-started.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/index.md
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/design/analysis.md
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/design/caching.md
--rw-r--r--   0        0        0    20504 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/design/data-retrieval.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/design/index.md
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/design/reference.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/design/report.md
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/javascripts/mathjax.js
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/javascripts/tablesort.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/stocktracer/__init__.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/stocktracer/__main__.py
--rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/stocktracer/cli.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/stocktracer/filter.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/stocktracer/interface.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/stocktracer/analysis/__init__.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/stocktracer/analysis/annual_reports.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/stocktracer/analysis/diluted_eps.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/stocktracer/analysis/stub.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/stocktracer/data/__init__.py
--rw-r--r--   0        0        0    23631 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/stocktracer/data/sec.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/__init__.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/test_cli.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/test_filter.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/analysis/__init__.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/analysis/test_annual_reports.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/analysis/test_diluted_eps.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/analysis/test_stub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/fixtures/network.py
--rw-r--r--   0        0        0     7126 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/fixtures/unit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/sec/__init__.py
--rw-r--r--   0        0        0     6507 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/sec/test_DataSelector.py
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/sec/test_DataSetReader.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/sec/test_filter.py
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/sec/test_network.py
--rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/src/tests/sec/test_sec.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 stocktracer-0.2.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 stocktracer-0.2.0/.gitignore
--rw-r--r--   0        0        0    14197 2020-02-02 00:00:00.000000 stocktracer-0.2.0/LICENSE
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 stocktracer-0.2.0/README.md
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 stocktracer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    21809 2020-02-02 00:00:00.000000 stocktracer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 stocktracer-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 stocktracer-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 stocktracer-0.3.0/Makefile
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 stocktracer-0.3.0/Pipfile
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 stocktracer-0.3.0/SECURITY.md
+-rwxr-xr-x   0        0        0      617 2020-02-02 00:00:00.000000 stocktracer-0.3.0/auto-format.sh
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 stocktracer-0.3.0/conftest.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 stocktracer-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 stocktracer-0.3.0/pydocktest.json
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 stocktracer-0.3.0/requirements.txt
+-rwxr-xr-x   0        0        0      757 2020-02-02 00:00:00.000000 stocktracer-0.3.0/smoke-test.sh
+-rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 stocktracer-0.3.0/verify-packaging.sh
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/release.yml
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/workflows/cleanup.yml
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/workflows/python.yml
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/workflows/release-test.yml
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/getting-started.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/index.md
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/design/analysis.md
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/design/caching.md
+-rw-r--r--   0        0        0    20504 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/design/data-retrieval.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/design/index.md
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/design/reference.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/design/report.md
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/javascripts/mathjax.js
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/javascripts/tablesort.js
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/__init__.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/__main__.py
+-rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/cli.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/filter.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/interface.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/analysis/__init__.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/analysis/annual_reports.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/analysis/diluted_eps.py
+-rw-r--r--   0        0        0     7289 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/analysis/f_score.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/analysis/stub.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/data/__init__.py
+-rw-r--r--   0        0        0    31671 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/data/sec.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/test_cli.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/test_filter.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/analysis/__init__.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/analysis/test_annual_reports.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/analysis/test_diluted_eps.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/analysis/test_f_score.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/analysis/test_stub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/fixtures/network.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/fixtures/unit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/sec/__init__.py
+-rw-r--r--   0        0        0     6507 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/sec/test_DataSelector.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/sec/test_DataSetReader.py
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/sec/test_filter.py
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/sec/test_network.py
+-rw-r--r--   0        0        0     8600 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/sec/test_sec.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.gitignore
+-rw-r--r--   0        0        0    14197 2020-02-02 00:00:00.000000 stocktracer-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 stocktracer-0.3.0/README.md
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 stocktracer-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    22066 2020-02-02 00:00:00.000000 stocktracer-0.3.0/PKG-INFO
```

### Comparing `stocktracer-0.2.0/CODE_OF_CONDUCT.md` & `stocktracer-0.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/CONTRIBUTING.md` & `stocktracer-0.3.0/CONTRIBUTING.md`

 * *Files 15% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 
 The following is a set of guidelines for the many ways you can join our collective effort.
 
 Before anything else, please take a moment to read our [Code of Conduct](CODE_OF_CONDUCT.md). We expect all participants, from full-timers to occasional tinkerers, to uphold it.
 
 ## Reporting Bugs, Asking Questions, and Suggesting Features
 
-Have a suggestion or feedback? Please go to [Issues](https://github.com/gyund/fundamental-analysis/issues) and [open a new issue](https://github.com/gyund/fundamental-analysis/issues/new). Prefix the title with a category like _"Bug:"_, _"Question:"_, or _"Feature Request:"_. Screenshots help us resolve issues and answer questions faster, so thanks for including some if you can.
+Have a suggestion or feedback? Please go to [Issues](https://github.com/gyund/fundamental-analysis/issues) and [open a new issue](https://github.com/gyund/fundamental-analysis/issues/new). Prefix the title with a category like _"Bug:"_, _"Question:"_, or _"Feature Request:"_. Logs help us resolve issues and answer questions faster, so thanks for including some if you can.
 
 ## Submitting Code Changes
 
-We use black and isort to keep our code clean. Please run `./autoformat.sh` in the project directory to cleanup code before submitting. Checks will be performed by automated tools.
+If you plan to work on an issue, coordinate with the team by commenting in the issue and discussing with maintainers before diving too deep on any sort of implementation. Committing a lot of effort only to have a PR rejected can be frustrating, so it's best to see if your ideas jive with the project for things you want to contribute back.  
+
+When submitting changes, we use black and isort to keep our code clean. Please run `./autoformat.sh` in the project directory to cleanup code before submitting. Checks will be performed by automated tools and give you a success message if the changes are expected to past all lint checks.
 
 ### Continuous Integration
 
 When opening a PR from a fork, some of the CI checks must be manually triggered by a member of the team. That means you don't need to worry if some of the CI checks are not running—we'll take care of it when we review the PR and, if there are any issues, we'll let you know.
 
 ### PR merge policy
 
 * PRs require one reviewer to approve the PR before it can be merged to the base branch
 * We keep the PR git history when merging (merge via "merge commit")
-* The reviewer who approved the PR may merge it right after approval (without waiting for the PR author) if all checks are green.
+* The reviewer who approved the PR may merge it right after approval (without waiting for the PR author) if all checks are green. 
+* The reviewer may also suggest, make changes, or decline the PR for various reasons. Know that we really appreciate and value the input and contribution effort. Start a discussion in issue tickets, PRs, or under [discussions](https://github.com/gyund/fundamental-analysis/discussions) to help plan your efforts effectively.
```

### Comparing `stocktracer-0.2.0/mkdocs.yml` & `stocktracer-0.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/requirements.txt` & `stocktracer-0.3.0/requirements.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 -i https://pypi.org/simple
+about-time==4.2.1 ; python_version >= '3.7' and python_version < '4'
+alive-progress==3.1.2
 attrs==23.1.0 ; python_version >= '3.7'
 beartype==0.14.0
 cattrs==22.2.0 ; python_version >= '3.7'
 certifi==2023.5.7 ; python_version >= '3.6'
 charset-normalizer==3.1.0 ; python_full_version >= '3.7.0'
 diskcache==5.6.1
 exceptiongroup==1.1.1 ; python_version < '3.11'
 fire==0.5.0
+grapheme==0.6.0
 idna==3.4 ; python_version >= '3.5'
 numpy==1.24.3 ; python_version >= '3.10'
 pandas==2.0.1
 platformdirs==3.5.1 ; python_version >= '3.7'
 python-dateutil==2.8.2
 pytz==2023.3
-requests==2.30.0
+requests==2.31.0
 requests-cache==1.0.1
-six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
+six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'
 tabulate==0.9.0
 termcolor==2.3.0 ; python_version >= '3.7'
 tzdata==2023.3 ; python_version >= '2'
 url-normalize==1.4.3 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
 urllib3==2.0.2 ; python_version >= '3.7'
```

### Comparing `stocktracer-0.2.0/.github/dependabot.yml` & `stocktracer-0.3.0/.github/dependabot.yml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # package ecosystems to update and where the package manifests are located.
 # Please see the documentation for all configuration options:
 # https://docs.github.com/github/administering-a-repository/configuration-options-for-dependency-updates
 
 version: 2
 updates:
   - package-ecosystem: "pip" # See documentation for possible values
-    versioning-strategy: lockfile-only
+    versioning-strategy: auto
     open-pull-requests-limit: 5
     directory: "/" # Location of package manifests
     schedule:
       interval: "weekly"
     assignees:
       - "gyund"
   - package-ecosystem: "github-actions"
```

### Comparing `stocktracer-0.2.0/.github/pull_request_template.md` & `stocktracer-0.3.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `stocktracer-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/.github/workflows/cleanup.yml` & `stocktracer-0.3.0/.github/workflows/cleanup.yml`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/.github/workflows/codeql.yml` & `stocktracer-0.3.0/.github/workflows/codeql.yml`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,28 @@
 # supported CodeQL languages.
 #
 name: "CodeQL"
 
 on:
   push:
     branches: [ "main" ]
+    paths:
+      - '**/*.py'
   pull_request:
     # The branches below must be a subset of the branches above
     branches: [ "main" ]
     types:
       - opened
       - reopened
       - synchronize
       - ready_for_review
-#   schedule:
-#     - cron: '42 16 * * 0'
+    paths:
+      - '**/*.py'
+  schedule:
+    - cron: '42 16 * * 0'
 
 concurrency:
   group: codeql-${{ github.ref }}
   cancel-in-progress: true
   
 jobs:
   analyze:
```

### Comparing `stocktracer-0.2.0/.github/workflows/docs.yml` & `stocktracer-0.3.0/.github/workflows/docs.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 name: docs 
 on:
   push:
     branches:
       - main
     paths:
+    - 'src/**'
     - 'docs/**'
     - '.github/workflows/docs.yml'
     - 'mkdocs.yml'
+    - 'Pipfile.lock'
   pull_request:
     paths:
+    - 'src/**'
     - 'docs/**'
     - '.github/workflows/docs.yml'
     - 'mkdocs.yml'
+    - 'Pipfile.lock'
 permissions:
   contents: write
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
@@ -27,14 +31,15 @@
         with:
           key: ${{ github.ref }}
           path: .cache
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install pipenv
+          pipenv lock --categories docs
           pipenv requirements --categories docs > requirements.txt
           pip install -r requirements.txt
       - name: Test
         if: github.ref != 'refs/heads/main'
         run: |
             mkdocs build --strict
       - name: Deploy
```

### Comparing `stocktracer-0.2.0/.github/workflows/publish-pypi.yml` & `stocktracer-0.3.0/.github/workflows/publish-pypi.yml`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         uses: actions/setup-python@v4
         with:
           python-version: '3.10'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install pipenv
+          pipenv lock
           pipenv requirements > requirements.txt
           pip install build
       - name: Build package
         # run: python -m build
         run: python3 -m build
       - name: Publish package
         uses: pypa/gh-action-pypi-publish@a56da0b891b3dc519c7ee3284aff1fad93cc8598
```

### Comparing `stocktracer-0.2.0/.github/workflows/python.yml` & `stocktracer-0.3.0/.github/workflows/python.yml`

 * *Files 9% similar despite different names*

```diff
@@ -38,37 +38,34 @@
         with:
           python-version: ${{ matrix.python-version }}
           cache: 'pip'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install pipenv
-          pipenv requirements --dev > requirements.txt
-          pip install -r requirements.txt
+          pipenv install --dev
       - name: Cache Network Requests
         uses: actions/cache@v3
         with:
           key: sqlite-${{ hashFiles('**/tests/fixtures/network.py') }}
           path: |
             **/.ticker-cache/*.sqlite
         if: ${{ !github.event.pull_request.draft }}
       - name: Run - unit-tests
         run: |
-          coverage run -m pytest --doctest-modules
-          # coverage run -m pytest --run-webtest --doctest-modules
-          coverage report
-          # coveralls --service=github
+          pipenv run coverage run -m pytest --doctest-modules
+          pipenv run coverage report
       # Just to cut down on network testing while initially iterating
       - name: Run - network-tests
         run: |
-          coverage run -a -m pytest -m webtest --run-webtest
+          pipenv run coverage run -a -m pytest -m webtest --run-webtest
         if: ${{ !github.event.pull_request.draft }}
       - name: Coveralls
         run: |
-          coveralls --service=github
+          pipenv run coveralls --service=github
       # - name: Coveralls
       #   uses: coverallsapp/github-action@v2
       #   with:
       #     github-token: ${{ secrets.GITHUB_TOKEN }}
       #     flag-name: run-${{ join(matrix.*, '-') }}
       #     parallel: true
       #     format: python
@@ -82,23 +79,24 @@
       #   # Use always() to always run this step to publish test results when there are test failures
       #   if: ${{ always() }}
 
   lint:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
-      - name: Set up Python ${{ matrix.python-version }}
+      - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python-version }}
+          python-version: 3.11
           cache: 'pip'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install pipenv
+          pipenv lock --dev
           pipenv requirements --dev > requirements.txt
           pip install -r requirements.txt
       - name: Lint - Ruff 
         run: |
           ruff src 
         if: ${{ always() }}
       - name: Lint - Black
@@ -107,25 +105,42 @@
         if: ${{ always() }}
       - name: Lint - isort
         run: |
           isort --check src
         if: ${{ always() }}
       - name: Lint - pylint (src/stocktracer)
         run: |
-          pylint src/stocktracer
+          pylint -E src/stocktracer
         if: ${{ always() }}
       # - name: Lint - pydocstyle
       #   run: |
       #     pydocstyle
       #   if: ${{ always() }}
       - name: Lint - pydoctest
         run: |
           PYTHONPATH=src pipenv run pydoctest --config pydocktest.json
         if: ${{ always() }}
 
+  verify-packaging:
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: '3.10'
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install pipenv
+          pipenv lock
+      - name: Run Test
+        run: |
+          ./verify-packaging.sh
+
   finish:
     needs: build
     if: ${{ always() }}
     runs-on: ubuntu-latest
     env:
       GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
     steps:
```

### Comparing `stocktracer-0.2.0/.github/workflows/release-test.yml` & `stocktracer-0.3.0/.github/workflows/release-test.yml`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/.github/workflows/release.yml` & `stocktracer-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/docs/gen_ref_pages.py` & `stocktracer-0.3.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/docs/getting-started.md` & `stocktracer-0.3.0/docs/getting-started.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,31 +11,34 @@
     ```sh
     # Clone Repository
     git clone https://github.com/gyund/fundamental-analysis.git
     cd fundamental-analysis.git
 
     pipenv install --dev
 
-    # Perform analysis (not supported yet)
-    PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft
+    # Perform analysis
+    PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft > report.txt
 
     # Help
     PYTHONPATH=src pipenv run python -m stocktracer
 
     # Run Unit Tests
     pipenv run pytest
     ```
 
 ## Generating a Basic Report
 
 ```sh
 # Perform analysis
-python -m ticker analyze --tickers aapl,msft
+python -m ticker analyze --tickers aapl,msft > report.txt
 ```
 
+!!! tip
+    If you want to figure out a list of tags you can filter the reports on, run the default analysis report. This shows the annual report and will then filter out any columns that contain `null` or `NaN` values. From here, you can establish what algorithms you can use and apply consistently across the stocks of interest. You may find that different sectors or 10-K/10-Q reports will have different data sets.
+
 
 ## Plugins
 
 If you wish to use your own analysis plugin, create your own module that implements this interface:
 
 ```python
 from ticker.data.sec import DataSelector as SecDataSelector
@@ -62,8 +65,8 @@
 
 If you wish to run tests using real network resources, such as downloading real reports and processing them, run the following:
 
 ```sh
 pytest --run-webtest
 ```
 
-Note that all data sets will be cached in the directory `${cwd}/.ticker-cache/` for both real and test runs. Expiry for quarterly reports are cached for 5 years and ticker mappings for `CIK -> Ticker` conversion are cached on a yearly basis. You generally won't be researching companies with less than a year's worth of reports though this could cause recently listed companies to lack `CIK -> Ticker` conversions for up to two years from poor timing. Just delete `${cwd}/.ticker-cache/tickers.sqlite` to get the latest.
+Note that all data sets will be cached in the directory `${cwd}/.ticker-cache/` for both real and test runs. Expiry for quarterly reports are cached for 5 years and ticker mappings for `CIK -> Ticker` conversion are cached on a yearly basis. You generally won't be researching companies with less than a year's worth of reports though this could cause recently listed companies to lack `CIK -> Ticker` conversions for up to two years from poor timing. Just delete `${cwd}/.ticker-cache/tickers.sqlite` to get the latest.
```

### Comparing `stocktracer-0.2.0/docs/index.md` & `stocktracer-0.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/docs/design/analysis.md` & `stocktracer-0.3.0/docs/design/analysis.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/docs/design/caching.md` & `stocktracer-0.3.0/docs/design/caching.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/docs/design/data-retrieval.md` & `stocktracer-0.3.0/docs/design/data-retrieval.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/docs/design/reference.md` & `stocktracer-0.3.0/docs/design/reference.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/docs/design/report.md` & `stocktracer-0.3.0/docs/design/report.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/docs/src/stocktracer/__main__.py` & `stocktracer-0.3.0/src/stocktracer/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 #!/usr/bin/env python
 """This is the main entrypoint for the CLI."""
 
 import sys
+from typing import Optional
 
 import beartype.roar
 import fire
 
 from stocktracer.cli import Cli
 
 
-def main_cli(command: str = None) -> any:
+def main_cli(command: Optional[str] = None) -> str | int | None:
     """Entry point for the packaging script.
 
     Args:
-        command (str): alternative input for CLI arguments. Defaults to None.
+        command (Optional[str]): alternative input for CLI arguments. Defaults to None.
 
     Returns:
-        any: _description_
+        str | int | None: exit code
     """
     cli = Cli()
 
     # Since we're running with Fire, we need to return None to avoid chaining
     Cli.return_results = False
     try:
         return fire.Fire(component=cli, name="stocktracer", command=command)
     except Exception as app_exception:  # pylint: disable=broad-exception-caught
         if isinstance(app_exception, beartype.roar.BeartypeException):
             raise app_exception
-        return app_exception
+        return str(app_exception)
 
 
 if __name__ == "__main__":
     sys.exit(main_cli())
```

### Comparing `stocktracer-0.2.0/docs/src/stocktracer/cli.py` & `stocktracer-0.3.0/src/stocktracer/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,27 @@
 from stocktracer.interface import Analysis as AnalysisInterface
 from stocktracer.interface import Options as CliOptions
 
 logger = logging.getLogger(__name__)
 
 
 @beartype
-def get_analysis_instance(module_name: str) -> AnalysisInterface:
+def get_analysis_instance(module_name: str, options: CliOptions) -> AnalysisInterface:
     """Dynamically import and load the Analysis class from a module.
 
     Args:
         module_name (str): full name of the module. For example, "my.module"
+        options (CliOptions): options provided from the CLI
 
     Returns:
         AnalysisInterface: analysis instance
     """
     module = importlib.import_module(module_name)
     class_ = getattr(module, "Analysis")
-    instance = class_()
+    instance = class_(options)
     assert isinstance(instance, AnalysisInterface)
     return instance
 
 
 @beartype
 def get_default_cache_path() -> Path:
     """Get the default path for caching data.
@@ -50,36 +51,36 @@
 
 @beartype
 class Cli:
     """Tools for gathering resources, analyzing data, and publishing the results."""
 
     return_results: bool = True
 
-    def analyze(
+    def analyze(  # pylint: disable=too-many-arguments
         self,
         tickers: Union[Sequence[str], str],
-        cache_path: str = str(get_default_cache_path()),
+        cache_path: Path | str = get_default_cache_path(),
         refresh: bool = False,
         analysis_plugin: str = "stocktracer.analysis.annual_reports",
         final_year: Optional[int] = None,
         final_quarter: Optional[int] = None,
-        report_format: Optional[ReportFormat] = "txt",
-        report_file: Optional[str] = None,
+        report_format: ReportFormat = "txt",
+        report_file: Optional[Path | str] = None,
     ) -> Optional[pd.DataFrame]:
         """Perform stock analysis.
 
         Args:
             tickers (Union[Sequence[str], str]): tickers to include in the analysis
-            cache_path (str): path where to cache data
+            cache_path (Path | str): path where to cache data
             refresh (bool): Whether to refresh the calculation or use the results from a prior one
             analysis_plugin (str): module to load for analysis
             final_year (Optional[int]): last year to consider for report collection
             final_quarter (Optional[int]): last quarter to consider for report collection
-            report_format (Optional[ReportFormat]): Format of the report. Options include: csv, json, md (markdown)
-            report_file (Optional[str]): Where to store the report. Required if report_format is specified.
+            report_format (ReportFormat): Format of the report. Options include: csv, json, md (markdown)
+            report_file (Optional[Path | str]): Where to store the report. Required if report_format is specified.
 
         Raises:
             LookupError: no analysis results found
 
         Returns:
             Optional[pd.DataFrame]: results of analysis
         """
@@ -87,39 +88,40 @@
         if report_file:
             report_file = Path(report_file)
         if isinstance(tickers, str):
             tickers = frozenset([tickers])
         else:
             tickers = frozenset(tickers)
 
-        analysis_module: AnalysisInterface = get_analysis_instance(analysis_plugin)
-        analysis_module.options = CliOptions(
-            tickers=tickers,
-            cache_path=cache_path,
-            final_year=final_year,
-            final_quarter=final_quarter,
+        analysis_module: AnalysisInterface = get_analysis_instance(
+            analysis_plugin,
+            CliOptions(
+                tickers=tickers,
+                cache_path=cache_path,
+                final_year=final_year,
+                final_quarter=final_quarter,
+            ),
         )
 
         cache, results_key, results = self._get_cached_results(
             tickers, cache_path, analysis_plugin
         )
 
         if (
             refresh
             or results is None
             or not isinstance(results, pd.DataFrame)
             or results.empty
         ):
             # Call analysis plugin
+            results = None
             results = analysis_module.analyze()
             if results is None or results.empty:
                 raise LookupError("No analysis results available!")
 
-            tickers = frozenset(tickers)
-
             # Save one week expiry
             cache.set(key=results_key, value=results, expire=3600 * 24 * 7)
 
         self._generate_report(report_format, report_file, results)
         if analysis_module.under_development:
             warnings.warn(
                 "This analysis module is under development and may be incorrect, incomplete, or may change."
@@ -133,14 +135,15 @@
         cls,
         report_format: ReportFormat,
         report_file: Path | io.StringIO | None,
         results: pd.DataFrame,
     ):
         if report_file is None:
             report_file = io.StringIO()
+        results = results.transpose()
         match report_format.lower():
             case "csv":
                 results.to_csv(report_file)
             case "md":
                 results.to_markdown(report_file)
             case "json":
                 results.to_json(report_file)
```

### Comparing `stocktracer-0.2.0/docs/src/stocktracer/filter.py` & `stocktracer-0.3.0/src/stocktracer/filter.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 from beartype import beartype
 
 from stocktracer.data.sec import Filter as SecFilter
 
 
 @beartype
 class Selectors:
+    """Selectors provide an aggregation point for a number of built-in filter mechanics.
+
+    The original intent for this was to provide a bag to throw a bunch of filters in. However,
+    analysis modules somewhat replace this concept by giving finer grained control over what
+    filters get applied. This may go away in the future pending a determination whether or not
+    the class is needed.
+    """
+
     def __init__(
         self, ticker_filter: set[str] | list[str], sec_filter: SecFilter
     ) -> None:
         """Entry for data to search for in various sources.
 
         Args:
             ticker_filter (set[str] | list[str]): list of stock tickers to get information about
```

### Comparing `stocktracer-0.2.0/docs/src/stocktracer/interface.py` & `stocktracer-0.3.0/src/stocktracer/interface.py`

 * *Files 25% similar despite different names*

```diff
@@ -33,16 +33,18 @@
         self.last_report = ReportDate(year=final_year, quarter=final_quarter)
 
 
 @beartype
 class Analysis(metaclass=abc.ABCMeta):
     """Base class for all analysis techniques."""
 
-    def __init__(self) -> None:
-        self.options: Optional[Options] = None
+    def __init__(self, options: Options) -> None:
+        self.options = options
+        assert self.options is not None
+        assert self.options.cache_path is not None
 
     @abc.abstractmethod
     def analyze(self) -> Optional[DataFrame]:
         """Perform financial analysis.
 
         Returns:
             Optional[DataFrame]: results of analysis
```

### Comparing `stocktracer-0.2.0/docs/src/stocktracer/analysis/annual_reports.py` & `stocktracer-0.3.0/src/stocktracer/analysis/diluted_eps.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""This analysis module determines the trend of EPS over the course of the past 5 years."""
 import logging
 from typing import Optional
 
 import pandas as pd
 from beartype import beartype
 
 from stocktracer.data.sec import Filter as SecFilter
@@ -9,33 +10,30 @@
 from stocktracer.interface import Analysis as AnalysisInterface
 
 logger = logging.getLogger(__name__)
 
 
 @beartype
 class Analysis(AnalysisInterface):
-    """Perform an analysis on the earnings per share over time."""
+    """Class that calculates the EPS slope."""
 
     under_development = True
+    years_of_analysis = 5
 
     def analyze(self) -> Optional[pd.DataFrame]:
-        # By omitting the tags, we'll collect all tags for securities
+        # Create the filter we'll use to scrape the results
         sec_filter = SecFilter(
-            # tags=["EarningsPerShareDiluted"],
-            years=1,  # Over the past 1 years
+            tags=["EarningsPerShareDiluted"],
+            years=self.years_of_analysis,
             last_report=self.options.last_report,
             only_annual=True,  # We only want the 10-K
         )
 
         # Create an SEC Data Source
-        assert self.options is not None
-        assert self.options.cache_path is not None
         sec = SecDataSource(storage_path=self.options.cache_path)
-        sec.select_data(tickers=self.options.tickers, filter=sec_filter)
 
-        table = sec_filter.select()
-        logger.debug(f"tags:\n{table.tags}")
-
-        return table.data
+        # This is an expensive operation
+        sec.filter_data(tickers=self.options.tickers, sec_filter=sec_filter)
+        return sec_filter.select("slope").data
 
     # Reuse documentation from parent
     analyze.__doc__ = AnalysisInterface.analyze.__doc__
```

### Comparing `stocktracer-0.2.0/docs/src/stocktracer/analysis/stub.py` & `stocktracer-0.3.0/src/stocktracer/analysis/stub.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 from stocktracer.interface import Analysis as AnalysisInterface
 
 logger = logging.getLogger(__name__)
 
 
 @beartype
 class Analysis(AnalysisInterface):
+    """Stub for analyzing the report."""
+
     def analyze(self) -> Optional[pd.DataFrame]:
-        """Analyze the report.
+        """
 
         As a stub, this does nothing
 
         Returns:
             Optional[pd.DataFrame]: Always None, since the stub doesn't analyze anything.
         """
         print(
```

### Comparing `stocktracer-0.2.0/docs/src/stocktracer/data/sec.py` & `stocktracer-0.3.0/src/stocktracer/data/sec.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 """This data source grabs information from quarterly SEC data archives."""
+import copy
 import logging
+import sys
 from datetime import date, timedelta
 from io import BytesIO
 from pathlib import Path
-from typing import Literal, Optional, SupportsInt
+from typing import Literal, Optional
 from zipfile import ZipFile
 
 import numpy as np
 import pandas as pd
+from alive_progress import alive_bar
 from beartype import beartype
 from beartype.typing import Callable, Sequence
+from numpy.linalg import LinAlgError
 from requests_cache import CachedSession, SQLiteCache
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_CHUNK_SIZE = 1000000
 pd.set_option("mode.chained_assignment", "raise")
 
 
 @beartype
 class ReportDate:
+    """ReportDate is used to select and identify archives created by the SEC."""
+
     def __init__(
         self,
         year: int | None = None,
         quarter: int | None = None,
     ):
-        """ReportDate is used to select and identify archives created by the SEC.
+        """
 
         Args:
             year (int, optional): Year of the archive. Defaults to date.today().year.
             quarter (int, optional): Quarter the archive was created. Defaults to ((date.today().month - 1) // 3)+1.
 
         Raises:
             ValueError: If the value for quarter or year is invalid
@@ -56,112 +62,267 @@
 
     def __eq__(self, other: "ReportDate") -> bool:
         return self.quarter == other.quarter and self.year == other.year
 
 
 @beartype
 class TickerReader:
+    """This class provides translation services for CIK and Ticker values.
+
+    The SEC has a `json` file that provides mappings from CIK values to Tickers.
+    The data providing this conversion is injected into this class and then
+    this class provides helper methods for performing the conversion on this data set.
+
+    This class is provided CSV data which is parsed upon initialization. So creating
+    this object is the most expensive part.
+    """
+
     def __init__(self, data: str):
-        self._data = pd.read_json(data, orient="index")
+        self._cik_to_ticker_map = pd.read_json(data, orient="index")
+
+    @property
+    def map_of_cik_to_ticker(self) -> pd.DataFrame:
+        """Dataframe containing mapping of cik and ticker information.
+
+        Returns:
+            pd.DataFrame: Dataframe with mapping information
+        """
+        return self._cik_to_ticker_map
 
     def convert_to_cik(self, ticker: str) -> np.int64:
         """Get the Cik from the stock ticker.
 
         Args:
             ticker (str): stock ticker. The case does not matter.
 
         Raises:
             LookupError: If ticker is not found
 
         Returns:
             np.int64: cik
         """
-        result = self._data[
-            self._data.ticker == ticker.upper()  # pylint: disable=no-member
-        ]  # pylint: disable=no-member
+        result = self.map_of_cik_to_ticker[
+            self.map_of_cik_to_ticker["ticker"] == ticker.upper()
+        ]
         if result.empty:
             raise LookupError(f"unable to find ticker: {ticker}")
         return result.cik_str.iloc[0]
 
     def convert_to_ticker(self, cik: int) -> str:
         """Get the stock ticker from the Cik number.
 
         Args:
             cik (int): Cik number for the stock
 
         Returns:
             str: stock ticker
         """
-        result = self._data[self._data.cik_str == cik]  # pylint: disable=no-member
+        result = self.map_of_cik_to_ticker[self.map_of_cik_to_ticker["cik_str"] == cik]
         return result.ticker.iloc[0]
 
     def contains(self, tickers: frozenset) -> bool:
         """Check that the tickers provided exist.
 
         Args:
             tickers (frozenset): tickers to check
 
         Returns:
             bool: if all the tickers are found
         """
-        for t in tickers:
-            self.convert_to_cik(t)
+        for ticker in tickers:
+            self.convert_to_cik(ticker)
 
         return True
 
 
-period_focus_options = Literal["FY", "Q1", "Q2", "Q3", "Q4"]
+@beartype
+def slope(data: pd.Series, order: int = 1) -> float:
+    """Calculate the trend of a series.
+
+    >>> import math
+    >>> math.isclose(slope(pd.Series((1,2,3))), 1)
+    True
+
+    >>> math.isclose(slope(pd.Series((3,2,1))), -1)
+    True
+
+    Args:
+        data (pd.Series): _description_
+        order (int): _description_. Defaults to 1.
+
+    Returns:
+        float: slope of the trend line
+    """
+    x_axis = range(len(data.keys()))
+    y_axis = data.values
+
+    try:
+        coeffs = np.polyfit(x_axis, y_axis, order)
+    except LinAlgError:
+        return float(0)
+    return coeffs[0]
 
 
 @beartype
 class Filter:
-    class Table:
-        """This is a table that is the output from a `Filter.select()` call.
+    """Filter for SEC tools to scrape relevant information when processing records."""
+
+    class Results:
+        """This is the results from a `Filter.select()` call.
 
-        When data is converted, it creates a pivot table that looks like the following:
+        The results table looks like the following:
 
-                                                        value
-            cik    tag
-            320193 EntityCommonStockSharesOutstanding   4000.0
-                    FakeAttributeTag                     400.0
-            ...
+        ```
+        tag            AccountsPayableCurrent  ...  WeightedAverageNumberOfSharesOutstandingBasic
+        ticker fy                              ...
+        AAPL   2021.0            4.852950e+10  ...                                   1.750824e+10
+               2022.0            5.943900e+10  ...                                   1.675645e+10
+        MSFT   2021.0            1.384650e+10  ...                                   7.610000e+09
+               2022.0            1.708150e+10  ...                                   7.551000e+09
+        TMO    2021.0            2.521000e+09  ...                                   3.966667e+08
+               2022.0            3.124000e+09  ...                                   3.940000e+08
+        ```
 
+        From here, you can call functions on this class like `get_value()` or `normalize()`.
+
+        !!! note
+            To get a list of all the tags, run the `annual_reports` analysis module and search through the output for meaningful tags.
 
         """
 
-        def __init__(self, table: pd.DataFrame) -> None:
-            self.data = table
+        def __init__(self, results: pd.DataFrame) -> None:
+            logger.debug(f"results:\n{results}")
+            self.data = results
 
         def __str__(self) -> str:
             return str(self.data)
 
         @property
-        def tags(self):
-            return self.data.index.get_level_values("tag").unique()
+        def tags(self) -> np.ndarray:
+            """List of tags that can be used on this data set.
 
-        def get_value(self, ticker_or_cik: str | int, tag: str) -> SupportsInt:
-            # TODO: access the either the ticker or cik index
-            if isinstance(ticker_or_cik, int):
-                return self.data.query(
-                    f'cik == {ticker_or_cik} and tag == "{tag}"'
-                ).values[0]
+            Returns:
+                np.ndarray: array with results
+            """
+            return self.data.columns.values
+
+        def get_value(self, ticker: str | int, tag: str, year: int) -> int | float:
+            """Retrieve the exact value of a table cell.
+
+            Args:
+                ticker (str | int): ticker identifying the equity of interest.
+                tag (str): attribute indicating the type of data to look at.
+                year (int): The year this data applies to.
+
+            Returns:
+                int | float: value of result
+            """
             # Lookup convert ticker to cik
-            ticker_or_cik = ticker_or_cik.upper()
-            return self.data.query(
-                f'ticker == "{ticker_or_cik}" and tag == "{tag}"'
-            ).values[0]
+            ticker = ticker.upper()
+            return self.data.loc[ticker].loc[year].loc[tag]
+
+        def normalize(self):
+            """Remove all values that are NaN."""
+            self.data = self.data.dropna(axis=1, how="any")
+
+        def slice(
+            self,
+            ticker: Optional[str | int] = None,
+            year: Optional[int] = None,
+            tags: Optional[list[str]] = None,
+        ) -> pd.DataFrame:
+            """Slice the results by the specified values
+
+            Args:
+                ticker (Optional[str  |  int]): _description_. Defaults to None.
+                tags (Optional[str]): _description_. Defaults to None.
+                year (Optional[int]): _description_. Defaults to None.
+
+            Returns:
+                pd.DataFrame: _description_
+            """
+            result = self.data
+            if ticker:
+                result = result.loc(axis=0)[ticker, :]
+            if year:
+                result = result.loc(axis=0)[:, year, :]
+            if tags:
+                result = pd.DataFrame(result.loc[:, tags], columns=tags)
+            return result
+
+        def calculate_net_income(self, column_name: str):
+            """Calculates the net income stocks as a series.
+
+            !!! example
+                ``` python
+                results.calculate_net_income()
+                ```
+
+            Args:
+                column_name (str): name to assign to the column
+            """
+            self.data[column_name] = self.data["OperatingIncomeLoss"]
+
+        def calculate_current_ratio(self, column_name: str):
+            """Calculate the current ratio.
+
+            The current ratio is a liquidity ratio that measures a company’s
+            ability to pay short-term obligations or those due within one year.
+
+            Args:
+                column_name (str): _description_
+            """
+            self.data[column_name] = (
+                self.data["AssetsCurrent"] / self.data["LiabilitiesCurrent"]
+            )
+
+        def calculate_debt_to_assets(self, column_name: str):
+            """Calculates the current debt to assets ratio.
+
+            Having more debt than assets is a risk indicator that could indicate
+            a potential for bankruptcy.
+
+            Args:
+                column_name (str): name to assign to the column
+            """
+            self.data[column_name] = (
+                self.data["LiabilitiesCurrent"] / self.data["AssetsCurrent"]
+            )
+
+        def calculate_return_on_assets(self, column_name: str):
+            """Returns the ROA of stocks as a series.
+
+            !!! example
+                ``` python
+                results.calculate_return_on_assets('ROA')
+                ```
+            Args:
+                column_name (str): name to assign to the column
+            """
+            self.data[column_name] = self.data["OperatingIncomeLoss"].div(
+                self.data["Assets"]
+            )
+
+        def calculate_delta(self, column_name: str, delta_of: str):
+            """Calculate the change between the latest row and the one before it within a ticker.
+
+            Args:
+                column_name (str): name to give the calculated column
+                delta_of (str): column name to calculate the delta of, such as ROI
+            """
+            self.data[column_name] = self.data.groupby(by=["ticker"]).diff()[delta_of]
 
     def __init__(
         self,
         tags: Optional[list[str]] = None,
         years: int = 1,
         last_report: ReportDate = ReportDate(),
         only_annual: bool = True,
     ) -> None:
-        """Filter for SEC tools to scrape relevant information when processing records.
+        """
 
         This is an important concept to dealing with large data sets. It allows us to chunk processing
         into batches and find/locate only records of interest. Without these filters, the tool would
         require absurd amounts of memory and storage to process.
 
         Args:
             tags (Optional[list[str]]): list of tags found in the SEC report, such as 'EntityCommonStockSharesOutstanding'
@@ -176,20 +337,21 @@
         self._cik_list: set[int] = None
         self._filtered_data: pd.DataFrame = None
 
     @property
     def filtered_data(self) -> pd.DataFrame:
         """Filtered data looks like this(in csv format):
 
+        Note that fp has the "Q" removed from the front so it can be stored as a simple number.
+
         .. code-block:: text
 
-            ticker,tag,cik,ddate,uom,value,period,fy,fp,title
-            TMO,EarningsPerShareDiluted,97745,2022-12-31,USD,17.63,2022-12-31,2022.0,FY,THERMO FISHER SCIENTIFIC INC.
-            TMO,EarningsPerShareDiluted,97745,2020-12-31,USD,15.96,2022-12-31,2022.0,FY,THERMO FISHER SCIENTIFIC INC.
-            TMO,EarningsPerShareDiluted,97745,2021-12-31,USD,19.46,2022-12-31,2022.0,FY,THERMO FISHER SCIENTIFIC INC.
+            ticker,tag,fy,fp,ddate,uom,value,period,title
+            AAPL,EntityCommonStockSharesOutstanding,2022,Q1,2023-01-31,shares,2000.0,2022-12-31,Apple Inc.
+            AAPL,FakeAttributeTag,2022,Q1,2023-01-31,shares,200.0,2022-12-31,Apple Inc.
 
         Returns:
             pd.DataFrame: _description_
         """
         return self._filtered_data
 
     @filtered_data.setter
@@ -208,44 +370,52 @@
 Annual Only: {self.only_annual}
 CIK(s): {','.join([str(i) for i in self._cik_list]) if self._cik_list else 'None'}
 Tags: {','.join(self.tags) if self.tags else 'None'}"""
 
     def select(
         self,
         aggregate_func: Optional[
-            Callable | Literal["mean", "std", "var", "sum", "min", "max"]
+            Callable | Literal["mean", "std", "var", "sum", "min", "max", "slope"]
         ] = "mean",
         tickers: Optional[Sequence[str]] = None,
-    ) -> Table:
+    ) -> Results:
         """Select only a subset of the data matching the specified criteria.
 
         Args:
-            aggregate_func (Optional[Callable | Literal['mean', 'std', 'var', 'sum', 'min','max']]): Numpy function to use for aggregating the results. This should be a function like `numpy.average` or `numpy.sum`.
+            aggregate_func (Optional[Callable | Literal['mean', 'std', 'var', 'sum', 'min','max','slope']]): Numpy function to use for aggregating the results. This should be a function like `numpy.average` or `numpy.sum`.
             tickers (Optional[Sequence[str]]): ticker symbol for the company
 
         Returns:
-            Filter.Table: Object that represents a pivot table with the data requested
+            Filter.Results: Object that represents a pivot table with the data requested
         """
         if tickers is not None:
             tickers = [t.upper() for t in tickers]
             logger.debug(f"ticker filter: {tickers}")
 
         data = (
             self.filtered_data
             if tickers is None
             else self.filtered_data.query("ticker in @tickers")
         )
         logger.debug(f"pre-pivot:\n{data}")
+
+        # Try and see if the function exists
+        if isinstance(aggregate_func, str):
+            if aggregate_func in globals():
+                aggregate_func = globals()[aggregate_func]
+
         table: pd.DataFrame = pd.pivot_table(
             data,
             values="value",
-            index=["cik", "tag", "ticker"],
+            columns="tag",
+            index=["ticker", "fy"],
             aggfunc=aggregate_func,
         )
-        return Filter.Table(table)
+
+        return Filter.Results(table)
 
     @property
     def ciks(self) -> set[int]:
         """Retrieves a list of CIK values corresponding to the tickers being looked up.
 
         The SEC object will call populateCikList to generate this information. This helps
         with dependency injection by avoiding the Filter having to maintain references to
@@ -308,15 +478,15 @@
         companies don't have the same fiscal year, we have to check every quarterly
         report just to see if their annual report is in there.
 
         Returns:
             list[ReportDate]: list of report dates to retrieve
         """
         dl_list: list[ReportDate] = []
-        next_report = self.last_report
+        next_report = copy.deepcopy(self.last_report)
         final_report = ReportDate(
             self.last_report.year - self.years, self.last_report.quarter
         )
         while 1:
             dl_list.append(
                 ReportDate(year=next_report.year, quarter=next_report.quarter)
             )
@@ -333,44 +503,44 @@
 @beartype
 class DataSetReader:
     """Reads the data from a zip file retrieved from the SEC website."""
 
     def __init__(self, zip_data: bytes) -> None:
         self.zip_data = BytesIO(zip_data)
 
-    def process_zip(self, filter: Filter) -> Optional[pd.DataFrame]:
+    def process_zip(self, sec_filter: Filter) -> Optional[pd.DataFrame]:
         """Process a zip archive with the provided filter.
 
         Args:
-            filter (Filter): results to filter out of the zip archive
+            sec_filter (Filter): results to filter out of the zip archive
 
         Raises:
             ImportError: the filter doesn't match anything
 
         Returns:
             Optional[pd.DataFrame]: filtered data
         """
         with ZipFile(self.zip_data) as myzip:
             # Process the mapping first
             logger.debug("opening sub.txt")
             with myzip.open("sub.txt") as myfile:
                 # Get reports that are 10-K or 10-Q
-                sub_dataframe = DataSetReader._process_sub_text(myfile, filter)
+                sub_dataframe = DataSetReader._process_sub_text(myfile, sec_filter)
 
                 if sub_dataframe is None or sub_dataframe.empty:
                     raise ImportError("nothing found in sub.txt matching the filter")
 
                 with myzip.open("num.txt") as myfile:
                     return DataSetReader._process_num_text(
-                        myfile, filter, sub_dataframe
+                        myfile, sec_filter, sub_dataframe
                     )
 
     @classmethod
     def _process_num_text(
-        cls, filepath_or_buffer, filter: Filter, sub_dataframe: pd.DataFrame
+        cls, filepath_or_buffer, sec_filter: Filter, sub_dataframe: pd.DataFrame
     ) -> Optional[pd.DataFrame]:
         """Contains the numerical data.
 
         adsh	tag	version	coreg	ddate	qtrs	uom	value	footnote
 
         """
         logger.debug("processing num.txt")
@@ -386,76 +556,118 @@
         filtered_data: pd.DataFrame = None
         chunk: pd.DataFrame
         for chunk in reader:
             # We want only the tables in left if they join on the key, so inner it is
             data = chunk.join(sub_dataframe, how="inner")
 
             # Additional Filtering if needed
-            if filter.tags is not None:
-                tag_list = filter.tags  # pylint: disable=unused-variable
+            if sec_filter.tags is not None:
+                tag_list = sec_filter.tags  # pylint: disable=unused-variable
                 data = data.query("tag in @tag_list")
 
             if data.empty:  # pragma: no cover
-                logger.debug(f"chunk:\n{chunk}")
-                logger.debug(f"sub_dataframe:\n{sub_dataframe}")
+                # logger.debug(f"chunk:\n{chunk}")
+                # logger.debug(f"sub_dataframe:\n{sub_dataframe}")
                 continue
 
-            if filtered_data is None:
-                filtered_data = data
-            else:
-                filtered_data.merge(data)
+            filtered_data = cls.append(filtered_data, data)
+
+        # if filtered_data is not None:  # pragma: no cover
+        #     logger.debug(f"Filtered Records (head+5): {filtered_data.head()}")
+        return filtered_data
+
+    @classmethod
+    def append(
+        cls, filtered_data: Optional[pd.DataFrame], data: pd.DataFrame
+    ) -> pd.DataFrame:
+        """Append data to the filtered_data and return the updated filtered DataFrame.
+
+        >>> df1 = pd.DataFrame({"A": ["A0", "A1", "A2", "A3"]},index=[0,1,2,3])
+        >>> df2 = pd.DataFrame({"B": ["B0", "B1", "B2", "B3"]},index=[4,5,6,7])
+        >>> DataSetReader.append(df1, df2)
+             A    B
+        0   A0  NaN
+        1   A1  NaN
+        2   A2  NaN
+        3   A3  NaN
+        4  NaN   B0
+        5  NaN   B1
+        6  NaN   B2
+        7  NaN   B3
+        >>> DataSetReader.append(None, df1)
+            A
+        0  A0
+        1  A1
+        2  A2
+        3  A3
+        >>> DataSetReader.append(df1, df1)
+            A
+        0  A0
+        1  A1
+        2  A2
+        3  A3
+        0  A0
+        1  A1
+        2  A2
+        3  A3
+
+        Args:
+            filtered_data (Optional[pd.DataFrame]): Existing Data
+            data (pd.DataFrame): New data
 
-            filtered_data.merge(data)
-        if filtered_data is not None:  # pragma: no cover
-            logger.debug(f"Filtered Records (head+5): {filtered_data.head()}")
+        Returns:
+            pd.DataFrame: Filtered Data
+        """
+        if filtered_data is None:
+            filtered_data = data
+        else:
+            filtered_data = pd.concat([filtered_data, data])
         return filtered_data
 
     @classmethod
     def _process_sub_text(
-        cls, filepath_or_buffer, filter: Filter
+        cls, filepath_or_buffer, sec_filter: Filter
     ) -> Optional[pd.DataFrame]:
         """Contains the submissions.
 
         adsh	cik	name	sic	countryba	stprba	cityba	zipba	bas1	bas2	baph	countryma
         stprma	cityma	zipma	mas1	mas2	countryinc	stprinc	ein	former	changed	afs	wksi
         fye	form	period	fy	fp	filed	accepted	prevrpt	detail	instance	nciks	aciks
         """
         logger.debug("processing sub.txt")
-        focus_periods = filter.focus_period
-        cik_list = filter.ciks  # pylint: disable=unused-variable
+        focus_periods = sec_filter.focus_period
+        cik_list = sec_filter.ciks  # pylint: disable=unused-variable
 
-        oldest_fy = filter.last_report.year - filter.years
+        oldest_fy = sec_filter.last_report.year - sec_filter.years
         query_str = f"cik in @cik_list and fp in @focus_periods and fy >= {oldest_fy}"
-        logger.debug(f"Query string: {query_str}")
+        # logger.debug(f"Query string: {query_str}")
         reader = pd.read_csv(
             filepath_or_buffer,
             delimiter="\t",
             usecols=["adsh", "cik", "period", "fy", "fp"],
             index_col=["adsh", "cik"],
             chunksize=DEFAULT_CHUNK_SIZE,
             parse_dates=["period"],
+            dtype={"cik": np.int32},
         )
-        logger.debug(f"keeping only these focus periods: {focus_periods}")
+        logger.info(f"keeping only these focus periods: {focus_periods}")
         filtered_data: pd.DataFrame = None
         chunk: pd.DataFrame
         for chunk in reader:
             data = chunk.query(query_str)
             if data.empty:
                 continue
-            if filtered_data is None:
-                filtered_data = data
-            else:
-                filtered_data.merge(data)
-        if filtered_data is not None:
-            logger.debug(f"Filtered Records (head+5):\n{filtered_data.head()}")
+            filtered_data = cls.append(filtered_data, data)
         return filtered_data
 
 
 @beartype
 class DownloadManager:
+    """This class is responsible for downloading and caching downloaded data sets from the SEC."""
+
     # Format of zip example: 2023q1.zip
     _base_url = "https://www.sec.gov/files/dera/data/financial-statement-data-sets"
 
     _company_tickers_url = "https://www.sec.gov/files/company_tickers.json"
 
     def __init__(
         self, ticker_session: CachedSession, data_session: CachedSession
@@ -506,94 +718,115 @@
         Returns:
             Optional[DataSetReader]: this object helps process the data received more granularly
         """
         request = self._create_download_uri(report_date)
         response = self._data_session.get(request)
         if response.from_cache:
             logger.info(f"Retrieved {request} from cache")
+
         if response.status_code == 200:
             return DataSetReader(response.content)
         return None  # pragma: no cover
 
 
 @beartype
 class DataSetCollector:
     """Take care of downloading all the data sets and aggregate them into a single structure."""
 
     def __init__(self, download_manager: DownloadManager):
         self.download_manager = download_manager
 
-    def get_data(self, filter: Filter) -> None:
+    def get_data(self, sec_filter: Filter) -> None:
         """Collect data based on the provided filter.
 
         Args:
-            filter (Filter): SEC specific filter of how to filter the results
+            sec_filter (Filter): SEC specific filter of how to filter the results
 
         Raises:
             LookupError: when there are no results matching the filter
 
         """
         data_frame = None
-        report_dates = filter.required_reports
+        report_dates = sec_filter.required_reports
         logger.info(f"Creating Unified Data record for these reports: {report_dates}")
-        for r in report_dates:
-            reader = self.download_manager.get_quarterly_report(r)
-            if isinstance(reader, DataSetReader):
-                try:
-                    data = reader.process_zip(filter)
-                    if data is None or data.empty:
-                        logger.debug(f"no results captured in report {r}")
-                    elif data_frame is None:
-                        logger.debug(f"keys: {data.keys()}")
-                        data_frame = data
-                    else:
-                        # df = pd.concat(df, data)
-                        data_frame.merge(right=data)
-                except ImportError:
-                    # Note, when searching for annual reports, this will generally occur 1/4 times
-                    # if we're only searching for one stock's tags
-                    logger.debug(
-                        f"{r} did not have any matches for the provided filter"
-                    )
-                    logger.debug(f"{filter}")
+        with alive_bar(
+            # total=len(report_dates) * 2,
+            theme="smooth",
+            # stats=False,
+            title="Records Retrieved",
+            file=sys.stderr,
+            calibrate=5_000,
+            dual_line=True,
+        ) as status_bar:
+            for report_date in report_dates:
+                status_bar.text(f"Downloading report {report_date}...")
+                reader = self.download_manager.get_quarterly_report(report_date)
+                if isinstance(reader, DataSetReader):
+                    try:
+                        status_bar.text(f"Processing report {report_date}...")
+                        data = reader.process_zip(sec_filter)
+                        if data_frame is not None:
+                            logger.debug(f"record count: {len(data_frame)}")
+                        if data is not None:
+                            logger.debug(f"new record count: {len(data)}")
+                            data_frame = DataSetReader.append(data_frame, data)
+                            record_count = len(data_frame)
+                            status_bar(record_count)  # pylint: disable=not-callable
+                            logger.info(
+                                f"There are now {record_count} filtered records"
+                            )
+
+                    except ImportError:
+                        # Note, when searching for annual reports, this will generally occur 1/4 times
+                        # if we're only searching for one stock's tags
+                        logger.debug(
+                            f"{report_date} did not have any matches for the provided filter"
+                        )
+                        logger.debug(f"{sec_filter}")
+
         logger.info(f"Created Unified Data record for these reports: {report_dates}")
-        if data_frame is not None:
-            logger.debug(f"keys: {data_frame.keys()}")
-            logger.debug(f"Rows: {len(data_frame)}")
-            logger.debug(data_frame.head())
-        else:
+        if data_frame is None:
             raise LookupError("No data matching the filter was retrieved")
 
         # Now add an index for ticker values to pair with the cik
-        logger.debug(f"filtered_df_before_merge:\n{data_frame.to_csv()}")
+        # logger.debug(f"filtered_df_before_merge:\n{data_frame.to_csv()}")
         data_frame = data_frame.reset_index().merge(
-            right=self.download_manager.ticker_reader._data,
+            right=self.download_manager.ticker_reader.map_of_cik_to_ticker,
             how="inner",
             left_on="cik",
             right_on=["cik_str"],
         )
 
         # Columns at this point look like this
         #  ,adsh,tag,cik,ddate,uom,value,period,fy,fp,cik_str,ticker,title
         # 0,0000097745-23-000008,EarningsPerShareDiluted,97745,2022-12-31,USD,17.63,2022-12-31,2022.0,FY,97745,TMO,THERMO FISHER SCIENTIFIC INC.
         # 1,0000097745-23-000008,EarningsPerShareDiluted,97745,2020-12-31,USD,15.96,2022-12-31,2022.0,FY,97745,TMO,THERMO FISHER SCIENTIFIC INC.
         # 2,0000097745-23-000008,EarningsPerShareDiluted,97745,2021-12-31,USD,19.46,2022-12-31,2022.0,FY,97745,TMO,THERMO FISHER SCIENTIFIC INC..
 
-        data_frame = data_frame.drop(columns=["cik_str", "adsh"]).set_index(
-            ["ticker", "tag", "cik"]
-        )
+        sec_filter.filtered_data = data_frame.drop(
+            columns=["cik_str", "adsh", "cik"]
+        ).set_index(["ticker", "tag", "fy", "fp"])
+
+        # # Convert fp to number so we can sort easily
+        # data_frame['fp'].mask(data_frame['fp'] == "Q1", 1, inplace=True)
+        # data_frame['fp'].mask(data_frame['fp'] == "Q2", 2, inplace=True)
+        # data_frame['fp'].mask(data_frame['fp'] == "Q3", 3, inplace=True)
+        # data_frame['fp'].mask(data_frame['fp'] == "Q4", 4, inplace=True)
+        # data_frame = data_frame.set_index("fp", append=True)
 
-        logger.debug(f"filtered_df:\n{data_frame.to_csv()}")
-        filter.filtered_data = data_frame
+        # logger.debug(f"filtered_df:\n{data_frame}")
+        # filter.filtered_data = data_frame
 
 
 @beartype
 class Sec:
+    """Object for handling requests for information relating to SEC data dumps."""
+
     def __init__(self, storage_path: Path):
-        """Object for handling requests for information relating to SEC data dumps.
+        """
 
         Args:
             storage_path (Path): Where to store the results.
         """
         storage_path.mkdir(parents=True, exist_ok=True)
         data_session = CachedSession(
             "data",
@@ -606,26 +839,26 @@
             "tickers",
             backend=SQLiteCache(db_path=storage_path / "tickers"),
             expire_after=timedelta(days=365),
             stale_if_error=True,
         )
         self.download_manager = DownloadManager(ticker_session, data_session)
 
-    def select_data(self, tickers: frozenset[str], filter: Filter) -> Filter:
+    def filter_data(self, tickers: frozenset[str], sec_filter: Filter) -> Filter:
         """Initiate the retrieval of ticker information based on the provided filters.
 
         Filtered data is stored with the filter
 
         Args:
             tickers (frozenset[str]): ticker symbols you want information about
-            filter (Filter): SEC specific data to scrape from the reports
+            sec_filter (Filter): SEC specific data to scrape from the reports
 
         Returns:
             Filter: filter with filtered data
         """
         collector = DataSetCollector(self.download_manager)
         ticker_reader = self.download_manager.ticker_reader
         if ticker_reader.contains(tickers):
-            filter.populate_ciks(tickers=tickers, ticker_reader=ticker_reader)
-            collector.get_data(filter)
+            sec_filter.populate_ciks(tickers=tickers, ticker_reader=ticker_reader)
+            collector.get_data(sec_filter)
 
-        return filter
+        return sec_filter
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stocktracer-0.2.0/docs/src/tests/test_cli.py` & `stocktracer-0.3.0/src/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 def test_generate(sec_harness: tuple[Sec, mock.MagicMock]):
     (sec, download_manager) = sec_harness
     d = {"col1": [1, 2], "col2": [3, 4]}
     data_frame = pd.DataFrame(data=d)
     result = io.StringIO()
     Cli._generate_report("csv", result, data_frame)
-    assert data_frame.to_csv() == result.getvalue()
+    assert data_frame.transpose().to_csv() == result.getvalue()
     result = io.StringIO()
     Cli._generate_report("json", result, data_frame)
-    assert data_frame.to_json() == result.getvalue()
+    assert data_frame.transpose().to_json() == result.getvalue()
     result = io.StringIO()
     Cli._generate_report("md", result, data_frame)
-    assert data_frame.to_markdown() == result.getvalue()
+    assert data_frame.transpose().to_markdown() == result.getvalue()
 
     with pytest.raises(beartype.roar.BeartypeCallHintParamViolation):
         Cli._generate_report("invalid", None, data_frame)
```

### Comparing `stocktracer-0.2.0/docs/src/tests/test_filter.py` & `stocktracer-0.3.0/src/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/docs/src/tests/analysis/test_annual_reports.py` & `stocktracer-0.3.0/src/tests/analysis/test_diluted_eps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 import logging
+import math
 
-import mock
 import pytest
 
 from stocktracer.analysis.diluted_eps import Analysis
 from stocktracer.cli import Cli
 
 logger = logging.getLogger(__name__)
 
 # We only need a year for testing, cut down on data
 Analysis.years_of_analysis = 1
 
 
-class TestCliAnnualReports:
+class TestCliDilutedEps:
     cli: Cli = Cli()
 
     @pytest.mark.webtest
     def test_analyze(self):
         self.cli.return_results = True
         result = self.cli.analyze(
             tickers=["aapl", "tmo", "msft"],
-            analysis_plugin="stocktracer.analysis.annual_reports",
+            analysis_plugin="stocktracer.analysis.diluted_eps",
             refresh=True,
             final_year=2023,
             final_quarter=1,
         )
         assert result is not None
-        logger.debug(f"annual_reports:\n{result}")
+        logger.debug(f"diluted_eps_result:\n{result}")
+        assert math.isclose(
+            # result.loc["TMO"]["EarningsPerShareDiluted"], 17.683333, rel_tol=0.001 # EPS last qtr
+            result.loc["TMO"]["EarningsPerShareDiluted"],
+            0.915,
+            rel_tol=0.001,  # trend
+        )
 
     def test_invalid(self):
         with pytest.raises(LookupError, match="unable to find ticker: invalid"):
             self.cli.analyze(
                 tickers="invalid", analysis_plugin="stocktracer.analysis.diluted_eps"
             )
```

### Comparing `stocktracer-0.2.0/docs/src/tests/analysis/test_diluted_eps.py` & `stocktracer-0.3.0/src/tests/analysis/test_f_score.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 import logging
+import math
 
-import mock
 import pytest
 
 from stocktracer.analysis.diluted_eps import Analysis
 from stocktracer.cli import Cli
 
 logger = logging.getLogger(__name__)
 
 # We only need a year for testing, cut down on data
 Analysis.years_of_analysis = 1
 
 
-class TestCliDilutedEps:
+class TestCliFScore:
     cli: Cli = Cli()
 
     @pytest.mark.webtest
     def test_analyze(self):
         self.cli.return_results = True
         result = self.cli.analyze(
             tickers=["aapl", "tmo", "msft"],
-            analysis_plugin="stocktracer.analysis.diluted_eps",
+            analysis_plugin="stocktracer.analysis.f_score",
             refresh=True,
             final_year=2023,
             final_quarter=1,
         )
         assert result is not None
-        logger.debug(
-            f"diluted_eps_result:\n{result.sort_values(ascending=True, by=['ddate'])}"
-        )
+        logger.debug(f"f_score_result:\n{result.to_string()}")
+        # assert math.isclose(
+        #     # result.loc["TMO"]["EarningsPerShareDiluted"], 17.683333, rel_tol=0.001 # EPS last qtr
+        #     result.loc["TMO"]["EarningsPerShareDiluted"],
+        #     -0.820571,
+        #     rel_tol=0.001,  # trend
+        # )
 
     def test_invalid(self):
         with pytest.raises(LookupError, match="unable to find ticker: invalid"):
             self.cli.analyze(
                 tickers="invalid", analysis_plugin="stocktracer.analysis.diluted_eps"
             )
```

### Comparing `stocktracer-0.2.0/docs/src/tests/analysis/test_stub.py` & `stocktracer-0.3.0/src/tests/analysis/test_stub.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/docs/src/tests/fixtures/network.py` & `stocktracer-0.3.0/src/tests/fixtures/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,11 +13,11 @@
     return Sec(get_default_cache_path())
 
 
 @pytest.fixture
 def sec_dataselector_2023q1(
     sec_instance: Sec, filter_aapl: Filter.Selectors
 ) -> Filter.Selectors:
-    sec_instance.select_data(
-        tickers=filter_aapl.ticker_filter, filter=filter_aapl.sec_filter
+    sec_instance.filter_data(
+        tickers=filter_aapl.ticker_filter, sec_filter=filter_aapl.sec_filter
     )
     return filter_aapl
```

### Comparing `stocktracer-0.2.0/docs/src/tests/fixtures/unit.py` & `stocktracer-0.3.0/src/tests/fixtures/unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,19 +80,20 @@
 @pytest.fixture
 def sec_fake_report(
     filter_aapl: Filter.Selectors, sub_txt_sample, data_txt_sample
 ) -> Filter.Selectors:
     filter_aapl.sec_filter._cik_list = set()
     filter_aapl.sec_filter._cik_list.add(320193)
     sub_df = DataSetReader._process_sub_text(
-        filepath_or_buffer=io.StringIO(sub_txt_sample), filter=filter_aapl.sec_filter
+        filepath_or_buffer=io.StringIO(sub_txt_sample),
+        sec_filter=filter_aapl.sec_filter,
     )
     num_df = DataSetReader._process_num_text(
         filepath_or_buffer=io.StringIO(data_txt_sample),
-        filter=filter_aapl.sec_filter,
+        sec_filter=filter_aapl.sec_filter,
         sub_dataframe=sub_df,
     )
     ticker_reader = mock.MagicMock(TickerReader)
     assert not num_df.empty
     return filter_aapl
 
 
@@ -109,16 +110,16 @@
     selector: Filter.Selectors, sub_txt: str, data_txt: str
 ) -> DataFrame:
     selector.sec_filter._cik_list = set()
     selector.sec_filter._cik_list.add(320193)
     selector.sec_filter.tags.append("FakeAttributeTag")
     sub_df = DataSetReader._process_sub_text(
         filepath_or_buffer=io.StringIO(sub_txt),
-        filter=selector.sec_filter,
+        sec_filter=selector.sec_filter,
     )
     num_df = DataSetReader._process_num_text(
         filepath_or_buffer=io.StringIO(data_txt),
-        filter=selector.sec_filter,
+        sec_filter=selector.sec_filter,
         sub_dataframe=sub_df,
     )
     assert num_df is not None
     return num_df
```

### Comparing `stocktracer-0.2.0/docs/src/tests/sec/test_DataSelector.py` & `stocktracer-0.3.0/src/tests/sec/test_DataSelector.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/docs/src/tests/sec/test_DataSetReader.py` & `stocktracer-0.3.0/src/tests/sec/test_DataSetReader.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,27 +27,29 @@
 
 def test_benchmark_DataSetReader_processNumText(
     benchmark, filter_aapl: Filter.Selectors, sub_txt_sample, data_txt_sample
 ):
     filter_aapl.sec_filter._cik_list = set()
     filter_aapl.sec_filter._cik_list.add(320193)
     sub_df = DataSetReader._process_sub_text(
-        filepath_or_buffer=io.StringIO(sub_txt_sample), filter=filter_aapl.sec_filter
+        filepath_or_buffer=io.StringIO(sub_txt_sample),
+        sec_filter=filter_aapl.sec_filter,
     )
     benchmark.pedantic(
         DataSetReader._process_num_text,
         args=(io.StringIO(data_txt_sample), filter_aapl.sec_filter, sub_df),
     )
 
 
 def test_DataSetReader_processSubText(filter_aapl: Filter.Selectors, sub_txt_sample):
     # Put AAPL's CIK in the list so it will be filtered
     filter_aapl.sec_filter._cik_list = set()
     filter_aapl.sec_filter._cik_list.add(320193)
     sub_df = DataSetReader._process_sub_text(
-        filepath_or_buffer=io.StringIO(sub_txt_sample), filter=filter_aapl.sec_filter
+        filepath_or_buffer=io.StringIO(sub_txt_sample),
+        sec_filter=filter_aapl.sec_filter,
     )
     logger.debug(f"sub keys: {sub_df.keys()}")
     logger.debug(sub_df)
     assert "0000320193-23-000006" in sub_df.index.get_level_values("adsh")
     assert "0000723125-23-000022" not in sub_df.index.get_level_values("adsh")
     assert "0000004457-23-000026" not in sub_df.index.get_level_values("adsh")
```

### Comparing `stocktracer-0.2.0/docs/src/tests/sec/test_network.py` & `stocktracer-0.3.0/src/tests/sec/test_network.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,25 +45,27 @@
         # assert aapl.empty == False
 
 
 @pytest.mark.webtest
 def test_update(sec_instance: Sec, filter_aapl: Filter.Selectors):
     # pytest.skip(
     #     "skip until we can resolve performance issues with large data sets")
-    sec_instance.select_data(tickers=frozenset(["aapl"]), filter=filter_aapl.sec_filter)
+    sec_instance.filter_data(
+        tickers=frozenset(["aapl"]), sec_filter=filter_aapl.sec_filter
+    )
     assert filter_aapl.sec_filter.filtered_data.empty == False
     logger.debug(
         f"There are {len(filter_aapl.sec_filter.filtered_data)} records about apple"
     )
     logger.debug(filter_aapl.sec_filter.filtered_data)
     # logger.debug(filter_aapl.sec_filter.filtered_data.to_markdown())
 
     # There should only be one record based on the filter
     EntityCommonStockSharesOutstanding = filter_aapl.sec_filter.filtered_data.query(
-        "cik == 320193 and tag == 'EntityCommonStockSharesOutstanding'"
+        "ticker == 'AAPL' and tag == 'EntityCommonStockSharesOutstanding'"
     )
     eo_series = EntityCommonStockSharesOutstanding.value
 
     assert len(eo_series) == 1
     assert eo_series[0] == 15821946000
     assert True == len(filter_aapl.sec_filter.filtered_data) == 1
 
@@ -74,15 +76,15 @@
     sec_filter = SecFilter(
         tags=["EarningsPerShareDiluted"],
         years=1,  # Over the past 1 year
         last_report=ReportDate(year=2023, quarter=1),
         only_annual=True,  # We only want the 10-K
     )
     tickers = frozenset(["aapl", "msft", "goog", "tmo"])
-    sec_instance.select_data(tickers=tickers, filter=sec_filter)
+    sec_instance.filter_data(tickers=tickers, sec_filter=sec_filter)
     logger.debug(sec_filter.filtered_data)
     # Get series for data and make sure they're all yearly-focus(YF)/annual reports
     yearly_focus_periods = "FY"
     quarterly_focus_periods = ("Q1", "Q2", "Q3", "Q4")
     assert False == sec_filter.filtered_data.query("fp in @yearly_focus_periods").empty
     qfp_results = sec_filter.filtered_data.query("fp in @quarterly_focus_periods")
     assert True == qfp_results.empty
```

### Comparing `stocktracer-0.2.0/docs/src/tests/sec/test_sec.py` & `stocktracer-0.3.0/src/tests/sec/test_sec.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import math
 import os
 from pathlib import Path
 
 import mock
 import numpy as np
 import pandas as pd
 import pytest
@@ -41,15 +42,15 @@
     sec.download_manager = mock.MagicMock(DownloadManager)
     return sec, sec.download_manager
 
 
 class TestSec:
     def test_init(self):
         with pytest.raises((TypeError, AssertionError)):
-            Sec()
+            Sec()  # type: ignore
 
     def test_select_data(
         self,
         sec_harness: tuple[Sec, mock.MagicMock],
         fake_sub_txt_sample: str,
         fake_data_txt_sample: str,
     ):
@@ -57,22 +58,25 @@
         data_reader = mock.MagicMock(DataSetReader)
         data_reader.process_zip = mock.MagicMock(return_value=pd.DataFrame())
 
         ticker_reader = mock.MagicMock(TickerReader)
         type(download_manager).ticker_reader = mock.PropertyMock(
             return_value=ticker_reader
         )
+        ticker_reader.map_of_cik_to_ticker = pd.read_json(
+            """{"0":{"cik_str":320193,"ticker":"AAPL","title":"Apple Inc."},
+         "1":{"cik_str":789019,"ticker":"MSFT","title":"MICROSOFT CORP"}}""",
+            orient="index",
+        )
         download_manager.get_quarterly_report = mock.MagicMock(return_value=data_reader)
 
-        with pytest.raises(
-            LookupError, match="No data matching the filter was retrieved"
-        ):
-            sec.select_data(
+        with pytest.raises(KeyError, match="cik"):
+            sec.filter_data(
                 tickers=frozenset(("aapl", "msft")),
-                filter=Filter.SecFilter(tags=["test"]),
+                sec_filter=Filter.SecFilter(tags=["test"]),
             )
         ticker_reader.contains.assert_called()
         download_manager.get_quarterly_report.assert_called()
         data_reader.process_zip.assert_called()
 
         # That's as far s this test goes because it requires download and unzipping and then processing
 
@@ -98,93 +102,119 @@
         """
         (sec, download_manager) = sec_harness
         aapl_filter = filter_aapl_years(1)
         data = sec_manufactured_fake_report_impl(
             aapl_filter, fake_sub_txt_sample, fake_data_txt_sample
         )
         data_reader = mock.MagicMock(DataSetReader)
-        data_reader.process_zip = mock.MagicMock(return_value=data)
+        data_reader.process_zip = mock.MagicMock()
+        data_reader.process_zip.side_effect = [data, None, None, None, None]
         download_manager.get_quarterly_report = mock.MagicMock(return_value=data_reader)
 
         ticker_reader = mock.MagicMock(TickerReader)
         type(download_manager).ticker_reader = mock.PropertyMock(
             return_value=ticker_reader
         )
-        ticker_reader._data = pd.read_json(
+        ticker_reader.map_of_cik_to_ticker = pd.read_json(
             """{"0":{"cik_str":320193,"ticker":"AAPL","title":"Apple Inc."},
          "1":{"cik_str":789019,"ticker":"MSFT","title":"MICROSOFT CORP"}}""",
             orient="index",
         )
 
-        filter = sec.select_data(
+        filter = sec.filter_data(
             tickers=frozenset("aapl"),
-            filter=Filter.SecFilter(last_report=ReportDate(2023, 1)),
+            sec_filter=Filter.SecFilter(last_report=ReportDate(2023, 1)),
         )
 
-        logger.debug(f"\n{data}")
+        logger.debug(f"\n{filter.filtered_data.to_csv()}")
+        # Make sure our bulk processing isn't duplicating data
+        assert len(filter.filtered_data) == len(filter.filtered_data.drop_duplicates())
+
         table = pd.pivot_table(
             filter.filtered_data,
             values="value",
-            index=["cik", "tag"],
+            index=["ticker", "tag"],
             aggfunc=np.average,
         )
         logger.debug(f"processed:\n{table}")
-        assert table.loc[320193].loc["EntityCommonStockSharesOutstanding"][0] == 4000
-        assert table.loc[320193].loc["FakeAttributeTag"][0] == 400
+        assert table.loc["AAPL"].loc["EntityCommonStockSharesOutstanding"][0] == 4000
+        assert table.loc["AAPL"].loc["FakeAttributeTag"][0] == 400
 
         table = filter.select(aggregate_func=np.average)
         logger.debug(f"select_avg:\n{table}")
 
-        assert table.get_value(320193, "EntityCommonStockSharesOutstanding") == 4000
-        assert table.get_value(320193, "FakeAttributeTag") == 400
+        assert (
+            table.get_value("aapl", "EntityCommonStockSharesOutstanding", 2023) == 6000
+        )
+        assert (
+            table.get_value("aapl", "EntityCommonStockSharesOutstanding", 2022) == 3500
+        )
+        assert table.get_value("AAPL", "FakeAttributeTag", 2023) == 600
+        assert table.get_value("AAPL", "FakeAttributeTag", 2022) == 350
+
+        # TODO: See if there's a nice way to leverage pandas mapping to do this simultaneously
+        # table = filter.select(aggregate_func={"EntityCommonStockSharesOutstanding":np.average,
+        #                                       "FakeAttributeTag":np.sum})
+        # logger.debug(f"select_avg_map:\n{table}")
+
+        # assert table.get_value("aapl", "EntityCommonStockSharesOutstanding") == 4000
+        # assert table.get_value("AAPL", "FakeAttributeTag") == 2000
 
         table = filter.select(aggregate_func=np.average, tickers=["bad"])
         # normally bad tickers throw exceptions, but we'll just have it filter on
         # an index we don't have so we get an empty value
         assert table.data.empty == True
 
         # Filter on aapl and get only thses results
         table = filter.select(aggregate_func=np.average, tickers=["aapl"])
         assert table.data.empty == False
         logger.debug(f"processed-ticker:\n{table.data}")
-        assert table.get_value(320193, "EntityCommonStockSharesOutstanding") == 4000
+        assert (
+            table.get_value("aapl", "EntityCommonStockSharesOutstanding", 2023) == 6000
+        )
         # assert table.data.loc[320193].loc["FakeAttributeTag"][0] == 400
         # assert table.data.loc[320193].loc["FakeAttributeTag"][0] == 400
-        assert table.get_value(ticker_or_cik="aapl", tag="FakeAttributeTag") == 400
-        assert table.get_value(ticker_or_cik=320193, tag="FakeAttributeTag") == 400
+        assert table.get_value(ticker="aapl", tag="FakeAttributeTag", year=2023) == 600
 
         assert (
             filter.select(aggregate_func="max", tickers=["aapl"]).get_value(
-                ticker_or_cik=320193, tag="FakeAttributeTag"
+                "aapl", tag="FakeAttributeTag", year=2022
             )
-            == 600
+            == 500
         )
         assert (
             filter.select(aggregate_func="min", tickers=["aapl"]).get_value(
-                ticker_or_cik=320193, tag="FakeAttributeTag"
+                "aapl", tag="FakeAttributeTag", year=2022
             )
             == 200
         )
         assert (
             filter.select(aggregate_func="mean", tickers=["aapl"]).get_value(
-                ticker_or_cik=320193, tag="FakeAttributeTag"
+                "aapl", tag="FakeAttributeTag", year=2022
             )
-            == 400
+            == 350
         )
-        assert (
+        assert math.isclose(
             filter.select(aggregate_func="std", tickers=["aapl"]).get_value(
-                ticker_or_cik=320193, tag="FakeAttributeTag"
-            )
-            == 158.11388300841898
+                "aapl", tag="FakeAttributeTag", year=2022
+            ),
+            129.09944487358,
         )
+
         assert (
             filter.select(aggregate_func="sum", tickers=["aapl"]).get_value(
-                ticker_or_cik=320193, tag="FakeAttributeTag"
+                "aapl", tag="FakeAttributeTag", year=2022
             )
-            == 2000
+            == 1400
         )
         assert (
             filter.select(aggregate_func="var", tickers=["aapl"]).get_value(
-                ticker_or_cik=320193, tag="FakeAttributeTag"
+                "aapl", tag="FakeAttributeTag", year=2022
             )
-            == 25000
+            == 16666.666666666668
+        )
+        assert math.isclose(
+            filter.select(aggregate_func="slope", tickers=["aapl"]).get_value(
+                "aapl", tag="FakeAttributeTag", year=2022
+            ),
+            100,
         )
```

### Comparing `stocktracer-0.2.0/docs/stylesheets/extra.css` & `stocktracer-0.3.0/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/.gitignore` & `stocktracer-0.3.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 .python-version
 
 # pipenv
 #   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
 #   However, in case of collaboration, if having platform-specific dependencies or dependencies
 #   having no cross-platform support, pipenv may install dependencies that don't work, or not
 #   install all needed dependencies.
-#Pipfile.lock
+Pipfile.lock
 
 # PEP 582; used by e.g. github.com/David-OConnor/pyflow
 __pypackages__/
 
 # Celery stuff
 celerybeat-schedule
 celerybeat.pid
```

### Comparing `stocktracer-0.2.0/LICENSE` & `stocktracer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stocktracer-0.2.0/README.md` & `stocktracer-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 <p align="center">
     <a href='https://github.com/gyund/fundamental-analysis/blob/main/LICENSE'><img alt="License" src="https://img.shields.io/github/license/gyund/fundamental-analysis"></a>
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/stocktracer">
     <a href='https://github.com/gyund/fundamental-analysis/actions/workflows/python.yml'><img alt="Test Status" src="https://github.com/gyund/fundamental-analysis/actions/workflows/python.yml/badge.svg?service=github"></a>
     <a href='https://coveralls.io/github/gyund/fundamental-analysis?branch=main'><img src='https://coveralls.io/repos/github/gyund/fundamental-analysis/badge.svg' alt='Coverage Status' /></a>
     <a href="https://beartype.readthedocs.io"><img src="https://raw.githubusercontent.com/beartype/beartype-assets/main/badge/bear-ified.svg?" alt="bear-ified"></a>
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black"></a>
+    <a href='https://pypi.org/project/stocktracer/'><img alt="PyPI - Python Version" src="https://img.shields.io/pypi/v/stocktracer"></a>
     <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/stocktracer">
     <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/stocktracer">
 </p>
 
 # StockTracer
 
 **Stock Analysis Framework**
@@ -27,30 +28,30 @@
 ## Getting Started
 
 ### Users
 
 ```sh
 pip install stocktracer
 
-# Perform analysis (not supported yet)
-stocktracer analyze --tickers aapl,msft
+# Perform analysis
+stocktracer analyze --tickers aapl,msft > report.txt
 
 # Help
 stocktracer
 
 ```
 
 ### Developers
 
 Make sure you have `pipenv` installed through a package manager or through pip.
 
 ```sh
 pipenv install --dev
 
-# Perform analysis (not supported yet)
+# Perform analysis
 PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft
 PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft -a stocktracer.analysis.diluted_eps
 PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft -a stocktracer.analysis.diluted_eps --report-format csv
 PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft -a stocktracer.analysis.diluted_eps --report-format json --report-file my_results.json
 
 # Help
 PYTHONPATH=src pipenv run python -m stocktracer
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
 [License] [PyPI - Python Version] [Test_Status] [Coverage_Status] [bear-ified]
-            [Code_style:_black] [PyPI - Downloads] [PyPI - Status]
+[Code_style:_black] [PyPI_-_Python_Version] [PyPI - Downloads] [PyPI - Status]
 # StockTracer **Stock Analysis Framework** The goal of this project is
 aggregate a variety of ways to consume information about a particular equity
 traded on the US stock market and provide a modular mechanism to process it.
 Core tenants of this project include: - **Heavy data caching** - don't download
 static data more than once - **Efficient use of storage** - leave data
 compressed while not in use - **Batch Processing** - We can't store all
 information in memory, so break problems up - **Speed** - Find and avoid
 bottlenecks of big data processing ## Requirements - `python 3.10+` ## Getting
-Started ### Users ```sh pip install stocktracer # Perform analysis (not
-supported yet) stocktracer analyze --tickers aapl,msft # Help stocktracer ```
-### Developers Make sure you have `pipenv` installed through a package manager
-or through pip. ```sh pipenv install --dev # Perform analysis (not supported
-yet) PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers
-aapl,msft PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers
-aapl,msft -a stocktracer.analysis.diluted_eps PYTHONPATH=src pipenv run python
--m stocktracer analyze --tickers aapl,msft -a stocktracer.analysis.diluted_eps
---report-format csv PYTHONPATH=src pipenv run python -m stocktracer analyze --
-tickers aapl,msft -a stocktracer.analysis.diluted_eps --report-format json --
-report-file my_results.json # Help PYTHONPATH=src pipenv run python -
-m stocktracer # Run Unit Tests pipenv run pytest ``` More information can be
-found in our [documentation](https://gyund.github.io/fundamental-analysis/) ##
-Disclaimer This project seeks to use publicly available information to perform
-security analysis and help perform long term risk analysis. Results provided
-from this project are generally for academic use only and are not considered
-advice or recommendations. This project makes no performance claims or
-guarantees. Please read the [license](LICENSE) for this project. Usage of any
-data is at your own risk.
+Started ### Users ```sh pip install stocktracer # Perform analysis stocktracer
+analyze --tickers aapl,msft > report.txt # Help stocktracer ``` ### Developers
+Make sure you have `pipenv` installed through a package manager or through pip.
+```sh pipenv install --dev # Perform analysis PYTHONPATH=src pipenv run python
+-m stocktracer analyze --tickers aapl,msft PYTHONPATH=src pipenv run python -
+m stocktracer analyze --tickers aapl,msft -a stocktracer.analysis.diluted_eps
+PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft -
+a stocktracer.analysis.diluted_eps --report-format csv PYTHONPATH=src pipenv
+run python -m stocktracer analyze --tickers aapl,msft -
+a stocktracer.analysis.diluted_eps --report-format json --report-file
+my_results.json # Help PYTHONPATH=src pipenv run python -m stocktracer # Run
+Unit Tests pipenv run pytest ``` More information can be found in our
+[documentation](https://gyund.github.io/fundamental-analysis/) ## Disclaimer
+This project seeks to use publicly available information to perform security
+analysis and help perform long term risk analysis. Results provided from this
+project are generally for academic use only and are not considered advice or
+recommendations. This project makes no performance claims or guarantees. Please
+read the [license](LICENSE) for this project. Usage of any data is at your own
+risk.
```

### Comparing `stocktracer-0.2.0/pyproject.toml` & `stocktracer-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.hatch.build.targets.wheel]
 only-include = ["src/stocktracer"]
 sources = ["src"]
 
 [project]
 name = "stocktracer"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Gary Yund", email="gary.yund@gmail.com" },
 ]
 description = "Tools for aggregating efficient ways to consume and process publically traded equities on the US stock market. Includes support for SEC quarterly data processing."
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
@@ -102,15 +102,15 @@
 match = '(?!(test_|conftest)).*\.py'
 match_dir = '^(?!(venv|tests|poc)).*'
 convention = "pep257"
 ignore_self_only_init = true
 
 [tool.pylint.main]
 source-roots = ["src"]
-fail-under = 9
+fail-under = 9.5
 fail-on = [
     # "redefined-builtin",    # unintended sideaffects
     "unused-variable",      # cleaner code
     "unused-import",        # cleaner code
     "no-self-argument",     # possible bug, annotate correctly
     "use-list-literal",     # cleaner code
     "no-else-return",       # cleaner code
```

### Comparing `stocktracer-0.2.0/PKG-INFO` & `stocktracer-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocktracer
-Version: 0.2.0
+Version: 0.3.0
 Summary: Tools for aggregating efficient ways to consume and process publically traded equities on the US stock market. Includes support for SEC quarterly data processing.
 Project-URL: Homepage, https://gyund.github.io/fundamental-analysis/
 Project-URL: Bug Tracker, https://github.com/gyund/fundamental-analysis/issues
 Author-email: Gary Yund <gary.yund@gmail.com>
 License: Eclipse Public License - v 2.0
         
             THE ACCOMPANYING PROGRAM IS PROVIDED UNDER THE TERMS OF THIS ECLIPSE
@@ -290,45 +290,49 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.10
+Requires-Dist: about-time==4.2.1; python_version >= '3.7' and python_version < '4'
+Requires-Dist: alive-progress==3.1.2
 Requires-Dist: attrs==23.1.0; python_version >= '3.7'
 Requires-Dist: beartype==0.14.0
 Requires-Dist: cattrs==22.2.0; python_version >= '3.7'
 Requires-Dist: certifi==2023.5.7; python_version >= '3.6'
 Requires-Dist: charset-normalizer==3.1.0; python_full_version >= '3.7.0'
 Requires-Dist: diskcache==5.6.1
 Requires-Dist: exceptiongroup==1.1.1; python_version < '3.11'
 Requires-Dist: fire==0.5.0
+Requires-Dist: grapheme==0.6.0
 Requires-Dist: idna==3.4; python_version >= '3.5'
 Requires-Dist: numpy==1.24.3; python_version >= '3.10'
 Requires-Dist: pandas==2.0.1
 Requires-Dist: platformdirs==3.5.1; python_version >= '3.7'
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: pytz==2023.3
 Requires-Dist: requests-cache==1.0.1
-Requires-Dist: requests==2.30.0
-Requires-Dist: six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
+Requires-Dist: requests==2.31.0
+Requires-Dist: six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: termcolor==2.3.0; python_version >= '3.7'
 Requires-Dist: tzdata==2023.3; python_version >= '2'
 Requires-Dist: url-normalize==1.4.3; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
 Requires-Dist: urllib3==2.0.2; python_version >= '3.7'
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href='https://github.com/gyund/fundamental-analysis/blob/main/LICENSE'><img alt="License" src="https://img.shields.io/github/license/gyund/fundamental-analysis"></a>
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/stocktracer">
     <a href='https://github.com/gyund/fundamental-analysis/actions/workflows/python.yml'><img alt="Test Status" src="https://github.com/gyund/fundamental-analysis/actions/workflows/python.yml/badge.svg?service=github"></a>
     <a href='https://coveralls.io/github/gyund/fundamental-analysis?branch=main'><img src='https://coveralls.io/repos/github/gyund/fundamental-analysis/badge.svg' alt='Coverage Status' /></a>
     <a href="https://beartype.readthedocs.io"><img src="https://raw.githubusercontent.com/beartype/beartype-assets/main/badge/bear-ified.svg?" alt="bear-ified"></a>
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black"></a>
+    <a href='https://pypi.org/project/stocktracer/'><img alt="PyPI - Python Version" src="https://img.shields.io/pypi/v/stocktracer"></a>
     <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/stocktracer">
     <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/stocktracer">
 </p>
 
 # StockTracer
 
 **Stock Analysis Framework**
@@ -347,30 +351,30 @@
 ## Getting Started
 
 ### Users
 
 ```sh
 pip install stocktracer
 
-# Perform analysis (not supported yet)
-stocktracer analyze --tickers aapl,msft
+# Perform analysis
+stocktracer analyze --tickers aapl,msft > report.txt
 
 # Help
 stocktracer
 
 ```
 
 ### Developers
 
 Make sure you have `pipenv` installed through a package manager or through pip.
 
 ```sh
 pipenv install --dev
 
-# Perform analysis (not supported yet)
+# Perform analysis
 PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft
 PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft -a stocktracer.analysis.diluted_eps
 PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft -a stocktracer.analysis.diluted_eps --report-format csv
 PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft -a stocktracer.analysis.diluted_eps --report-format json --report-file my_results.json
 
 # Help
 PYTHONPATH=src pipenv run python -m stocktracer
```

