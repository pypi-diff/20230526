# Comparing `tmp/burdoc-0.2.1.tar.gz` & `tmp/burdoc-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burdoc-0.2.1.tar", last modified: Mon Apr 10 11:18:13 2023, max compression
+gzip compressed data, was "burdoc-0.2.2.tar", last modified: Fri May 26 16:51:24 2023, max compression
```

## Comparing `burdoc-0.2.1.tar` & `burdoc-0.2.2.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.878250 burdoc-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.842248 burdoc-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.850249 burdoc-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-10 11:17:57.000000 burdoc-0.2.1/.github/workflows/build-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-10 11:17:57.000000 burdoc-0.2.1/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-10 11:17:57.000000 burdoc-0.2.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 11:17:57.000000 burdoc-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-04-10 11:17:57.000000 burdoc-0.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-10 11:17:57.000000 burdoc-0.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-10 11:17:57.000000 burdoc-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-10 11:18:13.878250 burdoc-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-04-10 11:17:57.000000 burdoc-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.850249 burdoc-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.850249 burdoc-0.2.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.850249 burdoc-0.2.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    55532 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/_static/Burdoc-1.png
--rw-r--r--   0 runner    (1001) docker     (123)    95456 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/_static/Burdoc-leaf.png
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.850249 burdoc-0.2.1/docs/source/module/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/module/burdoc_parser.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/module/elements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/module/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.854249 burdoc-0.2.1/docs/source/module/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/module/processors/aggregator_processor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/module/processors/heading_processor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/module/processors/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/module/processors/json_out_processor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/module/processors/layout_processor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/module/processors/list_processor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/module/processors/margin_processor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/module/processors/pdf_load_processor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/module/processors/processor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/module/processors/reading_order_processor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/module/processors/table_processors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/module/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-04-10 11:17:57.000000 burdoc-0.2.1/docs/source/output.md
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-10 11:17:57.000000 burdoc-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.854249 burdoc-0.2.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 11:17:57.000000 burdoc-0.2.1/scripts/compare_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    22968 2023-04-10 11:17:57.000000 burdoc-0.2.1/scripts/explore_test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 11:18:13.878250 burdoc-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.846248 burdoc-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.854249 burdoc-0.2.1/src/burdoc/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/burdoc_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.854249 burdoc-0.2.1/src/burdoc/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/elements/aside.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/elements/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/elements/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/elements/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/elements/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/elements/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/elements/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/elements/section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/elements/span.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/elements/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/elements/textblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/elements/textlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.858249 burdoc-0.2.1/src/burdoc/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/aggregator_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/heading_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/json_out_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16372 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/layout_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/list_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/margin_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.858249 burdoc-0.2.1/src/burdoc/processors/pdf_load_processor/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/pdf_load_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/pdf_load_processor/drawing_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13462 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/pdf_load_processor/image_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/pdf_load_processor/pdf_load_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/pdf_load_processor/text_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17183 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/reading_order_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.858249 burdoc-0.2.1/src/burdoc/processors/table_processors/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/table_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/table_processors/detr_table_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/table_processors/ml_table_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    23140 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/table_processors/rules_table_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/processors/table_processors/table_extractor_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.858249 burdoc-0.2.1/src/burdoc/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/scripts/burdoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.858249 burdoc-0.2.1/src/burdoc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/utils/image_manip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/utils/json_to_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/utils/layout_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/utils/regexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-10 11:17:57.000000 burdoc-0.2.1/src/burdoc/utils/render_pages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.854249 burdoc-0.2.1/src/burdoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-10 11:18:13.000000 burdoc-0.2.1/src/burdoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-04-10 11:18:13.000000 burdoc-0.2.1/src/burdoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 11:18:13.000000 burdoc-0.2.1/src/burdoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-10 11:18:13.000000 burdoc-0.2.1/src/burdoc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-10 11:18:13.000000 burdoc-0.2.1/src/burdoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 11:18:13.000000 burdoc-0.2.1/src/burdoc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.846248 burdoc-0.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.858249 burdoc-0.2.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)    34827 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/.burdoc.log
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.858249 burdoc-0.2.1/tests/integration/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.866249 burdoc-0.2.1/tests/integration/data/gold/
--rw-r--r--   0 runner    (1001) docker     (123)    29472 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/all_text_types_3.json
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/blockquote.json
--rw-r--r--   0 runner    (1001) docker     (123)    25697 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/blockquote_columns.json
--rw-r--r--   0 runner    (1001) docker     (123)    25753 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/column_switch.json
--rw-r--r--   0 runner    (1001) docker     (123)    33575 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/columns_with_headers.json
--rw-r--r--   0 runner    (1001) docker     (123)    26959 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/complex_doc.json
--rw-r--r--   0 runner    (1001) docker     (123)    28010 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/complex_doc_2.json
--rw-r--r--   0 runner    (1001) docker     (123)   110901 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/complex_fonts.json
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/drawing_bullets.json
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/duplicate_text.json
--rw-r--r--   0 runner    (1001) docker     (123)    66454 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/end_image.json
--rw-r--r--   0 runner    (1001) docker     (123)    66581 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/image_above_text.json
--rw-r--r--   0 runner    (1001) docker     (123)    66579 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/inline_images.json
--rw-r--r--   0 runner    (1001) docker     (123)    29433 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/inline_simple_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)    32852 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/lists.json
--rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/nested_lists.json
--rw-r--r--   0 runner    (1001) docker     (123)    48361 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/nested_lists_columns.json
--rw-r--r--   0 runner    (1001) docker     (123)    73264 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/out_of_line_image.json
--rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/structured_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)    40464 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/tables.json
--rw-r--r--   0 runner    (1001) docker     (123)    45546 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/three_columns.json
--rw-r--r--   0 runner    (1001) docker     (123)    39031 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/three_columns_landscape.json
--rw-r--r--   0 runner    (1001) docker     (123)    30428 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/two_columns.json
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/two_paragraphs.json
--rw-r--r--   0 runner    (1001) docker     (123)    62527 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/gold/wrapped_images.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.870249 burdoc-0.2.1/tests/integration/data/html/
--rw-r--r--   0 runner    (1001) docker     (123)    29828 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/all_text_types_3.html
--rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/blockquote.html
--rw-r--r--   0 runner    (1001) docker     (123)    18733 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/blockquote_columns.html
--rw-r--r--   0 runner    (1001) docker     (123)    21654 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/column_switch.html
--rw-r--r--   0 runner    (1001) docker     (123)    29957 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/columns_with_headers.html
--rw-r--r--   0 runner    (1001) docker     (123)    22183 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/complex_doc.html
--rw-r--r--   0 runner    (1001) docker     (123)    23065 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/complex_doc_2.html
--rw-r--r--   0 runner    (1001) docker     (123)    58696 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/complex_fonts.html
--rw-r--r--   0 runner    (1001) docker     (123)    14268 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/drawing_bullets.html
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/duplicate_text.html
--rw-r--r--   0 runner    (1001) docker     (123)   162656 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/end_image.html
--rw-r--r--   0 runner    (1001) docker     (123)   163916 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/image_above_text.html
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)   359418 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/inline_images.html
--rw-r--r--   0 runner    (1001) docker     (123)    22868 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/inline_simple_tables.html
--rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/lists.html
--rw-r--r--   0 runner    (1001) docker     (123)    26177 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/nested_lists.html
--rw-r--r--   0 runner    (1001) docker     (123)    46663 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/nested_lists_columns.html
--rw-r--r--   0 runner    (1001) docker     (123)   167138 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/out_of_line_image.html
--rw-r--r--   0 runner    (1001) docker     (123)    31434 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/tables.html
--rw-r--r--   0 runner    (1001) docker     (123)    35186 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/three_columns.html
--rw-r--r--   0 runner    (1001) docker     (123)    38498 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/three_columns_landscape.html
--rw-r--r--   0 runner    (1001) docker     (123)    21967 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/two_columns.html
--rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/two_paragraphs.html
--rw-r--r--   0 runner    (1001) docker     (123)   261135 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/html/wrapped_images.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.874249 burdoc-0.2.1/tests/integration/data/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)   179650 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/all_text_types_3.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    29051 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/blockquote.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/blockquote_columns.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/column_switch.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    68191 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/columns_with_headers.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    38923 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/complex_doc.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   139530 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/complex_doc_2.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   348284 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/complex_fonts.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    29916 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/drawing_bullets.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    43365 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/duplicate_text.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    93016 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/end_image.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    93026 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/image_above_text.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    73142 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/inline_images.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    53392 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/inline_simple_tables.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    60954 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/lists.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/nested_lists.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/nested_lists_columns.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    92014 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/out_of_line_image.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    75147 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/structured_tables.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   120823 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/tables.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    68392 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/three_columns.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    32116 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/three_columns_landscape.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/two_columns.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/two_paragraphs.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    72906 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/inputs/wrapped_images.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/report.json
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/data/scores.json
--rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/integration/run_integration_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.874249 burdoc-0.2.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.878250 burdoc-0.2.1/tests/unit/elements/
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/unit/elements/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/unit/elements/test_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/unit/elements/test_font.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/unit/elements/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/unit/elements/test_span.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.878250 burdoc-0.2.1/tests/unit/processors/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/unit/processors/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/unit/test_burdoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:18:13.878250 burdoc-0.2.1/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-10 11:17:57.000000 burdoc-0.2.1/tests/unit/utils/test_layout_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.823317 burdoc-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.795317 burdoc-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.795317 burdoc-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-26 16:51:05.000000 burdoc-0.2.2/.github/workflows/build-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-26 16:51:05.000000 burdoc-0.2.2/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-26 16:51:05.000000 burdoc-0.2.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-26 16:51:05.000000 burdoc-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-05-26 16:51:05.000000 burdoc-0.2.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-26 16:51:05.000000 burdoc-0.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 16:51:05.000000 burdoc-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-26 16:51:24.823317 burdoc-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-05-26 16:51:05.000000 burdoc-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.795317 burdoc-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.799317 burdoc-0.2.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.799317 burdoc-0.2.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    55532 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/_static/Burdoc-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    95456 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/_static/Burdoc-leaf.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.799317 burdoc-0.2.2/docs/source/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/module/burdoc_parser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/module/elements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/module/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.799317 burdoc-0.2.2/docs/source/module/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/module/processors/aggregator_processor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/module/processors/heading_processor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/module/processors/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/module/processors/json_out_processor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/module/processors/layout_processor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/module/processors/list_processor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/module/processors/margin_processor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/module/processors/pdf_load_processor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/module/processors/processor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/module/processors/reading_order_processor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/module/processors/table_processors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/module/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-05-26 16:51:05.000000 burdoc-0.2.2/docs/source/output.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-26 16:51:05.000000 burdoc-0.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.799317 burdoc-0.2.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 16:51:05.000000 burdoc-0.2.2/scripts/compare_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22968 2023-05-26 16:51:05.000000 burdoc-0.2.2/scripts/explore_test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:51:24.823317 burdoc-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.795317 burdoc-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.799317 burdoc-0.2.2/src/burdoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/burdoc_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.803317 burdoc-0.2.2/src/burdoc/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/elements/aside.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/elements/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/elements/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/elements/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/elements/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/elements/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/elements/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/elements/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/elements/span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/elements/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/elements/textblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/elements/textlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.803317 burdoc-0.2.2/src/burdoc/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/aggregator_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/heading_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/json_out_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16372 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/layout_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/list_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/margin_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.803317 burdoc-0.2.2/src/burdoc/processors/pdf_load_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/pdf_load_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/pdf_load_processor/drawing_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13462 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/pdf_load_processor/image_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/pdf_load_processor/pdf_load_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/pdf_load_processor/text_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17183 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/reading_order_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.807317 burdoc-0.2.2/src/burdoc/processors/table_processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/table_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/table_processors/detr_table_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/table_processors/ml_table_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23140 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/table_processors/rules_table_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/processors/table_processors/table_extractor_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.807317 burdoc-0.2.2/src/burdoc/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/scripts/burdoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.807317 burdoc-0.2.2/src/burdoc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/utils/image_manip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/utils/json_to_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/utils/layout_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/utils/regexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-26 16:51:05.000000 burdoc-0.2.2/src/burdoc/utils/render_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.799317 burdoc-0.2.2/src/burdoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-26 16:51:24.000000 burdoc-0.2.2/src/burdoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-05-26 16:51:24.000000 burdoc-0.2.2/src/burdoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:51:24.000000 burdoc-0.2.2/src/burdoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-26 16:51:24.000000 burdoc-0.2.2/src/burdoc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-26 16:51:24.000000 burdoc-0.2.2/src/burdoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 16:51:24.000000 burdoc-0.2.2/src/burdoc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.795317 burdoc-0.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.807317 burdoc-0.2.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)    34827 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/.burdoc.log
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.807317 burdoc-0.2.2/tests/integration/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.811317 burdoc-0.2.2/tests/integration/data/gold/
+-rw-r--r--   0 runner    (1001) docker     (123)    29472 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/all_text_types_3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/blockquote.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25697 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/blockquote_columns.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25753 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/column_switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33575 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/columns_with_headers.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26959 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/complex_doc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28010 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/complex_doc_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   110901 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/complex_fonts.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/drawing_bullets.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/duplicate_text.json
+-rw-r--r--   0 runner    (1001) docker     (123)    66454 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/end_image.json
+-rw-r--r--   0 runner    (1001) docker     (123)    66581 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/image_above_text.json
+-rw-r--r--   0 runner    (1001) docker     (123)    66579 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/inline_images.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29433 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/inline_simple_tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32852 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/lists.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/nested_lists.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48361 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/nested_lists_columns.json
+-rw-r--r--   0 runner    (1001) docker     (123)    73264 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/out_of_line_image.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/structured_tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40464 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)    45546 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/three_columns.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39031 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/three_columns_landscape.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30428 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/two_columns.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/two_paragraphs.json
+-rw-r--r--   0 runner    (1001) docker     (123)    62527 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/gold/wrapped_images.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.815317 burdoc-0.2.2/tests/integration/data/html/
+-rw-r--r--   0 runner    (1001) docker     (123)    29828 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/all_text_types_3.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/blockquote.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18733 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/blockquote_columns.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21654 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/column_switch.html
+-rw-r--r--   0 runner    (1001) docker     (123)    29957 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/columns_with_headers.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22183 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/complex_doc.html
+-rw-r--r--   0 runner    (1001) docker     (123)    23065 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/complex_doc_2.html
+-rw-r--r--   0 runner    (1001) docker     (123)    58696 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/complex_fonts.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14268 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/drawing_bullets.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/duplicate_text.html
+-rw-r--r--   0 runner    (1001) docker     (123)   162656 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/end_image.html
+-rw-r--r--   0 runner    (1001) docker     (123)   163916 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/image_above_text.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)   359418 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/inline_images.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22868 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/inline_simple_tables.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/lists.html
+-rw-r--r--   0 runner    (1001) docker     (123)    26177 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/nested_lists.html
+-rw-r--r--   0 runner    (1001) docker     (123)    46663 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/nested_lists_columns.html
+-rw-r--r--   0 runner    (1001) docker     (123)   167138 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/out_of_line_image.html
+-rw-r--r--   0 runner    (1001) docker     (123)    31434 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/tables.html
+-rw-r--r--   0 runner    (1001) docker     (123)    35186 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/three_columns.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38498 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/three_columns_landscape.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21967 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/two_columns.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/two_paragraphs.html
+-rw-r--r--   0 runner    (1001) docker     (123)   261135 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/html/wrapped_images.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.819317 burdoc-0.2.2/tests/integration/data/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)   179650 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/all_text_types_3.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    29051 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/blockquote.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/blockquote_columns.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/column_switch.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    68191 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/columns_with_headers.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    38923 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/complex_doc.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   139530 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/complex_doc_2.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   348284 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/complex_fonts.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    29916 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/drawing_bullets.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    43365 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/duplicate_text.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    93016 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/end_image.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    93026 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/image_above_text.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    73142 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/inline_images.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    53392 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/inline_simple_tables.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    60954 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/lists.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/nested_lists.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/nested_lists_columns.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    92014 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/out_of_line_image.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    75147 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/structured_tables.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   120823 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/tables.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    68392 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/three_columns.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    32116 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/three_columns_landscape.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/two_columns.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/two_paragraphs.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    72906 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/inputs/wrapped_images.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/report.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/data/scores.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/integration/run_integration_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.823317 burdoc-0.2.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.823317 burdoc-0.2.2/tests/unit/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/unit/elements/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/unit/elements/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/unit/elements/test_font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/unit/elements/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/unit/elements/test_span.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.823317 burdoc-0.2.2/tests/unit/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/unit/processors/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/unit/test_burdoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:51:24.823317 burdoc-0.2.2/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-05-26 16:51:05.000000 burdoc-0.2.2/tests/unit/utils/test_layout_graph.py
```

### Comparing `burdoc-0.2.1/.github/workflows/build-release.yml` & `burdoc-0.2.2/.github/workflows/build-release.yml`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/.github/workflows/pylint.yml` & `burdoc-0.2.2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/.github/workflows/python-package.yml` & `burdoc-0.2.2/.github/workflows/python-package.yml`

 * *Files 10% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         python -m pytest --cov=burdoc
         
     - name: Codecov
       uses: codecov/codecov-action@v3.1.1
       
     - name: Integration Tests
       run: |
