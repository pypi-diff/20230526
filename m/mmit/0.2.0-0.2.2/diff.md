# Comparing `tmp/mmit-0.2.0.tar.gz` & `tmp/mmit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmit-0.2.0.tar", last modified: Thu May 25 23:01:37 2023, max compression
+gzip compressed data, was "mmit-0.2.2.tar", last modified: Fri May 26 19:04:50 2023, max compression
```

## Comparing `mmit-0.2.0.tar` & `mmit-0.2.2.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.948250 mmit-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-25 23:01:24.000000 mmit-0.2.0/.github/issue_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-25 23:01:24.000000 mmit-0.2.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.948250 mmit-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-25 23:01:24.000000 mmit-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-25 23:01:24.000000 mmit-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-25 23:01:24.000000 mmit-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-25 23:01:24.000000 mmit-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-25 23:01:37.956250 mmit-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-25 23:01:24.000000 mmit-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.948250 mmit-0.2.0/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/docker/requirement.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.948250 mmit-0.2.0/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/_static/css/baseline.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/docs/source/_static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/_static/logo/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/_static/logo/logo_title.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/api/create_decoder.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/api/create_encoder.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/api/create_model.md
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/docs/source/guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/guide/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/guide/install.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/guide/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.948250 mmit-0.2.0/docs/source/modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/docs/source/modules/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/modules/decoders/deeplabv3+.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/modules/decoders/deeplabv3.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/modules/decoders/fpn.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/modules/decoders/unet++.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/modules/decoders/unet.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/docs/source/modules/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 23:01:24.000000 mmit-0.2.0/docs/source/modules/encoders/timm.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/mmit/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/mmit/base/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/base/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/base/extra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/base/mismatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/base/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/base/upsamplers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/mmit/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/basedecoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/mmit/decoders/deeplabv3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/deeplabv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/deeplabv3/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/deeplabv3/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/deeplabv3/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/decoders/deeplabv3plus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/deeplabv3plus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/deeplabv3plus/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/deeplabv3plus/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/deeplabv3plus/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/decoders/fpn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/fpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/fpn/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/fpn/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/decoders/unet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/unet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/unet/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/decoders/unetplusplus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/unetplusplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/unetplusplus/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/decoders/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/utils/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/decoders/utils/resizing_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/encoders/basencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/encoders/timm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/encoders/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/encoders/timm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/factory/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/factory/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/factory/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/factory/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/heads/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/heads/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/mmit/models/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-25 23:01:24.000000 mmit-0.2.0/mmit/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.952250 mmit-0.2.0/mmit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-25 23:01:37.000000 mmit-0.2.0/mmit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-25 23:01:37.000000 mmit-0.2.0/mmit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 23:01:37.000000 mmit-0.2.0/mmit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-25 23:01:37.000000 mmit-0.2.0/mmit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 23:01:37.000000 mmit-0.2.0/mmit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-25 23:01:24.000000 mmit-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 23:01:37.956250 mmit-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:37.956250 mmit-0.2.0/tests/demo_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/demo_blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/demo_blocks/classic_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/demo_blocks/classic_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/demo_blocks/cursed_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/test_base_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/test_decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-25 23:01:24.000000 mmit-0.2.0/tests/test_end2end.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.455819 mmit-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-26 19:04:38.000000 mmit-0.2.2/.github/issue_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-26 19:04:38.000000 mmit-0.2.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-26 19:04:38.000000 mmit-0.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-26 19:04:38.000000 mmit-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-26 19:04:38.000000 mmit-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-26 19:04:38.000000 mmit-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-26 19:04:50.455819 mmit-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-26 19:04:38.000000 mmit-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/docker/requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.443819 mmit-0.2.2/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/_static/css/baseline.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docs/source/_static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/_static/logo/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/_static/logo/logo_title.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/api/create_decoder.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/api/create_encoder.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/api/create_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docs/source/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/guide/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/guide/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/guide/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.443819 mmit-0.2.2/docs/source/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docs/source/modules/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/modules/decoders/deeplabv3+.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/modules/decoders/deeplabv3.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/modules/decoders/fpn.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/modules/decoders/unet++.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/modules/decoders/unet.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docs/source/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/modules/encoders/timm.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/mmit/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/base/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/base/extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/base/mismatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/base/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/base/upsamplers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/basedecoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/decoders/deeplabv3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/deeplabv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/deeplabv3/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/deeplabv3/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/deeplabv3/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/decoders/deeplabv3plus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/deeplabv3plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/deeplabv3plus/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/deeplabv3plus/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/deeplabv3plus/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/decoders/fpn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/fpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/fpn/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/fpn/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/decoders/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/unet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/unet/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/decoders/unetplusplus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/unetplusplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/unetplusplus/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/decoders/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/utils/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/utils/resizing_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/encoders/basencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.455819 mmit-0.2.2/mmit/encoders/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/encoders/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/encoders/timm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.455819 mmit-0.2.2/mmit/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/factory/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/factory/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/factory/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.455819 mmit-0.2.2/mmit/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/heads/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/heads/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.455819 mmit-0.2.2/mmit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-26 19:04:50.000000 mmit-0.2.2/mmit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-26 19:04:50.000000 mmit-0.2.2/mmit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:04:50.000000 mmit-0.2.2/mmit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-26 19:04:50.000000 mmit-0.2.2/mmit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 19:04:50.000000 mmit-0.2.2/mmit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-26 19:04:38.000000 mmit-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 19:04:50.455819 mmit-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.455819 mmit-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.455819 mmit-0.2.2/tests/demo_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/demo_blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/demo_blocks/classic_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/demo_blocks/classic_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/demo_blocks/cursed_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/test_base_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/test_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/test_end2end.py
```

### Comparing `mmit-0.2.0/.github/issue_template.md` & `mmit-0.2.2/.github/issue_template.md`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/.github/pull_request_template.md` & `mmit-0.2.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/.github/workflows/python-publish.yml` & `mmit-0.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/.gitignore` & `mmit-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/LICENSE` & `mmit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/PKG-INFO` & `mmit-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmit
-Version: 0.2.0
+Version: 0.2.2
 Summary: A Python package for computer vision experiments and research.
 Author-email: Andrea Boscolo Camiletto <abcamiletto@gmail.com>
 Project-URL: Homepage, https://github.com/abcamiletto/mmit
 Project-URL: Repository, https://github.com/abcamiletto/mmit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mmit-0.2.0/README.md` & `mmit-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/docs/.readthedocs.yaml` & `mmit-0.2.2/docs/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/docs/Makefile` & `mmit-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/docs/make.bat` & `mmit-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/docs/source/_static/css/baseline.css` & `mmit-0.2.2/docs/source/_static/css/baseline.css`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/docs/source/_static/logo/logo.png` & `mmit-0.2.2/docs/source/_static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/docs/source/_static/logo/logo_title.png` & `mmit-0.2.2/docs/source/_static/logo/logo_title.png`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/docs/source/conf.py` & `mmit-0.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/docs/source/guide/examples.md` & `mmit-0.2.2/docs/source/guide/examples.md`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/docs/source/index.md` & `mmit-0.2.2/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/base/activations.py` & `mmit-0.2.2/mmit/base/activations.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/base/extra.py` & `mmit-0.2.2/mmit/base/extra.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/base/mismatch.py` & `mmit-0.2.2/mmit/base/mismatch.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/base/norms.py` & `mmit-0.2.2/mmit/base/norms.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/base/upsamplers.py` & `mmit-0.2.2/mmit/base/upsamplers.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/decoders/basedecoder.py` & `mmit-0.2.2/mmit/decoders/basedecoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/decoders/deeplabv3/aspp.py` & `mmit-0.2.2/mmit/decoders/deeplabv3/aspp.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/decoders/deeplabv3/model.py` & `mmit-0.2.2/mmit/decoders/deeplabv3/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/decoders/deeplabv3/parts.py` & `mmit-0.2.2/mmit/decoders/deeplabv3/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/decoders/deeplabv3plus/model.py` & `mmit-0.2.2/mmit/decoders/deeplabv3plus/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,18 +20,16 @@
 DEFAULT_ATROUS_RATES = [12, 24, 36]
 
 
 @register
 class DeepLabV3Plus(BaseDecoder):
     """
     Implementation of the DeepLabV3+ decoder. Paper: https://arxiv.org/abs/1802.02611
-    To make it compatible with any encoder, we take the following decisions:
-
-        - If the input has only one feature map, we only do one upsampling (of course).
-        - Otherwise, we do two. The first one with the "middle" feature, and the last with the last.
+    To make it compatible with any encoder, the first skip connection is with
+    the "middle" feature and the second one with the last.
 
     Args:
         input_channels: The channels of the input features.
         input_reductions: The reduction factor of the input features.
         decoder_channel: The channel to use on the decoder.
         atrous_rates: The atrous rates to use on the ASPP module.
         norm_layer: Normalization layer to use.
@@ -66,17 +64,14 @@
         up_layer = uplays[-1]
 
         aspp = ASPP(skip_ch, init_ch, atrous_rates)
         conv = DWSConvNormActivation(init_ch, init_ch, 3, *specs)
         up = up_layer(init_ch)
         self.aspp_block = nn.Sequential(aspp, conv, up)
 
-        if len(skip_chans) == 1:
-            return
-
         final_ch = decoder_channels[-1]
         skip_ch = skip_chans[-2]
         up_layer = uplays[-2]
 
         # Setting up the skip connection
         self.skip_block = ConvNormActivation(skip_ch, skip_ch, 1, *specs)
         self.fix_mismatch = mismatch_layer()
@@ -87,34 +82,28 @@
         self.final_block = nn.Sequential(conv, up)
 
     @size_control
     def forward(self, *features: torch.Tensor) -> torch.Tensor:
         x = features[self.skip_idxes[-1]]
         x = self.aspp_block(x)
 
-        if len(features) == 2:
-            return x
-
         skip = features[self.skip_idxes[0]]
-
         skip = self.skip_block(skip)
         x, skip = self.fix_mismatch(x, skip)
         x = torch.cat([x, skip], dim=1)
 
         x = self.final_block(x)
         return x
 
     @property
     def out_classes(self) -> int:
         return self._out_classes
 
     def _get_skip_indexes(self, input_reductions: List[int]) -> List[int]:
         n_layers = len(input_reductions)
-        if n_layers == 2:
-            return [1]
         return [n_layers // 2, n_layers - 1]
 
     def _get_skip_reductions(self, input_reductions: List[int]) -> List[int]:
         return [input_reductions[idx] for idx in self.skip_idxes]
 
     def _get_skip_channels(self, input_channels: List[int]) -> List[int]:
         return [input_channels[idx] for idx in self.skip_idxes]
```

### Comparing `mmit-0.2.0/mmit/decoders/deeplabv3plus/parts.py` & `mmit-0.2.2/mmit/decoders/deeplabv3plus/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/decoders/fpn/model.py` & `mmit-0.2.2/mmit/decoders/fpn/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/decoders/fpn/parts.py` & `mmit-0.2.2/mmit/decoders/fpn/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/decoders/unet/model.py` & `mmit-0.2.2/mmit/decoders/unet/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/decoders/unet/parts.py` & `mmit-0.2.2/mmit/decoders/unet/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/decoders/unetplusplus/model.py` & `mmit-0.2.2/mmit/decoders/unetplusplus/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/decoders/utils/resize.py` & `mmit-0.2.2/mmit/decoders/utils/resize.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/encoders/basencoder.py` & `mmit-0.2.2/mmit/encoders/basencoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/encoders/timm/model.py` & `mmit-0.2.2/mmit/encoders/timm/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/factory/components.py` & `mmit-0.2.2/mmit/factory/components.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/mmit/factory/factory.py` & `mmit-0.2.2/mmit/factory/factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import List, Optional
 
 import torch.nn as nn
 
-from ..heads import heads_builder
 from ..models import MmitModel
 from .components import build_components
-from .registry import get_decoder, get_encoder
+from .registry import get_decoder, get_encoder, get_head
 
 __all__ = ["create_encoder", "create_decoder", "create_model"]
 
 
 class Factory:
-    out_channels: List[int]
-    out_reductions: List[int]
+    encoder_channels: List[int]
+    encoder_reductions: List[int]
+    decoder_channels: int
 
     @classmethod
     def create_encoder(
         cls,
         name: str,
         in_chans: int = 3,
         out_indices: Optional[tuple] = None,
@@ -40,16 +40,16 @@
             kwargs["output_stride"] = output_stride
         if out_indices is not None:
             kwargs["out_indices"] = out_indices
 
         encoder = Encoder(
             **kwargs,
         )
-        cls.out_channels = encoder.out_channels
-        cls.out_reductions = encoder.out_reductions
+        cls.encoder_channels = encoder.out_channels
+        cls.encoder_reductions = encoder.out_reductions
         return encoder
 
     @classmethod
     def create_decoder(
         cls,
         name: str,
         out_channels: Optional[int] = None,
@@ -65,44 +65,72 @@
             out_reductions: The reduction factor of the input tensors of the forward pass.
             kwargs: Keyword arguments for the decoder. Take a look at the specific decoder docs for more info!
         """
         Decoder = get_decoder(name)
         components = build_components(kwargs)
 
         kwargs.update(components)
