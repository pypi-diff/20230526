# Comparing `tmp/python-sonarqube-api-1.3.7.tar.gz` & `tmp/python-sonarqube-api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sonarqube-api-1.3.7.tar", last modified: Wed May 17 06:54:34 2023, max compression
+gzip compressed data, was "python-sonarqube-api-2.0.0.tar", last modified: Fri May 26 07:25:57 2023, max compression
```

## Comparing `python-sonarqube-api-1.3.7.tar` & `python-sonarqube-api-2.0.0.tar`

### file list

```diff
@@ -1,83 +1,66 @@
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-17 06:54:34.975991 python-sonarqube-api-1.3.7/
--rw-r--r--   0 shijialiang   (501) staff       (20)     1069 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/LICENSE
--rw-r--r--   0 shijialiang   (501) staff       (20)       33 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/MANIFEST.in
--rw-r--r--   0 shijialiang   (501) staff       (20)     5057 2023-05-17 06:54:34.975767 python-sonarqube-api-1.3.7/PKG-INFO
--rw-r--r--   0 shijialiang   (501) staff       (20)     3939 2023-05-17 05:23:41.000000 python-sonarqube-api-1.3.7/README.rst
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-17 06:54:34.929038 python-sonarqube-api-1.3.7/python_sonarqube_api.egg-info/
--rw-r--r--   0 shijialiang   (501) staff       (20)     5057 2023-05-17 06:54:34.000000 python-sonarqube-api-1.3.7/python_sonarqube_api.egg-info/PKG-INFO
--rw-r--r--   0 shijialiang   (501) staff       (20)     2330 2023-05-17 06:54:34.000000 python-sonarqube-api-1.3.7/python_sonarqube_api.egg-info/SOURCES.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        1 2023-05-17 06:54:34.000000 python-sonarqube-api-1.3.7/python_sonarqube_api.egg-info/dependency_links.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        9 2023-05-17 06:54:34.000000 python-sonarqube-api-1.3.7/python_sonarqube_api.egg-info/requires.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)       10 2023-05-17 06:54:34.000000 python-sonarqube-api-1.3.7/python_sonarqube_api.egg-info/top_level.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        9 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/requirements.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)       38 2023-05-17 06:54:34.976033 python-sonarqube-api-1.3.7/setup.cfg
--rw-r--r--   0 shijialiang   (501) staff       (20)     2496 2023-05-17 06:51:30.000000 python-sonarqube-api-1.3.7/setup.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-17 06:54:34.931913 python-sonarqube-api-1.3.7/sonarqube/
--rw-r--r--   0 shijialiang   (501) staff       (20)      240 2023-05-17 06:36:16.000000 python-sonarqube-api-1.3.7/sonarqube/__init__.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-17 06:54:34.946527 python-sonarqube-api-1.3.7/sonarqube/cloud/
--rw-r--r--   0 shijialiang   (501) staff       (20)     7413 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      536 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/auth.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1639 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/ce.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1289 2022-12-27 07:15:12.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/components.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     7513 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/issues.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    10994 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/permissions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1553 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/project_badges.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3369 2022-12-27 07:08:47.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/projects.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     6722 2022-12-27 07:17:05.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/qualitygates.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     7311 2022-12-27 07:12:06.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/qualityprofiles.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     9982 2022-12-27 07:14:27.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/rules.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3010 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/settings.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3657 2022-12-27 07:13:24.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/user_groups.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1870 2023-05-17 06:00:39.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/users.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1548 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/webhooks.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-17 06:54:34.970188 python-sonarqube-api-1.3.7/sonarqube/community/
--rw-r--r--   0 shijialiang   (501) staff       (20)    11056 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4082 2022-08-11 14:17:02.000000 python-sonarqube-api-1.3.7/sonarqube/community/alm_integrations.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    12791 2023-05-17 06:06:55.000000 python-sonarqube-api-1.3.7/sonarqube/community/alm_settings.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1089 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/auth.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3529 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/ce.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3908 2022-12-27 06:30:07.000000 python-sonarqube-api-1.3.7/sonarqube/community/components.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      814 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/duplications.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1504 2022-12-27 06:51:59.000000 python-sonarqube-api-1.3.7/sonarqube/community/favorites.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2614 2022-12-27 06:53:53.000000 python-sonarqube-api-1.3.7/sonarqube/community/hotspots.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    13630 2023-05-17 06:00:39.000000 python-sonarqube-api-1.3.7/sonarqube/community/issues.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      723 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/languages.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     5441 2022-12-27 06:57:44.000000 python-sonarqube-api-1.3.7/sonarqube/community/measures.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      947 2022-12-27 06:33:08.000000 python-sonarqube-api-1.3.7/sonarqube/community/metrics.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      890 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/monitoring.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2593 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/new_code_periods.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2503 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/notifications.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    14234 2022-12-27 06:43:16.000000 python-sonarqube-api-1.3.7/sonarqube/community/permissions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4195 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/plugins.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4319 2022-12-27 06:32:02.000000 python-sonarqube-api-1.3.7/sonarqube/community/project_analyses.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2677 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/project_badges.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2031 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/project_branches.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1064 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/project_dump.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1314 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/project_links.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1097 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/project_pull_requests.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1066 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/project_tags.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     6521 2023-05-17 06:03:35.000000 python-sonarqube-api-1.3.7/sonarqube/community/projects.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     9227 2022-12-27 07:04:18.000000 python-sonarqube-api-1.3.7/sonarqube/community/qualitygates.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    11215 2022-12-27 06:46:00.000000 python-sonarqube-api-1.3.7/sonarqube/community/qualityprofiles.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    11376 2023-05-17 06:01:22.000000 python-sonarqube-api-1.3.7/sonarqube/community/rules.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      623 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/server.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2216 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/settings.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2262 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/sources.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     5528 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/system.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4316 2023-05-17 06:00:39.000000 python-sonarqube-api-1.3.7/sonarqube/community/user_groups.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2018 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/user_tokens.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     5874 2023-05-17 06:00:39.000000 python-sonarqube-api-1.3.7/sonarqube/community/users.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3378 2022-12-27 07:07:40.000000 python-sonarqube-api-1.3.7/sonarqube/community/webhooks.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1258 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/webservices.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-17 06:54:34.972945 python-sonarqube-api-1.3.7/sonarqube/enterprise/
--rw-r--r--   0 shijialiang   (501) staff       (20)      954 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/enterprise/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4860 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/enterprise/applications.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      981 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/enterprise/audit_logs.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      666 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/enterprise/editions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    12235 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/enterprise/views.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-17 06:54:34.975358 python-sonarqube-api-1.3.7/sonarqube/utils/
--rw-r--r--   0 shijialiang   (501) staff       (20)       69 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/utils/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3631 2023-05-17 05:23:33.000000 python-sonarqube-api-1.3.7/sonarqube/utils/common.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    17635 2023-05-17 06:06:28.000000 python-sonarqube-api-1.3.7/sonarqube/utils/config.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      401 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/utils/exceptions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4841 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/utils/rest_client.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 07:25:57.081134 python-sonarqube-api-2.0.0/
+-rw-r--r--   0 shijialiang   (501) staff       (20)    34523 2023-05-26 04:56:09.000000 python-sonarqube-api-2.0.0/LICENSE
+-rw-r--r--   0 shijialiang   (501) staff       (20)       33 2022-05-23 11:32:43.000000 python-sonarqube-api-2.0.0/MANIFEST.in
+-rw-r--r--   0 shijialiang   (501) staff       (20)     5999 2023-05-26 07:25:57.079442 python-sonarqube-api-2.0.0/PKG-INFO
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4880 2023-05-26 07:11:49.000000 python-sonarqube-api-2.0.0/README.rst
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 07:25:57.018330 python-sonarqube-api-2.0.0/python_sonarqube_api.egg-info/
+-rw-r--r--   0 shijialiang   (501) staff       (20)     5999 2023-05-26 07:25:56.000000 python-sonarqube-api-2.0.0/python_sonarqube_api.egg-info/PKG-INFO
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1689 2023-05-26 07:25:56.000000 python-sonarqube-api-2.0.0/python_sonarqube_api.egg-info/SOURCES.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)        1 2023-05-26 07:25:56.000000 python-sonarqube-api-2.0.0/python_sonarqube_api.egg-info/dependency_links.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)        9 2023-05-26 07:25:56.000000 python-sonarqube-api-2.0.0/python_sonarqube_api.egg-info/requires.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)       10 2023-05-26 07:25:56.000000 python-sonarqube-api-2.0.0/python_sonarqube_api.egg-info/top_level.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)        9 2022-05-23 11:32:43.000000 python-sonarqube-api-2.0.0/requirements.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)       38 2023-05-26 07:25:57.081239 python-sonarqube-api-2.0.0/setup.cfg
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2497 2023-05-26 07:25:32.000000 python-sonarqube-api-2.0.0/setup.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 07:25:57.021285 python-sonarqube-api-2.0.0/sonarqube/
+-rw-r--r--   0 shijialiang   (501) staff       (20)      192 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/__init__.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 07:25:57.073487 python-sonarqube-api-2.0.0/sonarqube/rest/
+-rw-r--r--   0 shijialiang   (501) staff       (20)    10384 2023-05-26 06:28:40.000000 python-sonarqube-api-2.0.0/sonarqube/rest/__init__.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4212 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/alm_integrations.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)    12832 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/alm_settings.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      867 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/analysis_cache.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4930 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/applications.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      988 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/audit_logs.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1089 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/auth.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3668 2023-05-26 06:25:25.000000 python-sonarqube-api-2.0.0/sonarqube/rest/ce.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3972 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/components.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      814 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/duplications.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      742 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/editions.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1504 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/favorites.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3238 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/hotspots.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)    13831 2023-05-26 06:25:25.000000 python-sonarqube-api-2.0.0/sonarqube/rest/issues.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      723 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/languages.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     5441 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/measures.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      947 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/metrics.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      890 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/monitoring.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2593 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/new_code_periods.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2503 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/notifications.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)    15330 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/permissions.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4195 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/plugins.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4319 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/project_analyses.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2775 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/project_badges.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2031 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/project_branches.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1072 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/project_dump.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1314 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/project_links.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1111 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/project_pull_requests.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1194 2023-05-26 06:25:25.000000 python-sonarqube-api-2.0.0/sonarqube/rest/project_tags.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     6779 2023-05-26 06:25:25.000000 python-sonarqube-api-2.0.0/sonarqube/rest/projects.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     9227 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/qualitygates.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)    12092 2023-05-26 06:25:25.000000 python-sonarqube-api-2.0.0/sonarqube/rest/qualityprofiles.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)    11675 2023-05-26 06:25:25.000000 python-sonarqube-api-2.0.0/sonarqube/rest/rules.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      623 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/server.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2216 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/settings.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2262 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/sources.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     5528 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/system.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4921 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/user_groups.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2018 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/user_tokens.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     5991 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/users.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)    12507 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/views.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3510 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/webhooks.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1258 2023-05-26 05:35:49.000000 python-sonarqube-api-2.0.0/sonarqube/rest/webservices.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 07:25:57.079017 python-sonarqube-api-2.0.0/sonarqube/utils/
+-rw-r--r--   0 shijialiang   (501) staff       (20)       69 2022-05-23 11:32:43.000000 python-sonarqube-api-2.0.0/sonarqube/utils/__init__.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3631 2023-05-17 05:22:16.000000 python-sonarqube-api-2.0.0/sonarqube/utils/common.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)    17751 2023-05-26 04:55:45.000000 python-sonarqube-api-2.0.0/sonarqube/utils/config.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      401 2022-05-23 11:32:43.000000 python-sonarqube-api-2.0.0/sonarqube/utils/exceptions.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4841 2022-05-23 11:32:43.000000 python-sonarqube-api-2.0.0/sonarqube/utils/rest_client.py
```

### Comparing `python-sonarqube-api-1.3.7/python_sonarqube_api.egg-info/SOURCES.txt` & `python-sonarqube-api-2.0.0/python_sonarqube_api.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,70 +5,55 @@
 setup.py
 python_sonarqube_api.egg-info/PKG-INFO
 python_sonarqube_api.egg-info/SOURCES.txt
 python_sonarqube_api.egg-info/dependency_links.txt
 python_sonarqube_api.egg-info/requires.txt
 python_sonarqube_api.egg-info/top_level.txt
 sonarqube/__init__.py
