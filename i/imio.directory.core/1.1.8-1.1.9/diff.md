# Comparing `tmp/imio.directory.core-1.1.8.tar.gz` & `tmp/imio.directory.core-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio.directory.core-1.1.8.tar", last modified: Fri Mar 31 10:02:54 2023, max compression
+gzip compressed data, was "dist/imio.directory.core-1.1.9.tar", last modified: Fri May 26 09:27:00 2023, max compression
```

## Comparing `imio.directory.core-1.1.8.tar` & `imio.directory.core-1.1.9.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.831768 imio.directory.core-1.1.8/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2883 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/CHANGES.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      128 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/CONTRIBUTORS.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      586 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/DEVELOP.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/LICENSE.GPL
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      670 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/LICENSE.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      106 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/MANIFEST.in
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8512 2023-03-31 10:02:54.831768 imio.directory.core-1.1.8/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4458 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/README.rst
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.811768 imio.directory.core-1.1.8/docs/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7996 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/docs/conf.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/docs/index.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/requirements.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-03-31 10:02:54.831768 imio.directory.core-1.1.8/setup.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2766 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/setup.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.751768 imio.directory.core-1.1.8/src/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.811768 imio.directory.core-1.1.8/src/imio/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.815768 imio.directory.core-1.1.8/src/imio/directory/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.819768 imio.directory.core-1.1.8/src/imio/directory/core/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      335 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.819768 imio.directory.core-1.1.8/src/imio/directory/core/browser/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/browser/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      972 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/browser/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1363 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/browser/import.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    11997 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/browser/import.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.819768 imio.directory.core-1.1.8/src/imio/directory/core/browser/overrides/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/browser/overrides/.gitkeep
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.819768 imio.directory.core-1.1.8/src/imio/directory/core/browser/static/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/browser/static/.gitkeep
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      897 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/browser/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       53 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/config.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      958 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.823768 imio.directory.core-1.1.8/src/imio/directory/core/contents/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      107 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/contents/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      136 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/contents/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.823768 imio.directory.core-1.1.8/src/imio/directory/core/contents/contact/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/contents/contact/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1536 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/contents/contact/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10801 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/contents/contact/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2011 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/contents/contact/forms.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2808 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/contents/contact/serializer.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4136 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/contents/contact/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1737 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/contents/contact/view.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.823768 imio.directory.core-1.1.8/src/imio/directory/core/contents/entity/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/contents/entity/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      322 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/contents/entity/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      851 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/contents/entity/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      487 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/converters.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.803768 imio.directory.core-1.1.8/src/imio/directory/core/faceted/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.823768 imio.directory.core-1.1.8/src/imio/directory/core/faceted/config/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7958 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/faceted/config/entity.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3215 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/indexers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1357 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/indexers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      284 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/interfaces.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1070 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/monkey.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      668 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/monkey.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      350 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/overrides.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      640 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/permissions.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.807768 imio.directory.core-1.1.8/src/imio/directory/core/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.827768 imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1538 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/actions.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      182 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2099 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      730 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      661 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/registry.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      456 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.827768 imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/taxonomies/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      325 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/taxonomies/contact_category.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    89861 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/taxonomies/contact_category.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.827768 imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1884 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/types/imio.directory.Contact.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1598 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/types/imio.directory.Entity.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      242 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/types.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.827768 imio.directory.core-1.1.8/src/imio/directory/core/profiles/testing/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      162 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/profiles/testing/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      507 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/profiles/testing/registry.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.827768 imio.directory.core-1.1.8/src/imio/directory/core/profiles/uninstall/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      129 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1218 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/profiles.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      785 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/setuphandlers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1823 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/subscribers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      617 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/subscribers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1825 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/testing.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.831768 imio.directory.core-1.1.8/src/imio/directory/core/tests/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/tests/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.831768 imio.directory.core-1.1.8/src/imio/directory/core/tests/resources/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1802 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/tests/resources/json_contact.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9847 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/tests/resources/logo.png
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.831768 imio.directory.core-1.1.8/src/imio/directory/core/tests/robot/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2007 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/tests/robot/test_example.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    15994 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/tests/test_contact.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1530 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/tests/test_cropping.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3437 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/tests/test_entity.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1591 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/tests/test_local_roles.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8598 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/tests/test_multilingual.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      930 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/tests/test_robot.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2026 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/tests/test_setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2986 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/tests/test_utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2709 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/tests/test_vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      271 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/tests/utils.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.831768 imio.directory.core-1.1.8/src/imio/directory/core/upgrades/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/upgrades/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4024 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/upgrades/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.807768 imio.directory.core-1.1.8/src/imio/directory/core/upgrades/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.807768 imio.directory.core-1.1.8/src/imio/directory/core/upgrades/profiles/1003_to_1004/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.831768 imio.directory.core-1.1.8/src/imio/directory/core/upgrades/profiles/1003_to_1004/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      290 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/upgrades/profiles/1003_to_1004/types/imio.directory.Entity.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.831768 imio.directory.core-1.1.8/src/imio/directory/core/upgrades/profiles/1006_to_1007/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1066 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/upgrades/profiles/1006_to_1007/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7565 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/upgrades/upgrades.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2056 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3447 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1168 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio/directory/core/vocabularies.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-31 10:02:54.815768 imio.directory.core-1.1.8/src/imio.directory.core.egg-info/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8512 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio.directory.core.egg-info/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4031 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio.directory.core.egg-info/SOURCES.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio.directory.core.egg-info/dependency_links.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       20 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio.directory.core.egg-info/namespace_packages.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio.directory.core.egg-info/not-zip-safe
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      488 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio.directory.core.egg-info/requires.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-03-31 10:02:54.000000 imio.directory.core-1.1.8/src/imio.directory.core.egg-info/top_level.txt
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/
+-rw-r--r--   0 laurent    (501) staff       (20)     3216 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/CHANGES.rst
+-rw-r--r--   0 laurent    (501) staff       (20)      128 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/CONTRIBUTORS.rst
+-rw-r--r--   0 laurent    (501) staff       (20)      586 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/DEVELOP.rst
+-rw-r--r--   0 laurent    (501) staff       (20)    18092 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/LICENSE.GPL
+-rw-r--r--   0 laurent    (501) staff       (20)      670 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/LICENSE.rst
+-rw-r--r--   0 laurent    (501) staff       (20)      106 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/MANIFEST.in
+-rw-r--r--   0 laurent    (501) staff       (20)     8845 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/PKG-INFO
+-rw-r--r--   0 laurent    (501) staff       (20)     4458 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/README.rst
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)     7996 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/docs/conf.py
+-rw-r--r--   0 laurent    (501) staff       (20)       80 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/docs/index.rst
+-rw-r--r--   0 laurent    (501) staff       (20)       64 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/requirements.txt
+-rw-r--r--   0 laurent    (501) staff       (20)      518 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/setup.cfg
+-rw-r--r--   0 laurent    (501) staff       (20)     2766 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/setup.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/
+-rw-r--r--   0 laurent    (501) staff       (20)       80 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/
+-rw-r--r--   0 laurent    (501) staff       (20)       80 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/
+-rw-r--r--   0 laurent    (501) staff       (20)      335 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/browser/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/browser/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)      972 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/browser/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)     1363 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/browser/import.pt
+-rw-r--r--   0 laurent    (501) staff       (20)    11997 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/browser/import.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/browser/overrides/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/browser/overrides/.gitkeep
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/browser/static/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/browser/static/.gitkeep
+-rw-r--r--   0 laurent    (501) staff       (20)      897 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/browser/utils.py
+-rw-r--r--   0 laurent    (501) staff       (20)       53 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/config.py
+-rw-r--r--   0 laurent    (501) staff       (20)      958 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/configure.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/contents/
+-rw-r--r--   0 laurent    (501) staff       (20)      107 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/contents/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)      136 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/contents/configure.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/contents/contact/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/contents/contact/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1536 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/contents/contact/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)    10801 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/contents/contact/content.py
+-rw-r--r--   0 laurent    (501) staff       (20)     2011 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/contents/contact/forms.py
+-rw-r--r--   0 laurent    (501) staff       (20)     2796 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/contents/contact/serializer.py
+-rw-r--r--   0 laurent    (501) staff       (20)     4136 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/contents/contact/view.pt
+-rw-r--r--   0 laurent    (501) staff       (20)     1737 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/contents/contact/view.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/contents/entity/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/contents/entity/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)      322 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/contents/entity/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)      851 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/contents/entity/content.py
+-rw-r--r--   0 laurent    (501) staff       (20)      487 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/converters.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/faceted/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/faceted/config/
+-rw-r--r--   0 laurent    (501) staff       (20)     7958 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/faceted/config/entity.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     3215 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/indexers.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1357 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/indexers.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)      284 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/interfaces.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1070 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/monkey.py
+-rw-r--r--   0 laurent    (501) staff       (20)      668 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/monkey.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)      350 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/overrides.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)      640 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/permissions.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/
+-rw-r--r--   0 laurent    (501) staff       (20)     1538 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/actions.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      182 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/browserlayer.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     2099 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/catalog.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      730 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/metadata.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      661 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/registry.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      456 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/rolemap.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/taxonomies/
+-rw-r--r--   0 laurent    (501) staff       (20)      325 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/taxonomies/contact_category.cfg
+-rw-r--r--   0 laurent    (501) staff       (20)    92403 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/taxonomies/contact_category.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/types/
+-rw-r--r--   0 laurent    (501) staff       (20)     1884 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/types/imio.directory.Contact.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     1598 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/types/imio.directory.Entity.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      242 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/types.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/testing/
+-rw-r--r--   0 laurent    (501) staff       (20)      162 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/testing/metadata.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      507 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/testing/registry.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/uninstall/
+-rw-r--r--   0 laurent    (501) staff       (20)      129 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     1218 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/profiles.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)      785 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/setuphandlers.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1823 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/subscribers.py
+-rw-r--r--   0 laurent    (501) staff       (20)      617 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/subscribers.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)     1825 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/testing.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/resources/
+-rw-r--r--   0 laurent    (501) staff       (20)     1802 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/resources/json_contact.json
+-rw-r--r--   0 laurent    (501) staff       (20)     9847 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/resources/logo.png
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/robot/
+-rw-r--r--   0 laurent    (501) staff       (20)     2007 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/robot/test_example.robot
+-rw-r--r--   0 laurent    (501) staff       (20)    15994 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/test_contact.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1530 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/test_cropping.py
+-rw-r--r--   0 laurent    (501) staff       (20)     3437 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/test_entity.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1591 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/test_local_roles.py
+-rw-r--r--   0 laurent    (501) staff       (20)     8598 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/test_multilingual.py
+-rw-r--r--   0 laurent    (501) staff       (20)      930 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/test_robot.py
+-rw-r--r--   0 laurent    (501) staff       (20)     2026 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/test_setup.py
+-rw-r--r--   0 laurent    (501) staff       (20)     2986 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/test_utils.py
+-rw-r--r--   0 laurent    (501) staff       (20)     2709 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/test_vocabularies.py
+-rw-r--r--   0 laurent    (501) staff       (20)      271 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/tests/utils.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/upgrades/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/upgrades/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)     4024 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/upgrades/configure.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/upgrades/profiles/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/upgrades/profiles/1003_to_1004/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/upgrades/profiles/1003_to_1004/types/
+-rw-r--r--   0 laurent    (501) staff       (20)      290 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/upgrades/profiles/1003_to_1004/types/imio.directory.Entity.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio/directory/core/upgrades/profiles/1006_to_1007/
+-rw-r--r--   0 laurent    (501) staff       (20)     1066 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/upgrades/profiles/1006_to_1007/catalog.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     7565 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/upgrades/upgrades.py
+-rw-r--r--   0 laurent    (501) staff       (20)     2056 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/utils.py
+-rw-r--r--   0 laurent    (501) staff       (20)     3447 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/vocabularies.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1168 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio/directory/core/vocabularies.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-26 09:27:00.000000 imio.directory.core-1.1.9/src/imio.directory.core.egg-info/
+-rw-r--r--   0 laurent    (501) staff       (20)     8845 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio.directory.core.egg-info/PKG-INFO
+-rw-r--r--   0 laurent    (501) staff       (20)     4031 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio.directory.core.egg-info/SOURCES.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        1 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio.directory.core.egg-info/dependency_links.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       20 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio.directory.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        1 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio.directory.core.egg-info/not-zip-safe
+-rw-r--r--   0 laurent    (501) staff       (20)      488 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio.directory.core.egg-info/requires.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        5 2023-05-26 09:26:59.000000 imio.directory.core-1.1.9/src/imio.directory.core.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `imio.directory.core-1.1.8/CHANGES.rst` & `imio.directory.core-1.1.9/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 Changelog
 =========
 
 
+1.1.9 (2023-05-26)
+------------------
+
+- Fix condition when facing `Missing.Value` to avoid traceback in serializer
+  [laulaz]
+
+- WEB-3918 : Add missing DE translations for contact_category taxonomy
+  [laulaz]
+
+- Migrate to Plone 6.0.4
+  [boulch]
+
+- Update contact_category taxonomy data to reflect production site data
+  [laulaz]
+
+
 1.1.8 (2023-03-31)
 ------------------
 
 - WEB-3909 : Add upgrade step to fix wrongly stored datagrid fields values
   [laulaz]
```

