# Comparing `tmp/django-ows-lib-0.4.0.tar.gz` & `tmp/django-ows-lib-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ows-lib-0.4.0.tar", last modified: Fri May 26 08:54:34 2023, max compression
+gzip compressed data, was "django-ows-lib-0.4.1.tar", last modified: Fri May 26 10:13:36 2023, max compression
```

## Comparing `django-ows-lib-0.4.0.tar` & `django-ows-lib-0.4.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.119247 django-ows-lib-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-26 08:54:34.119247 django-ows-lib-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/django_ows_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-26 08:54:34.000000 django-ows-lib-0.4.0/django_ows_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-26 08:54:34.000000 django-ows-lib-0.4.0/django_ows_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:54:34.000000 django-ows-lib-0.4.0/django_ows_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 08:54:34.000000 django-ows-lib-0.4.0/django_ows_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 08:54:34.000000 django-ows-lib-0.4.0/django_ows_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/client/csw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/csw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/csw/csw202.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/csw/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/client/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/wfs/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/wfs/wfs200.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/client/wms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/wms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/wms/wms111.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/client/wms/wms130.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/models/ogc_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/xml_mapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/csw/
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/csw/csw202.py
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wfs/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wfs/wfs200.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wms/wms111.py
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wms/wms130.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/xml_mapper/gml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/gml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/gml/gml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/xml_mapper/iso_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/iso_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16727 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/iso_metadata/iso_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.115246 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_requests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.119247 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_requests/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_requests/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.119247 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.119247 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/csw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/csw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/csw/get_records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:34.119247 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:54:34.119247 django-ows-lib-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-26 08:54:33.000000 django-ows-lib-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.326119 django-ows-lib-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-26 10:13:36.326119 django-ows-lib-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.318119 django-ows-lib-0.4.1/django_ows_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-26 10:13:36.000000 django-ows-lib-0.4.1/django_ows_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-26 10:13:36.000000 django-ows-lib-0.4.1/django_ows_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:13:36.000000 django-ows-lib-0.4.1/django_ows_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 10:13:36.000000 django-ows-lib-0.4.1/django_ows_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 10:13:36.000000 django-ows-lib-0.4.1/django_ows_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.318119 django-ows-lib-0.4.1/ows_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.318119 django-ows-lib-0.4.1/ows_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.318119 django-ows-lib-0.4.1/ows_lib/client/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/client/csw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/client/csw/csw202.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/client/csw/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/client/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/client/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.318119 django-ows-lib-0.4.1/ows_lib/client/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/client/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/client/wfs/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/client/wfs/wfs200.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.318119 django-ows-lib-0.4.1/ows_lib/client/wms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/client/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/client/wms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/client/wms/wms111.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/client/wms/wms130.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.318119 django-ows-lib-0.4.1/ows_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/models/ogc_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.322119 django-ows-lib-0.4.1/ows_lib/xml_mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.322119 django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.322119 django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/csw/csw202.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.322119 django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/wfs/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/wfs/wfs200.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.322119 django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/wms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/wms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/wms/wms111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/wms/wms130.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.322119 django-ows-lib-0.4.1/ows_lib/xml_mapper/gml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/gml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/gml/gml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.322119 django-ows-lib-0.4.1/ows_lib/xml_mapper/iso_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/iso_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16938 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/iso_metadata/iso_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.322119 django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_requests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.322119 django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_requests/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_requests/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.322119 django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_responses/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.322119 django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_responses/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_responses/csw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_responses/csw/get_records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:36.326119 django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_responses/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_responses/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 10:13:36.326119 django-ows-lib-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-26 10:13:35.000000 django-ows-lib-0.4.1/setup.py
```

### Comparing `django-ows-lib-0.4.0/LICENSE` & `django-ows-lib-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/PKG-INFO` & `django-ows-lib-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ows-lib
-Version: 0.4.0
+Version: 0.4.1
 Summary: Well layered ows lib with a client implementation to communicate with ogc services with django based objects, including xml mapper classes to serialize and deserialize ows xml files, such as capabilities.
 Home-page: https://github.com/mrmap-community/django-ows-lib
 Author: mrmap-community
 Author-email: jonas.kiefer@live.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-ows-lib-0.4.0/README.rst` & `django-ows-lib-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/django_ows_lib.egg-info/PKG-INFO` & `django-ows-lib-0.4.1/django_ows_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ows-lib
