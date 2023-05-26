# Comparing `tmp/django-ows-lib-0.3.0.tar.gz` & `tmp/django-ows-lib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ows-lib-0.3.0.tar", last modified: Thu May 25 07:04:40 2023, max compression
+gzip compressed data, was "django-ows-lib-0.4.0.tar", last modified: Fri May 26 08:54:34 2023, max compression
```

## Comparing `django-ows-lib-0.3.0.tar` & `django-ows-lib-0.4.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.822106 django-ows-lib-0.3.0/django_ows_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-25 07:04:40.000000 django-ows-lib-0.3.0/django_ows_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-25 07:04:40.000000 django-ows-lib-0.3.0/django_ows_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:04:40.000000 django-ows-lib-0.3.0/django_ows_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-25 07:04:40.000000 django-ows-lib-0.3.0/django_ows_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 07:04:40.000000 django-ows-lib-0.3.0/django_ows_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.822106 django-ows-lib-0.3.0/ows_lib/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.822106 django-ows-lib-0.3.0/ows_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.822106 django-ows-lib-0.3.0/ows_lib/client/csw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/csw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/csw/csw202.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/csw/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.822106 django-ows-lib-0.3.0/ows_lib/client/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/wfs/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/wfs/wfs200.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.822106 django-ows-lib-0.3.0/ows_lib/client/wms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/wms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/wms/wms111.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/client/wms/wms130.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.822106 django-ows-lib-0.3.0/ows_lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/models/ogc_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.822106 django-ows-lib-0.3.0/ows_lib/xml_mapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/csw/
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/csw/csw202.py
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wfs/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wfs/wfs200.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wms/wms111.py
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wms/wms130.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/gml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/gml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/gml/gml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/iso_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/iso_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16727 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/iso_metadata/iso_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_requests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_requests/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_requests/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/csw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/csw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/csw/get_records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:04:40.826106 django-ows-lib-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-25 07:04:39.000000 django-ows-lib-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.119247 django-ows-lib-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-26 08:54:34.119247 django-ows-lib-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/django_ows_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-26 08:54:34.000000 django-ows-lib-0.4.0/django_ows_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-26 08:54:34.000000 django-ows-lib-0.4.0/django_ows_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:54:34.000000 django-ows-lib-0.4.0/django_ows_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 08:54:34.000000 django-ows-lib-0.4.0/django_ows_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 08:54:34.000000 django-ows-lib-0.4.0/django_ows_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/client/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/csw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/csw/csw202.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/csw/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/client/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/wfs/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/wfs/wfs200.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/client/wms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/wms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/wms/wms111.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/wms/wms130.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/models/ogc_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/xml_mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/csw/csw202.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wfs/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wfs/wfs200.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wms/wms111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wms/wms130.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/xml_mapper/gml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/gml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/gml/gml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/xml_mapper/iso_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/iso_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16727 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/iso_metadata/iso_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_requests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.119247 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_requests/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_requests/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.119247 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.119247 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/csw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/csw/get_records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.119247 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:54:34.119247 django-ows-lib-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/setup.py
```

### Comparing `django-ows-lib-0.3.0/LICENSE` & `django-ows-lib-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/PKG-INFO` & `django-ows-lib-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ows-lib
-Version: 0.3.0
+Version: 0.4.0
 Summary: Well layered ows lib with a client implementation to communicate with ogc services with django based objects, including xml mapper classes to serialize and deserialize ows xml files, such as capabilities.
 Home-page: https://github.com/mrmap-community/django-ows-lib
 Author: mrmap-community
 Author-email: jonas.kiefer@live.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-ows-lib-0.3.0/README.rst` & `django-ows-lib-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/django_ows_lib.egg-info/PKG-INFO` & `django-ows-lib-0.4.0/django_ows_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ows-lib
