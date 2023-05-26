# Comparing `tmp/noloadj-1.2.6.tar.gz` & `tmp/noloadj-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\noloadj-1.2.6.tar", last modified: Tue Apr 25 13:33:14 2023, max compression
+gzip compressed data, was "dist\noloadj-1.2.7.tar", last modified: Fri May 26 09:23:02 2023, max compression
```

## Comparing `noloadj-1.2.6.tar` & `noloadj-1.2.7.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.529621 noloadj-1.2.6/
--rw-rw-rw-   0        0        0      257 2021-12-02 13:17:49.000000 noloadj-1.2.6/AUTHORS.md
--rw-rw-rw-   0        0        0     2749 2021-12-02 13:17:49.000000 noloadj-1.2.6/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11550 2021-12-02 13:17:49.000000 noloadj-1.2.6/LICENSE
--rw-rw-rw-   0        0        0      166 2021-12-02 13:17:49.000000 noloadj-1.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0     5324 2023-04-25 13:33:14.529621 noloadj-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     4773 2023-01-18 15:18:00.000000 noloadj-1.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.398140 noloadj-1.2.6/docs/
--rw-rw-rw-   0        0        0      203 2021-12-02 13:17:49.000000 noloadj-1.2.6/docs/NoLOAD_Jax_description.rst
--rw-rw-rw-   0        0        0      379 2021-12-02 13:17:49.000000 noloadj-1.2.6/docs/about_NoLOAD_Jax.rst
--rw-rw-rw-   0        0        0    30996 2023-01-19 15:23:24.000000 noloadj-1.2.6/docs/how_to_NoLOAD_Jax.rst
--rw-rw-rw-   0        0        0     1639 2022-09-26 12:06:06.000000 noloadj-1.2.6/docs/index.rst
--rw-rw-rw-   0        0        0     9321 2023-01-18 15:19:37.000000 noloadj-1.2.6/docs/installation_requirements.rst
-drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.482757 noloadj-1.2.6/docs/new_features/
--rw-rw-rw-   0        0        0      814 2021-12-02 13:17:49.000000 noloadj-1.2.6/docs/new_features/v1.0.1.rst
--rw-rw-rw-   0        0        0      250 2021-12-02 13:17:49.000000 noloadj-1.2.6/docs/new_features/v1.0.2.rst
--rw-rw-rw-   0        0        0      469 2021-12-07 14:23:29.000000 noloadj-1.2.6/docs/new_features/v1.1.0.rst
--rw-rw-rw-   0        0        0      296 2022-03-28 19:16:25.000000 noloadj-1.2.6/docs/new_features/v1.1.1.rst
--rw-rw-rw-   0        0        0      271 2022-06-22 12:46:39.000000 noloadj-1.2.6/docs/new_features/v1.1.2.rst
--rw-rw-rw-   0        0        0      359 2022-07-04 14:52:17.000000 noloadj-1.2.6/docs/new_features/v1.1.3.rst
--rw-rw-rw-   0        0        0      435 2022-07-31 13:27:41.000000 noloadj-1.2.6/docs/new_features/v1.1.41.rst
--rw-rw-rw-   0        0        0      879 2022-09-15 14:23:43.000000 noloadj-1.2.6/docs/new_features/v1.1.5.rst
--rw-rw-rw-   0        0        0      233 2022-09-16 13:40:40.000000 noloadj-1.2.6/docs/new_features/v1.1.6.rst
--rw-rw-rw-   0        0        0      469 2022-09-26 12:42:53.000000 noloadj-1.2.6/docs/new_features/v1.1.7.rst
--rw-rw-rw-   0        0        0      411 2022-10-10 13:59:06.000000 noloadj-1.2.6/docs/new_features/v1.1.8.rst
--rw-rw-rw-   0        0        0      369 2022-11-10 08:54:10.000000 noloadj-1.2.6/docs/new_features/v1.1.9.rst
--rw-rw-rw-   0        0        0      615 2022-11-28 16:05:49.000000 noloadj-1.2.6/docs/new_features/v1.2.0.rst
--rw-rw-rw-   0        0        0      415 2023-01-06 10:14:29.000000 noloadj-1.2.6/docs/new_features/v1.2.1.rst
--rw-rw-rw-   0        0        0      257 2023-01-10 10:26:06.000000 noloadj-1.2.6/docs/new_features/v1.2.15.rst
--rw-rw-rw-   0        0        0      267 2023-01-11 14:31:56.000000 noloadj-1.2.6/docs/new_features/v1.2.2.rst
--rw-rw-rw-   0        0        0      349 2023-01-26 15:46:21.000000 noloadj-1.2.6/docs/new_features/v1.2.3.rst
--rw-rw-rw-   0        0        0      379 2023-03-03 15:08:46.000000 noloadj-1.2.6/docs/new_features/v1.2.4.rst
--rw-rw-rw-   0        0        0      380 2023-03-17 15:42:28.000000 noloadj-1.2.6/docs/new_features/v1.2.5.rst
--rw-rw-rw-   0        0        0      581 2023-04-25 12:44:12.000000 noloadj-1.2.6/docs/new_features/v1.2.6.rst
--rw-rw-rw-   0        0        0      805 2023-04-25 12:44:12.000000 noloadj-1.2.6/docs/new_functionnalities.rst
-drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.482757 noloadj-1.2.6/noloadj/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.498378 noloadj-1.2.6/noloadj/ODE/
--rw-rw-rw-   0        0        0    10618 2023-04-25 12:36:26.000000 noloadj-1.2.6/noloadj/ODE/ode45.py
--rw-rw-rw-   0        0        0    15882 2023-04-21 14:33:22.000000 noloadj-1.2.6/noloadj/ODE/ode45_extract.py
--rw-rw-rw-   0        0        0     4896 2023-04-25 12:42:14.000000 noloadj-1.2.6/noloadj/ODE/ode45_extract_fft.py
--rw-rw-rw-   0        0        0     1889 2023-04-25 12:38:23.000000 noloadj-1.2.6/noloadj/ODE/ode45_fft.py
--rw-rw-rw-   0        0        0     2794 2023-04-17 08:44:05.000000 noloadj-1.2.6/noloadj/ODE/ode_tools.py
--rw-rw-rw-   0        0        0       88 2022-11-14 15:31:43.000000 noloadj-1.2.6/noloadj/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.498378 noloadj-1.2.6/noloadj/analyse/
--rw-rw-rw-   0        0        0     4829 2023-01-19 13:47:35.000000 noloadj-1.2.6/noloadj/analyse/simulation.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.498378 noloadj-1.2.6/noloadj/gui/
--rw-rw-rw-   0        0        0     8873 2022-09-26 10:08:50.000000 noloadj-1.2.6/noloadj/gui/plotIterations.py
--rw-rw-rw-   0        0        0     6664 2022-09-15 13:49:58.000000 noloadj-1.2.6/noloadj/gui/plotPareto.py
--rw-rw-rw-   0        0        0     1671 2021-12-02 13:17:49.000000 noloadj-1.2.6/noloadj/gui/testOverLabels.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.514000 noloadj-1.2.6/noloadj/optimization/
--rw-rw-rw-   0        0        0     3042 2021-12-07 13:44:04.000000 noloadj-1.2.6/noloadj/optimization/ExportToXML.py
--rw-rw-rw-   0        0        0     6001 2023-01-13 10:49:31.000000 noloadj-1.2.6/noloadj/optimization/Tools.py
--rw-rw-rw-   0        0        0       88 2023-02-20 11:35:20.000000 noloadj-1.2.6/noloadj/optimization/__init__.py
--rw-rw-rw-   0        0        0     3278 2022-07-29 13:59:40.000000 noloadj-1.2.6/noloadj/optimization/iterationHandler.py
--rw-rw-rw-   0        0        0    12053 2023-01-26 15:54:37.000000 noloadj-1.2.6/noloadj/optimization/multiobjective.py
--rw-rw-rw-   0        0        0    12830 2023-02-24 13:24:55.000000 noloadj-1.2.6/noloadj/optimization/optimProblem.py
--rw-rw-rw-   0        0        0     5005 2021-12-02 13:17:49.000000 noloadj-1.2.6/noloadj/optimization/paretoTools.py
--rw-rw-rw-   0        0        0     7437 2023-01-19 13:13:53.000000 noloadj-1.2.6/noloadj/optimization/specifications.py
--rw-rw-rw-   0        0        0    36269 2023-01-26 15:34:33.000000 noloadj-1.2.6/noloadj/optimization/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.514000 noloadj-1.2.6/noloadj/tutorial/
--rw-rw-rw-   0        0        0     2043 2023-01-19 13:08:31.000000 noloadj-1.2.6/noloadj/tutorial/01-UnconstrainedMonoObjective.py
--rw-rw-rw-   0        0        0     2015 2023-01-19 13:14:21.000000 noloadj-1.2.6/noloadj/tutorial/02-ConstrainedMonoObjective.py
--rw-rw-rw-   0        0        0     2404 2023-01-19 13:10:12.000000 noloadj-1.2.6/noloadj/tutorial/03-ConstrainedMultiObjective.py
--rw-rw-rw-   0        0        0     3885 2023-01-18 15:05:58.000000 noloadj-1.2.6/noloadj/tutorial/04-ConstrainedMonoObjective2.py
--rw-rw-rw-   0        0        0     1097 2021-12-02 13:17:49.000000 noloadj-1.2.6/noloadj/tutorial/plotTools.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:33:14.482757 noloadj-1.2.6/noloadj.egg-info/
--rw-rw-rw-   0        0        0     5324 2023-04-25 13:33:14.000000 noloadj-1.2.6/noloadj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1784 2023-04-25 13:33:14.000000 noloadj-1.2.6/noloadj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 13:33:14.000000 noloadj-1.2.6/noloadj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-25 13:33:14.000000 noloadj-1.2.6/noloadj.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 13:33:14.000000 noloadj-1.2.6/noloadj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 13:33:14.529621 noloadj-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1625 2023-04-17 14:46:08.000000 noloadj-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 09:23:02.133499 noloadj-1.2.7/
+-rw-rw-rw-   0        0        0      257 2021-12-02 13:17:49.000000 noloadj-1.2.7/AUTHORS.md
+-rw-rw-rw-   0        0        0     2749 2021-12-02 13:17:49.000000 noloadj-1.2.7/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11550 2021-12-02 13:17:49.000000 noloadj-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0      166 2021-12-02 13:17:49.000000 noloadj-1.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     6139 2023-05-26 09:23:02.133499 noloadj-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5588 2023-05-26 09:21:24.000000 noloadj-1.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 09:23:02.002043 noloadj-1.2.7/docs/
+-rw-rw-rw-   0        0        0      203 2021-12-02 13:17:49.000000 noloadj-1.2.7/docs/NoLOAD_Jax_description.rst
+-rw-rw-rw-   0        0        0      379 2021-12-02 13:17:49.000000 noloadj-1.2.7/docs/about_NoLOAD_Jax.rst
+-rw-rw-rw-   0        0        0    30996 2023-01-19 15:23:24.000000 noloadj-1.2.7/docs/how_to_NoLOAD_Jax.rst
+-rw-rw-rw-   0        0        0     1639 2022-09-26 12:06:06.000000 noloadj-1.2.7/docs/index.rst
+-rw-rw-rw-   0        0        0     9880 2023-05-22 08:42:02.000000 noloadj-1.2.7/docs/installation_requirements.rst
+drwxrwxrwx   0        0        0        0 2023-05-26 09:23:02.071016 noloadj-1.2.7/docs/new_features/
+-rw-rw-rw-   0        0        0      814 2021-12-02 13:17:49.000000 noloadj-1.2.7/docs/new_features/v1.0.1.rst
+-rw-rw-rw-   0        0        0      250 2021-12-02 13:17:49.000000 noloadj-1.2.7/docs/new_features/v1.0.2.rst
+-rw-rw-rw-   0        0        0      469 2021-12-07 14:23:29.000000 noloadj-1.2.7/docs/new_features/v1.1.0.rst
+-rw-rw-rw-   0        0        0      296 2022-03-28 19:16:25.000000 noloadj-1.2.7/docs/new_features/v1.1.1.rst
+-rw-rw-rw-   0        0        0      271 2022-06-22 12:46:39.000000 noloadj-1.2.7/docs/new_features/v1.1.2.rst
+-rw-rw-rw-   0        0        0      359 2022-07-04 14:52:17.000000 noloadj-1.2.7/docs/new_features/v1.1.3.rst
+-rw-rw-rw-   0        0        0      435 2022-07-31 13:27:41.000000 noloadj-1.2.7/docs/new_features/v1.1.41.rst
+-rw-rw-rw-   0        0        0      879 2022-09-15 14:23:43.000000 noloadj-1.2.7/docs/new_features/v1.1.5.rst
+-rw-rw-rw-   0        0        0      233 2022-09-16 13:40:40.000000 noloadj-1.2.7/docs/new_features/v1.1.6.rst
+-rw-rw-rw-   0        0        0      469 2022-09-26 12:42:53.000000 noloadj-1.2.7/docs/new_features/v1.1.7.rst
+-rw-rw-rw-   0        0        0      411 2022-10-10 13:59:06.000000 noloadj-1.2.7/docs/new_features/v1.1.8.rst
+-rw-rw-rw-   0        0        0      369 2022-11-10 08:54:10.000000 noloadj-1.2.7/docs/new_features/v1.1.9.rst
+-rw-rw-rw-   0        0        0      615 2022-11-28 16:05:49.000000 noloadj-1.2.7/docs/new_features/v1.2.0.rst
+-rw-rw-rw-   0        0        0      415 2023-01-06 10:14:29.000000 noloadj-1.2.7/docs/new_features/v1.2.1.rst
+-rw-rw-rw-   0        0        0      257 2023-01-10 10:26:06.000000 noloadj-1.2.7/docs/new_features/v1.2.15.rst
+-rw-rw-rw-   0        0        0      267 2023-01-11 14:31:56.000000 noloadj-1.2.7/docs/new_features/v1.2.2.rst
+-rw-rw-rw-   0        0        0      349 2023-01-26 15:46:21.000000 noloadj-1.2.7/docs/new_features/v1.2.3.rst
+-rw-rw-rw-   0        0        0      379 2023-03-03 15:08:46.000000 noloadj-1.2.7/docs/new_features/v1.2.4.rst
+-rw-rw-rw-   0        0        0      380 2023-03-17 15:42:28.000000 noloadj-1.2.7/docs/new_features/v1.2.5.rst
+-rw-rw-rw-   0        0        0      581 2023-04-25 12:44:12.000000 noloadj-1.2.7/docs/new_features/v1.2.6.rst
+-rw-rw-rw-   0        0        0      795 2023-05-26 09:00:10.000000 noloadj-1.2.7/docs/new_features/v1.2.7.rst
+-rw-rw-rw-   0        0        0      827 2023-05-26 09:00:10.000000 noloadj-1.2.7/docs/new_functionnalities.rst
+drwxrwxrwx   0        0        0        0 2023-05-26 09:23:02.086636 noloadj-1.2.7/noloadj/
+drwxrwxrwx   0        0        0        0 2023-05-26 09:23:02.102284 noloadj-1.2.7/noloadj/ODE/
+-rw-rw-rw-   0        0        0    10514 2023-05-05 14:10:31.000000 noloadj-1.2.7/noloadj/ODE/ode45.py
+-rw-rw-rw-   0        0        0    15909 2023-05-14 16:22:48.000000 noloadj-1.2.7/noloadj/ODE/ode45_extract.py
+-rw-rw-rw-   0        0        0    11757 2023-05-24 09:33:54.000000 noloadj-1.2.7/noloadj/ODE/ode45_extract_fft.py
+-rw-rw-rw-   0        0        0     1889 2023-04-28 13:03:06.000000 noloadj-1.2.7/noloadj/ODE/ode45_fft.py
+-rw-rw-rw-   0        0        0     2794 2023-04-17 08:44:05.000000 noloadj-1.2.7/noloadj/ODE/ode_tools.py
+-rw-rw-rw-   0        0        0       88 2022-11-14 15:31:43.000000 noloadj-1.2.7/noloadj/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 09:23:02.102284 noloadj-1.2.7/noloadj/analyse/
+-rw-rw-rw-   0        0        0     4829 2023-01-19 13:47:35.000000 noloadj-1.2.7/noloadj/analyse/simulation.py
+drwxrwxrwx   0        0        0        0 2023-05-26 09:23:02.102284 noloadj-1.2.7/noloadj/gui/
+-rw-rw-rw-   0        0        0     8873 2022-09-26 10:08:50.000000 noloadj-1.2.7/noloadj/gui/plotIterations.py
+-rw-rw-rw-   0        0        0     6664 2022-09-15 13:49:58.000000 noloadj-1.2.7/noloadj/gui/plotPareto.py
+-rw-rw-rw-   0        0        0     1671 2021-12-02 13:17:49.000000 noloadj-1.2.7/noloadj/gui/testOverLabels.py
+drwxrwxrwx   0        0        0        0 2023-05-26 09:23:02.117879 noloadj-1.2.7/noloadj/optimization/
+-rw-rw-rw-   0        0        0     4598 2023-05-25 08:59:42.000000 noloadj-1.2.7/noloadj/optimization/ExportToXML.py
+-rw-rw-rw-   0        0        0     6001 2023-01-13 10:49:31.000000 noloadj-1.2.7/noloadj/optimization/Tools.py
+-rw-rw-rw-   0        0        0       88 2023-05-26 09:10:34.000000 noloadj-1.2.7/noloadj/optimization/__init__.py
+-rw-rw-rw-   0        0        0     3933 2023-05-24 14:34:19.000000 noloadj-1.2.7/noloadj/optimization/iterationHandler.py
+-rw-rw-rw-   0        0        0    12637 2023-05-26 09:10:49.000000 noloadj-1.2.7/noloadj/optimization/multiobjective.py
+-rw-rw-rw-   0        0        0    13150 2023-05-24 09:41:44.000000 noloadj-1.2.7/noloadj/optimization/optimProblem.py
+-rw-rw-rw-   0        0        0     5005 2021-12-02 13:17:49.000000 noloadj-1.2.7/noloadj/optimization/paretoTools.py
+-rw-rw-rw-   0        0        0     7759 2023-05-24 14:32:26.000000 noloadj-1.2.7/noloadj/optimization/specifications.py
+-rw-rw-rw-   0        0        0    38636 2023-05-24 13:44:54.000000 noloadj-1.2.7/noloadj/optimization/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-26 09:23:02.117879 noloadj-1.2.7/noloadj/tutorial/
+-rw-rw-rw-   0        0        0     2043 2023-05-25 09:00:14.000000 noloadj-1.2.7/noloadj/tutorial/01-UnconstrainedMonoObjective.py
+-rw-rw-rw-   0        0        0     2015 2023-05-24 14:21:43.000000 noloadj-1.2.7/noloadj/tutorial/02-ConstrainedMonoObjective.py
+-rw-rw-rw-   0        0        0     2404 2023-05-26 08:56:27.000000 noloadj-1.2.7/noloadj/tutorial/03-ConstrainedMultiObjective.py
+-rw-rw-rw-   0        0        0     3885 2023-05-25 09:02:41.000000 noloadj-1.2.7/noloadj/tutorial/04-ConstrainedMonoObjective2.py
+-rw-rw-rw-   0        0        0     1097 2023-05-25 10:47:26.000000 noloadj-1.2.7/noloadj/tutorial/plotTools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 09:23:02.086636 noloadj-1.2.7/noloadj.egg-info/
+-rw-rw-rw-   0        0        0     6139 2023-05-26 09:23:01.000000 noloadj-1.2.7/noloadj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1813 2023-05-26 09:23:01.000000 noloadj-1.2.7/noloadj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 09:23:01.000000 noloadj-1.2.7/noloadj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-26 09:23:01.000000 noloadj-1.2.7/noloadj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 09:23:01.000000 noloadj-1.2.7/noloadj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 09:23:02.133499 noloadj-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1642 2023-05-26 09:22:40.000000 noloadj-1.2.7/setup.py
```

### Comparing `noloadj-1.2.6/CONTRIBUTING.md` & `noloadj-1.2.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/LICENSE` & `noloadj-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/PKG-INFO` & `noloadj-1.2.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: noloadj
-Version: 1.2.6
-Summary: solving constrained optimization problem for the design of engineering systems
-Author: B. DELINCHANT, L. GERBAUD, F. WURTZ, L.AGOBERT
-Author-email: benoit.delinchant@G2ELab.grenoble-inp.fr
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Scientific/Engineering
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.md
-
 <!--
 SPDX-FileCopyrightText: 2021 G2Elab / MAGE
 
 SPDX-License-Identifier: Apache-2.0
 -->
 
 NoLOAD_Jax: Non Linear Optimization by Automatic Differentiation using Jax
