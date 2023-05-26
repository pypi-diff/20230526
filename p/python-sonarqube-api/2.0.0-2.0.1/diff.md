# Comparing `tmp/python-sonarqube-api-2.0.0.tar.gz` & `tmp/python-sonarqube-api-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sonarqube-api-2.0.0.tar", last modified: Fri May 26 07:25:57 2023, max compression
+gzip compressed data, was "python-sonarqube-api-2.0.1.tar", last modified: Fri May 26 14:53:49 2023, max compression
```

## Comparing `python-sonarqube-api-2.0.0.tar` & `python-sonarqube-api-2.0.1.tar`

### file list

```diff
@@ -1,66 +1,50 @@
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 07:25:57.081134 python-sonarqube-api-2.0.0/
--rw-r--r--   0 shijialiang   (501) staff       (20)    34523 2023-05-26 04:56:09.000000 python-sonarqube-api-2.0.0/LICENSE
--rw-r--r--   0 shijialiang   (501) staff       (20)       33 2022-05-23 11:32:43.000000 python-sonarqube-api-2.0.0/MANIFEST.in
--rw-r--r--   0 shijialiang   (501) staff       (20)     5999 2023-05-26 07:25:57.079442 python-sonarqube-api-2.0.0/PKG-INFO
--rw-r--r--   0 shijialiang   (501) staff       (20)     4880 2023-05-26 07:11:49.000000 python-sonarqube-api-2.0.0/README.rst
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 07:25:57.018330 python-sonarqube-api-2.0.0/python_sonarqube_api.egg-info/
--rw-r--r--   0 shijialiang   (501) staff       (20)     5999 2023-05-26 07:25:56.000000 python-sonarqube-api-2.0.0/python_sonarqube_api.egg-info/PKG-INFO
--rw-r--r--   0 shijialiang   (501) staff       (20)     1689 2023-05-26 07:25:56.000000 python-sonarqube-api-2.0.0/python_sonarqube_api.egg-info/SOURCES.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        1 2023-05-26 07:25:56.000000 python-sonarqube-api-2.0.0/python_sonarqube_api.egg-info/dependency_links.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        9 2023-05-26 07:25:56.000000 python-sonarqube-api-2.0.0/python_sonarqube_api.egg-info/requires.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)       10 2023-05-26 07:25:56.000000 python-sonarqube-api-2.0.0/python_sonarqube_api.egg-info/top_level.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        9 2022-05-23 11:32:43.000000 python-sonarqube-api-2.0.0/requirements.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)       38 2023-05-26 07:25:57.081239 python-sonarqube-api-2.0.0/setup.cfg
--rw-r--r--   0 shijialiang   (501) staff       (20)     2497 2023-05-26 07:25:32.000000 python-sonarqube-api-2.0.0/setup.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 07:25:57.021285 python-sonarqube-api-2.0.0/sonarqube/
--rw-r--r--   0 shijialiang   (501) staff       (20)      192 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/__init__.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 07:25:57.073487 python-sonarqube-api-2.0.0/sonarqube/rest/
--rw-r--r--   0 shijialiang   (501) staff       (20)    10384 2023-05-26 06:28:40.000000 python-sonarqube-api-2.0.0/sonarqube/rest/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4212 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/alm_integrations.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    12832 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/alm_settings.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      867 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/analysis_cache.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4930 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/applications.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      988 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/audit_logs.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1089 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/auth.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3668 2023-05-26 06:25:25.000000 python-sonarqube-api-2.0.0/sonarqube/rest/ce.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3972 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/components.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      814 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/duplications.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      742 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/editions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1504 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/favorites.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3238 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/hotspots.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    13831 2023-05-26 06:25:25.000000 python-sonarqube-api-2.0.0/sonarqube/rest/issues.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      723 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/languages.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     5441 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/measures.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      947 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/metrics.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      890 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/monitoring.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2593 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/new_code_periods.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2503 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/notifications.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    15330 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/permissions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4195 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/plugins.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4319 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/project_analyses.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2775 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/project_badges.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2031 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/project_branches.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1072 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/project_dump.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1314 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/project_links.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1111 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/project_pull_requests.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1194 2023-05-26 06:25:25.000000 python-sonarqube-api-2.0.0/sonarqube/rest/project_tags.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     6779 2023-05-26 06:25:25.000000 python-sonarqube-api-2.0.0/sonarqube/rest/projects.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     9227 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/qualitygates.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    12092 2023-05-26 06:25:25.000000 python-sonarqube-api-2.0.0/sonarqube/rest/qualityprofiles.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    11675 2023-05-26 06:25:25.000000 python-sonarqube-api-2.0.0/sonarqube/rest/rules.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      623 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/server.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2216 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/settings.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2262 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/sources.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     5528 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/system.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4921 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/user_groups.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2018 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/user_tokens.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     5991 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/users.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    12507 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/views.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3510 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/webhooks.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1258 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/webservices.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 07:25:57.079017 python-sonarqube-api-2.0.0/sonarqube/utils/
--rw-r--r--   0 shijialiang   (501) staff       (20)       69 2022-05-23 11:32:43.000000 python-sonarqube-api-2.0.0/sonarqube/utils/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3631 2023-05-17 05:22:16.000000 python-sonarqube-api-2.0.0/sonarqube/utils/common.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    17751 2023-05-26 04:55:45.000000 python-sonarqube-api-2.0.0/sonarqube/utils/config.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      401 2022-05-23 11:32:43.000000 python-sonarqube-api-2.0.0/sonarqube/utils/exceptions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4841 2022-05-23 11:32:43.000000 python-sonarqube-api-2.0.0/sonarqube/utils/rest_client.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 14:53:49.003585 python-sonarqube-api-2.0.1/
+-rw-r--r--   0 shijialiang   (501) staff       (20)    34523 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/LICENSE
+-rw-r--r--   0 shijialiang   (501) staff       (20)       33 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/MANIFEST.in
+-rw-r--r--   0 shijialiang   (501) staff       (20)     6065 2023-05-26 14:53:49.003365 python-sonarqube-api-2.0.1/PKG-INFO
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4946 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/README.rst
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 14:53:48.981671 python-sonarqube-api-2.0.1/python_sonarqube_api.egg-info/
+-rw-r--r--   0 shijialiang   (501) staff       (20)     6065 2023-05-26 14:53:48.000000 python-sonarqube-api-2.0.1/python_sonarqube_api.egg-info/PKG-INFO
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1200 2023-05-26 14:53:48.000000 python-sonarqube-api-2.0.1/python_sonarqube_api.egg-info/SOURCES.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)        1 2023-05-26 14:53:48.000000 python-sonarqube-api-2.0.1/python_sonarqube_api.egg-info/dependency_links.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)        9 2023-05-26 14:53:48.000000 python-sonarqube-api-2.0.1/python_sonarqube_api.egg-info/requires.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)       10 2023-05-26 14:53:48.000000 python-sonarqube-api-2.0.1/python_sonarqube_api.egg-info/top_level.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)        9 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/requirements.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)       38 2023-05-26 14:53:49.003692 python-sonarqube-api-2.0.1/setup.cfg
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2497 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/setup.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 14:53:48.982179 python-sonarqube-api-2.0.1/sonarqube/
+-rw-r--r--   0 shijialiang   (501) staff       (20)      192 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/__init__.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 14:53:48.999445 python-sonarqube-api-2.0.1/sonarqube/rest/
+-rw-r--r--   0 shijialiang   (501) staff       (20)     6785 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/__init__.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      988 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/audit_logs.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      622 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/auth.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3668 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/ce.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      814 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/duplications.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      742 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/editions.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      786 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/favorites.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     8130 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/issues.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      723 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/languages.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1272 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/measures.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      947 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/metrics.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      890 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/monitoring.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1917 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/project_analyses.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1250 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/project_badges.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      725 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/project_branches.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1072 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/project_dump.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      849 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/project_tags.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2159 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/projects.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     5352 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/qualitygates.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3115 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/qualityprofiles.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     8700 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/rules.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      623 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/server.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1528 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/settings.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3264 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/user_groups.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2018 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/user_tokens.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1034 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/users.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1627 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/views.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 14:53:49.003049 python-sonarqube-api-2.0.1/sonarqube/utils/
+-rw-r--r--   0 shijialiang   (501) staff       (20)       69 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/utils/__init__.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3631 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/utils/common.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3356 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/utils/config.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      401 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/utils/exceptions.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4841 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/utils/rest_client.py
```

### Comparing `python-sonarqube-api-2.0.0/LICENSE` & `python-sonarqube-api-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.0/PKG-INFO` & `python-sonarqube-api-2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sonarqube-api
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python wrapper for the SonarQube and SonarCloud API.
 Home-page: https://github.com/shijl0925/python-sonarqube-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: AGPL
 Keywords: api sonarqube sonar client wrapper sonarcloud
 Classifier: Development Status :: 5 - Production/Stable
