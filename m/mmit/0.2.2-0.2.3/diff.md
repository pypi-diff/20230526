# Comparing `tmp/mmit-0.2.2.tar.gz` & `tmp/mmit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmit-0.2.2.tar", last modified: Fri May 26 19:04:50 2023, max compression
+gzip compressed data, was "mmit-0.2.3.tar", last modified: Fri May 26 19:23:06 2023, max compression
```

## Comparing `mmit-0.2.2.tar` & `mmit-0.2.3.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.455819 mmit-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-26 19:04:38.000000 mmit-0.2.2/.github/issue_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-26 19:04:38.000000 mmit-0.2.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-26 19:04:38.000000 mmit-0.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-26 19:04:38.000000 mmit-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-26 19:04:38.000000 mmit-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-26 19:04:38.000000 mmit-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-26 19:04:50.455819 mmit-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-26 19:04:38.000000 mmit-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/docker/requirement.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.443819 mmit-0.2.2/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/_static/css/baseline.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docs/source/_static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/_static/logo/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/_static/logo/logo_title.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/api/create_decoder.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/api/create_encoder.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/api/create_model.md
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docs/source/guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/guide/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/guide/install.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/guide/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.443819 mmit-0.2.2/docs/source/modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docs/source/modules/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/modules/decoders/deeplabv3+.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/modules/decoders/deeplabv3.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/modules/decoders/fpn.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/modules/decoders/unet++.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/modules/decoders/unet.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/docs/source/modules/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 19:04:38.000000 mmit-0.2.2/docs/source/modules/encoders/timm.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.447819 mmit-0.2.2/mmit/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/base/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/base/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/base/extra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/base/mismatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/base/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/base/upsamplers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/basedecoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/decoders/deeplabv3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/deeplabv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/deeplabv3/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/deeplabv3/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/deeplabv3/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/decoders/deeplabv3plus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/deeplabv3plus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/deeplabv3plus/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/deeplabv3plus/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/deeplabv3plus/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/decoders/fpn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/fpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/fpn/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/fpn/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/decoders/unet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/unet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/unet/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/decoders/unetplusplus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/unetplusplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/unetplusplus/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/decoders/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/utils/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/decoders/utils/resizing_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/encoders/basencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.455819 mmit-0.2.2/mmit/encoders/timm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/encoders/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/encoders/timm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.455819 mmit-0.2.2/mmit/factory/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/factory/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/factory/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/factory/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.455819 mmit-0.2.2/mmit/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/heads/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/heads/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.455819 mmit-0.2.2/mmit/models/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-26 19:04:38.000000 mmit-0.2.2/mmit/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.451820 mmit-0.2.2/mmit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-26 19:04:50.000000 mmit-0.2.2/mmit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-26 19:04:50.000000 mmit-0.2.2/mmit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:04:50.000000 mmit-0.2.2/mmit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-26 19:04:50.000000 mmit-0.2.2/mmit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 19:04:50.000000 mmit-0.2.2/mmit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-26 19:04:38.000000 mmit-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 19:04:50.455819 mmit-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.455819 mmit-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:50.455819 mmit-0.2.2/tests/demo_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/demo_blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/demo_blocks/classic_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/demo_blocks/classic_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/demo_blocks/cursed_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/test_base_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/test_decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-26 19:04:38.000000 mmit-0.2.2/tests/test_end2end.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.063470 mmit-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.055470 mmit-0.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-26 19:22:54.000000 mmit-0.2.3/.github/issue_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-26 19:22:54.000000 mmit-0.2.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.055470 mmit-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-26 19:22:54.000000 mmit-0.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-26 19:22:54.000000 mmit-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-26 19:22:54.000000 mmit-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-26 19:22:54.000000 mmit-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-26 19:23:06.063470 mmit-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-26 19:22:54.000000 mmit-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.055470 mmit-0.2.3/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:22:54.000000 mmit-0.2.3/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:22:54.000000 mmit-0.2.3/docker/requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.055470 mmit-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.055470 mmit-0.2.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.051470 mmit-0.2.3/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.055470 mmit-0.2.3/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/_static/css/baseline.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.055470 mmit-0.2.3/docs/source/_static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/_static/logo/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/_static/logo/logo_title.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.055470 mmit-0.2.3/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/api/create_decoder.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/api/create_encoder.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/api/create_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.055470 mmit-0.2.3/docs/source/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/guide/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/guide/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/guide/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.051470 mmit-0.2.3/docs/source/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.055470 mmit-0.2.3/docs/source/modules/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/modules/decoders/deeplabv3+.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/modules/decoders/deeplabv3.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/modules/decoders/fpn.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/modules/decoders/unet++.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/modules/decoders/unet.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.055470 mmit-0.2.3/docs/source/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 19:22:54.000000 mmit-0.2.3/docs/source/modules/encoders/timm.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.059470 mmit-0.2.3/mmit/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.059470 mmit-0.2.3/mmit/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/base/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/base/extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/base/mismatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/base/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/base/upsamplers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.059470 mmit-0.2.3/mmit/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/basedecoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.059470 mmit-0.2.3/mmit/decoders/deeplabv3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/deeplabv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/deeplabv3/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/deeplabv3/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/deeplabv3/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.059470 mmit-0.2.3/mmit/decoders/deeplabv3plus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/deeplabv3plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/deeplabv3plus/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/deeplabv3plus/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/deeplabv3plus/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.059470 mmit-0.2.3/mmit/decoders/fpn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/fpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/fpn/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/fpn/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.059470 mmit-0.2.3/mmit/decoders/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/unet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/unet/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.059470 mmit-0.2.3/mmit/decoders/unetplusplus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/unetplusplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/unetplusplus/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.059470 mmit-0.2.3/mmit/decoders/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/utils/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/decoders/utils/resizing_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.059470 mmit-0.2.3/mmit/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/encoders/basencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.059470 mmit-0.2.3/mmit/encoders/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/encoders/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/encoders/timm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.063470 mmit-0.2.3/mmit/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/factory/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/factory/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/factory/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.063470 mmit-0.2.3/mmit/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/heads/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/heads/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.063470 mmit-0.2.3/mmit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-26 19:22:54.000000 mmit-0.2.3/mmit/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.059470 mmit-0.2.3/mmit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-26 19:23:06.000000 mmit-0.2.3/mmit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-26 19:23:06.000000 mmit-0.2.3/mmit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:23:06.000000 mmit-0.2.3/mmit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-26 19:23:06.000000 mmit-0.2.3/mmit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 19:23:06.000000 mmit-0.2.3/mmit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-26 19:22:54.000000 mmit-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 19:23:06.063470 mmit-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.063470 mmit-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-26 19:22:54.000000 mmit-0.2.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:23:06.063470 mmit-0.2.3/tests/demo_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 19:22:54.000000 mmit-0.2.3/tests/demo_blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-26 19:22:54.000000 mmit-0.2.3/tests/demo_blocks/classic_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 19:22:54.000000 mmit-0.2.3/tests/demo_blocks/classic_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-26 19:22:54.000000 mmit-0.2.3/tests/demo_blocks/cursed_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-26 19:22:54.000000 mmit-0.2.3/tests/test_base_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-26 19:22:54.000000 mmit-0.2.3/tests/test_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:22:54.000000 mmit-0.2.3/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-26 19:22:54.000000 mmit-0.2.3/tests/test_end2end.py
```

### Comparing `mmit-0.2.2/.github/issue_template.md` & `mmit-0.2.3/.github/issue_template.md`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/.github/pull_request_template.md` & `mmit-0.2.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/.github/workflows/python-publish.yml` & `mmit-0.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/.gitignore` & `mmit-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/LICENSE` & `mmit-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/PKG-INFO` & `mmit-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmit
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package for computer vision experiments and research.
 Author-email: Andrea Boscolo Camiletto <abcamiletto@gmail.com>
 Project-URL: Homepage, https://github.com/abcamiletto/mmit
 Project-URL: Repository, https://github.com/abcamiletto/mmit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mmit-0.2.2/README.md` & `mmit-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/docs/.readthedocs.yaml` & `mmit-0.2.3/docs/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/docs/Makefile` & `mmit-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/docs/make.bat` & `mmit-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/docs/source/_static/css/baseline.css` & `mmit-0.2.3/docs/source/_static/css/baseline.css`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/docs/source/_static/logo/logo.png` & `mmit-0.2.3/docs/source/_static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/docs/source/_static/logo/logo_title.png` & `mmit-0.2.3/docs/source/_static/logo/logo_title.png`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/docs/source/conf.py` & `mmit-0.2.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/docs/source/guide/examples.md` & `mmit-0.2.3/docs/source/guide/examples.md`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/docs/source/index.md` & `mmit-0.2.3/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/base/activations.py` & `mmit-0.2.3/mmit/base/activations.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/base/extra.py` & `mmit-0.2.3/mmit/base/extra.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/base/mismatch.py` & `mmit-0.2.3/mmit/base/mismatch.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/base/norms.py` & `mmit-0.2.3/mmit/base/norms.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/base/upsamplers.py` & `mmit-0.2.3/mmit/base/upsamplers.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/decoders/basedecoder.py` & `mmit-0.2.3/mmit/decoders/basedecoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/decoders/deeplabv3/aspp.py` & `mmit-0.2.3/mmit/decoders/deeplabv3/aspp.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/decoders/deeplabv3/model.py` & `mmit-0.2.3/mmit/decoders/deeplabv3/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/decoders/deeplabv3/parts.py` & `mmit-0.2.3/mmit/decoders/deeplabv3/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/decoders/deeplabv3plus/model.py` & `mmit-0.2.3/mmit/decoders/deeplabv3plus/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/decoders/deeplabv3plus/parts.py` & `mmit-0.2.3/mmit/decoders/deeplabv3plus/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/decoders/fpn/model.py` & `mmit-0.2.3/mmit/decoders/fpn/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/decoders/fpn/parts.py` & `mmit-0.2.3/mmit/decoders/fpn/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/decoders/unet/model.py` & `mmit-0.2.3/mmit/decoders/unet/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/decoders/unet/parts.py` & `mmit-0.2.3/mmit/decoders/unet/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/decoders/unetplusplus/model.py` & `mmit-0.2.3/mmit/decoders/unetplusplus/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/decoders/utils/resize.py` & `mmit-0.2.3/mmit/decoders/utils/resize.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/encoders/basencoder.py` & `mmit-0.2.3/mmit/encoders/basencoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/encoders/timm/model.py` & `mmit-0.2.3/mmit/encoders/timm/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/factory/components.py` & `mmit-0.2.3/mmit/factory/components.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/factory/factory.py` & `mmit-0.2.3/mmit/factory/factory.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/factory/registry.py` & `mmit-0.2.3/mmit/factory/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 import timm
 import torch.nn as nn
 
 __all__ = [
     "list_encoders",
     "list_decoders",
+    "list_heads",
     "register_decoder",
     "register_encoder",
+    "register_head",
     "register",
 ]
 
 
 class Registry:
     _decoders: Dict[str, Type[nn.Module]] = {}
     _encoders: Dict[str, Type[nn.Module]] = {}