@@ -24,15 +10,21 @@
 We are happy that you will use or develop the NoLOAD_Jax.
 It is an **Open Source** project located on GitLab at https://gricad-gitlab.univ-grenoble-alpes.fr/design_optimization/NoLoad_v2
 It aims at **solving constrained optimization** problem for the design of engineering systems
 
 Project Presentation
 ====================
 
-**NoLOAD_Jax:** Please have a look to NoLOAD presentation : https://noload_jax.readthedocs.io/en/latest/  
+**NoLOAD_Jax:** Please have a look to NoLOAD presentation : https://noload-jax.readthedocs.io/en/latest/
+
+A scientific article presenting NoLOAD is available here:
+
+Agobert Lucas, Hodencq Sacha, Delinchant Benoit, Gerbaud Laurent, Frederic Wurtz, “NoLOAD, Open Software for Optimal Design and Operation using Automatic Differentiation”, OIPE 2020, Poland, 09-2021. https://hal.archives-ouvertes.fr/hal-03352443
+
+Please cite us when you use NoLOAD.
 
 NoLOAD_Jax Community
 ====================
 
 Please use the git issues system to report an error: https://gricad-gitlab.univ-grenoble-alpes.fr/design_optimization/NoLoad_v2
 Otherwise you can also contact the developer team using the following email adress: benoit.delinchant@G2ELab.grenoble-inp.fr
 