-sonarqube/cloud/__init__.py
-sonarqube/cloud/auth.py
-sonarqube/cloud/ce.py
-sonarqube/cloud/components.py
-sonarqube/cloud/issues.py
-sonarqube/cloud/permissions.py
-sonarqube/cloud/project_badges.py
-sonarqube/cloud/projects.py
-sonarqube/cloud/qualitygates.py
-sonarqube/cloud/qualityprofiles.py
-sonarqube/cloud/rules.py
-sonarqube/cloud/settings.py
-sonarqube/cloud/user_groups.py
-sonarqube/cloud/users.py
-sonarqube/cloud/webhooks.py
-sonarqube/community/__init__.py
-sonarqube/community/alm_integrations.py
-sonarqube/community/alm_settings.py
-sonarqube/community/auth.py
-sonarqube/community/ce.py
-sonarqube/community/components.py
-sonarqube/community/duplications.py
-sonarqube/community/favorites.py
-sonarqube/community/hotspots.py
-sonarqube/community/issues.py
-sonarqube/community/languages.py
-sonarqube/community/measures.py
-sonarqube/community/metrics.py
-sonarqube/community/monitoring.py
-sonarqube/community/new_code_periods.py
-sonarqube/community/notifications.py
-sonarqube/community/permissions.py
-sonarqube/community/plugins.py
-sonarqube/community/project_analyses.py
-sonarqube/community/project_badges.py
-sonarqube/community/project_branches.py
-sonarqube/community/project_dump.py
-sonarqube/community/project_links.py
-sonarqube/community/project_pull_requests.py
-sonarqube/community/project_tags.py
-sonarqube/community/projects.py
-sonarqube/community/qualitygates.py
-sonarqube/community/qualityprofiles.py
-sonarqube/community/rules.py
-sonarqube/community/server.py
-sonarqube/community/settings.py
-sonarqube/community/sources.py
-sonarqube/community/system.py
-sonarqube/community/user_groups.py
-sonarqube/community/user_tokens.py
-sonarqube/community/users.py
-sonarqube/community/webhooks.py
-sonarqube/community/webservices.py
-sonarqube/enterprise/__init__.py
-sonarqube/enterprise/applications.py
-sonarqube/enterprise/audit_logs.py
-sonarqube/enterprise/editions.py
-sonarqube/enterprise/views.py
+sonarqube/rest/__init__.py
+sonarqube/rest/alm_integrations.py
+sonarqube/rest/alm_settings.py
+sonarqube/rest/analysis_cache.py
+sonarqube/rest/applications.py
+sonarqube/rest/audit_logs.py
+sonarqube/rest/auth.py
+sonarqube/rest/ce.py
+sonarqube/rest/components.py
+sonarqube/rest/duplications.py
+sonarqube/rest/editions.py
+sonarqube/rest/favorites.py
+sonarqube/rest/hotspots.py
+sonarqube/rest/issues.py
+sonarqube/rest/languages.py
+sonarqube/rest/measures.py
+sonarqube/rest/metrics.py
+sonarqube/rest/monitoring.py
+sonarqube/rest/new_code_periods.py
+sonarqube/rest/notifications.py
+sonarqube/rest/permissions.py
+sonarqube/rest/plugins.py
+sonarqube/rest/project_analyses.py
+sonarqube/rest/project_badges.py
+sonarqube/rest/project_branches.py
+sonarqube/rest/project_dump.py
+sonarqube/rest/project_links.py
+sonarqube/rest/project_pull_requests.py
+sonarqube/rest/project_tags.py
+sonarqube/rest/projects.py
+sonarqube/rest/qualitygates.py
+sonarqube/rest/qualityprofiles.py
+sonarqube/rest/rules.py
+sonarqube/rest/server.py
+sonarqube/rest/settings.py
+sonarqube/rest/sources.py
+sonarqube/rest/system.py
+sonarqube/rest/user_groups.py
+sonarqube/rest/user_tokens.py
+sonarqube/rest/users.py
+sonarqube/rest/views.py
+sonarqube/rest/webhooks.py
+sonarqube/rest/webservices.py
 sonarqube/utils/__init__.py
 sonarqube/utils/common.py
 sonarqube/utils/config.py
 sonarqube/utils/exceptions.py
 sonarqube/utils/rest_client.py
```

### Comparing `python-sonarqube-api-1.3.7/setup.py` & `python-sonarqube-api-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,22 +34,22 @@
     version=get_version(),
 
     description='Python wrapper for the SonarQube and SonarCloud API.',
     long_description=long_description,
     url='https://github.com/shijl0925/python-sonarqube-api',
     author='Jialiang Shi',
     author_email='kevin09254930sjl@gmail.com',
-    license='MIT',
+    license='AGPL',
 
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Plugins',
         'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
+        'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/cloud/auth.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/editions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-from sonarqube.community.auth import SonarQubeAuth
+from sonarqube.utils.common import POST
+from sonarqube.utils.rest_client import RestClient
 
+from sonarqube.utils.config import API_EDITIONS_SET_LICENSE  # pro
 
-class SonarCloudAuth(SonarQubeAuth):
+
+class SonarQubeEditions(RestClient):
     """
-    SonarCloud authentication Operations
+    Manage SonarSource commercial editions
     """
 
-    def authenticate_user(self, login, password):
+    def __init__(self, **kwargs):
+        """
+
+        :param kwargs:
+        """
+        super(SonarQubeEditions, self).__init__(**kwargs)
+
+    @POST(API_EDITIONS_SET_LICENSE)
+    def set_license(self, license):
         """
-        Authenticate a user.
+        since 7.2
+        Set the license for enabling features of commercial editions.
+        Require 'Administer System' permission.
 
-        :param login: Login of the user
-        :param password: Password of the user
+        :param license:
         :return:
         """
-        raise AttributeError(
-            "%s does not support this method" % self.__class__.__name__
-        )
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/cloud/permissions.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/permissions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,132 +1,183 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-from sonarqube.community.permissions import SonarQubePermissions
+from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
     API_PERMISSIONS_ADD_GROUP_ENDPOINT,
     API_PERMISSIONS_REMOVE_GROUP_ENDPOINT,
+    API_PERMISSIONS_USERS_ENDPOINT,
+    API_PERMISSIONS_GROUPS_ENDPOINT,
     API_PERMISSIONS_ADD_USER_ENDPOINT,
     API_PERMISSIONS_REMOVE_USER_ENDPOINT,
     API_PERMISSIONS_APPLY_TEMPLATE_ENDPOINT,
     API_PERMISSIONS_ADD_GROUP_TO_TEMPLATE_ENDPOINT,
     API_PERMISSIONS_REMOVE_GROUP_FROM_TEMPLATE_ENDPOINT,
     API_PERMISSIONS_ADD_PROJECT_CREATOR_TO_TEMPLATE_ENDPOINT,
     API_PERMISSIONS_REMOVE_PROJECT_CREATOR_FROM_TEMPLATE_ENDPOINT,
     API_PERMISSIONS_ADD_USER_TO_TEMPLATE_ENDPOINT,
     API_PERMISSIONS_REMOVE_USER_FROM_TEMPLATE_ENDPOINT,
     API_PERMISSIONS_BULK_APPLY_TEMPLATE_ENDPOINT,
     API_PERMISSIONS_CREATE_TEMPLATE_ENDPOINT,
     API_PERMISSIONS_DELETE_TEMPLATE_ENDPOINT,
     API_PERMISSIONS_SEARCH_TEMPLATES_ENDPOINT,
     API_PERMISSIONS_SET_DEFAULT_TEMPLATE_ENDPOINT,
+    API_PERMISSIONS_UPDATE_TEMPLATE_ENDPOINT,
+    API_PERMISSIONS_GET_TEMPLATE_USERS,
+    API_PERMISSIONS_GET_TEMPLATE_GROUPS,
 )
 from sonarqube.utils.common import GET, POST
 
 
-class SonarCloudPermissions(SonarQubePermissions):
+class SonarQubePermissions(RestClient):
     """
-    SonarCloud permissions Operations
+    SonarQube permissions Operations
     """
 
+    def __init__(self, **kwargs):
+        """
+
+        :param kwargs:
+        """
+        super(SonarQubePermissions, self).__init__(**kwargs)
+
     @POST(API_PERMISSIONS_ADD_GROUP_ENDPOINT)
-    def add_permission_to_group(
-        self, groupName, organization, permission, projectKey=None
-    ):
+    def add_permission_to_group(self, groupName, permission, organization=None, projectKey=None):
         """
+        SINCE 5.2
         Add permission to a group.
         This service defaults to global permissions, but can be limited to project permissions by providing project key.
         The group name must be provided.
 
         :param groupName: Group name or 'anyone' (case insensitive)
-        :param organization: Key of organization
         :param permission: Permission.
           Possible values are for:
             * Possible values for global permissions: admin, profileadmin, gateadmin, scan, provisioning
             * Possible values for project permissions admin, codeviewer, issueadmin, securityhotspotadmin, scan, user
+        :param organization: Key of organization
         :param projectKey: Project key
         :return:
         """
 
     @POST(API_PERMISSIONS_REMOVE_GROUP_ENDPOINT)
-    def remove_permission_from_group(
-        self, groupName, organization, permission, projectKey=None
-    ):
+    def remove_permission_from_group(self, groupName, permission, organization=None, projectKey=None):
         """
+        SINCE 5.2
         Remove a permission from a group.
         This service defaults to global permissions, but can be limited to project permissions by providing project key.
         The group name must be provided.
 
         :param groupName: Group name or 'anyone' (case insensitive)
-        :param organization: Key of organization
         :param permission: Permission
           Possible values are for:
             * Possible values for global permissions: admin, profileadmin, gateadmin, scan, provisioning
             * Possible values for project permissions admin, codeviewer, issueadmin, securityhotspotadmin, scan, user
+        :param organization: Key of organization
         :param projectKey: Project key
         :return:
         """
 
     @POST(API_PERMISSIONS_ADD_USER_ENDPOINT)
-    def add_permission_to_user(self, login, organization, permission, projectKey=None):
+    def add_permission_to_user(self, login, permission, organization=None, projectKey=None):
         """
+        SINCE 5.2
         Add permission to a user.
         This service defaults to global permissions, but can be limited to project permissions by providing project key.
 
         :param login: User login
+        :param permission: Permission
+          Possible values are for:
+            * Possible values for global permissions: admin, profileadmin, gateadmin, scan, provisioning
+            * Possible values for project permissions admin, codeviewer, issueadmin, securityhotspotadmin, scan, user
         :param organization: Key of organization
+        :param projectKey: Project key
+        :return:
+        """
+
+    @GET(API_PERMISSIONS_USERS_ENDPOINT)
+    def get_users_permissions(self, permission=None, projectKey=None, q=None, p=None, ps=None):
+        """
+        SINCE 5.2
+        Lists the users with their permissions as individual users rather than through group affiliation.
+        This service defaults to global permissions, but can be limited to project permissions by providing project id or project key.
+        This service defaults to all users, but can be limited to users with a specific permission by providing the desired permission.
+
+        :param permission: Permission
+          Possible values are for:
+            * Possible values for global permissions: admin, profileadmin, gateadmin, scan, provisioning
+            * Possible values for project permissions admin, codeviewer, issueadmin, securityhotspotadmin, scan, user
+        :param projectKey: Project key
+        :param q: Limit search to user names that contain the supplied string
+        :param p: page number.
+        :param ps: Page size. Must be greater than 0 and less or equal than 500
+        :return:
+        """
+
+    @GET(API_PERMISSIONS_GROUPS_ENDPOINT)
+    def get_groups_permissions(self, permission=None, projectKey=None, q=None, p=None, ps=None):
+        """
+        SINCE 5.2
+        Lists the groups with their permissions.
+        This service defaults to global permissions, but can be limited to project permissions by providing project id or project key.
+        This service defaults to all groups, but can be limited to groups with a specific permission by providing the desired permission.
+
         :param permission: Permission
           Possible values are for:
             * Possible values for global permissions: admin, profileadmin, gateadmin, scan, provisioning
             * Possible values for project permissions admin, codeviewer, issueadmin, securityhotspotadmin, scan, user
         :param projectKey: Project key
+        :param projectId: Project id
+        :param q: Limit search to group names that contain the supplied string
+        :param p: page number.
+        :param ps: Page size. Must be greater than 0 and less or equal than 500
         :return:
         """
 
     @POST(API_PERMISSIONS_REMOVE_USER_ENDPOINT)
-    def remove_permission_from_user(
-        self, login, organization, permission, projectKey=None
-    ):
+    def remove_permission_from_user(self, login, permission, organization=None, projectKey=None):
         """
+        SINCE 5.2
         Remove permission from a user.
         This service defaults to global permissions, but can be limited to project permissions by providing project key.
 
         :param login: User login
-        :param organization: Key of organization
         :param permission: Permission
           Possible values are for:
             * Possible values for global permissions: admin, profileadmin, gateadmin, scan, provisioning
             * Possible values for project permissions admin, codeviewer, issueadmin, securityhotspotadmin, scan, user
+        :param organization: Key of organization
         :param projectKey: Project key
         :return:
         """
 
     @POST(API_PERMISSIONS_APPLY_TEMPLATE_ENDPOINT)
-    def apply_template_to_project(self, templateName, organization, projectKey):
+    def apply_template_to_project(self, templateName, projectKey, organization=None):
         """
+        SINCE 5.2
         Apply a permission template to one project.
 
         :param templateName: Template name
-        :param organization: Key of organization
         :param projectKey: Project key
+        :param organization: Key of organization
         :return:
         """
 
     @POST(API_PERMISSIONS_BULK_APPLY_TEMPLATE_ENDPOINT)
     def apply_template_to_projects(
         self,
         templateName,
-        organization,
+        organization=None,
         projects=None,
         analyzedBefore=None,
         onProvisionedOnly="false",
         q=None,
         qualifiers="TRK",
     ):
         """
+        SINCE 5.5
         Apply a permission template to several projects.
 
         :param templateName: Template name
         :param organization: Key of organization
         :param projects: Comma-separated list of project keys
         :param analyzedBefore: Filter the projects for which last analysis is older than the given date (exclusive).
         :param onProvisionedOnly: Filter the projects that are provisioned.
@@ -139,139 +190,180 @@
           qualifiers. Possible values are:
             * TRK - Projects
           default value is TRK.
         :return:
         """
 
     @POST(API_PERMISSIONS_ADD_GROUP_TO_TEMPLATE_ENDPOINT)
-    def add_group_to_template(self, groupName, organization, templateName, permission):
+    def add_group_to_template(self, groupName, templateName, permission, organization=None):
         """
+        SINCE 5.2
         Add a group to a permission template.
 
         :param groupName: Group name or 'anyone' (case insensitive)
-        :param organization: Key of organization
         :param templateName: Template name
         :param permission: Permission
           Possible values are for:
             * Possible values for project permissions admin, codeviewer, issueadmin, securityhotspotadmin, scan, user
+        :param organization: Key of organization
         :return:
         """
 
     @POST(API_PERMISSIONS_REMOVE_GROUP_FROM_TEMPLATE_ENDPOINT)