-Version: 0.4.0
+Version: 0.4.1
 Summary: Well layered ows lib with a client implementation to communicate with ogc services with django based objects, including xml mapper classes to serialize and deserialize ows xml files, such as capabilities.
 Home-page: https://github.com/mrmap-community/django-ows-lib
 Author: mrmap-community
 Author-email: jonas.kiefer@live.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-ows-lib-0.4.0/django_ows_lib.egg-info/SOURCES.txt` & `django-ows-lib-0.4.1/django_ows_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/client/csw/mixins.py` & `django-ows-lib-0.4.1/ows_lib/client/csw/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/client/enums.py` & `django-ows-lib-0.4.1/ows_lib/client/enums.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/client/exceptions.py` & `django-ows-lib-0.4.1/ows_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/client/mixins.py` & `django-ows-lib-0.4.1/ows_lib/client/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/client/utils.py` & `django-ows-lib-0.4.1/ows_lib/client/utils.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/client/wfs/mixins.py` & `django-ows-lib-0.4.1/ows_lib/client/wfs/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/client/wms/mixins.py` & `django-ows-lib-0.4.1/ows_lib/client/wms/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/models/ogc_request.py` & `django-ows-lib-0.4.1/ows_lib/models/ogc_request.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/csw/csw202.py` & `django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/csw/csw202.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/mixins.py` & `django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wfs/mixins.py` & `django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/wfs/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wfs/wfs200.py` & `django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/wfs/wfs200.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wms/mixins.py` & `django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/wms/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wms/wms111.py` & `django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/wms/wms111.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/xml_mapper/capabilities/wms/wms130.py` & `django-ows-lib-0.4.1/ows_lib/xml_mapper/capabilities/wms/wms130.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/xml_mapper/iso_metadata/iso_metadata.py` & `django-ows-lib-0.4.1/ows_lib/xml_mapper/iso_metadata/iso_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,14 +279,15 @@
     """
     XSD_SCHEMA = "http://www.isotc211.org/2005/gmd"  # NOSONAR: the xml schema url will still be with insecure http protocol. To match all xml files, we need to let it as it is.
 
     ROOT_NAME = "MD_Metadata"
     ROOT_NS = GMD_NAMESPACE
     ROOT_NAMESPACES = {
         "gmd": GMD_NAMESPACE,
+        "gco": GCO_NAMESPACE
     }
 
     file_identifier = xmlmap.StringField(
         xpath="gmd:fileIdentifier/gco:CharacterString")
     # language = xmlmap.StringField(xpath=f"{NS_WC}identificationInfo']//{NS_WC}language']/{NS_WC}LanguageCode']")
     _hierarchy_level = xmlmap.StringField(
         xpath="gmd:hierarchyLevel/gmd:MD_ScopeCode[@codeList='http://standards.iso.org/ittf/PubliclyAvailableStandards/ISO_19139_Schemas/resources/codelist/ML_gmxCodelists.xml#MD_ScopeCode']/@codeListValue")
@@ -306,14 +307,22 @@
     def _get_child_identification(self):
         if self._md_data_identification:
             return self._md_data_identification
         elif self._sv_service_identification:
             return self._sv_service_identification
 
     @property
+    def is_dataset(self):
+        return self._hierarchy_level == "dataset"
+
+    @property
+    def is_service(self):
+        return self._hierarchy_level == "service"
+
+    @property
     def date_stamp(self):
         return self._date_stamp_date if self._date_stamp_date else self._date_stamp_date_time
 
     @date_stamp.setter
     def date_stamp(self, value):
         # TODO
         raise NotImplementedError()
```

### Comparing `django-ows-lib-0.4.0/ows_lib/xml_mapper/mixins.py` & `django-ows-lib-0.4.1/ows_lib/xml_mapper/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/xml_mapper/namespaces.py` & `django-ows-lib-0.4.1/ows_lib/xml_mapper/namespaces.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/xml_mapper/utils.py` & `django-ows-lib-0.4.1/ows_lib/xml_mapper/utils.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py` & `django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/csw/get_records.py` & `django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_responses/csw/get_records.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py` & `django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py` & `django-ows-lib-0.4.1/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.4.0/setup.py` & `django-ows-lib-0.4.1/setup.py`

 * *Files identical despite different names*