@@ -41,35 +33,34 @@
 You can install the library as a user or as a developer. Please follow the corresponding installation steps below.
 
 Prerequisite
 ------------
 
 Please install Python 3.8 or later
 https://www.python.org/downloads/
-You must run NoLOAD_Jax on Ubuntu : on Jupyter Notebook on a computer using Ubuntu, or as explained later, using WSL (Windows Subsystem for Linux) if your computer works on Windows.
-As it uses the JAX library, NoLOAD_Jax can run on CPU (Central Processor Unit) or GPU (Graphics Processor Unit), where GPU offers better performances than CPU.
-With WSL only CPU can be used. To use GPU you may run NoLOAD on Ubuntu.
-If you want to use GPU, you need to install CUDA and CuDNN on your computer then tape on Pycharm terminal (where 0.3.XX is your JAX version):
 
-    pip install --upgrade pip
-    pip install --upgrade jax jaxlib==0.3.XX+cuda111 -f https://storage.googleapis.com/jax-releases/jax_releases.html
-    
-If you use GPU, you need to put these lines at the beginning of your "optimization" file to avoid memory issues :
+Windows
+-------
 
-    import os
-    os.environ['XLA_PYTHON_CLIENT_PREALLOCATE']='false'
-    os.environ['XLA_PYTHON_CLIENT_MEM_FRACTION']='0.50'
-    
-To install IPOPT algorithm, please install an Anaconda environment and run this command on a terminal :
+The simplest way to install it
+------------------------------
+Go on  https://whls.blob.core.windows.net/unstable/index.html and download the cpu/jaxlib-0.3.25-cp3X-cp3X-win_amd64.whl, where 3.X is your Python version.
+Put it in your Python environment and tape on a terminal :
+
+    pip install cpu/jaxlib-0.3.25-cp3X-cp3X-win_amd64.whl
+    pip install jax==0.3.25
+    pip install noloadj
+
+The Jax version installed is not the newest one, but it is sufficient to use Noload_Jax.
 
-    conda install -c conda-forge cyipopt
     
-How to configure a virtual environment on WSL running with a Ubuntu distribution :
-----------------------
-At first, activate the WSL on you computer and install on it a Ubuntu distribution by following the 6 first steps of the link :
+How to configure a virtual environment on WSL running with an Ubuntu distribution :
+------------------------------
+The alternative to get Jax last versions is to install a virtual environment on WSL running with an Ubuntu distribution.
+At first, activate the WSL on you computer and install on it an Ubuntu distribution by following the 6 first steps of the link :
 https://docs.microsoft.com/en-us/windows/wsl/install-win10
 
 Then open WSL.exe using the Windows search bar and tape :
 
     cd ~
     sudo apt update
     sudo apt install python3-pip
@@ -86,40 +77,57 @@
 Choose WSL option then change the Python interpreter path by /home/_your_username_/pythonenv/bin/python3. (_your_username_ is the login you chose for WSL)
 Close the Settings window. Click on Terminal section at the bottom, and tape on the commande line  :
 
     source /home/your_username/pythonenv/bin/activate
 
 If you see a "(pythonenv)" written at the beginning of the command line, the configuration is completed and you can run your code now !
 
-Installation as a user
-----------------------
+Linux
+-----
 Please install NoLOAD_Jax with pip using the command prompt.   
 
-If you are admin on Windows or working on a virtual environment
+If you are working on a virtual environment on Linux
     
     pip install noloadj
 
 If you want a local installation or you are not admin
     
     pip install --user noloadj
 
 If you are admin on Linux:
     
     sudo pip install noloadj
 
 Launch the examples to understand how the NoLOAD_Jax works:
 	
-	python noload/01-UnconstrainedMonoObjective.py
-	python noload/02-ConstrainedMonoObjective.py
-	python noload/03-ConstrainedMultiObjective.py
-	python noload/04-ConstrainedMonoObjective2.py
+	python noloadj/01-UnconstrainedMonoObjective.py
+	python noloadj/02-ConstrainedMonoObjective.py
+	python noloadj/03-ConstrainedMultiObjective.py
+	python noloadj/04-ConstrainedMonoObjective2.py
 	
 Enjoy your time using NoLOAD_Jax !
 
+GPU & IPOPT Algorithm
+---------------------
+As it uses the JAX library, NoLOAD_Jax can run on CPU (Central Processor Unit) or GPU (Graphics Processor Unit), where GPU offers better performances than CPU.
+With WSL only CPU can be used. To use GPU you may run NoLOAD on Ubuntu.
+If you want to use GPU, you need to install CUDA and CuDNN on your computer then tape on Pycharm terminal (where 0.3.XX is your JAX version):
 