-    def remove_group_from_template(
-        self, groupName, organization, templateName, permission
-    ):
+    def remove_group_from_template(self, groupName, templateName, permission, organization=None):
         """
+        SINCE 5.2
         Remove a group from a permission template.
 
         :param groupName: Group name or 'anyone' (case insensitive)
-        :param organization: Key of organization
         :param templateName: Template name
         :param permission: Permission
           Possible values are for:
             * Possible values for project permissions admin, codeviewer, issueadmin, securityhotspotadmin, scan, user
+        :param organization: Key of organization
         :return:
         """
 
     @POST(API_PERMISSIONS_ADD_PROJECT_CREATOR_TO_TEMPLATE_ENDPOINT)
-    def add_project_creator_to_template(self, templateName, organization, permission):
+    def add_project_creator_to_template(self, templateName, permission, organization=None):
         """
+        SINCE 6.0
         Add a project creator to a permission template.
 
         :param templateName: Template name
-        :param organization: Key of organizatio
         :param permission: Permission
           Possible values are for:
             * Possible values for project permissions admin, codeviewer, issueadmin, securityhotspotadmin, scan, user
+        :param organization: Key of organization
         :return:
         """
 
     @POST(API_PERMISSIONS_REMOVE_PROJECT_CREATOR_FROM_TEMPLATE_ENDPOINT)
-    def remove_project_creator_from_template(
-        self, templateName, organization, permission
-    ):
+    def remove_project_creator_from_template(self, templateName, permission, organization=None):
         """
+        SINCE 6.0
         Remove a project creator from a permission template.
 
         :param templateName: Template name
-        :param organization: Key of organization
         :param permission: Permission
           Possible values are for:
             * Possible values for project permissions admin, codeviewer, issueadmin, securityhotspotadmin, scan, user
+        :param organization: Key of organization
         :return:
         """
 
     @POST(API_PERMISSIONS_ADD_USER_TO_TEMPLATE_ENDPOINT)
-    def add_user_to_template(self, login, organization, templateName, permission):
+    def add_user_to_template(self, login, templateName, permission, organization=None):
         """
+        SINCE 5.2
         Add a user to a permission template.
 
         :param login: User login
-        :param organization: Key of organization
         :param templateName: Template name
         :param permission: Permission
           Possible values are for:
             * Possible values for project permissions admin, codeviewer, issueadmin, securityhotspotadmin, scan, user
+        :param organization: Key of organization
         :return:
         """
 
     @POST(API_PERMISSIONS_REMOVE_USER_FROM_TEMPLATE_ENDPOINT)
-    def remove_user_from_template(self, login, organization, templateName, permission):
+    def remove_user_from_template(self, login, templateName, permission, organization=None):
         """
+        SINCE 5.2
         Remove a user from a permission template.
 
         :param login: User login
-        :param organization: Key of organization
         :param templateName: Template name
         :param permission: Permission
           Possible values are for:
             * Possible values for project permissions admin, codeviewer, issueadmin, securityhotspotadmin, scan, user
+        :param organization: Key of organization
         :return:
         """
 
     @POST(API_PERMISSIONS_CREATE_TEMPLATE_ENDPOINT)
-    def create_template(
-        self, name, organization, description=None, projectKeyPattern=None
-    ):
+    def create_template(self, name, organization=None, description=None, projectKeyPattern=None):
         """
+        SINCE 5.2
         Create a permission template.
 
         :param name: Template name
         :param organization: Key of organization
         :param description: Template description
         :param projectKeyPattern: Project key pattern. Must be a valid Java regular expression
         :return: request response.
         """
 
     @POST(API_PERMISSIONS_DELETE_TEMPLATE_ENDPOINT)
-    def delete_template(self, templateName, organization):
+    def delete_template(self, templateName, organization=None):
         """
+        SINCE 5.2
         Delete a permission template.
 
         :param templateName: Template name
         :param organization: Key of organization
         :return:
         """
 
     @GET(API_PERMISSIONS_SEARCH_TEMPLATES_ENDPOINT)
-    def search_templates(self, organization, q=None):
+    def search_templates(self, organization=None, q=None):
         """
+        SINCE 5.2
         List permission templates.
 
         :param organization: Key of organization
         :param q: Limit search to permission template names that contain the supplied string.
         :return: defaultTemplates, permissionTemplates, permissions
         """
 
+    @GET(API_PERMISSIONS_GET_TEMPLATE_USERS)
+    def get_template_users(self, templateId, permission=None, p=None, ps=None):
+        """
+        List of users and their permissions for the specified template.
+
+        :param templateId: Id of permission template
+        :param permission: Possible values for project permissions admin, codeviewer, issueadmin, securityhotspotadmin, scan, user
+        :param p: page number.
+        :param ps: Page size. Must be greater than 0 and less or equal than 500
+        return: users
+        """
+
+    @GET(API_PERMISSIONS_GET_TEMPLATE_GROUPS)
+    def get_template_groups(self, templateId, permission=None, p=None, ps=None):
+        """
+        List of groups and their permissions for the specified template.
+
+        :param templateId: Id of permission template
+        :param permission: Possible values for project permissions admin, codeviewer, issueadmin, securityhotspotadmin, scan, user
+        :param p: page number.
+        :param ps: Page size. Must be greater than 0 and less or equal than 500
+        return: groups
+        """
+
     @POST(API_PERMISSIONS_SET_DEFAULT_TEMPLATE_ENDPOINT)
-    def set_default_template(self, templateName, organization, qualifier="TRK"):
+    def set_default_template(self, templateName, organization=None, qualifier="TRK"):
         """
+        SINCE 5.2
         Set a permission template as default.
 
         :param templateName: Template name
         :param organization: Key of organization
         :param qualifier: Project qualifier. Filter the results with the specified qualifier.
           Possible values are:
             * TRK - Projects
           default value is TRK.
         :return:
         """
+
+    @POST(API_PERMISSIONS_UPDATE_TEMPLATE_ENDPOINT)
+    def update_template(self, id, name=None, description=None, projectKeyPattern=None):
+        """
+        SINCE 5.2
+        Update a permission template.
+
+        :param id: Template id
+        :param name: Template name
+        :param description: Template description
+        :param projectKeyPattern: Project key pattern. Must be a valid Java regular expression
+        :return: request response
+        """
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/cloud/qualitygates.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/qualitygates.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,217 +1,265 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-from sonarqube.community.qualitygates import SonarQubeQualityGates
+from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
     API_QUALITYGATES_LIST_ENDPOINT,
+    API_QUALITYGATES_PROJECT_STATUS_ENDPOINT,
     API_QUALITYGATES_SELECT_ENDPOINT,
     API_QUALITYGATES_DESELECT_ENDPOINT,
     API_QUALITYGATES_SHOW_ENDPOINT,
     API_QUALITYGATES_GET_BY_PROJECT_ENDPOINT,
     API_QUALITYGATES_COPY_ENDPOINT,
     API_QUALITYGATES_CREATE_ENDPOINT,
     API_QUALITYGATES_DESTROY_ENDPOINT,
     API_QUALITYGATES_RENAME_ENDPOINT,
     API_QUALITYGATES_CREATE_CONDITION_ENDPOINT,
     API_QUALITYGATES_DELETE_CONDITION_ENDPOINT,
     API_QUALITYGATES_UPDATE_CONDITION_ENDPOINT,
     API_QUALITYGATES_SEARCH_ENDPOINT,
     API_QUALITYGATES_SET_AS_DEFAULT_ENDPOINT,
+    API_QUALITYGATES_ADD_GROUP_ENDPOINT,
 )
 from sonarqube.utils.common import GET, POST
 
 
-class SonarCloudQualityGates(SonarQubeQualityGates):
+class SonarQubeQualityGates(RestClient):
     """
-    SonarCloud quality gates Operations
+    SonarQube quality gates Operations
     """
 
+    def __init__(self, **kwargs):
+        """
+
+        :param kwargs:
+        """
+        super(SonarQubeQualityGates, self).__init__(**kwargs)
+
+    @POST(API_QUALITYGATES_ADD_GROUP_ENDPOINT)
+    def add_group_to_gate(self, gateName, groupName):
+        """
+        SINCE 9.2
+        Allow a group of users to edit a Quality Gate.
+
+        :param gateName: The name of the quality gate
+        :param groupName: The name of the group that can administer the gate
+        :return:
+        """
+
     @POST(API_QUALITYGATES_COPY_ENDPOINT)
-    def copy_quality_gate(self, id, name, organization):
+    def copy_quality_gate(self, id, name, organization=None):
         """
+        SINCE 4.3
         Copy a Quality Gate.
 
         :param id: The ID of the source quality gate
         :param name: The name of the quality gate to create
-        :param organization: Organization key.
+        :param organization: Organization key. If no organization is provided, the default organization is used.
         :return:
         """
 
     @POST(API_QUALITYGATES_CREATE_ENDPOINT)
-    def create_quality_gate(self, name, organization):
+    def create_quality_gate(self, name, organization=None):
         """
+        SINCE 4.3
         Create a Quality Gate.
 
         :param name: The name of the quality gate to create
-        :param organization: Organization key.
+        :param organization: Organization key. If no organization is provided, the default organization is used.
         :return: request response
         """
 
     @POST(API_QUALITYGATES_DESTROY_ENDPOINT)
-    def delete_quality_gate(self, id, organization):
+    def delete_quality_gate(self, id, organization=None):
         """
+        SINCE 4.3
         Delete a Quality Gate.
 
         :param id: ID of the quality gate to delete
-        :param organization: Organization key.
+        :param organization: Organization key. If no organization is provided, the default organization is used.
         :return:
         """
 
     @POST(API_QUALITYGATES_RENAME_ENDPOINT)
-    def rename_quality_gate(self, id, name, organization):
+    def rename_quality_gate(self, id, name, organization=None):
         """
+        SINCE 4.3
         Rename a Quality Gate.
 
         :param id: ID of the quality gate to rename
         :param name: New name of the quality gate
-        :param organization: Organization key.
+        :param organization: Organization key. If no organization is provided, the default organization is used.
         :return:
         """
 
     @POST(API_QUALITYGATES_CREATE_CONDITION_ENDPOINT)
     def create_condition_to_quality_gate(
-        self, gateId, organization, metric, error, op=None
+        self, gateId, metric, error, op=None, organization=None
     ):
         """
+        SINCE 4.3
         Add a new condition to a quality gate.
 
         :param gateId: ID of the quality gate
-        :param organization: Organization key.
         :param metric: Condition metric.
           Only metric of the following types are allowed:
             * INT
             * MILLISEC
             * RATING
             * WORK_DUR
             * FLOAT
             * PERCENT
             * LEVEL
         :param error: Condition error threshold
         :param op: Condition operator
           Possible values are for:
             * LT = is lower than
             * GT = is greater than
-
+        :param organization: Organization key. If no organization is provided, the default organization is used.
         :return: request response
         """
 
     @POST(API_QUALITYGATES_DELETE_CONDITION_ENDPOINT)
-    def delete_condition_from_quality_gate(self, id, organization):
+    def delete_condition_from_quality_gate(self, id, organization=None):
         """
+        SINCE 4.3
         Delete a condition from a quality gate.
 
         :param id: Condition ID
-        :param organization: Organization key.
+        :param organization: Organization key. If no organization is provided, the default organization is used.
         :return:
         """
 
     @POST(API_QUALITYGATES_UPDATE_CONDITION_ENDPOINT)
     def update_condition_to_quality_gate(
-        self, id, organization, metric, error, op=None
+        self, id, metric, error, op=None, organization=None
     ):
         """
+        SINCE 4.3
         Update a condition attached to a quality gate.
 
         :param id: Condition ID
-        :param organization: Organization key.
         :param metric: Condition metric.
           Only metric of the following types are allowed:
             * INT
             * MILLISEC
             * RATING
             * WORK_DUR
             * FLOAT
             * PERCENT
             * LEVEL
         :param error: Condition error threshold
         :param op: Condition operator
           Possible values are for:
             * LT = is lower than
             * GT = is greater than
-
+        :param organization: Organization key. If no organization is provided, the default organization is used.
         :return:
         """
 
     @GET(API_QUALITYGATES_SEARCH_ENDPOINT)
     def get_qualitygate_projects(
-        self, gateId, organization, selected="selected", query=None, page=None, pageSize=None
+        self, gateId, selected="selected", query=None, organization=None, page=None, pageSize=None
     ):
         """
+        SINCE 4.3
         Search for projects associated (or not) to a quality gate.
 
         :param gateId: Quality Gate ID
-        :param organization: Organization key.
         :param selected: Depending on the value, show only selected items (selected=selected),
           deselected items (selected=deselected), or all items with their selection status (selected=all).
           Possible values are for:
             * all
             * deselected
             * selected
           default value is selected
         :param query: To search for projects containing this string.
           If this parameter is set, "selected" is set to "all".
-
+        :param organization: Organization key. If no organization is provided, the default organization is used.
         :param page: page number.
         :param pageSize: Page size.
         :return:
         """
 
     @POST(API_QUALITYGATES_SET_AS_DEFAULT_ENDPOINT)
