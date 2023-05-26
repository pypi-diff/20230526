# Comparing `tmp/cognite_neat-0.12.0.tar.gz` & `tmp/cognite_neat-0.12.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.12.0.tar", max compression
+gzip compressed data, was "cognite_neat-0.12.1.tar", max compression
```

## Comparing `cognite_neat-0.12.0.tar` & `cognite_neat-0.12.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0    11351 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/LICENSE
--rw-r--r--   0        0        0     8765 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/README.md
--rw-r--r--   0        0        0       23 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/__init__.py
--rw-r--r--   0        0        0      616 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/constants.py
--rw-r--r--   0        0        0        0 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/__init__.py
--rw-r--r--   0        0        0     2652 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/app.py
--rw-r--r--   0        0        0     1344 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/configuration.py
--rw-r--r--   0        0        0      408 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/data_classes/__init__.py
--rw-r--r--   0        0        0     4670 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/data_classes/config.py
--rw-r--r--   0        0        0     8132 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/data_classes/rules.py
--rw-r--r--   0        0        0    28433 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/data_classes/transformation_rules.py
--rw-r--r--   0        0        0        0 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/data_stores/__init__.py
--rw-r--r--   0        0        0     1520 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/data_stores/metrics.py
--rw-r--r--   0        0        0     9436 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/data_stores/oxrdflib.py
--rw-r--r--   0        0        0      470 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/extractors/__init__.py
--rw-r--r--   0        0        0     2250 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/extractors/labels.py
--rw-r--r--   0        0        0    34295 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/extractors/rdf_to_assets.py
--rw-r--r--   0        0        0    16995 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/extractors/rdf_to_relationships.py
--rw-r--r--   0        0        0     6700 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/extractors/rules_to_graphql.py
--rw-r--r--   0        0        0      115 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/loader/__init__.py
--rw-r--r--   0        0        0      711 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/loader/config.py
--rw-r--r--   0        0        0     1210 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/loader/graph.py
--rw-r--r--   0        0        0    10647 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/loader/graph_store.py
--rw-r--r--   0        0        0      913 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/loader/rules.py
--rw-r--r--   0        0        0        0 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/mocks/__init__.py
--rw-r--r--   0        0        0    12025 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/mocks/graph.py
--rw-r--r--   0        0        0    15303 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/modeler.py
--rw-r--r--   0        0        0      110 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/parser/__init__.py
--rw-r--r--   0        0        0     1727 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/parser/transformation_rules.py
--rw-r--r--   0        0        0       73 2023-05-23 13:09:59.805608 cognite_neat-0.12.0/cognite/neat/core/query_generator/__init__.py
--rw-r--r--   0        0        0     9595 2023-05-23 13:09:59.809608 cognite_neat-0.12.0/cognite/neat/core/query_generator/sparql.py
--rw-r--r--   0        0        0    10943 2023-05-23 13:09:59.809608 cognite_neat-0.12.0/cognite/neat/core/transformer.py
--rw-r--r--   0        0        0     3621 2023-05-23 13:09:59.809608 cognite_neat-0.12.0/cognite/neat/core/utils.py
--rw-r--r--   0        0        0     2558 2023-05-23 13:09:59.809608 cognite_neat-0.12.0/cognite/neat/core/validator.py
--rw-r--r--   0        0        0      311 2023-05-23 13:09:59.809608 cognite_neat-0.12.0/cognite/neat/core/workflow/__init__.py
--rw-r--r--   0        0        0    18140 2023-05-23 13:09:59.809608 cognite_neat-0.12.0/cognite/neat/core/workflow/base.py
--rw-r--r--   0        0        0    17630 2023-05-23 13:09:59.809608 cognite_neat-0.12.0/cognite/neat/core/workflow/cdf_store.py
--rw-r--r--   0        0        0     6200 2023-05-23 13:09:59.809608 cognite_neat-0.12.0/cognite/neat/core/workflow/manager.py
--rw-r--r--   0        0        0     3348 2023-05-23 13:09:59.809608 cognite_neat-0.12.0/cognite/neat/core/workflow/model.py
--rw-r--r--   0        0        0      781 2023-05-23 13:09:59.809608 cognite_neat-0.12.0/cognite/neat/core/workflow/tasks.py
--rw-r--r--   0        0        0     6648 2023-05-23 13:09:59.809608 cognite_neat-0.12.0/cognite/neat/core/workflow/triggers.py
--rw-r--r--   0        0        0      453 2023-05-23 13:09:59.809608 cognite_neat-0.12.0/cognite/neat/core/workflow/utils.py
--rw-r--r--   0        0        0    79580 2023-05-23 13:09:59.809608 cognite_neat-0.12.0/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    52178 2023-05-23 13:09:59.809608 cognite_neat-0.12.0/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0  1437851 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0     1461 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/examples/workflows/basic/workflow.py
--rw-r--r--   0        0        0     1782 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/examples/workflows/basic/workflow.yaml
--rw-r--r--   0        0        0    15541 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/examples/workflows/default/workflow.py
--rw-r--r--   0        0        0     6774 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/examples/workflows/default/workflow.yaml
--rw-r--r--   0        0        0    15552 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/examples/workflows/fast_graph/workflow.py
--rw-r--r--   0        0        0     6969 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/examples/workflows/fast_graph/workflow.yaml
--rw-r--r--   0        0        0    11477 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/examples/workflows/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4792 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0    13084 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/examples/workflows/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6025 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0        0 2023-05-23 13:09:59.861608 cognite_neat-0.12.0/cognite/neat/explorer/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 13:09:59.861608 cognite_neat-0.12.0/cognite/neat/explorer/data_classes/__init__.py
--rw-r--r--   0        0        0     1013 2023-05-23 13:09:59.861608 cognite_neat-0.12.0/cognite/neat/explorer/data_classes/rest.py
--rw-r--r--   0        0        0    19784 2023-05-23 13:09:59.861608 cognite_neat-0.12.0/cognite/neat/explorer/explorer.py
--rw-r--r--   0        0        0        0 2023-05-23 13:09:59.861608 cognite_neat-0.12.0/cognite/neat/explorer/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-05-23 13:09:59.861608 cognite_neat-0.12.0/cognite/neat/explorer/utils/data_mapping.py
--rw-r--r--   0        0        0     4003 2023-05-23 13:09:59.861608 cognite_neat-0.12.0/cognite/neat/explorer/utils/query_templates.py
--rw-r--r--   0        0        0       16 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/explorer-ui/index.html
--rw-r--r--   0        0        0      312 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2023-05-23 13:09:59.813608 cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1357145 2023-05-23 13:09:59.825608 cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.31582da0.js
--rw-r--r--   0        0        0     2667 2023-05-23 13:09:59.825608 cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.31582da0.js.LICENSE.txt
--rw-r--r--   0        0        0  5847225 2023-05-23 13:09:59.853608 cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.31582da0.js.map
--rw-r--r--   0        0        0     2633 2023-05-23 13:09:59.853608 cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      358 2023-05-23 13:09:59.861608 cognite_neat-0.12.0/cognite/neat/main.py
--rw-r--r--   0        0        0        0 2023-05-23 13:09:59.861608 cognite_neat-0.12.0/cognite/neat/migration/__init__.py
--rw-r--r--   0        0        0     1581 2023-05-23 13:09:59.861608 cognite_neat-0.12.0/cognite/neat/migration/wf_manifests.py
--rw-r--r--   0        0        0     2403 2023-05-23 13:10:00.301607 cognite_neat-0.12.0/pyproject.toml
--rw-r--r--   0        0        0    10191 1970-01-01 00:00:00.000000 cognite_neat-0.12.0/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/LICENSE
+-rw-r--r--   0        0        0     8765 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/README.md
+-rw-r--r--   0        0        0       23 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/__init__.py
+-rw-r--r--   0        0        0      616 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/constants.py
+-rw-r--r--   0        0        0        0 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/__init__.py
+-rw-r--r--   0        0        0     2652 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/app.py
+-rw-r--r--   0        0        0     1344 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/configuration.py
+-rw-r--r--   0        0        0      408 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/data_classes/__init__.py
+-rw-r--r--   0        0        0     4670 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/data_classes/config.py
+-rw-r--r--   0        0        0     8132 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/data_classes/rules.py
+-rw-r--r--   0        0        0    28433 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/data_classes/transformation_rules.py
+-rw-r--r--   0        0        0        0 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/data_stores/__init__.py
+-rw-r--r--   0        0        0     1520 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/data_stores/metrics.py
+-rw-r--r--   0        0        0     9436 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0      470 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/extractors/__init__.py
+-rw-r--r--   0        0        0     2250 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/extractors/labels.py
+-rw-r--r--   0        0        0    35280 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/extractors/rdf_to_assets.py
+-rw-r--r--   0        0        0    17870 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/extractors/rdf_to_relationships.py
+-rw-r--r--   0        0        0     6700 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/extractors/rules_to_graphql.py
+-rw-r--r--   0        0        0      115 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/loader/__init__.py
+-rw-r--r--   0        0        0      711 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/loader/config.py
+-rw-r--r--   0        0        0     1210 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/loader/graph.py
+-rw-r--r--   0        0        0    10647 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/loader/graph_store.py
+-rw-r--r--   0        0        0      913 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/loader/rules.py
+-rw-r--r--   0        0        0        0 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/mocks/__init__.py
+-rw-r--r--   0        0        0    12025 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/mocks/graph.py
+-rw-r--r--   0        0        0    15303 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/modeler.py
+-rw-r--r--   0        0        0      110 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/parser/__init__.py
+-rw-r--r--   0        0        0     1727 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/parser/transformation_rules.py
+-rw-r--r--   0        0        0       73 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/query_generator/__init__.py
+-rw-r--r--   0        0        0     9595 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/query_generator/sparql.py
+-rw-r--r--   0        0        0    10943 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/transformer.py
+-rw-r--r--   0        0        0     4524 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/utils.py
+-rw-r--r--   0        0        0     2558 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/validator.py
+-rw-r--r--   0        0        0      311 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/workflow/__init__.py
+-rw-r--r--   0        0        0    18503 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/workflow/base.py
+-rw-r--r--   0        0        0    17764 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/workflow/cdf_store.py
+-rw-r--r--   0        0        0     6200 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/workflow/manager.py
+-rw-r--r--   0        0        0     3398 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/workflow/model.py
+-rw-r--r--   0        0        0      781 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/workflow/tasks.py
+-rw-r--r--   0        0        0     6648 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/workflow/triggers.py
+-rw-r--r--   0        0        0      453 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/workflow/utils.py
+-rw-r--r--   0        0        0    79580 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    52178 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0  1437851 2023-05-26 15:36:22.003277 cognite_neat-0.12.1/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0     1461 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/basic/workflow.py
+-rw-r--r--   0        0        0     1782 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/basic/workflow.yaml
+-rw-r--r--   0        0        0    15601 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/default/workflow.py
+-rw-r--r--   0        0        0     6774 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/default/workflow.yaml
+-rw-r--r--   0        0        0    16351 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/fast_graph/workflow.py
+-rw-r--r--   0        0        0     8068 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/fast_graph/workflow.yaml
+-rw-r--r--   0        0        0    11477 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4792 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0    13084 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6025 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0        0 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/explorer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/explorer/data_classes/__init__.py
+-rw-r--r--   0        0        0     1013 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/explorer/data_classes/rest.py
+-rw-r--r--   0        0        0    19784 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/explorer/explorer.py
+-rw-r--r--   0        0        0        0 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/explorer/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/explorer/utils/data_mapping.py
+-rw-r--r--   0        0        0     4003 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/explorer/utils/query_templates.py
+-rw-r--r--   0        0        0       16 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/index.html
+-rw-r--r--   0        0        0      312 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1357930 2023-05-26 15:36:22.015277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js
+-rw-r--r--   0        0        0     2667 2023-05-26 15:36:22.015277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.LICENSE.txt
+-rw-r--r--   0        0        0  5848771 2023-05-26 15:36:22.051277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.map
+-rw-r--r--   0        0        0     2633 2023-05-26 15:36:22.051277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      358 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/main.py
+-rw-r--r--   0        0        0        0 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/migration/__init__.py
+-rw-r--r--   0        0        0     1581 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/migration/wf_manifests.py
+-rw-r--r--   0        0        0     2471 2023-05-26 15:36:22.535279 cognite_neat-0.12.1/pyproject.toml
+-rw-r--r--   0        0        0    10241 1970-01-01 00:00:00.000000 cognite_neat-0.12.1/PKG-INFO
```

### Comparing `cognite_neat-0.12.0/LICENSE` & `cognite_neat-0.12.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/README.md` & `cognite_neat-0.12.1/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/constants.py` & `cognite_neat-0.12.1/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/app.py` & `cognite_neat-0.12.1/cognite/neat/core/app.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/configuration.py` & `cognite_neat-0.12.1/cognite/neat/core/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/data_classes/config.py` & `cognite_neat-0.12.1/cognite/neat/core/data_classes/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/data_classes/rules.py` & `cognite_neat-0.12.1/cognite/neat/core/data_classes/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/data_classes/transformation_rules.py` & `cognite_neat-0.12.1/cognite/neat/core/data_classes/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/data_stores/metrics.py` & `cognite_neat-0.12.1/cognite/neat/core/data_stores/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/data_stores/oxrdflib.py` & `cognite_neat-0.12.1/cognite/neat/core/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/extractors/labels.py` & `cognite_neat-0.12.1/cognite/neat/core/extractors/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/extractors/rdf_to_assets.py` & `cognite_neat-0.12.1/cognite/neat/core/extractors/rdf_to_assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from rdflib import Graph, Namespace
 from rdflib.term import URIRef
 
 from cognite.neat.core.data_classes import AssetTemplate, Property
 from cognite.neat.core.data_classes.config import EXCLUDE_PATHS
 from cognite.neat.core.data_classes.transformation_rules import TransformationRules
 from cognite.neat.core.loader.graph_store import NeatGraphStore
