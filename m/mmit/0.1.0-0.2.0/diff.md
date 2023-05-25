# Comparing `tmp/mmit-0.1.0.tar.gz` & `tmp/mmit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmit-0.1.0.tar", last modified: Wed May 24 21:08:00 2023, max compression
+gzip compressed data, was "mmit-0.2.0.tar", last modified: Thu May 25 23:01:37 2023, max compression
```

## Comparing `mmit-0.1.0.tar` & `mmit-0.2.0.tar`

### file list

```diff
@@ -1,107 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.801251 mmit-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.785251 mmit-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-24 21:07:45.000000 mmit-0.1.0/.github/issue_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-24 21:07:45.000000 mmit-0.1.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.785251 mmit-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-24 21:07:45.000000 mmit-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-24 21:07:45.000000 mmit-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-24 21:07:45.000000 mmit-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-24 21:07:45.000000 mmit-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-24 21:08:00.801251 mmit-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-24 21:07:45.000000 mmit-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.785251 mmit-0.1.0/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:07:45.000000 mmit-0.1.0/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:07:45.000000 mmit-0.1.0/docker/requirement.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.781251 mmit-0.1.0/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/_static/css/baseline.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/docs/source/_static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/_static/logo/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/_static/logo/logo_title.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/api/create_decoder.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/api/create_encoder.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/api/create_model.md
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/docs/source/guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/guide/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/guide/install.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/guide/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.785251 mmit-0.1.0/docs/source/modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/docs/source/modules/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/modules/decoders/fpn.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/modules/decoders/unet++.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/modules/decoders/unet.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/docs/source/modules/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/modules/encoders/timm.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/mmit/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.793251 mmit-0.1.0/mmit/base/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/base/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/base/extra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/base/mismatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/base/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/base/upsamplers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.793251 mmit-0.1.0/mmit/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/basedecoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.793251 mmit-0.1.0/mmit/decoders/fpn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/fpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/fpn/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/fpn/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.793251 mmit-0.1.0/mmit/decoders/unet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/unet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/unet/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.793251 mmit-0.1.0/mmit/decoders/unetplusplus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/unetplusplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/unetplusplus/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.797251 mmit-0.1.0/mmit/decoders/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/utils/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/utils/resizing_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.797251 mmit-0.1.0/mmit/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/encoders/basencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.797251 mmit-0.1.0/mmit/encoders/timm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/encoders/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/encoders/timm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.797251 mmit-0.1.0/mmit/factory/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/factory/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/factory/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/factory/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.797251 mmit-0.1.0/mmit/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/heads/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/heads/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.797251 mmit-0.1.0/mmit/models/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.793251 mmit-0.1.0/mmit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-24 21:08:00.000000 mmit-0.1.0/mmit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-24 21:08:00.000000 mmit-0.1.0/mmit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 21:08:00.000000 mmit-0.1.0/mmit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-24 21:08:00.000000 mmit-0.1.0/mmit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 21:08:00.000000 mmit-0.1.0/mmit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-24 21:07:45.000000 mmit-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 21:08:00.801251 mmit-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.801251 mmit-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.801251 mmit-0.1.0/tests/demo_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/demo_blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/demo_blocks/classic_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/demo_blocks/classic_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/demo_blocks/cursed_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/test_base_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/test_decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/test_end2end.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.948250 mmit-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-25 23:01:24.000000 mmit-0.2.0/.github/issue_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-25 23:01:24.000000 mmit-0.2.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.948250 mmit-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-25 23:01:24.000000 mmit-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-25 23:01:24.000000 mmit-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-25 23:01:24.000000 mmit-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-25 23:01:24.000000 mmit-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-25 23:01:37.956250 mmit-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-25 23:01:24.000000 mmit-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.948250 mmit-0.2.0/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/docker/requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.948250 mmit-0.2.0/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/_static/css/baseline.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/docs/source/_static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/_static/logo/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/_static/logo/logo_title.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/api/create_decoder.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/api/create_encoder.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/api/create_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/docs/source/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/guide/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/guide/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/guide/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.948250 mmit-0.2.0/docs/source/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/docs/source/modules/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/modules/decoders/deeplabv3+.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/modules/decoders/deeplabv3.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/modules/decoders/fpn.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/modules/decoders/unet++.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/modules/decoders/unet.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/docs/source/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/modules/encoders/timm.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/mmit/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/mmit/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/base/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/base/extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/base/mismatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/base/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/base/upsamplers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/mmit/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/basedecoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/mmit/decoders/deeplabv3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/deeplabv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/deeplabv3/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/deeplabv3/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/deeplabv3/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/decoders/deeplabv3plus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/deeplabv3plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/deeplabv3plus/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/deeplabv3plus/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/deeplabv3plus/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/decoders/fpn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/fpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/fpn/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/fpn/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/decoders/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/unet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/unet/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/decoders/unetplusplus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/unetplusplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/unetplusplus/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/decoders/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/utils/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/utils/resizing_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/encoders/basencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/encoders/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/encoders/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/encoders/timm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/factory/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/factory/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/factory/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/heads/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/heads/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/mmit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-25 23:01:37.000000 mmit-0.2.0/mmit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-25 23:01:37.000000 mmit-0.2.0/mmit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 23:01:37.000000 mmit-0.2.0/mmit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-25 23:01:37.000000 mmit-0.2.0/mmit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 23:01:37.000000 mmit-0.2.0/mmit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-25 23:01:24.000000 mmit-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 23:01:37.956250 mmit-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/tests/demo_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/demo_blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/demo_blocks/classic_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/demo_blocks/classic_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/demo_blocks/cursed_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/test_base_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/test_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/test_end2end.py
```

### Comparing `mmit-0.1.0/.github/issue_template.md` & `mmit-0.2.0/.github/issue_template.md`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/.github/pull_request_template.md` & `mmit-0.2.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/.github/workflows/python-publish.yml` & `mmit-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/.gitignore` & `mmit-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/LICENSE` & `mmit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/PKG-INFO` & `mmit-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmit
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python package for computer vision experiments and research.
 Author-email: Andrea Boscolo Camiletto <abcamiletto@gmail.com>
 Project-URL: Homepage, https://github.com/abcamiletto/mmit
 Project-URL: Repository, https://github.com/abcamiletto/mmit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -13,15 +13,15 @@
 
 ![LogoTitle](docs/source/_static/logo/logo_title.png)
 
 <!--Introduction-->
 
 <div align="center">
 
- **mmit** is a python library with pretrained building blocks for Computer Vision experiments.
+ **mmit** is a python library to build any encoder matched with any decoder for any Computer Vision model.
 
 [![License badge](https://img.shields.io/github/license/abcamiletto/mmit?style=for-the-badge)](https://github.com/abcamiletto/mmit/blob/master/LICENSE)
 ![PyTorch - Version](https://img.shields.io/badge/PYTORCH-1.10+-red?style=for-the-badge&logo=pytorch)
 ![Python - Version](https://img.shields.io/badge/PYTHON-3.8+-red?style=for-the-badge&logo=python&logoColor=white)
 
 </div>
 <!--End Introduction-->
@@ -80,18 +80,20 @@
 In the future, we plan to add support for:
 
 - [x] timm encoders
 - [ ] some of timm transformers encoders with feature extraction
 - [ ] torchvision / torchub models
 - [ ] more decoders
 - [ ] lightning script to train models
-- [ ] multiple heads
+- [x] multiple heads
 - [ ] popular loss function
 - [ ] popular datasets
 - [ ] popular metrics
 
 ## [Awesome Sources](#awesome-sources) <!-- omit in toc -->
 
+This project is inspired by, and would not be possible without, the following amazing libraries
+
 - [PyTorch](https://pytorch.org/)
 - [PyTorch Lightning](https://www.pytorchlightning.ai/)
 - [Timm](https://github.com/huggingface/pytorch-image-models)
 - [SMP](https://github.com/qubvel/segmentation_models.pytorch)
```