-    def set_default_qualitygate(self, id, organization):
+    def set_default_qualitygate(self, id, organization=None):
         """
+        SINCE 4.3
         Set a quality gate as the default quality gate.
 
         :param id: ID of the quality gate to set as default
-        :param organization: Organization key.
+        :param organization: Organization key. If no organization is provided, the default organization is used.
+        :return:
+        """
+
+    @GET(API_QUALITYGATES_PROJECT_STATUS_ENDPOINT)
+    def get_project_qualitygates_status(
+        self, projectKey=None, analysisId=None, branch=None, pullRequest=None
+    ):
+        """
+        SINCE 5.3
+        Get the quality gate status of a project or a Compute Engine task. return 'ok','WARN','ERROR'
+        The NONE status is returned when there is no quality gate associated with the analysis.
+        Returns an HTTP code 404 if the analysis associated with the task is not found or does not exist.
+
+        :param projectKey: Project key
+        :param analysisId: Analysis id
+        :param branch: Branch key
+        :param pullRequest:
         :return:
         """
 
     @GET(API_QUALITYGATES_LIST_ENDPOINT)
-    def get_quality_gates(self, organization):
+    def get_quality_gates(self, organization=None):
         """
+        SINCE 4.3
         Get a list of quality gates
 
         :param organization: Organization key. If no organization is provided, the default organization is used.
         :return:
         """
 
     @POST(API_QUALITYGATES_SELECT_ENDPOINT)
-    def select_quality_gate_for_project(self, projectKey, gateId, organization):
+    def select_quality_gate_for_project(self, projectKey, gateName, organization=None):
         """
+        SINCE 4.3
         Associate a project to a quality gate.
 
         :param projectKey: Project key
-        :param gateId: Quality gate id
-        :param organization: Organization key.
+        :param gateName: Quality gate name (since version 8.4). Refer https://sonarqube.inria.fr/sonarqube/web_api/api/qualitygates
+        :param organization: Organization key. If no organization is provided, the default organization is used.
         :return:
         """
 
     @POST(API_QUALITYGATES_DESELECT_ENDPOINT)
-    def remove_project_from_quality_gate(self, projectKey, organization):
+    def remove_project_from_quality_gate(self, projectKey, organization=None):
         """
+        SINCE 4.3
         Remove the association of a project from a quality gate.
 
         :param projectKey: Project key
-        :param organization: Organization key.
+        :param organization: Organization key. If no organization is provided, the default organization is used.
         :return:
         """
 
     @GET(API_QUALITYGATES_SHOW_ENDPOINT)
-    def show_quality_gate(self, name, organization):
+    def show_quality_gate(self, name, organization=None):
         """
+        SINCE 4.3
         Display the details of a quality gate.
 
         :param name: Name of the quality gate.
-        :param organization: Organization key.
+        :param organization: Organization key. If no organization is provided, the default organization is used.
         :return:
         """
 
     @GET(API_QUALITYGATES_GET_BY_PROJECT_ENDPOINT)
-    def get_quality_gate_of_project(self, project, organization):
+    def get_quality_gate_of_project(self, project, organization=None):
         """
+        SINCE 6.1
         Get the quality gate of a project.
 
         :param project: Project key
-        :param organization: Organization key.
+        :param organization: Organization key. If no organization is provided, the default organization is used.
         :return:
         """
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/cloud/rules.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-from sonarqube.community.rules import SonarQubeRules
+from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
     API_RULES_SEARCH_ENDPOINT,
+    API_RULES_CREATE_ENDPOINT,
     API_RULES_UPDATE_ENDPOINT,
+    API_RULES_DELETE_ENDPOINT,
     API_RULES_SHOW_ENDPOINT,
     API_RULES_TAGS_ENDPOINT,
+    API_RULES_REPOSITORIES_ENDPOINT,
 )
 from sonarqube.utils.common import GET, POST
 
 
-class SonarCloudRules(SonarQubeRules):
+class SonarQubeRules(RestClient):
     """
-    SonarCloud rules Operations
+    SonarQube rules Operations
     """
 
+    def __init__(self, **kwargs):
+        """
+
+        :param kwargs:
+        """
+        super(SonarQubeRules, self).__init__(**kwargs)
+
     def get(self, key):
-        raise AttributeError(
-            "%s does not support this method" % self.__class__.__name__
-        )
+        result = self.search_rules(rule_key=key)
+        rules = result.get("rules", [])
+
+        for rule in rules:
+            if rule["key"] == key:
+                return rule
 
     @GET(API_RULES_SEARCH_ENDPOINT)
     def search_rules(
         self,
-        organization,
+        organization=None,
         activation=None,
         qprofile=None,
         languages=None,
         active_severities=None,
         asc="true",
         available_since=None,
         cwe=None,
@@ -49,14 +62,15 @@
         sonarsourceSecurity=None,
         statuses=None,
         tags=None,
         template_key=None,
         types=None,
     ):
         """
+        SINCE 4.4
         Search for a collection of relevant rules matching a specified query.
 
         :param organization: organization key.
         :param activation: Filter rules that are activated or deactivated on the selected Quality profile. Ignored if the parameter 'qprofile' is not set.
         :param qprofile: Quality profile key to filter on. Used only if the parameter 'activation' is set.
         :param languages: Comma-separated list of languages
         :param active_severities: Comma-separated list of activation severities,
@@ -207,105 +221,147 @@
             * BUG
             * VULNERABILITY
             * SECURITY_HOTSPOT
 
         :return:
         """
 
+    @POST(API_RULES_CREATE_ENDPOINT)
     def create_rule(
         self,
         custom_key,
         name,
         markdown_description,
         template_key,
         severity,
         status=None,
         type=None,
         params=None,
     ):
         """
+        SINCE 4.4
+        Create a a custom rule.
 
-        :param custom_key:
-        :param name:
-        :param markdown_description:
-        :param template_key:
-        :param severity:
-        :param status:
-        :param type:
-        :param params:
-        :return:
-        """
-        raise AttributeError(
-            "%s does not support this method" % self.__class__.__name__
-        )
-
-    @POST(API_RULES_UPDATE_ENDPOINT)
-    def update_rule(self, key, organization, **kwargs):
-        """
-        Update an existing rule.
-
-        :param key: Key of the rule to update
-        :param organization: organization key.
-
-        optional parameters:
-          * name: Rule name (mandatory for custom rule)
-          * description: Rule description (mandatory for custom rule and manual rule)
-          * markdown_note: Optional note in markdown format. Use empty value to remove current note.
-            Note is not changed if the parameter is not set.
-          * params: Parameters as semi-colon list of =, for example 'params=key1=v1;key2=v2'
-            (Only when updating a custom rule)
-          * remediation_fn_base_effort: Base effort of the remediation function of the rule
-          * remediation_fn_type: Type of the remediation function of the rule
-          * remediation_fy_gap_multiplier: Gap multiplier of the remediation function of the rule
-          * severity: Rule severity (Only when updating a custom rule).Possible values are for:
-
+        :param custom_key: Key of the custom rule
+        :param name: Rule name
+        :param markdown_description: Rule description
+        :param template_key: Key of the template rule in order to create a custom rule (mandatory for custom rule)
+        :param severity: Rule severity.
+          Possible values are for:
             * INFO
             * MINOR
             * MAJOR
             * CRITICAL
             * BLOCKER
-
-          * status: Rule status (Only when updating a custom rule). Possible values are for:
-
+        :param status: Rule status.
+          Possible values are for:
             * BETA
             * DEPRECATED
             * READY
             * REMOVED
+        :param type: Rule type.
+          Possible values are for:
+            * CODE_SMELL
+            * BUG
+            * VULNERABILITY
+            * SECURITY_HOTSPOT
+        :param params: Parameters as semi-colon list of =, for example 'params=key1=v1;key2=v2' (Only for custom rule)
+
+        :return: request response
+        """
 
-          * tags: Optional comma-separated list of tags to set. Use blank value to remove current tags.
-            Tags are not changed if the parameter is not set.
+    @POST(API_RULES_UPDATE_ENDPOINT)
+    def update_rule(
+        self,
+        key,
+        organization=None,
+        name=None,
+        markdown_description=None,
+        markdown_note=None,
+        remediation_fn_base_effort=None,
+        remediation_fn_type=None,
+        remediation_fy_gap_multiplier=None,
+        severity=None,
+        status=None,
+        tags=None,
+        params=None
+    ):
+        """
+        SINCE 4.4
+        Update an existing rule.
+
+        :param key: Key of the rule to update
+        :param organization: organization key.
+        :param name: Rule name (mandatory for custom rule)
+        :param markdown_description: Rule description (mandatory for custom rule and manual rule)
+        :param markdown_note: Optional note in markdown format. Use empty value to remove current note.
+          Note is not changed if the parameter is not set.
+        :param params: Parameters as semi-colon list of =, for example 'params=key1=v1;key2=v2'
+          (Only when updating a custom rule)
+        :param remediation_fn_base_effort: Base effort of the remediation function of the rule
+        :param remediation_fn_type: Type of the remediation function of the rule
+        :param remediation_fy_gap_multiplier: Gap multiplier of the remediation function of the rule
+        :param severity: Rule severity (Only when updating a custom rule).Possible values are for:
+
+          * INFO
+          * MINOR
+          * MAJOR
+          * CRITICAL
+          * BLOCKER
+
+        :param status: Rule status (Only when updating a custom rule). Possible values are for:
+
+          * BETA
+          * DEPRECATED
+          * READY
+          * REMOVED
+
+        :param tags: Optional comma-separated list of tags to set. Use blank value to remove current tags.
+          Tags are not changed if the parameter is not set.
 
         :return: request response
         """
 
+    @POST(API_RULES_DELETE_ENDPOINT)
     def delete_rule(self, key):
         """
-
+        SINCE 4.4
+        Delete custom rule.
         :param key:
         :return:
         """
-        raise AttributeError(
-            "%s does not support this method" % self.__class__.__name__
-        )
 
     @GET(API_RULES_SHOW_ENDPOINT)
-    def get_rule(self, key, organization, actives="false"):
+    def get_rule(self, key, organization=None, actives="false"):
         """
+        SINCE 4.2
         Get detailed information about a rule.
 
         :param key: Rule key
         :param organization: organization key.
         :param actives: Show rule's activations for all profiles ("active rules").
           Possible values are for: true or false. default value is false.
         :return:
         """
 
+    @GET(API_RULES_REPOSITORIES_ENDPOINT)
+    def get_rule_repositories(self, language=None, q=None):
+        """
+        SINCE 4.5
+        List available rule repositories
+
+        :param language: A language key; if provided, only repositories for the given language will be returned
+        :param q: A pattern to match repository keys/names against
+        :return:
+        """
+
     @GET(API_RULES_TAGS_ENDPOINT)
-    def get_rule_tags(self, organization, ps=10, q=None):
+    def get_rule_tags(self, organization=None, ps=10, q=None):
         """
+        SINCE 4.4
         List rule tags
 
         :param organization: organization key.
         :param ps: Page size. Must be greater than 0 and less or equal than 100.default value is 10.
         :param q: Limit search to tags that contain the supplied string.
         :return:
         """
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/cloud/settings.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,84 +7,68 @@
     API_SETTINGS_RESET_ENDPOINT,
     API_SETTINGS_VALUES_ENDPOINT,
     API_SETTINGS_LIST_DEFINITIONS_ENDPOINT,
 )
 from sonarqube.utils.common import GET, POST
 
 
-class SonarCloudSettings(RestClient):
+class SonarQubeSettings(RestClient):
     """
-    SonarCloud settings Operations
+    SonarQube settings Operations
     """
 
     def __init__(self, **kwargs):
         """
 
         :param kwargs:
         """
-        super(SonarCloudSettings, self).__init__(**kwargs)
+        super(SonarQubeSettings, self).__init__(**kwargs)
 
     @POST(API_SETTINGS_SET_ENDPOINT)
-    def update_setting_value(
-        self,
-        key,
-        value,
-        component=None,
-        branch=None,
-        pullRequest=None,
-        fieldValues=None,
-    ):
+    def update_setting_value(self, key, value, component=None, fieldValues=None):
         """
+        SINCE 6.1
         Update a setting value.
         The settings defined in conf/sonar.properties are read-only and can't be changed.
 
         :param key: Setting key
         :param value: Setting value. To reset a value, please use the reset web service.
         :param component: Component key
-        :param branch: Branch key. Only available on following settings : sonar.leak.period
-        :param pullRequest: Pull request id. Only available on following settings : sonar.leak.period
         :param fieldValues: Setting field values. To set several values, the parameter must be called once for
           each value.
         :return:
         """
 
     @POST(API_SETTINGS_RESET_ENDPOINT)
-    def remove_setting_value(self, keys, component=None, branch=None, pullRequest=None):
+    def remove_setting_value(self, keys, component=None):
         """
+        SINCE 6.1
         Remove a setting value.
         The settings defined in conf/sonar.properties are read-only and can't be changed.
 
         :param keys: Comma-separated list of keys
         :param component: Component key
-        :param branch: Branch key
-        :param pullRequest: Pull request id
-
         :return:
         """
 
     @GET(API_SETTINGS_VALUES_ENDPOINT)
-    def get_settings_values(
-        self, component=None, branch=None, pullRequest=None, keys=None
-    ):
+    def get_settings_values(self, component=None, keys=None):
         """
+        SINCE 6.3
         List settings values.
         If no value has been set for a setting, then the default value is returned.
         The settings from conf/sonar.properties are excluded from results.
 
         :param component: Component key
-        :param branch: Branch key. Only available on following settings : sonar.leak.period
-        :param pullRequest: Pull request id. Only available on following settings : sonar.leak.period
         :param keys: List of setting keys
         :return:
         """
 
     @GET(API_SETTINGS_LIST_DEFINITIONS_ENDPOINT)