### Comparing `imio.directory.core-1.1.8/DEVELOP.rst` & `imio.directory.core-1.1.9/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/LICENSE.GPL` & `imio.directory.core-1.1.9/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/LICENSE.rst` & `imio.directory.core-1.1.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/PKG-INFO` & `imio.directory.core-1.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.directory.core
-Version: 1.1.8
+Version: 1.1.9
 Summary: Core product for iMio contacts Directory websites
 Home-page: https://github.com/imio/imio.directory.core
 Author: Christophe Boulanger
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.directory.core
 Project-URL: Source, https://github.com/imio/imio.directory.core
@@ -187,14 +187,30 @@
 - Laurent Lasudry, laurent.lasudry@affinitic.be
 
 
 Changelog
 =========
 
 
+1.1.9 (2023-05-26)
+------------------
+
+- Fix condition when facing `Missing.Value` to avoid traceback in serializer
+  [laulaz]
+
+- WEB-3918 : Add missing DE translations for contact_category taxonomy
+  [laulaz]
+
+- Migrate to Plone 6.0.4
+  [boulch]
+
+- Update contact_category taxonomy data to reflect production site data
+  [laulaz]
+
+
 1.1.8 (2023-03-31)
 ------------------
 
 - WEB-3909 : Add upgrade step to fix wrongly stored datagrid fields values
   [laulaz]