-        out_channels = out_channels or cls.out_channels
-        out_reductions = out_reductions or cls.out_reductions
-        return Decoder(out_channels, out_reductions, **kwargs)
+        out_channels = out_channels or cls.encoder_channels
+        out_reductions = out_reductions or cls.encoder_reductions
 
+        decoder = Decoder(out_channels, out_reductions, **kwargs)
+        cls.decoder_channels = decoder.out_classes
+        return decoder
 
-create_encoder = Factory.create_encoder
-create_decoder = Factory.create_decoder
+    @classmethod
+    def create_head(
+        cls,
+        task: str,
+        classes: int,
+        in_channels: Optional[int] = None,
+        **kwargs,
+    ) -> nn.Module:
+        """
+        Build a head from a name and some keyword arguments.
+
+        Args:
+            name: The name of the head.
+            in_channels: The number of channels of the input tensors of the forward pass.
+            out_classes: The number of classes of the output tensors of the forward pass.
+            kwargs: Keyword arguments for the head. Take a look at the specific head docs for more info!
+        """
+        Head = get_head(task)
+        in_channels = in_channels or cls.decoder_channels
+
+        head = Head(in_channels, classes, **kwargs)
+        return head
 
+    @classmethod
+    def create_model(
+        cls,
+        encoder_name: str,
+        decoder_name: str,
+        classes: int,
+        task: str = "segmentation",
+        encoder_cfg: dict = None,
+        decoder_cfg: dict = None,
+    ):
+        """
+        Build a model from an encoder and a decoder.
+
+        Args:
+            encoder_name: The name of the encoder.
+            decoder_name: The name of the decoder.
+            classes: The number of classes.
+            task: The task of the model.
+            encoder_cfg: Keyword arguments for the encoder. Check the specific encoder docs for more info.
+            decoder_cfg: Keyword arguments for the decoder. Check the specific decoder docs for more info.
+        """
 