-    def get_settings_definitions(self, component=None, branch=None, pullRequest=None):
+    def get_settings_definitions(self, component=None):
         """
+        SINCE 6.3
         List settings definitions.
 
         :param component: Component key
-        :param branch: Branch key. Only available on following settings : sonar.leak.period
-        :param pullRequest: Pull request id. Only available on following settings : sonar.leak.period
-
         :return:
         """
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/cloud/webhooks.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/user_tokens.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,63 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-from sonarqube.community.webservices import SonarQubeWebservices
+from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
-    API_WEBHOOKS_CREATE_ENDPOINT,
-    API_WEBHOOKS_LIST_ENDPOINT,
+    API_USER_TOKENS_GENERATE_ENDPOINT,
+    API_USER_TOKENS_REVOKE_ENDPOINT,
+    API_USER_TOKENS_SEARCH_ENDPOINT,
 )
 from sonarqube.utils.common import GET, POST
 
 
-class SonarCloudWebhooks(SonarQubeWebservices):
+class SonarQubeUserTokens(RestClient):
     """
-    SonarCloud webhooks Operations
+    SonarQube user tokens Operations
     """
 
-    @POST(API_WEBHOOKS_CREATE_ENDPOINT)
-    def create_webhook(self, name, url, organization, project=None, secret=None):
+    def __init__(self, **kwargs):
         """
-        Create a Webhook.
 
-        :param name: Name displayed in the administration console of webhooks
-        :param url: Server endpoint that will receive the webhook payload, for example 'http://my_server/foo'. If HTTP
-          Basic authentication is used, HTTPS is recommended to avoid man in the middle attacks.
-          Example: 'https://myLogin:myPassword@my_server/foo'
-        :param organization: organization key.
-        :param project: The key of the project that will own the webhook
-        :param secret: If provided, secret will be used as the key to generate the HMAC hex (lowercase) digest value
-          in the 'X-Sonar-Webhook-HMAC-SHA256' header
+        :param kwargs:
+        """
+        super(SonarQubeUserTokens, self).__init__(**kwargs)
+
+    @POST(API_USER_TOKENS_GENERATE_ENDPOINT)
+    def generate_user_token(self, name, login=None):
+        """
+        SINCE 5.3
+        Generate a user access token.
+        Please keep your tokens secret. They enable to authenticate and analyze projects.
+        It requires administration permissions to specify a 'login' and generate a token for another user. Otherwise,
+        a token is generated for the current user.
+
+        :param name: Token name
+        :param login: User login. If not set, the token is generated for the authenticated user.
         :return: request response
         """
 
-    @GET(API_WEBHOOKS_LIST_ENDPOINT)
-    def search_webhooks(self, organization, project=None):
+    @POST(API_USER_TOKENS_REVOKE_ENDPOINT)
+    def revoke_user_token(self, name, login=None):
+        """
+        SINCE 5.3
+        Revoke a user access token.
+        It requires administration permissions to specify a 'login' and revoke a token for another user.
+        Otherwise, the token for the current user is revoked.
+
+        :param name: Token name
+        :param login: User login
+        :return:
+        """
+
+    @GET(API_USER_TOKENS_SEARCH_ENDPOINT)
+    def search_user_tokens(self, login=None):
         """
-        Search for global webhooks or project webhooks. Webhooks are ordered by name.
+        SINCE 5.3
+        List the access tokens of a user.
+        The login must exist and active.
+        Field 'lastConnectionDate' is only updated every hour, so it may not be accurate,
+        for instance when a user is using a token many times in less than one hour.
 
-        :param organization: organization key.
-        :param project: Project key
+        :param login: User login
         :return:
         """
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/alm_integrations.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/alm_integrations.py`

 * *Files 9% similar despite different names*

```diff
@@ -79,22 +79,24 @@
         :param almSetting: ALM setting key
         :param projectName: Project name filter
         :param repositoryName: Repository name filter
         :return:
         """
 
     @GET(API_ALM_INTEGRATION_SEARCH_BITBUCKETCLOUD_REPOS)
-    def search_bitbucketserver_repos(self, almSetting, repositoryName=None):
+    def search_bitbucketserver_repos(self, almSetting, repositoryName=None, p=None, ps=None):
         """
         since 9.0
         Search the Bitbucket Cloud repositories
         Requires the 'Create Projects' permission
 
         :param almSetting: ALM setting key
         :param repositoryName: Repository name filter
+        :param p: page number.
+        :param ps: Page size. Must be greater than 0 and less or equal than 100
         :return:
         """
 
     @GET(API_ALM_INTEGRATION_SEARCH_GITLAB_REPOS)
     def search_gitlab_repos(self, almSetting, p=None, projectName=None, ps=None):
         """
         since 8.5
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/alm_settings.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/alm_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from sonarqube.utils.common import GET, POST
 from sonarqube.utils.rest_client import RestClient
 
 from sonarqube.utils.config import (
     API_ALM_SETTINGS_VALIDATE,
-    API_ALM_SETTINGS_VALIDATE_BINDING,
     API_ALM_SETTINGS_UPDATE_GITLAB,
     API_ALM_SETTINGS_UPDATE_GITHUB,
     API_ALM_SETTINGS_UPDATE_BITBUCKET,
     API_ALM_SETTINGS_UPDATE_BITBUCKETCLOUD,
     API_ALM_SETTINGS_UPDATE_AZURE,
-    API_ALM_SETTINGS_SET_GITLAB_BINDING,
-    API_ALM_SETTINGS_SET_GITHUB_BINDING,
-    API_ALM_SETTINGS_SET_BITBUCKET_BINDING,
-    API_ALM_SETTINGS_SET_BITBUCKETCLOUD_BINDING,
-    API_ALM_SETTINGS_SET_AZURE_BINDING,
     API_ALM_SETTINGS_LIST_DEFINITIONS,
     API_ALM_SETTINGS_LIST,
     API_ALM_SETTINGS_DELETE,
     API_ALM_SETTINGS_GET_BINDING,
-    API_ALM_SETTINGS_DELETE_BINDING,
     API_ALM_SETTINGS_CREATE_GITLAB,
     API_ALM_SETTINGS_CREATE_GITHUB,
     API_ALM_SETTINGS_CREATE_BITBUCKET,
     API_ALM_SETTINGS_CREATE_BITBUCKETCLOUD,
     API_ALM_SETTINGS_CREATE_AZURE,
-    API_ALM_SETTINGS_COUNT_BINDING
+    API_ALM_SETTINGS_COUNT_BINDING,
+    API_ALM_SETTINGS_VALIDATE_BINDING,
+    API_ALM_SETTINGS_SET_GITLAB_BINDING,  # pro
+    API_ALM_SETTINGS_SET_GITHUB_BINDING,  # pro
+    API_ALM_SETTINGS_SET_BITBUCKET_BINDING,  # pro
+    API_ALM_SETTINGS_SET_BITBUCKETCLOUD_BINDING,  # pro
+    API_ALM_SETTINGS_SET_AZURE_BINDING,  # pro
+    API_ALM_SETTINGS_DELETE_BINDING,  # pro
 )
 
 
 class SonarQubeAlmSettings(RestClient):
 
     def __init__(self, **kwargs):
         """
@@ -141,25 +141,14 @@
         Get ALM binding of a given project.
         Requires the 'Administer' permission on the project
 
         :param project: Project key
         :return:
         """
 
-    @POST(API_ALM_SETTINGS_DELETE_BINDING)
-    def delete_binding(self, project):
-        """
-        since 8.1
-        Delete the ALM setting binding of a project.
-        Requires the 'Administer' permission on the project
-
-        :param project: Project key
-        :return:
-        """
-
     @GET(API_ALM_SETTINGS_LIST)
     def list(self, project=None):
         """
         since 8.1
         List ALM setting available for a given project, sorted by ALM key
         Requires the 'Administer project' permission if the 'project' parameter is provided,
         requires the 'Create Projects' permission otherwise.
@@ -174,92 +163,14 @@
         since 8.1
         List ALM Settings, sorted by created date.
         Requires the 'Administer System' permission
 
         :return:
         """
 
-    @POST(API_ALM_SETTINGS_SET_AZURE_BINDING)
-    def set_azure_binding(self, almSetting, project, projectName, repositoryName, monorepo="false"):
-        """
-        since 8.1
-        Bind a Azure DevOps ALM instance to a project.
-        If the project was already bound to a previous Azure DevOps ALM instance,
-        the binding will be updated to the new one.Requires the 'Administer' permission on the project
-
-        :param almSetting: Azure ALM setting key
-        :param project: SonarQube project key
-        :param projectName: Azure project name
-        :param repositoryName: Azure repository name
-        :param monorepo: Is this project part of a monorepo (since 8.7)
-        :return:
-        """
-
-    @POST(API_ALM_SETTINGS_SET_BITBUCKET_BINDING)
-    def set_bitbucket_binding(self, almSetting, project, repository, slug, monorepo="false"):
-        """
-        since 8.1
-        Bind a Bitbucket ALM instance to a project.
-        If the project was already bound to a previous Bitbucket ALM instance,
-        the binding will be updated to the new one.Requires the 'Administer' permission on the project
-
-        :param almSetting: Bitbucket ALM setting key
-        :param project: Project key
-        :param repository: Bitbucket repository key
-        :param slug: Bitbucket repository slug
-        :param monorepo: Is this project part of a monorepo (since 8.7)
-        :return:
-        """
-
-    @POST(API_ALM_SETTINGS_SET_BITBUCKETCLOUD_BINDING)
-    def set_bitbucketcloud_binding(self, almSetting, project, repository, monorepo="false"):
-        """
-        since 8.7
-        Bind a Bitbucket Cloud setting to a project.
-        If the project was already bound to a previous Bitbucket Cloud setting,
-        the binding will be updated to the new one.Requires the 'Administer' permission on the project
-
-        :param almSetting: Bitbucket ALM setting key
-        :param project: Project key
-        :param repository: Bitbucket Cloud repository key
-        :param monorepo: Is this project part of a monorepo
-        :return:
-        """
-
-    @POST(API_ALM_SETTINGS_SET_GITHUB_BINDING)
-    def set_github_binding(self, almSetting, project, repository, summaryCommentEnabled="true", monorepo="false"):
-        """
-        since 8.1
-        Bind a GitHub ALM instance to a project.
-        If the project was already bound to a previous GitHub ALM instance,
-        the binding will be updated to the new one.Requires the 'Administer' permission on the project
-
-        :param almSetting: GitHub ALM setting key
-        :param project: Project key
-        :param repository: GitHub Repository
-        :param summaryCommentEnabled: Enable/disable summary in PR discussion tab
-        :param monorepo: Is this project part of a monorepo (since 8.7)
-        :return:
-        """
-
-    @POST(API_ALM_SETTINGS_SET_GITLAB_BINDING)
-    def set_gitlab_binding(self, almSetting, project, repository, monorepo="false"):
-        """
-        since 8.1
-        Bind a GitLab instance to a project.
-        If the project was already bound to a previous Gitlab ALM instance,
-        the binding will be updated to the new one.Requires the 'Administer' permission on the project
-
-        :param almSetting: GitLab ALM setting key
-        :param project: Project key
-        :param repository: GitLab project ID
-        :param monorepo: Is this project part of a monorepo (since 8.7)
-        :return:
-        """
-
     @POST(API_ALM_SETTINGS_UPDATE_AZURE)
     def update_azure(self, key, personalAccessToken, url, newKey=None):
         """
         since 8.1
         Update Azure ALM instance Setting.
         Requires the 'Administer System' permission
 
@@ -337,18 +248,107 @@
         Validate an ALM Setting by checking connectivity and permissions
         Requires the 'Administer System' permission
 
         :param key: Unique key of the ALM settings
         :return:
         """
 
