# Comparing `tmp/sfapi_client-0.0.3.tar.gz` & `tmp/sfapi_client-0.0.4.tar.gz`

## Comparing `sfapi_client-0.0.3.tar` & `sfapi_client-0.0.4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/LEGAL
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/mkdocs.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/pytest.ini
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/requirements-dev.txt
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/.github/workflows/pytest.yml
--rwxr-xr-x   0        0        0     1097 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/gen_examples.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/gen_sync.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/index.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/community/contributing.md
--rw-r--r--   0        0        0    52808 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/examples/check_current_and_past_jobs.ipynb
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/examples/getting_bearer_token.ipynb
--rw-r--r--   0        0        0    11986 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/examples/run_job_and_check_status.ipynb
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/javascript/apiselector.js
--rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/quickstart/index.md
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/SUMMARY.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/client/index.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/compute/index.md
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/exceptions/index.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/groups/index.md
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/jobs/index.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/paths/index.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/projects/index.md
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/resources/index.md
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/users/index.md
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/scripts/run.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_compute.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_jobs.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_monitor.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/client.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/compute.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/exceptions.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/groups.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/jobs.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/paths.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/projects.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/resources.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_async/__init__.py
--rw-r--r--   0        0        0    15934 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_async/client.py
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_async/compute.py
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_async/groups.py
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_async/jobs.py
--rw-r--r--   0        0        0    11133 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_async/paths.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_async/projects.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_async/users.py
--rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_models/__init__.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_models/job_status_response_sacct.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_models/job_status_response_squeue.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_models/resources.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/__init__.py
--rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/_models.py
--rw-r--r--   0        0        0    15536 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/client.py
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/compute.py
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/groups.py
--rw-r--r--   0        0        0     7356 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/jobs.py
--rw-r--r--   0        0        0    11414 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/paths.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/projects.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/users.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_api.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_api_async.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_client.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_client_async.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_compute.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_compute_async.py
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_groups.py
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_groups_async.py
--rwxr-xr-x   0        0        0     4647 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_jobs.py
--rwxr-xr-x   0        0        0     6378 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_jobs_async.py
--rw-r--r--   0        0        0     8037 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_paths.py
--rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_paths_async.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_projects.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_projects_async.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_resources.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_resources_async.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_users.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_users_async.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/.gitignore
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/LICENSE
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/README.md
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/LEGAL
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/mkdocs.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/pytest.ini
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/requirements-dev.txt
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/.github/workflows/pytest.yml
+-rwxr-xr-x   0        0        0     1097 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/gen_examples.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/gen_sync.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/index.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/community/contributing.md
+-rw-r--r--   0        0        0    52808 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/examples/check_current_and_past_jobs.ipynb
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/examples/getting_bearer_token.ipynb
+-rw-r--r--   0        0        0    11986 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/examples/run_job_and_check_status.ipynb
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/javascript/apiselector.js
+-rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/quickstart/index.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/SUMMARY.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/client/index.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/compute/index.md
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/exceptions/index.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/groups/index.md
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/jobs/index.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/paths/index.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/projects/index.md
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/resources/index.md
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/users/index.md
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/scripts/run.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_compute.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_jobs.py
+-rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_monitor.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/client.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/compute.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/exceptions.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/groups.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/jobs.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/paths.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/projects.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/resources.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_async/__init__.py
+-rw-r--r--   0        0        0    15934 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_async/client.py
+-rw-r--r--   0        0        0     6564 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_async/compute.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_async/groups.py
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_async/jobs.py
+-rw-r--r--   0        0        0    11133 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_async/paths.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_async/projects.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_async/users.py
+-rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_models/__init__.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_models/job_status_response_sacct.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_models/job_status_response_squeue.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_models/resources.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/__init__.py
+-rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/_models.py
+-rw-r--r--   0        0        0    15536 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/client.py
+-rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/compute.py
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/groups.py
+-rw-r--r--   0        0        0     7356 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/jobs.py
+-rw-r--r--   0        0        0    11414 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/paths.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/projects.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/users.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_api.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_api_async.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_client.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_client_async.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_compute.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_compute_async.py
+-rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_groups.py
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_groups_async.py
+-rwxr-xr-x   0        0        0     4647 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_jobs.py
+-rwxr-xr-x   0        0        0     6378 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_jobs_async.py
+-rw-r--r--   0        0        0     8037 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_paths.py
+-rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_paths_async.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_projects.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_projects_async.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_resources.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_resources_async.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_users.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_users_async.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/.gitignore
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/README.md
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/PKG-INFO
```

### Comparing `sfapi_client-0.0.3/LEGAL` & `sfapi_client-0.0.4/LEGAL`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/mkdocs.yml` & `sfapi_client-0.0.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/.github/workflows/mkdocs.yml` & `sfapi_client-0.0.4/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/.github/workflows/pypi.yml` & `sfapi_client-0.0.4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/.github/workflows/pytest.yml` & `sfapi_client-0.0.4/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/docs/gen_examples.py` & `sfapi_client-0.0.4/docs/gen_examples.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/docs/gen_sync.py` & `sfapi_client-0.0.4/docs/gen_sync.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/docs/index.md` & `sfapi_client-0.0.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/docs/examples/check_current_and_past_jobs.ipynb` & `sfapi_client-0.0.4/docs/examples/check_current_and_past_jobs.ipynb`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/docs/examples/getting_bearer_token.ipynb` & `sfapi_client-0.0.4/docs/examples/getting_bearer_token.ipynb`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/docs/examples/run_job_and_check_status.ipynb` & `sfapi_client-0.0.4/docs/examples/run_job_and_check_status.ipynb`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/docs/javascript/apiselector.js` & `sfapi_client-0.0.4/docs/javascript/apiselector.js`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/docs/quickstart/index.md` & `sfapi_client-0.0.4/docs/quickstart/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/docs/reference/SUMMARY.txt` & `sfapi_client-0.0.4/docs/reference/SUMMARY.txt`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/docs/reference/async/compute/index.md` & `sfapi_client-0.0.4/docs/reference/async/compute/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/docs/reference/async/groups/index.md` & `sfapi_client-0.0.4/docs/reference/async/groups/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/docs/reference/async/jobs/index.md` & `sfapi_client-0.0.4/docs/reference/async/jobs/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/docs/reference/async/paths/index.md` & `sfapi_client-0.0.4/docs/reference/async/paths/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/docs/reference/async/projects/index.md` & `sfapi_client-0.0.4/docs/reference/async/projects/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/scripts/run.py` & `sfapi_client-0.0.4/scripts/run.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_jobs.py` & `sfapi_client-0.0.4/src/sfapi_client/_jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_monitor.py` & `sfapi_client-0.0.4/src/sfapi_client/_monitor.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,16 +58,17 @@
             index_of_next_type = (index_of_next_type + 1) % len(possible_job_types)
 
         self._last_job_type_fetched = job_type
 
         return job_type
 
     async def fetch_jobs(
-        self, job_type: Union[AsyncJobSacct, AsyncJobSqueue], jobids: List[int]
+        self, job_type: Union[AsyncJobSacct, AsyncJobSqueue], jobids: List[Union[int, str]]
     ) -> List[Union[AsyncJobSacct, AsyncJobSqueue]]:
+        jobids = list(map(str, jobids))
         jobids_for_type = self._jobids.setdefault(job_type, set())
         jobids_for_type.update(jobids)
 
         if self._monitor_task is None:
             await self._create_task()
             jobs = await self._monitor_task
             # process jobs and return
@@ -128,16 +129,17 @@
         self._requests: Dict[Type, Set[JobRequest]] = {}
         # Lock to protect access to self._requests
         self._requests_lock = Lock()
         # Lock to prevent multiple server requests concurrently
         self._request_lock = Lock()
 
     def fetch_jobs(
-        self, job_type: Union["JobSacct", "JobSqueue"], jobids: List[int]
+        self, job_type: Union["JobSacct", "JobSqueue"], jobids: List[Union[int, str]]
     ) -> List[Union[JobSqueue, JobSacct]]:
+        jobids = list(map(str, jobids))
         # First update the jobids and create a request context
         request = None
         with self._requests_lock:
             request = JobRequest(jobids)
             self._requests.setdefault(job_type, set()).add(request)
 
         # Only allow a single request at a time
```

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_async/client.py` & `sfapi_client-0.0.4/src/sfapi_client/_async/client.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_async/compute.py` & `sfapi_client-0.0.4/src/sfapi_client/_async/compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,28 +117,28 @@
         job = AsyncJobSqueue(jobid=jobid)
         job.compute = self
 
         return job
 
     @check_auth
     async def job(
-        self, jobid: int, command: Optional[JobCommand] = JobCommand.sacct
+        self, jobid: Union[int, str], command: Optional[JobCommand] = JobCommand.sacct
     ) -> Union["AsyncJobSacct", "AsyncJobSqueue"]:
         # Get different job depending on query
         Job = AsyncJobSacct if (command == JobCommand.sacct) else AsyncJobSqueue
         jobs = await self._monitor.fetch_jobs(job_type=Job, jobids=[jobid])
         if len(jobs) == 0:
             raise SfApiError(f"Job not found: ${jobid}")
 
         return jobs[0]
 
     @check_auth
     async def jobs(
         self,
-        jobids: Optional[int] = None,
+        jobids: Optional[List[Union[int, str]]] = None,
         user: Optional[str] = None,
         partition: Optional[str] = None,
         command: Optional[JobCommand] = JobCommand.squeue,
     ) -> List[Union[AsyncJobSacct, AsyncJobSqueue]]:
         Job = AsyncJobSacct if (command == JobCommand.sacct) else AsyncJobSqueue
 
         # If we have been given just jobids, use the monitor
```

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_async/groups.py` & `sfapi_client-0.0.4/src/sfapi_client/_async/groups.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_async/jobs.py` & `sfapi_client-0.0.4/src/sfapi_client/_async/jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_async/paths.py` & `sfapi_client-0.0.4/src/sfapi_client/_async/paths.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_async/projects.py` & `sfapi_client-0.0.4/src/sfapi_client/_async/projects.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_async/users.py` & `sfapi_client-0.0.4/src/sfapi_client/_async/users.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_models/__init__.py` & `sfapi_client-0.0.4/src/sfapi_client/_models/__init__.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_models/job_status_response_sacct.py` & `sfapi_client-0.0.4/src/sfapi_client/_models/job_status_response_sacct.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_models/job_status_response_squeue.py` & `sfapi_client-0.0.4/src/sfapi_client/_models/job_status_response_squeue.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_models/resources.py` & `sfapi_client-0.0.4/src/sfapi_client/_models/resources.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_sync/_models.py` & `sfapi_client-0.0.4/src/sfapi_client/_sync/_models.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_sync/client.py` & `sfapi_client-0.0.4/src/sfapi_client/_sync/client.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_sync/compute.py` & `sfapi_client-0.0.4/src/sfapi_client/_sync/compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,28 +117,28 @@
         job = JobSqueue(jobid=jobid)
         job.compute = self
 
         return job
 
     @check_auth
     def job(
-        self, jobid: int, command: Optional[JobCommand] = JobCommand.sacct
+        self, jobid: Union[int, str], command: Optional[JobCommand] = JobCommand.sacct
     ) -> Union["JobSacct", "JobSqueue"]:
         # Get different job depending on query
         Job = JobSacct if (command == JobCommand.sacct) else JobSqueue
         jobs = self._monitor.fetch_jobs(job_type=Job, jobids=[jobid])
         if len(jobs) == 0:
             raise SfApiError(f"Job not found: ${jobid}")
 
         return jobs[0]
 
     @check_auth
     def jobs(
         self,
-        jobids: Optional[int] = None,
+        jobids: Optional[List[Union[int, str]]] = None,
         user: Optional[str] = None,
         partition: Optional[str] = None,
         command: Optional[JobCommand] = JobCommand.squeue,
     ) -> List[Union[JobSacct, JobSqueue]]:
         Job = JobSacct if (command == JobCommand.sacct) else JobSqueue
 
         # If we have been given just jobids, use the monitor