+    pip install --upgrade pip
+    pip install --upgrade jax jaxlib==0.3.XX+cuda111 -f https://storage.googleapis.com/jax-releases/jax_releases.html
+    
+If you use GPU, you need to put these lines at the beginning of your "optimization" file to avoid memory issues :
+
+    import os
+    os.environ['XLA_PYTHON_CLIENT_PREALLOCATE']='false'
+    os.environ['XLA_PYTHON_CLIENT_MEM_FRACTION']='0.50'
+    
+To install IPOPT algorithm, please install an Anaconda environment and run this command on a terminal :
+
+    conda install -c conda-forge cyipopt
 
 Library Installation Requirements
 ---------------------------------
 Matplotlib >= 3.0
 Scipy >= 1.2
 Jax >= 0.3.25
 Jaxlib >= 0.3.25
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `noloadj-1.2.6/README.md` & `noloadj-1.2.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: noloadj
+Version: 1.2.7
+Summary: solving constrained optimization problem for the design of engineering systems
+Author: B. DELINCHANT, L. GERBAUD, F. WURTZ, L.AGOBERT
+Author-email: benoit.delinchant@G2ELab.grenoble-inp.fr
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Scientific/Engineering
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+
 <!--
 SPDX-FileCopyrightText: 2021 G2Elab / MAGE
 
 SPDX-License-Identifier: Apache-2.0
 -->
 
 NoLOAD_Jax: Non Linear Optimization by Automatic Differentiation using Jax
@@ -10,15 +24,21 @@
 We are happy that you will use or develop the NoLOAD_Jax.
 It is an **Open Source** project located on GitLab at https://gricad-gitlab.univ-grenoble-alpes.fr/design_optimization/NoLoad_v2
 It aims at **solving constrained optimization** problem for the design of engineering systems
 
 Project Presentation
 ====================
 
-**NoLOAD_Jax:** Please have a look to NoLOAD presentation : https://noload_jax.readthedocs.io/en/latest/  
+**NoLOAD_Jax:** Please have a look to NoLOAD presentation : https://noload-jax.readthedocs.io/en/latest/
+
+A scientific article presenting NoLOAD is available here:
+
+Agobert Lucas, Hodencq Sacha, Delinchant Benoit, Gerbaud Laurent, Frederic Wurtz, “NoLOAD, Open Software for Optimal Design and Operation using Automatic Differentiation”, OIPE 2020, Poland, 09-2021. https://hal.archives-ouvertes.fr/hal-03352443
+
+Please cite us when you use NoLOAD.
 
 NoLOAD_Jax Community
 ====================
 
 Please use the git issues system to report an error: https://gricad-gitlab.univ-grenoble-alpes.fr/design_optimization/NoLoad_v2
 Otherwise you can also contact the developer team using the following email adress: benoit.delinchant@G2ELab.grenoble-inp.fr
 
@@ -27,35 +47,34 @@
 You can install the library as a user or as a developer. Please follow the corresponding installation steps below.
 
 Prerequisite
 ------------
 
 Please install Python 3.8 or later
 https://www.python.org/downloads/
-You must run NoLOAD_Jax on Ubuntu : on Jupyter Notebook on a computer using Ubuntu, or as explained later, using WSL (Windows Subsystem for Linux) if your computer works on Windows.
-As it uses the JAX library, NoLOAD_Jax can run on CPU (Central Processor Unit) or GPU (Graphics Processor Unit), where GPU offers better performances than CPU.
-With WSL only CPU can be used. To use GPU you may run NoLOAD on Ubuntu.
-If you want to use GPU, you need to install CUDA and CuDNN on your computer then tape on Pycharm terminal (where 0.3.XX is your JAX version):
 
-    pip install --upgrade pip
-    pip install --upgrade jax jaxlib==0.3.XX+cuda111 -f https://storage.googleapis.com/jax-releases/jax_releases.html
-    
-If you use GPU, you need to put these lines at the beginning of your "optimization" file to avoid memory issues :
+Windows
+-------
 
-    import os
-    os.environ['XLA_PYTHON_CLIENT_PREALLOCATE']='false'
-    os.environ['XLA_PYTHON_CLIENT_MEM_FRACTION']='0.50'
-    
-To install IPOPT algorithm, please install an Anaconda environment and run this command on a terminal :
+The simplest way to install it
+------------------------------
+Go on  https://whls.blob.core.windows.net/unstable/index.html and download the cpu/jaxlib-0.3.25-cp3X-cp3X-win_amd64.whl, where 3.X is your Python version.
+Put it in your Python environment and tape on a terminal :
+
+    pip install cpu/jaxlib-0.3.25-cp3X-cp3X-win_amd64.whl
+    pip install jax==0.3.25
+    pip install noloadj
+
+The Jax version installed is not the newest one, but it is sufficient to use Noload_Jax.
 
-    conda install -c conda-forge cyipopt
     
-How to configure a virtual environment on WSL running with a Ubuntu distribution :
-----------------------
-At first, activate the WSL on you computer and install on it a Ubuntu distribution by following the 6 first steps of the link :
+How to configure a virtual environment on WSL running with an Ubuntu distribution :
+------------------------------
+The alternative to get Jax last versions is to install a virtual environment on WSL running with an Ubuntu distribution.
+At first, activate the WSL on you computer and install on it an Ubuntu distribution by following the 6 first steps of the link :
 https://docs.microsoft.com/en-us/windows/wsl/install-win10
 
 Then open WSL.exe using the Windows search bar and tape :
 
     cd ~
     sudo apt update
     sudo apt install python3-pip
@@ -72,40 +91,57 @@
 Choose WSL option then change the Python interpreter path by /home/_your_username_/pythonenv/bin/python3. (_your_username_ is the login you chose for WSL)
 Close the Settings window. Click on Terminal section at the bottom, and tape on the commande line  :
 
     source /home/your_username/pythonenv/bin/activate
 
 If you see a "(pythonenv)" written at the beginning of the command line, the configuration is completed and you can run your code now !
 
-Installation as a user
-----------------------
+Linux
+-----
 Please install NoLOAD_Jax with pip using the command prompt.   
 
-If you are admin on Windows or working on a virtual environment
+If you are working on a virtual environment on Linux
     
     pip install noloadj
 
 If you want a local installation or you are not admin
     
     pip install --user noloadj
 
 If you are admin on Linux:
     
     sudo pip install noloadj
 
 Launch the examples to understand how the NoLOAD_Jax works:
 	
-	python noload/01-UnconstrainedMonoObjective.py
-	python noload/02-ConstrainedMonoObjective.py
-	python noload/03-ConstrainedMultiObjective.py
-	python noload/04-ConstrainedMonoObjective2.py
+	python noloadj/01-UnconstrainedMonoObjective.py
+	python noloadj/02-ConstrainedMonoObjective.py
+	python noloadj/03-ConstrainedMultiObjective.py
+	python noloadj/04-ConstrainedMonoObjective2.py
 	
 Enjoy your time using NoLOAD_Jax !
 
+GPU & IPOPT Algorithm
+---------------------
+As it uses the JAX library, NoLOAD_Jax can run on CPU (Central Processor Unit) or GPU (Graphics Processor Unit), where GPU offers better performances than CPU.
+With WSL only CPU can be used. To use GPU you may run NoLOAD on Ubuntu.
+If you want to use GPU, you need to install CUDA and CuDNN on your computer then tape on Pycharm terminal (where 0.3.XX is your JAX version):
 
+    pip install --upgrade pip
+    pip install --upgrade jax jaxlib==0.3.XX+cuda111 -f https://storage.googleapis.com/jax-releases/jax_releases.html
+    
+If you use GPU, you need to put these lines at the beginning of your "optimization" file to avoid memory issues :
+
+    import os
+    os.environ['XLA_PYTHON_CLIENT_PREALLOCATE']='false'
+    os.environ['XLA_PYTHON_CLIENT_MEM_FRACTION']='0.50'
+    
+To install IPOPT algorithm, please install an Anaconda environment and run this command on a terminal :
+
+    conda install -c conda-forge cyipopt
 
 Library Installation Requirements
 ---------------------------------
 Matplotlib >= 3.0
 Scipy >= 1.2
 Jax >= 0.3.25
 Jaxlib >= 0.3.25
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `noloadj-1.2.6/docs/how_to_NoLOAD_Jax.rst` & `noloadj-1.2.7/docs/how_to_NoLOAD_Jax.rst`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/docs/index.rst` & `noloadj-1.2.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/docs/installation_requirements.rst` & `noloadj-1.2.7/docs/installation_requirements.rst`

 * *Files 8% similar despite different names*

```diff
@@ -11,65 +11,56 @@
 
 Python 3.8.0
 ************
 Please use Python 3.8.0 for the project interpreter:
 `Python 3.8 <https://www.python.org/downloads/release/python-380/>`_
 
 
-pip install noloadj
-*******************
+Linux
+*****
 Please install NoLOAD_Jax Lib with pip using on of the following the command prompt:
 
+    - **If you are admin on Linux**::
 
-    - **If you are admin on Windows or working on a virtual environment**::
-
-        pip install noloadj
+        sudo pip install noloadj
 
     - **If you want a local installation or you are not admin**::
 
         pip install --user noloadj
 
-    - **If you are admin on Linux**::
+    - **If you are working on a virtual environment on Linux**::
 
-        sudo pip install noloadj
+        pip install noloadj
 
 Then, you can download (or clone) the NoLOAD benchmark folder (repository) at :
 `NoLOAD Examples`_
 Make sure that the name of the examples folder is: "noload_benchmarks_open".
 
 Launch the examples (with Pycharm for instance) to understand how the NoLOAD_Jax Lib works.
 
 **Enjoy your time using NoLOAD_Jax !**
 
 
+Windows
+*******
 
-Other installation requirements
--------------------------------
-You must run NoLOAD_Jax on Ubuntu : on Jupyter Notebook on a computer using Ubuntu, or as explained later, using WSL (Windows Subsystem for Linux) if your computer works on Windows.
-As it uses the JAX library, NoLOAD_Jax can run on CPU (Central Processor Unit) or GPU (Graphics Processor Unit), where GPU offers better performances than CPU.
-With WSL only CPU can be used. To use GPU you may run NoLOAD on Ubuntu.
-If you want to use GPU, you need to install CUDA and CuDNN on your computer then tape on Pycharm terminal (where 0.3.XX is your JAX version):
---- ::
-    pip install --upgrade pip
-    pip install --upgrade jax jaxlib==0.3.XX+cuda111 -f https://storage.googleapis.com/jax-releases/jax_releases.html
-
-    
-If you use GPU, you need to put these lines at the beginning of your "optimization" file to avoid memory issues :
---- ::
-    import os
-    os.environ['XLA_PYTHON_CLIENT_PREALLOCATE']='false'
-    os.environ['XLA_PYTHON_CLIENT_MEM_FRACTION']='0.50'
-
-To install IPOPT algorithm, please install an Anaconda environment and run this command on a terminal :
---- ::
-    conda install -c conda-forge cyipopt
-    
-    
-How to configure a virtual environment on WSL running with a Ubuntu distribution :
-**********************************************************************************
+The simplest way to install it
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Go on  https://whls.blob.core.windows.net/unstable/index.html and download the cpu/jaxlib-0.3.25-cp3X-cp3X-win_amd64.whl, where 3.X is your Python version.
+Put it in your Python environment and tape on a terminal :
+--- ::
+    pip install cpu/jaxlib-0.3.25-cp3X-cp3X-win_amd64.whl
+    pip install jax==0.3.25
+    pip install noloadj
+
+The Jax version installed is not the newest one, but it is sufficient to use Noload_Jax.
+
+How to configure a virtual environment on WSL running with an Ubuntu distribution
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+The alternative to get Jax last versions is to install a virtual environment on WSL running with an Ubuntu distribution.
 At first, activate the WSL on you computer and install on it a Ubuntu distribution by following the 6 first steps of the link :
 https://docs.microsoft.com/en-us/windows/wsl/install-win10
 
 Then open WSL.exe using the Windows search bar and tape :
 --- ::
     cd ~
     sudo apt update