+    @POST(API_ALM_SETTINGS_SET_GITLAB_BINDING)
+    def set_gitlab_binding(self, almSetting, project, repository, monorepo="false"):
+        """
+        since 8.1
+        Bind a GitLab instance to a project.
+        If the project was already bound to a previous Gitlab ALM instance,
+        the binding will be updated to the new one.Requires the 'Administer' permission on the project
+
+        :param almSetting: GitLab ALM setting key
+        :param project: Project key
+        :param repository: GitLab project ID
+        :param monorepo: Is this project part of a monorepo (since 8.7)
+        :return:
+        """
+
+    @POST(API_ALM_SETTINGS_SET_GITHUB_BINDING)
+    def set_github_binding(self, almSetting, project, repository, summaryCommentEnabled="true", monorepo="false"):
+        """
+        since 8.1
+        Bind a GitHub ALM instance to a project.
+        If the project was already bound to a previous GitHub ALM instance,
+        the binding will be updated to the new one.Requires the 'Administer' permission on the project
+
+        :param almSetting: GitHub ALM setting key
+        :param project: Project key
+        :param repository: GitHub Repository
+        :param summaryCommentEnabled: Enable/disable summary in PR discussion tab
+        :param monorepo: Is this project part of a monorepo (since 8.7)
+        :return:
+        """
+
+    @POST(API_ALM_SETTINGS_SET_BITBUCKET_BINDING)
+    def set_bitbucket_binding(self, almSetting, project, repository, slug, monorepo="false"):
+        """
+        since 8.1
+        Bind a Bitbucket ALM instance to a project.
+        If the project was already bound to a previous Bitbucket ALM instance,
+        the binding will be updated to the new one.Requires the 'Administer' permission on the project
+
+        :param almSetting: Bitbucket ALM setting key
+        :param project: Project key
+        :param repository: Bitbucket repository key
+        :param slug: Bitbucket repository slug
+        :param monorepo: Is this project part of a monorepo (since 8.7)
+        :return:
+        """
+
+    @POST(API_ALM_SETTINGS_SET_BITBUCKETCLOUD_BINDING)
+    def set_bitbucketcloud_binding(self, almSetting, project, repository, monorepo="false"):
+        """
+        since 8.7
+        Bind a Bitbucket Cloud setting to a project.
+        If the project was already bound to a previous Bitbucket Cloud setting,
+        the binding will be updated to the new one.Requires the 'Administer' permission on the project
+
+        :param almSetting: Bitbucket ALM setting key
+        :param project: Project key
+        :param repository: Bitbucket Cloud repository key
+        :param monorepo: Is this project part of a monorepo
+        :return:
+        """
+
+    @POST(API_ALM_SETTINGS_SET_AZURE_BINDING)
+    def set_azure_binding(self, almSetting, project, projectName, repositoryName, monorepo="false"):
+        """
+        since 8.1
+        Bind a Azure DevOps ALM instance to a project.
+        If the project was already bound to a previous Azure DevOps ALM instance,
+        the binding will be updated to the new one.Requires the 'Administer' permission on the project
+
+        :param almSetting: Azure ALM setting key
+        :param project: SonarQube project key
+        :param projectName: Azure project name
+        :param repositoryName: Azure repository name
+        :param monorepo: Is this project part of a monorepo (since 8.7)
+        :return:
+        """
+
+    @POST(API_ALM_SETTINGS_DELETE_BINDING)
+    def delete_binding(self, project):
+        """
+        since 8.1
+        Delete the ALM setting binding of a project.
+        Requires the 'Administer' permission on the project
+
+        :param project: Project key
+        :return:
+        """
+
     @GET(API_ALM_SETTINGS_VALIDATE_BINDING)
     def validate_binding(self, project):
         """
         since 9.0
         Validate a project binding setting by checking connectivity and permissions
         Requires project 'Browse' permission
 
         :param project: Project key
         :raises ValidationError:
         :return:
-        """
+        """
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/auth.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/auth.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/ce.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/ce.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,32 +23,36 @@
         :param kwargs:
         """
         super(SonarQubeCe, self).__init__(**kwargs)
 
     @GET(API_CE_ACTIVITY_ENDPOINT)
     def search_tasks(
         self,
+        component=None,
         componentId=None,
         maxExecutedAt=None,
         minSubmittedAt=None,
         onlyCurrents=None,
+        p=None,
         ps=None,
         q=None,
         status=None,
         type=None,
     ):
         """
         SINCE 5.2
         Search for tasks.
 
+        :param component: Key of the component (project) to filter on
         :param componentId: Id of the component (project) to filter on
         :param maxExecutedAt: Maximum date of end of task processing (inclusive)
         :param minSubmittedAt: Minimum date of task submission (inclusive)
         :param onlyCurrents: Filter on the last tasks (only the most recent finished task by project).
           default value is false.
+        :param p: page number.
         :param ps: Page size. Must be greater than 0 and less or equal than 1000
         :param q: Limit search to:
 
           * component names that contain the supplied string
           * component keys that are exactly the same as the supplied string
           * task ids that are exactly the same as the supplied string
 
@@ -70,20 +74,20 @@
           * PROJECT_IMPORT
           * VIEW_REFRESH
 
         :return:
         """
 
     @GET(API_CE_ACTIVITY_STATUS_ENDPOINT)
-    def get_ce_activity_related_metrics(self, component_id=None):
+    def get_ce_activity_related_metrics(self, componentId=None):
         """
         SINCE 5.5
         Returns CE activity related metrics.
 
-        :param component_id: Id of the component (project) to filter on
+        :param componentId: Id of the component (project) to filter on
         :return:
         """
 
     @GET(API_CE_ANALYSIS_STATUS_ENDPOINT)
     def get_ce_analysis_status(self, component, branch=None, pullRequest=None):
         """
         Get last analysis status including warnings of a given component (usually a project).
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/components.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/components.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,28 +34,28 @@
         :param component: Component key
         :param branch: Branch key.
         :param pullRequest: Pull request id
         :return:
         """
 
     @GET(API_COMPONTENTS_SEARCH_ENDPOINT)
-    def search_components(self, qualifiers, language=None, q=None, p=None, ps=None):
+    def search_components(self, qualifiers, organization=None, language=None, q=None, p=None, ps=None):
         """
         SINCE 6.3
         Search for components
 
         :param qualifiers: Comma-separated list of component qualifiers. Filter the results with
           the specified qualifiers. Possible values are:
 
           * BRC - Sub-projects
           * DIR - Directories
           * FIL - Files
           * TRK - Projects
           * UTS - Test Files
-
+        :param organization: Organization key
         :param language: Language key. If provided, only components for the given language are returned.
         :param q: Limit search to:
 
           * component names that contain the supplied string
           * component keys that are exactly the same as the supplied string
         :param p: page number.
         :param ps: Page size. Must be greater than 0 and less or equal than 500
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/duplications.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/duplications.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/favorites.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/favorites.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/hotspots.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/hotspots.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
     API_HOTSPOTS_SHOW_ENDPOINT,
     API_HOTSPOTS_SEARCH_ENDPOINT,
+    API_HOTSPOTS_CHANGE_STATUS_ENDPOINT  # pro
 )
-from sonarqube.utils.common import GET
+from sonarqube.utils.common import GET, POST
 
 
 class SonarQubeHotspots(RestClient):
     """
     SonarQube Security Hotspots Operations
     """
 
@@ -84,7 +85,21 @@
         """
         SINCE 8.1
         Provides the details of a Security Hotspot.
 
         :param hotspot: Key of the Security Hotspot
         :return:
         """
+
+    @POST(API_HOTSPOTS_CHANGE_STATUS_ENDPOINT)
+    def change_hotspots_status(self, hotspot, status, comment=None, resolution=None):
+        """
+        since 8.1
+        Change the status of a Security Hotpot.
+        Requires the 'Administer Security Hotspot' permission.
+
+        :param hotspot: Key of the Security Hotspot
+        :param status: New status of the Security Hotspot.
+        :param comment: Comment text.
+        :param resolution: Resolution of the Security Hotspot when new status is REVIEWED, otherwise must not be set.
+        :return:
+        """
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/issues.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/issues.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         for issue in issues:
             if issue["key"] == key:
                 return issue
 
     @GET(API_ISSUES_SEARCH_ENDPOINT)
     def search_issues(
         self,
+        organization=None,
         componentKeys=None,
         branch=None,
         pullRequest=None,
         additionalFields=None,
         asc="true",
         assigned=None,
         assignees=None,
@@ -77,14 +78,15 @@
         tags=None,
         types=None,
     ):
         """
         SINCE 3.6
         Search for issues.
 
+        :param organization: Organization key
         :param componentKeys: Comma-separated list of component keys. Retrieve issues associated to a specific list of
             components (and all its descendants). A component can be a portfolio, project, module, directory or file.
         :param branch: Branch key.
         :param pullRequest: Pull request id.
         :param additionalFields: Comma-separated list of the optional fields to be returned in response. Possible values are for:
 
             * _all
@@ -327,21 +329,22 @@
           * openasvulnerability
           * resetastoreview
 
         :return: request response
         """
 
     @GET(API_ISSUES_AUTHORS_ENDPOINT)
-    def search_scm_accounts(self, project, q=None):
+    def search_scm_accounts(self, project, q=None, ps=None):
         """
         SINCE 5.1
         Search SCM accounts which match a given query
 
         :param project: Project key
         :param q: Limit search to authors that contain the supplied string.
+        :param ps: Page size. Must be greater than 0 and less or equal than 100
         :return:
         """
 
     @POST(API_ISSUES_BULK_CHANGE_ENDPOINT)
     def issues_bulk_change(
         self,
         issues,
@@ -417,16 +420,17 @@
         :param issue: Issue key
         :param tags: Comma-separated list of tags. All tags are removed if parameter is empty or not set.
           such as: security,cwe,misra-c
         :return: request response
         """
 
     @GET(API_ISSUES_TAGS_ENDPOINT)
-    def get_issues_tags(self, project, q=None):
+    def get_issues_tags(self, project, q=None, ps=None):
         """
         SINCE 5.1
         List tags
 
         :param project:
         :param q: Limit search to tags that contain the supplied string.
+        :param ps: Page size.
         :return:
         """
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/languages.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/languages.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/measures.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/measures.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/metrics.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/metrics.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/monitoring.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/monitoring.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/new_code_periods.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/new_code_periods.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/notifications.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/notifications.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/plugins.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/plugins.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/project_analyses.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/project_analyses.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/project_badges.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/project_badges.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         """
 
         :param kwargs:
         """
         super(SonarQubeProjectBadges, self).__init__(**kwargs)
 
     @GET(API_PROJECT_BADGES_MEASURE_ENDPOINT)
-    def generate_badge_for_project_measures(self, project, metric, branch=None):
+    def generate_badge_for_project_measures(self, project, metric, branch=None, token=None):
         """
         SINCE 7.1
         Generate badge for project's measure as an SVG.
 
         :param project: Project or application key
         :param branch: Long living branch key
         :param metric: Metric key,
@@ -40,25 +40,27 @@
             * ncloc
             * sqale_rating
             * alert_status
             * reliability_rating
             * security_rating
             * sqale_index
             * vulnerabilities
+        :param token: Security token
         :return:
         """
 
     @GET(API_PROJECT_BADGES_QUALITY_GATE_ENDPOINT)
-    def generate_badge_for_project_quality_gate(self, project, branch=None):
+    def generate_badge_for_project_quality_gate(self, project, branch=None, token=None):
         """
         SINCE 7.1
         Generate badge for project's quality gate as an SVG.
 
         :param project: Project or application key
         :param branch: Long living branch key
+        :param token: Security token
         :return:
         """
 
     @POST(API_PROJECT_BADGES_RENEW_TOKEN_ENDPOINT)
     def generate_new_token_for_project_badge_access(self, project):
         """
         SINCE 9.2
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/project_branches.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/project_branches.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/project_dump.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/project_dump.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
     API_PROJECT_DUMP_EXPORT_ENDPOINT,
-    API_PROJECT_DUMP_IMPORT_ENDPOINT,
+    API_PROJECT_DUMP_IMPORT_ENDPOINT  # pro
 )
 from sonarqube.utils.common import POST
 
 
-class SonarQubeProjectdump(RestClient):
+class SonarQubeProjectDump(RestClient):
     """
     SonarQube Project export/import Operations
     """
 
     def __init__(self, **kwargs):
         """
 
         :param kwargs:
         """
-        super(SonarQubeProjectdump, self).__init__(**kwargs)
+        super(SonarQubeProjectDump, self).__init__(**kwargs)
 
     @POST(API_PROJECT_DUMP_EXPORT_ENDPOINT)
     def export_project_dump(self, key):
         """
         SINCE 1.0
         Triggers project dump so that the project can be copied to another SonarQube server (see api/project_dump/import).
 
@@ -35,8 +35,8 @@
     def import_project_dump(self, key):
         """
         SINCE 1.0
         Triggers the import of a project dump.
 
         :param key:
         :return:
-        """
+        """
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/project_links.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/project_links.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/project_pull_requests.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/project_pull_requests.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
-    API_PROJECT_PULL_REQUESTS_DELETE_ENDPOINT,
-    API_PROJECT_PULL_REQUESTS_LIST_ENDPOINT,
+    API_PROJECT_PULL_REQUESTS_DELETE_ENDPOINT,  # pro
+    API_PROJECT_PULL_REQUESTS_LIST_ENDPOINT,  # pro
 )
 from sonarqube.utils.common import GET, POST
 
 
 class SonarQubeProjectPullRequests(RestClient):
     """
     SonarQube project pull requests Operations
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/project_tags.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/project_tags.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,20 +18,22 @@
         """
 
         :param kwargs:
         """
         super(SonarQubeProjectTags, self).__init__(**kwargs)
 
     @GET(API_PROJECT_TAGS_SEARCH_ENDPOINT)
-    def search_project_tags(self, q=None):
+    def search_project_tags(self, q=None, ps=None, p=None):
         """
         SINCE 6.4
         Search tags
 
         :param q: Limit search to tags that contain the supplied string.
+        :param p: page number.
+        :param ps: Page size. Must be greater than 0 and less or equal than 100
         :return:
         """
 
     @POST(API_PROJECT_TAGS_SET_ENDPOINT)
     def set_project_tags(self, project, tags):
         """
         SINCE 6.4
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/projects.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/projects.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     API_PROJECTS_BULK_DELETE_ENDPOINT,
     API_PROJECTS_SEARCH_ENDPOINT,
     API_PROJECTS_CREATE_ENDPOINT,
     API_PROJECTS_DELETE_ENDPOINT,
     API_PROJECTS_UPDATE_VISIBILITY_ENDPOINT,
     API_PROJECTS_UPDATE_KEY_ENDPOINT,
     API_PROJECTS_UPDATE_DEFAULT_VISIBILITY_ENDPOINT,
-    API_PROJECTS_EXPORT_FINDINGS_ENDPOINT,
-    API_PROJECTS_LICENSE_USAGE_ENDPOINT
+    API_PROJECTS_EXPORT_FINDINGS_ENDPOINT,  # pro
+    API_PROJECTS_LICENSE_USAGE_ENDPOINT  # pro
 )
 from sonarqube.utils.common import GET, POST
 
 
 class SonarQubeProjects(RestClient):
     """
     SonarQube projects Operations