-        python tests/integration/run_integration_tests.py
+        python tests/integration/run_integration_tests.py --update
     
     - name: Store Output on Failure
       uses: actions/upload-artifact@v3
       if: failure()
       with:
         name: integration-output
         path: tests/integration/data/report.json
```

### Comparing `burdoc-0.2.1/.pylintrc` & `burdoc-0.2.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/.readthedocs.yaml` & `burdoc-0.2.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/LICENSE` & `burdoc-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/PKG-INFO` & `burdoc-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burdoc
-Version: 0.2.1
+Version: 0.2.2
 Summary: Advanced PDF parsing for python
 Author: jennis0
 Project-URL: Homepage, https://github.com/jennis0/burdoc
 Project-URL: Bug Tracker, https://github.com/jennis0/burdoc/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: burdoc Version: 0.2.1 Summary: Advanced PDF parsing
+Metadata-Version: 2.1 Name: burdoc Version: 0.2.2 Summary: Advanced PDF parsing
 for python Author: jennis0 Project-URL: Homepage, https://github.com/jennis0/
 burdoc Project-URL: Bug Tracker, https://github.com/jennis0/burdoc/issues
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: General Classifier: Topic :: Text
```

### Comparing `burdoc-0.2.1/README.md` & `burdoc-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/docs/Makefile` & `burdoc-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/docs/make.bat` & `burdoc-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/docs/source/_static/Burdoc-1.png` & `burdoc-0.2.2/docs/source/_static/Burdoc-1.png`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/docs/source/_static/Burdoc-leaf.png` & `burdoc-0.2.2/docs/source/_static/Burdoc-leaf.png`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/docs/source/conf.py` & `burdoc-0.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/docs/source/getting_started.md` & `burdoc-0.2.2/docs/source/getting_started.md`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/docs/source/index.md` & `burdoc-0.2.2/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/docs/source/module/elements.rst` & `burdoc-0.2.2/docs/source/module/elements.rst`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/docs/source/module/processors/pdf_load_processor.rst` & `burdoc-0.2.2/docs/source/module/processors/pdf_load_processor.rst`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/docs/source/module/processors/table_processors.rst` & `burdoc-0.2.2/docs/source/module/processors/table_processors.rst`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/docs/source/module/utils.rst` & `burdoc-0.2.2/docs/source/module/utils.rst`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/docs/source/output.md` & `burdoc-0.2.2/docs/source/output.md`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/pyproject.toml` & `burdoc-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/scripts/compare_output.py` & `burdoc-0.2.2/scripts/compare_output.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/scripts/explore_test_results.py` & `burdoc-0.2.2/scripts/explore_test_results.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/burdoc_parser.py` & `burdoc-0.2.2/src/burdoc/burdoc_parser.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/elements/__init__.py` & `burdoc-0.2.2/src/burdoc/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/elements/bbox.py` & `burdoc-0.2.2/src/burdoc/elements/bbox.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/elements/drawing.py` & `burdoc-0.2.2/src/burdoc/elements/drawing.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/elements/element.py` & `burdoc-0.2.2/src/burdoc/elements/element.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/elements/font.py` & `burdoc-0.2.2/src/burdoc/elements/font.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/elements/image.py` & `burdoc-0.2.2/src/burdoc/elements/image.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/elements/line.py` & `burdoc-0.2.2/src/burdoc/elements/line.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/elements/section.py` & `burdoc-0.2.2/src/burdoc/elements/section.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/elements/span.py` & `burdoc-0.2.2/src/burdoc/elements/span.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/elements/table.py` & `burdoc-0.2.2/src/burdoc/elements/table.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/elements/textblock.py` & `burdoc-0.2.2/src/burdoc/elements/textblock.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/elements/textlist.py` & `burdoc-0.2.2/src/burdoc/elements/textlist.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/processors/__init__.py` & `burdoc-0.2.2/src/burdoc/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/processors/aggregator_processor.py` & `burdoc-0.2.2/src/burdoc/processors/aggregator_processor.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/processors/heading_processor.py` & `burdoc-0.2.2/src/burdoc/processors/heading_processor.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/processors/json_out_processor.py` & `burdoc-0.2.2/src/burdoc/processors/json_out_processor.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/processors/layout_processor.py` & `burdoc-0.2.2/src/burdoc/processors/layout_processor.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/processors/list_processor.py` & `burdoc-0.2.2/src/burdoc/processors/list_processor.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/processors/margin_processor.py` & `burdoc-0.2.2/src/burdoc/processors/margin_processor.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/processors/pdf_load_processor/drawing_handler.py` & `burdoc-0.2.2/src/burdoc/processors/pdf_load_processor/drawing_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             shape_info (Dict[str, Any]): A PyMuPDF shape dictionary
             page_colour (np.ndarray): An (r,g,b) array representing the primary page colour
 
         Returns:
             bool: True if this looks like a filled rectangle, False if it is not likely to be visible
         """
 
-        if 'fill_opacity' not in shape_info or shape_info['fill_opacity'] < 0.1:
+        if 'fill_opacity' not in shape_info or not shape_info['fill_opacity'] or shape_info['fill_opacity'] < 0.1:
             return False
 
         if np.linalg.norm(255.*np.array(shape_info['fill']) - page_colour) < 10:
             return False
 
         return True
```

### Comparing `burdoc-0.2.1/src/burdoc/processors/pdf_load_processor/image_handler.py` & `burdoc-0.2.2/src/burdoc/processors/pdf_load_processor/image_handler.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/processors/pdf_load_processor/pdf_load_processor.py` & `burdoc-0.2.2/src/burdoc/processors/pdf_load_processor/pdf_load_processor.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/processors/pdf_load_processor/text_handler.py` & `burdoc-0.2.2/src/burdoc/processors/pdf_load_processor/text_handler.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/processors/processor.py` & `burdoc-0.2.2/src/burdoc/processors/processor.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/processors/reading_order_processor.py` & `burdoc-0.2.2/src/burdoc/processors/reading_order_processor.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/processors/table_processors/detr_table_strategy.py` & `burdoc-0.2.2/src/burdoc/processors/table_processors/detr_table_strategy.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/processors/table_processors/ml_table_processor.py` & `burdoc-0.2.2/src/burdoc/processors/table_processors/ml_table_processor.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/processors/table_processors/rules_table_processor.py` & `burdoc-0.2.2/src/burdoc/processors/table_processors/rules_table_processor.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/processors/table_processors/table_extractor_strategy.py` & `burdoc-0.2.2/src/burdoc/processors/table_processors/table_extractor_strategy.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/scripts/burdoc.py` & `burdoc-0.2.2/src/burdoc/scripts/burdoc.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/utils/compare.py` & `burdoc-0.2.2/src/burdoc/utils/compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                 text = 'listitem-' + _hash(obj['items'])
     elif isinstance(obj, list):
         parts = [_hash(p) for p in obj]
         parts.sort()
         text = "-".join(parts)
     if not text:
         text = json.dumps(obj, sort_keys=True, indent=2)
-    return hashlib.md5(text.encode('utf-8'), usedforsecurity=False).hexdigest()
+    return hashlib.md5(text.encode('utf-8', 'replace'), usedforsecurity=False).hexdigest()
 
 
 def _diff_value(path: str, value1: Any, value2: Any) -> List[Dict[str, Any]]:
     if value1 != value2:
         return [{'path': path, 'type': 'change', 'old': value1, 'new': value2}]
     return []
```

### Comparing `burdoc-0.2.1/src/burdoc/utils/image_manip.py` & `burdoc-0.2.2/src/burdoc/utils/image_manip.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/utils/json_to_html.py` & `burdoc-0.2.2/src/burdoc/utils/json_to_html.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/utils/layout_graph.py` & `burdoc-0.2.2/src/burdoc/utils/layout_graph.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/utils/logging.py` & `burdoc-0.2.2/src/burdoc/utils/logging.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/utils/regexes.py` & `burdoc-0.2.2/src/burdoc/utils/regexes.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc/utils/render_pages.py` & `burdoc-0.2.2/src/burdoc/utils/render_pages.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/src/burdoc.egg-info/PKG-INFO` & `burdoc-0.2.2/src/burdoc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burdoc
-Version: 0.2.1
+Version: 0.2.2
 Summary: Advanced PDF parsing for python
 Author: jennis0
 Project-URL: Homepage, https://github.com/jennis0/burdoc
 Project-URL: Bug Tracker, https://github.com/jennis0/burdoc/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: burdoc Version: 0.2.1 Summary: Advanced PDF parsing
+Metadata-Version: 2.1 Name: burdoc Version: 0.2.2 Summary: Advanced PDF parsing
 for python Author: jennis0 Project-URL: Homepage, https://github.com/jennis0/
 burdoc Project-URL: Bug Tracker, https://github.com/jennis0/burdoc/issues
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: General Classifier: Topic :: Text
```

### Comparing `burdoc-0.2.1/src/burdoc.egg-info/SOURCES.txt` & `burdoc-0.2.2/src/burdoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/.burdoc.log` & `burdoc-0.2.2/tests/integration/.burdoc.log`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/all_text_types_3.json` & `burdoc-0.2.2/tests/integration/data/gold/all_text_types_3.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/blockquote.json` & `burdoc-0.2.2/tests/integration/data/gold/blockquote.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/blockquote_columns.json` & `burdoc-0.2.2/tests/integration/data/gold/blockquote_columns.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/column_switch.json` & `burdoc-0.2.2/tests/integration/data/gold/column_switch.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/columns_with_headers.json` & `burdoc-0.2.2/tests/integration/data/gold/columns_with_headers.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/complex_doc.json` & `burdoc-0.2.2/tests/integration/data/gold/complex_doc.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/complex_doc_2.json` & `burdoc-0.2.2/tests/integration/data/gold/complex_doc_2.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/complex_fonts.json` & `burdoc-0.2.2/tests/integration/data/gold/complex_fonts.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/drawing_bullets.json` & `burdoc-0.2.2/tests/integration/data/gold/drawing_bullets.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/duplicate_text.json` & `burdoc-0.2.2/tests/integration/data/gold/duplicate_text.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/end_image.json` & `burdoc-0.2.2/tests/integration/data/gold/end_image.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/image_above_text.json` & `burdoc-0.2.2/tests/integration/data/gold/image_above_text.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/inline_images.json` & `burdoc-0.2.2/tests/integration/data/gold/inline_images.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/inline_simple_tables.json` & `burdoc-0.2.2/tests/integration/data/gold/inline_simple_tables.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/lists.json` & `burdoc-0.2.2/tests/integration/data/gold/lists.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/nested_lists.json` & `burdoc-0.2.2/tests/integration/data/gold/nested_lists.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/nested_lists_columns.json` & `burdoc-0.2.2/tests/integration/data/gold/nested_lists_columns.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/out_of_line_image.json` & `burdoc-0.2.2/tests/integration/data/gold/out_of_line_image.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/structured_tables.json` & `burdoc-0.2.2/tests/integration/data/gold/structured_tables.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/tables.json` & `burdoc-0.2.2/tests/integration/data/gold/tables.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/three_columns.json` & `burdoc-0.2.2/tests/integration/data/gold/three_columns.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/three_columns_landscape.json` & `burdoc-0.2.2/tests/integration/data/gold/three_columns_landscape.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/two_columns.json` & `burdoc-0.2.2/tests/integration/data/gold/two_columns.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/two_paragraphs.json` & `burdoc-0.2.2/tests/integration/data/gold/two_paragraphs.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/gold/wrapped_images.json` & `burdoc-0.2.2/tests/integration/data/gold/wrapped_images.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/all_text_types_3.html` & `burdoc-0.2.2/tests/integration/data/html/all_text_types_3.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/blockquote.html` & `burdoc-0.2.2/tests/integration/data/html/blockquote.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/blockquote_columns.html` & `burdoc-0.2.2/tests/integration/data/html/blockquote_columns.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/column_switch.html` & `burdoc-0.2.2/tests/integration/data/html/column_switch.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/columns_with_headers.html` & `burdoc-0.2.2/tests/integration/data/html/columns_with_headers.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/complex_doc.html` & `burdoc-0.2.2/tests/integration/data/html/complex_doc.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/complex_doc_2.html` & `burdoc-0.2.2/tests/integration/data/html/complex_doc_2.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/complex_fonts.html` & `burdoc-0.2.2/tests/integration/data/html/complex_fonts.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/drawing_bullets.html` & `burdoc-0.2.2/tests/integration/data/html/drawing_bullets.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/duplicate_text.html` & `burdoc-0.2.2/tests/integration/data/html/duplicate_text.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/end_image.html` & `burdoc-0.2.2/tests/integration/data/html/end_image.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/image_above_text.html` & `burdoc-0.2.2/tests/integration/data/html/image_above_text.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/index.html` & `burdoc-0.2.2/tests/integration/data/html/index.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/inline_images.html` & `burdoc-0.2.2/tests/integration/data/html/inline_images.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/inline_simple_tables.html` & `burdoc-0.2.2/tests/integration/data/html/inline_simple_tables.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/lists.html` & `burdoc-0.2.2/tests/integration/data/html/lists.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/nested_lists.html` & `burdoc-0.2.2/tests/integration/data/html/nested_lists.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/nested_lists_columns.html` & `burdoc-0.2.2/tests/integration/data/html/nested_lists_columns.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/out_of_line_image.html` & `burdoc-0.2.2/tests/integration/data/html/out_of_line_image.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/tables.html` & `burdoc-0.2.2/tests/integration/data/html/tables.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/three_columns.html` & `burdoc-0.2.2/tests/integration/data/html/three_columns.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/three_columns_landscape.html` & `burdoc-0.2.2/tests/integration/data/html/three_columns_landscape.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/two_columns.html` & `burdoc-0.2.2/tests/integration/data/html/two_columns.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/two_paragraphs.html` & `burdoc-0.2.2/tests/integration/data/html/two_paragraphs.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/html/wrapped_images.html` & `burdoc-0.2.2/tests/integration/data/html/wrapped_images.html`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/all_text_types_3.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/all_text_types_3.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/blockquote.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/blockquote.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/blockquote_columns.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/blockquote_columns.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/column_switch.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/column_switch.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/columns_with_headers.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/columns_with_headers.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/complex_doc.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/complex_doc.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/complex_doc_2.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/complex_doc_2.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/complex_fonts.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/complex_fonts.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/drawing_bullets.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/drawing_bullets.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/duplicate_text.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/duplicate_text.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/end_image.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/end_image.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/image_above_text.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/image_above_text.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/inline_images.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/inline_images.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/inline_simple_tables.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/inline_simple_tables.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/lists.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/lists.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/nested_lists.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/nested_lists.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/nested_lists_columns.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/nested_lists_columns.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/out_of_line_image.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/out_of_line_image.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/structured_tables.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/structured_tables.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/tables.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/tables.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/three_columns.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/three_columns.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/three_columns_landscape.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/three_columns_landscape.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/two_columns.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/two_columns.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/two_paragraphs.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/two_paragraphs.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/inputs/wrapped_images.pdf` & `burdoc-0.2.2/tests/integration/data/inputs/wrapped_images.pdf`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/data/report.json` & `burdoc-0.2.2/tests/integration/data/report.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.828125%*

 * *Differences: {"'files'": "{'all_text_types_3': {'processing_time': 1.833}, 'blockquote': {'processing_time': "*

 * *            "0.63}, 'blockquote_columns': {'processing_time': 0.602}, 'columns_with_headers': "*

 * *            "{'processing_time': 0.614}, 'column_switch': {'processing_time': 1.195}, "*

 * *            "'complex_doc': {'processing_time': 0.592}, 'complex_doc_2': {'processing_time': "*

 * *            "0.973}, 'complex_fonts': {'processing_time': 1.729}, 'drawing_bullets': "*

 * *            "{'processing_time': 0.565}, 'duplic […]*

```diff
@@ -1,159 +1,159 @@
 {
     "files": {
         "all_text_types_3": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\all_text_types_3.pdf",
             "filetitle": "all_text_types_3",
-            "processing_time": 1.788
+            "processing_time": 1.833
         },
         "blockquote": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\blockquote.pdf",
             "filetitle": "blockquote",
-            "processing_time": 0.647
+            "processing_time": 0.63
         },
         "blockquote_columns": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\blockquote_columns.pdf",
             "filetitle": "blockquote_columns",
-            "processing_time": 0.63
+            "processing_time": 0.602
         },
         "column_switch": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\column_switch.pdf",
             "filetitle": "column_switch",
-            "processing_time": 1.278
+            "processing_time": 1.195
         },
         "columns_with_headers": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\columns_with_headers.pdf",
             "filetitle": "columns_with_headers",
-            "processing_time": 0.586
+            "processing_time": 0.614
         },
         "complex_doc": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\complex_doc.pdf",
             "filetitle": "complex_doc",
-            "processing_time": 0.584
+            "processing_time": 0.592
         },
         "complex_doc_2": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\complex_doc_2.pdf",
             "filetitle": "complex_doc_2",
-            "processing_time": 1.017
+            "processing_time": 0.973
         },
         "complex_fonts": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\complex_fonts.pdf",
             "filetitle": "complex_fonts",
-            "processing_time": 1.779
+            "processing_time": 1.729
         },
         "drawing_bullets": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\drawing_bullets.pdf",
             "filetitle": "drawing_bullets",
-            "processing_time": 0.584
+            "processing_time": 0.565
         },
         "duplicate_text": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\duplicate_text.pdf",
             "filetitle": "duplicate_text",
-            "processing_time": 0.555
+            "processing_time": 0.557
         },
         "end_image": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\end_image.pdf",
             "filetitle": "end_image",
-            "processing_time": 0.826
+            "processing_time": 0.796
         },
         "image_above_text": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\image_above_text.pdf",
             "filetitle": "image_above_text",
-            "processing_time": 0.744
+            "processing_time": 0.733
         },
         "inline_images": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\inline_images.pdf",
             "filetitle": "inline_images",
-            "processing_time": 0.985
+            "processing_time": 0.933
         },
         "inline_simple_tables": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\inline_simple_tables.pdf",
             "filetitle": "inline_simple_tables",
-            "processing_time": 1.061
+            "processing_time": 1.04
         },
         "lists": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\lists.pdf",
             "filetitle": "lists",
-            "processing_time": 0.575
+            "processing_time": 0.58
         },
         "nested_lists": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\nested_lists.pdf",
             "filetitle": "nested_lists",
-            "processing_time": 1.076
+            "processing_time": 1.162
         },
         "nested_lists_columns": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\nested_lists_columns.pdf",
             "filetitle": "nested_lists_columns",
-            "processing_time": 1.613
+            "processing_time": 1.565
         },
         "out_of_line_image": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\out_of_line_image.pdf",
             "filetitle": "out_of_line_image",
-            "processing_time": 0.7
+            "processing_time": 0.69
         },
         "structured_tables": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\structured_tables.pdf",
             "filetitle": "structured_tables",
-            "processing_time": 4.524
+            "processing_time": 4.602
         },
         "tables": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\tables.pdf",
             "filetitle": "tables",
-            "processing_time": 1.135
+            "processing_time": 1.092
         },
         "three_columns": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\three_columns.pdf",
             "filetitle": "three_columns",
-            "processing_time": 0.614
+            "processing_time": 0.608
         },
         "three_columns_landscape": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\three_columns_landscape.pdf",
             "filetitle": "three_columns_landscape",
-            "processing_time": 0.596
+            "processing_time": 0.593
         },
         "two_columns": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\two_columns.pdf",
             "filetitle": "two_columns",
-            "processing_time": 0.58
+            "processing_time": 0.562
         },
         "two_paragraphs": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\two_paragraphs.pdf",
             "filetitle": "two_paragraphs",
-            "processing_time": 1.1
+            "processing_time": 1.086
         },
         "wrapped_images": {
             "changes": {},
             "filename": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs\\wrapped_images.pdf",
             "filetitle": "wrapped_images",
-            "processing_time": 0.785
+            "processing_time": 0.795
         }
     },
     "gold_dir": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\gold",
     "in_dir": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\inputs",
     "out_dir": "C:\\Users\\jenni\\OneDrive\\Documents\\Code\\burdoc\\burdoc\\tests\\integration\\data\\outputs",
-    "processing_time": 27.592,
-    "timestamp": "04/10/2023-09:12:18"
+    "processing_time": 27.385,
+    "timestamp": "05/26/2023-17:26:20"
 }
```

### Comparing `burdoc-0.2.1/tests/integration/data/scores.json` & `burdoc-0.2.2/tests/integration/data/scores.json`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/integration/run_integration_tests.py` & `burdoc-0.2.2/tests/integration/run_integration_tests.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/unit/elements/test_bbox.py` & `burdoc-0.2.2/tests/unit/elements/test_bbox.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/unit/elements/test_element.py` & `burdoc-0.2.2/tests/unit/elements/test_element.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/unit/elements/test_font.py` & `burdoc-0.2.2/tests/unit/elements/test_font.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/unit/elements/test_line.py` & `burdoc-0.2.2/tests/unit/elements/test_line.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/unit/elements/test_span.py` & `burdoc-0.2.2/tests/unit/elements/test_span.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/unit/processors/test_processor.py` & `burdoc-0.2.2/tests/unit/processors/test_processor.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/unit/test_burdoc.py` & `burdoc-0.2.2/tests/unit/test_burdoc.py`

 * *Files identical despite different names*

### Comparing `burdoc-0.2.1/tests/unit/utils/test_layout_graph.py` & `burdoc-0.2.2/tests/unit/utils/test_layout_graph.py`

 * *Files identical despite different names*