### Comparing `mmit-0.1.0/README.md` & `mmit-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ![LogoTitle](docs/source/_static/logo/logo_title.png)
 
 <!--Introduction-->
 
 <div align="center">
 
- **mmit** is a python library with pretrained building blocks for Computer Vision experiments.
+ **mmit** is a python library to build any encoder matched with any decoder for any Computer Vision model.
 
 [![License badge](https://img.shields.io/github/license/abcamiletto/mmit?style=for-the-badge)](https://github.com/abcamiletto/mmit/blob/master/LICENSE)
 ![PyTorch - Version](https://img.shields.io/badge/PYTORCH-1.10+-red?style=for-the-badge&logo=pytorch)
 ![Python - Version](https://img.shields.io/badge/PYTHON-3.8+-red?style=for-the-badge&logo=python&logoColor=white)
 
 </div>
 <!--End Introduction-->
@@ -67,18 +67,20 @@
 In the future, we plan to add support for:
 
 - [x] timm encoders
 - [ ] some of timm transformers encoders with feature extraction
 - [ ] torchvision / torchub models
 - [ ] more decoders
 - [ ] lightning script to train models
-- [ ] multiple heads
+- [x] multiple heads
 - [ ] popular loss function
 - [ ] popular datasets
 - [ ] popular metrics
 
 ## [Awesome Sources](#awesome-sources) <!-- omit in toc -->
 
+This project is inspired by, and would not be possible without, the following amazing libraries
+
 - [PyTorch](https://pytorch.org/)
 - [PyTorch Lightning](https://www.pytorchlightning.ai/)
 - [Timm](https://github.com/huggingface/pytorch-image-models)
 - [SMP](https://github.com/qubvel/segmentation_models.pytorch)
```

### Comparing `mmit-0.1.0/docs/Makefile` & `mmit-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/docs/make.bat` & `mmit-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/docs/source/_static/css/baseline.css` & `mmit-0.2.0/docs/source/_static/css/baseline.css`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/docs/source/_static/logo/logo.png` & `mmit-0.2.0/docs/source/_static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/docs/source/_static/logo/logo_title.png` & `mmit-0.2.0/docs/source/_static/logo/logo_title.png`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/docs/source/conf.py` & `mmit-0.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/docs/source/guide/examples.md` & `mmit-0.2.0/docs/source/guide/examples.md`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/docs/source/index.md` & `mmit-0.2.0/docs/source/index.md`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 ```{toctree}
 :caption: 'Decoders'
 :maxdepth: 1
 
 modules/decoders/unet
 modules/decoders/unet++
 modules/decoders/fpn
+modules/decoders/deeplabv3
+modules/decoders/deeplabv3+
 ```
 
 ```{toctree}
 :caption: 'Encoders'
 :maxdepth: 1
 
 modules/encoders/timm
```

### Comparing `mmit-0.1.0/mmit/base/activations.py` & `mmit-0.2.0/mmit/base/activations.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/mmit/base/extra.py` & `mmit-0.2.0/mmit/base/extra.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/mmit/base/mismatch.py` & `mmit-0.2.0/mmit/base/mismatch.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/mmit/base/norms.py` & `mmit-0.2.0/mmit/base/norms.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/mmit/base/upsamplers.py` & `mmit-0.2.0/mmit/base/upsamplers.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/mmit/decoders/basedecoder.py` & `mmit-0.2.0/mmit/decoders/basedecoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/mmit/decoders/fpn/model.py` & `mmit-0.2.0/mmit/decoders/fpn/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from mmit.base import mismatch as mm
 from mmit.base import upsamplers as up
 from mmit.factory import register
 
 from ..basedecoder import BaseDecoder
 from ..utils import size_control
-from .parts import ConvNormReLU, SkipBlock
+from .parts import ConvNormActivation, SkipBlock
 
 __all__ = ["FPN"]
 
 DEFAULT_CHANNEL = 256
 
 
 @register
@@ -63,15 +63,15 @@
 
         # Setting up the output blocks
         specs = norm_layer, activation_layer, extra_layer
 
         out_blocks = []
         for red in input_reductions[1:][::-1]:
             up_lay = partial(upsample_layer, scale=red)
-            block = ConvNormReLU(decoder_channel, decoder_channel, up_lay, *specs)
+            block = ConvNormActivation(decoder_channel, decoder_channel, up_lay, *specs)
             out_blocks.append(block)
 
         self.out_blocks = nn.ModuleList(out_blocks)
         self._out_classes = decoder_channel * len(out_blocks)
 
         # Input block for the first layer
         self.input_block = nn.Conv2d(input_channels[0], decoder_channel, 1)
```

### Comparing `mmit-0.1.0/mmit/decoders/fpn/parts.py` & `mmit-0.2.0/mmit/decoders/fpn/parts.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch.nn as nn
 from torch import Tensor
 
 from mmit.base import mismatch as mm
 from mmit.base import upsamplers as up
 
 
-class ConvNormReLU(nn.Module):
+class ConvNormActivation(nn.Module):
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         upsample_layer: Type[nn.Module] = up.ConvTranspose2d,
         norm_layer: Type[nn.Module] = nn.BatchNorm2d,
         activation: Type[nn.Module] = nn.ReLU,
```

### Comparing `mmit-0.1.0/mmit/decoders/unet/model.py` & `mmit-0.2.0/mmit/decoders/unet/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/mmit/decoders/unet/parts.py` & `mmit-0.2.0/mmit/decoders/unet/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/mmit/decoders/unetplusplus/model.py` & `mmit-0.2.0/mmit/decoders/unetplusplus/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
         # The final output is the output of the last block
         final_output = features[f"0_{self.depth-1}"]
 
         return final_output
 
     @property
-    def out_classes(self):
+    def out_classes(self) -> int:
         return self._out_classes
 
     def _preprocess_features(self, features):
         """Preprocess features by removing the first feature and reversing the order."""
         features = {f"{i}_0": f for i, f in enumerate(features)}
         return features
```

### Comparing `mmit-0.1.0/mmit/decoders/utils/resize.py` & `mmit-0.2.0/mmit/decoders/utils/resize.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/mmit/encoders/timm/model.py` & `mmit-0.2.0/mmit/encoders/timm/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/mmit/factory/components.py` & `mmit-0.2.0/mmit/factory/components.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/mmit/factory/factory.py` & `mmit-0.2.0/mmit/factory/factory.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/mmit/factory/registry.py` & `mmit-0.2.0/mmit/factory/registry.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/mmit/heads/classification.py` & `mmit-0.2.0/mmit/heads/classification.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/mmit/heads/segmentation.py` & `mmit-0.2.0/mmit/heads/segmentation.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/mmit.egg-info/PKG-INFO` & `mmit-0.2.0/mmit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmit
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python package for computer vision experiments and research.
 Author-email: Andrea Boscolo Camiletto <abcamiletto@gmail.com>
 Project-URL: Homepage, https://github.com/abcamiletto/mmit
 Project-URL: Repository, https://github.com/abcamiletto/mmit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -13,15 +13,15 @@
 
 ![LogoTitle](docs/source/_static/logo/logo_title.png)
 
 <!--Introduction-->
 
 <div align="center">
 
- **mmit** is a python library with pretrained building blocks for Computer Vision experiments.
+ **mmit** is a python library to build any encoder matched with any decoder for any Computer Vision model.
 
 [![License badge](https://img.shields.io/github/license/abcamiletto/mmit?style=for-the-badge)](https://github.com/abcamiletto/mmit/blob/master/LICENSE)
 ![PyTorch - Version](https://img.shields.io/badge/PYTORCH-1.10+-red?style=for-the-badge&logo=pytorch)
 ![Python - Version](https://img.shields.io/badge/PYTHON-3.8+-red?style=for-the-badge&logo=python&logoColor=white)
 
 </div>
 <!--End Introduction-->
@@ -80,18 +80,20 @@
 In the future, we plan to add support for:
 
 - [x] timm encoders
 - [ ] some of timm transformers encoders with feature extraction
 - [ ] torchvision / torchub models
 - [ ] more decoders
 - [ ] lightning script to train models
-- [ ] multiple heads
+- [x] multiple heads
 - [ ] popular loss function
 - [ ] popular datasets
 - [ ] popular metrics
 
 ## [Awesome Sources](#awesome-sources) <!-- omit in toc -->
 
+This project is inspired by, and would not be possible without, the following amazing libraries
+
 - [PyTorch](https://pytorch.org/)
 - [PyTorch Lightning](https://www.pytorchlightning.ai/)
 - [Timm](https://github.com/huggingface/pytorch-image-models)
 - [SMP](https://github.com/qubvel/segmentation_models.pytorch)
```

### Comparing `mmit-0.1.0/mmit.egg-info/SOURCES.txt` & `mmit-0.2.0/mmit.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 .github/pull_request_template.md
 .github/workflows/python-publish.yml
 docker/Dockerfile
 docker/requirement.txt
 docs/.readthedocs.yaml
 docs/Makefile
 docs/make.bat
-docs/requirements.txt
 docs/source/conf.py
 docs/source/index.md
 docs/source/_static/css/baseline.css
 docs/source/_static/logo/logo.png
 docs/source/_static/logo/logo_title.png
 docs/source/api/create_decoder.md
 docs/source/api/create_encoder.md
 docs/source/api/create_model.md
 docs/source/guide/examples.md
 docs/source/guide/install.md
 docs/source/guide/quickstart.md
+docs/source/modules/decoders/deeplabv3+.md
+docs/source/modules/decoders/deeplabv3.md
 docs/source/modules/decoders/fpn.md
 docs/source/modules/decoders/unet++.md
 docs/source/modules/decoders/unet.md
 docs/source/modules/encoders/timm.md
 mmit/__init__.py
 mmit.egg-info/PKG-INFO
 mmit.egg-info/SOURCES.txt
@@ -37,14 +38,22 @@
 mmit/base/activations.py
 mmit/base/extra.py
 mmit/base/mismatch.py
 mmit/base/norms.py
 mmit/base/upsamplers.py
 mmit/decoders/__init__.py
 mmit/decoders/basedecoder.py
+mmit/decoders/deeplabv3/__init__.py
+mmit/decoders/deeplabv3/aspp.py
+mmit/decoders/deeplabv3/model.py
+mmit/decoders/deeplabv3/parts.py
+mmit/decoders/deeplabv3plus/__init__.py
+mmit/decoders/deeplabv3plus/aspp.py
+mmit/decoders/deeplabv3plus/model.py
+mmit/decoders/deeplabv3plus/parts.py
 mmit/decoders/fpn/__init__.py
 mmit/decoders/fpn/model.py
 mmit/decoders/fpn/parts.py
 mmit/decoders/unet/__init__.py
 mmit/decoders/unet/model.py
 mmit/decoders/unet/parts.py
 mmit/decoders/unetplusplus/__init__.py
```

### Comparing `mmit-0.1.0/pyproject.toml` & `mmit-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,28 @@
 readme = "README.md"
 authors = [{ name = "Andrea Boscolo Camiletto", email = "abcamiletto@gmail.com" }]
 dependencies = [
     "timm>=0.9.0",
     "torch>=1.10"
 ]
 requires-python = ">=3.8"
-version = "0.1.0"
+version = "0.2.0"
 
 [project.urls]
 Homepage = "https://github.com/abcamiletto/mmit"
 Repository = "https://github.com/abcamiletto/mmit"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pytest", "pytest-cov", "pytest-lazy-fixture", "pre-commit"]
 docs = ["sphinx==6.2.1",
+        "sphinx-rtd-theme==1.2.0",
+        "sphinx-copybutton==0.5.2",
+        "sphinx-autodoc-typehints==1.23.0",
+        "myst-parser==1.0.0",
         "sphinx-autobuild",
-        "sphinx-rtd-theme",
-        "sphinxcontrib.spelling",
-        "sphinx-autodoc-typehints",
-        "sphinx_copybutton",
-        "sphinx-autoapi",
-        "myst-parser"
 ]
 
 [tool.setuptools.packages.find]
 namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
 
 [tool.ruff]
 line-length = 120
```

### Comparing `mmit-0.1.0/tests/demo_blocks/classic_decoder.py` & `mmit-0.2.0/tests/demo_blocks/classic_decoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/tests/demo_blocks/classic_encoder.py` & `mmit-0.2.0/tests/demo_blocks/classic_encoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/tests/demo_blocks/cursed_encoder.py` & `mmit-0.2.0/tests/demo_blocks/cursed_encoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/tests/test_base_components.py` & `mmit-0.2.0/tests/test_base_components.py`

 * *Files identical despite different names*

### Comparing `mmit-0.1.0/tests/test_decoders.py` & `mmit-0.2.0/tests/test_decoders.py`

 * *Files identical despite different names*