@@ -65,16 +67,20 @@
         if name not in cls._encoders:
             raise KeyError(f"Encoder {name} is not registered")
 
         return cls._encoders[name]
 
     @classmethod
     def get_head(cls, name: str) -> Type[nn.Module]:
+        if (name not in cls._heads) and ((name + "head") not in cls._heads):
+            raise KeyError(f"Head '{name}' is not registered")
+
         if name not in cls._heads:
-            raise KeyError(f"Head {name} is not registered")
+            name = name + "head"
+
         return cls._heads[name]
 
 
 register_decoder = Registry.register_decoder
 list_decoders = Registry.list_all_decoders
 get_decoder = Registry.get_decoder
 register_encoder = Registry.register_encoder
```

### Comparing `mmit-0.2.2/mmit/heads/classification.py` & `mmit-0.2.3/mmit/heads/classification.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/mmit/heads/segmentation.py` & `mmit-0.2.3/mmit/heads/segmentation.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,17 @@
         in_channels: int,
         out_channels: int,
         kernel_size: int = 3,
         activation_layer: Type[nn.Module] = nn.Identity,
         extra_layer: Type[nn.Module] = nn.Identity,
     ):
         super().__init__()
-        self.conv = nn.Conv2d(in_channels, out_channels, kernel_size)
+        self.conv = nn.Conv2d(
+            in_channels, out_channels, kernel_size, padding=kernel_size // 2
+        )
         self.activation = activation_layer()
         self.extra = extra_layer()
 
     def forward(self, x: Tensor) -> Tensor:
         x = self.conv(x)
         x = self.activation(x)
         x = self.extra(x)