@@ -50,26 +50,26 @@
 
 Editions
 ========
 
 There are two editions of python-sonarqube-api:
 
  * Community Edition (CE) is available freely under the GNU Affero General Public License v3.0.
- * Professional Edition (PE) includes [extra features](https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference)
+ * Professional Edition (PE) includes `extra features <https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference>`_
    that are more useful for developers with more than 130 interface functions. To use PE and get timely Email support and continuous updates,
    please become a Purchaser(https://shijl0925.gumroad.com/l/nlokc) and become a subscriber(https://shijl0925.gumroad.com/subscribe).
 
 +---------------------+---------------------+-----------------------+
 | Differences         | Community Edition   | Professional Edition  |
 +=====================+=====================+=======================+
 | License             | GNU AGPLv3 License  | MIT License           |
 +---------------------+---------------------+-----------------------+
 | Commercial Use      | No                  | Yes                   |
 +---------------------+---------------------+-----------------------+
-| Functions           | 30                  | more than 130         |
+| Functions           | 60                  | more than 280         |
 | (REST APIs)         |                     |                       |
 +---------------------+---------------------+-----------------------+
 | Compatibility       | 7.9.x - 8.9.x       | 7.9.x - 10.x          |
 | (SonarQube Versions)|                     |                       |
 +---------------------+---------------------+-----------------------+
 
 Installation
@@ -138,8 +138,8 @@
 
 The example documentation for SonarQubeClient APIs is available on `API examples
 <https://python-sonarqube-pro-api.readthedocs.io/en/latest/examples.html>`_.
 
 
 Licensing
 -----------
-See the [LICENSE](LICENSE) file for licensing information as it pertains to files in this repository.
+See the `LICENSE <https://github.com/shijl0925/python-sonarqube-api/blob/master/LICENSE>`_ file for licensing information as it pertains to files in this repository.
```

### Comparing `python-sonarqube-api-2.0.0/README.rst` & `python-sonarqube-api-2.0.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -23,26 +23,26 @@
 
 Editions
 ========
 
 There are two editions of python-sonarqube-api:
 
  * Community Edition (CE) is available freely under the GNU Affero General Public License v3.0.
- * Professional Edition (PE) includes [extra features](https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference)
+ * Professional Edition (PE) includes `extra features <https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference>`_
    that are more useful for developers with more than 130 interface functions. To use PE and get timely Email support and continuous updates,
    please become a Purchaser(https://shijl0925.gumroad.com/l/nlokc) and become a subscriber(https://shijl0925.gumroad.com/subscribe).
 
 +---------------------+---------------------+-----------------------+
 | Differences         | Community Edition   | Professional Edition  |
 +=====================+=====================+=======================+
 | License             | GNU AGPLv3 License  | MIT License           |
 +---------------------+---------------------+-----------------------+
 | Commercial Use      | No                  | Yes                   |
 +---------------------+---------------------+-----------------------+
-| Functions           | 30                  | more than 130         |
+| Functions           | 60                  | more than 280         |
 | (REST APIs)         |                     |                       |
 +---------------------+---------------------+-----------------------+
 | Compatibility       | 7.9.x - 8.9.x       | 7.9.x - 10.x          |
 | (SonarQube Versions)|                     |                       |
 +---------------------+---------------------+-----------------------+
 
 Installation
@@ -111,8 +111,8 @@
 
 The example documentation for SonarQubeClient APIs is available on `API examples
 <https://python-sonarqube-pro-api.readthedocs.io/en/latest/examples.html>`_.
 
 
 Licensing
 -----------
-See the [LICENSE](LICENSE) file for licensing information as it pertains to files in this repository.
+See the `LICENSE <https://github.com/shijl0925/python-sonarqube-api/blob/master/LICENSE>`_ file for licensing information as it pertains to files in this repository.
```

### Comparing `python-sonarqube-api-2.0.0/python_sonarqube_api.egg-info/PKG-INFO` & `python-sonarqube-api-2.0.1/python_sonarqube_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sonarqube-api
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python wrapper for the SonarQube and SonarCloud API.
 Home-page: https://github.com/shijl0925/python-sonarqube-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: AGPL
 Keywords: api sonarqube sonar client wrapper sonarcloud
 Classifier: Development Status :: 5 - Production/Stable
@@ -50,26 +50,26 @@
 
 Editions
 ========
 
 There are two editions of python-sonarqube-api:
 
  * Community Edition (CE) is available freely under the GNU Affero General Public License v3.0.
- * Professional Edition (PE) includes [extra features](https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference)
+ * Professional Edition (PE) includes `extra features <https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference>`_
    that are more useful for developers with more than 130 interface functions. To use PE and get timely Email support and continuous updates,
    please become a Purchaser(https://shijl0925.gumroad.com/l/nlokc) and become a subscriber(https://shijl0925.gumroad.com/subscribe).
 
 +---------------------+---------------------+-----------------------+
 | Differences         | Community Edition   | Professional Edition  |
 +=====================+=====================+=======================+
 | License             | GNU AGPLv3 License  | MIT License           |
 +---------------------+---------------------+-----------------------+
 | Commercial Use      | No                  | Yes                   |
 +---------------------+---------------------+-----------------------+
-| Functions           | 30                  | more than 130         |
+| Functions           | 60                  | more than 280         |
 | (REST APIs)         |                     |                       |
 +---------------------+---------------------+-----------------------+
 | Compatibility       | 7.9.x - 8.9.x       | 7.9.x - 10.x          |
 | (SonarQube Versions)|                     |                       |
 +---------------------+---------------------+-----------------------+
 
 Installation
@@ -138,8 +138,8 @@
 
 The example documentation for SonarQubeClient APIs is available on `API examples
 <https://python-sonarqube-pro-api.readthedocs.io/en/latest/examples.html>`_.
 
 
 Licensing
 -----------
-See the [LICENSE](LICENSE) file for licensing information as it pertains to files in this repository.
+See the `LICENSE <https://github.com/shijl0925/python-sonarqube-api/blob/master/LICENSE>`_ file for licensing information as it pertains to files in this repository.
```

### Comparing `python-sonarqube-api-2.0.0/setup.py` & `python-sonarqube-api-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/__init__.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,51 +7,35 @@
 
 from sonarqube.utils.common import strip_trailing_slash
 from sonarqube.rest.users import SonarQubeUsers
 from sonarqube.rest.projects import SonarQubeProjects
 from sonarqube.rest.user_groups import SonarQubeUserGroups
 from sonarqube.rest.issues import SonarQubeIssues
 from sonarqube.rest.measures import SonarQubeMeasures
-from sonarqube.rest.notifications import SonarQubeNotifications
-from sonarqube.rest.project_links import SonarQubeProjectLinks
-from sonarqube.rest.permissions import SonarQubePermissions
 from sonarqube.rest.ce import SonarQubeCe
 from sonarqube.rest.project_branches import SonarQubeProjectBranches
 from sonarqube.rest.qualitygates import SonarQubeQualityGates
-from sonarqube.rest.components import SonarQubeComponents
 from sonarqube.rest.rules import SonarQubeRules
 from sonarqube.rest.qualityprofiles import SonarQubeQualityProfiles
 from sonarqube.rest.duplications import SonarQubeDuplications
 from sonarqube.rest.metrics import SonarQubeMetrics
-from sonarqube.rest.hotspots import SonarQubeHotspots
-from sonarqube.rest.new_code_periods import SonarQubeNewcodeperiods
 from sonarqube.rest.settings import SonarQubeSettings
-from sonarqube.rest.sources import SonarQubeSources
 from sonarqube.rest.auth import SonarQubeAuth
 from sonarqube.rest.favorites import SonarQubeFavorites
 from sonarqube.rest.languages import SonarQubeLanguages
-from sonarqube.rest.plugins import SonarQubePlugins
 from sonarqube.rest.project_badges import SonarQubeProjectBadges
 from sonarqube.rest.project_tags import SonarQubeProjectTags
 from sonarqube.rest.project_analyses import SonarQubeProjectAnalyses
 from sonarqube.rest.server import SonarQubeServer
 from sonarqube.rest.user_tokens import SonarQubeUserTokens
-from sonarqube.rest.webhooks import SonarQubeWebhooks
-from sonarqube.rest.webservices import SonarQubeWebservices
-from sonarqube.rest.system import SonarQubeSystem
-from sonarqube.rest.alm_integrations import SonarQubeAlmIntegrations
-from sonarqube.rest.alm_settings import SonarQubeAlmSettings
-from sonarqube.rest.analysis_cache import SonarQubeAnalysisCache
 from sonarqube.rest.monitoring import SonarQubeMonitoring
 from sonarqube.rest.project_dump import SonarQubeProjectDump
-from sonarqube.rest.applications import SonarQubeApplications
 from sonarqube.rest.audit_logs import SonarQubeAuditLogs
 from sonarqube.rest.editions import SonarQubeEditions
 from sonarqube.rest.views import SonarQubeViews
-from sonarqube.rest.project_pull_requests import SonarQubeProjectPullRequests
 
 
 class SonarQubeClient:
     """
     A Python Client for SonarQube Server APIs.
     """
 
@@ -130,41 +114,14 @@
         SonarQube issues Operations
 
         :return:
         """
         return SonarQubeIssues(api=self)
 
     @property
-    def notifications(self):
-        """
-        SonarQube notifications Operations
-
-        :return:
-        """
-        return SonarQubeNotifications(api=self)
-
-    @property
-    def project_links(self):
-        """
-        SonarQube project links Operations
-
-        :return:
-        """
-        return SonarQubeProjectLinks(api=self)
-
-    @property
-    def permissions(self):
-        """
-        SonarQube permissions Operations
-
-        :return:
-        """
-        return SonarQubePermissions(api=self)
-
-    @property
     def ce(self):
         """
         SonarQube ce Operations
 
         :return:
         """
         return SonarQubeCe(api=self)
@@ -184,23 +141,14 @@
         SonarQube quality gates Operations
 
         :return:
         """
         return SonarQubeQualityGates(api=self)
 
     @property
-    def components(self):
-        """
-        SonarQube components Operations
-
-        :return:
-        """
-        return SonarQubeComponents(api=self)
-
-    @property
     def rules(self):
         """
         SonarQube rules Operations
 
         :return:
         """
         return SonarQubeRules(api=self)
@@ -229,50 +177,23 @@
         SonarQube metrics Operations
 
         :return:
         """
         return SonarQubeMetrics(api=self)
 
     @property
-    def hotspots(self):
-        """
-        Security Hotspots
-
-        :return:
-        """
-        return SonarQubeHotspots(api=self)
-
-    @property
-    def new_code_periods(self):
-        """
-        SonarQube new code periods Operations
-
-        :return:
-        """
-        return SonarQubeNewcodeperiods(api=self)
-
-    @property
     def settings(self):
         """
         SonarQube settings Operations
 
         :return:
         """
         return SonarQubeSettings(api=self)
 
     @property
-    def sources(self):
-        """
-        SonarQube sources Operations
-
-        :return:
-        """
-        return SonarQubeSources(api=self)
-
-    @property
     def auth(self):
         """
         SonarQube authentication Operations
 
         :return:
         """
         return SonarQubeAuth(api=self)
@@ -337,96 +258,27 @@
         SonarQube user tokens Operations
 
         :return:
         """
         return SonarQubeUserTokens(api=self)
 
     @property
-    def webhooks(self):
-        """
-        SonarQube webhooks Operations
-
-        :return:
-        """
-        return SonarQubeWebhooks(api=self)
-
-    @property
-    def webservices(self):
-        """
-        SonarQube webservices Operations
-
-        :return:
-        """
-        return SonarQubeWebservices(api=self)
-
-    @property
-    def system(self):
-        """
-        SonarQube system Operations
-
-        :return:
-        """
-        return SonarQubeSystem(api=self)
-
-    @property
-    def plugins(self):
-        """
-        SonarQube plugins Operations
-
-        :return:
-        """
-        return SonarQubePlugins(api=self)
-
-    @property
-    def alm_integrations(self):
-        """
-        ALM Integrations
-
-        """
-        return SonarQubeAlmIntegrations(api=self)
-
-    @property
-    def alm_settings(self):
-        """
-        ALM settings
-
-        """
-        return SonarQubeAlmSettings(api=self)
-
-    @property
-    def analysis_cache(self):
-        """
-        Analysis cache
-
-        """
-        return SonarQubeAnalysisCache(api=self)
-
-    @property
     def monitoring(self):
         return SonarQubeMonitoring(api=self)
 
     @property
     def project_dump(self):
         """
         Project export/import
 
         :return:
         """
         return SonarQubeProjectDump(api=self)
 
     @property
-    def applications(self):
-        """
-        SonarQube applications Operations
-
-        :return:
-        """
-        return SonarQubeApplications(api=self)
-
-    @property
     def audit_logs(self):
         """
         Manage Audit logs
 
         """
         return SonarQubeAuditLogs(api=self)
 
@@ -435,23 +287,14 @@
         """
         Manage SonarSource commercial editions
 
         """
         return SonarQubeEditions(api=self)
 
     @property
-    def project_pull_requests(self):
-        """
-        SonarQube project pull requests Operations
-
-        :return:
-        """
-        return SonarQubeProjectPullRequests(api=self)
-
-    @property
     def views(self):
         """
         Manage Portfolios
 
         """
         return SonarQubeViews(api=self)
```

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/analysis_cache.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/languages.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-from sonarqube.utils.common import GET
 from sonarqube.utils.rest_client import RestClient
-
-from sonarqube.utils.config import (
-    API_ANALYSIS_CACHE,
-)
+from sonarqube.utils.config import API_LANGUAGES_LIST_ENDPOINT
+from sonarqube.utils.common import GET
 
 
-class SonarQubeAnalysisCache(RestClient):
+class SonarQubeLanguages(RestClient):
+    """
+    SonarQube languages Operations
+    """
 
     def __init__(self, **kwargs):
         """
 
         :param kwargs:
         """
-        super(SonarQubeAnalysisCache, self).__init__(**kwargs)
+        super(SonarQubeLanguages, self).__init__(**kwargs)
 
-    @GET(API_ANALYSIS_CACHE)
-    def get_analysis_cache(self, project, branch=None):
+    @GET(API_LANGUAGES_LIST_ENDPOINT)
+    def get_supported_programming_languages(self, q=None):
         """
-        since 9.4
-        Get the scanner's cached data for a branch. Requires scan permission on the project.
-        Data is returned gzipped if the corresponding 'Accept-Encoding' header is set in the request.
+        SINCE 5.1
+        List supported programming languages
 
-        :param project: Project key
-        :param branch: Branch key. If not provided, main branch will be used.
+        :param q: A pattern to match language keys/names against
         :return:
-        """
+        """
```

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/audit_logs.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/audit_logs.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/auth.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/auth.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
-    API_AUTH_LOGIN_ENDPOINT,
-    API_AUTH_LOGOUT_ENDPOINT,
     API_AUTH_VALIDATE_ENDPOINT,
 )
 from sonarqube.utils.common import GET, POST
 
 
 class SonarQubeAuth(RestClient):
     """
@@ -18,34 +16,14 @@
     def __init__(self, **kwargs):
         """
 
         :param kwargs:
         """
         super(SonarQubeAuth, self).__init__(**kwargs)
 
-    @POST(API_AUTH_LOGIN_ENDPOINT)
-    def authenticate_user(self, login, password):
-        """
-        SINCE 6.0
-        Authenticate a user.
-
-        :param login: Login of the user
-        :param password: Password of the user
-        :return:
-        """
-
-    @POST(API_AUTH_LOGOUT_ENDPOINT)
-    def logout_user(self):
-        """
-        SINCE 6.3
-        Logout a user.
-
-        :return:
-        """
-
     @GET(API_AUTH_VALIDATE_ENDPOINT)
     def check_credentials(self):
         """
         SINCE 3.3
         Check credentials.
 
         :return:
```

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/ce.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/ce.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/duplications.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/duplications.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/editions.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/editions.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/languages.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/metrics.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,43 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from sonarqube.utils.rest_client import RestClient
-from sonarqube.utils.config import API_LANGUAGES_LIST_ENDPOINT
+from sonarqube.utils.config import (
+    API_METRICS_SEARCH_ENDPOINT,
+    API_METRICS_TYPES_ENDPOINT,
+)
 from sonarqube.utils.common import GET
 
 
-class SonarQubeLanguages(RestClient):
+class SonarQubeMetrics(RestClient):
     """
-    SonarQube languages Operations
+    SonarQube metrics Operations
     """
 
     def __init__(self, **kwargs):
         """
 
         :param kwargs:
         """
-        super(SonarQubeLanguages, self).__init__(**kwargs)
+        super(SonarQubeMetrics, self).__init__(**kwargs)
 
-    @GET(API_LANGUAGES_LIST_ENDPOINT)
-    def get_supported_programming_languages(self, q=None):
+    @GET(API_METRICS_SEARCH_ENDPOINT)
+    def search_metrics(self, p=None, ps=None):
         """
-        SINCE 5.1
-        List supported programming languages
+        SINCE 5.2
+        Search for metrics
+
+        :param p: page number.
+        :param ps: Page size. Must be greater than 0 and less or equal than 500
+
+        :return:
+        """
+
+    @GET(API_METRICS_TYPES_ENDPOINT)
+    def get_metrics_types(self):
+        """
+        SINCE 5.2
+        List all available metric types.
 
-        :param q: A pattern to match language keys/names against
         :return:
         """
```

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/metrics.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/users.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
-    API_METRICS_SEARCH_ENDPOINT,
-    API_METRICS_TYPES_ENDPOINT,
+    API_USERS_SEARCH_ENDPOINT,
 )
-from sonarqube.utils.common import GET
+from sonarqube.utils.common import GET, POST
 
 
-class SonarQubeMetrics(RestClient):
+class SonarQubeUsers(RestClient):
     """
-    SonarQube metrics Operations
+    SonarQube users Operations
     """
 
+    MAX_SEARCH_NUM = 200
+
     def __init__(self, **kwargs):
         """
 
         :param kwargs:
         """
-        super(SonarQubeMetrics, self).__init__(**kwargs)
-
-    @GET(API_METRICS_SEARCH_ENDPOINT)
-    def search_metrics(self, p=None, ps=None):
-        """
-        SINCE 5.2
-        Search for metrics
+        super(SonarQubeUsers, self).__init__(**kwargs)
 
-        :param p: page number.
-        :param ps: Page size. Must be greater than 0 and less or equal than 500
+    def get(self, login):
+        result = self.search_users(q=login)
+        users = result.get("users", [])
 
-        :return:
-        """
+        for user in users:
+            if user["login"] == login:
+                return user
 
-    @GET(API_METRICS_TYPES_ENDPOINT)
-    def get_metrics_types(self):
+    @GET(API_USERS_SEARCH_ENDPOINT)
+    def search_users(self, q=None, p=None, ps=None):
         """
-        SINCE 5.2
-        List all available metric types.
+        SINCE 3.6
+        Get a list of active users.
 
+        :param q: Filter on login, name and email
+        :param p: page number.
+        :param ps: Page size. Must be greater than 0 and less or equal than 500
         :return:
-        """
+        """
```

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/monitoring.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/monitoring.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/new_code_periods.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/project_analyses.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,60 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
-    API_NEW_CODE_PERIODS_LIST_ENDPOINT,
-    API_NEW_CODE_PERIODS_SET_ENDPOINT,
-    API_NEW_CODE_PERIODS_SHOW_ENDPOINT,
-    API_NEW_CODE_PERIODS_UNSET_ENDPOINT,
+    API_PROJECT_ANALYSES_DELETE_ENDPOINT,
+    API_PROJECT_ANALYSES_SEARCH_ENDPOINT,
 )
 from sonarqube.utils.common import GET, POST
 
 
-class SonarQubeNewcodeperiods(RestClient):
+class SonarQubeProjectAnalyses(RestClient):
     """
-    SonarQube new code periods Operations
+    SonarQube project analyses Operations
     """
 
+    special_attributes_map = {"from_date": "from", "to_date": "to"}
+
     def __init__(self, **kwargs):
         """
 
         :param kwargs:
         """
-        super(SonarQubeNewcodeperiods, self).__init__(**kwargs)
-
-    @GET(API_NEW_CODE_PERIODS_LIST_ENDPOINT)
-    def list(self, project):
-        """
-        SINCE 8.0
-        List the New Code Periods for all branches in a project.
+        super(SonarQubeProjectAnalyses, self).__init__(**kwargs)
 
-        :param project: Project key
-        :return:
+    @POST(API_PROJECT_ANALYSES_DELETE_ENDPOINT)
+    def delete_project_analysis(self, analysis):
         """
+        SINCE 6.3
+        Delete a project analysis.
 
-    @POST(API_NEW_CODE_PERIODS_SET_ENDPOINT)
-    def set(self, type, project=None, branch=None, value=None):
-        """
-        SINCE 8.0
-        Updates the setting for the New Code Period on different levels:
-          * Project key must be provided to update the value for a project
-          * Both project and branch keys must be provided to update the value for a branch
-
-        :param type: Type
-          New code periods of the following types are allowed:
-          * SPECIFIC_ANALYSIS - can be set at branch level only
-          * PREVIOUS_VERSION - can be set at any level (global, project, branch)
-          * NUMBER_OF_DAYS - can be set at any level (global, project, branch)
-          * REFERENCE_BRANCH - can only be set for projects and branches
-        :param project: Project key
-        :param branch: Branch key
-        :param value: Value
-          For each type, a different value is expected:
-          * the uuid of an analysis, when type is SPECIFIC_ANALYSIS
-          * no value, when type is PREVIOUS_VERSION
-          * a number, when type is NUMBER_OF_DAYS
-          * a string, when type is REFERENCE_BRANCH
-        :return:
-        """
-
-    @GET(API_NEW_CODE_PERIODS_SHOW_ENDPOINT)
-    def show(self, project=None, branch=None):
-        """
-        SINCE 8.0
-        Shows a setting for the New Code Period.
-
-        :param project: Project key
-        :param branch: Branch key
+        :param analysis: Analysis key
         :return:
         """
 
-    @POST(API_NEW_CODE_PERIODS_UNSET_ENDPOINT)
-    def unset(self, project=None, branch=None):
+    @GET(API_PROJECT_ANALYSES_SEARCH_ENDPOINT)
+    def search_project_analyses_and_events(
+        self, project, branch=None, category=None, from_date=None, to_date=None, p=None, ps=None
+    ):
         """
-        SINCE 8.0
-        Unset the New Code Period setting for a branch, project or global.
+        SINCE 6.3
+        Search a project analyses and attached events.
 
         :param project: Project key
         :param branch: Branch key
+        :param category: Event category. Filter analyses that have at least one event of the category specified.
+          Possible values are for:
+            * VERSION
+            * OTHER
+            * QUALITY_PROFILE
+            * QUALITY_GATE
+            * DEFINITION_CHANGE
+        :param from_date: Filter analyses created after the given date (inclusive).
+          Either a date (server timezone) or datetime can be provided
+        :param to_date: Filter analyses created before the given date (inclusive).
+          Either a date (server timezone) or datetime can be provided
+        :param p: page number.
+        :param ps: Page size. Must be greater than 0 and less or equal than 500
         :return:
         """
```

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/project_badges.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/qualityprofiles.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,90 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
-    API_PROJECT_BADGES_MEASURE_ENDPOINT,
-    API_PROJECT_BADGES_QUALITY_GATE_ENDPOINT,
-    API_PROJECT_BADGES_RENEW_TOKEN_ENDPOINT,
-    API_PROJECT_BADGES_TOKEN_ENDPOINT
+    API_QUALITYPROFILES_ACTIVATE_RULE_ENDPOINT,
+    API_QUALITYPROFILES_SEARCH_ENDPOINT,
+    API_QUALITYPROFILES_DELETE_ENDPOINT,
 )
 from sonarqube.utils.common import GET, POST
 
 
-class SonarQubeProjectBadges(RestClient):
+class SonarQubeQualityProfiles(RestClient):
     """
-    SonarQube project badges Operations
+    SonarQube quality profiles Operations
     """
 
     def __init__(self, **kwargs):
         """
 
         :param kwargs:
         """
-        super(SonarQubeProjectBadges, self).__init__(**kwargs)
+        super(SonarQubeQualityProfiles, self).__init__(**kwargs)
 
-    @GET(API_PROJECT_BADGES_MEASURE_ENDPOINT)
-    def generate_badge_for_project_measures(self, project, metric, branch=None, token=None):
-        """
-        SINCE 7.1
-        Generate badge for project's measure as an SVG.
-
-        :param project: Project or application key
-        :param branch: Long living branch key
-        :param metric: Metric key,
+    def activate_rule_for_quality_profile(
+        self, key, rule, reset=False, severity=None, **params
+    ):
+        """
+        SINCE 4.4
+        Activate a rule for a given quality profile.
+
+        :param key: Quality Profile key.
+        :param rule: Rule key
+        :param reset: Reset severity and parameters of activated rule.
+          Set the values defined on parent profile or from rule default values.
+        :param severity: Severity. Ignored if parameter reset is true.
           Possible values are for:
-            * bugs
-            * code_smells
-            * coverage
-            * duplicated_lines_density
-            * ncloc
-            * sqale_rating
-            * alert_status
-            * reliability_rating
-            * security_rating
-            * sqale_index
-            * vulnerabilities
-        :param token: Security token
-        :return:
-        """
-
-    @GET(API_PROJECT_BADGES_QUALITY_GATE_ENDPOINT)
-    def generate_badge_for_project_quality_gate(self, project, branch=None, token=None):
-        """
-        SINCE 7.1
-        Generate badge for project's quality gate as an SVG.
-
-        :param project: Project or application key
-        :param branch: Long living branch key
-        :param token: Security token
+            * INFO
+            * MINOR
+            * MAJOR
+            * CRITICAL
+            * BLOCKER
+        :param params: customized parameters for the rule.Ignored if parameter reset is true.
         :return:
         """
+        data = {"rule": rule, "key": key, "reset": reset and "true" or "false"}
 
-    @POST(API_PROJECT_BADGES_RENEW_TOKEN_ENDPOINT)
-    def generate_new_token_for_project_badge_access(self, project):
-        """
-        SINCE 9.2
-        Creates new token replacing any existing token for project badge access for private projects.
-        This token can be used to authenticate with api/project_badges/quality_gate and api/project_badges/measure endpoints.
-        Requires 'Administer' permission on the specified project.
-
+        if not reset:
+            # No reset, Add severity if given (if not default will be used?)
+            if severity:
+                data["severity"] = severity.upper()
+
+            # Add params if we have any
+            # Note: sort by key to allow checking easily
+            params = ";".join(
+                "{}={}".format(k, v) for k, v in sorted(params.items()) if v
+            )
+            if params:
+                data["params"] = params
+
+        return self._post(API_QUALITYPROFILES_ACTIVATE_RULE_ENDPOINT, data=data)
+
+    @GET(API_QUALITYPROFILES_SEARCH_ENDPOINT)
+    def search_quality_profiles(
+        self, organization=None, defaults="false", language=None, project=None, qualityProfile=None
+    ):
+        """
+        SINCE 5.2
+        Search quality profiles
+
+        :param organization: organization key.
+        :param defaults: If set to true, return only the quality profiles marked as default for each language.
+          Possible values are for: true or false. default value is false.
+        :param language: Language key. If provided, only profiles for the given language are returned.
         :param project: Project key
+        :param qualityProfile: Quality profile name
         :return:
         """
-
-    @GET(API_PROJECT_BADGES_TOKEN_ENDPOINT)
-    def retrieve_token_for_project_badge_access(self, project):
+    @POST(API_QUALITYPROFILES_DELETE_ENDPOINT)
+    def delete_quality_profile(self, language, qualityProfile, organization=None):
         """
-        SINCE 9.2
-        Retrieve a token to use for project badge access for private projects.
-        This token can be used to authenticate with api/project_badges/quality_gate and api/project_badges/measure endpoints.
-        Requires 'Browse' permission on the specified project.
-
-        :param project: Project or application key
+        SINCE 5.2
+        Delete a quality profile and all its descendants.
+        The default quality profile cannot be deleted.
+
+        :param language: Quality profile language.
+        :param qualityProfile: Quality profile name.
+        :param organization: Organization key.
         :return:
-        """
+        """
```

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/project_dump.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/project_dump.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/project_links.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/project_branches.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,31 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
-    API_PROJECT_LINKS_CREATE_ENDPOINT,
-    API_PROJECT_LINKS_DELETE_ENDPOINT,
-    API_PROJECT_LINKS_SEARCH_ENDPOINT,
+    API_PROJECT_BRANCHES_LIST_ENDPOINT,
 )
 from sonarqube.utils.common import GET, POST
 
 
-class SonarQubeProjectLinks(RestClient):
+class SonarQubeProjectBranches(RestClient):
     """
-    SonarQube project links Operations
+    SonarQube project branches Operations
     """
 
     def __init__(self, **kwargs):
         """
 
         :param kwargs:
         """
-        super(SonarQubeProjectLinks, self).__init__(**kwargs)
+        super(SonarQubeProjectBranches, self).__init__(**kwargs)
 
-    @POST(API_PROJECT_LINKS_CREATE_ENDPOINT)
-    def create_project_link(self, projectKey, name, url):
+    @GET(API_PROJECT_BRANCHES_LIST_ENDPOINT)
+    def search_project_branches(self, project):
         """
-        SINCE 6.1
-        Create a new project link.
+        SINCE 6.6
+        List the branches of a project.
 
-        :param projectKey: Project key
-        :param name: Link name
-        :param url: Link url
-        :return: request response
-        """
-
-    @POST(API_PROJECT_LINKS_DELETE_ENDPOINT)
-    def delete_project_link(self, id):
-        """
-        SINCE 6.1
-        Delete existing project link.
-
-        :param id: Link id
-        :return:
-        """
-
-    @GET(API_PROJECT_LINKS_SEARCH_ENDPOINT)
-    def search_project_links(self, projectKey):
-        """
-        SINCE 6.1
-        List links of a project.
-
-        :param projectKey: Project Key
+        :param project: Project key
         :return:
-        """
+        """
```

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/project_tags.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/project_tags.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
     API_PROJECT_TAGS_SEARCH_ENDPOINT,
-    API_PROJECT_TAGS_SET_ENDPOINT,
 )
 from sonarqube.utils.common import GET, POST
 
 
 class SonarQubeProjectTags(RestClient):
     """
     SonarQube project tags Operations
@@ -27,19 +26,8 @@
         SINCE 6.4
         Search tags
 
         :param q: Limit search to tags that contain the supplied string.
         :param p: page number.
         :param ps: Page size. Must be greater than 0 and less or equal than 100
         :return:
-        """
-
-    @POST(API_PROJECT_TAGS_SET_ENDPOINT)
-    def set_project_tags(self, project, tags):
-        """
-        SINCE 6.4
-        Set tags on a project.
-
-        :param project: Project key
-        :param tags: Comma-separated list of tags.Possible values are for: finance, offshore
-        :return:
-        """
+        """
```

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/rules.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/rules.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
     API_RULES_SEARCH_ENDPOINT,
     API_RULES_CREATE_ENDPOINT,
-    API_RULES_UPDATE_ENDPOINT,
-    API_RULES_DELETE_ENDPOINT,
     API_RULES_SHOW_ENDPOINT,
-    API_RULES_TAGS_ENDPOINT,
-    API_RULES_REPOSITORIES_ENDPOINT,
 )
 from sonarqube.utils.common import GET, POST
 
 
 class SonarQubeRules(RestClient):
     """
     SonarQube rules Operations