@@ -138,14 +129,35 @@
     **Pycharm lover**
     ---
 
     Install automatically the library using pip with Pycharm on "File", "settings...", "Project Interpreter", "+",
     and choosing the required library
 
 
+GPU & IPOPT Algorithm
+---------------------
+You must run NoLOAD_Jax on Ubuntu : on Jupyter Notebook on a computer using Ubuntu, or as explained later, using WSL (Windows Subsystem for Linux) if your computer works on Windows.
+As it uses the JAX library, NoLOAD_Jax can run on CPU (Central Processor Unit) or GPU (Graphics Processor Unit), where GPU offers better performances than CPU.
+With WSL only CPU can be used. To use GPU you may run NoLOAD on Ubuntu.
+If you want to use GPU, you need to install CUDA and CuDNN on your computer then tape on Pycharm terminal (where 0.3.XX is your JAX version):
+--- ::
+    pip install --upgrade pip
+    pip install --upgrade jax jaxlib==0.3.XX+cuda111 -f https://storage.googleapis.com/jax-releases/jax_releases.html
+
+
+If you use GPU, you need to put these lines at the beginning of your "optimization" file to avoid memory issues :
+--- ::
+    import os
+    os.environ['XLA_PYTHON_CLIENT_PREALLOCATE']='false'
+    os.environ['XLA_PYTHON_CLIENT_MEM_FRACTION']='0.50'
+
+To install IPOPT algorithm, please install an Anaconda environment and run this command on a terminal :
+--- ::
+    conda install -c conda-forge cyipopt
+
 
 Install NoLOAD_Jax as a developer
 ---------------------------------
 Installation as a developer and local branch creation
 ******************************************************
 
 1. Create a new folder in the suitable path, name it as you wish for instance : NoLOAD_Jax
```

### Comparing `noloadj-1.2.6/docs/new_features/v1.0.1.rst` & `noloadj-1.2.7/docs/new_features/v1.0.1.rst`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/docs/new_features/v1.1.5.rst` & `noloadj-1.2.7/docs/new_features/v1.1.5.rst`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/docs/new_features/v1.2.0.rst` & `noloadj-1.2.7/docs/new_features/v1.2.0.rst`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/docs/new_features/v1.2.6.rst` & `noloadj-1.2.7/docs/new_features/v1.2.6.rst`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/docs/new_functionnalities.rst` & `noloadj-1.2.7/docs/new_functionnalities.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 What's new in the latest versions
 =================================
 
-The new version of NoLOAD_Jax v1.2.6 is available!
-The release is from 25th of April 2023.
+The new version of NoLOAD_Jax v1.2.7 is available!
+The release is from 26th of May 2023.
 
 .. toctree::
    :maxdepth: 2
 
-   new_features/v1.2.6
+   new_features/v1.2.7
 
 
 Information about the latest versions
 -------------------------------------
 
 .. toctree::
    :maxdepth: 1
 
-   new_features/v1.2.4
+   new_features/v1.2.6
+   new_features/v1.2.5
    new_features/v1.2.4
    new_features/v1.2.3
    new_features/v1.2.2
    new_features/v1.2.15
    new_features/v1.2.1
    new_features/v1.2.0
    new_features/v1.1.9
```

### Comparing `noloadj-1.2.6/noloadj/ODE/ode45.py` & `noloadj-1.2.7/noloadj/ODE/ode45.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,30 +61,31 @@
     else:
         _,x,y=f.update(x,y,t_now,i)
     return x,y,h,t_now
 
 def next_step_simulation(x_prev,t_prev,y_prev,i,c,h,f,tol,h0,T,*P):
     if hasattr(f,'etat'):
         f.etat=i
+    if hasattr(f,'topo_fixe'):
+        f.compute_topo_fixe()
     x,xest,t_now=rk_step(x_prev,t_prev,h,f.derivative,*P)
     if hasattr(f,'computeotherX'):
         x=f.computeotherX(x,t_now,*P)
         xest=f.computeotherX(xest,t_now,*P)
     y=f.output(x,t_now,*P)
     hopt,cnew,tpdi=0.,0,0.
     if hasattr(f,'etat'):
         if hasattr(f,'commande'):
             tpdi,cnew=f.commande(t_now,T)
             inew,_,yb=f.update(x,y,t_now,i,cnew)
-            x,y,h,t_now=cond(inew!=i,lambda state:interp_state_chgt(x_prev,y_prev,
-              yb,t_prev,x,y,t_now,f,i,h,cnew),lambda state:state,(x,y,h,t_now))
         else:
+            cnew=c
             inew,_,yb=f.update(x,y,t_now,i)
-            x,y,h,t_now=cond(inew!=i,lambda state:interp_state_chgt(x_prev,y_prev,
-             yb,t_prev,x,y,t_now,f,i,h,0),lambda state:state,(x,y,h,t_now))
+        x,y,h,t_now=cond(inew!=i,lambda state:interp_state_chgt(x_prev,y_prev,
+        yb,t_prev,x,y,t_now,f,i,h,cnew),lambda state:state,(x,y,h,t_now))
 
         y=f.output(x,t_now,*P)
         hopt = optimal_step(x,xest, h, tol)
         if hasattr(f,'commande'):
             hopt=np.minimum(tpdi-t_now,hopt)
         hopt=np.where(inew!=i,h0,hopt) # pour accelerer code
     else:
@@ -133,15 +134,15 @@
         x=((x_prev-x_now)*t+t_prev*x_now-t_now*x_prev)/(t_prev-t_now)
         y=((y_prev-y_now)*t+t_prev*y_now-t_now*y_prev)/(t_prev-t_now)
         return (x_prev,t_prev,y_prev,x,t,y,h,i,c),(x,y)
 
     if hasattr(f,'etat'):
         i0=f.etat
         if hasattr(f,'commande'):
-            _,c0=f.commande(0.,T)
+            _,c0=f.commande(t[0],T)
         else:
             c0=0
     else:
         i0=0
         c0=0
     y0=f.output(x0,0.,*P)
     vect,(xs,ys)=scan(scan_fun,(x0,t[0],y0,x0,t[0],y0,h0,i0,c0),t[1:])
@@ -216,20 +217,20 @@
         y = ((y_prev- y_now)*t+t_prev*y_now-t_now*y_prev)/(t_prev - t_now)
         delta_y = ((delta_y_prev-delta_y_now)*t+t_prev*delta_y_now-t_now*
                    delta_y_prev) / (t_prev - t_now)
         return (x_prev,delta_x_prev,y_prev,delta_y_prev,t_prev,x,delta_x,y,
                 delta_y,t, h,i,c), (x,delta_x,y,delta_y)
 
     for element in f.__dict__.keys(): # pour eviter erreurs de code
-        if isinstance(f.__dict__[element],interpreters.ad.JVPTracer):
+        if hasattr(f.__dict__[element],'primal'):
             f.__dict__[element]=f.__dict__[element].primal
     if hasattr(f,'etat'):
         i0=f.etat
         if hasattr(f,'commande'):
-            _,c0=f.commande(0.,T)
+            _,c0=f.commande(t[0],T)
         else:
             c0=0
     else:
         i0=0
         c0=0
     y0=f.output(x0,0.,*P)
     delta_y0=jvp(f.output,(x0,0.,*P),(delta_x0,0.,*dP))[1]
```

### Comparing `noloadj-1.2.6/noloadj/ODE/ode45_extract.py` & `noloadj-1.2.7/noloadj/ODE/ode45_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             ind=f.xnames.index(name)
             cstr[i]=np.where(test_exp(0.),init(x0[ind],0.,h0),
                              cstr[i])
             delta_cstr[i]=np.where(test_exp(0.),dinit(x0[ind],delta_x0[ind],0.,
                                     h0),delta_cstr[i])
 
     for element in f.__dict__.keys(): # pour eviter erreurs de code
-        if isinstance(f.__dict__[element],interpreters.ad.JVPTracer):
+        if hasattr(f.__dict__[element],'primal'):
             f.__dict__[element]=f.__dict__[element].primal
     if hasattr(f,'etat'):
         i0=f.etat
         if hasattr(f,'commande'):
             _,c0=f.commande(0.,T)
         else:
             c0=0
@@ -213,15 +213,16 @@
             delta_cstr[i]=der_fin(ts,cstr[i],T,delta_cstr[i],dT,xf[ind])
 
     if type=='seuil': # partial derivatives of ts
         dout,_=cond_stop(delta_xf,f.xnames)
         xseuil,_=cond_stop(f.derivative(xf,ts,*P),f.xnames)
         dts=-(1/xseuil)*dout
     elif type=='rp':
-        #f.etat=ifinal
+        if hasattr(f,'topo_fixe'):
+            f.compute_topo_fixe()
         ind_rp=f.xnames.index(f.last_var_bf_rp)
         xseuil=f.derivative(xf,ts,*P)[ind_rp]
         dts=-(1/xseuil)*delta_xf[ind_rp]
     else:
         dts=0.
     return xf,yf,cstr,ts,dts,delta_xf,delta_yf,delta_cstr