```

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_sync/groups.py` & `sfapi_client-0.0.4/src/sfapi_client/_sync/groups.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_sync/jobs.py` & `sfapi_client-0.0.4/src/sfapi_client/_sync/jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_sync/paths.py` & `sfapi_client-0.0.4/src/sfapi_client/_sync/paths.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_sync/projects.py` & `sfapi_client-0.0.4/src/sfapi_client/_sync/projects.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/src/sfapi_client/_sync/users.py` & `sfapi_client-0.0.4/src/sfapi_client/_sync/users.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/tests/conftest.py` & `sfapi_client-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/tests/test_compute.py` & `sfapi_client-0.0.4/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/tests/test_compute_async.py` & `sfapi_client-0.0.4/tests/test_compute_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/tests/test_groups.py` & `sfapi_client-0.0.4/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/tests/test_groups_async.py` & `sfapi_client-0.0.4/tests/test_groups_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/tests/test_jobs.py` & `sfapi_client-0.0.4/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/tests/test_jobs_async.py` & `sfapi_client-0.0.4/tests/test_jobs_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/tests/test_paths.py` & `sfapi_client-0.0.4/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/tests/test_paths_async.py` & `sfapi_client-0.0.4/tests/test_paths_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/tests/test_projects.py` & `sfapi_client-0.0.4/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/tests/test_projects_async.py` & `sfapi_client-0.0.4/tests/test_projects_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/tests/test_resources.py` & `sfapi_client-0.0.4/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/tests/test_resources_async.py` & `sfapi_client-0.0.4/tests/test_resources_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/tests/test_users.py` & `sfapi_client-0.0.4/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/tests/test_users_async.py` & `sfapi_client-0.0.4/tests/test_users_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/LICENSE` & `sfapi_client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/README.md` & `sfapi_client-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/pyproject.toml` & `sfapi_client-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.3/PKG-INFO` & `sfapi_client-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfapi_client
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python client for NERSC SF API
 Author-email: Chris Harris <cjh@lbl.gov>, Nicholas Tyler <tylern@lbl.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