-def create_model(
-    encoder_name: str,
-    decoder_name: str,
-    classes: int,
-    task: str = "segmentation",
-    encoder_cfg: dict = None,
-    decoder_cfg: dict = None,
-):
-    """
-    Build a model from an encoder and a decoder.
-
-    Args:
-        encoder_name: The name of the encoder.
-        decoder_name: The name of the decoder.
-        classes: The number of classes.
-        task: The task of the model.
-        encoder_cfg: Keyword arguments for the encoder. Check the specific encoder docs for more info.
-        decoder_cfg: Keyword arguments for the decoder. Check the specific decoder docs for more info.
-    """
-
-    encoder_cfg = encoder_cfg or {}
-    decoder_cfg = decoder_cfg or {}
-
-    encoder = create_encoder(encoder_name, **encoder_cfg)
-    decoder = create_decoder(decoder_name, **decoder_cfg)
-    head = heads_builder[task](decoder.out_classes, classes)
+        encoder_cfg = encoder_cfg or {}
+        decoder_cfg = decoder_cfg or {}
 
-    return MmitModel(encoder, decoder, head)
+        encoder = cls.create_encoder(encoder_name, **encoder_cfg)
+        decoder = cls.create_decoder(decoder_name, **decoder_cfg)
+        head = cls.create_head(task, classes)
+
+        return MmitModel(encoder, decoder, head)
+
+
+create_encoder = Factory.create_encoder
+create_decoder = Factory.create_decoder
+create_model = Factory.create_model
```

### Comparing `mmit-0.2.0/mmit/factory/registry.py` & `mmit-0.2.2/mmit/factory/registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "register",
 ]
 
 
 class Registry:
     _decoders: Dict[str, Type[nn.Module]] = {}
     _encoders: Dict[str, Type[nn.Module]] = {}