@@ -265,103 +261,19 @@
             * VULNERABILITY
             * SECURITY_HOTSPOT
         :param params: Parameters as semi-colon list of =, for example 'params=key1=v1;key2=v2' (Only for custom rule)
 
         :return: request response
         """
 
-    @POST(API_RULES_UPDATE_ENDPOINT)
-    def update_rule(
-        self,
-        key,
-        organization=None,
-        name=None,
-        markdown_description=None,
-        markdown_note=None,
-        remediation_fn_base_effort=None,
-        remediation_fn_type=None,
-        remediation_fy_gap_multiplier=None,
-        severity=None,
-        status=None,
-        tags=None,
-        params=None
-    ):
-        """
-        SINCE 4.4
-        Update an existing rule.
-
-        :param key: Key of the rule to update
-        :param organization: organization key.
-        :param name: Rule name (mandatory for custom rule)
-        :param markdown_description: Rule description (mandatory for custom rule and manual rule)
-        :param markdown_note: Optional note in markdown format. Use empty value to remove current note.
-          Note is not changed if the parameter is not set.
-        :param params: Parameters as semi-colon list of =, for example 'params=key1=v1;key2=v2'
-          (Only when updating a custom rule)
-        :param remediation_fn_base_effort: Base effort of the remediation function of the rule
-        :param remediation_fn_type: Type of the remediation function of the rule
-        :param remediation_fy_gap_multiplier: Gap multiplier of the remediation function of the rule
-        :param severity: Rule severity (Only when updating a custom rule).Possible values are for:
-
-          * INFO
-          * MINOR
-          * MAJOR
-          * CRITICAL
-          * BLOCKER
-
-        :param status: Rule status (Only when updating a custom rule). Possible values are for:
-
-          * BETA
-          * DEPRECATED
-          * READY
-          * REMOVED
-
-        :param tags: Optional comma-separated list of tags to set. Use blank value to remove current tags.
-          Tags are not changed if the parameter is not set.
-
-        :return: request response
-        """
-
-    @POST(API_RULES_DELETE_ENDPOINT)
-    def delete_rule(self, key):
-        """
-        SINCE 4.4
-        Delete custom rule.
-        :param key:
-        :return:
-        """
-
     @GET(API_RULES_SHOW_ENDPOINT)
     def get_rule(self, key, organization=None, actives="false"):
         """
         SINCE 4.2
         Get detailed information about a rule.
 
         :param key: Rule key
         :param organization: organization key.
         :param actives: Show rule's activations for all profiles ("active rules").
           Possible values are for: true or false. default value is false.
         :return:
-        """
-
-    @GET(API_RULES_REPOSITORIES_ENDPOINT)
-    def get_rule_repositories(self, language=None, q=None):
-        """
-        SINCE 4.5
-        List available rule repositories
-
-        :param language: A language key; if provided, only repositories for the given language will be returned
-        :param q: A pattern to match repository keys/names against
-        :return:
-        """
-
-    @GET(API_RULES_TAGS_ENDPOINT)
-    def get_rule_tags(self, organization=None, ps=10, q=None):
-        """
-        SINCE 4.4
-        List rule tags
-
-        :param organization: organization key.
-        :param ps: Page size. Must be greater than 0 and less or equal than 100.default value is 10.
-        :param q: Limit search to tags that contain the supplied string.
-        :return:
-        """
+        """
```

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/server.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/server.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/settings.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
     API_SETTINGS_SET_ENDPOINT,
-    API_SETTINGS_RESET_ENDPOINT,
     API_SETTINGS_VALUES_ENDPOINT,
-    API_SETTINGS_LIST_DEFINITIONS_ENDPOINT,
 )
 from sonarqube.utils.common import GET, POST
 
 
 class SonarQubeSettings(RestClient):
     """
     SonarQube settings Operations
@@ -34,41 +32,19 @@
         :param value: Setting value. To reset a value, please use the reset web service.
         :param component: Component key
         :param fieldValues: Setting field values. To set several values, the parameter must be called once for
           each value.
         :return:
         """
 
-    @POST(API_SETTINGS_RESET_ENDPOINT)
-    def remove_setting_value(self, keys, component=None):
-        """
-        SINCE 6.1
-        Remove a setting value.
-        The settings defined in conf/sonar.properties are read-only and can't be changed.
-
-        :param keys: Comma-separated list of keys
-        :param component: Component key
-        :return:
-        """
-
     @GET(API_SETTINGS_VALUES_ENDPOINT)
     def get_settings_values(self, component=None, keys=None):
         """
         SINCE 6.3
         List settings values.
         If no value has been set for a setting, then the default value is returned.
         The settings from conf/sonar.properties are excluded from results.
 
         :param component: Component key
         :param keys: List of setting keys
         :return:
         """
-
-    @GET(API_SETTINGS_LIST_DEFINITIONS_ENDPOINT)
-    def get_settings_definitions(self, component=None):
-        """
-        SINCE 6.3
-        List settings definitions.
-
-        :param component: Component key
-        :return:
-        """
```

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/user_groups.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/user_groups.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 # @Author: Jialiang Shi
 from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
     API_USER_GROUPS_SEARCH_ENDPOINT,
     API_USER_GROUPS_CREATE_ENDPOINT,
     API_USER_GROUPS_DELETE_ENDPOINT,
     API_USER_GROUPS_UPDATE_ENDPOINT,