```

### Comparing `noloadj-1.2.6/noloadj/ODE/ode45_fft.py` & `noloadj-1.2.7/noloadj/ODE/ode45_fft.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/noloadj/ODE/ode_tools.py` & `noloadj-1.2.7/noloadj/ODE/ode_tools.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/noloadj/analyse/simulation.py` & `noloadj-1.2.7/noloadj/analyse/simulation.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/noloadj/gui/plotIterations.py` & `noloadj-1.2.7/noloadj/gui/plotIterations.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/noloadj/gui/plotPareto.py` & `noloadj-1.2.7/noloadj/gui/plotPareto.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/noloadj/gui/testOverLabels.py` & `noloadj-1.2.7/noloadj/gui/testOverLabels.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/noloadj/optimization/ExportToXML.py` & `noloadj-1.2.7/noloadj/optimization/ExportToXML.py`

 * *Files 24% similar despite different names*

```diff
@@ -66,10 +66,52 @@
             output.setAttribute('Name', iter.fNames[oCmpt])
             outputs.appendChild(output)
             oCmpt=oCmpt+1
     #< SPECIFICATIONS >
     spec = root.createElement('SPECIFICATIONS') #not used but required
     xml.appendChild(spec)
 
+    objs = root.createElement('Objective functions')
+    objs.setAttribute('Number',str(len(iter.objectives)))
+    spec.appendChild(objs)
+
+    for name,value in iter.objectives.items():
+        obj = root.createElement('Objective')
+        obj.setAttribute('Value', str(value))
+        obj.setAttribute('Name', name)
+        objs.appendChild(obj)
+
+    if iter.eq_cstr!={}:
+        eqs = root.createElement('Equality Constraints')
+        eqs.setAttribute('Number', str(len(iter.eq_cstr)))
+        spec.appendChild(eqs)
+
+        for name,value in iter.eq_cstr.items():
+            eq = root.createElement('Equality Constraint')
+            eq.setAttribute('Value', str(value))
+            eq.setAttribute('Name', name)
+            eqs.appendChild(eq)
+
+    if iter.ineq_cstr!={}:
+        ineqs = root.createElement('Inequality Constraints')
+        ineqs.setAttribute('Number', str(len(iter.ineq_cstr)))
+        spec.appendChild(ineqs)
+
+        for name, value in iter.ineq_cstr.items():
+            ineq = root.createElement('Inequality Constraint')
+            ineq.setAttribute('Value', str(value))
+            ineq.setAttribute('Name', name)
+            ineqs.appendChild(ineq)
+
+    if iter.fNames!=[]:
+        fOuts = root.createElement('Free Outputs')
+        fOuts.setAttribute('Number', str(len(iter.fNames)))
+        spec.appendChild(fOuts)
+
+        for name in iter.fNames:
+            fOut=root.createElement('Free Output')
+            fOut.setAttribute('Name', name)
+            fOuts.appendChild(fOut)
+
     xml_str = root.toprettyxml(indent ="\t")
     with open(fileName, "w") as f:
         f.write(xml_str)
```

### Comparing `noloadj-1.2.6/noloadj/optimization/Tools.py` & `noloadj-1.2.7/noloadj/optimization/Tools.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/noloadj/optimization/iterationHandler.py` & `noloadj-1.2.7/noloadj/optimization/iterationHandler.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,25 +25,37 @@
 class Iterations:
     """
     At each gradient computation, gets the inputs and outputs of the model.
     solutions: class Solution
     iNames = list : model inputs
     oNames = list : model outputs
     fNames = list : model free outputs names
+    objectives = dict : objective functions of the model
+    eq_cstr = dict : equality constraints of the model
+    ineq_cstr = dict : inequality constraints of the model
     """
     solutions: Solution = []
     iNames = [] # noms des entrées du modèle
     oNames = [] # noms des sorties du modèle
-    fNames = []
+    fNames = [] # noms des sorties 'libres' du modèle
+    objectives = {} # fonctions objectives du modèle
+    eq_cstr = {} # contraintes d'égalité
+    ineq_cstr = {} # contraintes d'inégalité
 
-    def __init__(self, iNames, oNames, fNames=[], handler = None):
+    def __init__(self, spec,iNames, oNames, fNames=[], handler = None):
         self.iNames = iNames
         self.oNames = oNames
         self.fNames = fNames
         self.solutions = []
+        if len(spec.objectives)==1:
+            self.objectives=dict(zip(spec.objectives,[spec.objectives_val]))
+        else:
+            self.objectives=dict(zip(spec.objectives,spec.objectives_val))
+        self.eq_cstr=spec.dict_eq_cstr
+        self.ineq_cstr=spec.dict_ineq_cstr
         self.handler = handler #TODO : n'est plus utilisé. Modifier la création
         # automatique du Handler (dans constructeur Wrapper) lorsqu'il s'agit
         # d'un affichage dynamique : dynamicPlot.update
 
     def updateData(self, inp, out, freeOutputs=[]):
         """
         Adds the inputs and outputs of the model computed at each iteration to
```

### Comparing `noloadj-1.2.6/noloadj/optimization/multiobjective.py` & `noloadj-1.2.7/noloadj/optimization/multiobjective.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,43 +77,45 @@
                 res['fobj']=fobj
                 return res.items()
             return model_extended
         self.w.model=decorateur(model)
 
         self.optim_with_param(0.0,x0,options) #left
         [xM,ym]=self.pareto.pts[0] # normalisation
-        xM=(xM-self.fobjs_val[0][0])/(self.fobjs_val[0][1]-self.fobjs_val[0][0])
-        ym=(ym-self.fobjs_val[1][0])/(self.fobjs_val[1][1]-self.fobjs_val[1][0])
+        xmax,ymin=xM,ym
+        xM,ym=1.,0.
 
         self.optim_with_param(1.0,x0,options) #right
         [xm,yM]=self.pareto.pts[1] # normalisation
-        xm=(xm-self.fobjs_val[0][0])/(self.fobjs_val[0][1]-self.fobjs_val[0][0])
-        yM=(yM-self.fobjs_val[1][0])/(self.fobjs_val[1][1]-self.fobjs_val[1][0])
+        ymax,xmin=yM,xm
+        yM,xm=1.,0.
 
         otherspts=optimNb-2
         i=0 # initialisation de l'algorithme de dichotomie
         left,right=0,1
 
         while i<otherspts: #dichotomie
             param=(left+right)/2
             self.optim_with_param(param,x0,options)
             [xmid,ymid]=self.pareto.pts[i+2]
+            xmid,ymid=(xmid-xmin)/(xmax-xmin),(ymid-ymin)/(ymax-ymin)
             normidleft=np.sqrt((xM-xmid)**2+(ym-ymid)**2)
             normidright=np.sqrt((xm-xmid)**2+(yM-ymid)**2)
             if normidright<normidleft:
                 xm,yM=xmid,ymid
                 right=param
             else:
                 xM,ym=xmid,ymid
                 left=param
             i+=1
             x0=self.pareto.vars[-1] # dernier point calculé
 
         # à la fin
         self.w.model=model
+        self.exclude_dominated_points()
         self.w.resultsHandler=self.resultsHandler
         return self.pareto
 
 
     def optim_with_param(self,a,x0,options):
         '''
         Solves a ponderated objective optimization problem with
@@ -182,14 +184,15 @@
         #on reinitialise x0 à la valeur d'extremité du pareto trouvée au début.
         for i in range(1,optimNb-2):
             obj, point = getXorYmid(self.pareto.pts, normX, normY)
             x0 = self.modifySpec_Optim(x0, options, obj, point)
             #print("add a point :"+ str(obj) +" / " + str(point))
 
         #à la fin
+        self.exclude_dominated_points()
         self.w.resultsHandler = self.resultsHandler
         return self.pareto
 
     '''
     def optim2D_basic(self, x0, optimNb=10, options=None):
         """
         Solves a 2D optimization problem (with two objective functions) by
@@ -285,7 +288,23 @@
         out =[self.w.rawResults[vars] for vars in self.spec.oNames]
         fOut = [self.w.rawResults[vars] for vars in self.spec.freeOutputs]
         xopt = result.x
         self.resultsHandler.updateData(xopt, out, fOut)
         self.pareto.pts.append([out[0], out[1]])
         self.pareto.vars.append(xopt)
 
+    def exclude_dominated_points(self):
+        """Filters a list of points in the Pareto front to exclude any dominated points.
+        """
+        pareto_pts=self.pareto.pts
+        for i, point1 in enumerate(pareto_pts):
+            dominated = False
+            for j, point2 in enumerate(pareto_pts):
+                if i == j:
+                    continue
+                if all(p1 >= p2 for p1, p2 in zip(point1, point2)):
+                    dominated = True
+                    break
+            if dominated:
+                self.pareto.pts.pop(i)
+                self.pareto.vars.pop(i)
+                self.resultsHandler.solutions.pop(i)
```

### Comparing `noloadj-1.2.6/noloadj/optimization/optimProblem.py` & `noloadj-1.2.7/noloadj/optimization/optimProblem.py`

 * *Files 4% similar despite different names*

```diff
@@ -210,15 +210,19 @@
     bounds = wrapper.spec.bounds.T
 
     # https: // docs.scipy.org / doc / scipy / reference / generated /
     # scipy.optimize.least_squares.html
     result = scipyOpt.least_squares(fun=wrapper.f_val, x0=x0, bounds=bounds,
                                     jac=wrapper.f_grad,
                              ftol=options['ftol'], max_nfev=options['maxiter'])