@@ -37,26 +37,28 @@
         for project in projects:
             if project["key"] == key:
                 return project
 
     @GET(API_PROJECTS_SEARCH_ENDPOINT)
     def search_projects(
         self,
+        organization=None,
         analyzedBefore=None,
         onProvisionedOnly="false",
         projects=None,
         p=None,
         ps=None,
         q=None,
         qualifiers="TRK",
     ):
         """
         SINCE 6.3
         Search for projects or views to administrate them.
 
+        :param organization: The key of the organization
         :param analyzedBefore: Filter the projects for which last analysis is older than the given date (exclusive).
           Either a date (server timezone) or datetime can be provided.
         :param onProvisionedOnly: Filter the projects that are provisioned.
           Possible values are for: true or false. default value is false.
         :param projects: Comma-separated list of project keys
         :param p: page number.
         :param ps: Page size. Must be greater than 0 and less or equal than 500
@@ -71,21 +73,22 @@
             * APP
           default value is TRK.
 
         :return:
         """
 
     @POST(API_PROJECTS_CREATE_ENDPOINT)
-    def create_project(self, project, name, visibility=None):
+    def create_project(self, project, name, organization=None, visibility=None):
         """
         SINCE 4.0
         Create a project.
 
         :param project: Key of the project
         :param name: Name of the project. If name is longer than 500, it is abbreviated.
+        :param organization: The key of the organization
         :param visibility: Whether the created project should be visible to everyone, or only specific user/groups.
           If no visibility is specified, the default project visibility of the organization will be used.
           Possible values are for:
             * private
             * public
         :return: request response
         """
@@ -99,25 +102,27 @@
         :param project: Project key
         :return:
         """
 
     @POST(API_PROJECTS_BULK_DELETE_ENDPOINT)
     def bulk_delete_projects(
         self,
+        organization=None,
         analyzedBefore=None,
         onProvisionedOnly="false",
         projects=None,
         q=None,
         qualifiers="TRK",
     ):
         """
         SINCE 5.2
         Delete one or several projects.
         At least one parameter is required among analyzedBefore, projects, projectIds (deprecated since 6.4) and q
 
+        :param organization: The key of the organization
         :param analyzedBefore: Filter the projects for which last analysis is older than the given date (exclusive).
           Either a date (server timezone) or datetime can be provided.
         :param onProvisionedOnly: Filter the projects that are provisioned.
           Possible values are for: true or false. default value is false.
         :param projects: Comma-separated list of project keys
         :param q:
           Limit to:
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/qualityprofiles.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/qualityprofiles.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             # Note: sort by key to allow checking easily
             params = ";".join(
                 "{}={}".format(k, v) for k, v in sorted(params.items()) if v
             )
             if params:
                 data["params"] = params
 
-        return self._post(API_QUALITYPROFILES_ACTIVATE_RULE_ENDPOINT, params=data)
+        return self._post(API_QUALITYPROFILES_ACTIVATE_RULE_ENDPOINT, data=data)
 
     @POST(API_QUALITYPROFILES_ADD_GROUP_ENDPOINT)
     def add_group_to_quality_profile(self, group, language, qualityProfile):
         """
         SINCE 6.6
         Allow a group of users to edit a Quality Profile.
 
@@ -87,101 +87,108 @@
         :param language: Quality profile language
         :param qualityProfile: Quality Profile name
         :return:
         """
 
     @GET(API_QUALITYPROFILES_SEARCH_ENDPOINT)
     def search_quality_profiles(
-        self, defaults="false", language=None, project=None, qualityProfile=None
+        self, organization=None, defaults="false", language=None, project=None, qualityProfile=None
     ):
         """
         SINCE 5.2
         Search quality profiles
 
+        :param organization: organization key.
         :param defaults: If set to true, return only the quality profiles marked as default for each language.
           Possible values are for: true or false. default value is false.
         :param language: Language key. If provided, only profiles for the given language are returned.
         :param project: Project key
         :param qualityProfile: Quality profile name
         :return:
         """
 
     @POST(API_QUALITYPROFILES_SET_DEFAULT_ENDPOINT)
-    def set_default_quality_profile(self, language, qualityProfile):
+    def set_default_quality_profile(self, language, qualityProfile, organization=None):
         """
         SINCE 5.2
         Select the default profile for a given language.
 
         :param language: Quality profile language.
         :param qualityProfile: Quality profile name.
+        :param organization: organization key.
         :return:
         """
 
     @POST(API_QUALITYPROFILES_ADD_PROJECT_ENDPOINT)
-    def associate_project_with_quality_profile(self, project, language, qualityProfile):
+    def associate_project_with_quality_profile(self, project, language, qualityProfile, organization=None):
         """
         SINCE 5.2
         Associate a project with a quality profile.
 
         :param project: Project key.
         :param language: Quality profile language.
         :param qualityProfile: Quality profile name.
+        :param organization: organization key.
         :return:
         """
 
     @POST(API_QUALITYPROFILES_REMOVE_PROJECT_ENDPOINT)
     def remove_project_associate_with_quality_profile(
-        self, project, language, qualityProfile
+        self, project, language, qualityProfile, organization=None
     ):
         """
         SINCE 5.2
         Remove a project's association with a quality profile.
 
         :param project: Project key
         :param language: Quality profile language.
         :param qualityProfile: Quality profile name.
+        :param organization: Organization key.
         :return:
         """
 
     @GET(API_QUALITYPROFILES_BACKUP_ENDPOINT)
-    def backup_quality_profile(self, language, qualityProfile):
+    def backup_quality_profile(self, language, qualityProfile, organization=None):
         """
         SINCE 5.2
         Backup a quality profile in XML form. The exported profile can be restored through api/qualityprofiles/restore.
 
         :param language: Quality profile language.
         :param qualityProfile: Quality profile name.
+        :param organization: organization key.
         :return:
         """
 
     @POST(API_QUALITYPROFILES_CHANGE_PARENT_ENDPOINT)
     def change_parent_of_quality_profile(
-        self, parentQualityProfile, language, qualityProfile
+        self, parentQualityProfile, language, qualityProfile, organization=None
     ):
         """
         SINCE 5.2
         Change a quality profile's parent.
 
         :param parentQualityProfile: Parent quality profile name.
         :param language: Quality profile language.
         :param qualityProfile: Quality profile name.
+        :param organization: organization key.
         :return:
         """
 
     @GET(API_QUALITYPROFILES_CHANGELOG_ENDPOINT)
     def get_history_of_changes_on_quality_profile(
-        self, language, qualityProfile, since=None, to=None, p=None, ps=None
+        self, language, qualityProfile, organization=None, since=None, to=None, p=None, ps=None
     ):
         """
         SINCE 5.2
         Get the history of changes on a quality profile: rule activation/deactivation, change in parameters/severity.
         Events are ordered by date in descending order (most recent first).
 
         :param language: Quality profile language.
         :param qualityProfile: Quality profile language.
+        :param organization: organization key.
         :param since: Start date for the changelog. Either a date (server timezone) or datetime can be provided.
         :param to: End date for the changelog. Either a date (server timezone) or datetime can be provided.
         :param p: page number.
         :param ps: Page size. Must be greater than 0 and less or equal than 500
         :return:
         """
 
@@ -193,21 +200,22 @@
 
         :param fromKey: Quality profile key
         :param toName: Name for the new quality profile.
         :return: request response
         """
 
     @POST(API_QUALITYPROFILES_CREATE_ENDPOINT)
-    def create_quality_profile(self, language, name):
+    def create_quality_profile(self, language, name, organization=None):
         """
         SINCE 5.2
         Create a quality profile.
 
         :param language: Quality profile language
         :param name: Quality profile name
+        :param organization: organization key.
         :return: request response
         """
 
     @POST(API_QUALITYPROFILES_DEACTIVATE_RULE_ENDPOINT)
     def deactivate_rule_on_quality_profile(self, key, rule):
         """
         SINCE 4.4
@@ -215,28 +223,29 @@
 
         :param key: Quality Profile key. Can be obtained through api/qualityprofiles/search
         :param rule: Rule key
         :return:
         """
 
     @POST(API_QUALITYPROFILES_DELETE_ENDPOINT)
-    def delete_quality_profile(self, language, qualityProfile):
+    def delete_quality_profile(self, language, qualityProfile, organization=None):
         """
         SINCE 5.2
         Delete a quality profile and all its descendants.
         The default quality profile cannot be deleted.
 
         :param language: Quality profile language.
         :param qualityProfile: Quality profile name.
+        :param organization: Organization key.
         :return:
         """
 
     @GET(API_QUALITYPROFILES_EXPORT_ENDPOINT)
     def export_quality_profile(
-        self, exporterKey=None, language=None, qualityProfile=None
+        self, exporterKey=None, language=None, qualityProfile=None, organization=None
     ):
         """
         SINCE 5.2
         Export a quality profile.
 
         :param exporterKey: Output format. If left empty, the same format as api/qualityprofiles/backup is used.
           Possible values are described by api/qualityprofiles/exporters.
@@ -246,14 +255,15 @@
             * pmd
             * sonarlint-vs-cs
             * roslyn-vbnet
             * roslyn-cs
         :param language: Quality profile language
         :param qualityProfile: Quality profile name to export. If left empty, the default profile for the language
         is exported.
+        :param organization: Organization key.
         :return:
         """
 
     @GET(API_QUALITYPROFILES_EXPORTERS_ENDPOINT)
     def get_supported_exporters(self):
         """
         SINCE 5.2
@@ -268,21 +278,22 @@
         SINCE 5.2
         List supported importers.
 
         :return:
         """
 
     @GET(API_QUALITYPROFILES_INHERITANCE_ENDPOINT)
-    def show_quality_profile(self, language, qualityProfile):
+    def show_quality_profile(self, language, qualityProfile, organization=None):
         """
         SINCE 5.2
         Show a quality profile's ancestors and children.
 
         :param language: Quality profile language.
         :param qualityProfile: Quality profile name.
+        :param organization: Organization key.
         :return:
         """
 
     @GET(API_QUALITYPROFILES_PROJECTS_ENDPOINT)
     def get_projects_associate_with_quality_profile(
         self, key, q=None, selected="selected", p=None, ps=None
     ):
@@ -311,19 +322,25 @@
         Rename a quality profile.
 
         :param key: Quality profile key
         :param name: New quality profile name
         :return:
         """
 
-    def restore_quality_profile(self, backup):
+    def restore_quality_profile(self, backup, organization=None):
         """
         SINCE 5.2
         Restore a quality profile using an XML file. The restored profile name is taken from the backup file,
         so if a profile with the same name and language already exists, it will be overwritten.
 
         :param backup: A profile backup file in XML format, as generated by api/qualityprofiles/backup
           or the former api/profiles/backup.
         :return:
         """
+        if organization is None:
+            data = {"organization": organization}
+        else:
+            data = None
+
         files = {'backup': backup}
-        return self._post(API_QUALITYPROFILES_RESTORE_ENDPOINT, files=files)
+
+        return self._post(API_QUALITYPROFILES_RESTORE_ENDPOINT, data=data, files=files)
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/server.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/server.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/sources.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/sources.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/system.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/system.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/user_groups.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/user_groups.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,96 +31,104 @@
         groups = result.get("groups", [])
 
         for group in groups:
             if group["name"] == name:
                 return group
 
     @GET(API_USER_GROUPS_SEARCH_ENDPOINT)
-    def search_user_groups(self, f=None, q=None, p=None, ps=None):
+    def search_user_groups(self, organization=None, f=None, managed=None, q=None, p=None, ps=None):
         """
         SINCE 5.2
         Search for user groups.
 
+        :param organization: organization key.
         :param f: Comma-separated list of the fields to be returned in response.
           All the fields are returned by default. Possible values are for:
             * name
             * description
             * membersCount
+        :param managed: Return managed or non-managed groups.
+          Only available for managed instances, throws for non-managed instances. (since 10.0)
         :param p: page number.
         :param ps: Page size. Must be greater than 0 and less or equal than 500
         :param q: Limit search to names that contain the supplied string.
         :return:
         """
 
     @POST(API_USER_GROUPS_CREATE_ENDPOINT)
-    def create_group(self, name, description=None):
+    def create_group(self, name, organization=None, description=None):
         """
         SINCE 5.2
         Create a group.
 
         :param name: Name for the new group. A group name cannot be larger than 255 characters and must be unique.
           The value 'anyone' (whatever the case) is reserved and cannot be used.
+        :param organization: organization key.
         :param description: Description for the new group. A group description cannot be larger than 200 characters.
         :return: request response
         """
 
     @POST(API_USER_GROUPS_DELETE_ENDPOINT)
-    def delete_group(self, name):
+    def delete_group(self, name, organization=None):
         """
         SINCE 5.2
         Delete a group. The default groups cannot be deleted.
 
         :param name: group name
+        :param organization: organization key.
         :return:
         """
 
     @POST(API_USER_GROUPS_UPDATE_ENDPOINT)
-    def update_group(self, id, name=None, description=None):
+    def update_group(self, currentName, name=None, description=None):
         """
         SINCE 5.2
         Update a group.
 
-        :param id: Identifier of the group.
+        :param currentName: Name of the group to be updated. (since 8.5)
         :param name: New optional name for the group. A group name cannot be larger than 255 characters and must
           be unique. Value 'anyone' (whatever the case) is reserved and cannot be used. If value is empty or not
           defined, then name is not changed.
         :param description: New optional description for the group. A group description cannot be larger than
           200 characters. If value is not defined, then description is not changed.
         :return:
         """
 
     @POST(API_USER_GROUPS_ADD_USER_ENDPOINT)
-    def add_user_to_group(self, name, login):
+    def add_user_to_group(self, name, login, organization=None):
         """
         SINCE 5.2
         Add a user to a group.
 
         :param name: Group name
+        :param organization: organization key.
         :param login: User login
         :return:
         """
 
     @POST(API_USER_GROUPS_REMOVE_USER_ENDPOINT)
-    def remove_user_from_group(self, name, login):
+    def remove_user_from_group(self, name, login, organization=None):
         """
         SINCE 5.2
         Remove a user from a group.
 
         :param name: Group name
         :param login: User login
+        :param organization: organization key.
         :return:
         """
 
     @GET(API_USER_GROUPS_USERS_ENDPOINT)