-Version: 0.3.0
+Version: 0.4.0
 Summary: Well layered ows lib with a client implementation to communicate with ogc services with django based objects, including xml mapper classes to serialize and deserialize ows xml files, such as capabilities.
 Home-page: https://github.com/mrmap-community/django-ows-lib
 Author: mrmap-community
 Author-email: jonas.kiefer@live.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-ows-lib-0.3.0/django_ows_lib.egg-info/SOURCES.txt` & `django-ows-lib-0.4.0/django_ows_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/client/csw/mixins.py` & `django-ows-lib-0.4.0/ows_lib/client/csw/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/client/enums.py` & `django-ows-lib-0.4.0/ows_lib/client/enums.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/client/exceptions.py` & `django-ows-lib-0.4.0/ows_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/client/mixins.py` & `django-ows-lib-0.4.0/ows_lib/client/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/client/utils.py` & `django-ows-lib-0.4.0/ows_lib/client/utils.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/client/wfs/mixins.py` & `django-ows-lib-0.4.0/ows_lib/client/wfs/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/client/wms/mixins.py` & `django-ows-lib-0.4.0/ows_lib/client/wms/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/models/ogc_request.py` & `django-ows-lib-0.4.0/ows_lib/models/ogc_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Dict, List
 
 from django.contrib.gis.geos import GEOSGeometry
+from django.http.request import HttpRequest as DjangoRequest
 from eulxml.xmlmap import XmlObject, load_xmlobject_from_string
 from requests import Request
 
 from ows_lib.client.enums import OGCOperationEnum
 from ows_lib.client.exceptions import MissingBboxParam, MissingServiceParam
 from ows_lib.client.utils import (construct_polygon_from_bbox_query_param,
                                   get_requested_feature_types,
@@ -13,16 +14,17 @@
 from ows_lib.xml_mapper.xml_requests.wfs.get_feature import (GetFeatureRequest,
                                                              Query)
 
 
 class OGCRequest(Request):
     """Extended Request class which provides some analyzing functionality for ogc requests."""
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, django_request: DjangoRequest = None, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
+        self._djano_request = django_request
         self._ogc_query_params: Dict = {}
         self._bbox: GEOSGeometry = None
         self._requested_entities: List[str] = []
         self._xml_request: XmlObject = None
 
         if self.method == "GET":
             self.operation: str = self.ogc_query_params.get("REQUEST", "")
@@ -33,14 +35,27 @@
             post_request: PostRequest = load_xmlobject_from_string(
                 string=self.data, xmlclass=PostRequest)
 
             self.operation: str = post_request.operation
             self.service_version: str = post_request.version
             self.service_type: str = post_request.service_type
 
+    @classmethod
+    def from_django_request(cls, request: DjangoRequest):
+        """helper function to construct an OGCRequest from a django request object."""
+        ogc_request = cls(
+            method=request.method,
+            url=request.build_absolute_uri(),
+            params={**request.GET, **request.POST},
+            data=request.body,
+            cookies=request.COOKIES,
+            django_request=request
+        )
+        return ogc_request
+
     @property
     def requested_entities(self) -> List[str]:
         """Returns the list of requested entities
 
         This function analyzes the request and find out which layers or featuretypes are requests.
 
         :return: list of requested layers | list of request featuretypes
```

### Comparing `django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/csw/csw202.py` & `django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/csw/csw202.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/mixins.py` & `django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wfs/mixins.py` & `django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wfs/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wfs/wfs200.py` & `django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wfs/wfs200.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wms/mixins.py` & `django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wms/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wms/wms111.py` & `django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wms/wms111.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/xml_mapper/capabilities/wms/wms130.py` & `django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wms/wms130.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/xml_mapper/iso_metadata/iso_metadata.py` & `django-ows-lib-0.4.0/ows_lib/xml_mapper/iso_metadata/iso_metadata.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/xml_mapper/mixins.py` & `django-ows-lib-0.4.0/ows_lib/xml_mapper/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/xml_mapper/namespaces.py` & `django-ows-lib-0.4.0/ows_lib/xml_mapper/namespaces.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/xml_mapper/utils.py` & `django-ows-lib-0.4.0/ows_lib/xml_mapper/utils.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py` & `django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/csw/get_records.py` & `django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/csw/get_records.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py` & `django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py` & `django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.3.0/setup.py` & `django-ows-lib-0.4.0/setup.py`

 * *Files identical despite different names*