-    API_USER_GROUPS_USERS_ENDPOINT,
-    API_USER_GROUPS_ADD_USER_ENDPOINT,
-    API_USER_GROUPS_REMOVE_USER_ENDPOINT,
 )
 from sonarqube.utils.common import GET, POST
 
 
 class SonarQubeUserGroups(RestClient):
     """
     SonarQube user_groups Operations
@@ -87,52 +84,8 @@
         :param currentName: Name of the group to be updated. (since 8.5)
         :param name: New optional name for the group. A group name cannot be larger than 255 characters and must
           be unique. Value 'anyone' (whatever the case) is reserved and cannot be used. If value is empty or not
           defined, then name is not changed.
         :param description: New optional description for the group. A group description cannot be larger than
           200 characters. If value is not defined, then description is not changed.
         :return:
-        """
-
-    @POST(API_USER_GROUPS_ADD_USER_ENDPOINT)
-    def add_user_to_group(self, name, login, organization=None):
-        """
-        SINCE 5.2
-        Add a user to a group.
-
-        :param name: Group name
-        :param organization: organization key.
-        :param login: User login
-        :return:
-        """
-
-    @POST(API_USER_GROUPS_REMOVE_USER_ENDPOINT)
-    def remove_user_from_group(self, name, login, organization=None):
-        """
-        SINCE 5.2
-        Remove a user from a group.
-
-        :param name: Group name
-        :param login: User login
-        :param organization: organization key.
-        :return:
-        """
-
-    @GET(API_USER_GROUPS_USERS_ENDPOINT)
-    def search_users_belong_to_group(self, name, organization=None, q=None, selected="selected", p=None, ps=None):
-        """
-        SINCE 5.2
-        Search for users with membership information with respect to a group.
-
-        :param name: Group name
-        :param organization: organization key.
-        :param q: Limit search to names or logins that contain the supplied string.
-        :param selected: Depending on the value, show only selected items (selected=selected), deselected items
-          (selected=deselected), or all items with their selection status (selected=all).Possible values are for:
-            * all
-            * deselected
-            * selected
-          default value is selected.
-        :param p: page number.
-        :param ps: Page size. Must be greater than 0 and less or equal than 500
-        :return:
-        """
+        """
```

### Comparing `python-sonarqube-api-2.0.0/sonarqube/rest/user_tokens.py` & `python-sonarqube-api-2.0.1/sonarqube/rest/user_tokens.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.0/sonarqube/utils/common.py` & `python-sonarqube-api-2.0.1/sonarqube/utils/common.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.0/sonarqube/utils/rest_client.py` & `python-sonarqube-api-2.0.1/sonarqube/utils/rest_client.py`

 * *Files identical despite different names*

