# Comparing `tmp/ddev-2.0.0.tar.gz` & `tmp/ddev-2.1.0.tar.gz`

## Comparing `ddev-2.0.0.tar` & `ddev-2.1.0.tar`

### file list

```diff
@@ -1,92 +1,94 @@
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 ddev-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/__about__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/py.typed
--rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/__init__.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/application.py
--rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/terminal.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/ci/__init__.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/config/__init__.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/docs/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/env/__init__.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/meta/__init__.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/meta/scripts/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/release/__init__.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/release/agent/__init__.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/release/show/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/release/stats/__init__.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/status/__init__.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/validate/__init__.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/validate/ci.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/cli/validate/manifest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/config/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/config/constants.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/config/file.py
--rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/config/model.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/config/utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/integration/__init__.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/integration/core.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/integration/manifest.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/plugin/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/plugin/api.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/plugin/specs.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/plugin/external/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/plugin/external/starship/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/plugin/external/starship/__main__.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/plugin/external/starship/prompt.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/repo/__init__.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/repo/config.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/repo/constants.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/repo/core.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/ci.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/fs.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/git.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/json.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/network.py
--rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/platform.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/structures.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/toml.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/scripts/__init__.py
--rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/utils/scripts/ci_matrix.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/validation/__init__.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 ddev-2.0.0/src/ddev/validation/tracker.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/test__utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/config/__init__.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/config/test_edit.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/config/test_explore.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/config/test_find.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/config/test_restore.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/config/test_set.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/config/test_show.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/status/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/status/test_status.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/validate/__init__.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/cli/validate/test_manifest.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/config/__init__.py
--rw-r--r--   0        0        0    40933 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/config/test_model.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/helpers/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/helpers/api.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/integration/test_core.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/integration/test_manifest.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/repo/__init__.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/repo/test_config.py
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/repo/test_core.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/utils/test_fs.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/utils/test_git.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/utils/test_json.py
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/utils/test_platform.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/utils/test_structures.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/validation/__init__.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 ddev-2.0.0/tests/validation/test_tracker.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 ddev-2.0.0/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ddev-2.0.0/README.md
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 ddev-2.0.0/hatch.toml
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 ddev-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 ddev-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 ddev-2.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/__about__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/py.typed
+-rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/__init__.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/application.py
+-rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/terminal.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/ci/__init__.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/config/__init__.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/docs/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/env/__init__.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/meta/__init__.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/meta/scripts/__init__.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/release/__init__.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/release/agent/__init__.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/release/show/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/release/stats/__init__.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/status/__init__.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/validate/__init__.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/validate/ci.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/validate/manifest.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/validate/openmetrics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/config/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/config/constants.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/config/file.py
+-rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/config/model.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/config/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/integration/__init__.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/integration/core.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/integration/manifest.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/plugin/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/plugin/api.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/plugin/specs.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/plugin/external/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/plugin/external/starship/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/plugin/external/starship/__main__.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/plugin/external/starship/prompt.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/repo/__init__.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/repo/config.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/repo/constants.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/repo/core.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/ci.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/fs.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/git.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/json.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/network.py
+-rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/platform.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/structures.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/toml.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/scripts/__init__.py
+-rw-r--r--   0        0        0     9620 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/scripts/ci_matrix.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/validation/__init__.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/validation/tracker.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/test__utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/config/__init__.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/config/test_edit.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/config/test_explore.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/config/test_find.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/config/test_restore.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/config/test_set.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/config/test_show.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/status/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/status/test_status.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/validate/__init__.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/validate/test_manifest.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/validate/test_openmetrics.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/config/__init__.py
+-rw-r--r--   0        0        0    40933 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/config/test_model.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/helpers/api.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/integration/test_core.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/integration/test_manifest.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/repo/__init__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/repo/test_config.py
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/repo/test_core.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/utils/test_fs.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/utils/test_git.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/utils/test_json.py
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/utils/test_platform.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/utils/test_structures.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/validation/__init__.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/validation/test_tracker.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 ddev-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ddev-2.1.0/README.md
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 ddev-2.1.0/hatch.toml
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 ddev-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 ddev-2.1.0/PKG-INFO
```

### Comparing `ddev-2.0.0/CHANGELOG.md` & `ddev-2.1.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # CHANGELOG - ddev
 