-
+    result.x=denormalize(result.x,wrapper.spec.bounds)
+    result.fun=result.fun*(wrapper.spec.objectives_val[1]-
+        wrapper.spec.objectives_val[0])+wrapper.spec.objectives_val[0]
+    result.grad=result.grad*(wrapper.spec.objectives_val[1]-
+        wrapper.spec.objectives_val[0])+wrapper.spec.objectives_val[0]
     if (not result.success or options['disp']):  # TODO gérer une exception
         print(result.message)
         print("Solution found: ", result.x)
         print("Value of the cost function at the solution: ", result.cost)
         print("Vector of residuals at the solution: ", result.fun)
         print("Gradient of the cost function at the solution: ", result.grad)
```

### Comparing `noloadj-1.2.6/noloadj/optimization/paretoTools.py` & `noloadj-1.2.7/noloadj/optimization/paretoTools.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/noloadj/optimization/specifications.py` & `noloadj-1.2.7/noloadj/optimization/specifications.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import numpy as np
 from noloadj.optimization.Tools import *
 
 '''Define optimization specifications including objectives and constraints'''
 class Spec:
     """
+    dict_eq_cstr = dict including equality constraints
+    dict_ineq_cstr = dict including inequality constraints
     iNames = list including names of optimization variables
     bounds = list including range of values of optimization variables
     xinit = list including initial values of the optimization variables
     xinit_sh = list including shape of the optimization variables
     objectives = list including names of objective functions
     objectives_val = list including bounds of objective functions
     eq_cstr = list including names of equality constraints
@@ -20,14 +22,16 @@
     ineq_cstr_bnd : class StructList including bounds of inequality constraints
     freeOutputs = list of outputs to monitor
     nb = int number of  output variables (objective functions + constraints)
     oNames = list including names of output variables
     oShape = list giving the dimension of each output (objectives + constraints)
     nb_outputs = int number of output variables(objective functions+constraints)
     """
+    dict_eq_cstr = {} # dictionnaire des contraintes d'egalite
+    dict_ineq_cstr = {} # dictionnaire des contraintes d'inegalite
     iNames      = []  #noms des variables d'optimisation
     bounds      = []  #domaine de recherche
     xinit       = []  #valeurs initiales du vecteur d'optimisation
     xinit_sh    = [] # shape des valeurs d'optimization
     objectives  = []  #noms des objectifs
     objectives_val = [] # bornes des objectifs
     eq_cstr     = []  #noms des contraintes d'équalité
@@ -43,14 +47,16 @@
     nb_sorties  = 0  # nombre de variables de sorties (fonctions objectives +
     # contraintes)
     debug = False
 
 
     def __init__(self, variables, bounds, objectives, eq_cstr={}, ineq_cstr={},
                  freeOutputs=[],debug=False):
+        self.dict_eq_cstr=eq_cstr
+        self.dict_ineq_cstr=ineq_cstr
         self.iNames = list(variables.keys())
         xinit=list(variables.values())
         x0 = StructList(xinit)
         self.xinit_sh = x0.shape
         bounds=list(bounds.values())
         if self.xinit_sh != [0] * len(x0.List) or bounds!=[]:
             bnds = bounds
```

### Comparing `noloadj-1.2.6/noloadj/optimization/wrapper.py` & `noloadj-1.2.7/noloadj/optimization/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         self.model = model # fonction du modèle où l'on calcule les fonctions
         # objectives et contraintes
         self.p = parameters # paramètres constants du modèle (optionnel)
         self.spec = specifications # les performances désirées (fonctions
         # objectives, contraintes)
         if resultsHandler==True: # permet de sauvegarder les résultats au fur
             # et à mesure (optionnel)