-    def search_users_belong_to_group(self, name, q=None, selected="selected", p=None, ps=None):
+    def search_users_belong_to_group(self, name, organization=None, q=None, selected="selected", p=None, ps=None):
         """
         SINCE 5.2
         Search for users with membership information with respect to a group.
 
         :param name: Group name
+        :param organization: organization key.
         :param q: Limit search to names or logins that contain the supplied string.
         :param selected: Depending on the value, show only selected items (selected=selected), deselected items
           (selected=deselected), or all items with their selection status (selected=all).Possible values are for:
             * all
             * deselected
             * selected
           default value is selected.
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/users.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/users.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,58 +13,60 @@
     API_USERS_UPDATE_LOGIN_ENDPOINT,
     API_USERS_DISMISS_SONARLINT_AD_ENDPOINT,
     API_USERS_UPDATE_IDENTITY_ENDPOINT
 )
 from sonarqube.utils.common import GET, POST
 
 
-class SonarQubeUsers(RestClient):
-    """
-    SonarQube users Operations
-    """
-
+class SonarQubeBaseUsers(RestClient):
     MAX_SEARCH_NUM = 200
 
     def __init__(self, **kwargs):
         """
 
         :param kwargs:
         """
-        super(SonarQubeUsers, self).__init__(**kwargs)
+        super(SonarQubeBaseUsers, self).__init__(**kwargs)
 
     def get(self, login):
         result = self.search_users(q=login)
         users = result.get("users", [])
 
         for user in users:
             if user["login"] == login:
                 return user
 
-    @POST(API_USERS_ANONYMIZE_ENDPOINT)
-    def anonymize_deactivated_user(self, login):
-        """
-        SINCE 9.7
-        Anonymize a deactivated user.
-
-        :param login: User login
-        :return: request response
-        """
-
     @GET(API_USERS_SEARCH_ENDPOINT)
     def search_users(self, q=None, p=None, ps=None):
         """
         SINCE 3.6
         Get a list of active users.
 
         :param q: Filter on login, name and email
         :param p: page number.
         :param ps: Page size. Must be greater than 0 and less or equal than 500
         :return:
         """
 
+
+class SonarQubeUsers(SonarQubeBaseUsers):
+    """
+    SonarQube users Operations
+    """
+
+    @POST(API_USERS_ANONYMIZE_ENDPOINT)
+    def anonymize_deactivated_user(self, login):
+        """
+        SINCE 9.7
+        Anonymize a deactivated user.
+
+        :param login: User login
+        :return: request response
+        """
+
     def create_user(
         self, login, name, email=None, password=None, local="true", scmAccount=None
     ):
         """
         SINCE 3.7
         Create a user.
 
@@ -124,29 +126,30 @@
         Deactivate a user.
 
         :param login: User login
         :return: request response
         """
 
     @GET(API_USERS_GROUPS_ENDPOINT)
-    def search_groups_user_belongs_to(self, login, q=None, selected="selected", p=None, ps=None):
+    def search_groups_user_belongs_to(self, login, q=None, selected="selected", p=None, ps=None, organization=None):
         """
         SINCE 5.2
         Lists the groups a user belongs to.
 
         :param login:
         :param q: Limit search to group names that contain the supplied string.
         :param selected: Depending on the value, show only selected items (selected=selected), deselected items
           (selected=deselected), or all items with their selection status (selected=all).Possible values are for:
             * all
             * deselected
             * selected
           default value is selected.
         :param p: page number.
         :param ps: Page size. Must be greater than 0 and less or equal than 500
+        :param organization: organization key.
         :return:
         """
 
     @POST(API_USERS_UPDATE_LOGIN_ENDPOINT)
     def update_user_login(self, login, newLogin):
         """
         SINCE 7.6
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/webhooks.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/webhooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,23 +22,24 @@
         """
 
         :param kwargs:
         """
         super(SonarQubeWebhooks, self).__init__(**kwargs)
 
     @POST(API_WEBHOOKS_CREATE_ENDPOINT)
-    def create_webhook(self, name, url, project=None, secret=None):
+    def create_webhook(self, name, url, organization=None, project=None, secret=None):
         """
         SINCE 7.1
         Create a Webhook.
 
         :param name: Name displayed in the administration console of webhooks
         :param url: Server endpoint that will receive the webhook payload, for example 'http://my_server/foo'. If HTTP
           Basic authentication is used, HTTPS is recommended to avoid man in the middle attacks.
           Example: 'https://myLogin:myPassword@my_server/foo'
+        :param organization: organization key.
         :param project: The key of the project that will own the webhook
         :param secret: If provided, secret will be used as the key to generate the HMAC hex (lowercase) digest value
           in the 'X-Sonar-Webhook-HMAC-SHA256' header
         :return: request response
         """
 
     @POST(API_WEBHOOKS_DELETE_ENDPOINT)
@@ -73,19 +74,20 @@
         Get a webhook delivery by its id.
 
         :param deliveryId: Id of delivery
         :return:
         """
 
     @GET(API_WEBHOOKS_LIST_ENDPOINT)
-    def search_webhooks(self, project=None):
+    def search_webhooks(self, organization=None, project=None):
         """
         SINCE 7.1
         Search for global webhooks or project webhooks. Webhooks are ordered by name.
 
+        :param organization: organization key.
         :param project: Project key
         :return:
         """
 
     @POST(API_WEBHOOKS_UPDATE_ENDPOINT)
     def update_webhook(self, webhook, name, url, secret=None):
         """
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/community/webservices.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/webservices.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/enterprise/applications.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/applications.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jacek Hojczak
 from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
-    API_APPLICATIONS_CREATE_ENDPOINT,
-    API_APPLICATIONS_DELETE_ENDPOINT,
-    API_APPLICATIONS_SHOW_ENDPOINT,
-    API_APPLICATIONS_UPDATE_ENDPOINT,
-    API_APPLICATIONS_ADD_PROJECT_ENDPOINT,
-    API_APPLICATIONS_REMOVE_PROJECT_ENDPOINT,
-    API_APPLICATIONS_CREATE_BRANCH_ENDPOINT,
-    API_APPLICATIONS_DELETE_BRANCH_ENDPOINT,
-    API_APPLICATIONS_SET_TAGS_ENDPOINT,
-    API_APPLICATIONS_UPDATE_BRANCH_ENDPOINT
+    API_APPLICATIONS_CREATE_ENDPOINT,  # pro
+    API_APPLICATIONS_DELETE_ENDPOINT,  # pro
+    API_APPLICATIONS_SHOW_ENDPOINT,  # pro
+    API_APPLICATIONS_UPDATE_ENDPOINT,  # pro
+    API_APPLICATIONS_ADD_PROJECT_ENDPOINT,  # pro
+    API_APPLICATIONS_REMOVE_PROJECT_ENDPOINT,  # pro
+    API_APPLICATIONS_CREATE_BRANCH_ENDPOINT,  # pro
+    API_APPLICATIONS_DELETE_BRANCH_ENDPOINT,  # pro
+    API_APPLICATIONS_SET_TAGS_ENDPOINT,  # pro
+    API_APPLICATIONS_UPDATE_BRANCH_ENDPOINT  # pro
 )
 from sonarqube.utils.common import POST, GET
 
 
 class SonarQubeApplications(RestClient):
     """
     SonarQube applications Operations
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/enterprise/audit_logs.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/audit_logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from sonarqube.utils.rest_client import RestClient
-from sonarqube.utils.config import API_AUDIT_LOGS_DOWNLOAD_ENDPOINT
+from sonarqube.utils.config import API_AUDIT_LOGS_DOWNLOAD_ENDPOINT  # pro
 from sonarqube.utils.common import GET
 
 
 class SonarQubeAuditLogs(RestClient):
     """
     SonarQube audit logs Operations
     """
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/enterprise/views.py` & `python-sonarqube-api-2.0.0/sonarqube/rest/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,43 @@
+#!/usr/bin/env python
+# -*- coding:utf-8 -*-
+# @Author: Jialiang Shi
 from sonarqube.utils.common import POST, GET
 from sonarqube.utils.rest_client import RestClient
 
 from sonarqube.utils.config import (
-    API_VIEWS_UPDATE,
-    API_VIEWS_SHOW,
-    API_VIEWS_SET_TAGS_MODE,
-    API_VIEWS_SET_REMAINING_PROJECTS_MODE,
-    API_VIEWS_SET_REGEXP_MODE,
-    API_VIEWS_SET_MANUAL_MODE,
-    API_VIEWS_REMOVE_PROJECT,
-    API_VIEWS_MOVE_OPTIONS,
-    API_VIEWS_MOVE,
-    API_VIEWS_LOCAL_VIEWS,
-    API_VIEWS_LIST,
-    API_VIEWS_DEFINITION,
-    API_VIEWS_DEFINE,
-    API_VIEWS_CREATE,
-    API_VIEWS_DELETE,
-    API_VIEWS_ADD_SUB_VIEW,
-    API_VIEWS_ADD_PROJECT,
-    API_VIEWS_ADD_LOCAL_VIEW,
-    API_VIEWS_SET_NONE_MODE_VIEW,
-    API_VIEWS_ADD_PROJECT_BRANCH_VIEW,
-    API_VIEWS_REMOVE_PROJECT_BRANCH_VIEW,
-    API_VIEWS_ADD_APPLICATION_BRANCH_VIEW,
-    API_VIEWS_REMOVE_APPLICATION_BRANCH_VIEW,
-    API_VIEWS_APPLICATIONS_VIEW,
-    API_VIEWS_ADD_APPLICATION_VIEW,
-    API_VIEWS_REMOVE_APPLICATION_VIEW,
-    API_VIEWS_PORTFOLIOS_VIEW,
-    API_VIEWS_ADD_PORTFOLIO_VIEW,
-    API_VIEWS_REMOVE_PORTFOLIO_VIEW
+    API_VIEWS_UPDATE,  # pro
+    API_VIEWS_SHOW,  # pro
+    API_VIEWS_SET_TAGS_MODE,  # pro
+    API_VIEWS_SET_REMAINING_PROJECTS_MODE,  # pro
+    API_VIEWS_SET_REGEXP_MODE,  # pro
+    API_VIEWS_SET_MANUAL_MODE,  # pro
+    API_VIEWS_REMOVE_PROJECT,  # pro
+    API_VIEWS_MOVE_OPTIONS,  # pro
+    API_VIEWS_MOVE,  # pro
+    API_VIEWS_LOCAL_VIEWS,  # pro
+    API_VIEWS_LIST,  # pro
+    API_VIEWS_DEFINITION,  # pro
+    API_VIEWS_DEFINE,  # pro
+    API_VIEWS_CREATE,  # pro
+    API_VIEWS_DELETE,  # pro
+    API_VIEWS_ADD_SUB_VIEW,  # pro
+    API_VIEWS_ADD_PROJECT,  # pro
+    API_VIEWS_ADD_LOCAL_VIEW,  # pro
+    API_VIEWS_SET_NONE_MODE_VIEW,  # pro
+    API_VIEWS_ADD_PROJECT_BRANCH_VIEW,  # pro
+    API_VIEWS_REMOVE_PROJECT_BRANCH_VIEW,  # pro
+    API_VIEWS_ADD_APPLICATION_BRANCH_VIEW,  # pro
+    API_VIEWS_REMOVE_APPLICATION_BRANCH_VIEW,  # pro
+    API_VIEWS_APPLICATIONS_VIEW,  # pro
+    API_VIEWS_ADD_APPLICATION_VIEW,  # pro
+    API_VIEWS_REMOVE_APPLICATION_VIEW,  # pro
+    API_VIEWS_PORTFOLIOS_VIEW,  # pro
+    API_VIEWS_ADD_PORTFOLIO_VIEW,  # pro
+    API_VIEWS_REMOVE_PORTFOLIO_VIEW  # pro
 )
 
 
 class SonarQubeViews(RestClient):
     """
     Manage Portfolios
     """
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/utils/common.py` & `python-sonarqube-api-2.0.0/sonarqube/utils/common.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.7/sonarqube/utils/config.py` & `python-sonarqube-api-2.0.0/sonarqube/utils/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,14 +192,17 @@
 
 API_FAVORITES_ADD_ENDPOINT = "/api/favorites/add"
 API_FAVORITES_REMOVE_ENDPOINT = "/api/favorites/remove"
 API_FAVORITES_SEARCH_ENDPOINT = "/api/favorites/search"
 
 API_HOTSPOTS_SEARCH_ENDPOINT = "/api/hotspots/search"
 API_HOTSPOTS_SHOW_ENDPOINT = "/api/hotspots/show"
+API_HOTSPOTS_CHANGE_STATUS_ENDPOINT = "/api/hotspots/change_status"
+
+API_ANALYSIS_CACHE = "/api/analysis_cache/get"
 
 API_LANGUAGES_LIST_ENDPOINT = "/api/languages/list"
 
 API_PROJECT_BADGES_MEASURE_ENDPOINT = "/api/project_badges/measure"
 API_PROJECT_BADGES_QUALITY_GATE_ENDPOINT = "/api/project_badges/quality_gate"
 API_PROJECT_BADGES_RENEW_TOKEN_ENDPOINT = "/api/project_badges/renew_token"
 API_PROJECT_BADGES_TOKEN_ENDPOINT = "/api/project_badges/token"
```

### Comparing `python-sonarqube-api-1.3.7/sonarqube/utils/rest_client.py` & `python-sonarqube-api-2.0.0/sonarqube/utils/rest_client.py`

 * *Files identical despite different names*