+## 2.1.0 / 2023-05-26
+
+* [Added] Add validation for metric limit. See [#14528](https://github.com/DataDog/integrations-core/pull/14528).
+* [Fixed] Consider changes to `metadata.csv` as testable. See [#14429](https://github.com/DataDog/integrations-core/pull/14429).
+* [Fixed] Account for dependency upgrades in CI matrix logic. See [#14366](https://github.com/DataDog/integrations-core/pull/14366).
+* [Fixed] Fix edge case in CI matrix construction. See [#14355](https://github.com/DataDog/integrations-core/pull/14355).
+
 ## 2.0.0 / 2023-04-11
 
 * [Changed] Replace flake8 and isort with Ruff. See [#14212](https://github.com/DataDog/integrations-core/pull/14212).
 
 ## 1.6.0 / 2023-03-31
 
 * [Added] Add GitHub Actions workflows. See [#14187](https://github.com/DataDog/integrations-core/pull/14187).
```

### Comparing `ddev-2.0.0/src/ddev/cli/__init__.py` & `ddev-2.1.0/src/ddev/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/cli/application.py` & `ddev-2.1.0/src/ddev/cli/application.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/cli/terminal.py` & `ddev-2.1.0/src/ddev/cli/terminal.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/cli/config/__init__.py` & `ddev-2.1.0/src/ddev/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/cli/env/__init__.py` & `ddev-2.1.0/src/ddev/cli/env/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/cli/meta/__init__.py` & `ddev-2.1.0/src/ddev/cli/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/cli/meta/scripts/__init__.py` & `ddev-2.1.0/src/ddev/cli/meta/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/cli/release/__init__.py` & `ddev-2.1.0/src/ddev/cli/release/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/cli/release/agent/__init__.py` & `ddev-2.1.0/src/ddev/cli/release/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/cli/release/show/__init__.py` & `ddev-2.1.0/src/ddev/cli/release/show/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/cli/status/__init__.py` & `ddev-2.1.0/src/ddev/cli/status/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/cli/validate/__init__.py` & `ddev-2.1.0/src/ddev/cli/validate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from datadog_checks.dev.tooling.commands.validate.recommended_monitors import recommended_monitors
 from datadog_checks.dev.tooling.commands.validate.saved_views import saved_views
 from datadog_checks.dev.tooling.commands.validate.service_checks import service_checks
 from datadog_checks.dev.tooling.commands.validate.typos import typos
 
 from ddev.cli.validate.ci import ci
 from ddev.cli.validate.manifest import manifest
+from ddev.cli.validate.openmetrics import openmetrics
 
 
 @click.group(short_help='Verify certain aspects of the repo')
 def validate():
     """
     Verify certain aspects of the repo.
     """
@@ -50,13 +51,14 @@
 validate.add_command(jmx_metrics)
 validate.add_command(legacy_signature)
 validate.add_command(license_headers)
 validate.add_command(licenses)
 validate.add_command(manifest)
 validate.add_command(metadata)
 validate.add_command(models)
+validate.add_command(openmetrics)
 validate.add_command(package)
 validate.add_command(readmes)
 validate.add_command(recommended_monitors)
 validate.add_command(saved_views)
 validate.add_command(service_checks)
 validate.add_command(typos)
```

### Comparing `ddev-2.0.0/src/ddev/cli/validate/ci.py` & `ddev-2.1.0/src/ddev/cli/validate/ci.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/cli/validate/manifest.py` & `ddev-2.1.0/src/ddev/cli/validate/manifest.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/config/file.py` & `ddev-2.1.0/src/ddev/config/file.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/config/model.py` & `ddev-2.1.0/src/ddev/config/model.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/config/utils.py` & `ddev-2.1.0/src/ddev/config/utils.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/integration/core.py` & `ddev-2.1.0/src/ddev/integration/core.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/repo/core.py` & `ddev-2.1.0/src/ddev/repo/core.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/utils/fs.py` & `ddev-2.1.0/src/ddev/utils/fs.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/utils/git.py` & `ddev-2.1.0/src/ddev/utils/git.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/utils/json.py` & `ddev-2.1.0/src/ddev/utils/json.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/utils/platform.py` & `ddev-2.1.0/src/ddev/utils/platform.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/utils/structures.py` & `ddev-2.1.0/src/ddev/utils/structures.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/src/ddev/utils/scripts/ci_matrix.py` & `ddev-2.1.0/src/ddev/utils/scripts/ci_matrix.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import argparse
 import json
 import os
 import re
 import subprocess
 import sys
 from collections import defaultdict, namedtuple
-from fnmatch import fnmatch
 from functools import lru_cache
 from pathlib import Path
 from typing import Any
 
 if sys.version_info[:2] >= (3, 11):
     import tomllib
 # TODO: remove this once ddev drops versions less than 3.11
@@ -30,26 +29,34 @@
 OUTPUT_LIMIT = 1024 * 1024
 
 # https://docs.github.com/en/actions/using-jobs/using-a-matrix-for-your-jobs#using-a-matrix-strategy
 JOB_LIMIT = 256
 
 # GitHub Actions' `paths-ignore` job filtering option requires that every changed path must match at least one of
 # the exclusion patterns, but we want any to cause that condition for the core repository to run all jobs
-SKIPPED_PATTERNS = (
-    'datadog_checks_base/datadog_checks/**',
-    'datadog_checks_dev/datadog_checks/dev/*.py',
+SKIPPED_PATTERN = re.compile(
+    r"""
+    datadog_checks_base/datadog_checks/.+
+  | datadog_checks_dev/datadog_checks/dev/[^/]+\.py
+    """,
+    re.VERBOSE,
 )
-TESTABLE_FILE_PATTERNS = (
-    'assets/configuration/**/*',
-    'tests/**/*',
-    '*.py',
-    'hatch.toml',
-    'pyproject.toml',
+TESTABLE_FILE_PATTERN = re.compile(
+    r"""
+    assets/configuration/.+
+  | tests/.+
+  | [^/]+\.py
+  | hatch\.toml
+  | metadata\.csv
+  | pyproject\.toml
+    """,
+    re.VERBOSE,
 )
-NON_TESTABLE_FILES = {'auto_conf.yaml', 'agent_requirements.in'}
+AGENT_REQUIREMENTS_FILE = 'datadog_checks_base/datadog_checks/base/data/agent_requirements.in'
+NON_TESTABLE_FILES = {'auto_conf.yaml'}
 DISPLAY_ORDER_OVERRIDE = {
     _d: _i
     for _i, _d in enumerate(
         (
             'ddev',
             'datadog_checks_base',
             'datadog_checks_dev',
@@ -124,38 +131,39 @@
 
 
 def get_changed_targets(root: Path, *, ref: str, local: bool, verbose: bool) -> list[str]:
     changed_files = get_changed_files(ref=ref, local=local)
     if verbose:
         print('\n'.join(changed_files), file=sys.stderr)
 
-    if (root / 'datadog_checks_base').is_dir() and any(
-        fnmatch(str(root / changed_file), str(root / pattern))
-        for changed_file in changed_files
-        for pattern in SKIPPED_PATTERNS
+    if (
+        (root / 'datadog_checks_base').is_dir()
+        and AGENT_REQUIREMENTS_FILE not in changed_files
+        and any(SKIPPED_PATTERN.search(path) for path in changed_files)
     ):
         return []
 
     changed_directories: defaultdict[str, list[str]] = defaultdict(list)
     for changed_file in changed_files:
         directory_name, _, remaining_path = changed_file.partition('/')
         if remaining_path:
             changed_directories[directory_name].append(remaining_path)
 
+    agent_requirements_file = root / AGENT_REQUIREMENTS_FILE
     targets = []
     for directory_name, files in changed_directories.items():
         directory = root / directory_name
         if not ((directory / 'hatch.toml').is_file() and (directory / 'tests').is_dir()):
             continue
 
         for remaining_path in files:
             possible_file = directory / remaining_path
-            if possible_file.name in NON_TESTABLE_FILES:
+            if possible_file.name in NON_TESTABLE_FILES or possible_file == agent_requirements_file:
                 continue
-            elif any(fnmatch(str(possible_file), str(directory / pattern)) for pattern in TESTABLE_FILE_PATTERNS):
+            elif TESTABLE_FILE_PATTERN.search(remaining_path):
                 targets.append(directory_name)
                 break
 
     return targets
 
 
 def get_all_targets(root: Path) -> list[str]:
```

### Comparing `ddev-2.0.0/src/ddev/validation/tracker.py` & `ddev-2.1.0/src/ddev/validation/tracker.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/conftest.py` & `ddev-2.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/test__utils.py` & `ddev-2.1.0/tests/test__utils.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/cli/config/test_find.py` & `ddev-2.1.0/tests/cli/config/test_find.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/cli/config/test_restore.py` & `ddev-2.1.0/tests/cli/config/test_restore.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/cli/config/test_set.py` & `ddev-2.1.0/tests/cli/config/test_set.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/cli/config/test_show.py` & `ddev-2.1.0/tests/cli/config/test_show.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/cli/status/test_status.py` & `ddev-2.1.0/tests/cli/status/test_status.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/cli/validate/test_manifest.py` & `ddev-2.1.0/tests/cli/validate/test_manifest.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/config/test_model.py` & `ddev-2.1.0/tests/config/test_model.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/helpers/api.py` & `ddev-2.1.0/tests/helpers/api.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/integration/test_core.py` & `ddev-2.1.0/tests/integration/test_core.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/repo/test_core.py` & `ddev-2.1.0/tests/repo/test_core.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/utils/test_fs.py` & `ddev-2.1.0/tests/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/utils/test_git.py` & `ddev-2.1.0/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/utils/test_json.py` & `ddev-2.1.0/tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/utils/test_platform.py` & `ddev-2.1.0/tests/utils/test_platform.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/utils/test_structures.py` & `ddev-2.1.0/tests/utils/test_structures.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/tests/validation/test_tracker.py` & `ddev-2.1.0/tests/validation/test_tracker.py`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/.gitignore` & `ddev-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/README.md` & `ddev-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/pyproject.toml` & `ddev-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ddev-2.0.0/PKG-INFO` & `ddev-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddev
-Version: 2.0.0
+Version: 2.1.0
 Summary: The Datadog Agent integration developer tool
 Project-URL: Source, https://github.com/DataDog/integrations-core
 Author-email: Datadog <packages@datadoghq.com>
 License-Expression: BSD-3-Clause
 Keywords: agent,datadog,integration
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