```

### Comparing `mmit-0.2.2/mmit.egg-info/PKG-INFO` & `mmit-0.2.3/mmit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmit
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package for computer vision experiments and research.
 Author-email: Andrea Boscolo Camiletto <abcamiletto@gmail.com>
 Project-URL: Homepage, https://github.com/abcamiletto/mmit
 Project-URL: Repository, https://github.com/abcamiletto/mmit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mmit-0.2.2/mmit.egg-info/SOURCES.txt` & `mmit-0.2.3/mmit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/pyproject.toml` & `mmit-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 readme = "README.md"
 authors = [{ name = "Andrea Boscolo Camiletto", email = "abcamiletto@gmail.com" }]
 dependencies = [
     "timm>=0.9.0",
     "torch>=1.10"
 ]
 requires-python = ">=3.8"
-version = "0.2.2"
+version = "0.2.3"
 
 [project.urls]
 Homepage = "https://github.com/abcamiletto/mmit"
 Repository = "https://github.com/abcamiletto/mmit"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pytest", "pytest-cov", "pytest-lazy-fixture", "pre-commit"]
```

### Comparing `mmit-0.2.2/tests/demo_blocks/classic_decoder.py` & `mmit-0.2.3/tests/demo_blocks/classic_decoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/tests/demo_blocks/classic_encoder.py` & `mmit-0.2.3/tests/demo_blocks/classic_encoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/tests/demo_blocks/cursed_encoder.py` & `mmit-0.2.3/tests/demo_blocks/cursed_encoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/tests/test_base_components.py` & `mmit-0.2.3/tests/test_base_components.py`

 * *Files identical despite different names*

### Comparing `mmit-0.2.2/tests/test_decoders.py` & `mmit-0.2.3/tests/test_decoders.py`

 * *Files identical despite different names*