-from cognite.neat.core.utils import chunker, datetime_utc_now, remove_namespace
+from cognite.neat.core.utils import chunker, datetime_utc_now, remove_namespace, retry_decorator
 
 ORPHANAGE = {
     "external_id": "orphanage",
     "name": "Orphanage",
     "parent_external_id": None,
     "description": "Used to store all assets which parent does not exist",
     "metadata": {
@@ -815,15 +815,21 @@
         rdf_assets, cdf_assets, update_ids, stop_on_exception=stop_on_exception
     )
 
     return (categorized_assets, report) if return_report else categorized_assets
 
 
 def _micro_batch_push(
-    client: CogniteClient, assets: list, batch_size: int = 1000, push_type: str = "update", message: str = "Updated"
+    client: CogniteClient,
+    assets: list,
+    batch_size: int = 1000,
+    push_type: str = "update",
+    message: str = "Updated",
+    max_retries: int = 1,
+    retry_delay: int = 5,
 ):
     """Updates assets in batches of 1000
 
     Parameters
     ----------
     client : CogniteClient
         Instance of CogniteClient
@@ -834,80 +840,109 @@
     push_type : str, optional
         Type of push, either "update" or "create", by default "update"
     message : str, optional
         Message to logged, by default "Updated"
     """
     total = len(assets)
     counter = 0
-
+    if push_type not in ["update", "create"]:
+        logging.info(f"push_type {push_type} not supported")
+        raise ValueError(f"push_type {push_type} not supported")
     for batch in chunker(assets, batch_size):
         counter += len(batch)
         start_time = datetime_utc_now()
-        if push_type == "update":
-            client.assets.update(batch)
-        elif push_type == "create":
-            client.assets.create_hierarchy(batch)
-        else:
-            logging.info(f"push_type {push_type} not supported")
-            raise ValueError(f"push_type {push_type} not supported")
+
+        @retry_decorator(max_retries=max_retries, retry_delay=retry_delay, component_name="microbatch-assets")
+        def upsert_assets(batch):
+            if push_type == "update":
+                client.assets.update(batch)
+            elif push_type == "create":
+                client.assets.create_hierarchy(batch)
+
+        upsert_assets(batch)
 
         delta_time = (datetime_utc_now() - start_time).seconds
 
         msg = f"{message} {counter} of {total} assets, batch processing time: {delta_time:.2f} "
         msg += f"seconds ETC: {delta_time * (total - counter) / (60*batch_size) :.2f} minutes"
         logging.info(msg)
 
 
-def upload_assets(client: CogniteClient, categorized_assets: Dict[str, list], batch_size: int = 5000):
+def upload_assets(
+    client: CogniteClient,
+    categorized_assets: Dict[str, list],
+    batch_size: int = 5000,
+    max_retries: int = 1,
+    retry_delay: int = 3,
+):
     """Uploads categorized assets to CDF
 
     Parameters
     ----------
     client : CogniteClient
         Instance of CogniteClient
     categorized_assets : Dict[str, list]
         dictionary containing asset category - list of asset pairs
     batch_size : int, optional
         Size of batch, by default 5000
     """
     if batch_size:
         logging.info(f"Uploading assets in batches of {batch_size}")
         if categorized_assets["create"]:
-            _micro_batch_push(client, categorized_assets["create"], batch_size, push_type="create", message="Created")
+            _micro_batch_push(
+                client,
+                categorized_assets["create"],
+                batch_size,
+                push_type="create",
+                message="Created",
+                max_retries=max_retries,
+                retry_delay=retry_delay,
+            )
 
         if categorized_assets["update"]:
             _micro_batch_push(
                 client,
                 categorized_assets["update"],
                 batch_size,
                 message="Updated",
+                max_retries=max_retries,
+                retry_delay=retry_delay,
             )
 
         if categorized_assets["resurrect"]:
             _micro_batch_push(
                 client,
                 categorized_assets["resurrect"],
                 batch_size,
                 message="Resurrected",
+                max_retries=max_retries,
+                retry_delay=retry_delay,
             )
 
         if categorized_assets["decommission"]:
             _micro_batch_push(
                 client,
                 categorized_assets["decommission"],
                 batch_size,
                 message="Decommissioned",
+                max_retries=max_retries,
+                retry_delay=retry_delay,
             )
 
     else:
         logging.info("Batch size not set, pushing all assets to CDF in one go!")
-        if categorized_assets["create"]:
-            client.assets.create_hierarchy(categorized_assets["create"])
 
-        if categorized_assets["update"]:
-            client.assets.create_hierarchy(categorized_assets["update"], upsert=True, upsert_mode="replace")
+        @retry_decorator(max_retries=max_retries, retry_delay=retry_delay, component_name="create-assets")
+        def create_assets():
+            if categorized_assets["create"]:
+                client.assets.create_hierarchy(categorized_assets["create"])
 
-        if categorized_assets["resurrect"]:
-            client.assets.create_hierarchy(categorized_assets["resurrect"], upsert=True, upsert_mode="replace")
+            if categorized_assets["update"]:
+                client.assets.create_hierarchy(categorized_assets["update"], upsert=True, upsert_mode="replace")
 
-        if categorized_assets["decommission"]:
-            client.assets.create_hierarchy(categorized_assets["decommission"], upsert=True, upsert_mode="replace")
+            if categorized_assets["resurrect"]:
+                client.assets.create_hierarchy(categorized_assets["resurrect"], upsert=True, upsert_mode="replace")
+
+            if categorized_assets["decommission"]:
+                client.assets.create_hierarchy(categorized_assets["decommission"], upsert=True, upsert_mode="replace")
+
+        create_assets()
```

### Comparing `cognite_neat-0.12.0/cognite/neat/core/extractors/rdf_to_relationships.py` & `cognite_neat-0.12.1/cognite/neat/core/extractors/rdf_to_relationships.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pandas as pd
 from cognite.client import CogniteClient
 from cognite.client.data_classes import LabelFilter, Relationship, RelationshipUpdate
 
 from cognite.neat.core.data_classes.transformation_rules import TransformationRules
 from cognite.neat.core.extractors.rdf_to_assets import _categorize_cdf_assets
 from cognite.neat.core.loader.graph_store import NeatGraphStore
-from cognite.neat.core.utils import chunker, datetime_utc_now, epoch_now_ms, remove_namespace
+from cognite.neat.core.utils import chunker, datetime_utc_now, epoch_now_ms, remove_namespace, retry_decorator
 
 # should be renamed to rdf2relationship_data_frame -> rdf2relationships
 
 
 def rdf2relationships(
     graph_store: NeatGraphStore,
     transformation_rules: TransformationRules,
@@ -330,14 +330,16 @@
 
 def _micro_batch_push(
     client: CogniteClient,
     relationships: list,
     batch_size: int = 1000,
     push_type: str = "update",
     message: str = "Updated",
+    max_retries: int = 1,
+    retry_delay: int = 5,
 ):
     """Updates assets in batches of 1000
 
     Parameters
     ----------
     client : CogniteClient
         Instance of CogniteClient
@@ -348,37 +350,43 @@
     push_type : str, optional
         Type of push, either "update" or "create", by default "update"
     message : str, optional
         Message to logged, by default "Updated"
     """
     total = len(relationships)
     counter = 0
+    if push_type not in ["update", "create"]:
+        logging.info(f"push_type {push_type} not supported")
+        raise ValueError(f"push_type {push_type} not supported")
 
     for batch in chunker(relationships, batch_size):
         counter += len(batch)
         start_time = datetime_utc_now()
-        if push_type == "update":
-            client.relationships.update(batch)
-        elif push_type == "create":
-            client.relationships.create(batch)
-        else:
-            logging.info(f"push_type {push_type} not supported")
-            raise ValueError(f"push_type {push_type} not supported")
 
+        @retry_decorator(max_retries=max_retries, retry_delay=retry_delay, component_name="microbatch-relationships")
+        def update_relationships(batch):
+            if push_type == "update":
+                client.relationships.update(batch)
+            elif push_type == "create":
+                client.relationships.create(batch)
+
+        update_relationships(batch)
         delta_time = (datetime_utc_now() - start_time).seconds
 
         msg = f"{message} {counter} of {total} relationships, batch processing time: {delta_time:.2f} "
         msg += f"seconds ETC: {delta_time * (total - counter) / (60*batch_size) :.2f} minutes"
         logging.info(msg)
 
 
 def upload_relationships(
     client: CogniteClient,
     categorized_relationships: Dict[str, list[Union[Relationship, RelationshipUpdate]]],
     batch_size: int = 5000,
+    max_retries: int = 1,
+    retry_delay: int = 3,
 ):
     """Uploads categorized relationships to CDF
 
     Parameters
     ----------
     client : CogniteClient
         Instance of CogniteClient
@@ -387,36 +395,51 @@
     batch_size : int, optional
         Size of batch, by default 5000
     """
     if batch_size:
         logging.info(f"Uploading relationships in batches of {batch_size}")
         if categorized_relationships["create"]:
             _micro_batch_push(
-                client, categorized_relationships["create"], batch_size, push_type="create", message="Created"
+                client,
+                categorized_relationships["create"],
+                batch_size,
+                push_type="create",
+                message="Created",
+                max_retries=max_retries,
+                retry_delay=retry_delay,
             )
 
         if categorized_relationships["resurrect"]:
             _micro_batch_push(
                 client,
                 categorized_relationships["resurrect"],
                 batch_size,
                 message="Resurrected",
+                max_retries=max_retries,
+                retry_delay=retry_delay,
             )
 
         if categorized_relationships["decommission"]:
             _micro_batch_push(
                 client,
                 categorized_relationships["decommission"],
                 batch_size,
                 message="Decommissioned",
+                max_retries=max_retries,
+                retry_delay=retry_delay,
             )
 
     else:
         logging.info("Batch size not set, pushing all relationships to CDF in one go!")
-        if categorized_relationships["create"]:
-            client.relationships.create(categorized_relationships["create"])
 
-        if categorized_relationships["resurrect"]:
-            client.relationships.update(categorized_relationships["resurrect"])
+        @retry_decorator(max_retries=max_retries, retry_delay=retry_delay, component_name="create-relationships")
+        def create_relationships():
+            if categorized_relationships["create"]:
+                client.relationships.create(categorized_relationships["create"])
 
-        if categorized_relationships["decommission"]:
-            client.relationships.update(categorized_relationships["decommission"])
+            if categorized_relationships["resurrect"]:
+                client.relationships.update(categorized_relationships["resurrect"])
+
+            if categorized_relationships["decommission"]:
+                client.relationships.update(categorized_relationships["decommission"])
+
+        create_relationships()
```

### Comparing `cognite_neat-0.12.0/cognite/neat/core/extractors/rules_to_graphql.py` & `cognite_neat-0.12.1/cognite/neat/core/extractors/rules_to_graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/loader/config.py` & `cognite_neat-0.12.1/cognite/neat/core/loader/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/loader/graph.py` & `cognite_neat-0.12.1/cognite/neat/core/loader/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/loader/graph_store.py` & `cognite_neat-0.12.1/cognite/neat/core/loader/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/loader/rules.py` & `cognite_neat-0.12.1/cognite/neat/core/loader/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/mocks/graph.py` & `cognite_neat-0.12.1/cognite/neat/core/mocks/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/modeler.py` & `cognite_neat-0.12.1/cognite/neat/core/modeler.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/parser/transformation_rules.py` & `cognite_neat-0.12.1/cognite/neat/core/parser/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/query_generator/sparql.py` & `cognite_neat-0.12.1/cognite/neat/core/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/transformer.py` & `cognite_neat-0.12.1/cognite/neat/core/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/utils.py` & `cognite_neat-0.12.1/cognite/neat/core/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+import logging
+import time
 from collections import OrderedDict
 from datetime import datetime, timezone
+from functools import wraps
 
 import pandas as pd
 from cognite.client import ClientConfig, CogniteClient
 from cognite.client.credentials import CredentialProvider, OAuthClientCredentials, OAuthInteractive
 from rdflib.term import URIRef
 
 from cognite.neat.core.data_classes.config import InteractiveClient, ServiceClient
@@ -101,7 +104,30 @@
 
 def chunker(sequence, chunk_size):
     return [sequence[i : i + chunk_size] for i in range(0, len(sequence), chunk_size)]
 
 
 def datetime_utc_now():
     return datetime.now(timezone.utc)
+
+
+def retry_decorator(max_retries=2, retry_delay=3, component_name=""):
+    def decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            for attempt in range(max_retries + 1):
+                try:
+                    logging.debug(f"Attempt {attempt + 1} of {max_retries + 1} for {component_name}")
+                    return func(*args, **kwargs)
+                except Exception as e:
+                    if attempt < max_retries:
+                        logging.error(
+                            f"Retry attempt {attempt + 1} failed for {component_name} . Retrying in {retry_delay} second(s)."
+                        )
+                        logging.error(e)
+                        time.sleep(retry_delay)
+                    else:
+                        raise e
+
+        return wrapper
+
+    return decorator
```

### Comparing `cognite_neat-0.12.0/cognite/neat/core/validator.py` & `cognite_neat-0.12.1/cognite/neat/core/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/workflow/base.py` & `cognite_neat-0.12.1/cognite/neat/core/workflow/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import yaml
 from cognite.client import ClientConfig as CogniteClientConfig
 from cognite.client import CogniteClient
 from prometheus_client import Gauge
 
 from cognite.neat.core.data_classes.config import ClientConfig, Config
 from cognite.neat.core.data_stores.metrics import NeatMetricsCollector
+from cognite.neat.core.utils import retry_decorator
 from cognite.neat.core.workflow import cdf_store
 from cognite.neat.core.workflow.model import (
     FlowMessage,
     StepExecutionStatus,
     StepType,
     WorkflowConfigItem,
     WorkflowDefinition,
@@ -224,15 +225,25 @@
                 else:
                     method_name = f"step_{step.id}"
                     if hasattr(self, method_name):
                         method = getattr(self, method_name)
                     else:
                         logging.error(f"Workflow step {step.id} has no method {method_name}")
                         raise Exception(f"Workflow step {step.id} has no method {method_name}")
-                new_flow_message = method(flow_message)
+
+                @retry_decorator(
+                    max_retries=step.max_retries,
+                    retry_delay=step.retry_delay,
+                    component_name=f"wf step runner , step.id = {step.id}",
+                )
+                def method_runner():
+                    return method(flow_message)
+
+                new_flow_message = method_runner()
+
             elif step.stype == StepType.START_WORKFLOW_TASK_STEP:
                 if self.task_builder:
                     sync_str = step.params.get("sync", "false")
                     sync = sync_str.lower() == "true" or sync_str == "1"
                     new_flow_message = self.task_builder.start_workflow_task(
                         workflow_name=step.params.get("workflow_name", ""), sync=sync, flow_message=self.flow_message
                     )
```

### Comparing `cognite_neat-0.12.0/cognite/neat/core/workflow/cdf_store.py` & `cognite_neat-0.12.1/cognite/neat/core/workflow/cdf_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import time
 import zipfile
 from pathlib import Path
 from typing import Dict
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import Event, FileMetadataUpdate, LabelDefinition, LabelFilter
+from fastapi.encoders import jsonable_encoder
 from pydantic import BaseModel
 
 from cognite.neat.core.workflow.model import WorkflowFullStateReport, WorkflowState, WorkflowStepEvent
 from cognite.neat.core.workflow.utils import get_file_hash
 
 
 class NeatCdfResource(BaseModel):
@@ -324,15 +325,16 @@
             "run_id": report.run_id,
             "elapsed_time": report.elapsed_time,
             "error": report.last_error,
             "execution_log": "",
             "workflow_name": report.workflow_name,
         }
         external_id = f"neat-wf-run-{report.run_id}"
-        serialized_execution_log = json.dumps([step.dict() for step in report.execution_log])
+        # serialized_execution_log = json.dumps([step.dict() for step in report.execution_log])
+        serialized_execution_log = json.dumps(jsonable_encoder(report.execution_log))
         execution_log_size = bytes(serialized_execution_log, "utf-8").__sizeof__()
         logging.debug(f"Serialized execution log size: {execution_log_size}")
         # logging.debug(f"Serialized execution log: {serialized_execution_log}")
 
         if report.start_time:
             report.start_time = report.start_time * 1000
         if report.end_time:
```

### Comparing `cognite_neat-0.12.0/cognite/neat/core/workflow/manager.py` & `cognite_neat-0.12.1/cognite/neat/core/workflow/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/workflow/model.py` & `cognite_neat-0.12.1/cognite/neat/core/workflow/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,16 @@
     method: str = None
     enabled: bool = True
     system_component_id: str = None
     trigger: bool = False
     transition_to: list[str] = None
     ui_config: UIConfig = UIConfig()
     params: dict[str, str] = None
+    max_retries: int = 0
+    retry_delay: int = 3
 
 
 class WorkflowSystemComponent(BaseModel):
     # Container for steps
     id: str
     label: str
     transition_to: list[str] = None
```

### Comparing `cognite_neat-0.12.0/cognite/neat/core/workflow/tasks.py` & `cognite_neat-0.12.1/cognite/neat/core/workflow/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/core/workflow/triggers.py` & `cognite_neat-0.12.1/cognite/neat/core/workflow/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.12.1/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.12.1/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.12.1/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/examples/workflows/basic/workflow.py` & `cognite_neat-0.12.1/cognite/neat/examples/workflows/basic/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/examples/workflows/basic/workflow.yaml` & `cognite_neat-0.12.1/cognite/neat/examples/workflows/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/examples/workflows/default/workflow.py` & `cognite_neat-0.12.1/cognite/neat/examples/workflows/default/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
         return FlowMessage(output_text=msg)
 
     def step_upload_cdf_assets(self, flow_msg: FlowMessage = None):
         if not self.cdf_client:
             logging.error("No CDF client available")
             raise Exception("No CDF client available")
 
-        upload_assets(self.cdf_client, self.categorized_assets)
+        upload_assets(self.cdf_client, self.categorized_assets, max_retries=2, retry_delay=4)
         for _ in range(1000):
             total_assets_after = self.cdf_client.assets.aggregate(
                 filter=AssetFilter(data_set_ids=[{"id": self.dataset_id}])
             )[0]["count"]
             if total_assets_after >= self.count_create_assets:
                 break
             logging.info(f"Waiting for assets to be created, current count {total_assets_after}")
@@ -300,12 +300,12 @@
         return FlowMessage(output_text=msg)
 
     def step_upload_cdf_relationships(self, flow_msg: FlowMessage = None):
         if not self.cdf_client:
             logging.error("No CDF client available")
             raise Exception("No CDF client available")
 
-        upload_relationships(self.cdf_client, self.categorized_relationships)
+        upload_relationships(self.cdf_client, self.categorized_relationships, max_retries=2, retry_delay=4)
 
     def step_cleanup(self, flow_msg: FlowMessage):
         self.categorized_assets = None
         self.categorized_relationships = None
```

### Comparing `cognite_neat-0.12.0/cognite/neat/examples/workflows/default/workflow.yaml` & `cognite_neat-0.12.1/cognite/neat/examples/workflows/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/examples/workflows/fast_graph/workflow.py` & `cognite_neat-0.12.1/cognite/neat/examples/workflows/fast_graph/workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -213,15 +213,17 @@
         elif orphan_assets:
             msg = f"Not able to fix orphans: {', '.join(orphan_assets)}"
             logging.error(msg)
             raise Exception(msg)
         else:
             logging.info("No circular dependency among assets found, your assets hierarchy look healthy !")
 
-        self.categorized_assets = categorize_assets(self.cdf_client, rdf_asset_dicts, self.dataset_id)
+        self.categorized_assets, report = categorize_assets(
+            self.cdf_client, rdf_asset_dicts, self.dataset_id, return_report=True
+        )
 
         count_create_assets = len(self.categorized_assets["create"])
         count_update_assets = len(self.categorized_assets["update"])
         count_decommission_assets = len(self.categorized_assets["decommission"])
         count_resurrect_assets = len(self.categorized_assets["resurrect"])
 
         prom_cdf_resource_stats.labels(resource_type="asset", state="create").set(count_create_assets)
@@ -236,23 +238,34 @@
         logging.info(f"Total count of assets to be decommission: { count_decommission_assets }")
         logging.info(f"Total count of assets to be resurrect: { count_resurrect_assets }")
 
         msg = f"Total count of assets { len(rdf_asset_dicts) } of which: { count_create_assets } to be created"
         msg += f", { count_update_assets } to be updated"
         msg += f", { count_decommission_assets } to be decommissioned"
         msg += f", { count_resurrect_assets } to be resurrected"
-
-        return FlowMessage(output_text=msg)
+        number_of_updates = len(report["decommission"])
+        logging.info(f"Total number of updates: {number_of_updates}")
+        if number_of_updates > int(self.get_config_item_value("update_upproval_threshold", 1000)):
+            return FlowMessage(
+                output_text=f"Very high number of updates({number_of_updates}) requeres manual approval",
+                payload=report,
+                next_step_ids=["asset_update_approval"],
+            )
+        return FlowMessage(output_text=msg, next_step_ids=["upload_cdf_assets"])
 
     def step_upload_cdf_assets(self, flow_msg: FlowMessage = None):
+        if flow_msg and flow_msg.payload and "action" in flow_msg.payload:
+            if flow_msg.payload["action"] != "approve":
+                raise Exception("Update not approved")
+
         if not self.cdf_client:
             logging.error("No CDF client available")
             raise Exception("No CDF client available")
 
-        upload_assets(self.cdf_client, self.categorized_assets)
+        upload_assets(self.cdf_client, self.categorized_assets, max_retries=2, retry_delay=4)
         for _ in range(1000):
             total_assets_after = self.cdf_client.assets.aggregate(
                 filter=AssetFilter(data_set_ids=[{"id": self.dataset_id}])
             )[0]["count"]
             if total_assets_after >= self.count_create_assets:
                 break
             logging.info(f"Waiting for assets to be created, current count {total_assets_after}")
@@ -300,12 +313,12 @@
         return FlowMessage(output_text=msg)
 
     def step_upload_cdf_relationships(self, flow_msg: FlowMessage = None):
         if not self.cdf_client:
             logging.error("No CDF client available")
             raise Exception("No CDF client available")
 
-        upload_relationships(self.cdf_client, self.categorized_relationships)
+        upload_relationships(self.cdf_client, self.categorized_relationships, max_retries=2, retry_delay=4)
 
     def step_cleanup(self, flow_msg: FlowMessage):
         self.categorized_assets = None
         self.categorized_relationships = None
```

### Comparing `cognite_neat-0.12.0/cognite/neat/examples/workflows/fast_graph/workflow.yaml` & `cognite_neat-0.12.1/cognite/neat/examples/workflows/fast_graph/workflow.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -58,14 +58,21 @@
 -   group: system
     label: null
     name: system.execution_reporting_type
     options: null
     required: false
     type: null
     value: all_disabled
+-   group: safety
+    label: null
+    name: update_upproval_threshold
+    options: null
+    required: false
+    type: null
+    value: '10'
 description: null
 system_components:
 -   description: null
     id: grid_management_system
     label: Grid management system
     transition_to:
     - rdf_xml_file
@@ -158,173 +165,214 @@
         pos_x: 347
         pos_y: 586
 implementation_module: null
 name: fast_graph
 steps:
 -   description: null
     enabled: true
-    group_id: null
     id: load_transformation_rules
     label: Loading transformation rules
+    max_retries: 0
     method: null
     params: null
+    retry_delay: 3
     stype: pystep
+    system_component_id: null
     transition_to:
     - configuring_stores
     trigger: false
     ui_config:
         pos_x: 123
         pos_y: 123
 -   description: null
     enabled: true
-    group_id: null
     id: configuring_stores
     label: Configuring graph stores
+    max_retries: 0
     method: null
     params: null
+    retry_delay: 3
     stype: pystep
+    system_component_id: null
     transition_to:
     - load_source_graph
     trigger: false
     ui_config:
         pos_x: 120
         pos_y: 229
 -   description: null
     enabled: true
-    group_id: null
     id: load_source_graph
     label: Loading source graph
+    max_retries: 0
     method: null
     params: null
+    retry_delay: 3
     stype: pystep
+    system_component_id: null
     transition_to:
     - run_transformation
     trigger: false
     ui_config:
         pos_x: 121
         pos_y: 315
 -   description: null
     enabled: true
-    group_id: null
     id: run_transformation
     label: Run transformation
+    max_retries: 0
     method: null
     params: null
+    retry_delay: 3
     stype: pystep
+    system_component_id: null
     transition_to:
     - create_cdf_labels
     trigger: false
     ui_config:
         pos_x: 121
         pos_y: 384
 -   description: null
     enabled: true
-    group_id: null
     id: prepare_cdf_assets
     label: Preparing CDF assets
+    max_retries: 0
     method: null
     params: null
+    retry_delay: 3
     stype: pystep
+    system_component_id: null
     transition_to:
     - upload_cdf_assets
+    - asset_update_approval
     trigger: false
     ui_config:
         pos_x: 119
         pos_y: 574
 -   description: null
     enabled: true
-    group_id: null
     id: upload_cdf_assets
     label: Uploading CDF assets to CDF
+    max_retries: 0
     method: null
     params: null
+    retry_delay: 5
     stype: pystep
+    system_component_id: null
     transition_to:
     - prepare_cdf_relationships
     trigger: false
     ui_config:
-        pos_x: 117
-        pos_y: 662
+        pos_x: 114
+        pos_y: 681
 -   description: null
     enabled: true
-    group_id: null
     id: prepare_cdf_relationships
     label: Preparing CDF relationships
+    max_retries: 0
     method: null
     params: null
+    retry_delay: 3
     stype: pystep
+    system_component_id: null
     transition_to:
     - upload_cdf_relationships
     trigger: false
     ui_config:
         pos_x: 115
         pos_y: 768
 -   description: Uploading CDF relationships to CDF
     enabled: true
-    group_id: null
     id: upload_cdf_relationships
     label: Uploading CDF relationships to CDF
+    max_retries: 0
     method: null
     params: null
+    retry_delay: 3
     stype: pystep
+    system_component_id: null
     transition_to: []
     trigger: false
     ui_config:
         pos_x: 114
         pos_y: 874
 -   description: Upload CDF labels
     enabled: true
-    group_id: null
     id: create_cdf_labels
     label: Upload CDF labels
+    max_retries: 0
     method: null
     params: {}
+    retry_delay: 3
     stype: pystep
+    system_component_id: null
     transition_to:
     - prepare_cdf_assets
     trigger: false
     ui_config:
         pos_x: 118
         pos_y: 483
 -   description: null
     enabled: true
-    group_id: null
     id: cleanup
     label: Cleanup
+    max_retries: 0
     method: null
     params: null
+    retry_delay: 3
     stype: pystep
+    system_component_id: null
     transition_to: []
     trigger: false
     ui_config:
         pos_x: 112
         pos_y: 993
 -   description: null
     enabled: true
-    group_id: null
     id: http_trigger
     label: Http trigger
+    max_retries: 0
     method: null
     params:
         interval: every 2 minutes
+    retry_delay: 3
     stype: http_trigger
+    system_component_id: null
     transition_to:
     - load_transformation_rules
     trigger: true
     ui_config:
         pos_x: 124
         pos_y: 32
 -   description: null
     enabled: false
-    group_id: null
     id: step_time_trigger
     label: Time trigger
+    max_retries: 0
     method: null
     params:
         interval: every 2 minutes
+    retry_delay: 3
     stype: time_trigger
+    system_component_id: null
     transition_to:
     - load_transformation_rules
     trigger: true
     ui_config:
         pos_x: 321
         pos_y: 31
+-   description: null
+    enabled: true
+    id: asset_update_approval
+    label: Asset update approval
+    max_retries: 0
+    method: null
+    params: {}
+    retry_delay: 3
+    stype: wait_for_event
+    system_component_id: null
+    transition_to:
+    - upload_cdf_assets
+    trigger: false
+    ui_config:
+        pos_x: 313
+        pos_y: 634
```

### Comparing `cognite_neat-0.12.0/cognite/neat/examples/workflows/graph_db_import/workflow.py` & `cognite_neat-0.12.1/cognite/neat/examples/workflows/graph_db_import/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/examples/workflows/graph_db_import/workflow.yaml` & `cognite_neat-0.12.1/cognite/neat/examples/workflows/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/examples/workflows/sheet2cdf/workflow.py` & `cognite_neat-0.12.1/cognite/neat/examples/workflows/sheet2cdf/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml` & `cognite_neat-0.12.1/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/explorer/data_classes/rest.py` & `cognite_neat-0.12.1/cognite/neat/explorer/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/explorer/explorer.py` & `cognite_neat-0.12.1/cognite/neat/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/explorer/utils/query_templates.py` & `cognite_neat-0.12.1/cognite/neat/explorer/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/README.md` & `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/favicon.ico` & `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/index.html` & `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="./favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="NEAT controll panel"/><link rel="apple-touch-icon" href="./logo192.png"/><link rel="manifest" href="./manifest.json"/><title>React App</title><script defer="defer" src="./static/js/main.31582da0.js"></script><link href="./static/css/main.38a62222.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="./favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="NEAT controll panel"/><link rel="apple-touch-icon" href="./logo192.png"/><link rel="manifest" href="./manifest.json"/><title>React App</title><script defer="defer" src="./static/js/main.e4f085cf.js"></script><link href="./static/css/main.38a62222.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/logo192.png` & `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.31582da0.js` & `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.31582da0.js.LICENSE.txt */ ! function() {
+/*! For license information please see main.e4f085cf.js.LICENSE.txt */ ! function() {
     var e = {
             3361: function(e, t, n) {
                 "use strict";
                 n.d(t, {
                     Z: function() {
                         return oe
                     }
@@ -31924,15 +31924,15 @@
             var Rd = _d((function e() {
                     Pd(this, e), this.pos_x = 0, this.pos_y = 0
                 })),
                 jd = _d((function e() {
                     Pd(this, e), this.name = void 0, this.value = void 0, this.label = void 0, this.type = void 0, this.required = !1, this.options = void 0, this.group = void 0
                 })),
                 Id = _d((function e() {
-                    Pd(this, e), this.id = void 0, this.label = void 0, this.stype = void 0, this.description = void 0, this.method = void 0, this.enabled = !0, this.system_component_id = void 0, this.trigger = !1, this.transition_to = void 0, this.params = {}, this.ui_config = new Rd
+                    Pd(this, e), this.id = void 0, this.label = void 0, this.stype = void 0, this.description = void 0, this.method = void 0, this.enabled = !0, this.system_component_id = void 0, this.trigger = !1, this.max_retries = 0, this.retry_delay = 3, this.transition_to = void 0, this.params = {}, this.ui_config = new Rd
                 })),
                 Td = _d((function e() {
                     Pd(this, e), this.id = void 0, this.label = void 0, this.transition_to = void 0, this.description = void 0, this.ui_config = new Rd
                 })),
                 Ld = function() {
                     function e() {
                         Pd(this, e), this.name = void 0, this.description = void 0, this.steps = void 0, this.system_components = void 0, this.configs = void 0
@@ -57508,15 +57508,15 @@
                     r = (0, o.Z)(n, 2),
                     i = r[0],
                     a = r[1],
                     l = (0, e.useState)(""),
                     u = (0, o.Z)(l, 2),
                     s = u[0],
                     c = u[1],
-                    d = t + "/data/rules/" + i.file_name;
+                    d = t + "/data/rules/" + i.file_name + "?version=" + i.hash;
                 (0, e.useEffect)((function() {
                     f("", "")
                 }), []);
                 var f = function(e, n) {
                         var r = Nn(),
                             o = t + "/api/rules?" + new URLSearchParams({
                                 workflow_name: r,
@@ -60012,15 +60012,15 @@
                     open: i,
                     onClose: g,
                     children: [(0, E.jsx)(Jv, {
                         children: "Step configurator"
                     }), (0, E.jsx)(Xv, {
                         children: (0, E.jsxs)(Wd, {
                             sx: {
-                                width: 300
+                                width: 500
                             },
                             children: [(0, E.jsx)(fg, {
                                 sx: {
                                     marginTop: 1
                                 },
                                 id: "step-config-id",
                                 fullWidth: !0,
@@ -60131,19 +60131,48 @@
                                 control: (0, E.jsx)(xE, {
                                     checked: null === s || void 0 === s ? void 0 : s.trigger,
                                     onChange: function(e) {
                                         m("trigger", e.target.checked)
                                     }
                                 }),
                                 label: "Is trigger"
+                            }), (0, E.jsx)(fg, {
+                                sx: {
+                                    marginTop: 1
+                                },
+                                id: "step-config-max-retries",
+                                fullWidth: !0,
+                                label: "Max retries on failure",
+                                size: "small",
+                                type: "number",
+                                variant: "outlined",
+                                value: null === s || void 0 === s ? void 0 : s.max_retries,
+                                onChange: function(e) {
+                                    m("max_retries", e.target.value)
+                                }
+                            }), (0, E.jsx)(fg, {
+                                sx: {
+                                    marginTop: 1
+                                },
+                                id: "step-config-retry-delay",
+                                fullWidth: !0,
+                                label: "Retry delay",
+                                size: "small",
+                                variant: "outlined",
+                                type: "number",
+                                value: null === s || void 0 === s ? void 0 : s.retry_delay,
+                                onChange: function(e) {
+                                    m("retry_delay", e.target.value)
+                                }
                             }), ("http_trigger" == (null === s || void 0 === s ? void 0 : s.stype) || "wait_for_event" == (null === s || void 0 === s ? void 0 : s.stype)) && (0, E.jsx)(fg, {
                                 sx: {
                                     marginTop: 1
                                 },
                                 value: h,
+                                label: "Run payload",
                                 onChange: function(e) {
                                     return v(e.target.value)
                                 },
                                 id: "run_payload",
                                 children: " "
                             })]
                         })
@@ -60254,15 +60283,15 @@
                     ee = J[0],
                     te = J[1],
                     ne = (0, e.useState)(""),
                     re = (0, o.Z)(ne, 2),
                     oe = re[0],
                     ie = re[1];
                 (0, e.useEffect)((function() {
-                    ue(), se(Nn()), le()
+                    ue(), se(Nn()), le(R)
                 }), []);
                 var ae = function() {
                     var e = Gn(Hn().mark((function e() {
                         var n, r, o;
                         return Hn().wrap((function(e) {
                             for (;;) switch (e.prev = e.next) {
                                 case 0:
@@ -60288,21 +60317,20 @@
                     return function() {
                         return e.apply(this, arguments)
                     }
                 }();
                 (0, e.useEffect)((function() {
                     console.log("workflow definition changed"), fe(A)
                 }), [Z]);
-                var le = function() {
-                        if (!x) {
-                            var e = setInterval((function() {
-                                ce()
-                            }), 2e3);
-                            C(e)
-                        }
+                var le = function(e) {
+                        x && clearInterval(x);
+                        var t = setInterval((function() {
+                            ce(e)
+                        }), 2e3);
+                        C(t)
                     },
                     ue = function() {
                         fetch(t + "/api/workflow/workflows").then((function(e) {
                             return e.json()
                         })).then((function(e) {
                             N(e.workflows)
                         })).catch((function(e) {
@@ -60438,15 +60466,15 @@
                                 labelId: "workflowSelectorLabel",
                                 id: "workflowSelector",
                                 value: R,
                                 size: "small",
                                 label: "Query template",
                                 onChange: function(e) {
                                     var t;
-                                    console.dir("Workflow changed to :" + e.target.value), t = e.target.value, localStorage.setItem("selectedWorkflowName", t), j(e.target.value), se(e.target.value), z("system"), fe("system")
+                                    console.dir("Workflow changed to :" + e.target.value), t = e.target.value, localStorage.setItem("selectedWorkflowName", t), j(e.target.value), se(e.target.value), z("system"), fe("system"), le(e.target.value)
                                 },
                                 children: L && L.map((function(e, t) {
                                     return (0, E.jsxs)(gv, {
                                         value: e,
                                         children: [e, " "]
                                     }, e)
                                 }))
@@ -60555,15 +60583,15 @@
                                             body: JSON.stringify(e),
                                             headers: {
                                                 "Content-Type": "application/json;charset=utf-8"
                                             }
                                         }).then((function(e) {
                                             return e.json()
                                         })).then((function(e) {
-                                            console.dir(e), y(e), le(), ce()
+                                            console.dir(e), y(e), le(R), ce()
                                         })).catch((function(e) {
                                             console.error("Error:", e)
                                         }))
                                     },
                                     sx: {
                                         marginTop: 2,
                                         marginRight: 1
@@ -61409,22 +61437,28 @@
                     }), []), r ? (0, E.jsxs)("div", {
                         children: [(0, E.jsxs)(Mn, {
                             variant: "h5",
                             children: ["NEAT Version: ", r.version]
                         }), (0, E.jsxs)(Mn, {
                             variant: "h6",
                             children: ["Docs URL: ", (0, E.jsx)("a", {
-                                href: "https://thisisneat.io/index.html",
-                                children: "https://thisisneat.io/index.html"
+                                href: "https://thisisneat.io",
+                                children: "https://thisisneat.io"
+                            })]
+                        }), (0, E.jsxs)(Mn, {
+                            variant: "h6",
+                            children: ["Docs URL: ", (0, E.jsx)("a", {
+                                href: "https://cognite-neat.readthedocs-hosted.com/en/latest/",
+                                children: "https://cognite-neat.readthedocs-hosted.com/en/latest/"
                             })]
                         }), (0, E.jsxs)(Mn, {
                             variant: "h6",
                             children: ["Github: ", (0, E.jsx)("a", {
                                 href: "https://github.com/cognitedata/neat",
-                                children: "hhttps://github.com/cognitedata/neat"
+                                children: "https://github.com/cognitedata/neat"
                             })]
                         }), (0, E.jsxs)(Mn, {
                             variant: "h6",
                             children: ["Issues tracker (Github): ", (0, E.jsx)("a", {
                                 href: "https://github.com/cognitedata/neat/issues",
                                 children: " https://github.com/cognitedata/neat/issues "
                             })]
@@ -61608,8 +61642,8 @@
                 })
             };
             r.createRoot(document.getElementById("root")).render((0, E.jsxs)(e.Fragment, {
                 children: [(0, E.jsx)(aO, {}), (0, E.jsx)(rO, {})]
             }))
         }()
 }();
-//# sourceMappingURL=main.31582da0.js.map
+//# sourceMappingURL=main.e4f085cf.js.map
```

### Comparing `cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.31582da0.js.LICENSE.txt` & `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.31582da0.js.map` & `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8563449011060839%*

 * *Differences: {"'file'": "'static/js/main.e4f085cf.js'",*

 * * "'mappings'": "';sFAqDA,IAAIA,EAA0B,WAE5B,SAASA,EAAWC,GAClB,IAAIC,EAAQC,KAEZA,KAAKC,WAAa,SAAUC,GAC1B,IAAIC,EAIAA,EAFsB,IAAtBJ,EAAMK,KAAKC,OACTN,EAAMO,eACCP,EAAMO,eAAeC,YACrBR,EAAMS,QACNT,EAAMU,UAAUC,WAEhBX,EAAMI,OAGRJ,EAAMK,KAAKL,EAAMK,KAAKC,OAAS,GAAGE,YAG7CR,EAAMU,UAAUE,aAAaT,EAAKC,GAElCJ,EAAMK,KAAKQ,KAAKV,EAClB,EAEAF,KAAKa,cAA8BC,IAAnBhB,EAAQiB,QAA+DjB,EAAQiB,OAC/Ff,KAAKI,KAAO,GACZJ,KAAKgB,IAAM,EACXhB,KAAKiB,MAAQnB,EAAQmB,MAErBjB,KAAKkB,IAAMpB,EAAQoB,IACnBlB,KAA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.31582da0.js",
+    "file": "static/js/main.e4f085cf.js",
     "names": [
         "StyleSheet",
         "options",
         "_this",
         "this",
         "_insertTag",
         "tag",
@@ -6251,14 +6251,16 @@
         "pos_x",
         "pos_y",
         "WorkflowConfigItem",
         "WorkflowStepDefinition",
         "stype",
         "system_component_id",
         "trigger",
+        "max_retries",
+        "retry_delay",
         "transition_to",
         "ui_config",
         "WorkflowSystemComponent",
         "WorkflowDefinition",
         "steps",
         "system_components",
         "configs",
@@ -10688,14 +10690,15 @@
         "loadListOfWorkflows",
         "loadWorkflowDefinitions",
         "startStatePolling",
         "fetchFileContent",
         "myHeaders",
         "Headers",
         "syncWorkflowDefToNodesAndEdges",
+        "newTimerInterval",
         "loadWorkflowStats",
         "workflows",
         "syncNodesAndEdgesToWorkflowDef",
         "updateSystemComponentTransitions",
         "updateStepTransitions",
         "convertStepsToNodes",
         "convertStepsToEdges",
@@ -12108,15 +12111,15 @@
         "import { jsx, jsxs } from 'react/jsx-runtime';\nimport { memo, useRef } from 'react';\nimport cc from 'classcat';\nimport { useStore } from '@reactflow/core';\nimport shallow from 'zustand/shallow';\n\nvar BackgroundVariant;\r\n(function (BackgroundVariant) {\r\n    BackgroundVariant[\"Lines\"] = \"lines\";\r\n    BackgroundVariant[\"Dots\"] = \"dots\";\r\n    BackgroundVariant[\"Cross\"] = \"cross\";\r\n})(BackgroundVariant || (BackgroundVariant = {}));\n\nfunction LinePattern({ color, dimensions, lineWidth, }) {\r\n    return (jsx(\"path\", { stroke: color, strokeWidth: lineWidth, d: `M${dimensions[0] / 2} 0 V${dimensions[1]} M0 ${dimensions[1] / 2} H${dimensions[0]}` }));\r\n}\r\nfunction DotPattern({ color, radius }) {\r\n    return jsx(\"circle\", { cx: radius, cy: radius, r: radius, fill: color });\r\n}\n\nconst defaultColor = {\r\n    [BackgroundVariant.Dots]: '#91919a',\r\n    [BackgroundVariant.Lines]: '#eee',\r\n    [BackgroundVariant.Cross]: '#e2e2e2',\r\n};\r\nconst defaultSize = {\r\n    [BackgroundVariant.Dots]: 1,\r\n    [BackgroundVariant.Lines]: 1,\r\n    [BackgroundVariant.Cross]: 6,\r\n};\r\nconst selector = (s) => ({ transform: s.transform, patternId: `pattern-${s.rfId}` });\r\nfunction Background({ variant = BackgroundVariant.Dots, gap = 20, \r\n// only used for dots and cross\r\nsize, \r\n// only used for lines and cross\r\nlineWidth = 1, color, style, className, }) {\r\n    const ref = useRef(null);\r\n    const { transform, patternId } = useStore(selector, shallow);\r\n    const patternColor = color || defaultColor[variant];\r\n    const patternSize = size || defaultSize[variant];\r\n    const isDots = variant === BackgroundVariant.Dots;\r\n    const isCross = variant === BackgroundVariant.Cross;\r\n    const gapXY = Array.isArray(gap) ? gap : [gap, gap];\r\n    const scaledGap = [gapXY[0] * transform[2] || 1, gapXY[1] * transform[2] || 1];\r\n    const scaledSize = patternSize * transform[2];\r\n    const patternDimensions = isCross ? [scaledSize, scaledSize] : scaledGap;\r\n    const patternOffset = isDots\r\n        ? [scaledSize / 2, scaledSize / 2]\r\n        : [patternDimensions[0] / 2, patternDimensions[1] / 2];\r\n    return (jsxs(\"svg\", { className: cc(['react-flow__background', className]), style: {\r\n            ...style,\r\n            position: 'absolute',\r\n            width: '100%',\r\n            height: '100%',\r\n            top: 0,\r\n            left: 0,\r\n        }, ref: ref, children: [jsx(\"pattern\", { id: patternId, x: transform[0] % scaledGap[0], y: transform[1] % scaledGap[1], width: scaledGap[0], height: scaledGap[1], patternUnits: \"userSpaceOnUse\", patternTransform: `translate(-${patternOffset[0]},-${patternOffset[1]})`, children: isDots ? (jsx(DotPattern, { color: patternColor, radius: scaledSize / 2 })) : (jsx(LinePattern, { dimensions: patternDimensions, color: patternColor, lineWidth: lineWidth })) }), jsx(\"rect\", { x: \"0\", y: \"0\", width: \"100%\", height: \"100%\", fill: `url(#${patternId})` })] }));\r\n}\r\nBackground.displayName = 'Background';\r\nvar Background$1 = memo(Background);\n\nexport { Background$1 as Background, BackgroundVariant };\n",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getButtonUtilityClass(slot) {\n  return generateUtilityClass('MuiButton', slot);\n}\nconst buttonClasses = generateUtilityClasses('MuiButton', ['root', 'text', 'textInherit', 'textPrimary', 'textSecondary', 'textSuccess', 'textError', 'textInfo', 'textWarning', 'outlined', 'outlinedInherit', 'outlinedPrimary', 'outlinedSecondary', 'outlinedSuccess', 'outlinedError', 'outlinedInfo', 'outlinedWarning', 'contained', 'containedInherit', 'containedPrimary', 'containedSecondary', 'containedSuccess', 'containedError', 'containedInfo', 'containedWarning', 'disableElevation', 'focusVisible', 'disabled', 'colorInherit', 'textSizeSmall', 'textSizeMedium', 'textSizeLarge', 'outlinedSizeSmall', 'outlinedSizeMedium', 'outlinedSizeLarge', 'containedSizeSmall', 'containedSizeMedium', 'containedSizeLarge', 'sizeMedium', 'sizeSmall', 'sizeLarge', 'fullWidth', 'startIcon', 'endIcon', 'iconSizeSmall', 'iconSizeMedium', 'iconSizeLarge']);\nexport default buttonClasses;",
         "import * as React from 'react';\n/**\n * @ignore - internal component.\n */\nconst ButtonGroupContext = /*#__PURE__*/React.createContext({});\nif (process.env.NODE_ENV !== 'production') {\n  ButtonGroupContext.displayName = 'ButtonGroupContext';\n}\nexport default ButtonGroupContext;",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"children\", \"color\", \"component\", \"className\", \"disabled\", \"disableElevation\", \"disableFocusRipple\", \"endIcon\", \"focusVisibleClassName\", \"fullWidth\", \"size\", \"startIcon\", \"type\", \"variant\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { internal_resolveProps as resolveProps } from '@mui/utils';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport { alpha } from '@mui/system';\nimport styled, { rootShouldForwardProp } from '../styles/styled';\nimport useThemeProps from '../styles/useThemeProps';\nimport ButtonBase from '../ButtonBase';\nimport capitalize from '../utils/capitalize';\nimport buttonClasses, { getButtonUtilityClass } from './buttonClasses';\nimport ButtonGroupContext from '../ButtonGroup/ButtonGroupContext';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nimport { jsxs as _jsxs } from \"react/jsx-runtime\";\nconst useUtilityClasses = ownerState => {\n  const {\n    color,\n    disableElevation,\n    fullWidth,\n    size,\n    variant,\n    classes\n  } = ownerState;\n  const slots = {\n    root: ['root', variant, `${variant}${capitalize(color)}`, `size${capitalize(size)}`, `${variant}Size${capitalize(size)}`, color === 'inherit' && 'colorInherit', disableElevation && 'disableElevation', fullWidth && 'fullWidth'],\n    label: ['label'],\n    startIcon: ['startIcon', `iconSize${capitalize(size)}`],\n    endIcon: ['endIcon', `iconSize${capitalize(size)}`]\n  };\n  const composedClasses = composeClasses(slots, getButtonUtilityClass, classes);\n  return _extends({}, classes, composedClasses);\n};\nconst commonIconStyles = ownerState => _extends({}, ownerState.size === 'small' && {\n  '& > *:nth-of-type(1)': {\n    fontSize: 18\n  }\n}, ownerState.size === 'medium' && {\n  '& > *:nth-of-type(1)': {\n    fontSize: 20\n  }\n}, ownerState.size === 'large' && {\n  '& > *:nth-of-type(1)': {\n    fontSize: 22\n  }\n});\nconst ButtonRoot = styled(ButtonBase, {\n  shouldForwardProp: prop => rootShouldForwardProp(prop) || prop === 'classes',\n  name: 'MuiButton',\n  slot: 'Root',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.root, styles[ownerState.variant], styles[`${ownerState.variant}${capitalize(ownerState.color)}`], styles[`size${capitalize(ownerState.size)}`], styles[`${ownerState.variant}Size${capitalize(ownerState.size)}`], ownerState.color === 'inherit' && styles.colorInherit, ownerState.disableElevation && styles.disableElevation, ownerState.fullWidth && styles.fullWidth];\n  }\n})(({\n  theme,\n  ownerState\n}) => {\n  var _theme$palette$getCon, _theme$palette;\n  return _extends({}, theme.typography.button, {\n    minWidth: 64,\n    padding: '6px 16px',\n    borderRadius: (theme.vars || theme).shape.borderRadius,\n    transition: theme.transitions.create(['background-color', 'box-shadow', 'border-color', 'color'], {\n      duration: theme.transitions.duration.short\n    }),\n    '&:hover': _extends({\n      textDecoration: 'none',\n      backgroundColor: theme.vars ? `rgba(${theme.vars.palette.text.primaryChannel} / ${theme.vars.palette.action.hoverOpacity})` : alpha(theme.palette.text.primary, theme.palette.action.hoverOpacity),\n      // Reset on touch devices, it doesn't add specificity\n      '@media (hover: none)': {\n        backgroundColor: 'transparent'\n      }\n    }, ownerState.variant === 'text' && ownerState.color !== 'inherit' && {\n      backgroundColor: theme.vars ? `rgba(${theme.vars.palette[ownerState.color].mainChannel} / ${theme.vars.palette.action.hoverOpacity})` : alpha(theme.palette[ownerState.color].main, theme.palette.action.hoverOpacity),\n      // Reset on touch devices, it doesn't add specificity\n      '@media (hover: none)': {\n        backgroundColor: 'transparent'\n      }\n    }, ownerState.variant === 'outlined' && ownerState.color !== 'inherit' && {\n      border: `1px solid ${(theme.vars || theme).palette[ownerState.color].main}`,\n      backgroundColor: theme.vars ? `rgba(${theme.vars.palette[ownerState.color].mainChannel} / ${theme.vars.palette.action.hoverOpacity})` : alpha(theme.palette[ownerState.color].main, theme.palette.action.hoverOpacity),\n      // Reset on touch devices, it doesn't add specificity\n      '@media (hover: none)': {\n        backgroundColor: 'transparent'\n      }\n    }, ownerState.variant === 'contained' && {\n      backgroundColor: (theme.vars || theme).palette.grey.A100,\n      boxShadow: (theme.vars || theme).shadows[4],\n      // Reset on touch devices, it doesn't add specificity\n      '@media (hover: none)': {\n        boxShadow: (theme.vars || theme).shadows[2],\n        backgroundColor: (theme.vars || theme).palette.grey[300]\n      }\n    }, ownerState.variant === 'contained' && ownerState.color !== 'inherit' && {\n      backgroundColor: (theme.vars || theme).palette[ownerState.color].dark,\n      // Reset on touch devices, it doesn't add specificity\n      '@media (hover: none)': {\n        backgroundColor: (theme.vars || theme).palette[ownerState.color].main\n      }\n    }),\n    '&:active': _extends({}, ownerState.variant === 'contained' && {\n      boxShadow: (theme.vars || theme).shadows[8]\n    }),\n    [`&.${buttonClasses.focusVisible}`]: _extends({}, ownerState.variant === 'contained' && {\n      boxShadow: (theme.vars || theme).shadows[6]\n    }),\n    [`&.${buttonClasses.disabled}`]: _extends({\n      color: (theme.vars || theme).palette.action.disabled\n    }, ownerState.variant === 'outlined' && {\n      border: `1px solid ${(theme.vars || theme).palette.action.disabledBackground}`\n    }, ownerState.variant === 'contained' && {\n      color: (theme.vars || theme).palette.action.disabled,\n      boxShadow: (theme.vars || theme).shadows[0],\n      backgroundColor: (theme.vars || theme).palette.action.disabledBackground\n    })\n  }, ownerState.variant === 'text' && {\n    padding: '6px 8px'\n  }, ownerState.variant === 'text' && ownerState.color !== 'inherit' && {\n    color: (theme.vars || theme).palette[ownerState.color].main\n  }, ownerState.variant === 'outlined' && {\n    padding: '5px 15px',\n    border: '1px solid currentColor'\n  }, ownerState.variant === 'outlined' && ownerState.color !== 'inherit' && {\n    color: (theme.vars || theme).palette[ownerState.color].main,\n    border: theme.vars ? `1px solid rgba(${theme.vars.palette[ownerState.color].mainChannel} / 0.5)` : `1px solid ${alpha(theme.palette[ownerState.color].main, 0.5)}`\n  }, ownerState.variant === 'contained' && {\n    color: theme.vars ?\n    // this is safe because grey does not change between default light/dark mode\n    theme.vars.palette.text.primary : (_theme$palette$getCon = (_theme$palette = theme.palette).getContrastText) == null ? void 0 : _theme$palette$getCon.call(_theme$palette, theme.palette.grey[300]),\n    backgroundColor: (theme.vars || theme).palette.grey[300],\n    boxShadow: (theme.vars || theme).shadows[2]\n  }, ownerState.variant === 'contained' && ownerState.color !== 'inherit' && {\n    color: (theme.vars || theme).palette[ownerState.color].contrastText,\n    backgroundColor: (theme.vars || theme).palette[ownerState.color].main\n  }, ownerState.color === 'inherit' && {\n    color: 'inherit',\n    borderColor: 'currentColor'\n  }, ownerState.size === 'small' && ownerState.variant === 'text' && {\n    padding: '4px 5px',\n    fontSize: theme.typography.pxToRem(13)\n  }, ownerState.size === 'large' && ownerState.variant === 'text' && {\n    padding: '8px 11px',\n    fontSize: theme.typography.pxToRem(15)\n  }, ownerState.size === 'small' && ownerState.variant === 'outlined' && {\n    padding: '3px 9px',\n    fontSize: theme.typography.pxToRem(13)\n  }, ownerState.size === 'large' && ownerState.variant === 'outlined' && {\n    padding: '7px 21px',\n    fontSize: theme.typography.pxToRem(15)\n  }, ownerState.size === 'small' && ownerState.variant === 'contained' && {\n    padding: '4px 10px',\n    fontSize: theme.typography.pxToRem(13)\n  }, ownerState.size === 'large' && ownerState.variant === 'contained' && {\n    padding: '8px 22px',\n    fontSize: theme.typography.pxToRem(15)\n  }, ownerState.fullWidth && {\n    width: '100%'\n  });\n}, ({\n  ownerState\n}) => ownerState.disableElevation && {\n  boxShadow: 'none',\n  '&:hover': {\n    boxShadow: 'none'\n  },\n  [`&.${buttonClasses.focusVisible}`]: {\n    boxShadow: 'none'\n  },\n  '&:active': {\n    boxShadow: 'none'\n  },\n  [`&.${buttonClasses.disabled}`]: {\n    boxShadow: 'none'\n  }\n});\nconst ButtonStartIcon = styled('span', {\n  name: 'MuiButton',\n  slot: 'StartIcon',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.startIcon, styles[`iconSize${capitalize(ownerState.size)}`]];\n  }\n})(({\n  ownerState\n}) => _extends({\n  display: 'inherit',\n  marginRight: 8,\n  marginLeft: -4\n}, ownerState.size === 'small' && {\n  marginLeft: -2\n}, commonIconStyles(ownerState)));\nconst ButtonEndIcon = styled('span', {\n  name: 'MuiButton',\n  slot: 'EndIcon',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.endIcon, styles[`iconSize${capitalize(ownerState.size)}`]];\n  }\n})(({\n  ownerState\n}) => _extends({\n  display: 'inherit',\n  marginRight: -4,\n  marginLeft: 8\n}, ownerState.size === 'small' && {\n  marginRight: -2\n}, commonIconStyles(ownerState)));\nconst Button = /*#__PURE__*/React.forwardRef(function Button(inProps, ref) {\n  // props priority: `inProps` > `contextProps` > `themeDefaultProps`\n  const contextProps = React.useContext(ButtonGroupContext);\n  const resolvedProps = resolveProps(contextProps, inProps);\n  const props = useThemeProps({\n    props: resolvedProps,\n    name: 'MuiButton'\n  });\n  const {\n      children,\n      color = 'primary',\n      component = 'button',\n      className,\n      disabled = false,\n      disableElevation = false,\n      disableFocusRipple = false,\n      endIcon: endIconProp,\n      focusVisibleClassName,\n      fullWidth = false,\n      size = 'medium',\n      startIcon: startIconProp,\n      type,\n      variant = 'text'\n    } = props,\n    other = _objectWithoutPropertiesLoose(props, _excluded);\n  const ownerState = _extends({}, props, {\n    color,\n    component,\n    disabled,\n    disableElevation,\n    disableFocusRipple,\n    fullWidth,\n    size,\n    type,\n    variant\n  });\n  const classes = useUtilityClasses(ownerState);\n  const startIcon = startIconProp && /*#__PURE__*/_jsx(ButtonStartIcon, {\n    className: classes.startIcon,\n    ownerState: ownerState,\n    children: startIconProp\n  });\n  const endIcon = endIconProp && /*#__PURE__*/_jsx(ButtonEndIcon, {\n    className: classes.endIcon,\n    ownerState: ownerState,\n    children: endIconProp\n  });\n  return /*#__PURE__*/_jsxs(ButtonRoot, _extends({\n    ownerState: ownerState,\n    className: clsx(contextProps.className, classes.root, className),\n    component: component,\n    disabled: disabled,\n    focusRipple: !disableFocusRipple,\n    focusVisibleClassName: clsx(classes.focusVisible, focusVisibleClassName),\n    ref: ref,\n    type: type\n  }, other, {\n    classes: classes,\n    children: [startIcon, children, endIcon]\n  }));\n});\nprocess.env.NODE_ENV !== \"production\" ? Button.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * The content of the component.\n   */\n  children: PropTypes.node,\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n  /**\n   * The color of the component.\n   * It supports both default and custom theme colors, which can be added as shown in the\n   * [palette customization guide](https://mui.com/material-ui/customization/palette/#adding-new-colors).\n   * @default 'primary'\n   */\n  color: PropTypes /* @typescript-to-proptypes-ignore */.oneOfType([PropTypes.oneOf(['inherit', 'primary', 'secondary', 'success', 'error', 'info', 'warning']), PropTypes.string]),\n  /**\n   * The component used for the root node.\n   * Either a string to use a HTML element or a component.\n   */\n  component: PropTypes.elementType,\n  /**\n   * If `true`, the component is disabled.\n   * @default false\n   */\n  disabled: PropTypes.bool,\n  /**\n   * If `true`, no elevation is used.\n   * @default false\n   */\n  disableElevation: PropTypes.bool,\n  /**\n   * If `true`, the  keyboard focus ripple is disabled.\n   * @default false\n   */\n  disableFocusRipple: PropTypes.bool,\n  /**\n   * If `true`, the ripple effect is disabled.\n   *\n   * \u26a0\ufe0f Without a ripple there is no styling for :focus-visible by default. Be sure\n   * to highlight the element by applying separate styles with the `.Mui-focusVisible` class.\n   * @default false\n   */\n  disableRipple: PropTypes.bool,\n  /**\n   * Element placed after the children.\n   */\n  endIcon: PropTypes.node,\n  /**\n   * @ignore\n   */\n  focusVisibleClassName: PropTypes.string,\n  /**\n   * If `true`, the button will take up the full width of its container.\n   * @default false\n   */\n  fullWidth: PropTypes.bool,\n  /**\n   * The URL to link to when the button is clicked.\n   * If defined, an `a` element will be used as the root node.\n   */\n  href: PropTypes.string,\n  /**\n   * The size of the component.\n   * `small` is equivalent to the dense button styling.\n   * @default 'medium'\n   */\n  size: PropTypes /* @typescript-to-proptypes-ignore */.oneOfType([PropTypes.oneOf(['small', 'medium', 'large']), PropTypes.string]),\n  /**\n   * Element placed before the children.\n   */\n  startIcon: PropTypes.node,\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object]),\n  /**\n   * @ignore\n   */\n  type: PropTypes.oneOfType([PropTypes.oneOf(['button', 'reset', 'submit']), PropTypes.string]),\n  /**\n   * The variant to use.\n   * @default 'text'\n   */\n  variant: PropTypes /* @typescript-to-proptypes-ignore */.oneOfType([PropTypes.oneOf(['contained', 'outlined', 'text']), PropTypes.string])\n} : void 0;\nexport default Button;",
         "import createStyled from './createStyled';\nconst styled = createStyled();\nexport default styled;",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"component\", \"direction\", \"spacing\", \"divider\", \"children\", \"className\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { deepmerge, unstable_composeClasses as composeClasses, unstable_generateUtilityClass as generateUtilityClass } from '@mui/utils';\nimport systemStyled from '../styled';\nimport useThemePropsSystem from '../useThemeProps';\nimport { extendSxProp } from '../styleFunctionSx';\nimport createTheme from '../createTheme';\nimport { handleBreakpoints, mergeBreakpointsInOrder, resolveBreakpointValues } from '../breakpoints';\nimport { createUnarySpacing, getValue } from '../spacing';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst defaultTheme = createTheme();\n// widening Theme to any so that the consumer can own the theme structure.\nconst defaultCreateStyledComponent = systemStyled('div', {\n  name: 'MuiStack',\n  slot: 'Root',\n  overridesResolver: (props, styles) => styles.root\n});\nfunction useThemePropsDefault(props) {\n  return useThemePropsSystem({\n    props,\n    name: 'MuiStack',\n    defaultTheme\n  });\n}\n\n/**\n * Return an array with the separator React element interspersed between\n * each React node of the input children.\n *\n * > joinChildren([1,2,3], 0)\n * [1,0,2,0,3]\n */\nfunction joinChildren(children, separator) {\n  const childrenArray = React.Children.toArray(children).filter(Boolean);\n  return childrenArray.reduce((output, child, index) => {\n    output.push(child);\n    if (index < childrenArray.length - 1) {\n      output.push( /*#__PURE__*/React.cloneElement(separator, {\n        key: `separator-${index}`\n      }));\n    }\n    return output;\n  }, []);\n}\nconst getSideFromDirection = direction => {\n  return {\n    row: 'Left',\n    'row-reverse': 'Right',\n    column: 'Top',\n    'column-reverse': 'Bottom'\n  }[direction];\n};\nexport const style = ({\n  ownerState,\n  theme\n}) => {\n  let styles = _extends({\n    display: 'flex',\n    flexDirection: 'column'\n  }, handleBreakpoints({\n    theme\n  }, resolveBreakpointValues({\n    values: ownerState.direction,\n    breakpoints: theme.breakpoints.values\n  }), propValue => ({\n    flexDirection: propValue\n  })));\n  if (ownerState.spacing) {\n    const transformer = createUnarySpacing(theme);\n    const base = Object.keys(theme.breakpoints.values).reduce((acc, breakpoint) => {\n      if (typeof ownerState.spacing === 'object' && ownerState.spacing[breakpoint] != null || typeof ownerState.direction === 'object' && ownerState.direction[breakpoint] != null) {\n        acc[breakpoint] = true;\n      }\n      return acc;\n    }, {});\n    const directionValues = resolveBreakpointValues({\n      values: ownerState.direction,\n      base\n    });\n    const spacingValues = resolveBreakpointValues({\n      values: ownerState.spacing,\n      base\n    });\n    if (typeof directionValues === 'object') {\n      Object.keys(directionValues).forEach((breakpoint, index, breakpoints) => {\n        const directionValue = directionValues[breakpoint];\n        if (!directionValue) {\n          const previousDirectionValue = index > 0 ? directionValues[breakpoints[index - 1]] : 'column';\n          directionValues[breakpoint] = previousDirectionValue;\n        }\n      });\n    }\n    const styleFromPropValue = (propValue, breakpoint) => {\n      return {\n        '& > :not(style) + :not(style)': {\n          margin: 0,\n          [`margin${getSideFromDirection(breakpoint ? directionValues[breakpoint] : ownerState.direction)}`]: getValue(transformer, propValue)\n        }\n      };\n    };\n    styles = deepmerge(styles, handleBreakpoints({\n      theme\n    }, spacingValues, styleFromPropValue));\n  }\n  styles = mergeBreakpointsInOrder(theme.breakpoints, styles);\n  return styles;\n};\nexport default function createStack(options = {}) {\n  const {\n    // This will allow adding custom styled fn (for example for custom sx style function)\n    createStyledComponent = defaultCreateStyledComponent,\n    useThemeProps = useThemePropsDefault,\n    componentName = 'MuiStack'\n  } = options;\n  const useUtilityClasses = () => {\n    const slots = {\n      root: ['root']\n    };\n    return composeClasses(slots, slot => generateUtilityClass(componentName, slot), {});\n  };\n  const StackRoot = createStyledComponent(style);\n  const Stack = /*#__PURE__*/React.forwardRef(function Grid(inProps, ref) {\n    const themeProps = useThemeProps(inProps);\n    const props = extendSxProp(themeProps); // `color` type conflicts with html color attribute.\n    const {\n        component = 'div',\n        direction = 'column',\n        spacing = 0,\n        divider,\n        children,\n        className\n      } = props,\n      other = _objectWithoutPropertiesLoose(props, _excluded);\n    const ownerState = {\n      direction,\n      spacing\n    };\n    const classes = useUtilityClasses();\n    return /*#__PURE__*/_jsx(StackRoot, _extends({\n      as: component,\n      ownerState: ownerState,\n      ref: ref,\n      className: clsx(classes.root, className)\n    }, other, {\n      children: divider ? joinChildren(children, divider) : children\n    }));\n  });\n  process.env.NODE_ENV !== \"production\" ? Stack.propTypes /* remove-proptypes */ = {\n    children: PropTypes.node,\n    direction: PropTypes.oneOfType([PropTypes.oneOf(['column-reverse', 'column', 'row-reverse', 'row']), PropTypes.arrayOf(PropTypes.oneOf(['column-reverse', 'column', 'row-reverse', 'row'])), PropTypes.object]),\n    divider: PropTypes.node,\n    spacing: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.number, PropTypes.string])), PropTypes.number, PropTypes.object, PropTypes.string]),\n    sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object])\n  } : void 0;\n  return Stack;\n}",
         "import PropTypes from 'prop-types';\nimport { createStack } from '@mui/system';\nimport styled from '../styles/styled';\nimport useThemeProps from '../styles/useThemeProps';\nconst Stack = createStack({\n  createStyledComponent: styled('div', {\n    name: 'MuiStack',\n    slot: 'Root',\n    overridesResolver: (props, styles) => styles.root\n  }),\n  useThemeProps: inProps => useThemeProps({\n    props: inProps,\n    name: 'MuiStack'\n  })\n});\nprocess.env.NODE_ENV !== \"production\" ? Stack.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * The content of the component.\n   */\n  children: PropTypes.node,\n  /**\n   * The component used for the root node.\n   * Either a string to use a HTML element or a component.\n   */\n  component: PropTypes.elementType,\n  /**\n   * Defines the `flex-direction` style property.\n   * It is applied for all screen sizes.\n   * @default 'column'\n   */\n  direction: PropTypes.oneOfType([PropTypes.oneOf(['column-reverse', 'column', 'row-reverse', 'row']), PropTypes.arrayOf(PropTypes.oneOf(['column-reverse', 'column', 'row-reverse', 'row'])), PropTypes.object]),\n  /**\n   * Add an element between each child.\n   */\n  divider: PropTypes.node,\n  /**\n   * Defines the space between immediate children.\n   * @default 0\n   */\n  spacing: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.number, PropTypes.string])), PropTypes.number, PropTypes.object, PropTypes.string]),\n  /**\n   * The system prop, which allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object])\n} : void 0;\nexport default Stack;",
-        "export enum WorkflowState {\n    CREATED = \"CREATED\",\n    RUNNING = \"RUNNING\",\n    COMPLETED = \"COMPLETED\",\n    FAILED = \"FAILED\"\n}\n\nexport enum StepExecutionStatus {\n    SUCCESS = \"COMPLETED\",\n    FAILED = \"FAILED\",\n    SKIPPED = \"SKIPPED\",\n    STARTED = \"STARTED\",\n    UNKNOWN = \"UNKNOWN\"\n}\n\nexport class UIConfig {\n    pos_x: number = 0;\n    pos_y: number = 0;\n}\n\nexport class WorkflowConfigItem {\n    name: string;\n    value: string;\n    label?: string;\n    type?: string;\n    required: boolean = false;\n    options?: string[];\n    group?: string;\n}\n\nexport class WorkflowStepDefinition {\n    id: string;\n    label?: string;\n    stype?: string;\n    description?: string;\n    method?: string;\n    enabled?: boolean = true;\n    system_component_id?: string;\n    trigger?: boolean = false;\n    transition_to?: string[];\n    params?:any = {}\n    ui_config?: UIConfig = new UIConfig();\n}\n\n\nexport class WorkflowSystemComponent {\n    id: string;\n    label: string;\n    transition_to?: string[];\n    description?: string;\n    ui_config?: UIConfig = new UIConfig();\n}\n\nexport class WorkflowDefinition {\n    name: string;\n    description?: string;\n    steps: WorkflowStepDefinition[];\n    system_components: WorkflowSystemComponent[];\n    configs?: WorkflowConfigItem[];\n    static fromJSON(json: any): WorkflowDefinition {\n        let workflow = new WorkflowDefinition();\n        Object.assign(workflow, json);\n        return workflow;\n    }\n    serializeToJson(): any {\n        let json = JSON.stringify(this);\n        return json;\n    }\n\n    toJSON() {\n        return {\n            name: this.name,\n            description: this.description,\n            configs: this.configs,\n            steps: this.steps,\n            system_components: this.system_components\n        };\n    }\n\n    upsertConfigItem(config: WorkflowConfigItem) {\n        let index = this.configs.findIndex(c => c.name == config.name);\n        if (index >= 0) {\n            this.configs[index] = config;\n        }else {\n            this.configs.push(config);\n        }\n    }\n\n    addConfigItem(config: WorkflowConfigItem) {\n        this.configs.push(config);\n    }\n\n    deleteConfigItem(name: string) {\n        let index = this.configs.findIndex(c => c.name == name);\n        if (index >= 0) {\n            this.configs.splice(index, 1);\n\n        }\n    }\n\n    getStepById(id: string): WorkflowStepDefinition {\n        let step = this.steps.find(step => step.id == id);\n        return step;\n    }\n\n    getSystemComponentById(id: string): WorkflowSystemComponent {\n        let systemComponent = this.system_components.find(systemComponent => systemComponent.id == id);\n        return systemComponent;\n    }\n\n    updateStep(id:string,step: WorkflowStepDefinition) {\n        let index = this.steps.findIndex(s => s.id == id);\n        if (index >= 0) {\n            this.steps[index] = step;\n        }\n    }\n\n    updateSystemComponent(id:string,systemComponent: WorkflowSystemComponent) {\n        let index = this.system_components.findIndex(g => g.id == id);\n        if (index >= 0) {\n            this.system_components[index] = systemComponent;\n        }\n    }\n\n    convertStepsToNodes():any {\n        let nodes = [];\n        this.steps.forEach(step => {\n            let style = {};\n            if (step.enabled == false) {\n                style = { borderColor: 'red'};\n            }\n            let node = {\n                id: step.id,\n                position: {\n                    x: step.ui_config.pos_x,\n                    y: step.ui_config.pos_y\n                },\n                data: {\n                    label: step.label\n                },\n                width: 150,\n                height: 40,\n                style : style,\n                selected: false,\n                positionAbsolute: {\n                    x: step.ui_config.pos_x,\n                    y: step.ui_config.pos_y\n                },\n                dragging: false\n            }\n            nodes.push(node);\n        });\n        return nodes;\n    }\n\n\n    convertSystemComponentsToNodes():any {\n        let nodes = [];\n        this.system_components?.forEach(step => {\n            let style = {};\n            let node = {\n                id: step.id,\n                position: {\n                    x: step.ui_config.pos_x,\n                    y: step.ui_config.pos_y\n                },\n                data: {\n                    label: step.label\n                },\n                width: 150,\n                height: 40,\n                style : style,\n                selected: false,\n                positionAbsolute: {\n                    x: step.ui_config.pos_x,\n                    y: step.ui_config.pos_y\n                },\n                dragging: false\n            }\n            nodes.push(node);\n        });\n        return nodes;\n    }\n\n    convertStepsToEdges():any {\n        let edges = [];\n        this.steps?.forEach(step => {\n            if (step.transition_to) {\n                step.transition_to.forEach(transition => {\n                    let edge = {\n                        id: step.id + \"_\" + transition,\n                        source: step.id,\n                        target: transition,\n                        animated: true,\n                        label: \"\",\n                        arrowHeadType: \"arrowclosed\"\n                    }\n                    edges.push(edge);\n                });\n            }\n        });\n        return edges;\n    }\n\n    convertSystemComponentsToEdges():any {\n        let edges = [];\n        this.system_components?.forEach(step => {\n            if (step.transition_to) {\n                step.transition_to.forEach(transition => {\n                    let edge = {\n                        id: step.id + \"_\" + transition,\n                        source: step.id,\n                        target: transition,\n                        animated: true,\n                        label: \"\",\n                        arrowHeadType: \"arrowclosed\"\n                    }\n                    edges.push(edge);\n                });\n            }\n        });\n        console.log(\"Component edges: \");\n        console.dir(edges)\n        return edges;\n    }\n\n    updatePositions(nodes:any) {\n        nodes.forEach(node => {\n            let step = this.steps.find(step => step.id == node.id);\n            if (step) {\n                step.ui_config.pos_x = node.position.x;\n                step.ui_config.pos_y = node.position.y;\n            }else {\n                let systemComponent = this.system_components.find(systemComponent => systemComponent.id == node.id);\n                if (systemComponent) {\n                    systemComponent.ui_config.pos_x = node.position.x;\n                    systemComponent.ui_config.pos_y = node.position.y;\n                }\n            }\n        });\n    }\n    // Update step transitions from edges\n    updateStepTransitions(edges:any) {\n        this.steps.forEach(step => {\n            step.transition_to = [];\n        });\n        edges.forEach(edge => {\n            let source = this.steps.find(step => step.id == edge.source);\n            if (source) {\n                source.transition_to.push(edge.target);\n            }\n        });\n    }\n    // Update systemComponent transitions from edges\n    updateSystemComponentTransitions(edges:any) {\n        this.system_components.forEach(systemComponent => {\n            systemComponent.transition_to = [];\n        });\n        edges.forEach(edge => {\n            let source = this.system_components.find(systemComponent => systemComponent.id == edge.source);\n            if (source) {\n                source.transition_to.push(edge.target);\n            }\n        });\n    }\n\n    deleteStep(id:string) {\n        let index = this.steps.findIndex(s => s.id == id);\n        if (index >= 0) {\n            this.steps.splice(index,1);\n        }\n    }\n\n    deleteSystemComponent(id:string) {\n        let index = this.system_components.findIndex(g => g.id == id);\n        if (index >= 0) {\n            this.system_components.splice(index,1);\n        }\n    }\n\n\n}\n",
+        "export enum WorkflowState {\n    CREATED = \"CREATED\",\n    RUNNING = \"RUNNING\",\n    COMPLETED = \"COMPLETED\",\n    FAILED = \"FAILED\"\n}\n\nexport enum StepExecutionStatus {\n    SUCCESS = \"COMPLETED\",\n    FAILED = \"FAILED\",\n    SKIPPED = \"SKIPPED\",\n    STARTED = \"STARTED\",\n    UNKNOWN = \"UNKNOWN\"\n}\n\nexport class UIConfig {\n    pos_x: number = 0;\n    pos_y: number = 0;\n}\n\nexport class WorkflowConfigItem {\n    name: string;\n    value: string;\n    label?: string;\n    type?: string;\n    required: boolean = false;\n    options?: string[];\n    group?: string;\n}\n\nexport class WorkflowStepDefinition {\n    id: string;\n    label?: string;\n    stype?: string;\n    description?: string;\n    method?: string;\n    enabled?: boolean = true;\n    system_component_id?: string;\n    trigger?: boolean = false;\n    max_retries?: number = 0;\n    retry_delay?: number = 3;\n    transition_to?: string[];\n    params?:any = {}\n    ui_config?: UIConfig = new UIConfig();\n}\n\n\nexport class WorkflowSystemComponent {\n    id: string;\n    label: string;\n    transition_to?: string[];\n    description?: string;\n    ui_config?: UIConfig = new UIConfig();\n}\n\nexport class WorkflowDefinition {\n    name: string;\n    description?: string;\n    steps: WorkflowStepDefinition[];\n    system_components: WorkflowSystemComponent[];\n    configs?: WorkflowConfigItem[];\n    static fromJSON(json: any): WorkflowDefinition {\n        let workflow = new WorkflowDefinition();\n        Object.assign(workflow, json);\n        return workflow;\n    }\n    serializeToJson(): any {\n        let json = JSON.stringify(this);\n        return json;\n    }\n\n    toJSON() {\n        return {\n            name: this.name,\n            description: this.description,\n            configs: this.configs,\n            steps: this.steps,\n            system_components: this.system_components\n        };\n    }\n\n    upsertConfigItem(config: WorkflowConfigItem) {\n        let index = this.configs.findIndex(c => c.name == config.name);\n        if (index >= 0) {\n            this.configs[index] = config;\n        }else {\n            this.configs.push(config);\n        }\n    }\n\n    addConfigItem(config: WorkflowConfigItem) {\n        this.configs.push(config);\n    }\n\n    deleteConfigItem(name: string) {\n        let index = this.configs.findIndex(c => c.name == name);\n        if (index >= 0) {\n            this.configs.splice(index, 1);\n\n        }\n    }\n\n    getStepById(id: string): WorkflowStepDefinition {\n        let step = this.steps.find(step => step.id == id);\n        return step;\n    }\n\n    getSystemComponentById(id: string): WorkflowSystemComponent {\n        let systemComponent = this.system_components.find(systemComponent => systemComponent.id == id);\n        return systemComponent;\n    }\n\n    updateStep(id:string,step: WorkflowStepDefinition) {\n        let index = this.steps.findIndex(s => s.id == id);\n        if (index >= 0) {\n            this.steps[index] = step;\n        }\n    }\n\n    updateSystemComponent(id:string,systemComponent: WorkflowSystemComponent) {\n        let index = this.system_components.findIndex(g => g.id == id);\n        if (index >= 0) {\n            this.system_components[index] = systemComponent;\n        }\n    }\n\n    convertStepsToNodes():any {\n        let nodes = [];\n        this.steps.forEach(step => {\n            let style = {};\n            if (step.enabled == false) {\n                style = { borderColor: 'red'};\n            }\n            let node = {\n                id: step.id,\n                position: {\n                    x: step.ui_config.pos_x,\n                    y: step.ui_config.pos_y\n                },\n                data: {\n                    label: step.label\n                },\n                width: 150,\n                height: 40,\n                style : style,\n                selected: false,\n                positionAbsolute: {\n                    x: step.ui_config.pos_x,\n                    y: step.ui_config.pos_y\n                },\n                dragging: false\n            }\n            nodes.push(node);\n        });\n        return nodes;\n    }\n\n\n    convertSystemComponentsToNodes():any {\n        let nodes = [];\n        this.system_components?.forEach(step => {\n            let style = {};\n            let node = {\n                id: step.id,\n                position: {\n                    x: step.ui_config.pos_x,\n                    y: step.ui_config.pos_y\n                },\n                data: {\n                    label: step.label\n                },\n                width: 150,\n                height: 40,\n                style : style,\n                selected: false,\n                positionAbsolute: {\n                    x: step.ui_config.pos_x,\n                    y: step.ui_config.pos_y\n                },\n                dragging: false\n            }\n            nodes.push(node);\n        });\n        return nodes;\n    }\n\n    convertStepsToEdges():any {\n        let edges = [];\n        this.steps?.forEach(step => {\n            if (step.transition_to) {\n                step.transition_to.forEach(transition => {\n                    let edge = {\n                        id: step.id + \"_\" + transition,\n                        source: step.id,\n                        target: transition,\n                        animated: true,\n                        label: \"\",\n                        arrowHeadType: \"arrowclosed\"\n                    }\n                    edges.push(edge);\n                });\n            }\n        });\n        return edges;\n    }\n\n    convertSystemComponentsToEdges():any {\n        let edges = [];\n        this.system_components?.forEach(step => {\n            if (step.transition_to) {\n                step.transition_to.forEach(transition => {\n                    let edge = {\n                        id: step.id + \"_\" + transition,\n                        source: step.id,\n                        target: transition,\n                        animated: true,\n                        label: \"\",\n                        arrowHeadType: \"arrowclosed\"\n                    }\n                    edges.push(edge);\n                });\n            }\n        });\n        console.log(\"Component edges: \");\n        console.dir(edges)\n        return edges;\n    }\n\n    updatePositions(nodes:any) {\n        nodes.forEach(node => {\n            let step = this.steps.find(step => step.id == node.id);\n            if (step) {\n                step.ui_config.pos_x = node.position.x;\n                step.ui_config.pos_y = node.position.y;\n            }else {\n                let systemComponent = this.system_components.find(systemComponent => systemComponent.id == node.id);\n                if (systemComponent) {\n                    systemComponent.ui_config.pos_x = node.position.x;\n                    systemComponent.ui_config.pos_y = node.position.y;\n                }\n            }\n        });\n    }\n    // Update step transitions from edges\n    updateStepTransitions(edges:any) {\n        this.steps.forEach(step => {\n            step.transition_to = [];\n        });\n        edges.forEach(edge => {\n            let source = this.steps.find(step => step.id == edge.source);\n            if (source) {\n                source.transition_to.push(edge.target);\n            }\n        });\n    }\n    // Update systemComponent transitions from edges\n    updateSystemComponentTransitions(edges:any) {\n        this.system_components.forEach(systemComponent => {\n            systemComponent.transition_to = [];\n        });\n        edges.forEach(edge => {\n            let source = this.system_components.find(systemComponent => systemComponent.id == edge.source);\n            if (source) {\n                source.transition_to.push(edge.target);\n            }\n        });\n    }\n\n    deleteStep(id:string) {\n        let index = this.steps.findIndex(s => s.id == id);\n        if (index >= 0) {\n            this.steps.splice(index,1);\n        }\n    }\n\n    deleteSystemComponent(id:string) {\n        let index = this.system_components.findIndex(g => g.id == id);\n        if (index >= 0) {\n            this.system_components.splice(index,1);\n        }\n    }\n\n\n}\n",
         "import toPropertyKey from \"./toPropertyKey.js\";\nfunction _defineProperties(target, props) {\n  for (var i = 0; i < props.length; i++) {\n    var descriptor = props[i];\n    descriptor.enumerable = descriptor.enumerable || false;\n    descriptor.configurable = true;\n    if (\"value\" in descriptor) descriptor.writable = true;\n    Object.defineProperty(target, toPropertyKey(descriptor.key), descriptor);\n  }\n}\nexport default function _createClass(Constructor, protoProps, staticProps) {\n  if (protoProps) _defineProperties(Constructor.prototype, protoProps);\n  if (staticProps) _defineProperties(Constructor, staticProps);\n  Object.defineProperty(Constructor, \"prototype\", {\n    writable: false\n  });\n  return Constructor;\n}",
         "export default function _classCallCheck(instance, Constructor) {\n  if (!(instance instanceof Constructor)) {\n    throw new TypeError(\"Cannot call a class as a function\");\n  }\n}",
         "// Supports determination of isControlled().\n// Controlled input accepts its current value as a prop.\n//\n// @see https://facebook.github.io/react/docs/forms.html#controlled-components\n// @param value\n// @returns {boolean} true if string (including '') or number (including zero)\nexport function hasValue(value) {\n  return value != null && !(Array.isArray(value) && value.length === 0);\n}\n\n// Determine if field is empty or filled.\n// Response determines if label is presented above field or as placeholder.\n//\n// @param obj\n// @param SSR\n// @returns {boolean} False when not present or empty string.\n//                    True when any number or string with length.\nexport function isFilled(obj, SSR = false) {\n  return obj && (hasValue(obj.value) && obj.value !== '' || SSR && hasValue(obj.defaultValue) && obj.defaultValue !== '');\n}\n\n// Determine if an Input is adorned on start.\n// It's corresponding to the left with LTR.\n//\n// @param obj\n// @returns {boolean} False when no adornments.\n//                    True when adorned at the start.\nexport function isAdornedStart(obj) {\n  return obj.startAdornment;\n}",
         "import * as React from 'react';\n/**\n * @ignore - internal component.\n */\nconst FormControlContext = /*#__PURE__*/React.createContext(undefined);\nif (process.env.NODE_ENV !== 'production') {\n  FormControlContext.displayName = 'FormControlContext';\n}\nexport default FormControlContext;",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getFormControlUtilityClasses(slot) {\n  return generateUtilityClass('MuiFormControl', slot);\n}\nconst formControlClasses = generateUtilityClasses('MuiFormControl', ['root', 'marginNone', 'marginNormal', 'marginDense', 'fullWidth', 'disabled']);\nexport default formControlClasses;",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"children\", \"className\", \"color\", \"component\", \"disabled\", \"error\", \"focused\", \"fullWidth\", \"hiddenLabel\", \"margin\", \"required\", \"size\", \"variant\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport useThemeProps from '../styles/useThemeProps';\nimport styled from '../styles/styled';\nimport { isFilled, isAdornedStart } from '../InputBase/utils';\nimport capitalize from '../utils/capitalize';\nimport isMuiElement from '../utils/isMuiElement';\nimport FormControlContext from './FormControlContext';\nimport { getFormControlUtilityClasses } from './formControlClasses';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst useUtilityClasses = ownerState => {\n  const {\n    classes,\n    margin,\n    fullWidth\n  } = ownerState;\n  const slots = {\n    root: ['root', margin !== 'none' && `margin${capitalize(margin)}`, fullWidth && 'fullWidth']\n  };\n  return composeClasses(slots, getFormControlUtilityClasses, classes);\n};\nconst FormControlRoot = styled('div', {\n  name: 'MuiFormControl',\n  slot: 'Root',\n  overridesResolver: ({\n    ownerState\n  }, styles) => {\n    return _extends({}, styles.root, styles[`margin${capitalize(ownerState.margin)}`], ownerState.fullWidth && styles.fullWidth);\n  }\n})(({\n  ownerState\n}) => _extends({\n  display: 'inline-flex',\n  flexDirection: 'column',\n  position: 'relative',\n  // Reset fieldset default style.\n  minWidth: 0,\n  padding: 0,\n  margin: 0,\n  border: 0,\n  verticalAlign: 'top'\n}, ownerState.margin === 'normal' && {\n  marginTop: 16,\n  marginBottom: 8\n}, ownerState.margin === 'dense' && {\n  marginTop: 8,\n  marginBottom: 4\n}, ownerState.fullWidth && {\n  width: '100%'\n}));\n\n/**\n * Provides context such as filled/focused/error/required for form inputs.\n * Relying on the context provides high flexibility and ensures that the state always stays\n * consistent across the children of the `FormControl`.\n * This context is used by the following components:\n *\n *  - FormLabel\n *  - FormHelperText\n *  - Input\n *  - InputLabel\n *\n * You can find one composition example below and more going to [the demos](/material-ui/react-text-field/#components).\n *\n * ```jsx\n * <FormControl>\n *   <InputLabel htmlFor=\"my-input\">Email address</InputLabel>\n *   <Input id=\"my-input\" aria-describedby=\"my-helper-text\" />\n *   <FormHelperText id=\"my-helper-text\">We'll never share your email.</FormHelperText>\n * </FormControl>\n * ```\n *\n * \u26a0\ufe0f Only one `InputBase` can be used within a FormControl because it creates visual inconsistencies.\n * For instance, only one input can be focused at the same time, the state shouldn't be shared.\n */\nconst FormControl = /*#__PURE__*/React.forwardRef(function FormControl(inProps, ref) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiFormControl'\n  });\n  const {\n      children,\n      className,\n      color = 'primary',\n      component = 'div',\n      disabled = false,\n      error = false,\n      focused: visuallyFocused,\n      fullWidth = false,\n      hiddenLabel = false,\n      margin = 'none',\n      required = false,\n      size = 'medium',\n      variant = 'outlined'\n    } = props,\n    other = _objectWithoutPropertiesLoose(props, _excluded);\n  const ownerState = _extends({}, props, {\n    color,\n    component,\n    disabled,\n    error,\n    fullWidth,\n    hiddenLabel,\n    margin,\n    required,\n    size,\n    variant\n  });\n  const classes = useUtilityClasses(ownerState);\n  const [adornedStart, setAdornedStart] = React.useState(() => {\n    // We need to iterate through the children and find the Input in order\n    // to fully support server-side rendering.\n    let initialAdornedStart = false;\n    if (children) {\n      React.Children.forEach(children, child => {\n        if (!isMuiElement(child, ['Input', 'Select'])) {\n          return;\n        }\n        const input = isMuiElement(child, ['Select']) ? child.props.input : child;\n        if (input && isAdornedStart(input.props)) {\n          initialAdornedStart = true;\n        }\n      });\n    }\n    return initialAdornedStart;\n  });\n  const [filled, setFilled] = React.useState(() => {\n    // We need to iterate through the children and find the Input in order\n    // to fully support server-side rendering.\n    let initialFilled = false;\n    if (children) {\n      React.Children.forEach(children, child => {\n        if (!isMuiElement(child, ['Input', 'Select'])) {\n          return;\n        }\n        if (isFilled(child.props, true)) {\n          initialFilled = true;\n        }\n      });\n    }\n    return initialFilled;\n  });\n  const [focusedState, setFocused] = React.useState(false);\n  if (disabled && focusedState) {\n    setFocused(false);\n  }\n  const focused = visuallyFocused !== undefined && !disabled ? visuallyFocused : focusedState;\n  let registerEffect;\n  if (process.env.NODE_ENV !== 'production') {\n    // eslint-disable-next-line react-hooks/rules-of-hooks\n    const registeredInput = React.useRef(false);\n    registerEffect = () => {\n      if (registeredInput.current) {\n        console.error(['MUI: There are multiple `InputBase` components inside a FormControl.', 'This creates visual inconsistencies, only use one `InputBase`.'].join('\\n'));\n      }\n      registeredInput.current = true;\n      return () => {\n        registeredInput.current = false;\n      };\n    };\n  }\n  const childContext = React.useMemo(() => {\n    return {\n      adornedStart,\n      setAdornedStart,\n      color,\n      disabled,\n      error,\n      filled,\n      focused,\n      fullWidth,\n      hiddenLabel,\n      size,\n      onBlur: () => {\n        setFocused(false);\n      },\n      onEmpty: () => {\n        setFilled(false);\n      },\n      onFilled: () => {\n        setFilled(true);\n      },\n      onFocus: () => {\n        setFocused(true);\n      },\n      registerEffect,\n      required,\n      variant\n    };\n  }, [adornedStart, color, disabled, error, filled, focused, fullWidth, hiddenLabel, registerEffect, required, size, variant]);\n  return /*#__PURE__*/_jsx(FormControlContext.Provider, {\n    value: childContext,\n    children: /*#__PURE__*/_jsx(FormControlRoot, _extends({\n      as: component,\n      ownerState: ownerState,\n      className: clsx(classes.root, className),\n      ref: ref\n    }, other, {\n      children: children\n    }))\n  });\n});\nprocess.env.NODE_ENV !== \"production\" ? FormControl.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * The content of the component.\n   */\n  children: PropTypes.node,\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n  /**\n   * The color of the component.\n   * It supports both default and custom theme colors, which can be added as shown in the\n   * [palette customization guide](https://mui.com/material-ui/customization/palette/#adding-new-colors).\n   * @default 'primary'\n   */\n  color: PropTypes /* @typescript-to-proptypes-ignore */.oneOfType([PropTypes.oneOf(['primary', 'secondary', 'error', 'info', 'success', 'warning']), PropTypes.string]),\n  /**\n   * The component used for the root node.\n   * Either a string to use a HTML element or a component.\n   */\n  component: PropTypes.elementType,\n  /**\n   * If `true`, the label, input and helper text should be displayed in a disabled state.\n   * @default false\n   */\n  disabled: PropTypes.bool,\n  /**\n   * If `true`, the label is displayed in an error state.\n   * @default false\n   */\n  error: PropTypes.bool,\n  /**\n   * If `true`, the component is displayed in focused state.\n   */\n  focused: PropTypes.bool,\n  /**\n   * If `true`, the component will take up the full width of its container.\n   * @default false\n   */\n  fullWidth: PropTypes.bool,\n  /**\n   * If `true`, the label is hidden.\n   * This is used to increase density for a `FilledInput`.\n   * Be sure to add `aria-label` to the `input` element.\n   * @default false\n   */\n  hiddenLabel: PropTypes.bool,\n  /**\n   * If `dense` or `normal`, will adjust vertical spacing of this and contained components.\n   * @default 'none'\n   */\n  margin: PropTypes.oneOf(['dense', 'none', 'normal']),\n  /**\n   * If `true`, the label will indicate that the `input` is required.\n   * @default false\n   */\n  required: PropTypes.bool,\n  /**\n   * The size of the component.\n   * @default 'medium'\n   */\n  size: PropTypes /* @typescript-to-proptypes-ignore */.oneOfType([PropTypes.oneOf(['medium', 'small']), PropTypes.string]),\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object]),\n  /**\n   * The variant to use.\n   * @default 'outlined'\n   */\n  variant: PropTypes.oneOf(['filled', 'outlined', 'standard'])\n} : void 0;\nexport default FormControl;",
         "export default function formControlState({\n  props,\n  states,\n  muiFormControl\n}) {\n  return states.reduce((acc, state) => {\n    acc[state] = props[state];\n    if (muiFormControl) {\n      if (typeof props[state] === 'undefined') {\n        acc[state] = muiFormControl[state];\n      }\n    }\n    return acc;\n  }, {});\n}",
@@ -12542,15 +12545,15 @@
         "/******************************************************************************\r\nCopyright (c) Microsoft Corporation.\r\n\r\nPermission to use, copy, modify, and/or distribute this software for any\r\npurpose with or without fee is hereby granted.\r\n\r\nTHE SOFTWARE IS PROVIDED \"AS IS\" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH\r\nREGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY\r\nAND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,\r\nINDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM\r\nLOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR\r\nOTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR\r\nPERFORMANCE OF THIS SOFTWARE.\r\n***************************************************************************** */\r\n/* global Reflect, Promise */\r\n\r\nvar extendStatics = function(d, b) {\r\n    extendStatics = Object.setPrototypeOf ||\r\n        ({ __proto__: [] } instanceof Array && function (d, b) { d.__proto__ = b; }) ||\r\n        function (d, b) { for (var p in b) if (Object.prototype.hasOwnProperty.call(b, p)) d[p] = b[p]; };\r\n    return extendStatics(d, b);\r\n};\r\n\r\nexport function __extends(d, b) {\r\n    if (typeof b !== \"function\" && b !== null)\r\n        throw new TypeError(\"Class extends value \" + String(b) + \" is not a constructor or null\");\r\n    extendStatics(d, b);\r\n    function __() { this.constructor = d; }\r\n    d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());\r\n}\r\n\r\nexport var __assign = function() {\r\n    __assign = Object.assign || function __assign(t) {\r\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\r\n            s = arguments[i];\r\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p)) t[p] = s[p];\r\n        }\r\n        return t;\r\n    }\r\n    return __assign.apply(this, arguments);\r\n}\r\n\r\nexport function __rest(s, e) {\r\n    var t = {};\r\n    for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p) && e.indexOf(p) < 0)\r\n        t[p] = s[p];\r\n    if (s != null && typeof Object.getOwnPropertySymbols === \"function\")\r\n        for (var i = 0, p = Object.getOwnPropertySymbols(s); i < p.length; i++) {\r\n            if (e.indexOf(p[i]) < 0 && Object.prototype.propertyIsEnumerable.call(s, p[i]))\r\n                t[p[i]] = s[p[i]];\r\n        }\r\n    return t;\r\n}\r\n\r\nexport function __decorate(decorators, target, key, desc) {\r\n    var c = arguments.length, r = c < 3 ? target : desc === null ? desc = Object.getOwnPropertyDescriptor(target, key) : desc, d;\r\n    if (typeof Reflect === \"object\" && typeof Reflect.decorate === \"function\") r = Reflect.decorate(decorators, target, key, desc);\r\n    else for (var i = decorators.length - 1; i >= 0; i--) if (d = decorators[i]) r = (c < 3 ? d(r) : c > 3 ? d(target, key, r) : d(target, key)) || r;\r\n    return c > 3 && r && Object.defineProperty(target, key, r), r;\r\n}\r\n\r\nexport function __param(paramIndex, decorator) {\r\n    return function (target, key) { decorator(target, key, paramIndex); }\r\n}\r\n\r\nexport function __metadata(metadataKey, metadataValue) {\r\n    if (typeof Reflect === \"object\" && typeof Reflect.metadata === \"function\") return Reflect.metadata(metadataKey, metadataValue);\r\n}\r\n\r\nexport function __awaiter(thisArg, _arguments, P, generator) {\r\n    function adopt(value) { return value instanceof P ? value : new P(function (resolve) { resolve(value); }); }\r\n    return new (P || (P = Promise))(function (resolve, reject) {\r\n        function fulfilled(value) { try { step(generator.next(value)); } catch (e) { reject(e); } }\r\n        function rejected(value) { try { step(generator[\"throw\"](value)); } catch (e) { reject(e); } }\r\n        function step(result) { result.done ? resolve(result.value) : adopt(result.value).then(fulfilled, rejected); }\r\n        step((generator = generator.apply(thisArg, _arguments || [])).next());\r\n    });\r\n}\r\n\r\nexport function __generator(thisArg, body) {\r\n    var _ = { label: 0, sent: function() { if (t[0] & 1) throw t[1]; return t[1]; }, trys: [], ops: [] }, f, y, t, g;\r\n    return g = { next: verb(0), \"throw\": verb(1), \"return\": verb(2) }, typeof Symbol === \"function\" && (g[Symbol.iterator] = function() { return this; }), g;\r\n    function verb(n) { return function (v) { return step([n, v]); }; }\r\n    function step(op) {\r\n        if (f) throw new TypeError(\"Generator is already executing.\");\r\n        while (g && (g = 0, op[0] && (_ = 0)), _) try {\r\n            if (f = 1, y && (t = op[0] & 2 ? y[\"return\"] : op[0] ? y[\"throw\"] || ((t = y[\"return\"]) && t.call(y), 0) : y.next) && !(t = t.call(y, op[1])).done) return t;\r\n            if (y = 0, t) op = [op[0] & 2, t.value];\r\n            switch (op[0]) {\r\n                case 0: case 1: t = op; break;\r\n                case 4: _.label++; return { value: op[1], done: false };\r\n                case 5: _.label++; y = op[1]; op = [0]; continue;\r\n                case 7: op = _.ops.pop(); _.trys.pop(); continue;\r\n                default:\r\n                    if (!(t = _.trys, t = t.length > 0 && t[t.length - 1]) && (op[0] === 6 || op[0] === 2)) { _ = 0; continue; }\r\n                    if (op[0] === 3 && (!t || (op[1] > t[0] && op[1] < t[3]))) { _.label = op[1]; break; }\r\n                    if (op[0] === 6 && _.label < t[1]) { _.label = t[1]; t = op; break; }\r\n                    if (t && _.label < t[2]) { _.label = t[2]; _.ops.push(op); break; }\r\n                    if (t[2]) _.ops.pop();\r\n                    _.trys.pop(); continue;\r\n            }\r\n            op = body.call(thisArg, _);\r\n        } catch (e) { op = [6, e]; y = 0; } finally { f = t = 0; }\r\n        if (op[0] & 5) throw op[1]; return { value: op[0] ? op[1] : void 0, done: true };\r\n    }\r\n}\r\n\r\nexport var __createBinding = Object.create ? (function(o, m, k, k2) {\r\n    if (k2 === undefined) k2 = k;\r\n    var desc = Object.getOwnPropertyDescriptor(m, k);\r\n    if (!desc || (\"get\" in desc ? !m.__esModule : desc.writable || desc.configurable)) {\r\n        desc = { enumerable: true, get: function() { return m[k]; } };\r\n    }\r\n    Object.defineProperty(o, k2, desc);\r\n}) : (function(o, m, k, k2) {\r\n    if (k2 === undefined) k2 = k;\r\n    o[k2] = m[k];\r\n});\r\n\r\nexport function __exportStar(m, o) {\r\n    for (var p in m) if (p !== \"default\" && !Object.prototype.hasOwnProperty.call(o, p)) __createBinding(o, m, p);\r\n}\r\n\r\nexport function __values(o) {\r\n    var s = typeof Symbol === \"function\" && Symbol.iterator, m = s && o[s], i = 0;\r\n    if (m) return m.call(o);\r\n    if (o && typeof o.length === \"number\") return {\r\n        next: function () {\r\n            if (o && i >= o.length) o = void 0;\r\n            return { value: o && o[i++], done: !o };\r\n        }\r\n    };\r\n    throw new TypeError(s ? \"Object is not iterable.\" : \"Symbol.iterator is not defined.\");\r\n}\r\n\r\nexport function __read(o, n) {\r\n    var m = typeof Symbol === \"function\" && o[Symbol.iterator];\r\n    if (!m) return o;\r\n    var i = m.call(o), r, ar = [], e;\r\n    try {\r\n        while ((n === void 0 || n-- > 0) && !(r = i.next()).done) ar.push(r.value);\r\n    }\r\n    catch (error) { e = { error: error }; }\r\n    finally {\r\n        try {\r\n            if (r && !r.done && (m = i[\"return\"])) m.call(i);\r\n        }\r\n        finally { if (e) throw e.error; }\r\n    }\r\n    return ar;\r\n}\r\n\r\n/** @deprecated */\r\nexport function __spread() {\r\n    for (var ar = [], i = 0; i < arguments.length; i++)\r\n        ar = ar.concat(__read(arguments[i]));\r\n    return ar;\r\n}\r\n\r\n/** @deprecated */\r\nexport function __spreadArrays() {\r\n    for (var s = 0, i = 0, il = arguments.length; i < il; i++) s += arguments[i].length;\r\n    for (var r = Array(s), k = 0, i = 0; i < il; i++)\r\n        for (var a = arguments[i], j = 0, jl = a.length; j < jl; j++, k++)\r\n            r[k] = a[j];\r\n    return r;\r\n}\r\n\r\nexport function __spreadArray(to, from, pack) {\r\n    if (pack || arguments.length === 2) for (var i = 0, l = from.length, ar; i < l; i++) {\r\n        if (ar || !(i in from)) {\r\n            if (!ar) ar = Array.prototype.slice.call(from, 0, i);\r\n            ar[i] = from[i];\r\n        }\r\n    }\r\n    return to.concat(ar || Array.prototype.slice.call(from));\r\n}\r\n\r\nexport function __await(v) {\r\n    return this instanceof __await ? (this.v = v, this) : new __await(v);\r\n}\r\n\r\nexport function __asyncGenerator(thisArg, _arguments, generator) {\r\n    if (!Symbol.asyncIterator) throw new TypeError(\"Symbol.asyncIterator is not defined.\");\r\n    var g = generator.apply(thisArg, _arguments || []), i, q = [];\r\n    return i = {}, verb(\"next\"), verb(\"throw\"), verb(\"return\"), i[Symbol.asyncIterator] = function () { return this; }, i;\r\n    function verb(n) { if (g[n]) i[n] = function (v) { return new Promise(function (a, b) { q.push([n, v, a, b]) > 1 || resume(n, v); }); }; }\r\n    function resume(n, v) { try { step(g[n](v)); } catch (e) { settle(q[0][3], e); } }\r\n    function step(r) { r.value instanceof __await ? Promise.resolve(r.value.v).then(fulfill, reject) : settle(q[0][2], r); }\r\n    function fulfill(value) { resume(\"next\", value); }\r\n    function reject(value) { resume(\"throw\", value); }\r\n    function settle(f, v) { if (f(v), q.shift(), q.length) resume(q[0][0], q[0][1]); }\r\n}\r\n\r\nexport function __asyncDelegator(o) {\r\n    var i, p;\r\n    return i = {}, verb(\"next\"), verb(\"throw\", function (e) { throw e; }), verb(\"return\"), i[Symbol.iterator] = function () { return this; }, i;\r\n    function verb(n, f) { i[n] = o[n] ? function (v) { return (p = !p) ? { value: __await(o[n](v)), done: n === \"return\" } : f ? f(v) : v; } : f; }\r\n}\r\n\r\nexport function __asyncValues(o) {\r\n    if (!Symbol.asyncIterator) throw new TypeError(\"Symbol.asyncIterator is not defined.\");\r\n    var m = o[Symbol.asyncIterator], i;\r\n    return m ? m.call(o) : (o = typeof __values === \"function\" ? __values(o) : o[Symbol.iterator](), i = {}, verb(\"next\"), verb(\"throw\"), verb(\"return\"), i[Symbol.asyncIterator] = function () { return this; }, i);\r\n    function verb(n) { i[n] = o[n] && function (v) { return new Promise(function (resolve, reject) { v = o[n](v), settle(resolve, reject, v.done, v.value); }); }; }\r\n    function settle(resolve, reject, d, v) { Promise.resolve(v).then(function(v) { resolve({ value: v, done: d }); }, reject); }\r\n}\r\n\r\nexport function __makeTemplateObject(cooked, raw) {\r\n    if (Object.defineProperty) { Object.defineProperty(cooked, \"raw\", { value: raw }); } else { cooked.raw = raw; }\r\n    return cooked;\r\n};\r\n\r\nvar __setModuleDefault = Object.create ? (function(o, v) {\r\n    Object.defineProperty(o, \"default\", { enumerable: true, value: v });\r\n}) : function(o, v) {\r\n    o[\"default\"] = v;\r\n};\r\n\r\nexport function __importStar(mod) {\r\n    if (mod && mod.__esModule) return mod;\r\n    var result = {};\r\n    if (mod != null) for (var k in mod) if (k !== \"default\" && Object.prototype.hasOwnProperty.call(mod, k)) __createBinding(result, mod, k);\r\n    __setModuleDefault(result, mod);\r\n    return result;\r\n}\r\n\r\nexport function __importDefault(mod) {\r\n    return (mod && mod.__esModule) ? mod : { default: mod };\r\n}\r\n\r\nexport function __classPrivateFieldGet(receiver, state, kind, f) {\r\n    if (kind === \"a\" && !f) throw new TypeError(\"Private accessor was defined without a getter\");\r\n    if (typeof state === \"function\" ? receiver !== state || !f : !state.has(receiver)) throw new TypeError(\"Cannot read private member from an object whose class did not declare it\");\r\n    return kind === \"m\" ? f : kind === \"a\" ? f.call(receiver) : f ? f.value : state.get(receiver);\r\n}\r\n\r\nexport function __classPrivateFieldSet(receiver, state, value, kind, f) {\r\n    if (kind === \"m\") throw new TypeError(\"Private method is not writable\");\r\n    if (kind === \"a\" && !f) throw new TypeError(\"Private accessor was defined without a setter\");\r\n    if (typeof state === \"function\" ? receiver !== state || !f : !state.has(receiver)) throw new TypeError(\"Cannot write private member to an object whose class did not declare it\");\r\n    return (kind === \"a\" ? f.call(receiver, value) : f ? f.value = value : state.set(receiver, value)), value;\r\n}\r\n\r\nexport function __classPrivateFieldIn(state, receiver) {\r\n    if (receiver === null || (typeof receiver !== \"object\" && typeof receiver !== \"function\")) throw new TypeError(\"Cannot use 'in' operator on non-object\");\r\n    return typeof state === \"function\" ? receiver === state : state.has(receiver);\r\n}\r\n",
         null,
         null,
         "import Box from '@mui/material/Box';\nimport Button from '@mui/material/Button';\nimport Dialog from '@mui/material/Dialog';\nimport DialogActions from '@mui/material/DialogActions';\nimport DialogContent from '@mui/material/DialogContent';\nimport DialogTitle from '@mui/material/DialogTitle';\nimport FormControl from '@mui/material/FormControl';\nimport TextField from '@mui/material/TextField';\nimport { Container } from '@mui/system';\nimport React from 'react';\nimport { useState } from 'react';\nimport FileUpload from 'react-mui-fileuploader';\nimport { getNeatApiRootUrl, getSelectedWorkflowName } from './Utils';\n\nexport default function LocalUploader(props: any) {\n    const [dialogOpen, setDialogOpen] = useState(false);\n    const [data, setData] = useState<any>({comments:\"\",author:\"\"});\n    const [error, setError] = useState<string>(\"\");\n    const handleDialogClickOpen = () => {\n        setDialogOpen(true);\n    };\n\n    const handleDialogClose = () => {\n        setDialogOpen(false);\n    };\n    const handleDialogPublish = () => {\n        uploadFiles();\n    };\n    const handleStepConfigChange = (name: string, value: any) => {\n        console.log('handleStepConfigChange')\n        data[name] = value;\n    }\n\n    const [filesToUpload, setFilesToUpload] = useState([])\n\n    const handleFilesChange = (files) => {\n        // Update chosen files\n        setFilesToUpload([ ...files ])\n    };\n\n    const uploadFiles = () => {\n        // Create a form and post it to server\n        const neatApiRootUrl = getNeatApiRootUrl();\n        const workflowName = getSelectedWorkflowName();\n        let formData = new FormData()\n        filesToUpload.forEach((file) => formData.append(\"files\", file))\n\n        fetch(neatApiRootUrl+\"/api/file/upload/\"+workflowName+\"/rules\", {\n        method: \"POST\",\n        body: formData\n        }).then((response) => {\n            if (response.ok) {\n                setDialogOpen(false);\n                return response.json();\n            }else{\n                setError(response.statusText);\n            }\n\n        }).then((data) => {\n        const fileName = data.file_name;\n        const fileHash = data.hash;\n        props.onUpload(fileName, fileHash);\n        setDialogOpen(false);\n        }).catch((error) => {\n            setError(error);\n        } )\n    }\n\n    return (\n        <React.Fragment>\n          <Dialog open={dialogOpen} onClose={handleDialogClose}>\n            <DialogTitle>Upload {props.type} to local storage</DialogTitle>\n            <DialogContent>\n            <FileUpload\n                title=\"Rules file uploader\"\n                multiFile={true}\n                showPlaceholderImage={false}\n                header=\"[Drag to drop new rules file here or click to select a file]\"\n                onFilesChange={handleFilesChange}\n                onContextReady={(context) => {}}\n                filesContainerHeight={100}\n            />\n                {error && <Container sx={{ color: 'red' }}>{error}</Container>}\n            </DialogContent>\n            <DialogActions>\n                <Button onClick={handleDialogClose}>Cancel</Button>\n                <Button onClick={handleDialogPublish}>Upload</Button>\n            </DialogActions>\n          </Dialog>\n          <Button variant=\"outlined\" sx={{ marginTop: 2, marginRight: 1 }} onClick={handleDialogClickOpen} >Upload to local storage </Button>\n        </React.Fragment>\n    )\n}\n",
         "import PropTypes from 'prop-types';\nimport { createContainer } from '@mui/system';\nimport capitalize from '../utils/capitalize';\nimport styled from '../styles/styled';\nimport useThemeProps from '../styles/useThemeProps';\nconst Container = createContainer({\n  createStyledComponent: styled('div', {\n    name: 'MuiContainer',\n    slot: 'Root',\n    overridesResolver: (props, styles) => {\n      const {\n        ownerState\n      } = props;\n      return [styles.root, styles[`maxWidth${capitalize(String(ownerState.maxWidth))}`], ownerState.fixed && styles.fixed, ownerState.disableGutters && styles.disableGutters];\n    }\n  }),\n  useThemeProps: inProps => useThemeProps({\n    props: inProps,\n    name: 'MuiContainer'\n  })\n});\nprocess.env.NODE_ENV !== \"production\" ? Container.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * @ignore\n   */\n  children: PropTypes.node,\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * The component used for the root node.\n   * Either a string to use a HTML element or a component.\n   */\n  component: PropTypes.elementType,\n  /**\n   * If `true`, the left and right padding is removed.\n   * @default false\n   */\n  disableGutters: PropTypes.bool,\n  /**\n   * Set the max-width to match the min-width of the current breakpoint.\n   * This is useful if you'd prefer to design for a fixed set of sizes\n   * instead of trying to accommodate a fully fluid viewport.\n   * It's fluid by default.\n   * @default false\n   */\n  fixed: PropTypes.bool,\n  /**\n   * Determine the max-width of the container.\n   * The container width grows with the size of the screen.\n   * Set to `false` to disable `maxWidth`.\n   * @default 'lg'\n   */\n  maxWidth: PropTypes /* @typescript-to-proptypes-ignore */.oneOfType([PropTypes.oneOf(['xs', 'sm', 'md', 'lg', 'xl', false]), PropTypes.string]),\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object])\n} : void 0;\nexport default Container;",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getAlertTitleUtilityClass(slot) {\n  return generateUtilityClass('MuiAlertTitle', slot);\n}\nconst alertTitleClasses = generateUtilityClasses('MuiAlertTitle', ['root']);\nexport default alertTitleClasses;",
         "import _extends from \"@babel/runtime/helpers/esm/extends\";\nimport _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nconst _excluded = [\"className\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport styled from '../styles/styled';\nimport useThemeProps from '../styles/useThemeProps';\nimport Typography from '../Typography';\nimport { getAlertTitleUtilityClass } from './alertTitleClasses';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst useUtilityClasses = ownerState => {\n  const {\n    classes\n  } = ownerState;\n  const slots = {\n    root: ['root']\n  };\n  return composeClasses(slots, getAlertTitleUtilityClass, classes);\n};\nconst AlertTitleRoot = styled(Typography, {\n  name: 'MuiAlertTitle',\n  slot: 'Root',\n  overridesResolver: (props, styles) => styles.root\n})(({\n  theme\n}) => {\n  return {\n    fontWeight: theme.typography.fontWeightMedium,\n    marginTop: -2\n  };\n});\nconst AlertTitle = /*#__PURE__*/React.forwardRef(function AlertTitle(inProps, ref) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiAlertTitle'\n  });\n  const {\n      className\n    } = props,\n    other = _objectWithoutPropertiesLoose(props, _excluded);\n  const ownerState = props;\n  const classes = useUtilityClasses(ownerState);\n  return /*#__PURE__*/_jsx(AlertTitleRoot, _extends({\n    gutterBottom: true,\n    component: \"div\",\n    ownerState: ownerState,\n    ref: ref,\n    className: clsx(classes.root, className)\n  }, other));\n});\nprocess.env.NODE_ENV !== \"production\" ? AlertTitle.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * The content of the component.\n   */\n  children: PropTypes.node,\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object])\n} : void 0;\nexport default AlertTitle;",
-        "import * as React from 'react';\nimport {useState,useEffect} from 'react';\n\nimport { DataGrid, GridColDef, GridRenderCellParams } from '@mui/x-data-grid';\nimport Box from '@mui/material/Box';\nimport Collapse from '@mui/material/Collapse';\nimport IconButton from '@mui/material/IconButton';\nimport Table from '@mui/material/Table';\nimport TableBody from '@mui/material/TableBody';\nimport TableCell from '@mui/material/TableCell';\nimport TableContainer from '@mui/material/TableContainer';\nimport TableHead from '@mui/material/TableHead';\nimport TableRow from '@mui/material/TableRow';\nimport Typography from '@mui/material/Typography';\nimport Paper from '@mui/material/Paper';\nimport KeyboardArrowDownIcon from '@mui/icons-material/KeyboardArrowDown';\nimport KeyboardArrowUpIcon from '@mui/icons-material/KeyboardArrowUp';\nimport Button from '@mui/material/Button';\nimport { getNeatApiRootUrl, getSelectedWorkflowName } from 'components/Utils';\nimport FileUpload from 'react-mui-fileuploader';\nimport { margin } from '@mui/system';\nimport CdfPublisher from 'components/CdfPublisher';\nimport LocalUploader from 'components/LocalUploader';\nimport Container from '@mui/material/Container';\nimport CdfDownloader from 'components/CdfDownloader';\nimport Alert from '@mui/material/Alert';\nimport AlertTitle from '@mui/material/AlertTitle';\n\nfunction Row(props: { row: any,properties: any }) {\n  const { row,properties } = props;\n  const [open, setOpen] = React.useState(false);\n  const getPropertyByClass = (className: string) => {\n    const r = properties.filter((f: any) => f.class == className);\n    return r;\n  }\n  const [fProps,setFProps] = useState(getPropertyByClass(row.class));\n\n  console.log(\"row = \",row.class);\n\n  return (\n    <React.Fragment>\n      <TableRow sx={{ '& > *': { borderBottom: 'unset' } }}>\n        <TableCell>\n          <IconButton\n            aria-label=\"expand row\"\n            size=\"small\"\n            onClick={() => setOpen(!open)}\n          >\n            {open ? <KeyboardArrowUpIcon /> : <KeyboardArrowDownIcon />}\n          </IconButton>\n        </TableCell>\n        <TableCell component=\"th\" scope=\"row\">\n          {row.class}\n        </TableCell>\n        <TableCell align=\"right\">{row.class_description}</TableCell>\n        <TableCell align=\"right\">{row.cdf_resource_type}</TableCell>\n        <TableCell align=\"right\">{row.cdf_parent_resource}</TableCell>\n        <TableCell align=\"center\"><Button >test</Button></TableCell>\n      </TableRow>\n      <TableRow>\n        <TableCell style={{ paddingBottom: 0, paddingTop: 0 }} colSpan={6}>\n          <Collapse in={open} timeout=\"auto\" unmountOnExit>\n            <Box sx={{ margin: 1 }}>\n              <Typography variant=\"h6\" gutterBottom component=\"div\">\n                Properties\n              </Typography>\n              { fProps != undefined &&(<Table size=\"small\" aria-label=\"purchases\">\n                <TableHead>\n                  <TableRow>\n                    <TableCell><b>Property</b></TableCell>\n                    <TableCell><b>Description</b></TableCell>\n                    <TableCell><b>Value type</b></TableCell>\n                    <TableCell><b>CDF metadata</b></TableCell>\n                    <TableCell><b>Rule type</b></TableCell>\n                    <TableCell><b>Rule (transform from source to solution object)</b></TableCell>\n                    <TableCell><b>Action</b></TableCell>\n                  </TableRow>\n                </TableHead>\n                <TableBody>\n                  {fProps.map((pr) => (\n                    <TableRow key={pr.property}>\n                      <TableCell component=\"th\" scope=\"row\"> {pr.property} </TableCell>\n                      <TableCell>{pr.property_description}</TableCell>\n                      <TableCell>{pr.property_type}</TableCell>\n                      <TableCell>{pr.cdf_resource_type}.{pr.cdf_metadata_type}</TableCell>\n                      <TableCell>{pr.rule_type}</TableCell>\n                      <TableCell>{pr.rule}</TableCell>\n                      <TableCell><Button >test</Button></TableCell>\n                    </TableRow>\n                  ))}\n                </TableBody>\n              </Table> )}\n            </Box>\n          </Collapse>\n        </TableCell>\n      </TableRow>\n    </React.Fragment>\n  );\n}\n\nexport default function TransformationTable() {\n  const neatApiRootUrl = getNeatApiRootUrl();\n  const [data, setData] = useState({\"classes\":[],\"properties\":[],\"file_name\":\"\",\"hash\":\"\",\"error_text\":\"\",\"src\":\"\"});\n  const [alertMsg, setAlertMsg] = useState(\"\");\n  const columns: GridColDef[] = [\n    {field: 'id', headerName: 'ID', width: 70},\n    {field: 'name', headerName: 'Name', width: 130},\n    {field: 'value', headerName: 'Value', type: 'number', width: 90},\n  ];\n  const downloadUrl = neatApiRootUrl+\"/data/rules/\"+data.file_name\n  useEffect(() => {\n    loadDataset(\"\",\"\");\n  }, []);\n\n  const loadDataset = (fileName:string,fileHash:string) => {\n    const workflowName = getSelectedWorkflowName();\n    let url = neatApiRootUrl+\"/api/rules?\"+new URLSearchParams({\"workflow_name\":workflowName,\"file_name\":fileName,\"version\":fileHash}).toString()\n    fetch(url)\n    .then((response) => {\n      return response.json();\n    }).then((data) => {\n      // console.log(text);\n      setAlertMsg(\"\");\n      setData(data);\n    }).catch((err) => {\n      console.log(err);\n      setAlertMsg(\"Transformation rules file \"+fileName+\" is either invalid or missing. Please ensure that you have a valid data model and the necessary transformation rules file in place.\");\n    }\n  )}\n\n  const [filesToUpload, setFilesToUpload] = useState([])\n\n  const onUpload = (fileName:string , hash: string) => {\n    console.log(\"onUpload\",fileName,hash)\n    loadDataset(fileName,hash);\n  }\n\n  const onDownloadSuccess = (fileName:string , hash: string) => {\n    console.log(\"onDownloadSuccess\",fileName,hash)\n    loadDataset(fileName,hash);\n  }\n\n  return (\n    <Box>\n    <Typography variant=\"subtitle1\" gutterBottom>\n        Rules file : <a href={downloadUrl} >{data.file_name}</a>  version : {data.hash} source: {data.src}\n        {data.error_text && <Container sx={{ color: 'red' }}>{data.error_text}</Container>}\n    </Typography>\n    {alertMsg != \"\" && (<Alert severity=\"warning\">\n      <AlertTitle>Warning</AlertTitle>\n        {alertMsg}\n    </Alert> )}\n    <TableContainer component={Paper}>\n      <Table aria-label=\"collapsible table\">\n        <TableHead>\n          <TableRow>\n            <TableCell />\n            <TableCell> <b>Solution class</b></TableCell>\n            <TableCell align=\"right\"><b>Description</b></TableCell>\n            <TableCell align=\"right\"><b>CDF resource</b></TableCell>\n            <TableCell align=\"right\"><b>Parent resource</b></TableCell>\n            <TableCell align=\"right\"><b>Action</b></TableCell>\n          </TableRow>\n        </TableHead>\n        <TableBody>\n          {data.classes.map((row:any) => (\n            <Row key={row.class} row={row} properties={data.properties} />\n          ))}\n        </TableBody>\n      </Table>\n    </TableContainer>\n    <Box sx={{margin:5}}>\n      <CdfPublisher type=\"transformation rules\" fileName={data.file_name} />\n      <CdfDownloader type=\"neat-wf-rules\" onDownloadSuccess={onDownloadSuccess} />\n      <LocalUploader type=\"transformation rules\" onUpload={onUpload} />\n    </Box>\n\n\n    </Box>\n  );\n}\n",
+        "import * as React from 'react';\nimport {useState,useEffect} from 'react';\n\nimport { DataGrid, GridColDef, GridRenderCellParams } from '@mui/x-data-grid';\nimport Box from '@mui/material/Box';\nimport Collapse from '@mui/material/Collapse';\nimport IconButton from '@mui/material/IconButton';\nimport Table from '@mui/material/Table';\nimport TableBody from '@mui/material/TableBody';\nimport TableCell from '@mui/material/TableCell';\nimport TableContainer from '@mui/material/TableContainer';\nimport TableHead from '@mui/material/TableHead';\nimport TableRow from '@mui/material/TableRow';\nimport Typography from '@mui/material/Typography';\nimport Paper from '@mui/material/Paper';\nimport KeyboardArrowDownIcon from '@mui/icons-material/KeyboardArrowDown';\nimport KeyboardArrowUpIcon from '@mui/icons-material/KeyboardArrowUp';\nimport Button from '@mui/material/Button';\nimport { getNeatApiRootUrl, getSelectedWorkflowName } from 'components/Utils';\nimport FileUpload from 'react-mui-fileuploader';\nimport { margin } from '@mui/system';\nimport CdfPublisher from 'components/CdfPublisher';\nimport LocalUploader from 'components/LocalUploader';\nimport Container from '@mui/material/Container';\nimport CdfDownloader from 'components/CdfDownloader';\nimport Alert from '@mui/material/Alert';\nimport AlertTitle from '@mui/material/AlertTitle';\n\nfunction Row(props: { row: any,properties: any }) {\n  const { row,properties } = props;\n  const [open, setOpen] = React.useState(false);\n  const getPropertyByClass = (className: string) => {\n    const r = properties.filter((f: any) => f.class == className);\n    return r;\n  }\n  const [fProps,setFProps] = useState(getPropertyByClass(row.class));\n\n  console.log(\"row = \",row.class);\n\n  return (\n    <React.Fragment>\n      <TableRow sx={{ '& > *': { borderBottom: 'unset' } }}>\n        <TableCell>\n          <IconButton\n            aria-label=\"expand row\"\n            size=\"small\"\n            onClick={() => setOpen(!open)}\n          >\n            {open ? <KeyboardArrowUpIcon /> : <KeyboardArrowDownIcon />}\n          </IconButton>\n        </TableCell>\n        <TableCell component=\"th\" scope=\"row\">\n          {row.class}\n        </TableCell>\n        <TableCell align=\"right\">{row.class_description}</TableCell>\n        <TableCell align=\"right\">{row.cdf_resource_type}</TableCell>\n        <TableCell align=\"right\">{row.cdf_parent_resource}</TableCell>\n        <TableCell align=\"center\"><Button >test</Button></TableCell>\n      </TableRow>\n      <TableRow>\n        <TableCell style={{ paddingBottom: 0, paddingTop: 0 }} colSpan={6}>\n          <Collapse in={open} timeout=\"auto\" unmountOnExit>\n            <Box sx={{ margin: 1 }}>\n              <Typography variant=\"h6\" gutterBottom component=\"div\">\n                Properties\n              </Typography>\n              { fProps != undefined &&(<Table size=\"small\" aria-label=\"purchases\">\n                <TableHead>\n                  <TableRow>\n                    <TableCell><b>Property</b></TableCell>\n                    <TableCell><b>Description</b></TableCell>\n                    <TableCell><b>Value type</b></TableCell>\n                    <TableCell><b>CDF metadata</b></TableCell>\n                    <TableCell><b>Rule type</b></TableCell>\n                    <TableCell><b>Rule (transform from source to solution object)</b></TableCell>\n                    <TableCell><b>Action</b></TableCell>\n                  </TableRow>\n                </TableHead>\n                <TableBody>\n                  {fProps.map((pr) => (\n                    <TableRow key={pr.property}>\n                      <TableCell component=\"th\" scope=\"row\"> {pr.property} </TableCell>\n                      <TableCell>{pr.property_description}</TableCell>\n                      <TableCell>{pr.property_type}</TableCell>\n                      <TableCell>{pr.cdf_resource_type}.{pr.cdf_metadata_type}</TableCell>\n                      <TableCell>{pr.rule_type}</TableCell>\n                      <TableCell>{pr.rule}</TableCell>\n                      <TableCell><Button >test</Button></TableCell>\n                    </TableRow>\n                  ))}\n                </TableBody>\n              </Table> )}\n            </Box>\n          </Collapse>\n        </TableCell>\n      </TableRow>\n    </React.Fragment>\n  );\n}\n\nexport default function TransformationTable() {\n  const neatApiRootUrl = getNeatApiRootUrl();\n  const [data, setData] = useState({\"classes\":[],\"properties\":[],\"file_name\":\"\",\"hash\":\"\",\"error_text\":\"\",\"src\":\"\"});\n  const [alertMsg, setAlertMsg] = useState(\"\");\n  const columns: GridColDef[] = [\n    {field: 'id', headerName: 'ID', width: 70},\n    {field: 'name', headerName: 'Name', width: 130},\n    {field: 'value', headerName: 'Value', type: 'number', width: 90},\n  ];\n  const downloadUrl = neatApiRootUrl+\"/data/rules/\"+data.file_name+\"?version=\"+data.hash;\n  useEffect(() => {\n    loadDataset(\"\",\"\");\n  }, []);\n\n  const loadDataset = (fileName:string,fileHash:string) => {\n    const workflowName = getSelectedWorkflowName();\n    let url = neatApiRootUrl+\"/api/rules?\"+new URLSearchParams({\"workflow_name\":workflowName,\"file_name\":fileName,\"version\":fileHash}).toString()\n    fetch(url)\n    .then((response) => {\n      return response.json();\n    }).then((data) => {\n      // console.log(text);\n      setAlertMsg(\"\");\n      setData(data);\n    }).catch((err) => {\n      console.log(err);\n      setAlertMsg(\"Transformation rules file \"+fileName+\" is either invalid or missing. Please ensure that you have a valid data model and the necessary transformation rules file in place.\");\n    }\n  )}\n\n  const [filesToUpload, setFilesToUpload] = useState([])\n\n  const onUpload = (fileName:string , hash: string) => {\n    console.log(\"onUpload\",fileName,hash)\n    loadDataset(fileName,hash);\n  }\n\n  const onDownloadSuccess = (fileName:string , hash: string) => {\n    console.log(\"onDownloadSuccess\",fileName,hash)\n    loadDataset(fileName,hash);\n  }\n\n  return (\n    <Box>\n    <Typography variant=\"subtitle1\" gutterBottom>\n        Rules file : <a href={downloadUrl} >{data.file_name}</a>  version : {data.hash} source: {data.src}\n        {data.error_text && <Container sx={{ color: 'red' }}>{data.error_text}</Container>}\n    </Typography>\n    {alertMsg != \"\" && (<Alert severity=\"warning\">\n      <AlertTitle>Warning</AlertTitle>\n        {alertMsg}\n    </Alert> )}\n    <TableContainer component={Paper}>\n      <Table aria-label=\"collapsible table\">\n        <TableHead>\n          <TableRow>\n            <TableCell />\n            <TableCell> <b>Solution class</b></TableCell>\n            <TableCell align=\"right\"><b>Description</b></TableCell>\n            <TableCell align=\"right\"><b>CDF resource</b></TableCell>\n            <TableCell align=\"right\"><b>Parent resource</b></TableCell>\n            <TableCell align=\"right\"><b>Action</b></TableCell>\n          </TableRow>\n        </TableHead>\n        <TableBody>\n          {data.classes.map((row:any) => (\n            <Row key={row.class} row={row} properties={data.properties} />\n          ))}\n        </TableBody>\n      </Table>\n    </TableContainer>\n    <Box sx={{margin:5}}>\n      <CdfPublisher type=\"transformation rules\" fileName={data.file_name} />\n      <CdfDownloader type=\"neat-wf-rules\" onDownloadSuccess={onDownloadSuccess} />\n      <LocalUploader type=\"transformation rules\" onUpload={onUpload} />\n    </Box>\n\n\n    </Box>\n  );\n}\n",
         "import * as React from 'react';\nimport createSvgIcon from '../../utils/createSvgIcon';\n\n/**\n * @ignore - internal component.\n */\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nexport default createSvgIcon( /*#__PURE__*/_jsx(\"path\", {\n  d: \"M6 10c-1.1 0-2 .9-2 2s.9 2 2 2 2-.9 2-2-.9-2-2-2zm12 0c-1.1 0-2 .9-2 2s.9 2 2 2 2-.9 2-2-.9-2-2-2zm-6 0c-1.1 0-2 .9-2 2s.9 2 2 2 2-.9 2-2-.9-2-2-2z\"\n}), 'MoreHoriz');",
         "import _extends from \"@babel/runtime/helpers/esm/extends\";\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport { emphasize } from '@mui/system';\nimport styled from '../styles/styled';\nimport MoreHorizIcon from '../internal/svg-icons/MoreHoriz';\nimport ButtonBase from '../ButtonBase';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst BreadcrumbCollapsedButton = styled(ButtonBase)(({\n  theme\n}) => _extends({\n  display: 'flex',\n  marginLeft: `calc(${theme.spacing(1)} * 0.5)`,\n  marginRight: `calc(${theme.spacing(1)} * 0.5)`\n}, theme.palette.mode === 'light' ? {\n  backgroundColor: theme.palette.grey[100],\n  color: theme.palette.grey[700]\n} : {\n  backgroundColor: theme.palette.grey[700],\n  color: theme.palette.grey[100]\n}, {\n  borderRadius: 2,\n  '&:hover, &:focus': _extends({}, theme.palette.mode === 'light' ? {\n    backgroundColor: theme.palette.grey[200]\n  } : {\n    backgroundColor: theme.palette.grey[600]\n  }),\n  '&:active': _extends({\n    boxShadow: theme.shadows[0]\n  }, theme.palette.mode === 'light' ? {\n    backgroundColor: emphasize(theme.palette.grey[200], 0.12)\n  } : {\n    backgroundColor: emphasize(theme.palette.grey[600], 0.12)\n  })\n}));\nconst BreadcrumbCollapsedIcon = styled(MoreHorizIcon)({\n  width: 24,\n  height: 16\n});\n\n/**\n * @ignore - internal component.\n */\nfunction BreadcrumbCollapsed(props) {\n  const ownerState = props;\n  return /*#__PURE__*/_jsx(\"li\", {\n    children: /*#__PURE__*/_jsx(BreadcrumbCollapsedButton, _extends({\n      focusRipple: true\n    }, props, {\n      ownerState: ownerState,\n      children: /*#__PURE__*/_jsx(BreadcrumbCollapsedIcon, {\n        ownerState: ownerState\n      })\n    }))\n  });\n}\nprocess.env.NODE_ENV !== \"production\" ? BreadcrumbCollapsed.propTypes = {\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.object\n} : void 0;\nexport default BreadcrumbCollapsed;",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getBreadcrumbsUtilityClass(slot) {\n  return generateUtilityClass('MuiBreadcrumbs', slot);\n}\nconst breadcrumbsClasses = generateUtilityClasses('MuiBreadcrumbs', ['root', 'ol', 'li', 'separator']);\nexport default breadcrumbsClasses;",
         "import _extends from \"@babel/runtime/helpers/esm/extends\";\nimport _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nconst _excluded = [\"children\", \"className\", \"component\", \"expandText\", \"itemsAfterCollapse\", \"itemsBeforeCollapse\", \"maxItems\", \"separator\"];\nimport * as React from 'react';\nimport { isFragment } from 'react-is';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { integerPropType } from '@mui/utils';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport styled from '../styles/styled';\nimport useThemeProps from '../styles/useThemeProps';\nimport Typography from '../Typography';\nimport BreadcrumbCollapsed from './BreadcrumbCollapsed';\nimport breadcrumbsClasses, { getBreadcrumbsUtilityClass } from './breadcrumbsClasses';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst useUtilityClasses = ownerState => {\n  const {\n    classes\n  } = ownerState;\n  const slots = {\n    root: ['root'],\n    li: ['li'],\n    ol: ['ol'],\n    separator: ['separator']\n  };\n  return composeClasses(slots, getBreadcrumbsUtilityClass, classes);\n};\nconst BreadcrumbsRoot = styled(Typography, {\n  name: 'MuiBreadcrumbs',\n  slot: 'Root',\n  overridesResolver: (props, styles) => {\n    return [{\n      [`& .${breadcrumbsClasses.li}`]: styles.li\n    }, styles.root];\n  }\n})({});\nconst BreadcrumbsOl = styled('ol', {\n  name: 'MuiBreadcrumbs',\n  slot: 'Ol',\n  overridesResolver: (props, styles) => styles.ol\n})({\n  display: 'flex',\n  flexWrap: 'wrap',\n  alignItems: 'center',\n  padding: 0,\n  margin: 0,\n  listStyle: 'none'\n});\nconst BreadcrumbsSeparator = styled('li', {\n  name: 'MuiBreadcrumbs',\n  slot: 'Separator',\n  overridesResolver: (props, styles) => styles.separator\n})({\n  display: 'flex',\n  userSelect: 'none',\n  marginLeft: 8,\n  marginRight: 8\n});\nfunction insertSeparators(items, className, separator, ownerState) {\n  return items.reduce((acc, current, index) => {\n    if (index < items.length - 1) {\n      acc = acc.concat(current, /*#__PURE__*/_jsx(BreadcrumbsSeparator, {\n        \"aria-hidden\": true,\n        className: className,\n        ownerState: ownerState,\n        children: separator\n      }, `separator-${index}`));\n    } else {\n      acc.push(current);\n    }\n    return acc;\n  }, []);\n}\nconst Breadcrumbs = /*#__PURE__*/React.forwardRef(function Breadcrumbs(inProps, ref) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiBreadcrumbs'\n  });\n  const {\n      children,\n      className,\n      component = 'nav',\n      expandText = 'Show path',\n      itemsAfterCollapse = 1,\n      itemsBeforeCollapse = 1,\n      maxItems = 8,\n      separator = '/'\n    } = props,\n    other = _objectWithoutPropertiesLoose(props, _excluded);\n  const [expanded, setExpanded] = React.useState(false);\n  const ownerState = _extends({}, props, {\n    component,\n    expanded,\n    expandText,\n    itemsAfterCollapse,\n    itemsBeforeCollapse,\n    maxItems,\n    separator\n  });\n  const classes = useUtilityClasses(ownerState);\n  const listRef = React.useRef(null);\n  const renderItemsBeforeAndAfter = allItems => {\n    const handleClickExpand = () => {\n      setExpanded(true);\n\n      // The clicked element received the focus but gets removed from the DOM.\n      // Let's keep the focus in the component after expanding.\n      // Moving it to the <ol> or <nav> does not cause any announcement in NVDA.\n      // By moving it to some link/button at least we have some announcement.\n      const focusable = listRef.current.querySelector('a[href],button,[tabindex]');\n      if (focusable) {\n        focusable.focus();\n      }\n    };\n\n    // This defends against someone passing weird input, to ensure that if all\n    // items would be shown anyway, we just show all items without the EllipsisItem\n    if (itemsBeforeCollapse + itemsAfterCollapse >= allItems.length) {\n      if (process.env.NODE_ENV !== 'production') {\n        console.error(['MUI: You have provided an invalid combination of props to the Breadcrumbs.', `itemsAfterCollapse={${itemsAfterCollapse}} + itemsBeforeCollapse={${itemsBeforeCollapse}} >= maxItems={${maxItems}}`].join('\\n'));\n      }\n      return allItems;\n    }\n    return [...allItems.slice(0, itemsBeforeCollapse), /*#__PURE__*/_jsx(BreadcrumbCollapsed, {\n      \"aria-label\": expandText,\n      onClick: handleClickExpand\n    }, \"ellipsis\"), ...allItems.slice(allItems.length - itemsAfterCollapse, allItems.length)];\n  };\n  const allItems = React.Children.toArray(children).filter(child => {\n    if (process.env.NODE_ENV !== 'production') {\n      if (isFragment(child)) {\n        console.error([\"MUI: The Breadcrumbs component doesn't accept a Fragment as a child.\", 'Consider providing an array instead.'].join('\\n'));\n      }\n    }\n    return /*#__PURE__*/React.isValidElement(child);\n  }).map((child, index) => /*#__PURE__*/_jsx(\"li\", {\n    className: classes.li,\n    children: child\n  }, `child-${index}`));\n  return /*#__PURE__*/_jsx(BreadcrumbsRoot, _extends({\n    ref: ref,\n    component: component,\n    color: \"text.secondary\",\n    className: clsx(classes.root, className),\n    ownerState: ownerState\n  }, other, {\n    children: /*#__PURE__*/_jsx(BreadcrumbsOl, {\n      className: classes.ol,\n      ref: listRef,\n      ownerState: ownerState,\n      children: insertSeparators(expanded || maxItems && allItems.length <= maxItems ? allItems : renderItemsBeforeAndAfter(allItems), classes.separator, separator, ownerState)\n    })\n  }));\n});\nprocess.env.NODE_ENV !== \"production\" ? Breadcrumbs.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * The content of the component.\n   */\n  children: PropTypes.node,\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n  /**\n   * The component used for the root node.\n   * Either a string to use a HTML element or a component.\n   */\n  component: PropTypes.elementType,\n  /**\n   * Override the default label for the expand button.\n   *\n   * For localization purposes, you can use the provided [translations](/material-ui/guides/localization/).\n   * @default 'Show path'\n   */\n  expandText: PropTypes.string,\n  /**\n   * If max items is exceeded, the number of items to show after the ellipsis.\n   * @default 1\n   */\n  itemsAfterCollapse: integerPropType,\n  /**\n   * If max items is exceeded, the number of items to show before the ellipsis.\n   * @default 1\n   */\n  itemsBeforeCollapse: integerPropType,\n  /**\n   * Specifies the maximum number of breadcrumbs to display. When there are more\n   * than the maximum number, only the first `itemsBeforeCollapse` and last `itemsAfterCollapse`\n   * will be shown, with an ellipsis in between.\n   * @default 8\n   */\n  maxItems: integerPropType,\n  /**\n   * Custom separator node.\n   * @default '/'\n   */\n  separator: PropTypes.node,\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object])\n} : void 0;\nexport default Breadcrumbs;",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getLinkUtilityClass(slot) {\n  return generateUtilityClass('MuiLink', slot);\n}\nconst linkClasses = generateUtilityClasses('MuiLink', ['root', 'underlineNone', 'underlineHover', 'underlineAlways', 'button', 'focusVisible']);\nexport default linkClasses;",
         "import { alpha, getPath } from '@mui/system';\nexport const colorTransformations = {\n  primary: 'primary.main',\n  textPrimary: 'text.primary',\n  secondary: 'secondary.main',\n  textSecondary: 'text.secondary',\n  error: 'error.main'\n};\nconst transformDeprecatedColors = color => {\n  return colorTransformations[color] || color;\n};\nconst getTextDecoration = ({\n  theme,\n  ownerState\n}) => {\n  const transformedColor = transformDeprecatedColors(ownerState.color);\n  const color = getPath(theme, `palette.${transformedColor}`, false) || ownerState.color;\n  const channelColor = getPath(theme, `palette.${transformedColor}Channel`);\n  if ('vars' in theme && channelColor) {\n    return `rgba(${channelColor} / 0.4)`;\n  }\n  return alpha(color, 0.4);\n};\nexport default getTextDecoration;",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"className\", \"color\", \"component\", \"onBlur\", \"onFocus\", \"TypographyClasses\", \"underline\", \"variant\", \"sx\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { elementTypeAcceptingRef } from '@mui/utils';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport capitalize from '../utils/capitalize';\nimport styled from '../styles/styled';\nimport useThemeProps from '../styles/useThemeProps';\nimport useIsFocusVisible from '../utils/useIsFocusVisible';\nimport useForkRef from '../utils/useForkRef';\nimport Typography from '../Typography';\nimport linkClasses, { getLinkUtilityClass } from './linkClasses';\nimport getTextDecoration, { colorTransformations } from './getTextDecoration';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst useUtilityClasses = ownerState => {\n  const {\n    classes,\n    component,\n    focusVisible,\n    underline\n  } = ownerState;\n  const slots = {\n    root: ['root', `underline${capitalize(underline)}`, component === 'button' && 'button', focusVisible && 'focusVisible']\n  };\n  return composeClasses(slots, getLinkUtilityClass, classes);\n};\nconst LinkRoot = styled(Typography, {\n  name: 'MuiLink',\n  slot: 'Root',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.root, styles[`underline${capitalize(ownerState.underline)}`], ownerState.component === 'button' && styles.button];\n  }\n})(({\n  theme,\n  ownerState\n}) => {\n  return _extends({}, ownerState.underline === 'none' && {\n    textDecoration: 'none'\n  }, ownerState.underline === 'hover' && {\n    textDecoration: 'none',\n    '&:hover': {\n      textDecoration: 'underline'\n    }\n  }, ownerState.underline === 'always' && _extends({\n    textDecoration: 'underline'\n  }, ownerState.color !== 'inherit' && {\n    textDecorationColor: getTextDecoration({\n      theme,\n      ownerState\n    })\n  }, {\n    '&:hover': {\n      textDecorationColor: 'inherit'\n    }\n  }), ownerState.component === 'button' && {\n    position: 'relative',\n    WebkitTapHighlightColor: 'transparent',\n    backgroundColor: 'transparent',\n    // Reset default value\n    // We disable the focus ring for mouse, touch and keyboard users.\n    outline: 0,\n    border: 0,\n    margin: 0,\n    // Remove the margin in Safari\n    borderRadius: 0,\n    padding: 0,\n    // Remove the padding in Firefox\n    cursor: 'pointer',\n    userSelect: 'none',\n    verticalAlign: 'middle',\n    MozAppearance: 'none',\n    // Reset\n    WebkitAppearance: 'none',\n    // Reset\n    '&::-moz-focus-inner': {\n      borderStyle: 'none' // Remove Firefox dotted outline.\n    },\n\n    [`&.${linkClasses.focusVisible}`]: {\n      outline: 'auto'\n    }\n  });\n});\nconst Link = /*#__PURE__*/React.forwardRef(function Link(inProps, ref) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiLink'\n  });\n  const {\n      className,\n      color = 'primary',\n      component = 'a',\n      onBlur,\n      onFocus,\n      TypographyClasses,\n      underline = 'always',\n      variant = 'inherit',\n      sx\n    } = props,\n    other = _objectWithoutPropertiesLoose(props, _excluded);\n  const {\n    isFocusVisibleRef,\n    onBlur: handleBlurVisible,\n    onFocus: handleFocusVisible,\n    ref: focusVisibleRef\n  } = useIsFocusVisible();\n  const [focusVisible, setFocusVisible] = React.useState(false);\n  const handlerRef = useForkRef(ref, focusVisibleRef);\n  const handleBlur = event => {\n    handleBlurVisible(event);\n    if (isFocusVisibleRef.current === false) {\n      setFocusVisible(false);\n    }\n    if (onBlur) {\n      onBlur(event);\n    }\n  };\n  const handleFocus = event => {\n    handleFocusVisible(event);\n    if (isFocusVisibleRef.current === true) {\n      setFocusVisible(true);\n    }\n    if (onFocus) {\n      onFocus(event);\n    }\n  };\n  const ownerState = _extends({}, props, {\n    color,\n    component,\n    focusVisible,\n    underline,\n    variant\n  });\n  const classes = useUtilityClasses(ownerState);\n  return /*#__PURE__*/_jsx(LinkRoot, _extends({\n    color: color,\n    className: clsx(classes.root, className),\n    classes: TypographyClasses,\n    component: component,\n    onBlur: handleBlur,\n    onFocus: handleFocus,\n    ref: handlerRef,\n    ownerState: ownerState,\n    variant: variant,\n    sx: [...(!Object.keys(colorTransformations).includes(color) ? [{\n      color\n    }] : []), ...(Array.isArray(sx) ? sx : [sx])]\n  }, other));\n});\nprocess.env.NODE_ENV !== \"production\" ? Link.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * The content of the component.\n   */\n  children: PropTypes.node,\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n  /**\n   * The color of the link.\n   * @default 'primary'\n   */\n  color: PropTypes /* @typescript-to-proptypes-ignore */.any,\n  /**\n   * The component used for the root node.\n   * Either a string to use a HTML element or a component.\n   */\n  component: elementTypeAcceptingRef,\n  /**\n   * @ignore\n   */\n  onBlur: PropTypes.func,\n  /**\n   * @ignore\n   */\n  onFocus: PropTypes.func,\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object]),\n  /**\n   * `classes` prop applied to the [`Typography`](/material-ui/api/typography/) element.\n   */\n  TypographyClasses: PropTypes.object,\n  /**\n   * Controls when the link should have an underline.\n   * @default 'always'\n   */\n  underline: PropTypes.oneOf(['always', 'hover', 'none']),\n  /**\n   * Applies the theme typography styles.\n   * @default 'inherit'\n   */\n  variant: PropTypes /* @typescript-to-proptypes-ignore */.oneOfType([PropTypes.oneOf(['body1', 'body2', 'button', 'caption', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'inherit', 'overline', 'subtitle1', 'subtitle2']), PropTypes.string])\n} : void 0;\nexport default Link;",
@@ -12597,25 +12600,25 @@
         "import React, { useState, useRef, useCallback, useEffect } from 'react';\nimport loader from '@monaco-editor/loader';\n\nimport MonacoContainer from '../MonacoContainer';\nimport useMount from '../hooks/useMount';\nimport useUpdate from '../hooks/useUpdate';\nimport { noop, getOrCreateModel } from '../utils';\nimport { type DiffEditorProps, type MonacoDiffEditor } from './types';\nimport { type Monaco } from '..';\n\nfunction DiffEditor({\n  original,\n  modified,\n  language,\n  originalLanguage,\n  modifiedLanguage,\n  originalModelPath,\n  modifiedModelPath,\n  keepCurrentOriginalModel = false,\n  keepCurrentModifiedModel = false,\n  theme = 'light',\n  loading = 'Loading...',\n  options = {},\n  height = '100%',\n  width = '100%',\n  className,\n  wrapperProps = {},\n  beforeMount = noop,\n  onMount = noop,\n}: DiffEditorProps) {\n  const [isEditorReady, setIsEditorReady] = useState(false);\n  const [isMonacoMounting, setIsMonacoMounting] = useState(true);\n  const editorRef = useRef<MonacoDiffEditor | null>(null);\n  const monacoRef = useRef<Monaco | null>(null);\n  const containerRef = useRef<HTMLDivElement>(null);\n  const onMountRef = useRef(onMount);\n  const beforeMountRef = useRef(beforeMount);\n  const preventCreation = useRef(false);\n\n  useMount(() => {\n    const cancelable = loader.init();\n\n    cancelable\n      .then((monaco) => (monacoRef.current = monaco) && setIsMonacoMounting(false))\n      .catch(\n        (error) =>\n          error?.type !== 'cancelation' && console.error('Monaco initialization: error:', error),\n      );\n\n    return () => (editorRef.current ? disposeEditor() : cancelable.cancel());\n  });\n\n  useUpdate(\n    () => {\n      const modifiedEditor = editorRef.current!.getModifiedEditor();\n      if (modifiedEditor.getOption(monacoRef.current!.editor.EditorOption.readOnly)) {\n        modifiedEditor.setValue(modified || '');\n      } else {\n        if (modified !== modifiedEditor.getValue()) {\n          modifiedEditor.executeEdits('', [\n            {\n              range: modifiedEditor.getModel()!.getFullModelRange(),\n              text: modified || '',\n              forceMoveMarkers: true,\n            },\n          ]);\n\n          modifiedEditor.pushUndoStop();\n        }\n      }\n    },\n    [modified],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      editorRef.current?.getModel()?.original.setValue(original || '');\n    },\n    [original],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      const { original, modified } = editorRef.current!.getModel()!;\n\n      monacoRef.current!.editor.setModelLanguage(original, originalLanguage || language || 'text');\n      monacoRef.current!.editor.setModelLanguage(modified, modifiedLanguage || language || 'text');\n    },\n    [language, originalLanguage, modifiedLanguage],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      monacoRef.current?.editor.setTheme(theme);\n    },\n    [theme],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      editorRef.current?.updateOptions(options);\n    },\n    [options],\n    isEditorReady,\n  );\n\n  const setModels = useCallback(() => {\n    if (!monacoRef.current) return;\n    beforeMountRef.current(monacoRef.current);\n    const originalModel = getOrCreateModel(\n      monacoRef.current,\n      original || '',\n      originalLanguage || language || 'text',\n      originalModelPath || '',\n    );\n\n    const modifiedModel = getOrCreateModel(\n      monacoRef.current,\n      modified || '',\n      modifiedLanguage || language || 'text',\n      modifiedModelPath || '',\n    );\n\n    editorRef.current?.setModel({\n      original: originalModel,\n      modified: modifiedModel,\n    });\n  }, [\n    language,\n    modified,\n    modifiedLanguage,\n    original,\n    originalLanguage,\n    originalModelPath,\n    modifiedModelPath,\n  ]);\n\n  const createEditor = useCallback(() => {\n    if (!preventCreation.current && containerRef.current) {\n      editorRef.current = monacoRef.current!.editor.createDiffEditor(containerRef.current, {\n        automaticLayout: true,\n        ...options,\n      });\n\n      setModels();\n\n      monacoRef.current?.editor.setTheme(theme);\n\n      setIsEditorReady(true);\n      preventCreation.current = true;\n    }\n  }, [options, theme, setModels]);\n\n  useEffect(() => {\n    if (isEditorReady) {\n      onMountRef.current(editorRef.current!, monacoRef.current!);\n    }\n  }, [isEditorReady]);\n\n  useEffect(() => {\n    !isMonacoMounting && !isEditorReady && createEditor();\n  }, [isMonacoMounting, isEditorReady, createEditor]);\n\n  useUpdate(\n    () => {\n      if (editorRef.current && monacoRef.current) {\n        const originalEditor = editorRef.current.getOriginalEditor();\n        const model = getOrCreateModel(\n          monacoRef.current,\n          original || '',\n          originalLanguage || language || 'text',\n          originalModelPath || '',\n        );\n\n        if (model !== originalEditor.getModel()) {\n          originalEditor.setModel(model);\n        }\n      }\n    },\n    [originalModelPath],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      if (editorRef.current && monacoRef.current) {\n        const modifiedEditor = editorRef.current.getModifiedEditor();\n        const model = getOrCreateModel(\n          monacoRef.current,\n          modified || '',\n          modifiedLanguage || language || 'text',\n          modifiedModelPath || '',\n        );\n\n        if (model !== modifiedEditor.getModel()) {\n          modifiedEditor.setModel(model);\n        }\n      }\n    },\n    [modifiedModelPath],\n    isEditorReady,\n  );\n\n  function disposeEditor() {\n    const models = editorRef.current?.getModel();\n\n    if (!keepCurrentOriginalModel) {\n      models?.original?.dispose();\n    }\n\n    if (!keepCurrentModifiedModel) {\n      models?.modified?.dispose();\n    }\n\n    editorRef.current?.dispose();\n  }\n\n  return (\n    <MonacoContainer\n      width={width}\n      height={height}\n      isEditorReady={isEditorReady}\n      loading={loading}\n      _ref={containerRef}\n      className={className}\n      wrapperProps={wrapperProps}\n    />\n  );\n}\n\nexport default DiffEditor;\n",
         "import { memo } from 'react';\n\nimport DiffEditor from './DiffEditor';\n\nexport * from './types';\n\nexport default memo(DiffEditor);\n",
         "import { useEffect, useRef } from 'react';\n\nfunction usePrevious<T>(value: T) {\n  const ref = useRef<T>();\n\n  useEffect(() => {\n    ref.current = value;\n  }, [value]);\n\n  return ref.current;\n}\n\nexport default usePrevious;\n",
         "import React, { useState, useEffect, useRef, useCallback } from 'react';\nimport loader from '@monaco-editor/loader';\nimport useMount from '../hooks/useMount';\nimport useUpdate from '../hooks/useUpdate';\nimport usePrevious from '../hooks/usePrevious';\nimport { type IDisposable, type editor } from 'monaco-editor';\nimport { noop, getOrCreateModel } from '../utils';\nimport { type EditorProps } from './types';\nimport { type Monaco } from '..';\nimport MonacoContainer from '../MonacoContainer';\n\nconst viewStates = new Map();\n\nfunction Editor({\n  defaultValue,\n  defaultLanguage,\n  defaultPath,\n  value,\n  language,\n  path,\n  /* === */\n  theme = 'light',\n  line,\n  loading = 'Loading...',\n  options = {},\n  overrideServices = {},\n  saveViewState = true,\n  keepCurrentModel = false,\n  /* === */\n  width = '100%',\n  height = '100%',\n  className,\n  wrapperProps = {},\n  /* === */\n  beforeMount = noop,\n  onMount = noop,\n  onChange,\n  onValidate = noop,\n}: EditorProps) {\n  const [isEditorReady, setIsEditorReady] = useState(false);\n  const [isMonacoMounting, setIsMonacoMounting] = useState(true);\n  const monacoRef = useRef<Monaco | null>(null);\n  const editorRef = useRef<editor.IStandaloneCodeEditor | null>(null);\n  const containerRef = useRef<HTMLDivElement>(null);\n  const onMountRef = useRef(onMount);\n  const beforeMountRef = useRef(beforeMount);\n  const subscriptionRef = useRef<IDisposable>();\n  const valueRef = useRef(value);\n  const previousPath = usePrevious(path);\n  const preventCreation = useRef(false);\n  const preventTriggerChangeEvent = useRef<boolean>(false);\n\n  useMount(() => {\n    const cancelable = loader.init();\n\n    cancelable\n      .then((monaco) => (monacoRef.current = monaco) && setIsMonacoMounting(false))\n      .catch(\n        (error) =>\n          error?.type !== 'cancelation' && console.error('Monaco initialization: error:', error),\n      );\n\n    return () => (editorRef.current ? disposeEditor() : cancelable.cancel());\n  });\n\n  useUpdate(\n    () => {\n      const model = getOrCreateModel(\n        monacoRef.current!,\n        defaultValue || value || '',\n        defaultLanguage || language || '',\n        path || defaultPath || '',\n      );\n\n      if (model !== editorRef.current?.getModel()) {\n        if (saveViewState) viewStates.set(previousPath, editorRef.current?.saveViewState());\n        editorRef.current?.setModel(model);\n        if (saveViewState) editorRef.current?.restoreViewState(viewStates.get(path));\n      }\n    },\n    [path],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      editorRef.current?.updateOptions(options);\n    },\n    [options],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      if (!editorRef.current || value === undefined) return;\n      if (editorRef.current.getOption(monacoRef.current!.editor.EditorOption.readOnly)) {\n        editorRef.current.setValue(value);\n      } else if (value !== editorRef.current.getValue()) {\n        preventTriggerChangeEvent.current = true;\n        editorRef.current.executeEdits('', [\n          {\n            range: editorRef.current.getModel()!.getFullModelRange(),\n            text: value,\n            forceMoveMarkers: true,\n          },\n        ]);\n\n        editorRef.current.pushUndoStop();\n        preventTriggerChangeEvent.current = false;\n      }\n    },\n    [value],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      const model = editorRef.current?.getModel();\n      if (model && language) monacoRef.current?.editor.setModelLanguage(model, language);\n    },\n    [language],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      // reason for undefined check: https://github.com/suren-atoyan/monaco-react/pull/188\n      if (line !== undefined) {\n        editorRef.current?.revealLine(line);\n      }\n    },\n    [line],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      monacoRef.current?.editor.setTheme(theme);\n    },\n    [theme],\n    isEditorReady,\n  );\n\n  const createEditor = useCallback(() => {\n    if (!containerRef.current || !monacoRef.current) return;\n    if (!preventCreation.current) {\n      beforeMountRef.current(monacoRef.current);\n      const autoCreatedModelPath = path || defaultPath;\n\n      const defaultModel = getOrCreateModel(\n        monacoRef.current,\n        value || defaultValue || '',\n        defaultLanguage || language || '',\n        autoCreatedModelPath || '',\n      );\n\n      editorRef.current = monacoRef.current?.editor.create(\n        containerRef.current,\n        {\n          model: defaultModel,\n          automaticLayout: true,\n          ...options,\n        },\n        overrideServices,\n      );\n\n      saveViewState && editorRef.current.restoreViewState(viewStates.get(autoCreatedModelPath));\n\n      monacoRef.current.editor.setTheme(theme);\n\n      setIsEditorReady(true);\n      preventCreation.current = true;\n    }\n  }, [\n    defaultValue,\n    defaultLanguage,\n    defaultPath,\n    value,\n    language,\n    path,\n    options,\n    overrideServices,\n    saveViewState,\n    theme,\n  ]);\n\n  useEffect(() => {\n    if (isEditorReady) {\n      onMountRef.current(editorRef.current!, monacoRef.current!);\n    }\n  }, [isEditorReady]);\n\n  useEffect(() => {\n    !isMonacoMounting && !isEditorReady && createEditor();\n  }, [isMonacoMounting, isEditorReady, createEditor]);\n\n  // subscription\n  // to avoid unnecessary updates (attach - dispose listener) in subscription\n  valueRef.current = value;\n\n  // onChange\n  useEffect(() => {\n    if (isEditorReady && onChange) {\n      subscriptionRef.current?.dispose();\n      subscriptionRef.current = editorRef.current?.onDidChangeModelContent((event) => {\n        if (!preventTriggerChangeEvent.current) {\n          onChange(editorRef.current!.getValue(), event);\n        }\n      });\n    }\n  }, [isEditorReady, onChange]);\n\n  // onValidate\n  useEffect(() => {\n    if (isEditorReady) {\n      const changeMarkersListener = monacoRef.current!.editor.onDidChangeMarkers((uris) => {\n        const editorUri = editorRef.current!.getModel()?.uri;\n\n        if (editorUri) {\n          const currentEditorHasMarkerChanges = uris.find((uri) => uri.path === editorUri.path);\n          if (currentEditorHasMarkerChanges) {\n            const markers = monacoRef.current!.editor.getModelMarkers({\n              resource: editorUri,\n            });\n            onValidate?.(markers);\n          }\n        }\n      });\n\n      return () => {\n        changeMarkersListener?.dispose();\n      };\n    }\n    return () => {\n      // eslint happy\n    };\n  }, [isEditorReady, onValidate]);\n\n  function disposeEditor() {\n    subscriptionRef.current?.dispose();\n\n    if (keepCurrentModel) {\n      saveViewState && viewStates.set(path, editorRef.current!.saveViewState());\n    } else {\n      editorRef.current!.getModel()?.dispose();\n    }\n\n    editorRef.current!.dispose();\n  }\n\n  return (\n    <MonacoContainer\n      width={width}\n      height={height}\n      isEditorReady={isEditorReady}\n      loading={loading}\n      _ref={containerRef}\n      className={className}\n      wrapperProps={wrapperProps}\n    />\n  );\n}\n\nexport default Editor;\n",
         "import loader from '@monaco-editor/loader';\nexport { loader };\n\nimport DiffEditor from './DiffEditor';\nexport * from './DiffEditor/types';\nexport { DiffEditor };\n\nimport useMonaco from './hooks/useMonaco';\nexport { useMonaco };\n\nimport Editor from './Editor';\nexport * from './Editor/types';\nexport { Editor };\nexport default Editor;\n\n// Monaco\nimport type * as monaco from 'monaco-editor/esm/vs/editor/editor.api';\nexport type Monaco = typeof monaco;\n\n// Default themes\nexport type Theme = 'vs-dark' | 'light';\n",
         "import { memo } from 'react';\n\nimport Editor from './Editor';\n\nexport * from './types';\n\nexport default memo(Editor);\n",
         "import Button from \"@mui/material/Button\"\nimport Dialog from \"@mui/material/Dialog\"\nimport DialogActions from \"@mui/material/DialogActions\"\nimport DialogContent from \"@mui/material/DialogContent\"\nimport DialogTitle from \"@mui/material/DialogTitle\"\nimport FormControl from \"@mui/material/FormControl\"\nimport TextField from \"@mui/material/TextField\"\nimport { useEffect, useState } from \"react\"\nimport { WorkflowSystemComponent } from \"types/WorkflowTypes\"\n\nexport default function OverviewComponentEditorDialog(props: any)\n{\n    const [dialogOpen, setDialogOpen] = useState(false);\n    const [component, setComponent] = useState<WorkflowSystemComponent>(null);\n    const handleDialogSave = () => {\n        setDialogOpen(false);\n        props.onClose(component,\"save\");\n    };\n    const handleDialogCancel = () => {\n        setDialogOpen(false);\n        props.onClose(component,\"cancel\");\n    };\n    const handleDelete = () => {\n        setDialogOpen(false);\n        props.onClose(component,\"delete\");\n    };\n    const handleStepConfigChange = (name: string, value: any) => {\n        console.log('handleComponentConfigChange')\n        console.dir(component);\n        let updComponent = Object.assign({},component);\n        updComponent[name] = value;\n        console.log(\"Updateed component\")\n        console.dir(updComponent);\n        setComponent(updComponent);\n    }\n    useEffect(() => {\n        if (props.open){\n            setDialogOpen(true);\n            setComponent(props.component);\n            console.dir(props.component);\n        }\n      }, [props.open]);\n\n\n\nreturn (\n<Dialog open={dialogOpen} onClose={handleDialogCancel}>\n<DialogTitle>Component editor</DialogTitle>\n<DialogContent>\n  <FormControl sx={{ width: 300 }} >\n    <TextField sx={{ marginTop: 1 }} id=\"step-config-id\" fullWidth label=\"Component id\" size='small' variant=\"outlined\" value={component?.id} onChange={(event) => { handleStepConfigChange(\"id\", event.target.value) }} />\n    <TextField sx={{ marginTop: 1 }} id=\"step-config-label\" fullWidth label=\"Label\" size='small' variant=\"outlined\" value={component?.label} onChange={(event) => { handleStepConfigChange(\"label\", event.target.value) }} />\n    <TextField sx={{ marginTop: 1 }} id=\"step-config-descr\" fullWidth label=\"Description\" size='small' variant=\"outlined\" value={component?.description} onChange={(event) => { handleStepConfigChange(\"description\", event.target.value) }} />\n  </FormControl>\n</DialogContent>\n<DialogActions>\n  <Button variant=\"outlined\" size=\"small\" onClick={handleDialogSave}>Save</Button>\n  <Button variant=\"outlined\" size=\"small\" onClick={handleDialogCancel}>Cancel</Button>\n  <Button variant=\"outlined\" size=\"small\" color=\"error\" onClick={handleDelete}>Delete</Button>\n</DialogActions>\n</Dialog>\n)\n}\n",
-        "import Button from \"@mui/material/Button\"\nimport Checkbox from \"@mui/material/Checkbox\"\nimport { red } from \"@mui/material/colors\"\nimport Dialog from \"@mui/material/Dialog\"\nimport DialogActions from \"@mui/material/DialogActions\"\nimport DialogContent from \"@mui/material/DialogContent\"\nimport DialogTitle from \"@mui/material/DialogTitle\"\nimport FormControl from \"@mui/material/FormControl\"\nimport FormControlLabel from \"@mui/material/FormControlLabel\"\nimport MenuItem from \"@mui/material/MenuItem\"\nimport Select from \"@mui/material/Select\"\nimport TextField from \"@mui/material/TextField\"\nimport { useEffect, useState } from \"react\"\nimport { WorkflowStepDefinition, WorkflowSystemComponent } from \"types/WorkflowTypes\"\nimport { getNeatApiRootUrl } from \"./Utils\"\n\nexport default function StepEditorDialog(props: any)\n{\n    const [dialogOpen, setDialogOpen] = useState(false);\n    const [selectedStep, setSelectedStep] = useState<WorkflowStepDefinition>();\n    const neatApiRootUrl = getNeatApiRootUrl();\n    const [runPayload,setRunPayload] = useState<string>(JSON.stringify({\"action\":\"approve\"}))\n\n    const handleDialogSave = () => {\n        setDialogOpen(false);\n        props.onClose(selectedStep,\"save\");\n    };\n    const handleDialogCancel = () => {\n        setDialogOpen(false);\n        props.onClose(selectedStep,\"cancel\");\n    };\n    const handleDelete = () => {\n        setDialogOpen(false);\n        props.onClose(selectedStep,\"delete\");\n    };\n\n    const handleRunCommand = () => {\n        setDialogOpen(false);\n        // send POST request to run the step\n        fetch(neatApiRootUrl +'/api/workflow/'+props.workflowName+'/http_trigger/'+selectedStep.id, { method: 'POST', body: runPayload })\n        .then(response => response.json())\n        .then(data => {\n            console.log('Success:', data);\n        }).catch((error) => {\n            console.error('Error:', error);\n        })\n        props.onClose(selectedStep,\"run\");\n    };\n\n    useEffect(() => {\n        if (props.open){\n            setDialogOpen(true);\n            setSelectedStep(props.step);\n            console.dir(props.step);\n        }\n      }, [props.open]);\n\n      const handleStepConfigChange = (name: string, value: any) => {\n        console.log('handleStepConfigChange')\n        console.dir(selectedStep);\n        let updStep= Object.assign({},selectedStep);\n\n        if (selectedStep) {\n          if (!selectedStep.params) {\n            selectedStep.params = {}\n          }\n          if (name == \"stype\") {\n            switch (value) {\n              case \"time_trigger\":\n                updStep.params = { \"interval\": \"every 60 minutes\" }\n                break;\n              case \"start_workflow_task_step\":\n                updStep.params = { \"workflow_name\": \"\", \"sync\": \"false\" }\n                break;\n            }\n            updStep[\"stype\"] = value;\n          } else {\n            switch (name) {\n              case \"time-interval\":\n                updStep.params[\"interval\"] = value;\n                break;\n              case \"workflow_name\":\n                updStep.params[\"workflow_name\"] = value;\n                break;\n              case \"workflow_sync_run_flag\":\n                value = \"false\"\n                if (value) {\n                  value = \"true\"\n                }\n                updStep.params[\"sync\"] = value;\n                break;\n              default:\n                updStep[name] = value;\n            }\n          }\n          console.log(\"rendering view\")\n        }\n        setSelectedStep(updStep);\n      }\n\n\nreturn (\n  <Dialog open={dialogOpen} onClose={handleDialogCancel}>\n        <DialogTitle>Step configurator</DialogTitle>\n        <DialogContent>\n          <FormControl sx={{ width: 300 }} >\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-id\" fullWidth label=\"Step id\" size='small' variant=\"outlined\" value={selectedStep?.id} onChange={(event) => { handleStepConfigChange(\"id\", event.target.value) }} />\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-label\" fullWidth label=\"Label\" size='small' variant=\"outlined\" value={selectedStep?.label} onChange={(event) => { handleStepConfigChange(\"label\", event.target.value) }} />\n            <Select sx={{ marginTop: 1 }}\n              id=\"step-config-stype\"\n              value={selectedStep?.stype}\n              label=\"Step type\"\n              size='small'\n              variant=\"outlined\"\n              onChange={(event) => { handleStepConfigChange(\"stype\", event.target.value) }}\n            >\n              <MenuItem value=\"pystep\">Python function</MenuItem>\n              <MenuItem value=\"http_trigger\">HTTP trigger</MenuItem>\n              <MenuItem value=\"time_trigger\">Time trigger</MenuItem>\n              <MenuItem value=\"wait_for_event\">Wait for event</MenuItem>\n              <MenuItem value=\"start_workflow_task_step\">Start workflow</MenuItem>\n            </Select>\n\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-descr\" fullWidth label=\"Description\" size='small' variant=\"outlined\" value={selectedStep?.description} onChange={(event) => { handleStepConfigChange(\"description\", event.target.value) }} />\n            {(selectedStep?.stype == \"time_trigger\") && (\n              <TextField sx={{ marginTop: 1 }} id=\"step-config-time-config\" fullWidth label=\"Time interval\" size='small' variant=\"outlined\" value={selectedStep?.params[\"interval\"]} onChange={(event) => { handleStepConfigChange(\"time-interval\", event.target.value) }} />\n            )}\n            {(selectedStep?.stype == \"start_workflow_task_step\") && (\n              <TextField sx={{ marginTop: 1 }} id=\"step-start_workflow_task_step\" fullWidth label=\"Name of the workflow\" size='small' variant=\"outlined\" value={selectedStep?.params[\"workflow_name\"]} onChange={(event) => { handleStepConfigChange(\"workflow_name\", event.target.value) }} />\n            )}\n            {(selectedStep?.stype == \"start_workflow_task_step\") && (\n              <FormControlLabel control={<Checkbox checked={selectedStep?.params[\"sync\"] == \"true\"} onChange={(event) => { handleStepConfigChange(\"workflow_sync_run_flag\", event.target.checked) }} />} label=\"Synchronous execution\" />\n            )}\n            <FormControlLabel control={<Checkbox checked={selectedStep?.enabled} onChange={(event) => { handleStepConfigChange(\"enabled\", event.target.checked) }} />} label=\"Is enabled\" />\n            <FormControlLabel control={<Checkbox checked={selectedStep?.trigger} onChange={(event) => { handleStepConfigChange(\"trigger\", event.target.checked) }} />} label=\"Is trigger\" />\n            {(selectedStep?.stype == \"http_trigger\" || selectedStep?.stype == \"wait_for_event\") && (\n              <TextField sx={{ marginTop: 1 }} value={runPayload} onChange={(event)=>setRunPayload(event.target.value)} id=\"run_payload\"> </TextField>\n            )}\n          </FormControl>\n\n        </DialogContent>\n        <DialogActions>\n          <Button variant=\"outlined\" size=\"small\" onClick={handleDialogSave}>Save</Button>\n          <Button variant=\"outlined\" size=\"small\" onClick={handleDialogCancel}>Cancel</Button>\n          <Button variant=\"outlined\" size=\"small\" color=\"error\" onClick={handleDelete} >Delete</Button>\n          {(selectedStep?.stype == \"http_trigger\" || selectedStep?.stype == \"wait_for_event\") && (\n              <Button variant=\"outlined\" size=\"small\" color=\"success\" onClick={handleRunCommand}>Run</Button>\n          )}\n\n        </DialogActions>\n      </Dialog>\n)\n}\n",
-        "import { useCallback, useRef } from 'react';\nimport ReactFlow, {\n  MiniMap,\n  Controls,\n  Background,\n  useNodesState,\n  useEdgesState,\n  addEdge,\n  Node,\n  updateEdge,\n  Panel,\n  NodeChange,\n  EdgeChange,\n} from 'reactflow';\n// \ud83d\udc47 you need to import the reactflow styles\nimport 'reactflow/dist/style.css';\nimport Button from '@mui/material/Button';\nimport { useState, useEffect } from 'react';\nimport Stack from '@mui/material/Stack';\nimport { styled } from '@mui/material/styles';\nimport Paper from '@mui/material/Paper';\nimport { UIConfig, WorkflowDefinition, WorkflowStepDefinition, WorkflowSystemComponent} from 'types/WorkflowTypes';\nimport FormControl from '@mui/material/FormControl';\nimport InputLabel from '@mui/material/InputLabel';\nimport Select, { SelectChangeEvent } from '@mui/material/Select';\nimport { Box } from '@mui/system';\nimport MenuItem from '@mui/material/MenuItem';\nimport ToggleButtonGroup from '@mui/material/ToggleButtonGroup';\nimport ToggleButton from '@mui/material/ToggleButton';\nimport { getNeatApiRootUrl, getSelectedWorkflowName, setSelectedWorkflowName } from 'components/Utils';\nimport CdfPublisher from 'components/CdfPublisher';\nimport CdfDownloader from 'components/CdfDownloader';\nimport WorkflowExecutionReport from 'components/WorkflowExecutionReport';\nimport ConfigView from './ConfigView';\nimport TransformationTable from './TransformationView';\nimport QDataTable from './ExplorerView';\nimport Editor, { DiffEditor, useMonaco, loader } from '@monaco-editor/react';\nimport OverviewComponentEditorDialog from 'components/OverviewComponentEditorDialog';\nimport StepEditorDialog from 'components/StepEditorDialog';\n\nexport interface ExecutionLog {\n  id: string;\n  state: string;\n  elapsed_time: number;\n  timestamp: string;\n  error: string;\n  output_text: string;\n  data: any;\n}\n\nexport interface WorkflowStats {\n  state: string;\n  elapsed_time: number;\n  last_error: string;\n  execution_log: ExecutionLog[];\n}\n\nconst Item = styled(Paper)(({ theme }) => ({\n  backgroundColor: theme.palette.mode === 'dark' ? '#1A2027' : '#fff',\n  ...theme.typography.body2,\n  padding: theme.spacing(1),\n  textAlign: 'left',\n  color: theme.palette.text.secondary,\n}));\n\n\n\nexport default function WorkflowView() {\n  const neatApiRootUrl = getNeatApiRootUrl();\n  const edgeUpdateSuccessful = useRef(true);\n  const [nodes, setNodes, onNodesChange] = useNodesState([]);\n  const [edges, setEdges, onEdgesChange] = useEdgesState([]);\n  const [workflowStats, setWorkflowStats] = useState<WorkflowStats>();\n  const [timerInterval, setTimerInterval] = useState(null);\n  const [workflowDefinitions, setWorkflowDefinitions] = useState<WorkflowDefinition>();\n  const [selectedWorkflow, setSelectedWorkflow] = useState<string>(getSelectedWorkflowName());\n  const [listOfWorkflows, setListOfWorkflows] = useState<string[]>([]);\n  const [viewType, setViewType] = useState<string>(\"system\");\n  const [dialogOpen, setDialogOpen] = useState(false);\n  const [openOverviewComponentEditorDialog, setOpenOverviewComponentEditorDialog] = useState(false);\n  const [selectedStep, setSelectedStep] = useState<WorkflowStepDefinition>();\n  const [selectedComponent, setSelectedComponent] = useState<WorkflowSystemComponent>();\n  const [fileContent, setFileContent] = useState('');\n\n\n  useEffect(() => {\n    loadListOfWorkflows();\n    loadWorkflowDefinitions(getSelectedWorkflowName());\n    startStatePolling();\n\n  }, []);\n\n  const fetchFileContent = async () => {\n    try {\n      var myHeaders = new Headers();\n      myHeaders.append('pragma', 'no-cache');\n      myHeaders.append('cache-control', 'no-cache');\n      const response = await fetch(neatApiRootUrl + '/data/workflows/' + selectedWorkflow + '/workflow.py', { method: \"get\", headers: myHeaders });\n      const content = await response.text();\n      setFileContent(content);\n    } catch (error) {\n      console.error('Error fetching file:', error);\n    }\n  };\n\n  useEffect(() => {\n    console.log(\"workflow definition changed\")\n    syncWorkflowDefToNodesAndEdges(viewType);\n  }, [workflowDefinitions]);\n\n  // useEffect(() => {\n  //   console.log(\"node or edge changed\")\n  //   syncNodesAndEdgesToWorkflowDef();\n  // }, [nodes, edges]);\n\n  const startStatePolling = () => {\n    if (!timerInterval) {\n      let timerInterval = setInterval(() => {\n        loadWorkflowStats();\n      }, 2000);\n      setTimerInterval(timerInterval);\n    }\n\n  }\n\n  const stopStatePolling = () => {\n    clearInterval(timerInterval);\n    // timerInterval = null;\n  }\n\n  const loadListOfWorkflows = () => {\n    const url = neatApiRootUrl + \"/api/workflow/workflows\";\n    fetch(url).then((response) => response.json()).then((data) => {\n      setListOfWorkflows(data.workflows);\n    }).catch((error) => {\n      console.error('Error:', error);\n    }).finally(() => { });\n  }\n\n  const loadWorkflowDefinitions = (workflowName: string = \"\") => {\n    if (workflowName == \"\")\n      workflowName = selectedWorkflow;\n    const url = neatApiRootUrl + \"/api/workflow/workflow-definition/\" + workflowName;\n    fetch(url).then((response) => response.json()).then((data) => {\n      const workflows = WorkflowDefinition.fromJSON(data.definition);\n      setWorkflowDefinitions(workflows);\n      // loadWorkflowStats(workflowName);\n  }).catch ((error) => {\n    console.error('Error:', error);\n  }).finally(() => { });\n}\n\nconst filterStats = (stats: WorkflowStats) => {\n  console.log(\"loadWorkflowStats\")\n  console.dir(stats)\n  // detelete all log RUNNING entries that have both RUNNING and COMPLETED entries for the same step\n  if (stats.execution_log == null)\n    return stats;\n\n  const filteredLog = stats.execution_log!.filter((log, index) => {\n    if (log.state == \"STARTED\") {\n      const nextLog = stats.execution_log[index + 1];\n      if (nextLog && nextLog.state == \"COMPLETED\" && nextLog.id == log.id)\n        return false;\n    }\n    return true;\n  })\n  stats.execution_log = filteredLog;\n  return stats;\n}\n\nconst loadWorkflowStats = (workflowName: string = \"\") => {\n  if (workflowName == \"\")\n    workflowName = selectedWorkflow;\n  const url = neatApiRootUrl + \"/api/workflow/stats/\" + workflowName;\n  fetch(url).then((response) => response.json()).then((data) => {\n\n    // const filteredStats = filterStats(data);\n    setWorkflowStats(data);\n    if (data.state == \"RUNNING\") {\n      // startStatePolling();\n    } else if (data.state == \"COMPLETED\" || data.state == \"FAILED\") {\n      // stopStatePolling();\n    }\n\n  }).catch((error) => {\n    console.error('Error:', error);\n  })\n}\n\nconst startWorkflow = () => {\n  const url = neatApiRootUrl + \"/api/workflow/start\";\n  const params = { name: selectedWorkflow, config: \"\", start_step: \"\" };\n  fetch(url, {\n    method: \"post\", body: JSON.stringify(params), headers: {\n      'Content-Type': 'application/json;charset=utf-8'\n    }\n  }).then((response) => response.json()).then((data) => {\n    console.dir(data)\n    setWorkflowStats(data);\n    startStatePolling();\n    loadWorkflowStats();\n  }).catch((error) => {\n    console.error('Error:', error);\n  })\n}\n\n\nconst saveWorkflow = () => {\n  console.dir(nodes);\n  syncNodesAndEdgesToWorkflowDef();\n  let wdef = workflowDefinitions;\n  console.dir(wdef);\n  const url = neatApiRootUrl + \"/api/workflow/workflow-definition/\" + selectedWorkflow;\n  fetch(url, {\n    method: \"post\", body: wdef.serializeToJson(), headers: {\n      'Content-Type': 'application/json;charset=utf-8'\n    }\n  }).then((response) => response.json()).then((data) => {\n    console.dir(data)\n  }\n  ).catch((error) => {\n    console.error('Error:', error);\n  })\n};\n\nconst syncNodesAndEdgesToWorkflowDef = () => {\n  if (workflowDefinitions) {\n    workflowDefinitions.updatePositions(nodes);\n    if (viewType == \"system\")\n      workflowDefinitions.updateSystemComponentTransitions(edges);\n    else\n      workflowDefinitions.updateStepTransitions(edges);\n  } else {\n    console.error(\"workflowDefinitions is null\");\n  }\n\n}\n\nconst syncWorkflowDefToNodesAndEdges = (viewType:string) => {\n  if (!workflowDefinitions)\n    return;\n  switch (viewType) {\n    case 'steps':\n      setNodes(workflowDefinitions.convertStepsToNodes());\n      setEdges(workflowDefinitions.convertStepsToEdges());\n      break;\n    case 'system':\n      setNodes(workflowDefinitions.convertSystemComponentsToNodes());\n      setEdges(workflowDefinitions.convertSystemComponentsToEdges());\n  }\n}\n\n\nconst reloadWorkflows = () => {\n  const url = neatApiRootUrl + \"/api/workflow/reload-workflows\";\n  fetch(url, {\n    method: \"post\", body: \"\", headers: {\n      'Content-Type': 'application/json;charset=utf-8'\n    }\n  }).then((response) => response.json()).then((data) => {\n    loadWorkflowDefinitions();\n  }\n  ).catch((error) => {\n    console.error('Error:', error);\n  })\n};\n\nconst handleWorkflowSelectorChange = (event: SelectChangeEvent) => {\n  console.dir(\"Workflow changed to :\" + event.target.value);\n  setSelectedWorkflowName(event.target.value);\n  setSelectedWorkflow(event.target.value);\n  loadWorkflowDefinitions(event.target.value);\n  setViewType(\"system\");\n  syncWorkflowDefToNodesAndEdges(\"system\");\n};\n\nconst handleViewTypeChange = (\n  event: React.MouseEvent<HTMLElement>,\n  newViewType: string,\n) => {\n\n  setViewType(newViewType);\n  syncWorkflowDefToNodesAndEdges(newViewType);\n  if (newViewType == \"src\") {\n    fetchFileContent();\n  }\n};\n\n\nconst onConnect = useCallback((params) => {\n  console.log('onConnect')\n  setEdges((eds) => addEdge(params, eds))\n  syncNodesAndEdgesToWorkflowDef();\n}, [setEdges]);\n\nconst onEdgeUpdateStart = useCallback(() => {\n  console.log('onEdgeUpdateStart')\n  edgeUpdateSuccessful.current = false;\n}, []);\n\nconst onEdgeUpdate = useCallback((oldEdge, newConnection) => {\n  console.log('onEdgeUpdate')\n  edgeUpdateSuccessful.current = true;\n  setEdges((els) => updateEdge(oldEdge, newConnection, els));\n}, [setEdges]);\n\nconst onEdgeUpdateEnd = useCallback((_, edge) => {\n  console.log('onEdgeUpdateEnd')\n  if (!edgeUpdateSuccessful.current) {\n    setEdges((eds) => eds.filter((e) => e.id !== edge.id));\n    syncNodesAndEdgesToWorkflowDef();\n  }\n\n  edgeUpdateSuccessful.current = true;\n}, [setEdges]);\n\nconst onNodeClick = useCallback((event, node) => {\n  console.log('onNodeClick')\n  console.dir(node);\n  handleDialogClickOpen(node.id, viewType);\n}, [workflowDefinitions, viewType]);\n\nconst onAddStep = (() => {\n  console.log('onAddStep')\n  const ui_config = new UIConfig();\n  ui_config.pos_x = 100;\n  ui_config.pos_y = 100;\n  if (viewType == \"steps\") {\n    const step = new WorkflowStepDefinition();\n    step.id = \"step_\" + Math.floor(Math.random() * 1000000);\n    step.label = \"New step\";\n    step.ui_config = ui_config;\n    workflowDefinitions.steps.push(step);\n  } else {\n    const systemComponent = new WorkflowSystemComponent();\n    systemComponent.id = \"system_comp_\" + Math.floor(Math.random() * 1000000);\n    systemComponent.label = \"New component\";\n    systemComponent.ui_config = ui_config;\n    if (workflowDefinitions.system_components == null)\n      workflowDefinitions.system_components = [];\n    workflowDefinitions.system_components.push(systemComponent);\n  }\n  syncWorkflowDefToNodesAndEdges(viewType);\n});\n\nconst handleDialogClickOpen = (id: string, viewType: string) => {\n  console.log(viewType);\n  if (viewType == \"steps\") {\n    setSelectedStep(workflowDefinitions.getStepById(id));\n    setDialogOpen(true);\n  } else {\n    setSelectedComponent(workflowDefinitions.getSystemComponentById(id));\n    setOpenOverviewComponentEditorDialog(true);\n  }\n};\n\nconst handleDialogClose = (step:WorkflowStepDefinition,action:string) => {\n  setDialogOpen(false);\n  switch (action) {\n    case \"delete\":\n      workflowDefinitions.deleteStep(selectedStep.id);\n      syncWorkflowDefToNodesAndEdges(viewType);\n      break;\n    case \"save\":\n      workflowDefinitions.updateStep(selectedStep.id, step);\n      setSelectedStep(step);\n      syncWorkflowDefToNodesAndEdges(viewType);\n      break;\n  }\n\n};\n\n\nconst onDownloadSuccess = (fileName: string, hash: string) => {\n  console.log(\"onDownloadSuccess\", fileName, hash)\n  reloadWorkflows();\n}\nconst solutionComponentEditorDialogHandler = (component: WorkflowSystemComponent,action: string) => {\n  console.log(\"OverviewComponentEditorDialogHandler\")\n  console.dir(component)\n  switch (action) {\n    case \"save\":\n      workflowDefinitions.updateSystemComponent(selectedComponent.id, component);\n      setSelectedComponent(component);\n      syncWorkflowDefToNodesAndEdges(viewType);\n      break;\n    case \"delete\":\n      workflowDefinitions.deleteSystemComponent(component.id);\n      syncWorkflowDefToNodesAndEdges(viewType);\n      break;\n  }\n  setOpenOverviewComponentEditorDialog(false);\n}\n\nconst onNodesChangeN = useCallback((nodeChanges: NodeChange[]) => {\n  // console.log('onNodesChange')\n  // console.dir(nodeChanges);\n  onNodesChange(nodeChanges);\n  syncNodesAndEdgesToWorkflowDef();\n}, [workflowDefinitions,nodes,edges]);\n\nconst onEdgesChangeN = useCallback((edgeChanges: EdgeChange[]) => {\n  console.log('onEdgesChange')\n  console.dir(edgeChanges);\n  onEdgesChange(edgeChanges);\n  syncNodesAndEdgesToWorkflowDef();\n}, [workflowDefinitions,nodes,edges]);\n\nreturn (\n  <div style={{ height: '85vh', width: '97vw' }}>\n    <Box>\n      <FormControl sx={{ width: 300, marginBottom: 2 }}>\n        <InputLabel id=\"workflowSelectorLabel\">Workflow selector</InputLabel>\n        <Select\n          labelId=\"workflowSelectorLabel\"\n          id=\"workflowSelector\"\n          value={selectedWorkflow}\n          size='small'\n          label=\"Query template\"\n          onChange={handleWorkflowSelectorChange}\n        >\n          {\n            listOfWorkflows && listOfWorkflows.map((item, i) => (\n              <MenuItem value={item} key={item}>{item} </MenuItem>\n            ))\n          }\n        </Select>\n      </FormControl>\n      <ToggleButtonGroup\n        color=\"primary\"\n        value={viewType}\n        exclusive\n        size='small'\n        sx={{ marginLeft: 2 }}\n        onChange={handleViewTypeChange}\n        aria-label=\"View type\"\n      >\n        <ToggleButton value=\"system\">Solution overview</ToggleButton>\n        <ToggleButton value=\"steps\">Workflow steps</ToggleButton>\n        <ToggleButton value=\"configurations\">Configurations</ToggleButton>\n        <ToggleButton value=\"src\">Source code</ToggleButton>\n        <ToggleButton value=\"transformations\">Transformation rules</ToggleButton>\n        <ToggleButton value=\"data_explorer\">Data explorer</ToggleButton>\n\n      </ToggleButtonGroup>\n    </Box>\n    {(viewType == \"system\" || viewType == \"steps\") && (\n      <Stack direction=\"row\" spacing={1} justifyContent=\"left\"\n        alignItems=\"left\">\n        <Item>\n          <OverviewComponentEditorDialog open={openOverviewComponentEditorDialog} component={selectedComponent} onClose={solutionComponentEditorDialogHandler} />\n          <StepEditorDialog open={dialogOpen} step={selectedStep} workflowName={selectedWorkflow} onClose={handleDialogClose} />\n          <div style={{ height: '75vh', width: '70vw' }}>\n            <ReactFlow\n              nodes={nodes}\n              edges={edges}\n              onNodeClick={onNodeClick}\n              onNodesChange={onNodesChangeN}\n              onEdgesChange={onEdgesChangeN}\n              onEdgeUpdate={onEdgeUpdate}\n              onEdgeUpdateStart={onEdgeUpdateStart}\n              onEdgeUpdateEnd={onEdgeUpdateEnd}\n              onConnect={onConnect}\n            >\n              <MiniMap />\n              <Controls />\n              <Background />\n              <Panel position=\"bottom-center\">\n              {viewType == \"system\" && (<Button variant=\"outlined\" onClick={onAddStep}>Add solution component</Button>)}\n              {viewType == \"steps\" && (<Button variant=\"outlined\" onClick={onAddStep}>Add workflow step</Button>)}\n              </Panel>\n            </ReactFlow>\n\n            <Button variant=\"outlined\" onClick={startWorkflow} sx={{ marginTop: 2, marginRight: 1 }}>Start workflow</Button>\n            <Button variant=\"outlined\" onClick={saveWorkflow} sx={{ marginTop: 2, marginRight: 1 }}>Save workflow</Button>\n            <Button variant=\"outlined\" onClick={reloadWorkflows} sx={{ marginTop: 2, marginRight: 1 }} >Reload local workflows</Button>\n            <Box sx={{ marginTop: 1, marginBottom: 1 }}>\n              <CdfPublisher type=\"workflow\" />\n              <CdfDownloader type=\"workflow-package\" onDownloadSuccess={onDownloadSuccess} />\n            </Box>\n          </div>\n\n        </Item>\n        <Item >\n          <WorkflowExecutionReport report={workflowStats} />\n        </Item>\n      </Stack>\n    )}\n    {viewType == \"configurations\" && (\n      <ConfigView></ConfigView>\n    )}\n    {viewType == \"transformations\" && (\n      <TransformationTable />\n    )}\n    {viewType == \"data_explorer\" && (\n      <QDataTable />\n    )}\n    {viewType == \"src\" && (\n      <Editor height=\"90vh\" defaultLanguage=\"python\" value={fileContent} />\n    )}\n\n  </div>\n\n\n);\n}\n",
+        "import Button from \"@mui/material/Button\"\nimport Checkbox from \"@mui/material/Checkbox\"\nimport { red } from \"@mui/material/colors\"\nimport Dialog from \"@mui/material/Dialog\"\nimport DialogActions from \"@mui/material/DialogActions\"\nimport DialogContent from \"@mui/material/DialogContent\"\nimport DialogTitle from \"@mui/material/DialogTitle\"\nimport FormControl from \"@mui/material/FormControl\"\nimport FormControlLabel from \"@mui/material/FormControlLabel\"\nimport MenuItem from \"@mui/material/MenuItem\"\nimport Select from \"@mui/material/Select\"\nimport TextField from \"@mui/material/TextField\"\nimport { useEffect, useState } from \"react\"\nimport { WorkflowStepDefinition, WorkflowSystemComponent } from \"types/WorkflowTypes\"\nimport { getNeatApiRootUrl } from \"./Utils\"\n\nexport default function StepEditorDialog(props: any)\n{\n    const [dialogOpen, setDialogOpen] = useState(false);\n    const [selectedStep, setSelectedStep] = useState<WorkflowStepDefinition>();\n    const neatApiRootUrl = getNeatApiRootUrl();\n    const [runPayload,setRunPayload] = useState<string>(JSON.stringify({\"action\":\"approve\"}))\n\n    const handleDialogSave = () => {\n        setDialogOpen(false);\n        props.onClose(selectedStep,\"save\");\n    };\n    const handleDialogCancel = () => {\n        setDialogOpen(false);\n        props.onClose(selectedStep,\"cancel\");\n    };\n    const handleDelete = () => {\n        setDialogOpen(false);\n        props.onClose(selectedStep,\"delete\");\n    };\n\n    const handleRunCommand = () => {\n        setDialogOpen(false);\n        // send POST request to run the step\n        fetch(neatApiRootUrl +'/api/workflow/'+props.workflowName+'/http_trigger/'+selectedStep.id, { method: 'POST', body: runPayload })\n        .then(response => response.json())\n        .then(data => {\n            console.log('Success:', data);\n        }).catch((error) => {\n            console.error('Error:', error);\n        })\n        props.onClose(selectedStep,\"run\");\n    };\n\n    useEffect(() => {\n        if (props.open){\n            setDialogOpen(true);\n            setSelectedStep(props.step);\n            console.dir(props.step);\n        }\n      }, [props.open]);\n\n      const handleStepConfigChange = (name: string, value: any) => {\n        console.log('handleStepConfigChange')\n        console.dir(selectedStep);\n        let updStep= Object.assign({},selectedStep);\n\n        if (selectedStep) {\n          if (!selectedStep.params) {\n            selectedStep.params = {}\n          }\n          if (name == \"stype\") {\n            switch (value) {\n              case \"time_trigger\":\n                updStep.params = { \"interval\": \"every 60 minutes\" }\n                break;\n              case \"start_workflow_task_step\":\n                updStep.params = { \"workflow_name\": \"\", \"sync\": \"false\" }\n                break;\n            }\n            updStep[\"stype\"] = value;\n          } else {\n            switch (name) {\n              case \"time-interval\":\n                updStep.params[\"interval\"] = value;\n                break;\n              case \"workflow_name\":\n                updStep.params[\"workflow_name\"] = value;\n                break;\n              case \"workflow_sync_run_flag\":\n                value = \"false\"\n                if (value) {\n                  value = \"true\"\n                }\n                updStep.params[\"sync\"] = value;\n                break;\n              default:\n                updStep[name] = value;\n            }\n          }\n          console.log(\"rendering view\")\n        }\n        setSelectedStep(updStep);\n      }\n\n\nreturn (\n  <Dialog open={dialogOpen} onClose={handleDialogCancel}>\n        <DialogTitle>Step configurator</DialogTitle>\n        <DialogContent>\n          <FormControl sx={{ width: 500 }} >\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-id\" fullWidth label=\"Step id\" size='small' variant=\"outlined\" value={selectedStep?.id} onChange={(event) => { handleStepConfigChange(\"id\", event.target.value) }} />\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-label\" fullWidth label=\"Label\" size='small' variant=\"outlined\" value={selectedStep?.label} onChange={(event) => { handleStepConfigChange(\"label\", event.target.value) }} />\n            <Select sx={{ marginTop: 1 }}\n              id=\"step-config-stype\"\n              value={selectedStep?.stype}\n              label=\"Step type\"\n              size='small'\n              variant=\"outlined\"\n              onChange={(event) => { handleStepConfigChange(\"stype\", event.target.value) }}\n            >\n              <MenuItem value=\"pystep\">Python function</MenuItem>\n              <MenuItem value=\"http_trigger\">HTTP trigger</MenuItem>\n              <MenuItem value=\"time_trigger\">Time trigger</MenuItem>\n              <MenuItem value=\"wait_for_event\">Wait for event</MenuItem>\n              <MenuItem value=\"start_workflow_task_step\">Start workflow</MenuItem>\n            </Select>\n\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-descr\" fullWidth label=\"Description\" size='small' variant=\"outlined\" value={selectedStep?.description} onChange={(event) => { handleStepConfigChange(\"description\", event.target.value) }} />\n            {(selectedStep?.stype == \"time_trigger\") && (\n              <TextField sx={{ marginTop: 1 }} id=\"step-config-time-config\" fullWidth label=\"Time interval\" size='small' variant=\"outlined\" value={selectedStep?.params[\"interval\"]} onChange={(event) => { handleStepConfigChange(\"time-interval\", event.target.value) }} />\n            )}\n            {(selectedStep?.stype == \"start_workflow_task_step\") && (\n              <TextField sx={{ marginTop: 1 }} id=\"step-start_workflow_task_step\" fullWidth label=\"Name of the workflow\" size='small' variant=\"outlined\" value={selectedStep?.params[\"workflow_name\"]} onChange={(event) => { handleStepConfigChange(\"workflow_name\", event.target.value) }} />\n            )}\n            {(selectedStep?.stype == \"start_workflow_task_step\") && (\n              <FormControlLabel control={<Checkbox checked={selectedStep?.params[\"sync\"] == \"true\"} onChange={(event) => { handleStepConfigChange(\"workflow_sync_run_flag\", event.target.checked) }} />} label=\"Synchronous execution\" />\n            )}\n            <FormControlLabel control={<Checkbox checked={selectedStep?.enabled} onChange={(event) => { handleStepConfigChange(\"enabled\", event.target.checked) }} />} label=\"Is enabled\" />\n            <FormControlLabel control={<Checkbox checked={selectedStep?.trigger} onChange={(event) => { handleStepConfigChange(\"trigger\", event.target.checked) }} />} label=\"Is trigger\" />\n\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-max-retries\" fullWidth label=\"Max retries on failure\" size='small' type=\"number\" variant=\"outlined\" value={selectedStep?.max_retries} onChange={(event) => { handleStepConfigChange(\"max_retries\", event.target.value) }} />\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-retry-delay\" fullWidth label=\"Retry delay\" size='small' variant=\"outlined\" type=\"number\" value={selectedStep?.retry_delay} onChange={(event) => { handleStepConfigChange(\"retry_delay\", event.target.value) }} />\n\n            {(selectedStep?.stype == \"http_trigger\" || selectedStep?.stype == \"wait_for_event\") && (\n              <TextField sx={{ marginTop: 1 }} value={runPayload} label=\"Run payload\" onChange={(event)=>setRunPayload(event.target.value)} id=\"run_payload\"> </TextField>\n            )}\n          </FormControl>\n\n        </DialogContent>\n        <DialogActions>\n          <Button variant=\"outlined\" size=\"small\" onClick={handleDialogSave}>Save</Button>\n          <Button variant=\"outlined\" size=\"small\" onClick={handleDialogCancel}>Cancel</Button>\n          <Button variant=\"outlined\" size=\"small\" color=\"error\" onClick={handleDelete} >Delete</Button>\n          {(selectedStep?.stype == \"http_trigger\" || selectedStep?.stype == \"wait_for_event\") && (\n              <Button variant=\"outlined\" size=\"small\" color=\"success\" onClick={handleRunCommand}>Run</Button>\n          )}\n\n        </DialogActions>\n      </Dialog>\n)\n}\n",
+        "import { useCallback, useRef } from 'react';\nimport ReactFlow, {\n  MiniMap,\n  Controls,\n  Background,\n  useNodesState,\n  useEdgesState,\n  addEdge,\n  Node,\n  updateEdge,\n  Panel,\n  NodeChange,\n  EdgeChange,\n} from 'reactflow';\n// \ud83d\udc47 you need to import the reactflow styles\nimport 'reactflow/dist/style.css';\nimport Button from '@mui/material/Button';\nimport { useState, useEffect } from 'react';\nimport Stack from '@mui/material/Stack';\nimport { styled } from '@mui/material/styles';\nimport Paper from '@mui/material/Paper';\nimport { UIConfig, WorkflowDefinition, WorkflowStepDefinition, WorkflowSystemComponent} from 'types/WorkflowTypes';\nimport FormControl from '@mui/material/FormControl';\nimport InputLabel from '@mui/material/InputLabel';\nimport Select, { SelectChangeEvent } from '@mui/material/Select';\nimport { Box } from '@mui/system';\nimport MenuItem from '@mui/material/MenuItem';\nimport ToggleButtonGroup from '@mui/material/ToggleButtonGroup';\nimport ToggleButton from '@mui/material/ToggleButton';\nimport { getNeatApiRootUrl, getSelectedWorkflowName, setSelectedWorkflowName } from 'components/Utils';\nimport CdfPublisher from 'components/CdfPublisher';\nimport CdfDownloader from 'components/CdfDownloader';\nimport WorkflowExecutionReport from 'components/WorkflowExecutionReport';\nimport ConfigView from './ConfigView';\nimport TransformationTable from './TransformationView';\nimport QDataTable from './ExplorerView';\nimport Editor, { DiffEditor, useMonaco, loader } from '@monaco-editor/react';\nimport OverviewComponentEditorDialog from 'components/OverviewComponentEditorDialog';\nimport StepEditorDialog from 'components/StepEditorDialog';\n\nexport interface ExecutionLog {\n  id: string;\n  state: string;\n  elapsed_time: number;\n  timestamp: string;\n  error: string;\n  output_text: string;\n  data: any;\n}\n\nexport interface WorkflowStats {\n  state: string;\n  elapsed_time: number;\n  last_error: string;\n  execution_log: ExecutionLog[];\n}\n\nconst Item = styled(Paper)(({ theme }) => ({\n  backgroundColor: theme.palette.mode === 'dark' ? '#1A2027' : '#fff',\n  ...theme.typography.body2,\n  padding: theme.spacing(1),\n  textAlign: 'left',\n  color: theme.palette.text.secondary,\n}));\n\n\n\nexport default function WorkflowView() {\n  const neatApiRootUrl = getNeatApiRootUrl();\n  const edgeUpdateSuccessful = useRef(true);\n  const [nodes, setNodes, onNodesChange] = useNodesState([]);\n  const [edges, setEdges, onEdgesChange] = useEdgesState([]);\n  const [workflowStats, setWorkflowStats] = useState<WorkflowStats>();\n  const [timerInterval, setTimerInterval] = useState(null);\n  const [workflowDefinitions, setWorkflowDefinitions] = useState<WorkflowDefinition>();\n  const [selectedWorkflow, setSelectedWorkflow] = useState<string>(getSelectedWorkflowName());\n  const [listOfWorkflows, setListOfWorkflows] = useState<string[]>([]);\n  const [viewType, setViewType] = useState<string>(\"system\");\n  const [dialogOpen, setDialogOpen] = useState(false);\n  const [openOverviewComponentEditorDialog, setOpenOverviewComponentEditorDialog] = useState(false);\n  const [selectedStep, setSelectedStep] = useState<WorkflowStepDefinition>();\n  const [selectedComponent, setSelectedComponent] = useState<WorkflowSystemComponent>();\n  const [fileContent, setFileContent] = useState('');\n\n\n  useEffect(() => {\n    loadListOfWorkflows();\n    loadWorkflowDefinitions(getSelectedWorkflowName());\n    startStatePolling(selectedWorkflow);\n\n  }, []);\n\n  const fetchFileContent = async () => {\n    try {\n      var myHeaders = new Headers();\n      myHeaders.append('pragma', 'no-cache');\n      myHeaders.append('cache-control', 'no-cache');\n      const response = await fetch(neatApiRootUrl + '/data/workflows/' + selectedWorkflow + '/workflow.py', { method: \"get\", headers: myHeaders });\n      const content = await response.text();\n      setFileContent(content);\n    } catch (error) {\n      console.error('Error fetching file:', error);\n    }\n  };\n\n  useEffect(() => {\n    console.log(\"workflow definition changed\")\n    syncWorkflowDefToNodesAndEdges(viewType);\n  }, [workflowDefinitions]);\n\n  const startStatePolling = (workflowName:string) => {\n    if (timerInterval) {\n      clearInterval(timerInterval);\n    }\n    let newTimerInterval = setInterval(() => {\n      loadWorkflowStats(workflowName);\n    }, 2000);\n    setTimerInterval(newTimerInterval);\n  }\n\n  const stopStatePolling = () => {\n    clearInterval(timerInterval);\n  }\n\n  const loadListOfWorkflows = () => {\n    const url = neatApiRootUrl + \"/api/workflow/workflows\";\n    fetch(url).then((response) => response.json()).then((data) => {\n      setListOfWorkflows(data.workflows);\n    }).catch((error) => {\n      console.error('Error:', error);\n    }).finally(() => { });\n  }\n\n  const loadWorkflowDefinitions = (workflowName: string = \"\") => {\n    if (workflowName == \"\")\n      workflowName = selectedWorkflow;\n    const url = neatApiRootUrl + \"/api/workflow/workflow-definition/\" + workflowName;\n    fetch(url).then((response) => response.json()).then((data) => {\n      const workflows = WorkflowDefinition.fromJSON(data.definition);\n      setWorkflowDefinitions(workflows);\n      // loadWorkflowStats(workflowName);\n  }).catch ((error) => {\n    console.error('Error:', error);\n  }).finally(() => { });\n}\n\nconst filterStats = (stats: WorkflowStats) => {\n  console.log(\"loadWorkflowStats\")\n  console.dir(stats)\n  // detelete all log RUNNING entries that have both RUNNING and COMPLETED entries for the same step\n  if (stats.execution_log == null)\n    return stats;\n\n  const filteredLog = stats.execution_log!.filter((log, index) => {\n    if (log.state == \"STARTED\") {\n      const nextLog = stats.execution_log[index + 1];\n      if (nextLog && nextLog.state == \"COMPLETED\" && nextLog.id == log.id)\n        return false;\n    }\n    return true;\n  })\n  stats.execution_log = filteredLog;\n  return stats;\n}\n\nconst loadWorkflowStats = (workflowName: string = \"\") => {\n  if (workflowName == \"\")\n    workflowName = selectedWorkflow;\n  const url = neatApiRootUrl + \"/api/workflow/stats/\" + workflowName;\n  fetch(url).then((response) => response.json()).then((data) => {\n\n    // const filteredStats = filterStats(data);\n    setWorkflowStats(data);\n    if (data.state == \"RUNNING\") {\n      // startStatePolling();\n    } else if (data.state == \"COMPLETED\" || data.state == \"FAILED\") {\n      // stopStatePolling();\n    }\n\n  }).catch((error) => {\n    console.error('Error:', error);\n  })\n}\n\nconst startWorkflow = () => {\n  const url = neatApiRootUrl + \"/api/workflow/start\";\n  const params = { name: selectedWorkflow, config: \"\", start_step: \"\" };\n  fetch(url, {\n    method: \"post\", body: JSON.stringify(params), headers: {\n      'Content-Type': 'application/json;charset=utf-8'\n    }\n  }).then((response) => response.json()).then((data) => {\n    console.dir(data)\n    setWorkflowStats(data);\n    startStatePolling(selectedWorkflow);\n    loadWorkflowStats();\n  }).catch((error) => {\n    console.error('Error:', error);\n  })\n}\n\n\nconst saveWorkflow = () => {\n  console.dir(nodes);\n  syncNodesAndEdgesToWorkflowDef();\n  let wdef = workflowDefinitions;\n  console.dir(wdef);\n  const url = neatApiRootUrl + \"/api/workflow/workflow-definition/\" + selectedWorkflow;\n  fetch(url, {\n    method: \"post\", body: wdef.serializeToJson(), headers: {\n      'Content-Type': 'application/json;charset=utf-8'\n    }\n  }).then((response) => response.json()).then((data) => {\n    console.dir(data)\n  }\n  ).catch((error) => {\n    console.error('Error:', error);\n  })\n};\n\nconst syncNodesAndEdgesToWorkflowDef = () => {\n  if (workflowDefinitions) {\n    workflowDefinitions.updatePositions(nodes);\n    if (viewType == \"system\")\n      workflowDefinitions.updateSystemComponentTransitions(edges);\n    else\n      workflowDefinitions.updateStepTransitions(edges);\n  } else {\n    console.error(\"workflowDefinitions is null\");\n  }\n\n}\n\nconst syncWorkflowDefToNodesAndEdges = (viewType:string) => {\n  if (!workflowDefinitions)\n    return;\n  switch (viewType) {\n    case 'steps':\n      setNodes(workflowDefinitions.convertStepsToNodes());\n      setEdges(workflowDefinitions.convertStepsToEdges());\n      break;\n    case 'system':\n      setNodes(workflowDefinitions.convertSystemComponentsToNodes());\n      setEdges(workflowDefinitions.convertSystemComponentsToEdges());\n  }\n}\n\n\nconst reloadWorkflows = () => {\n  const url = neatApiRootUrl + \"/api/workflow/reload-workflows\";\n  fetch(url, {\n    method: \"post\", body: \"\", headers: {\n      'Content-Type': 'application/json;charset=utf-8'\n    }\n  }).then((response) => response.json()).then((data) => {\n    loadWorkflowDefinitions();\n  }\n  ).catch((error) => {\n    console.error('Error:', error);\n  })\n};\n\nconst handleWorkflowSelectorChange = (event: SelectChangeEvent) => {\n  console.dir(\"Workflow changed to :\" + event.target.value);\n  setSelectedWorkflowName(event.target.value);\n  setSelectedWorkflow(event.target.value);\n  loadWorkflowDefinitions(event.target.value);\n  setViewType(\"system\");\n  syncWorkflowDefToNodesAndEdges(\"system\");\n  startStatePolling(event.target.value);\n};\n\nconst handleViewTypeChange = (\n  event: React.MouseEvent<HTMLElement>,\n  newViewType: string,\n) => {\n\n  setViewType(newViewType);\n  syncWorkflowDefToNodesAndEdges(newViewType);\n  if (newViewType == \"src\") {\n    fetchFileContent();\n  }\n};\n\n\nconst onConnect = useCallback((params) => {\n  console.log('onConnect')\n  setEdges((eds) => addEdge(params, eds))\n  syncNodesAndEdgesToWorkflowDef();\n}, [setEdges]);\n\nconst onEdgeUpdateStart = useCallback(() => {\n  console.log('onEdgeUpdateStart')\n  edgeUpdateSuccessful.current = false;\n}, []);\n\nconst onEdgeUpdate = useCallback((oldEdge, newConnection) => {\n  console.log('onEdgeUpdate')\n  edgeUpdateSuccessful.current = true;\n  setEdges((els) => updateEdge(oldEdge, newConnection, els));\n}, [setEdges]);\n\nconst onEdgeUpdateEnd = useCallback((_, edge) => {\n  console.log('onEdgeUpdateEnd')\n  if (!edgeUpdateSuccessful.current) {\n    setEdges((eds) => eds.filter((e) => e.id !== edge.id));\n    syncNodesAndEdgesToWorkflowDef();\n  }\n\n  edgeUpdateSuccessful.current = true;\n}, [setEdges]);\n\nconst onNodeClick = useCallback((event, node) => {\n  console.log('onNodeClick')\n  console.dir(node);\n  handleDialogClickOpen(node.id, viewType);\n}, [workflowDefinitions, viewType]);\n\nconst onAddStep = (() => {\n  console.log('onAddStep')\n  const ui_config = new UIConfig();\n  ui_config.pos_x = 100;\n  ui_config.pos_y = 100;\n  if (viewType == \"steps\") {\n    const step = new WorkflowStepDefinition();\n    step.id = \"step_\" + Math.floor(Math.random() * 1000000);\n    step.label = \"New step\";\n    step.ui_config = ui_config;\n    workflowDefinitions.steps.push(step);\n  } else {\n    const systemComponent = new WorkflowSystemComponent();\n    systemComponent.id = \"system_comp_\" + Math.floor(Math.random() * 1000000);\n    systemComponent.label = \"New component\";\n    systemComponent.ui_config = ui_config;\n    if (workflowDefinitions.system_components == null)\n      workflowDefinitions.system_components = [];\n    workflowDefinitions.system_components.push(systemComponent);\n  }\n  syncWorkflowDefToNodesAndEdges(viewType);\n});\n\nconst handleDialogClickOpen = (id: string, viewType: string) => {\n  console.log(viewType);\n  if (viewType == \"steps\") {\n    setSelectedStep(workflowDefinitions.getStepById(id));\n    setDialogOpen(true);\n  } else {\n    setSelectedComponent(workflowDefinitions.getSystemComponentById(id));\n    setOpenOverviewComponentEditorDialog(true);\n  }\n};\n\nconst handleDialogClose = (step:WorkflowStepDefinition,action:string) => {\n  setDialogOpen(false);\n  switch (action) {\n    case \"delete\":\n      workflowDefinitions.deleteStep(selectedStep.id);\n      syncWorkflowDefToNodesAndEdges(viewType);\n      break;\n    case \"save\":\n      workflowDefinitions.updateStep(selectedStep.id, step);\n      setSelectedStep(step);\n      syncWorkflowDefToNodesAndEdges(viewType);\n      break;\n  }\n\n};\n\n\nconst onDownloadSuccess = (fileName: string, hash: string) => {\n  console.log(\"onDownloadSuccess\", fileName, hash)\n  reloadWorkflows();\n}\nconst solutionComponentEditorDialogHandler = (component: WorkflowSystemComponent,action: string) => {\n  console.log(\"OverviewComponentEditorDialogHandler\")\n  console.dir(component)\n  switch (action) {\n    case \"save\":\n      workflowDefinitions.updateSystemComponent(selectedComponent.id, component);\n      setSelectedComponent(component);\n      syncWorkflowDefToNodesAndEdges(viewType);\n      break;\n    case \"delete\":\n      workflowDefinitions.deleteSystemComponent(component.id);\n      syncWorkflowDefToNodesAndEdges(viewType);\n      break;\n  }\n  setOpenOverviewComponentEditorDialog(false);\n}\n\nconst onNodesChangeN = useCallback((nodeChanges: NodeChange[]) => {\n  // console.log('onNodesChange')\n  // console.dir(nodeChanges);\n  onNodesChange(nodeChanges);\n  syncNodesAndEdgesToWorkflowDef();\n}, [workflowDefinitions,nodes,edges]);\n\nconst onEdgesChangeN = useCallback((edgeChanges: EdgeChange[]) => {\n  console.log('onEdgesChange')\n  console.dir(edgeChanges);\n  onEdgesChange(edgeChanges);\n  syncNodesAndEdgesToWorkflowDef();\n}, [workflowDefinitions,nodes,edges]);\n\nreturn (\n  <div style={{ height: '85vh', width: '97vw' }}>\n    <Box>\n      <FormControl sx={{ width: 300, marginBottom: 2 }}>\n        <InputLabel id=\"workflowSelectorLabel\">Workflow selector</InputLabel>\n        <Select\n          labelId=\"workflowSelectorLabel\"\n          id=\"workflowSelector\"\n          value={selectedWorkflow}\n          size='small'\n          label=\"Query template\"\n          onChange={handleWorkflowSelectorChange}\n        >\n          {\n            listOfWorkflows && listOfWorkflows.map((item, i) => (\n              <MenuItem value={item} key={item}>{item} </MenuItem>\n            ))\n          }\n        </Select>\n      </FormControl>\n      <ToggleButtonGroup\n        color=\"primary\"\n        value={viewType}\n        exclusive\n        size='small'\n        sx={{ marginLeft: 2 }}\n        onChange={handleViewTypeChange}\n        aria-label=\"View type\"\n      >\n        <ToggleButton value=\"system\">Solution overview</ToggleButton>\n        <ToggleButton value=\"steps\">Workflow steps</ToggleButton>\n        <ToggleButton value=\"configurations\">Configurations</ToggleButton>\n        <ToggleButton value=\"src\">Source code</ToggleButton>\n        <ToggleButton value=\"transformations\">Transformation rules</ToggleButton>\n        <ToggleButton value=\"data_explorer\">Data explorer</ToggleButton>\n\n      </ToggleButtonGroup>\n    </Box>\n    {(viewType == \"system\" || viewType == \"steps\") && (\n      <Stack direction=\"row\" spacing={1} justifyContent=\"left\"\n        alignItems=\"left\">\n        <Item>\n          <OverviewComponentEditorDialog open={openOverviewComponentEditorDialog} component={selectedComponent} onClose={solutionComponentEditorDialogHandler} />\n          <StepEditorDialog open={dialogOpen} step={selectedStep} workflowName={selectedWorkflow} onClose={handleDialogClose} />\n          <div style={{ height: '75vh', width: '70vw' }}>\n            <ReactFlow\n              nodes={nodes}\n              edges={edges}\n              onNodeClick={onNodeClick}\n              onNodesChange={onNodesChangeN}\n              onEdgesChange={onEdgesChangeN}\n              onEdgeUpdate={onEdgeUpdate}\n              onEdgeUpdateStart={onEdgeUpdateStart}\n              onEdgeUpdateEnd={onEdgeUpdateEnd}\n              onConnect={onConnect}\n            >\n              <MiniMap />\n              <Controls />\n              <Background />\n              <Panel position=\"bottom-center\">\n              {viewType == \"system\" && (<Button variant=\"outlined\" onClick={onAddStep}>Add solution component</Button>)}\n              {viewType == \"steps\" && (<Button variant=\"outlined\" onClick={onAddStep}>Add workflow step</Button>)}\n              </Panel>\n            </ReactFlow>\n\n            <Button variant=\"outlined\" onClick={startWorkflow} sx={{ marginTop: 2, marginRight: 1 }}>Start workflow</Button>\n            <Button variant=\"outlined\" onClick={saveWorkflow} sx={{ marginTop: 2, marginRight: 1 }}>Save workflow</Button>\n            <Button variant=\"outlined\" onClick={reloadWorkflows} sx={{ marginTop: 2, marginRight: 1 }} >Reload local workflows</Button>\n            <Box sx={{ marginTop: 1, marginBottom: 1 }}>\n              <CdfPublisher type=\"workflow\" />\n              <CdfDownloader type=\"workflow-package\" onDownloadSuccess={onDownloadSuccess} />\n            </Box>\n          </div>\n\n        </Item>\n        <Item >\n          <WorkflowExecutionReport report={workflowStats} />\n        </Item>\n      </Stack>\n    )}\n    {viewType == \"configurations\" && (\n      <ConfigView></ConfigView>\n    )}\n    {viewType == \"transformations\" && (\n      <TransformationTable />\n    )}\n    {viewType == \"data_explorer\" && (\n      <QDataTable />\n    )}\n    {viewType == \"src\" && (\n      <Editor height=\"90vh\" defaultLanguage=\"python\" value={fileContent} />\n    )}\n\n  </div>\n\n\n);\n}\n",
         "import * as React from 'react';\nimport {useState,useEffect} from 'react';\n\nimport { DataGrid, GridColDef, GridRenderCellParams } from '@mui/x-data-grid';\nimport parsePrometheusTextFormat from 'parse-prometheus-text-format';\nimport Box from '@mui/material/Box';\nimport Collapse from '@mui/material/Collapse';\nimport IconButton from '@mui/material/IconButton';\nimport Table from '@mui/material/Table';\nimport TableBody from '@mui/material/TableBody';\nimport TableCell from '@mui/material/TableCell';\nimport TableContainer from '@mui/material/TableContainer';\nimport TableHead from '@mui/material/TableHead';\nimport TableRow from '@mui/material/TableRow';\nimport Typography from '@mui/material/Typography';\nimport Paper from '@mui/material/Paper';\nimport KeyboardArrowDownIcon from '@mui/icons-material/KeyboardArrowDown';\nimport KeyboardArrowUpIcon from '@mui/icons-material/KeyboardArrowUp';\nimport { convertMillisToStr, getNeatApiRootUrl } from 'components/Utils';\nimport WorkflowExecutionReport from 'components/WorkflowExecutionReport';\n\nfunction Row(props: { row: any }) {\n  const { row } = props;\n  const [open, setOpen] = React.useState(false);\n  const [activeRunId, setActiveRunId] = React.useState(\"\");\n  const [detailedExecutionReport, setDetailedExecutionReport] = React.useState(\"\");\n\n\n  const loadExecutionLog = () => {\n    setOpen(!open)\n    console.log(\"run_id: \"+row.run_id)\n\n  }\n\n  return (\n    <React.Fragment>\n      <TableRow sx={{ '& > *': { borderBottom: 'unset' } }}>\n        <TableCell>\n          <IconButton\n            aria-label=\"expand row\"\n            size=\"small\"\n            onClick={() => loadExecutionLog()}\n          >\n            {open ? <KeyboardArrowUpIcon /> : <KeyboardArrowDownIcon />}\n          </IconButton>\n        </TableCell>\n        <TableCell component=\"th\" scope=\"row\">\n          {row.workflow_name}\n        </TableCell>\n        <TableCell align=\"right\">{row.run_id}</TableCell>\n        <TableCell align=\"right\" style={{color: row.state == \"FAILED\" || row.state == \"EXPIRED\" ? \"red\" : \"green\"}}>{row.state}</TableCell>\n        <TableCell align=\"right\">{convertMillisToStr(row.start_time)}</TableCell>\n        <TableCell align=\"right\">{convertMillisToStr(row.end_time)}</TableCell>\n        <TableCell align=\"right\">{row.elapsed_time} sec</TableCell>\n      </TableRow>\n      <TableRow>\n        <TableCell style={{ paddingBottom: 0, paddingTop: 0 }} colSpan={6}>\n          <Collapse in={open} timeout=\"auto\" unmountOnExit>\n            <Box sx={{ margin: 1 }}>\n              <Typography variant=\"h6\" gutterBottom component=\"div\">\n                Detailed execution log\n              </Typography>\n              {open && (\n                <WorkflowExecutionReport report={row} run_id = {row.run_id}/>\n              )}\n\n            </Box>\n          </Collapse>\n        </TableCell>\n      </TableRow>\n    </React.Fragment>\n  );\n}\n\nexport default function ExecutionsTable() {\n  const neatApiRootUrl = getNeatApiRootUrl();\n  const [data, setData] = useState(Array<any>);\n\n  useEffect(() => {\n    loadDataset();\n  }, []);\n\n  const loadDataset = () => {\n    let url = neatApiRootUrl+\"/api/workflow/executions\"\n    fetch(url)\n    .then((response) => {\n      return response.json();\n    }).then((jdata) => {\n      setData(jdata.executions);\n\n    }\n  )}\n  return (\n    <div>\n    <TableContainer component={Paper}>\n      <Table aria-label=\"collapsible table\">\n        <TableHead>\n          <TableRow>\n            <TableCell />\n            <TableCell>Workflow name</TableCell>\n            <TableCell align=\"right\">Run id</TableCell>\n            <TableCell align=\"right\">State</TableCell>\n            <TableCell align=\"right\">Start time</TableCell>\n            <TableCell align=\"right\">End time</TableCell>\n            <TableCell align=\"right\">Duration</TableCell>\n          </TableRow>\n        </TableHead>\n        <TableBody>\n          {data.map((row:any) => (\n            <Row key={row.name} row={row} />\n          ))}\n        </TableBody>\n      </Table>\n\n    </TableContainer>\n    </div>\n  );\n}\n",
         "import * as React from 'react';\nimport Box from '@mui/material/Box';\nimport Paper from '@mui/material/Paper';\nimport Stack from '@mui/material/Stack';\nimport { styled } from '@mui/material/styles';\nimport Button from '@mui/material/Button';\nimport TextField from '@mui/material/TextField';\nimport LinearProgress from '@mui/material/LinearProgress';\nimport { useState, useEffect } from 'react';\nimport { getNeatApiRootUrl } from 'components/Utils';\nimport FormControlLabel from '@mui/material/FormControlLabel';\nimport Switch from '@mui/material/Switch';\n\nconst Item = styled(Paper)(({ theme }) => ({\n  backgroundColor: theme.palette.mode === 'dark' ? '#1A2027' : '#fff',\n  ...theme.typography.body2,\n  padding: theme.spacing(1),\n  textAlign: 'left',\n  color: theme.palette.text.secondary,\n}));\n\nexport default function GlobalConfigView() {\n  const [loading, setLoading] = React.useState(false);\n  const [configs, setConfigs] = React.useState({\n    \"data_store_path\": \"\",\n    \"cdf_client\": {\n      \"project\": \"\",\n      \"client_id\": \"\",\n      \"client_name\": \"neat\",\n      \"base_url\": \"https://az-power-no-northeurope.cognitedata.com\",\n      \"scopes\": [\n        \"https://az-power-no-northeurope.cognitedata.com/.default\"\n      ],\n      \"token_url\": \"\",\n      \"client_secret\": \"\"\n    },\n    \"cdf_default_dataset_id\": 0,\n    \"load_examples\": true,\n    \"download_workflows_from_cdf\": false,\n    \"workflow_downloader_filter\": \"\",\n    \"log_level\": \"DEBUG\",\n    \"log_format\": \"%(asctime)s.%(msecs)03d %(levelname)-8s %(message)s\",\n    \"stop_on_error\": false\n  });\n\n  let initCdfResourcesResult:string = \"\";\n\n  const [neatApiRootUrl, setNeatApiRootUrl] = useState(getNeatApiRootUrl());\n\n  useEffect(() => {\n    loadConfigs();\n  }, []);\n\n  const loadConfigs = () => {\n    const url = neatApiRootUrl+\"/api/configs/global\";\n    fetch(url).then((response) => response.json()).then((data) => {\n      console.dir(data)\n      setConfigs(data)\n    }).catch((error) => {\n      console.error('Error:', error);\n    }).finally(() => { setLoading(false); });\n  }\n\n\n  const saveConfigButtonHandler = () => {\n    console.dir(configs);\n    setLoading(true);\n    let url = neatApiRootUrl+\"/api/configs/global\";\n\n    fetch(url, {\n      method: \"post\", body: JSON.stringify(configs), headers: {\n        'Content-Type': 'application/json;charset=utf-8'\n      }\n    }).then((response) => response.json()).then((data) => {\n      console.dir(data)\n    }).catch((error) => {\n      console.error('Error:', error);\n    }).finally(() => { setLoading(false); });\n  }\n\n  const saveNeatApiConfigButtonHandler = () => {\n    localStorage.setItem(\"neatApiRootUrl\", neatApiRootUrl);\n  }\n\n  const handleConfigChange = (name, value) => {\n    if (name == \"neatApiRootUrl\") {\n      setNeatApiRootUrl(value);\n    }else {\n      setConfigs({ ...configs, [name]: value });\n    }\n  };\n  const handleCdfConfigChange = (name, value) => {\n    let new_config  = {...configs};\n    new_config.cdf_client[name] = value;\n    setConfigs(new_config);\n  };\n\n  const initCdfResources = () => {\n    setLoading(true);\n    let url = neatApiRootUrl+\"/api/cdf/init-neat-resources\";\n    // send post request\n    fetch(url, {\n      method: \"post\"})\n      .then((response) => response.json())\n      .then((data) => {\n        console.dir(data)\n        initCdfResourcesResult = data.result;\n      }).catch((error) => {\n        console.error('Error:', error);\n        initCdfResourcesResult = \"Error: \"+error;\n      }).finally(() => { setLoading(false); });\n  }\n\n  return (\n    <Box sx={{ width: \"70%\" }}>\n      <Stack spacing={2}>\n        <Item>\n          <h3>Global configurations</h3>\n          <Box sx={{ minWidth: 200 }}>\n            <Stack spacing={2} direction=\"column\">\n              <h4>CDF configurations</h4>\n              <TextField id=\"project_name\" label=\"Project name\" size='small' variant=\"outlined\" value={configs.cdf_client.project} onChange={(event) => { handleCdfConfigChange(\"project\", event.target.value) }} />\n              <TextField id=\"client_id\" label=\"Client id\" size='small' variant=\"outlined\" value={configs.cdf_client.client_id} onChange={(event) => { handleCdfConfigChange(\"client_id\", event.target.value) }} />\n              <TextField id=\"client_secret\" label=\"Client secret\" type=\"password\" size='small' variant=\"outlined\" value={configs.cdf_client.client_secret} onChange={(event) => { handleCdfConfigChange(\"client_secret\", event.target.value) }} />\n              <TextField id=\"client_name\" label=\"Client name\" size='small' variant=\"outlined\" value={configs.cdf_client.client_name} onChange={(event) => { handleCdfConfigChange(\"client_name\", event.target.value) }} />\n              <TextField id=\"cdf_api_base_url\" label=\"CDF api base url\" size='small' variant=\"outlined\" value={configs.cdf_client.base_url} onChange={(event) => { handleCdfConfigChange(\"base_url\", event.target.value) }} />\n              <TextField id=\"scopes\" label=\"Scopes\" size='small' variant=\"outlined\" value={configs.cdf_client.scopes} onChange={(event) => { handleCdfConfigChange(\"scopes\", event.target.value) }} />\n              <TextField id=\"oidc_token_url\" label=\"OIDC token url\" size='small' variant=\"outlined\" value={configs.cdf_client.token_url} onChange={(event) => { handleCdfConfigChange(\"token_url\", event.target.value) }} />\n              <TextField id=\"cdf_default_dataset_id\" type=\"number\"  label=\"Default CDF dataset id.The dataset is used as workflow and rules storage.\" size='small' variant=\"outlined\" value={configs.cdf_default_dataset_id} onChange={(event) => { handleConfigChange(\"cdf_default_dataset_id\", event.target.value) }} />\n              <h4>Storage and workflows</h4>\n              <TextField id=\"data_store_path\" label=\"Data directory.Is used as local workflow , rules and db storage.\" size='small' variant=\"outlined\" value={configs.data_store_path} onChange={(event) => { handleConfigChange(\"data_store_path\", event.target.value) }} />\n              <FormControlLabel control={<Switch checked={configs.download_workflows_from_cdf} onChange={(event) => { handleConfigChange(\"download_workflows_from_cdf\", event.target.checked) }} />} label=\"Automatically download workflows from CDF on startup\"  />\n              <TextField id=\"workflow_downloader_filter\" label=\"List of workflows or filters that will be used for downloading workflows\" size='small' variant=\"outlined\" value={configs.workflow_downloader_filter} onChange={(event) => { handleConfigChange(\"workflow_downloader_filter\", event.target.value) }} />\n              <FormControlLabel control={<Switch checked={configs.load_examples} onChange={(event) => { handleConfigChange(\"load_examples\", event.target.checked) }} />} label=\"Load default examples\"  />\n              <TextField id=\"log_level\" label=\"Log level\" size='small' variant=\"outlined\" value={configs.log_level} onChange={(event) => { handleConfigChange(\"log_level\", event.target.value) }} />\n              <Button variant=\"contained\" onClick={saveConfigButtonHandler}>Save</Button>\n              {loading && (<LinearProgress />)}\n            </Stack>\n          </Box>\n          <h3>NEAT UI configuration</h3>\n          <Box sx={{ minWidth: 120 }}>\n            <Stack spacing={2} direction=\"column\">\n              <TextField id=\"neat_api_root_url\" label=\"API root url\" size='small' variant=\"outlined\" value={neatApiRootUrl} onChange={(event) => { handleConfigChange(\"neatApiRootUrl\", event.target.value) }} />\n              <Button variant=\"contained\" onClick={saveNeatApiConfigButtonHandler}>Save</Button>\n            </Stack>\n          </Box>\n          <h3>Neat internal CDF resources (used for storing files and execution history)</h3>\n\n          <Button variant=\"contained\" onClick={initCdfResources}>Initialize CDF resources</Button>\n\n        </Item>\n\n\n      </Stack>\n    </Box>\n  );\n}\n",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getListItemUtilityClass(slot) {\n  return generateUtilityClass('MuiListItem', slot);\n}\nconst listItemClasses = generateUtilityClasses('MuiListItem', ['root', 'container', 'focusVisible', 'dense', 'alignItemsFlexStart', 'disabled', 'divider', 'gutters', 'padding', 'button', 'secondaryAction', 'selected']);\nexport default listItemClasses;",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getListItemButtonUtilityClass(slot) {\n  return generateUtilityClass('MuiListItemButton', slot);\n}\nconst listItemButtonClasses = generateUtilityClasses('MuiListItemButton', ['root', 'focusVisible', 'dense', 'alignItemsFlexStart', 'disabled', 'divider', 'gutters', 'selected']);\nexport default listItemButtonClasses;",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getListItemSecondaryActionClassesUtilityClass(slot) {\n  return generateUtilityClass('MuiListItemSecondaryAction', slot);\n}\nconst listItemSecondaryActionClasses = generateUtilityClasses('MuiListItemSecondaryAction', ['root', 'disableGutters']);\nexport default listItemSecondaryActionClasses;",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"className\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport styled from '../styles/styled';\nimport useThemeProps from '../styles/useThemeProps';\nimport ListContext from '../List/ListContext';\nimport { getListItemSecondaryActionClassesUtilityClass } from './listItemSecondaryActionClasses';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst useUtilityClasses = ownerState => {\n  const {\n    disableGutters,\n    classes\n  } = ownerState;\n  const slots = {\n    root: ['root', disableGutters && 'disableGutters']\n  };\n  return composeClasses(slots, getListItemSecondaryActionClassesUtilityClass, classes);\n};\nconst ListItemSecondaryActionRoot = styled('div', {\n  name: 'MuiListItemSecondaryAction',\n  slot: 'Root',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.root, ownerState.disableGutters && styles.disableGutters];\n  }\n})(({\n  ownerState\n}) => _extends({\n  position: 'absolute',\n  right: 16,\n  top: '50%',\n  transform: 'translateY(-50%)'\n}, ownerState.disableGutters && {\n  right: 0\n}));\n\n/**\n * Must be used as the last child of ListItem to function properly.\n */\nconst ListItemSecondaryAction = /*#__PURE__*/React.forwardRef(function ListItemSecondaryAction(inProps, ref) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiListItemSecondaryAction'\n  });\n  const {\n      className\n    } = props,\n    other = _objectWithoutPropertiesLoose(props, _excluded);\n  const context = React.useContext(ListContext);\n  const ownerState = _extends({}, props, {\n    disableGutters: context.disableGutters\n  });\n  const classes = useUtilityClasses(ownerState);\n  return /*#__PURE__*/_jsx(ListItemSecondaryActionRoot, _extends({\n    className: clsx(classes.root, className),\n    ownerState: ownerState,\n    ref: ref\n  }, other));\n});\nprocess.env.NODE_ENV !== \"production\" ? ListItemSecondaryAction.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * The content of the component, normally an `IconButton` or selection control.\n   */\n  children: PropTypes.node,\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object])\n} : void 0;\nListItemSecondaryAction.muiName = 'ListItemSecondaryAction';\nexport default ListItemSecondaryAction;",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"className\"],\n  _excluded2 = [\"alignItems\", \"autoFocus\", \"button\", \"children\", \"className\", \"component\", \"components\", \"componentsProps\", \"ContainerComponent\", \"ContainerProps\", \"dense\", \"disabled\", \"disableGutters\", \"disablePadding\", \"divider\", \"focusVisibleClassName\", \"secondaryAction\", \"selected\", \"slotProps\", \"slots\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { unstable_composeClasses as composeClasses, isHostComponent } from '@mui/base';\nimport { chainPropTypes, elementTypeAcceptingRef } from '@mui/utils';\nimport { alpha } from '@mui/system';\nimport styled from '../styles/styled';\nimport useThemeProps from '../styles/useThemeProps';\nimport ButtonBase from '../ButtonBase';\nimport isMuiElement from '../utils/isMuiElement';\nimport useEnhancedEffect from '../utils/useEnhancedEffect';\nimport useForkRef from '../utils/useForkRef';\nimport ListContext from '../List/ListContext';\nimport listItemClasses, { getListItemUtilityClass } from './listItemClasses';\nimport { listItemButtonClasses } from '../ListItemButton';\nimport ListItemSecondaryAction from '../ListItemSecondaryAction';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nimport { jsxs as _jsxs } from \"react/jsx-runtime\";\nexport const overridesResolver = (props, styles) => {\n  const {\n    ownerState\n  } = props;\n  return [styles.root, ownerState.dense && styles.dense, ownerState.alignItems === 'flex-start' && styles.alignItemsFlexStart, ownerState.divider && styles.divider, !ownerState.disableGutters && styles.gutters, !ownerState.disablePadding && styles.padding, ownerState.button && styles.button, ownerState.hasSecondaryAction && styles.secondaryAction];\n};\nconst useUtilityClasses = ownerState => {\n  const {\n    alignItems,\n    button,\n    classes,\n    dense,\n    disabled,\n    disableGutters,\n    disablePadding,\n    divider,\n    hasSecondaryAction,\n    selected\n  } = ownerState;\n  const slots = {\n    root: ['root', dense && 'dense', !disableGutters && 'gutters', !disablePadding && 'padding', divider && 'divider', disabled && 'disabled', button && 'button', alignItems === 'flex-start' && 'alignItemsFlexStart', hasSecondaryAction && 'secondaryAction', selected && 'selected'],\n    container: ['container']\n  };\n  return composeClasses(slots, getListItemUtilityClass, classes);\n};\nexport const ListItemRoot = styled('div', {\n  name: 'MuiListItem',\n  slot: 'Root',\n  overridesResolver\n})(({\n  theme,\n  ownerState\n}) => _extends({\n  display: 'flex',\n  justifyContent: 'flex-start',\n  alignItems: 'center',\n  position: 'relative',\n  textDecoration: 'none',\n  width: '100%',\n  boxSizing: 'border-box',\n  textAlign: 'left'\n}, !ownerState.disablePadding && _extends({\n  paddingTop: 8,\n  paddingBottom: 8\n}, ownerState.dense && {\n  paddingTop: 4,\n  paddingBottom: 4\n}, !ownerState.disableGutters && {\n  paddingLeft: 16,\n  paddingRight: 16\n}, !!ownerState.secondaryAction && {\n  // Add some space to avoid collision as `ListItemSecondaryAction`\n  // is absolutely positioned.\n  paddingRight: 48\n}), !!ownerState.secondaryAction && {\n  [`& > .${listItemButtonClasses.root}`]: {\n    paddingRight: 48\n  }\n}, {\n  [`&.${listItemClasses.focusVisible}`]: {\n    backgroundColor: (theme.vars || theme).palette.action.focus\n  },\n  [`&.${listItemClasses.selected}`]: {\n    backgroundColor: theme.vars ? `rgba(${theme.vars.palette.primary.mainChannel} / ${theme.vars.palette.action.selectedOpacity})` : alpha(theme.palette.primary.main, theme.palette.action.selectedOpacity),\n    [`&.${listItemClasses.focusVisible}`]: {\n      backgroundColor: theme.vars ? `rgba(${theme.vars.palette.primary.mainChannel} / calc(${theme.vars.palette.action.selectedOpacity} + ${theme.vars.palette.action.focusOpacity}))` : alpha(theme.palette.primary.main, theme.palette.action.selectedOpacity + theme.palette.action.focusOpacity)\n    }\n  },\n  [`&.${listItemClasses.disabled}`]: {\n    opacity: (theme.vars || theme).palette.action.disabledOpacity\n  }\n}, ownerState.alignItems === 'flex-start' && {\n  alignItems: 'flex-start'\n}, ownerState.divider && {\n  borderBottom: `1px solid ${(theme.vars || theme).palette.divider}`,\n  backgroundClip: 'padding-box'\n}, ownerState.button && {\n  transition: theme.transitions.create('background-color', {\n    duration: theme.transitions.duration.shortest\n  }),\n  '&:hover': {\n    textDecoration: 'none',\n    backgroundColor: (theme.vars || theme).palette.action.hover,\n    // Reset on touch devices, it doesn't add specificity\n    '@media (hover: none)': {\n      backgroundColor: 'transparent'\n    }\n  },\n  [`&.${listItemClasses.selected}:hover`]: {\n    backgroundColor: theme.vars ? `rgba(${theme.vars.palette.primary.mainChannel} / calc(${theme.vars.palette.action.selectedOpacity} + ${theme.vars.palette.action.hoverOpacity}))` : alpha(theme.palette.primary.main, theme.palette.action.selectedOpacity + theme.palette.action.hoverOpacity),\n    // Reset on touch devices, it doesn't add specificity\n    '@media (hover: none)': {\n      backgroundColor: theme.vars ? `rgba(${theme.vars.palette.primary.mainChannel} / ${theme.vars.palette.action.selectedOpacity})` : alpha(theme.palette.primary.main, theme.palette.action.selectedOpacity)\n    }\n  }\n}, ownerState.hasSecondaryAction && {\n  // Add some space to avoid collision as `ListItemSecondaryAction`\n  // is absolutely positioned.\n  paddingRight: 48\n}));\nconst ListItemContainer = styled('li', {\n  name: 'MuiListItem',\n  slot: 'Container',\n  overridesResolver: (props, styles) => styles.container\n})({\n  position: 'relative'\n});\n\n/**\n * Uses an additional container component if `ListItemSecondaryAction` is the last child.\n */\nconst ListItem = /*#__PURE__*/React.forwardRef(function ListItem(inProps, ref) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiListItem'\n  });\n  const {\n      alignItems = 'center',\n      autoFocus = false,\n      button = false,\n      children: childrenProp,\n      className,\n      component: componentProp,\n      components = {},\n      componentsProps = {},\n      ContainerComponent = 'li',\n      ContainerProps: {\n        className: ContainerClassName\n      } = {},\n      dense = false,\n      disabled = false,\n      disableGutters = false,\n      disablePadding = false,\n      divider = false,\n      focusVisibleClassName,\n      secondaryAction,\n      selected = false,\n      slotProps = {},\n      slots = {}\n    } = props,\n    ContainerProps = _objectWithoutPropertiesLoose(props.ContainerProps, _excluded),\n    other = _objectWithoutPropertiesLoose(props, _excluded2);\n  const context = React.useContext(ListContext);\n  const childContext = React.useMemo(() => ({\n    dense: dense || context.dense || false,\n    alignItems,\n    disableGutters\n  }), [alignItems, context.dense, dense, disableGutters]);\n  const listItemRef = React.useRef(null);\n  useEnhancedEffect(() => {\n    if (autoFocus) {\n      if (listItemRef.current) {\n        listItemRef.current.focus();\n      } else if (process.env.NODE_ENV !== 'production') {\n        console.error('MUI: Unable to set focus to a ListItem whose component has not been rendered.');\n      }\n    }\n  }, [autoFocus]);\n  const children = React.Children.toArray(childrenProp);\n\n  // v4 implementation, deprecated in v5, will be removed in v6\n  const hasSecondaryAction = children.length && isMuiElement(children[children.length - 1], ['ListItemSecondaryAction']);\n  const ownerState = _extends({}, props, {\n    alignItems,\n    autoFocus,\n    button,\n    dense: childContext.dense,\n    disabled,\n    disableGutters,\n    disablePadding,\n    divider,\n    hasSecondaryAction,\n    selected\n  });\n  const classes = useUtilityClasses(ownerState);\n  const handleRef = useForkRef(listItemRef, ref);\n  const Root = slots.root || components.Root || ListItemRoot;\n  const rootProps = slotProps.root || componentsProps.root || {};\n  const componentProps = _extends({\n    className: clsx(classes.root, rootProps.className, className),\n    disabled\n  }, other);\n  let Component = componentProp || 'li';\n  if (button) {\n    componentProps.component = componentProp || 'div';\n    componentProps.focusVisibleClassName = clsx(listItemClasses.focusVisible, focusVisibleClassName);\n    Component = ButtonBase;\n  }\n\n  // v4 implementation, deprecated in v5, will be removed in v6\n  if (hasSecondaryAction) {\n    // Use div by default.\n    Component = !componentProps.component && !componentProp ? 'div' : Component;\n\n    // Avoid nesting of li > li.\n    if (ContainerComponent === 'li') {\n      if (Component === 'li') {\n        Component = 'div';\n      } else if (componentProps.component === 'li') {\n        componentProps.component = 'div';\n      }\n    }\n    return /*#__PURE__*/_jsx(ListContext.Provider, {\n      value: childContext,\n      children: /*#__PURE__*/_jsxs(ListItemContainer, _extends({\n        as: ContainerComponent,\n        className: clsx(classes.container, ContainerClassName),\n        ref: handleRef,\n        ownerState: ownerState\n      }, ContainerProps, {\n        children: [/*#__PURE__*/_jsx(Root, _extends({}, rootProps, !isHostComponent(Root) && {\n          as: Component,\n          ownerState: _extends({}, ownerState, rootProps.ownerState)\n        }, componentProps, {\n          children: children\n        })), children.pop()]\n      }))\n    });\n  }\n  return /*#__PURE__*/_jsx(ListContext.Provider, {\n    value: childContext,\n    children: /*#__PURE__*/_jsxs(Root, _extends({}, rootProps, {\n      as: Component,\n      ref: handleRef\n    }, !isHostComponent(Root) && {\n      ownerState: _extends({}, ownerState, rootProps.ownerState)\n    }, componentProps, {\n      children: [children, secondaryAction && /*#__PURE__*/_jsx(ListItemSecondaryAction, {\n        children: secondaryAction\n      })]\n    }))\n  });\n});\nprocess.env.NODE_ENV !== \"production\" ? ListItem.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * Defines the `align-items` style property.\n   * @default 'center'\n   */\n  alignItems: PropTypes.oneOf(['center', 'flex-start']),\n  /**\n   * If `true`, the list item is focused during the first mount.\n   * Focus will also be triggered if the value changes from false to true.\n   * @default false\n   * @deprecated checkout [ListItemButton](/material-ui/api/list-item-button/) instead\n   */\n  autoFocus: PropTypes.bool,\n  /**\n   * If `true`, the list item is a button (using `ButtonBase`). Props intended\n   * for `ButtonBase` can then be applied to `ListItem`.\n   * @default false\n   * @deprecated checkout [ListItemButton](/material-ui/api/list-item-button/) instead\n   */\n  button: PropTypes.bool,\n  /**\n   * The content of the component if a `ListItemSecondaryAction` is used it must\n   * be the last child.\n   */\n  children: chainPropTypes(PropTypes.node, props => {\n    const children = React.Children.toArray(props.children);\n\n    // React.Children.toArray(props.children).findLastIndex(isListItemSecondaryAction)\n    let secondaryActionIndex = -1;\n    for (let i = children.length - 1; i >= 0; i -= 1) {\n      const child = children[i];\n      if (isMuiElement(child, ['ListItemSecondaryAction'])) {\n        secondaryActionIndex = i;\n        break;\n      }\n    }\n\n    //  is ListItemSecondaryAction the last child of ListItem\n    if (secondaryActionIndex !== -1 && secondaryActionIndex !== children.length - 1) {\n      return new Error('MUI: You used an element after ListItemSecondaryAction. ' + 'For ListItem to detect that it has a secondary action ' + 'you must pass it as the last child to ListItem.');\n    }\n    return null;\n  }),\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n  /**\n   * The component used for the root node.\n   * Either a string to use a HTML element or a component.\n   */\n  component: PropTypes.elementType,\n  /**\n   * The components used for each slot inside.\n   *\n   * This prop is an alias for the `slots` prop.\n   * It's recommended to use the `slots` prop instead.\n   *\n   * @default {}\n   */\n  components: PropTypes.shape({\n    Root: PropTypes.elementType\n  }),\n  /**\n   * The extra props for the slot components.\n   * You can override the existing props or add new ones.\n   *\n   * This prop is an alias for the `slotProps` prop.\n   * It's recommended to use the `slotProps` prop instead, as `componentsProps` will be deprecated in the future.\n   *\n   * @default {}\n   */\n  componentsProps: PropTypes.shape({\n    root: PropTypes.object\n  }),\n  /**\n   * The container component used when a `ListItemSecondaryAction` is the last child.\n   * @default 'li'\n   * @deprecated\n   */\n  ContainerComponent: elementTypeAcceptingRef,\n  /**\n   * Props applied to the container component if used.\n   * @default {}\n   * @deprecated\n   */\n  ContainerProps: PropTypes.object,\n  /**\n   * If `true`, compact vertical padding designed for keyboard and mouse input is used.\n   * The prop defaults to the value inherited from the parent List component.\n   * @default false\n   */\n  dense: PropTypes.bool,\n  /**\n   * If `true`, the component is disabled.\n   * @default false\n   * @deprecated checkout [ListItemButton](/material-ui/api/list-item-button/) instead\n   */\n  disabled: PropTypes.bool,\n  /**\n   * If `true`, the left and right padding is removed.\n   * @default false\n   */\n  disableGutters: PropTypes.bool,\n  /**\n   * If `true`, all padding is removed.\n   * @default false\n   */\n  disablePadding: PropTypes.bool,\n  /**\n   * If `true`, a 1px light border is added to the bottom of the list item.\n   * @default false\n   */\n  divider: PropTypes.bool,\n  /**\n   * @ignore\n   */\n  focusVisibleClassName: PropTypes.string,\n  /**\n   * The element to display at the end of ListItem.\n   */\n  secondaryAction: PropTypes.node,\n  /**\n   * Use to apply selected styling.\n   * @default false\n   * @deprecated checkout [ListItemButton](/material-ui/api/list-item-button/) instead\n   */\n  selected: PropTypes.bool,\n  /**\n   * The extra props for the slot components.\n   * You can override the existing props or add new ones.\n   *\n   * This prop is an alias for the `componentsProps` prop, which will be deprecated in the future.\n   *\n   * @default {}\n   */\n  slotProps: PropTypes.shape({\n    root: PropTypes.object\n  }),\n  /**\n   * The components used for each slot inside.\n   *\n   * This prop is an alias for the `components` prop, which will be deprecated in the future.\n   *\n   * @default {}\n   */\n  slots: PropTypes.shape({\n    root: PropTypes.elementType\n  }),\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object])\n} : void 0;\nexport default ListItem;",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"children\", \"className\", \"disableTypography\", \"inset\", \"primary\", \"primaryTypographyProps\", \"secondary\", \"secondaryTypographyProps\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport Typography from '../Typography';\nimport ListContext from '../List/ListContext';\nimport useThemeProps from '../styles/useThemeProps';\nimport styled from '../styles/styled';\nimport listItemTextClasses, { getListItemTextUtilityClass } from './listItemTextClasses';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nimport { jsxs as _jsxs } from \"react/jsx-runtime\";\nconst useUtilityClasses = ownerState => {\n  const {\n    classes,\n    inset,\n    primary,\n    secondary,\n    dense\n  } = ownerState;\n  const slots = {\n    root: ['root', inset && 'inset', dense && 'dense', primary && secondary && 'multiline'],\n    primary: ['primary'],\n    secondary: ['secondary']\n  };\n  return composeClasses(slots, getListItemTextUtilityClass, classes);\n};\nconst ListItemTextRoot = styled('div', {\n  name: 'MuiListItemText',\n  slot: 'Root',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [{\n      [`& .${listItemTextClasses.primary}`]: styles.primary\n    }, {\n      [`& .${listItemTextClasses.secondary}`]: styles.secondary\n    }, styles.root, ownerState.inset && styles.inset, ownerState.primary && ownerState.secondary && styles.multiline, ownerState.dense && styles.dense];\n  }\n})(({\n  ownerState\n}) => _extends({\n  flex: '1 1 auto',\n  minWidth: 0,\n  marginTop: 4,\n  marginBottom: 4\n}, ownerState.primary && ownerState.secondary && {\n  marginTop: 6,\n  marginBottom: 6\n}, ownerState.inset && {\n  paddingLeft: 56\n}));\nconst ListItemText = /*#__PURE__*/React.forwardRef(function ListItemText(inProps, ref) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiListItemText'\n  });\n  const {\n      children,\n      className,\n      disableTypography = false,\n      inset = false,\n      primary: primaryProp,\n      primaryTypographyProps,\n      secondary: secondaryProp,\n      secondaryTypographyProps\n    } = props,\n    other = _objectWithoutPropertiesLoose(props, _excluded);\n  const {\n    dense\n  } = React.useContext(ListContext);\n  let primary = primaryProp != null ? primaryProp : children;\n  let secondary = secondaryProp;\n  const ownerState = _extends({}, props, {\n    disableTypography,\n    inset,\n    primary: !!primary,\n    secondary: !!secondary,\n    dense\n  });\n  const classes = useUtilityClasses(ownerState);\n  if (primary != null && primary.type !== Typography && !disableTypography) {\n    primary = /*#__PURE__*/_jsx(Typography, _extends({\n      variant: dense ? 'body2' : 'body1',\n      className: classes.primary,\n      component: primaryTypographyProps != null && primaryTypographyProps.variant ? undefined : 'span',\n      display: \"block\"\n    }, primaryTypographyProps, {\n      children: primary\n    }));\n  }\n  if (secondary != null && secondary.type !== Typography && !disableTypography) {\n    secondary = /*#__PURE__*/_jsx(Typography, _extends({\n      variant: \"body2\",\n      className: classes.secondary,\n      color: \"text.secondary\",\n      display: \"block\"\n    }, secondaryTypographyProps, {\n      children: secondary\n    }));\n  }\n  return /*#__PURE__*/_jsxs(ListItemTextRoot, _extends({\n    className: clsx(classes.root, className),\n    ownerState: ownerState,\n    ref: ref\n  }, other, {\n    children: [primary, secondary]\n  }));\n});\nprocess.env.NODE_ENV !== \"production\" ? ListItemText.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * Alias for the `primary` prop.\n   */\n  children: PropTypes.node,\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n  /**\n   * If `true`, the children won't be wrapped by a Typography component.\n   * This can be useful to render an alternative Typography variant by wrapping\n   * the `children` (or `primary`) text, and optional `secondary` text\n   * with the Typography component.\n   * @default false\n   */\n  disableTypography: PropTypes.bool,\n  /**\n   * If `true`, the children are indented.\n   * This should be used if there is no left avatar or left icon.\n   * @default false\n   */\n  inset: PropTypes.bool,\n  /**\n   * The main content element.\n   */\n  primary: PropTypes.node,\n  /**\n   * These props will be forwarded to the primary typography component\n   * (as long as disableTypography is not `true`).\n   */\n  primaryTypographyProps: PropTypes.object,\n  /**\n   * The secondary content element.\n   */\n  secondary: PropTypes.node,\n  /**\n   * These props will be forwarded to the secondary typography component\n   * (as long as disableTypography is not `true`).\n   */\n  secondaryTypographyProps: PropTypes.object,\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object])\n} : void 0;\nexport default ListItemText;",
-        "import React, { useState, useEffect } from 'react';\nimport { Typography, List, ListItem, ListItemText } from '@mui/material';\nimport { getNeatApiRootUrl } from 'components/Utils';\n\n\nconst AboutView = () => {\n  const [structure, setStructure] = useState(null);\n  const [neatApiRootUrl, setNeatApiRootUrl] = useState(getNeatApiRootUrl());\n  useEffect(() => {\n    const fetchData = async () => {\n      try {\n        const response = await fetch(neatApiRootUrl+'/api/about');\n        const data = await response.json();\n        setStructure(data);\n      } catch (error) {\n        console.error('Error fetching data:', error);\n      }\n    };\n\n    fetchData();\n  }, []);\n\n  if (!structure) {\n    return <div>Loading...</div>;\n  }\n\n  return (\n    <div >\n      <Typography variant=\"h5\" >\n        NEAT Version: {structure.version}\n      </Typography>\n      <Typography variant=\"h6\" >\n        Docs URL: <a href='https://thisisneat.io/index.html'>https://thisisneat.io/index.html</a>\n      </Typography>\n      <Typography variant=\"h6\" >\n        Github: <a href='https://github.com/cognitedata/neat'>hhttps://github.com/cognitedata/neat</a>\n      </Typography>\n      <Typography variant=\"h6\" >\n        Issues tracker (Github): <a href='https://github.com/cognitedata/neat/issues'> https://github.com/cognitedata/neat/issues </a>\n      </Typography>\n      <Typography variant=\"h6\" >\n        License (Apache 2.0): <a href='https://github.com/cognitedata/neat/blob/main/LICENSE'> https://github.com/cognitedata/neat/blob/main/LICENSE </a>\n      </Typography>\n      <Typography variant=\"h5\">\n        3rd party packages :\n      </Typography>\n      <List dense={true}>\n        {structure.packages.map((spackage, index) => (\n          <ListItem key={index}>\n            <ListItemText primary={spackage} />\n          </ListItem>\n        ))}\n      </List>\n    </div>\n  );\n};\n\nexport default AboutView;\n",
+        "import React, { useState, useEffect } from 'react';\nimport { Typography, List, ListItem, ListItemText } from '@mui/material';\nimport { getNeatApiRootUrl } from 'components/Utils';\n\n\nconst AboutView = () => {\n  const [structure, setStructure] = useState(null);\n  const [neatApiRootUrl, setNeatApiRootUrl] = useState(getNeatApiRootUrl());\n  useEffect(() => {\n    const fetchData = async () => {\n      try {\n        const response = await fetch(neatApiRootUrl+'/api/about');\n        const data = await response.json();\n        setStructure(data);\n      } catch (error) {\n        console.error('Error fetching data:', error);\n      }\n    };\n\n    fetchData();\n  }, []);\n\n  if (!structure) {\n    return <div>Loading...</div>;\n  }\n\n  return (\n    <div >\n      <Typography variant=\"h5\" >\n        NEAT Version: {structure.version}\n      </Typography>\n      <Typography variant=\"h6\" >\n        Docs URL: <a href='https://thisisneat.io'>https://thisisneat.io</a>\n      </Typography>\n      <Typography variant=\"h6\" >\n        Docs URL: <a href='https://cognite-neat.readthedocs-hosted.com/en/latest/'>https://cognite-neat.readthedocs-hosted.com/en/latest/</a>\n      </Typography>\n      <Typography variant=\"h6\" >\n        Github: <a href='https://github.com/cognitedata/neat'>https://github.com/cognitedata/neat</a>\n      </Typography>\n      <Typography variant=\"h6\" >\n        Issues tracker (Github): <a href='https://github.com/cognitedata/neat/issues'> https://github.com/cognitedata/neat/issues </a>\n      </Typography>\n      <Typography variant=\"h6\" >\n        License (Apache 2.0): <a href='https://github.com/cognitedata/neat/blob/main/LICENSE'> https://github.com/cognitedata/neat/blob/main/LICENSE </a>\n      </Typography>\n      <Typography variant=\"h5\">\n        3rd party packages :\n      </Typography>\n      <List dense={true}>\n        {structure.packages.map((spackage, index) => (\n          <ListItem key={index}>\n            <ListItemText primary={spackage} />\n          </ListItem>\n        ))}\n      </List>\n    </div>\n  );\n};\n\nexport default AboutView;\n",
         "import * as React from 'react';\nimport Tabs from '@mui/material/Tabs';\nimport Tab from '@mui/material/Tab';\nimport Typography from '@mui/material/Typography';\nimport Box from '@mui/material/Box';\nimport QDataTable from './views/ExplorerView';\n\nimport Button from '@mui/material/Button';\nimport MetricsTable from './views/MetricsView';\nimport ConfigView from './views/ConfigView';\nimport TransformationTable from './views/TransformationView';\nimport WorkflowView from './views/WorkflowView';\nimport ExecutionsTable from 'views/ExecutionsView';\nimport BuildRoundedIcon from '@mui/icons-material/BuildRounded';\nimport HelpIcon from '@mui/icons-material/Help';\nimport GlobalConfigView from 'views/GlobalConfigView';\nimport AboutView from 'views/AboutView';\n\ninterface TabPanelProps {\n  children?: React.ReactNode;\n  index: number;\n  value: number;\n}\n\nfunction TabPanel(props: TabPanelProps) {\n  const { children, value, index, ...other } = props;\n\n  return (\n    <div\n      role=\"tabpanel\"\n      hidden={value !== index}\n      id={`simple-tabpanel-${index}`}\n      aria-labelledby={`simple-tab-${index}`}\n      {...other}\n    >\n      {value === index && (\n        <Box sx={{ p: 3 }}>\n          {children}\n        </Box>\n      )}\n    </div>\n  );\n}\n\nfunction a11yProps(index: number) {\n  return {\n    id: `simple-tab-${index}`,\n    'aria-controls': `simple-tabpanel-${index}`,\n  };\n}\n\nexport default function BasicTabs() {\n  const [value, setValue] = React.useState(0);\n\n  const handleChange = (event: React.SyntheticEvent, newValue: number) => {\n    setValue(newValue);\n  };\n\n  return (\n    <Box sx={{ width: '100%' }}>\n      <Box sx={{ borderBottom: 1, borderColor: 'divider' }}>\n        <Tabs value={value} onChange={handleChange} aria-label=\"basic tabs example\">\n          <Tab label=\"Solutions\" {...a11yProps(0)} />\n          <Tab label=\"Execution history\" {...a11yProps(1)} />\n          <Tab label=\"Statistics\" {...a11yProps(2)} />\n          <Tab icon={<BuildRoundedIcon />} aria-label=\"Global config\" {...a11yProps(3)} />\n          <Tab icon={<HelpIcon />} aria-label=\"Global config\" {...a11yProps(4)} />\n        </Tabs>\n      </Box>\n      <TabPanel value={value} index={0}>\n        <WorkflowView/>\n      </TabPanel>\n      <TabPanel value={value} index={1}>\n        <ExecutionsTable />\n      </TabPanel>\n      <TabPanel value={value} index={2}>\n        <MetricsTable />\n      </TabPanel>\n      <TabPanel value={value} index={3}>\n        <GlobalConfigView />\n      </TabPanel>\n      <TabPanel value={value} index={4}>\n        <AboutView />\n      </TabPanel>\n\n    </Box>\n  );\n}\n",
         "import logo from './logo.svg';\nimport './App.css';\nimport * as React from 'react';\nimport BasicTabs from './MainContainer.tsx';\nimport CssBaseline from '@mui/material/CssBaseline';\n\nfunction App() {\n  return (\n    <div >\n      <BasicTabs/>\n    </div>\n\n  );\n}\n\nexport default App;\n",
         "import _extends from \"@babel/runtime/helpers/esm/extends\";\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport useThemeProps from '../styles/useThemeProps';\nimport GlobalStyles from '../GlobalStyles';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nimport { jsxs as _jsxs } from \"react/jsx-runtime\";\nexport const html = (theme, enableColorScheme) => _extends({\n  WebkitFontSmoothing: 'antialiased',\n  // Antialiasing.\n  MozOsxFontSmoothing: 'grayscale',\n  // Antialiasing.\n  // Change from `box-sizing: content-box` so that `width`\n  // is not affected by `padding` or `border`.\n  boxSizing: 'border-box',\n  // Fix font resize problem in iOS\n  WebkitTextSizeAdjust: '100%'\n}, enableColorScheme && !theme.vars && {\n  colorScheme: theme.palette.mode\n});\nexport const body = theme => _extends({\n  color: (theme.vars || theme).palette.text.primary\n}, theme.typography.body1, {\n  backgroundColor: (theme.vars || theme).palette.background.default,\n  '@media print': {\n    // Save printer ink.\n    backgroundColor: (theme.vars || theme).palette.common.white\n  }\n});\nexport const styles = (theme, enableColorScheme = false) => {\n  var _theme$components, _theme$components$Mui;\n  const colorSchemeStyles = {};\n  if (enableColorScheme && theme.colorSchemes) {\n    Object.entries(theme.colorSchemes).forEach(([key, scheme]) => {\n      var _scheme$palette;\n      colorSchemeStyles[theme.getColorSchemeSelector(key).replace(/\\s*&/, '')] = {\n        colorScheme: (_scheme$palette = scheme.palette) == null ? void 0 : _scheme$palette.mode\n      };\n    });\n  }\n  let defaultStyles = _extends({\n    html: html(theme, enableColorScheme),\n    '*, *::before, *::after': {\n      boxSizing: 'inherit'\n    },\n    'strong, b': {\n      fontWeight: theme.typography.fontWeightBold\n    },\n    body: _extends({\n      margin: 0\n    }, body(theme), {\n      // Add support for document.body.requestFullScreen().\n      // Other elements, if background transparent, are not supported.\n      '&::backdrop': {\n        backgroundColor: (theme.vars || theme).palette.background.default\n      }\n    })\n  }, colorSchemeStyles);\n  const themeOverrides = (_theme$components = theme.components) == null ? void 0 : (_theme$components$Mui = _theme$components.MuiCssBaseline) == null ? void 0 : _theme$components$Mui.styleOverrides;\n  if (themeOverrides) {\n    defaultStyles = [defaultStyles, themeOverrides];\n  }\n  return defaultStyles;\n};\n\n/**\n * Kickstart an elegant, consistent, and simple baseline to build upon.\n */\nfunction CssBaseline(inProps) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiCssBaseline'\n  });\n  const {\n    children,\n    enableColorScheme = false\n  } = props;\n  return /*#__PURE__*/_jsxs(React.Fragment, {\n    children: [/*#__PURE__*/_jsx(GlobalStyles, {\n      styles: theme => styles(theme, enableColorScheme)\n    }), children]\n  });\n}\nprocess.env.NODE_ENV !== \"production\" ? CssBaseline.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * You can wrap a node.\n   */\n  children: PropTypes.node,\n  /**\n   * Enable `color-scheme` CSS property to use `theme.palette.mode`.\n   * For more details, check out https://developer.mozilla.org/en-US/docs/Web/CSS/color-scheme\n   * For browser support, check out https://caniuse.com/?search=color-scheme\n   * @default false\n   */\n  enableColorScheme: PropTypes.bool\n} : void 0;\nexport default CssBaseline;",
         "import React from 'react';\nimport ReactDOM from 'react-dom/client';\nimport './index.css';\nimport App from './App';\nimport CssBaseline from '@mui/material/CssBaseline';\n\nconst root = ReactDOM.createRoot(document.getElementById('root'));\nroot.render(\n  <React.Fragment>\n     <CssBaseline />\n    <App />\n  </React.Fragment>\n);\n"
     ],
     "version": 3
 }
```

### Comparing `cognite_neat-0.12.0/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/cognite/neat/migration/wf_manifests.py` & `cognite_neat-0.12.1/cognite/neat/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.0/pyproject.toml` & `cognite_neat-0.12.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.12.0"
+version = "0.12.1"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
 packages = [
@@ -61,17 +61,18 @@
 
 mkdocs =  {version="*", optional=true}
 mkdocs-jupyter = {version="*", optional=true}
 mkdocs-material-extensions = {version="*", optional=true}
 mkdocs-git-revision-date-localized-plugin = {version="*", optional=true}
 mkdocs-git-authors-plugin = {version="*", optional=true}
 mkdocs-gitbook = {version="*", optional=true}
+mkdocs-glightbox = {version="*", optional=true}
 
 [tool.poetry.extras]
-docs = ["mkdocs", "mkdocs-jupyter", "mkdocs-material-extensions", "mkdocs-git-revision-date-localized-plugin", "mkdocs-git-authors-plugin", "mkdocs-gitbook"]
+docs = ["mkdocs", "mkdocs-jupyter", "mkdocs-material-extensions", "mkdocs-git-revision-date-localized-plugin", "mkdocs-git-authors-plugin", "mkdocs-gitbook", "mkdocs-glightbox"]
 
 [tool.poetry.dev-dependencies]
 twine = "*"
 pytest = "*"
 pytest-cov = "*"
 pre-commit = "*"
 safety = "*"
```

### Comparing `cognite_neat-0.12.0/PKG-INFO` & `cognite_neat-0.12.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.12.0
+Version: 0.12.1
 Summary: Knowledge graph transformation
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,15 @@
 Requires-Dist: google-auth-oauthlib
 Requires-Dist: graphql-core (>=3.2.3,<4.0.0)
 Requires-Dist: gspread
 Requires-Dist: mkdocs ; extra == "docs"
 Requires-Dist: mkdocs-git-authors-plugin ; extra == "docs"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin ; extra == "docs"
 Requires-Dist: mkdocs-gitbook ; extra == "docs"
+Requires-Dist: mkdocs-glightbox ; extra == "docs"
 Requires-Dist: mkdocs-jupyter ; extra == "docs"
 Requires-Dist: mkdocs-material-extensions ; extra == "docs"
 Requires-Dist: openpyxl
 Requires-Dist: oxrdflib[oxigraph] (>=0.3.3,<0.4.0)
 Requires-Dist: pandas
 Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
 Requires-Dist: pydantic
```