```

### Comparing `imio.directory.core-1.1.8/README.rst` & `imio.directory.core-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/docs/conf.py` & `imio.directory.core-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/setup.cfg` & `imio.directory.core-1.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/setup.py` & `imio.directory.core-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.directory.core",
-    version="1.1.8",
+    version="1.1.9",
     description="Core product for iMio contacts Directory websites",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/browser/configure.zcml` & `imio.directory.core-1.1.9/src/imio/directory/core/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/browser/import.pt` & `imio.directory.core-1.1.9/src/imio/directory/core/browser/import.pt`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/browser/import.py` & `imio.directory.core-1.1.9/src/imio/directory/core/browser/import.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/browser/utils.py` & `imio.directory.core-1.1.9/src/imio/directory/core/browser/utils.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/configure.zcml` & `imio.directory.core-1.1.9/src/imio/directory/core/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/contents/contact/configure.zcml` & `imio.directory.core-1.1.9/src/imio/directory/core/contents/contact/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/contents/contact/content.py` & `imio.directory.core-1.1.9/src/imio/directory/core/contents/contact/content.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/contents/contact/forms.py` & `imio.directory.core-1.1.9/src/imio/directory/core/contents/contact/forms.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/contents/contact/serializer.py` & `imio.directory.core-1.1.9/src/imio/directory/core/contents/contact/serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,12 +60,12 @@
             value = getattr(obj, accessor, None)
             try:
                 if callable(value):
                     value = value()
             except WorkflowException:
                 summary[orig_field] = None
                 continue
-            if orig_field == "description" and value is not None:
+            if orig_field == "description" and value:
                 value = value.replace("**", "")
             summary[orig_field] = json_compatible(value)
 
         return summary
```

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/contents/contact/view.pt` & `imio.directory.core-1.1.9/src/imio/directory/core/contents/contact/view.pt`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/contents/contact/view.py` & `imio.directory.core-1.1.9/src/imio/directory/core/contents/contact/view.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/contents/entity/content.py` & `imio.directory.core-1.1.9/src/imio/directory/core/contents/entity/content.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/faceted/config/entity.xml` & `imio.directory.core-1.1.9/src/imio/directory/core/faceted/config/entity.xml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/indexers.py` & `imio.directory.core-1.1.9/src/imio/directory/core/indexers.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/indexers.zcml` & `imio.directory.core-1.1.9/src/imio/directory/core/indexers.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/monkey.py` & `imio.directory.core-1.1.9/src/imio/directory/core/monkey.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/monkey.zcml` & `imio.directory.core-1.1.9/src/imio/directory/core/monkey.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/permissions.zcml` & `imio.directory.core-1.1.9/src/imio/directory/core/permissions.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/actions.xml` & `imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/catalog.xml` & `imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/metadata.xml` & `imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/metadata.xml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/registry.xml` & `imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/taxonomies/contact_category.xml` & `imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/taxonomies/contact_category.xml`

 * *Files 2% similar despite different names*

#### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/taxonomies/contact_category.xml` & `imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/taxonomies/contact_category.xml`

```diff
@@ -9,14 +9,15 @@
     <caption>
       <langstring language="de">Geschäfte und Unternehmen</langstring>
       <langstring language="fr">Commerces et entreprises</langstring>
     </caption>
     <term>
       <termIdentifier>i09jveh714</termIdentifier>
       <caption>
+        <langstring language="de">Landwirtschaft</langstring>
         <langstring language="fr">Agriculture</langstring>
       </caption>
     </term>
     <term>
       <termIdentifier>hlsm9bijb1</termIdentifier>
       <caption>
         <langstring language="de">Nahrungsmittelgeschäfte</langstring>
@@ -224,27 +225,29 @@
       <caption>
         <langstring language="de">Kommunikation und Multimedia</langstring>
         <langstring language="fr">Communication et multimedia</langstring>
       </caption>
       <term>
         <termIdentifier>43962135gg</termIdentifier>
         <caption>
+          <langstring language="de">Agentur für Kommunikation</langstring>
           <langstring language="fr">Agence de communication</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>h3vsf8u3nv</termIdentifier>
         <caption>
           <langstring language="de">Comic-Buchhandlung</langstring>
           <langstring language="fr">Bande dessinée</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>8u3qc6u2i3</termIdentifier>
         <caption>
+          <langstring language="de">Grafiker/in</langstring>
           <langstring language="fr">Graphiste</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>v3c2dhpi7h</termIdentifier>
         <caption>
           <langstring language="de">Buchhandlung - Presse - Schreibwaren</langstring>
@@ -614,14 +617,15 @@
           <langstring language="de">Reinigungsunternehmen</langstring>
           <langstring language="fr">Entreprise de nettoyage</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>7774o3b4b4</termIdentifier>
         <caption>
+          <langstring language="de">Schlosserei</langstring>
           <langstring language="fr">Ferronnerie</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>o5a5c53ncl</termIdentifier>
         <caption>
           <langstring language="de">Blumenhändler</langstring>
@@ -648,52 +652,71 @@
           <langstring language="de">Bettwäsche</langstring>
           <langstring language="fr">Literie</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>hxmev56yg2</termIdentifier>
         <caption>
+          <langstring language="de">Baumaterial</langstring>
           <langstring language="fr">Matériel de construction</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>36ny59kxy4</termIdentifier>
         <caption>
+          <langstring language="de">Maurerarbeiten</langstring>
           <langstring language="fr">Maçonnerie</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>a6vcl1jfwb</termIdentifier>
         <caption>
+          <langstring language="de">Schreinerei</langstring>
           <langstring language="fr">Menuiserie</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>1d1mxx3w7i</termIdentifier>
         <caption>
           <langstring language="de">Mobiliar</langstring>
           <langstring language="fr">Mobilier</langstring>
         </caption>
       </term>
       <term>
+        <termIdentifier>ti22x1biwl</termIdentifier>
+        <caption>
+          <langstring language="de">Malerarbeiten</langstring>
+          <langstring language="fr">Peinture</langstring>
+        </caption>
+      </term>
+      <term>
         <termIdentifier>osqo095x3c</termIdentifier>
         <caption>
+          <langstring language="de">Bodenbelag</langstring>
           <langstring language="fr">Revêtement de sol</langstring>
         </caption>
       </term>
       <term>
+        <termIdentifier>gxirqs3ldi</termIdentifier>
+        <caption>
+          <langstring language="de">Solar- und Photovoltaikanlagen</langstring>
+          <langstring language="fr">Solaire et photovoltaïque</langstring>
+        </caption>
+      </term>
+      <term>
         <termIdentifier>2bvo1inf4p</termIdentifier>
         <caption>
           <langstring language="de">Dienstleistungsschecks</langstring>
           <langstring language="fr">Titres-services</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>n1pwe29524</termIdentifier>
         <caption>
+          <langstring language="de">Dachdeckerei und Isolierung</langstring>
           <langstring language="fr">Toiture et isolation</langstring>
         </caption>
       </term>
     </term>
     <term>
       <termIdentifier>usv28rqjti</termIdentifier>
       <caption>
@@ -769,44 +792,50 @@
       <caption>
         <langstring language="de">Landwirtschaft - Forstwirtschaft - Jagd - Fischerei</langstring>
         <langstring language="fr">Nature et forêts</langstring>
       </caption>
       <term>
         <termIdentifier>xlyiud5id3</termIdentifier>
         <caption>
+          <langstring language="de">Bienenzucht</langstring>
           <langstring language="fr">Apiculture</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>siyw79j07l</termIdentifier>
         <caption>
+          <langstring language="de">Jagd</langstring>
           <langstring language="fr">Chasse</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>v8dj1w45gp</termIdentifier>
         <caption>
+          <langstring language="de">Angeln</langstring>
           <langstring language="fr">Pêche</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>93nwskjb9a</termIdentifier>
         <caption>
+          <langstring language="de">Fischzucht</langstring>
           <langstring language="fr">Pisciculture</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>6d8i7irsoc</termIdentifier>
         <caption>
+          <langstring language="de">Sägewerk</langstring>
           <langstring language="fr">Scierie</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>toxrnabkl0</termIdentifier>
         <caption>
+          <langstring language="de">Forstwirtschaft</langstring>
           <langstring language="fr">Sylviculture - Exploitation forestière</langstring>
         </caption>
       </term>
     </term>
     <term>
       <termIdentifier>2ya5fa7v13</termIdentifier>
       <caption>
@@ -896,14 +925,15 @@
           <langstring language="de">Friterie</langstring>
           <langstring language="fr">Friterie</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>mff5h605eq</termIdentifier>
         <caption>
+          <langstring language="de">Fahrende Eisdiele</langstring>
           <langstring language="fr">Glacier ambulant</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>gl55dplfo0</termIdentifier>
         <caption>
           <langstring language="de">Hamburger</langstring>
@@ -1511,14 +1541,15 @@
           <langstring language="de">Vergnügungspark</langstring>
           <langstring language="fr">Parc d'attraction</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>na1o59kh5a</termIdentifier>
         <caption>
+          <langstring language="de">Sportwetten</langstring>
           <langstring language="fr">Paris sportifs</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>ro7mn6fyao</termIdentifier>
         <caption>
           <langstring language="de">Spielplatz im Freien</langstring>
@@ -1636,14 +1667,15 @@
           <langstring language="de">Psychologe</langstring>
           <langstring language="fr">Psychologue</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>y9eadd4jb2</termIdentifier>
         <caption>
+          <langstring language="de">Kinesiologe</langstring>
           <langstring language="fr">Kinésiologue</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>35vxssxqqq</termIdentifier>
         <caption>
           <langstring language="de">Persönliche Entwicklung</langstring>
@@ -1669,16 +1701,24 @@
       <termIdentifier>xhowidw6kd</termIdentifier>
       <caption>
         <langstring language="de">Gemeindeverwaltung</langstring>
         <langstring language="fr">Administration communale</langstring>
       </caption>
     </term>
     <term>
+      <termIdentifier>myi2y7swrk</termIdentifier>
+      <caption>
+        <langstring language="de">Provinzverwaltung</langstring>
+        <langstring language="fr">Administration provinciale</langstring>
+      </caption>
+    </term>
+    <term>
       <termIdentifier>qs5vbftgho</termIdentifier>
       <caption>
+        <langstring language="de">ÖSHZ</langstring>
         <langstring language="fr">CPAS</langstring>
       </caption>
     </term>
     <term>
       <termIdentifier>mng17jgr5o</termIdentifier>
       <caption>
         <langstring language="de">Energie</langstring>
@@ -1753,20 +1793,29 @@
           <langstring language="de">Gemeinderat</langstring>
           <langstring language="fr">Conseil communal</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>fe722h2phb</termIdentifier>
         <caption>
+          <langstring language="de">Sozialhilferat</langstring>
           <langstring language="fr">Conseil de l'action sociale</langstring>
         </caption>
       </term>
       <term>
+        <termIdentifier>6xo6fraolh</termIdentifier>
+        <caption>
+          <langstring language="de">Provinzkollegium</langstring>
+          <langstring language="fr">Collège provincial</langstring>
+        </caption>
+      </term>
+      <term>
         <termIdentifier>28uj2npn2e</termIdentifier>
         <caption>
+          <langstring language="de">Provinzialrat</langstring>
           <langstring language="fr">Conseil provincial</langstring>
         </caption>
       </term>
       <term>
         <termIdentifier>0vkwvnabuu</termIdentifier>
         <caption>
           <langstring language="de">Kommissionen und beratende oder partizipative Räte</langstring>
@@ -2582,14 +2631,21 @@
     <term>
       <termIdentifier>f032co7ls6</termIdentifier>
       <caption>
         <langstring language="de">Schießsport</langstring>
         <langstring language="fr">Sports de tir</langstring>
       </caption>
       <term>
+        <termIdentifier>rvaoefu6v9</termIdentifier>
+        <caption>
+          <langstring language="de">Airsoft</langstring>
+          <langstring language="fr">Airsoft</langstring>
+        </caption>
+      </term>
+      <term>
         <termIdentifier>9tei8u2m2o</termIdentifier>
         <caption>
           <langstring language="de">Bogenschießen</langstring>
           <langstring language="fr">Tir à l'arc</langstring>
         </caption>
       </term>
       <term>
```

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/types/imio.directory.Contact.xml` & `imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/types/imio.directory.Contact.xml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/profiles/default/types/imio.directory.Entity.xml` & `imio.directory.core-1.1.9/src/imio/directory/core/profiles/default/types/imio.directory.Entity.xml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/profiles.zcml` & `imio.directory.core-1.1.9/src/imio/directory/core/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/setuphandlers.py` & `imio.directory.core-1.1.9/src/imio/directory/core/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/subscribers.py` & `imio.directory.core-1.1.9/src/imio/directory/core/subscribers.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/subscribers.zcml` & `imio.directory.core-1.1.9/src/imio/directory/core/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/testing.py` & `imio.directory.core-1.1.9/src/imio/directory/core/testing.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/tests/resources/json_contact.json` & `imio.directory.core-1.1.9/src/imio/directory/core/tests/resources/json_contact.json`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/tests/resources/logo.png` & `imio.directory.core-1.1.9/src/imio/directory/core/tests/resources/logo.png`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/tests/robot/test_example.robot` & `imio.directory.core-1.1.9/src/imio/directory/core/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/tests/test_contact.py` & `imio.directory.core-1.1.9/src/imio/directory/core/tests/test_contact.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/tests/test_cropping.py` & `imio.directory.core-1.1.9/src/imio/directory/core/tests/test_cropping.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/tests/test_entity.py` & `imio.directory.core-1.1.9/src/imio/directory/core/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/tests/test_local_roles.py` & `imio.directory.core-1.1.9/src/imio/directory/core/tests/test_local_roles.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/tests/test_multilingual.py` & `imio.directory.core-1.1.9/src/imio/directory/core/tests/test_multilingual.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/tests/test_robot.py` & `imio.directory.core-1.1.9/src/imio/directory/core/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/tests/test_setup.py` & `imio.directory.core-1.1.9/src/imio/directory/core/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/tests/test_utils.py` & `imio.directory.core-1.1.9/src/imio/directory/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/tests/test_vocabularies.py` & `imio.directory.core-1.1.9/src/imio/directory/core/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/upgrades/configure.zcml` & `imio.directory.core-1.1.9/src/imio/directory/core/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/upgrades/profiles/1006_to_1007/catalog.xml` & `imio.directory.core-1.1.9/src/imio/directory/core/upgrades/profiles/1006_to_1007/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/upgrades/upgrades.py` & `imio.directory.core-1.1.9/src/imio/directory/core/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/utils.py` & `imio.directory.core-1.1.9/src/imio/directory/core/utils.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/vocabularies.py` & `imio.directory.core-1.1.9/src/imio/directory/core/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio/directory/core/vocabularies.zcml` & `imio.directory.core-1.1.9/src/imio/directory/core/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.1.8/src/imio.directory.core.egg-info/PKG-INFO` & `imio.directory.core-1.1.9/src/imio.directory.core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.directory.core
-Version: 1.1.8
+Version: 1.1.9
 Summary: Core product for iMio contacts Directory websites
 Home-page: https://github.com/imio/imio.directory.core
 Author: Christophe Boulanger
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.directory.core
 Project-URL: Source, https://github.com/imio/imio.directory.core
@@ -187,14 +187,30 @@
 - Laurent Lasudry, laurent.lasudry@affinitic.be
 
 
 Changelog
 =========
 
 
+1.1.9 (2023-05-26)
+------------------
+
+- Fix condition when facing `Missing.Value` to avoid traceback in serializer
+  [laulaz]
+
+- WEB-3918 : Add missing DE translations for contact_category taxonomy
+  [laulaz]
+
+- Migrate to Plone 6.0.4
+  [boulch]
+
+- Update contact_category taxonomy data to reflect production site data
+  [laulaz]
+
+
 1.1.8 (2023-03-31)
 ------------------
 
 - WEB-3909 : Add upgrade step to fix wrongly stored datagrid fields values
   [laulaz]
```

### Comparing `imio.directory.core-1.1.8/src/imio.directory.core.egg-info/SOURCES.txt` & `imio.directory.core-1.1.9/src/imio.directory.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