+    _heads: Dict[str, Type[nn.Module]] = {}
 
     @classmethod
     def _register(cls, item: Type[nn.Module], registry: Dict[str, Type[nn.Module]]):
         """Helper method to register encoders or decoders."""
         classname = item.__name__.lower()
         registry[classname] = item
 
@@ -29,22 +30,30 @@
         cls._register(decoder, cls._decoders)
 
     @classmethod
     def register_encoder(cls, encoder: Type[nn.Module]):
         cls._register(encoder, cls._encoders)
 
     @classmethod
+    def register_head(cls, head: Type[nn.Module]):
+        cls._register(head, cls._heads)
+
+    @classmethod
     def list_all_decoders(cls) -> List[str]:
         return list(cls._decoders.keys())
 
     @classmethod
     def list_all_encoders(cls) -> List[str]:
         return list(cls._encoders.keys())
 
     @classmethod
+    def list_all_heads(cls) -> List[str]:
+        return list(cls._heads.keys())
+
+    @classmethod
     def get_decoder(cls, name: str) -> Type[nn.Module]:
         if name not in cls._decoders:
             raise KeyError(f"Decoder {name} is not registered")
         return cls._decoders[name]
 
     @classmethod
     def get_encoder(cls, name: str) -> Type[nn.Module]:
@@ -54,32 +63,43 @@
             return partial(encoder, name=name)
 
         if name not in cls._encoders:
             raise KeyError(f"Encoder {name} is not registered")
 
         return cls._encoders[name]
 
+    @classmethod
+    def get_head(cls, name: str) -> Type[nn.Module]:
+        if name not in cls._heads:
+            raise KeyError(f"Head {name} is not registered")
+        return cls._heads[name]
+
 
 register_decoder = Registry.register_decoder
 list_decoders = Registry.list_all_decoders
 get_decoder = Registry.get_decoder
 register_encoder = Registry.register_encoder
 list_encoders = Registry.list_all_encoders
 get_encoder = Registry.get_encoder
+register_head = Registry.register_head
+list_heads = Registry.list_all_heads
+get_head = Registry.get_head
 
 
 def register(cls: Type[nn.Module]):
     """Decorator helper to register encoders or decoders classes in this package."""
     module_name = inspect.getmodule(cls).__name__
 
-    # Split the module name by "." and check if "encoders" or "decoders" is in the list
+    # Split the module name by "." and check if parent name is in the list
     module_parts = module_name.split(".")
     if "decoders" in module_parts:
         Registry.register_decoder(cls)
     elif "encoders" in module_parts:
         Registry.register_encoder(cls)