-            self.resultsHandler = Iterations(specifications.iNames,
+            self.resultsHandler = Iterations(self.spec,specifications.iNames,
                                              specifications.oNames,
                                              specifications.freeOutputs)
             self.ParetoList=[]
 #        elif resultsHandler != None:
 #            self.resultsHandler = resultsHandler
         #else : no resultHandler => no iteration history
 
@@ -180,15 +180,15 @@
         self.compute_model=jit(self.compute_model) # on accélère le calcul du
         # modèle pour améliorer les performances
         #if self.spec.nb_entrees>=self.spec.nb_sorties: # s'il y a plus
             # d'entrées que de sorties dans le modèle
             #self.Jac_model=jit(jacrev(self.compute_model)) # on utilise le
             # mode "reverse" de la différentiation automatique
         #else: # s'il y a plus  de sorties que d'entrées dans le modèle
-        self.Jac_model=jit(jacfwd(self.compute_model)) # on utilise le
+        self.Jac_model=jit(jacfwd(self.compute_model_jac)) # on utilise le
             # mode "forward" de la différentiation automatique
         
     ## 3 fonctions pour récupérer les VALEURS des objectifs et contraintes
 
     def f_val(self, x):
         """
         Gets the value of the objective function evaluated in x according to
@@ -487,17 +487,16 @@
             res = self.model(**xList, **self.p) # on calcule le modèle
             # (entrées + fonctions objectives + contraintes)
         else: # s'il n'y a pas des paramètres constants
             res = self.model(**xList) # on calcule le modèle (entrées +
             # fonctions objectives + contraintes)
         dico = {k: v for k, v in res.__iter__()}  # conversion en dictionnaire
         for name in list(dico.keys()):#pour retirer les types 'function'/ class'
-            if not isinstance(dico[name],(int,float,list,
-                jax.interpreters.partial_eval.DynamicJaxprTracer,
-                        jax.interpreters.ad.JVPTracer)):
+            if hasattr(dico[name],'__dict__') or isinstance(dico[name],
+                                                            (dict,tuple,str)):
                 del dico[name]
         out=[]
         for vars in self.spec.oNames:
             try:
                 if vars not in list(dico.keys()):
                     raise KeyError(vars) #si la variable du cahier des charges
             except KeyError: # n'appartient pas aux sorties du modèle
@@ -537,17 +536,64 @@
                     var=StructList(x,'flattened',self.spec.xinit_sh)
                     self.resultsHandler.updateData(var.unflatten(),out,fData)
                 else:
                     self.resultsHandler.updateData(x,out,fData)
                 # on ajoute au resultsHandler le vecteur des entrées x et le
                 # vecteur des sorties out
             return out2
-        if not isinstance(x[0],jax.interpreters.ad.JVPTracer):
-            output_type=jax.ShapeDtypeStruct(out2.shape,out2.dtype)
-            out2=jax.pure_callback(save_dico,output_type,x,out,dico,out2)
+
+        output_type=jax.ShapeDtypeStruct(out2.shape,out2.dtype)
+        out2=jax.pure_callback(save_dico,output_type,x,out,dico,out2)
+        return out2 # renvoie la sortie sous forme de jax.numpy array
+
+    def compute_model_jac(self, x):
+        """
+        Computes the model outputs jacobians (objective function + constraints) in x.
+        :param x: the vector of optimization variables
+        :return: returns a "flattened" vector out including the model outputs
+        """
+        if self.spec.bounds!=[]:
+            x = denormalize(x, self.spec.bounds)
+        if len(self.spec.iNames)==1 and len(x)!=1:
+            xList = dict(zip(self.spec.iNames, [x]))
+        elif self.spec.xinit_sh != [0] * len(self.spec.iNames) and \
+                self.spec.xinit_sh != []:
+            var = StructList(x, 'flattened', self.spec.xinit_sh)
+            xList = dict(zip(self.spec.iNames, var.unflatten()))
+        else:
+            xList = dict(zip(self.spec.iNames, x))
+        if self.p != {}: # s'il y a des paramètres constants
+            res = self.model(**xList, **self.p) # on calcule le modèle
+            # (entrées + fonctions objectives + contraintes)
+        else: # s'il n'y a pas des paramètres constants
+            res = self.model(**xList) # on calcule le modèle (entrées +
+            # fonctions objectives + contraintes)
+        dico = {k: v for k, v in res.__iter__()}  # conversion en dictionnaire
+        for name in list(dico.keys()):#pour retirer les types 'function'/ class'
+            if hasattr(dico[name],'__dict__') or isinstance(dico[name],
+                                                            (dict,tuple,str)):
+                del dico[name]
+        out=[]
+        for vars in self.spec.oNames:
+            try:
+                if vars not in list(dico.keys()):
+                    raise KeyError(vars) #si la variable du cahier des charges
+            except KeyError: # n'appartient pas aux sorties du modèle
+                print('Warning :',vars,'is not in model')
+                pass
+            else:
+                out.append(dico[vars])
+        for i in range(len(out)): # si les contraintes sont sous la forme
+            # np.array
+            if jnp.size(jnp.array(out[i]))!=1:
+                out[i]=list(out[i]) # on les décompose pour les mettre sous
+                # forme de list
+        out1 = StructList(out)  # on récupère les sorties du modèle
+        self.resultsShape = out1.shape
+        out2 = jnp.array(out1.flatten()) # on aplatit les sorties du modèle
         return out2 # renvoie la sortie sous forme de jax.numpy array
 
 
     def solution(self):
         """
         Returns the model inputs computed at the last iteration of the algorithm
         :return: list of model inputs
```

### Comparing `noloadj-1.2.6/noloadj/tutorial/01-UnconstrainedMonoObjective.py` & `noloadj-1.2.7/noloadj/tutorial/01-UnconstrainedMonoObjective.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/noloadj/tutorial/02-ConstrainedMonoObjective.py` & `noloadj-1.2.7/noloadj/tutorial/02-ConstrainedMonoObjective.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/noloadj/tutorial/03-ConstrainedMultiObjective.py` & `noloadj-1.2.7/noloadj/tutorial/03-ConstrainedMultiObjective.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/noloadj/tutorial/04-ConstrainedMonoObjective2.py` & `noloadj-1.2.7/noloadj/tutorial/04-ConstrainedMonoObjective2.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/noloadj/tutorial/plotTools.py` & `noloadj-1.2.7/noloadj/tutorial/plotTools.py`

 * *Files identical despite different names*

### Comparing `noloadj-1.2.6/noloadj.egg-info/PKG-INFO` & `noloadj-1.2.7/noloadj.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noloadj
-Version: 1.2.6
+Version: 1.2.7
 Summary: solving constrained optimization problem for the design of engineering systems
 Author: B. DELINCHANT, L. GERBAUD, F. WURTZ, L.AGOBERT
 Author-email: benoit.delinchant@G2ELab.grenoble-inp.fr
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering
@@ -24,15 +24,21 @@
 We are happy that you will use or develop the NoLOAD_Jax.
 It is an **Open Source** project located on GitLab at https://gricad-gitlab.univ-grenoble-alpes.fr/design_optimization/NoLoad_v2
 It aims at **solving constrained optimization** problem for the design of engineering systems
 
 Project Presentation
 ====================
 
-**NoLOAD_Jax:** Please have a look to NoLOAD presentation : https://noload_jax.readthedocs.io/en/latest/  
+**NoLOAD_Jax:** Please have a look to NoLOAD presentation : https://noload-jax.readthedocs.io/en/latest/
+
+A scientific article presenting NoLOAD is available here:
+
+Agobert Lucas, Hodencq Sacha, Delinchant Benoit, Gerbaud Laurent, Frederic Wurtz, “NoLOAD, Open Software for Optimal Design and Operation using Automatic Differentiation”, OIPE 2020, Poland, 09-2021. https://hal.archives-ouvertes.fr/hal-03352443
+
+Please cite us when you use NoLOAD.
 
 NoLOAD_Jax Community
 ====================
 
 Please use the git issues system to report an error: https://gricad-gitlab.univ-grenoble-alpes.fr/design_optimization/NoLoad_v2
 Otherwise you can also contact the developer team using the following email adress: benoit.delinchant@G2ELab.grenoble-inp.fr
 
@@ -41,35 +47,34 @@
 You can install the library as a user or as a developer. Please follow the corresponding installation steps below.
 
 Prerequisite
 ------------
 
 Please install Python 3.8 or later
 https://www.python.org/downloads/
-You must run NoLOAD_Jax on Ubuntu : on Jupyter Notebook on a computer using Ubuntu, or as explained later, using WSL (Windows Subsystem for Linux) if your computer works on Windows.
-As it uses the JAX library, NoLOAD_Jax can run on CPU (Central Processor Unit) or GPU (Graphics Processor Unit), where GPU offers better performances than CPU.
-With WSL only CPU can be used. To use GPU you may run NoLOAD on Ubuntu.
-If you want to use GPU, you need to install CUDA and CuDNN on your computer then tape on Pycharm terminal (where 0.3.XX is your JAX version):
 
-    pip install --upgrade pip
-    pip install --upgrade jax jaxlib==0.3.XX+cuda111 -f https://storage.googleapis.com/jax-releases/jax_releases.html
-    
-If you use GPU, you need to put these lines at the beginning of your "optimization" file to avoid memory issues :
+Windows
+-------
 
-    import os
-    os.environ['XLA_PYTHON_CLIENT_PREALLOCATE']='false'
-    os.environ['XLA_PYTHON_CLIENT_MEM_FRACTION']='0.50'
-    
-To install IPOPT algorithm, please install an Anaconda environment and run this command on a terminal :
+The simplest way to install it
+------------------------------
+Go on  https://whls.blob.core.windows.net/unstable/index.html and download the cpu/jaxlib-0.3.25-cp3X-cp3X-win_amd64.whl, where 3.X is your Python version.
+Put it in your Python environment and tape on a terminal :
+
+    pip install cpu/jaxlib-0.3.25-cp3X-cp3X-win_amd64.whl
+    pip install jax==0.3.25
+    pip install noloadj
+
+The Jax version installed is not the newest one, but it is sufficient to use Noload_Jax.
 
-    conda install -c conda-forge cyipopt
     
-How to configure a virtual environment on WSL running with a Ubuntu distribution :
-----------------------
-At first, activate the WSL on you computer and install on it a Ubuntu distribution by following the 6 first steps of the link :
+How to configure a virtual environment on WSL running with an Ubuntu distribution :
+------------------------------
+The alternative to get Jax last versions is to install a virtual environment on WSL running with an Ubuntu distribution.
+At first, activate the WSL on you computer and install on it an Ubuntu distribution by following the 6 first steps of the link :
 https://docs.microsoft.com/en-us/windows/wsl/install-win10
 
 Then open WSL.exe using the Windows search bar and tape :
 
     cd ~
     sudo apt update
     sudo apt install python3-pip
@@ -86,40 +91,57 @@
 Choose WSL option then change the Python interpreter path by /home/_your_username_/pythonenv/bin/python3. (_your_username_ is the login you chose for WSL)
 Close the Settings window. Click on Terminal section at the bottom, and tape on the commande line  :
 
     source /home/your_username/pythonenv/bin/activate
 
 If you see a "(pythonenv)" written at the beginning of the command line, the configuration is completed and you can run your code now !
 
-Installation as a user
-----------------------
+Linux
+-----
 Please install NoLOAD_Jax with pip using the command prompt.   
 
-If you are admin on Windows or working on a virtual environment
+If you are working on a virtual environment on Linux
     
     pip install noloadj
 
 If you want a local installation or you are not admin
     
     pip install --user noloadj
 
 If you are admin on Linux:
     
     sudo pip install noloadj
 
 Launch the examples to understand how the NoLOAD_Jax works:
 	
-	python noload/01-UnconstrainedMonoObjective.py
-	python noload/02-ConstrainedMonoObjective.py
-	python noload/03-ConstrainedMultiObjective.py
-	python noload/04-ConstrainedMonoObjective2.py
+	python noloadj/01-UnconstrainedMonoObjective.py
+	python noloadj/02-ConstrainedMonoObjective.py
+	python noloadj/03-ConstrainedMultiObjective.py
+	python noloadj/04-ConstrainedMonoObjective2.py
 	
 Enjoy your time using NoLOAD_Jax !
 
+GPU & IPOPT Algorithm
+---------------------
+As it uses the JAX library, NoLOAD_Jax can run on CPU (Central Processor Unit) or GPU (Graphics Processor Unit), where GPU offers better performances than CPU.
+With WSL only CPU can be used. To use GPU you may run NoLOAD on Ubuntu.
+If you want to use GPU, you need to install CUDA and CuDNN on your computer then tape on Pycharm terminal (where 0.3.XX is your JAX version):
 
+    pip install --upgrade pip
+    pip install --upgrade jax jaxlib==0.3.XX+cuda111 -f https://storage.googleapis.com/jax-releases/jax_releases.html
+    
+If you use GPU, you need to put these lines at the beginning of your "optimization" file to avoid memory issues :
+
+    import os
+    os.environ['XLA_PYTHON_CLIENT_PREALLOCATE']='false'
+    os.environ['XLA_PYTHON_CLIENT_MEM_FRACTION']='0.50'
+    
+To install IPOPT algorithm, please install an Anaconda environment and run this command on a terminal :
+
+    conda install -c conda-forge cyipopt
 
 Library Installation Requirements
 ---------------------------------
 Matplotlib >= 3.0
 Scipy >= 1.2
 Jax >= 0.3.25
 Jaxlib >= 0.3.25
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `noloadj-1.2.6/noloadj.egg-info/SOURCES.txt` & `noloadj-1.2.7/noloadj.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 docs/new_features/v1.2.1.rst
 docs/new_features/v1.2.15.rst
 docs/new_features/v1.2.2.rst
 docs/new_features/v1.2.3.rst
 docs/new_features/v1.2.4.rst
 docs/new_features/v1.2.5.rst
 docs/new_features/v1.2.6.rst
+docs/new_features/v1.2.7.rst
 noloadj/__init__.py
 noloadj.egg-info/PKG-INFO
 noloadj.egg-info/SOURCES.txt
 noloadj.egg-info/dependency_links.txt
 noloadj.egg-info/requires.txt
 noloadj.egg-info/top_level.txt
 noloadj/ODE/ode45.py
```

### Comparing `noloadj-1.2.6/setup.py` & `noloadj-1.2.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 # SPDX-FileCopyrightText: 2021 G2Elab / MAGE
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """
 NoLOAD_Jax installation script
-:version: 1.2.6
+:version: 1.2.7
 """
 
 from setuptools import setup, find_packages
 
 # ------------------------------------------------------------------------------
 
 # Module version
-__version_info__ = (1, 2, 6)
+__version_info__ = (1, 2, 7)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 #__docformat__ = "restructuredtext en"
 
 # ------------------------------------------------------------------------------
 
@@ -35,15 +35,15 @@
               "noloadj.optimization",
               "noloadj.tutorial",
               ],
     author="B. DELINCHANT, L. GERBAUD, F. WURTZ, L.AGOBERT",
     author_email='benoit.delinchant@G2ELab.grenoble-inp.fr',
     description="solving constrained optimization problem for the design of engineering systems",
     long_description_content_type='text/markdown',
-    long_description=open('README.md').read(),
+    long_description=open('README.md',encoding='UTF-8').read(),
     install_requires=[
         "Matplotlib >3.0",
         "Scipy >= 1.2",
         "Jax >= 0.3.25",
         "Jaxlib >= 0.3.25",
         "Pandas >= 1.3.5"
     ],
```