+    elif "heads" in module_parts:
+        Registry.register_head(cls)
     else:
         raise ValueError(
             "Invalid module for registration. Class must be in a subpackage named 'encoders' or 'decoders'."
         )
 
     return cls
```

### Comparing `mmit-0.2.0/mmit/heads/classification.py` & `mmit-0.2.2/mmit/heads/classification.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from typing import Type
 
 import torch.nn as nn
 
+from mmit.factory import register
+
 __all__ = ["ClassificationHead"]
 
 
+@register
 class ClassificationHead(nn.Module):
     def __init__(
         self,
         in_channels: int,
         num_classes: int,
         activation_layer: Type[nn.Module] = nn.ReLU,
         pooling_layer: Type[nn.Module] = nn.AdaptiveAvgPool2d,
```

### Comparing `mmit-0.2.0/mmit/heads/segmentation.py` & `mmit-0.2.2/mmit/heads/segmentation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from typing import Type
 
 import torch.nn as nn
 from torch import Tensor
 
+from mmit.factory import register
+
 __all__ = ["SegmentationHead"]
 
 
+@register
 class SegmentationHead(nn.Module):
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
-        kernel_size: int = 1,
-        activation_layer: Type[nn.Module] = nn.ReLU,
+        kernel_size: int = 3,
+        activation_layer: Type[nn.Module] = nn.Identity,
         extra_layer: Type[nn.Module] = nn.Identity,
     ):
         super().__init__()
         self.conv = nn.Conv2d(in_channels, out_channels, kernel_size)
         self.activation = activation_layer()
         self.extra = extra_layer()
```

### Comparing `mmit-0.2.0/mmit.egg-info/PKG-INFO` & `mmit-0.2.2/mmit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmit
-Version: 0.2.0
+Version: 0.2.2
 Summary: A Python package for computer vision experiments and research.
 Author-email: Andrea Boscolo Camiletto <abcamiletto@gmail.com>
 Project-URL: Homepage, https://github.com/abcamiletto/mmit
 Project-URL: Repository, https://github.com/abcamiletto/mmit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mmit-0.2.0/mmit.egg-info/SOURCES.txt` & `mmit-0.2.2/mmit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/pyproject.toml` & `mmit-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 readme = "README.md"
 authors = [{ name = "Andrea Boscolo Camiletto", email = "abcamiletto@gmail.com" }]
 dependencies = [
     "timm>=0.9.0",
     "torch>=1.10"
 ]
 requires-python = ">=3.8"
-version = "0.2.0"
+version = "0.2.2"
 
 [project.urls]
 Homepage = "https://github.com/abcamiletto/mmit"
 Repository = "https://github.com/abcamiletto/mmit"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pytest", "pytest-cov", "pytest-lazy-fixture", "pre-commit"]
```

### Comparing `mmit-0.2.0/tests/demo_blocks/classic_decoder.py` & `mmit-0.2.2/tests/demo_blocks/classic_decoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/tests/demo_blocks/classic_encoder.py` & `mmit-0.2.2/tests/demo_blocks/classic_encoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/tests/demo_blocks/cursed_encoder.py` & `mmit-0.2.2/tests/demo_blocks/cursed_encoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/tests/test_base_components.py` & `mmit-0.2.2/tests/test_base_components.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.0/tests/test_decoders.py` & `mmit-0.2.2/tests/test_decoders.py`

 * *Files identical despite different names*

