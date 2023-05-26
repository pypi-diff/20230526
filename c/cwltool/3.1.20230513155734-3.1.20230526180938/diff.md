# Comparing `tmp/cwltool-3.1.20230513155734.tar.gz` & `tmp/cwltool-3.1.20230526180938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwltool-3.1.20230513155734.tar", last modified: Sat May 13 16:25:14 2023, max compression
+gzip compressed data, was "cwltool-3.1.20230526180938.tar", last modified: Fri May 26 18:38:42 2023, max compression
```

## Comparing `cwltool-3.1.20230513155734.tar` & `cwltool-3.1.20230526180938.tar`

### file list

```diff
@@ -1,931 +1,938 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.104286 cwltool-3.1.20230513155734/
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)     4343 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/CONTRIBUTING.md
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     3195 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     7971 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/Makefile
--rw-r--r--   0 michael   (1000) michael   (1000)    47216 2023-05-13 16:25:14.104286 cwltool-3.1.20230513155734/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    38146 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.016284 cwltool-3.1.20230513155734/cwltool/
--rw-r--r--   0 michael   (1000) michael   (1000)      280 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)       81 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    30745 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/argparser.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29589 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/builder.py
--rw-r--r--   0 michael   (1000) michael   (1000)    21318 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/checker.py
--rw-r--r--   0 michael   (1000) michael   (1000)    65608 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/command_line_tool.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9078 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/context.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2341 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/cuda.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6387 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/cwlrdf.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7317 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/cwlviewer.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19183 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/docker.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4319 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/docker_id.py
--rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/env_to_stdout.py
--rw-r--r--   0 michael   (1000) michael   (1000)      346 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/errors.py
--rw-r--r--   0 michael   (1000) michael   (1000)    18167 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/executors.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3545 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/extensions-v1.1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     7950 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/extensions-v1.2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     6788 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/extensions.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2402 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/factory.py
--rw-r--r--   0 michael   (1000) michael   (1000)      704 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/flatten.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4127 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/hello.simg
--rw-r--r--   0 michael   (1000) michael   (1000)    39780 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/job.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.016284 cwltool-3.1.20230513155734/cwltool/jshint/
--rwxr-xr-x   0 michael   (1000) michael   (1000)  1286196 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/jshint/jshint.js
--rw-r--r--   0 michael   (1000) michael   (1000)     1240 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/jshint/jshint_wrapper.js
--rw-r--r--   0 michael   (1000) michael   (1000)    24044 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/load_tool.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1289 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/loghandler.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    53441 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/main.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2612 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/mpi.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3221 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/mutation.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11059 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/pack.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8648 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/pathmapper.py
--rw-r--r--   0 michael   (1000) michael   (1000)    51444 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/process.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4656 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/procgenerator.py
--rw-r--r--   0 michael   (1000) michael   (1000)    39169 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/provenance.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1889 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/provenance_constants.py
--rw-r--r--   0 michael   (1000) michael   (1000)    32925 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/provenance_profile.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/py.typed
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.016284 cwltool-3.1.20230513155734/cwltool/rdfqueries/
--rw-r--r--   0 michael   (1000) michael   (1000)     2722 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/rdfqueries/get_inner_edges.sparql
--rw-r--r--   0 michael   (1000) michael   (1000)     2149 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/rdfqueries/get_input_edges.sparql
--rw-r--r--   0 michael   (1000) michael   (1000)     2134 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/rdfqueries/get_output_edges.sparql
--rw-r--r--   0 michael   (1000) michael   (1000)     2146 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/rdfqueries/get_root.sparql
--rw-r--r--   0 michael   (1000) michael   (1000)     3507 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/resolver.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3679 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/run_job.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.020284 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/
--rw-r--r--   0 michael   (1000) michael   (1000)       53 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    35108 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    33209 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      856 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)       83 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/UserGuide.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    21941 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    18072 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)      985 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)      884 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     7889 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.020284 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1692 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      370 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      235 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10104 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3696 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10837 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      765 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      193 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.0/userguide-intro.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.024284 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)      904 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/CONFORMANCE_TESTS.md
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    47777 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    36571 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      416 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    25923 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    24688 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)      769 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     2402 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      891 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8140 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.032284 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1692 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      370 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      235 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10277 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10837 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      765 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.024284 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/
--rw-r--r--   0 michael   (1000) michael   (1000)       53 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    47285 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    36569 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      423 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    25411 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    24564 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)      769 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)      891 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8140 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.028284 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1692 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      370 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      235 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10277 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10837 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      765 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.032284 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1004 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/CONFORMANCE_TESTS.md
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    51493 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    40072 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    29004 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    29634 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1746 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     2459 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      821 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.056285 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.036285 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    45433 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    38245 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      293 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    27116 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    25563 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1688 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)      960 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.036285 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.040285 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    45578 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    39141 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    27124 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    25563 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1688 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     2466 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      960 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.044285 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.044285 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1004 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/CONFORMANCE_TESTS.md
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    51543 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    40042 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    29054 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    26611 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1245 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     2466 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      960 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.048285 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.048285 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1004 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/CONFORMANCE_TESTS.md
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    51543 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    40064 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    29054 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    29634 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1737 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     2466 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      821 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.004284 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.052285 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2375 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/secrets.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19350 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/singularity.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1094 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/singularity_utils.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6340 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/software_requirements.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1775 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/stdfsaccess.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9751 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/subgraph.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3669 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/task_queue.py
--rw-r--r--   0 michael   (1000) michael   (1000)      540 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/udocker.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11159 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/update.py
--rw-r--r--   0 michael   (1000) michael   (1000)    16416 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/utils.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8837 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/validate_js.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19034 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/workflow.py
--rw-r--r--   0 michael   (1000) michael   (1000)    41279 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool/workflow_job.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.016284 cwltool-3.1.20230513155734/cwltool.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)    47216 2023-05-13 16:25:13.000000 cwltool-3.1.20230513155734/cwltool.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    36537 2023-05-13 16:25:13.000000 cwltool-3.1.20230513155734/cwltool.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-13 16:25:13.000000 cwltool-3.1.20230513155734/cwltool.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       46 2023-05-13 16:25:13.000000 cwltool-3.1.20230513155734/cwltool.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      361 2023-05-13 16:25:13.000000 cwltool-3.1.20230513155734/cwltool.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-05-13 16:25:13.000000 cwltool-3.1.20230513155734/cwltool.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-13 16:24:56.000000 cwltool-3.1.20230513155734/cwltool.egg-info/zip-safe
--rwxr-xr-x   0 michael   (1000) michael   (1000)      335 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/cwltool.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1180 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/gittaggers.py
--rw-r--r--   0 michael   (1000) michael   (1000)       46 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/lint-requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      165 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.060285 cwltool-3.1.20230513155734/mypy-stubs/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.060285 cwltool-3.1.20230513155734/mypy-stubs/arcp/
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/arcp/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      788 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/arcp/parse.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.060285 cwltool-3.1.20230513155734/mypy-stubs/argcomplete/
--rw-r--r--   0 michael   (1000) michael   (1000)      525 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/argcomplete/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1736 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/bagit.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.060285 cwltool-3.1.20230513155734/mypy-stubs/black/
--rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/black/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.060285 cwltool-3.1.20230513155734/mypy-stubs/cachecontrol/
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/cachecontrol/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      194 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/cachecontrol/cache.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.060285 cwltool-3.1.20230513155734/mypy-stubs/cachecontrol/caches/
--rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/cachecontrol/caches/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      843 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/cachecontrol/caches/file_cache.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/cachecontrol/compat.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      425 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/cachecontrol/controller.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      403 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/cachecontrol/wrapper.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.060285 cwltool-3.1.20230513155734/mypy-stubs/coloredlogs/
--rw-r--r--   0 michael   (1000) michael   (1000)      196 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/coloredlogs/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.060285 cwltool-3.1.20230513155734/mypy-stubs/graphviz/
--rw-r--r--   0 michael   (1000) michael   (1000)      495 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/graphviz/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      332 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/graphviz/_compat.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      363 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/graphviz/backend.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2053 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/graphviz/dot.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1862 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/graphviz/files.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      538 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/graphviz/lang.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      271 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/graphviz/tools.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     7565 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/mistune.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.064285 cwltool-3.1.20230513155734/mypy-stubs/prov/
--rw-r--r--   0 michael   (1000) michael   (1000)      170 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/prov/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     6855 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/prov/constants.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1721 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/prov/dot.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1498 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/prov/graph.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1060 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/prov/identifier.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)    15069 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/prov/model.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.064285 cwltool-3.1.20230513155734/mypy-stubs/prov/serializers/
--rw-r--r--   0 michael   (1000) michael   (1000)     1405 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/prov/serializers/provjson.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      255 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/prov/serializers/provn.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     3009 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/prov/serializers/provrdf.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      767 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/prov/serializers/provxml.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     5310 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/pydot.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.064285 cwltool-3.1.20230513155734/mypy-stubs/rdflib/
--rw-r--r--   0 michael   (1000) michael   (1000)     1292 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/collection.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     8337 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/graph.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.064285 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/
--rw-r--r--   0 michael   (1000) michael   (1000)     2010 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_CSVW.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_DC.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1034 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_DCAT.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2361 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1109 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_DOAP.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1847 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_FOAF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4691 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_ODRL2.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1259 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_ORG.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2260 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_OWL.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      441 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_PROF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4520 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_PROV.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1105 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_QB.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_RDF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      519 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_RDFS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)    41401 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_SDO.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4965 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_SH.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      943 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_SKOS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1075 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_SOSA.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_SSN.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2462 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_TIME.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_VOID.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_XSD.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2282 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      724 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/paths.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      325 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/plugin.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.064285 cwltool-3.1.20230513155734/mypy-stubs/rdflib/plugins/
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/plugins/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.064285 cwltool-3.1.20230513155734/mypy-stubs/rdflib/plugins/parsers/
--rw-r--r--   0 michael   (1000) michael   (1000)      126 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1354 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/query.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1370 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/resource.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1337 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/rdflib/term.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.064285 cwltool-3.1.20230513155734/mypy-stubs/ruamel/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/ruamel/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.068285 cwltool-3.1.20230513155734/mypy-stubs/shellescape/
--rw-r--r--   0 michael   (1000) michael   (1000)      147 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/shellescape/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      104 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/shellescape/main.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)    34792 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/subprocess.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.068285 cwltool-3.1.20230513155734/mypy-stubs/urllib/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/urllib/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5488 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy-stubs/urllib/parse.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      258 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/mypy.ini
--rw-r--r--   0 michael   (1000) michael   (1000)      492 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/pyproject.toml
--rw-r--r--   0 michael   (1000) michael   (1000)      496 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      251 2023-05-13 16:25:14.104286 cwltool-3.1.20230513155734/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     6292 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/setup.py
--rw-r--r--   0 michael   (1000) michael   (1000)      218 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/test-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.076286 cwltool-3.1.20230513155734/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)      671 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/2.fasta
--rw-r--r--   0 michael   (1000) michael   (1000)      255 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/2.fastq
--rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      340 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/arg-empty-prefix-separate-false.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     3735 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/bundle-context.jsonld
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.076286 cwltool-3.1.20230513155734/tests/checker_wf/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1358 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/checker_wf/broken-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1350 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/checker_wf/broken-wf2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      776 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/checker_wf/broken-wf3.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      255 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/checker_wf/broken-wf4.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      196 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/checker_wf/cat-a.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      188 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/checker_wf/cat.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      543 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/checker_wf/circ-dep-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      534 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/checker_wf/circ-dep-wf2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      215 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/checker_wf/echo.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1283 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/checker_wf/functional-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      185 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/checker_wf/ls.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      359 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/checker_wf/optional_array_mismatch.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)        2 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/checker_wf/test.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)      257 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/checker_wf/wc.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.076286 cwltool-3.1.20230513155734/tests/cwl-conformance/
--rw-r--r--   0 michael   (1000) michael   (1000)     1063 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/cwl-conformance/cwltool-conftest.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      205 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/debian_image_id.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      215 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/debian_image_id2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      339 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/default_values_list.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      517 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/echo-badposition-expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/echo-job.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)       14 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/echo-position-expr-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/echo-position-expr.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      313 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/echo-stderr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      178 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/echo-stdout-log-dir.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      297 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/echo.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      167 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/echo_broken_outputs.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      280 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/env.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      285 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/env2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      145 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/env3.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      360 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/env4.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      157 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/env_with_software_req.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.080286 cwltool-3.1.20230513155734/tests/input_deps/
--rw-r--r--   0 michael   (1000) michael   (1000)      202 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/input_deps/docker-array-secondaryfiles-job.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1081 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/input_deps/docker-array-secondaryfiles.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)    12010 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/input_deps/ref.fasta
--rw-r--r--   0 michael   (1000) michael   (1000)      193 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/input_deps/ref.fasta.fai
--rw-r--r--   0 michael   (1000) michael   (1000)    12010 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/input_deps/ref2.fasta
--rw-r--r--   0 michael   (1000) michael   (1000)      193 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/input_deps/ref2.fasta.fai
--rw-r--r--   0 michael   (1000) michael   (1000)      510 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/iwdr_bad_expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      506 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/iwdr_dir_literal_real_file.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/listing-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/listing2-job.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.080286 cwltool-3.1.20230513155734/tests/loop/
--rw-r--r--   0 michael   (1000) michael   (1000)      590 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/all-output-loop-no-iteration.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      591 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/all-output-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1038 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/default-value-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      558 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/invalid-loop-command-line-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      409 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/invalid-loop-expression-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      584 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/invalid-loop-hint.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      725 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/invalid-loop-scatter.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      733 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/invalid-loop-when.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      695 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/invalid-loop-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1518 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/invalid-multi-source-loop-no-requirement.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      669 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/invalid-no-loopWhen.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      700 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/invalid-non-boolean-loopWhen.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/invalid-value-from-loop-no-requirement.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1311 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/loop-inside-loop-all.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1246 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/loop-inside-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/loop-inside-scatter-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1076 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/loop-inside-scatter.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1556 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/multi-source-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/single-var-loop-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      590 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/single-var-loop-no-iteration.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      591 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/single-var-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      637 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/two-vars-loop-2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       11 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/two-vars-loop-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      691 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/two-vars-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      711 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/loop/value-from-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      371 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/non_portable.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      406 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/non_portable2.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.080286 cwltool-3.1.20230513155734/tests/override/
--rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/override/echo-job-ov.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      144 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/override/echo-job-ov2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/override/echo-job.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)      211 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/override/echo-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      427 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/override/echo.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      206 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/override/env-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      133 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/override/env-tool_cwl-requirement_override.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      168 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/override/env-tool_cwl-requirement_override_default.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      187 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/override/env-tool_cwl-requirement_override_default_wrongver.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      213 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/override/env-tool_v1.1.0-dev1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      206 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/override/env-tool_v1.1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      116 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/override/ov.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      127 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/override/ov2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      119 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/override/ov3.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      413 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/portable.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      530 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/random_lines.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      100 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/random_lines_job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/random_lines_mapping.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.080286 cwltool-3.1.20230513155734/tests/reloc/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.080286 cwltool-3.1.20230513155734/tests/reloc/dir1/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/reloc/dir1/foo
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.080286 cwltool-3.1.20230513155734/tests/reloc/dir2/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/reloc/dir2/foo
--rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/reloc/test.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1063 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/scatter_numbers.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/secondary-files-bad.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       45 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/secondary-files-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      369 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/secondary-files-string-v1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      609 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/secondary-files.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      430 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/seqtk_seq.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       69 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/seqtk_seq_job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      504 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/seqtk_seq_with_docker.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      539 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/seqtk_seq_wrong_name.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      206 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/sing_pullfolder_test.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.084286 cwltool-3.1.20230513155734/tests/subgraph/
--rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/1432.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      946 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/count-lines1-wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     4722 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/count-lines17-wf.cwl.json
--rw-r--r--   0 michael   (1000) michael   (1000)       31 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/env-job.json
--rw-r--r--   0 michael   (1000) michael   (1000)      260 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/env-tool2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      190 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/env-tool2_no_env.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/env-tool2_req.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      298 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/env-wf2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      291 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/env-wf2_hint_collision.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      295 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/env-wf2_hint_req_collision.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      307 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/env-wf2_long.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      315 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/env-wf2_only_hint.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      302 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/env-wf2_req_collision.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     3679 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/env-wf2_subwf-packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      340 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/env-wf2_subwf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/env-wf2_subwf_b.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1181 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/extract_count_output.json
--rw-r--r--   0 michael   (1000) michael   (1000)     2623 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/extract_file1.json
--rw-r--r--   0 michael   (1000) michael   (1000)      854 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/extract_file2.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/extract_file3.json
--rw-r--r--   0 michael   (1000) michael   (1000)      854 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/extract_output3.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1232 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/extract_output4.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/extract_output5.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1788 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/extract_step1.json
--rw-r--r--   0 michael   (1000) michael   (1000)      810 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/extract_step2.json
--rw-r--r--   0 michael   (1000) michael   (1000)      818 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/extract_step2_1432.json
--rw-r--r--   0 michael   (1000) michael   (1000)      854 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/extract_step3.json
--rw-r--r--   0 michael   (1000) michael   (1000)      861 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/extract_step4.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/extract_step5.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      279 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/parseInt-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1162 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/single_step1.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1189 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/single_step2.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1230 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/single_step3.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1245 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/single_step4.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1584 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/single_step5.json
--rw-r--r--   0 michael   (1000) michael   (1000)      538 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/steplevel-resreq.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      803 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/timelimit2-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      301 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/subgraph/wc-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5329 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_anon_types.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      558 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_bad_outputs_wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      376 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_check.py
--rw-r--r--   0 michael   (1000) michael   (1000)      563 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_conditionals.py
--rw-r--r--   0 michael   (1000) michael   (1000)      794 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_content_type.py
--rw-r--r--   0 michael   (1000) michael   (1000)      820 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_context.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9294 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_cuda.py
--rw-r--r--   0 michael   (1000) michael   (1000)      369 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_cwl_version.py
--rw-r--r--   0 michael   (1000) michael   (1000)      562 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_default_path.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5651 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_dependencies.py
--rw-r--r--   0 michael   (1000) michael   (1000)       55 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_deps_env_modules_resolvers_conf.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       60 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_deps_env_resolvers_conf.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_deps_env_resolvers_conf_rewrite.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      101 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_deps_mapping.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3881 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_docker.py
--rw-r--r--   0 michael   (1000) michael   (1000)      414 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_docker_info.py
--rw-r--r--   0 michael   (1000) michael   (1000)      845 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_docker_paths_with_colons.py
--rw-r--r--   0 michael   (1000) michael   (1000)      513 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_empty_input.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8204 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_environment.py
--rw-r--r--   0 michael   (1000) michael   (1000)    62418 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_examples.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7431 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_ext.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2533 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_fetch.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2487 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_http_input.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4335 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_input_deps.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10931 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_iwdr.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4452 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_js_sandbox.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6890 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_load_tool.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8993 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_loop.py
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_make_template.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2761 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_misc_cli.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11953 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_mpi.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3979 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_override.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7708 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_pack.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1126 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_parallel.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6158 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_path_checks.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2682 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_pathmapper.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1382 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_procgenerator.py
--rw-r--r--   0 michael   (1000) michael   (1000)    27748 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_provenance.py
--rw-r--r--   0 michael   (1000) michael   (1000)      589 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_rdfprint.py
--rw-r--r--   0 michael   (1000) michael   (1000)      526 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_recursive_validation.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1232 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_relocate.py
--rw-r--r--   0 michael   (1000) michael   (1000)      319 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_schemadef.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3034 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_secrets.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4596 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_singularity.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4443 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_singularity_versions.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1870 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_stdout_stderr_log_dir.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2725 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_streaming.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1730 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_subclass_mypyc.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11067 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_subgraph.py
--rw-r--r--   0 michael   (1000) michael   (1000)      936 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_target.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9930 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_tmpdir.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5691 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_toolargparse.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4342 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_trs.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3463 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_udocker.py
--rw-r--r--   0 michael   (1000) michael   (1000)      596 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_validate.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2170 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_validate_js.py
--rw-r--r--   0 michael   (1000) michael   (1000)      867 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/test_windows_warning.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.008284 cwltool-3.1.20230513155734/tests/tmp1/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.008284 cwltool-3.1.20230513155734/tests/tmp1/tmp2/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.084286 cwltool-3.1.20230513155734/tests/tmp1/tmp2/tmp3/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/tmp1/tmp2/tmp3/.gitkeep
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.008284 cwltool-3.1.20230513155734/tests/tmp4/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.084286 cwltool-3.1.20230513155734/tests/tmp4/alpha/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/tmp4/alpha/baker
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/tmp4/alpha/charlie
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/tmp4/alpha/delta
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/tmp4/alpha/echo
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/tmp4/alpha/foxtrot
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.084286 cwltool-3.1.20230513155734/tests/trs/
--rw-r--r--   0 michael   (1000) michael   (1000)     1505 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/trs/Dockstore.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      821 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/trs/md5sum-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/trs/md5sum-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/utf_doc_example.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5127 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/util.py
--rw-r--r--   0 michael   (1000) michael   (1000)      236 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wc-tool-bad-hints.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wc-tool-bad-reqs.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.100286 cwltool-3.1.20230513155734/tests/wf/
--rw-r--r--   0 michael   (1000) michael   (1000)      286 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/1496.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      468 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/1590.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      373 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/1st-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      181 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/811-12.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      178 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/811.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       26 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/811_inputs.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      212 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/816_tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      155 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/816_wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      650 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/910.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/arguments.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      254 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/bad-stderr-expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      225 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/bad-stdin-expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      239 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/bad-stdout-expr.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      523 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/bad_formattest.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/bad_formattest2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      222 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/bad_networkaccess.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/bad_timelimit.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/badout1.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      304 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/badout2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/badout3.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      272 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/cache_test_workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/cat-tool.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      130 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/cat.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/conditional_step_no_inputs.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      644 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/conflict.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      266 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/cores_float.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      388 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/count-lines1-wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      409 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/default-dir5.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/default-wf5.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      212 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/default_path.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      210 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/dir_deps.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1479 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/directory.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1420 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/double-nested.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/echo.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/empty.ttl
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/empty2.ttl
--rw-r--r--   0 michael   (1000) michael   (1000)      922 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/expect_iwd-passthrough1_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     4397 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/expect_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     4564 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/expect_revsort_datetime_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     4574 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/expect_trick_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      619 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/floats_small_and_large.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      120 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/formattest-job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      412 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/formattest.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.100286 cwltool-3.1.20230513155734/tests/wf/generator/
--rw-r--r--   0 michael   (1000) michael   (1000)      709 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/generator/pytoolgen.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      275 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/generator/zing.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      672 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/hello-workflow-badhints.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      673 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/hello-workflow-badhints2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      657 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/hello-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       35 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/hello.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)      168 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/hello_single_tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      580 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/iwd-passthrough1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      230 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/iwdr-empty.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      414 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/iwdr-entry.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1775 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/iwdr-passthrough-successive.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2268 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/iwdr_permutations.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      155 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/iwdr_permutations_inplace.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1016 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/iwdr_permutations_nocontainer.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      282 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/js_output.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      364 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/js_output_workflow.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      291 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/listing_deep.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      276 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/listing_none.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/listing_shallow.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      158 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/listing_v1_0.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       35 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/literalfile-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/literalfile.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/malformed_outputs.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      145 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/missing-tool.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      548 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/missing_cwlVersion.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      249 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/mpi_env.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      644 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/mpi_expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/mpi_expr.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      401 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/mpi_line_count.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      470 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/mpi_simple.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      640 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/mpi_simple_wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/mut.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/mut2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      281 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/mut3.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1107 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/nested.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      362 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/networkaccess-fail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      425 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/networkaccess.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      233 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/no-parameters-echo.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/nvidia-smi-cc.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      434 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/nvidia-smi-container.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      382 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/nvidia-smi-max.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      408 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/nvidia-smi-range.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      429 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/nvidia-smi.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-13 16:25:14.104286 cwltool-3.1.20230513155734/tests/wf/operation/
--rw-r--r--   0 michael   (1000) michael   (1000)      442 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/operation/abstract-cosifer.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5209 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/operation/expect_operation-single_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      969 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/operation/operation-single.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      337 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/optional-numerical-output-0.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      174 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/optional_src_mandatory_sink.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      221 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/override-no-secrets.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1921 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/packed-with-loadlisting.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1056 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/packed_no_main.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      786 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/paramref_arguments_roundtrip.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      877 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/paramref_arguments_self.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      279 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/parseInt-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      984 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/record_outputeval.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      377 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/resreq_expr_float_v1_0.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      377 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/resreq_expr_float_v1_2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      152 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/revsort-job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2331 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/revsort.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2447 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/revsort_datetime.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2317 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/revsort_step_bad_schema.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1367 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/revtool.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1471 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/revtool_bad_schema.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       62 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/scatter-job2.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      927 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/scatter-wf4.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2999 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/scatter-wf4.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1563 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/scatter2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1805 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/scatter2_subwf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      703 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/scatterfail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)    94112 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/schemadef-bug-1473.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      412 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/schemadef-tool-12.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      412 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/schemadef-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      158 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/schemadef-type.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      163 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/sec-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      948 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/sec-wf-out.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      214 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/sec-wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      403 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/secret_job.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      380 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/secret_wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      363 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/separate_without_prefix.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1101 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/sorttool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      391 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/storage_float.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/tar-param.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1124 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/three_step_color.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      222 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/timelimit-fail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      277 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/timelimit.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      304 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/touch_tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      278 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/trick_defaults.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      260 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/trick_defaults2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2400 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/trick_revsort.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      318 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/updatedir.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      431 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/updatedir_inplace.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      488 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/updateval.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      102 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/updateval.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      603 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/updateval_inplace.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      382 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/vf-concat.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       82 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/wc-job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      301 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/wc-tool.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      639 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/wffail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1111 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/whale.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      329 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/workreuse-fail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      392 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/workreuse.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      565 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/wf/wrong_cwlVersion.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      150 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/with_doc.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tests/without_doc.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2137 2023-05-13 16:24:48.000000 cwltool-3.1.20230513155734/tox.ini
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.440960 cwltool-3.1.20230526180938/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     4343 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/CONTRIBUTING.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3195 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     7977 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)    47216 2023-05-26 18:38:42.440960 cwltool-3.1.20230526180938/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    38146 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.968949 cwltool-3.1.20230526180938/cwltool/
+-rw-r--r--   0 michael   (1000) michael   (1000)      280 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       81 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    30745 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/argparser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29613 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/builder.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    21318 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/checker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    65632 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/command_line_tool.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9085 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/context.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2341 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/cuda.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.976950 cwltool-3.1.20230526180938/cwltool/cwlprov/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5198 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/cwlprov/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1887 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/cwlprov/provenance_constants.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    32956 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/cwlprov/provenance_profile.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23810 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/cwlprov/ro.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10899 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/cwlprov/writablebagfile.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6386 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/cwlrdf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7317 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/cwlviewer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19183 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/docker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4319 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/docker_id.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/env_to_stdout.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      346 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/errors.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    18175 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/executors.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3545 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/extensions-v1.1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     7950 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/extensions-v1.2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     6788 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/extensions.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2402 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/factory.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      704 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/flatten.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4127 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/hello.simg
+-rw-r--r--   0 michael   (1000) michael   (1000)    39805 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/job.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.980950 cwltool-3.1.20230526180938/cwltool/jshint/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)  1286196 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/jshint/jshint.js
+-rw-r--r--   0 michael   (1000) michael   (1000)     1240 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/jshint/jshint_wrapper.js
+-rw-r--r--   0 michael   (1000) michael   (1000)    24043 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/load_tool.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1289 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/loghandler.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    53616 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/main.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2612 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/mpi.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3221 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/mutation.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11058 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/pack.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8648 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/pathmapper.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    51405 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/process.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4655 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/procgenerator.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/py.typed
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.980950 cwltool-3.1.20230526180938/cwltool/rdfqueries/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2722 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/rdfqueries/get_inner_edges.sparql
+-rw-r--r--   0 michael   (1000) michael   (1000)     2149 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/rdfqueries/get_input_edges.sparql
+-rw-r--r--   0 michael   (1000) michael   (1000)     2134 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/rdfqueries/get_output_edges.sparql
+-rw-r--r--   0 michael   (1000) michael   (1000)     2146 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/rdfqueries/get_root.sparql
+-rw-r--r--   0 michael   (1000) michael   (1000)     3507 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/resolver.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3679 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/run_job.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.920948 cwltool-3.1.20230526180938/cwltool/schemas/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.984950 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)       53 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    35108 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    33209 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      856 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       83 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/UserGuide.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    21941 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    18072 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      985 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      884 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     7889 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.916948 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.916948 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.008950 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1692 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      370 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      235 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10104 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3696 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10837 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      765 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      193 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.0/userguide-intro.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.016950 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      904 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/CONFORMANCE_TESTS.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    47777 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    36571 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      416 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    25923 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    24688 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      769 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     2402 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      891 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8140 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.916948 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.920948 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.064952 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1692 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      370 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      235 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10277 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10837 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      765 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.028951 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/
+-rw-r--r--   0 michael   (1000) michael   (1000)       53 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    47285 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    36569 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      423 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    25411 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    24564 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      769 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      891 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8140 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.916948 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.916948 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.052951 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1692 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      370 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      235 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10277 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10837 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      765 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.080952 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1004 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/CONFORMANCE_TESTS.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    51493 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    40072 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    29004 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    29634 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1746 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     2459 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      821 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.920948 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.920948 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.212955 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.096952 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    45433 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    38245 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      293 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    27116 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    25563 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1688 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      960 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.920948 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.920948 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.104952 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.120953 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    45578 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    39141 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    27124 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    25563 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1688 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     2466 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      960 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.920948 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.920948 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.148953 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.152953 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1004 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/CONFORMANCE_TESTS.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    51543 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    40042 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    29054 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    26611 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1245 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     2466 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      960 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.920948 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.920948 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.164954 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.184954 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1004 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/CONFORMANCE_TESTS.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    51543 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    40064 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    29054 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    29634 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1737 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     2466 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      821 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.920948 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.920948 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.192954 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2375 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/secrets.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19350 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/singularity.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1094 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/singularity_utils.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6340 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/software_requirements.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1775 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/stdfsaccess.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9751 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/subgraph.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3669 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/task_queue.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      540 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/udocker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11158 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/update.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    16509 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/utils.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8824 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/validate_js.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19090 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/workflow.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    41287 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool/workflow_job.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.972950 cwltool-3.1.20230526180938/cwltool.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)    47216 2023-05-26 18:38:41.000000 cwltool-3.1.20230526180938/cwltool.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    36734 2023-05-26 18:38:41.000000 cwltool-3.1.20230526180938/cwltool.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-26 18:38:41.000000 cwltool-3.1.20230526180938/cwltool.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       46 2023-05-26 18:38:41.000000 cwltool-3.1.20230526180938/cwltool.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      361 2023-05-26 18:38:41.000000 cwltool-3.1.20230526180938/cwltool.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-05-26 18:38:41.000000 cwltool-3.1.20230526180938/cwltool.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-26 18:37:51.000000 cwltool-3.1.20230526180938/cwltool.egg-info/zip-safe
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      335 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/cwltool.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1336 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/gittaggers.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       46 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/lint-requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      165 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.224955 cwltool-3.1.20230526180938/mypy-stubs/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.224955 cwltool-3.1.20230526180938/mypy-stubs/arcp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/arcp/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      788 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/arcp/parse.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.228955 cwltool-3.1.20230526180938/mypy-stubs/argcomplete/
+-rw-r--r--   0 michael   (1000) michael   (1000)      525 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/argcomplete/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1736 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/bagit.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.228955 cwltool-3.1.20230526180938/mypy-stubs/black/
+-rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/black/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.228955 cwltool-3.1.20230526180938/mypy-stubs/cachecontrol/
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/cachecontrol/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      194 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/cachecontrol/cache.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.228955 cwltool-3.1.20230526180938/mypy-stubs/cachecontrol/caches/
+-rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/cachecontrol/caches/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      843 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/cachecontrol/caches/file_cache.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/cachecontrol/compat.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      425 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/cachecontrol/controller.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      403 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/cachecontrol/wrapper.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.228955 cwltool-3.1.20230526180938/mypy-stubs/coloredlogs/
+-rw-r--r--   0 michael   (1000) michael   (1000)      196 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/coloredlogs/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.232955 cwltool-3.1.20230526180938/mypy-stubs/graphviz/
+-rw-r--r--   0 michael   (1000) michael   (1000)      495 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/graphviz/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      332 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/graphviz/_compat.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      363 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/graphviz/backend.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2053 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/graphviz/dot.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1862 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/graphviz/files.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      538 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/graphviz/lang.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      271 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/graphviz/tools.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.232955 cwltool-3.1.20230526180938/mypy-stubs/importlib_metadata/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5101 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/importlib_metadata/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      842 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/importlib_metadata/_meta.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     7565 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/mistune.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.232955 cwltool-3.1.20230526180938/mypy-stubs/prov/
+-rw-r--r--   0 michael   (1000) michael   (1000)      170 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/prov/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     6855 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/prov/constants.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1721 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/prov/dot.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1498 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/prov/graph.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1060 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/prov/identifier.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    15085 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/prov/model.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.232955 cwltool-3.1.20230526180938/mypy-stubs/prov/serializers/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1405 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/prov/serializers/provjson.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      255 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/prov/serializers/provn.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     3009 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/prov/serializers/provrdf.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      767 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/prov/serializers/provxml.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     5310 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/pydot.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.240955 cwltool-3.1.20230526180938/mypy-stubs/rdflib/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1292 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/collection.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     8337 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/graph.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.256956 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2010 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_CSVW.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_DC.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1034 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_DCAT.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2361 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1109 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_DOAP.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1847 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_FOAF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4691 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_ODRL2.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1259 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_ORG.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2260 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_OWL.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      441 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_PROF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4520 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_PROV.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1105 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_QB.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_RDF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      519 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_RDFS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    41401 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_SDO.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4965 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_SH.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      943 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_SKOS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1075 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_SOSA.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_SSN.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2462 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_TIME.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_VOID.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_XSD.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2282 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      724 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/paths.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      325 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/plugin.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.256956 cwltool-3.1.20230526180938/mypy-stubs/rdflib/plugins/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/plugins/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.256956 cwltool-3.1.20230526180938/mypy-stubs/rdflib/plugins/parsers/
+-rw-r--r--   0 michael   (1000) michael   (1000)      126 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1354 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/query.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1370 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/resource.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1337 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/rdflib/term.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.256956 cwltool-3.1.20230526180938/mypy-stubs/ruamel/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/ruamel/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.256956 cwltool-3.1.20230526180938/mypy-stubs/shellescape/
+-rw-r--r--   0 michael   (1000) michael   (1000)      147 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/shellescape/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      104 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/shellescape/main.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    34792 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/subprocess.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.260956 cwltool-3.1.20230526180938/mypy-stubs/urllib/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/urllib/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5488 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy-stubs/urllib/parse.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      258 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/mypy.ini
+-rw-r--r--   0 michael   (1000) michael   (1000)      525 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/pyproject.toml
+-rw-r--r--   0 michael   (1000) michael   (1000)      617 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      251 2023-05-26 18:38:42.440960 cwltool-3.1.20230526180938/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     6575 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/setup.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      218 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/test-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.308957 cwltool-3.1.20230526180938/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)      671 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/2.fasta
+-rw-r--r--   0 michael   (1000) michael   (1000)      255 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/2.fastq
+-rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      340 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/arg-empty-prefix-separate-false.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     3735 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/bundle-context.jsonld
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.316957 cwltool-3.1.20230526180938/tests/checker_wf/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1358 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/checker_wf/broken-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1350 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/checker_wf/broken-wf2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      776 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/checker_wf/broken-wf3.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      255 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/checker_wf/broken-wf4.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      196 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/checker_wf/cat-a.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      188 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/checker_wf/cat.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      543 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/checker_wf/circ-dep-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      534 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/checker_wf/circ-dep-wf2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      215 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/checker_wf/echo.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1283 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/checker_wf/functional-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      185 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/checker_wf/ls.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      359 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/checker_wf/optional_array_mismatch.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        2 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/checker_wf/test.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      257 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/checker_wf/wc.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.316957 cwltool-3.1.20230526180938/tests/cwl-conformance/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1063 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/cwl-conformance/cwltool-conftest.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      205 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/debian_image_id.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      215 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/debian_image_id2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      339 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/default_values_list.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      517 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/echo-badposition-expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/echo-job.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)       14 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/echo-position-expr-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/echo-position-expr.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      313 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/echo-stderr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      178 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/echo-stdout-log-dir.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      297 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/echo.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      167 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/echo_broken_outputs.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      280 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/env.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      285 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/env2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      145 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/env3.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      360 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/env4.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      157 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/env_with_software_req.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.320957 cwltool-3.1.20230526180938/tests/input_deps/
+-rw-r--r--   0 michael   (1000) michael   (1000)      202 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/input_deps/docker-array-secondaryfiles-job.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1081 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/input_deps/docker-array-secondaryfiles.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)    12010 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/input_deps/ref.fasta
+-rw-r--r--   0 michael   (1000) michael   (1000)      193 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/input_deps/ref.fasta.fai
+-rw-r--r--   0 michael   (1000) michael   (1000)    12010 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/input_deps/ref2.fasta
+-rw-r--r--   0 michael   (1000) michael   (1000)      193 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/input_deps/ref2.fasta.fai
+-rw-r--r--   0 michael   (1000) michael   (1000)      510 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/iwdr_bad_expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      506 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/iwdr_dir_literal_real_file.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/listing-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/listing2-job.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.328957 cwltool-3.1.20230526180938/tests/loop/
+-rw-r--r--   0 michael   (1000) michael   (1000)      590 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/all-output-loop-no-iteration.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      591 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/all-output-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1038 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/default-value-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      558 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/invalid-loop-command-line-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      409 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/invalid-loop-expression-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      584 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/invalid-loop-hint.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      725 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/invalid-loop-scatter.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      733 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/invalid-loop-when.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      695 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/invalid-loop-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1518 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/invalid-multi-source-loop-no-requirement.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      669 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/invalid-no-loopWhen.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      700 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/invalid-non-boolean-loopWhen.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/invalid-value-from-loop-no-requirement.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1311 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/loop-inside-loop-all.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1246 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/loop-inside-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/loop-inside-scatter-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1076 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/loop-inside-scatter.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1556 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/multi-source-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/single-var-loop-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      590 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/single-var-loop-no-iteration.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      591 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/single-var-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      637 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/two-vars-loop-2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       11 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/two-vars-loop-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      691 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/two-vars-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      711 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/loop/value-from-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      371 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/non_portable.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      406 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/non_portable2.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.332957 cwltool-3.1.20230526180938/tests/override/
+-rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/override/echo-job-ov.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      144 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/override/echo-job-ov2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/override/echo-job.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      211 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/override/echo-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      427 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/override/echo.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      206 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/override/env-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      133 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/override/env-tool_cwl-requirement_override.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      168 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/override/env-tool_cwl-requirement_override_default.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      187 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/override/env-tool_cwl-requirement_override_default_wrongver.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      213 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/override/env-tool_v1.1.0-dev1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      206 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/override/env-tool_v1.1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      116 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/override/ov.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      127 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/override/ov2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      119 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/override/ov3.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      413 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/portable.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      530 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/random_lines.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      100 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/random_lines_job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/random_lines_mapping.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.332957 cwltool-3.1.20230526180938/tests/reloc/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.336958 cwltool-3.1.20230526180938/tests/reloc/dir1/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/reloc/dir1/foo
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.336958 cwltool-3.1.20230526180938/tests/reloc/dir2/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/reloc/dir2/foo
+-rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/reloc/test.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1063 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/scatter_numbers.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/secondary-files-bad.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       45 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/secondary-files-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      369 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/secondary-files-string-v1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      609 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/secondary-files.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      430 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/seqtk_seq.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       69 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/seqtk_seq_job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      504 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/seqtk_seq_with_docker.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      539 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/seqtk_seq_wrong_name.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      206 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/sing_pullfolder_test.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.348958 cwltool-3.1.20230526180938/tests/subgraph/
+-rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/1432.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      946 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/count-lines1-wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     4722 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/count-lines17-wf.cwl.json
+-rw-r--r--   0 michael   (1000) michael   (1000)       31 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/env-job.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      260 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/env-tool2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      190 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/env-tool2_no_env.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/env-tool2_req.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      298 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/env-wf2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      291 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/env-wf2_hint_collision.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      295 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/env-wf2_hint_req_collision.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      307 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/env-wf2_long.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      315 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/env-wf2_only_hint.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      302 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/env-wf2_req_collision.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     3679 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/env-wf2_subwf-packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      340 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/env-wf2_subwf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/env-wf2_subwf_b.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1181 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/extract_count_output.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     2623 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/extract_file1.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      854 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/extract_file2.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/extract_file3.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      854 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/extract_output3.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1232 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/extract_output4.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/extract_output5.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1788 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/extract_step1.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      810 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/extract_step2.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      818 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/extract_step2_1432.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      854 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/extract_step3.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      861 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/extract_step4.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/extract_step5.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      279 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/parseInt-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1162 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/single_step1.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1189 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/single_step2.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1230 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/single_step3.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1245 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/single_step4.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1584 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/single_step5.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      538 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/steplevel-resreq.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      803 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/timelimit2-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      301 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/subgraph/wc-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5329 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_anon_types.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      558 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_bad_outputs_wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      376 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_check.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      563 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_conditionals.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      794 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_content_type.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      820 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_context.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9294 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_cuda.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      369 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_cwl_version.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      562 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_default_path.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5651 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_dependencies.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       55 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_deps_env_modules_resolvers_conf.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       60 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_deps_env_resolvers_conf.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_deps_env_resolvers_conf_rewrite.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      101 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_deps_mapping.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3881 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_docker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      414 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_docker_info.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      845 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_docker_paths_with_colons.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      513 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_empty_input.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8204 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_environment.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    62418 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_examples.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7431 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_ext.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2533 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_fetch.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2487 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_http_input.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4335 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_input_deps.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10931 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_iwdr.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4452 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_js_sandbox.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6890 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_load_tool.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8993 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_loop.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_make_template.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2761 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_misc_cli.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11953 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_mpi.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3979 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_override.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7708 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_pack.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1126 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_parallel.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6158 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_path_checks.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2682 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_pathmapper.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1382 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_procgenerator.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    28315 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_provenance.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      589 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_rdfprint.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      526 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_recursive_validation.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1232 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_relocate.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      319 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_schemadef.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3034 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_secrets.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4596 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_singularity.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4443 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_singularity_versions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1870 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_stdout_stderr_log_dir.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2725 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_streaming.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1730 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_subclass_mypyc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11067 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_subgraph.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      936 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_target.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9930 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_tmpdir.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5691 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_toolargparse.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4342 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_trs.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3463 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_udocker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      596 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_validate.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2170 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_validate_js.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      867 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/test_windows_warning.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.928948 cwltool-3.1.20230526180938/tests/tmp1/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.928948 cwltool-3.1.20230526180938/tests/tmp1/tmp2/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.348958 cwltool-3.1.20230526180938/tests/tmp1/tmp2/tmp3/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/tmp1/tmp2/tmp3/.gitkeep
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:41.928948 cwltool-3.1.20230526180938/tests/tmp4/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.348958 cwltool-3.1.20230526180938/tests/tmp4/alpha/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/tmp4/alpha/baker
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/tmp4/alpha/charlie
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/tmp4/alpha/delta
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/tmp4/alpha/echo
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/tmp4/alpha/foxtrot
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.352958 cwltool-3.1.20230526180938/tests/trs/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1505 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/trs/Dockstore.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      821 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/trs/md5sum-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/trs/md5sum-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/utf_doc_example.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5127 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/util.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      236 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wc-tool-bad-hints.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wc-tool-bad-reqs.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.432960 cwltool-3.1.20230526180938/tests/wf/
+-rw-r--r--   0 michael   (1000) michael   (1000)      286 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/1496.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      468 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/1590.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      373 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/1st-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      181 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/811-12.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      178 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/811.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       26 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/811_inputs.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      212 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/816_tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      155 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/816_wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      650 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/910.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/arguments.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      254 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/bad-stderr-expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      225 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/bad-stdin-expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      239 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/bad-stdout-expr.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      523 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/bad_formattest.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/bad_formattest2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      222 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/bad_networkaccess.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/bad_timelimit.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/badout1.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      304 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/badout2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/badout3.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      272 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/cache_test_workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/cat-tool.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      130 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/cat.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/conditional_step_no_inputs.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      644 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/conflict.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      266 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/cores_float.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      388 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/count-lines1-wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      409 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/default-dir5.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/default-wf5.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      212 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/default_path.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      210 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/dir_deps.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1479 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/directory.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1420 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/double-nested.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/echo.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/empty.ttl
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/empty2.ttl
+-rw-r--r--   0 michael   (1000) michael   (1000)      922 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/expect_iwd-passthrough1_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     4397 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/expect_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     4564 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/expect_revsort_datetime_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     4574 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/expect_trick_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      619 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/floats_small_and_large.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      120 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/formattest-job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      412 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/formattest.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.440960 cwltool-3.1.20230526180938/tests/wf/generator/
+-rw-r--r--   0 michael   (1000) michael   (1000)      709 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/generator/pytoolgen.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      275 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/generator/zing.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      672 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/hello-workflow-badhints.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      673 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/hello-workflow-badhints2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      657 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/hello-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       35 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/hello.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      168 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/hello_single_tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      580 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/iwd-passthrough1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      230 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/iwdr-empty.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      414 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/iwdr-entry.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1775 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/iwdr-passthrough-successive.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2268 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/iwdr_permutations.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      155 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/iwdr_permutations_inplace.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1016 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/iwdr_permutations_nocontainer.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      282 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/js_output.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      364 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/js_output_workflow.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      291 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/listing_deep.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      276 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/listing_none.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/listing_shallow.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      158 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/listing_v1_0.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       35 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/literalfile-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/literalfile.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/malformed_outputs.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      145 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/missing-tool.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      548 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/missing_cwlVersion.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      249 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/mpi_env.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      644 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/mpi_expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/mpi_expr.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      401 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/mpi_line_count.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      470 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/mpi_simple.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      640 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/mpi_simple_wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/mut.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/mut2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      281 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/mut3.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1107 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/nested.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      362 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/networkaccess-fail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      425 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/networkaccess.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      233 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/no-parameters-echo.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/nvidia-smi-cc.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      434 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/nvidia-smi-container.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      382 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/nvidia-smi-max.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      408 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/nvidia-smi-range.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      429 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/nvidia-smi.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-26 18:38:42.440960 cwltool-3.1.20230526180938/tests/wf/operation/
+-rw-r--r--   0 michael   (1000) michael   (1000)      442 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/operation/abstract-cosifer.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5209 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/operation/expect_operation-single_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      969 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/operation/operation-single.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      337 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/optional-numerical-output-0.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      174 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/optional_src_mandatory_sink.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      221 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/override-no-secrets.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1921 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/packed-with-loadlisting.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1056 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/packed_no_main.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      786 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/paramref_arguments_roundtrip.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      877 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/paramref_arguments_self.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      279 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/parseInt-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      984 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/record_outputeval.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      377 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/resreq_expr_float_v1_0.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      377 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/resreq_expr_float_v1_2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      181 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/revsort-job-shortcut.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      152 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/revsort-job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2331 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/revsort.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2447 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/revsort_datetime.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2317 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/revsort_step_bad_schema.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1367 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/revtool.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1471 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/revtool_bad_schema.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       62 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/scatter-job2.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      927 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/scatter-wf4.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2999 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/scatter-wf4.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1563 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/scatter2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1805 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/scatter2_subwf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      703 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/scatterfail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)    94112 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/schemadef-bug-1473.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      412 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/schemadef-tool-12.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      412 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/schemadef-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      158 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/schemadef-type.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      163 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/sec-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      948 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/sec-wf-out.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      214 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/sec-wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      403 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/secret_job.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      380 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/secret_wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      363 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/separate_without_prefix.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1101 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/sorttool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      391 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/storage_float.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/tar-param.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1124 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/three_step_color.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      222 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/timelimit-fail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      277 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/timelimit.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      304 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/touch_tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      278 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/trick_defaults.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      260 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/trick_defaults2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2400 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/trick_revsort.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      318 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/updatedir.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      431 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/updatedir_inplace.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      488 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/updateval.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      102 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/updateval.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      603 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/updateval_inplace.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      382 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/vf-concat.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       82 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/wc-job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      301 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/wc-tool.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      639 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/wffail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1111 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/whale.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      329 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/workreuse-fail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      392 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/workreuse.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      565 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/wf/wrong_cwlVersion.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      150 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/with_doc.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tests/without_doc.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2137 2023-05-26 18:37:17.000000 cwltool-3.1.20230526180938/tox.ini
```

### Comparing `cwltool-3.1.20230513155734/CODE_OF_CONDUCT.md` & `cwltool-3.1.20230526180938/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/CONTRIBUTING.md` & `cwltool-3.1.20230526180938/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/LICENSE.txt` & `cwltool-3.1.20230526180938/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/MANIFEST.in` & `cwltool-3.1.20230526180938/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/Makefile` & `cwltool-3.1.20230526180938/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #  and documentation
 # make coverage-report to check coverage of the python scripts by the tests
 
 MODULE=cwltool
 
 # `SHELL=bash` doesn't work for some, so don't use BASH-isms like
 # `[[` conditional expressions.
-PYSOURCES=$(wildcard ${MODULE}/**.py tests/*.py) setup.py
+PYSOURCES=$(wildcard ${MODULE}/**.py cwltool/cwlprov/*.py tests/*.py) setup.py
 DEVPKGS=diff_cover pylint pep257 pydocstyle 'tox<4' tox-pyenv \
 	isort wheel autoflake pyupgrade bandit -rlint-requirements.txt\
 	-rtest-requirements.txt -rmypy-requirements.txt -rdocs/requirements.txt
 DEBDEVPKGS=pep8 python-autopep8 pylint python-coverage pydocstyle sloccount \
 	   python-flake8 python-mock shellcheck
 
 VERSION=3.1.$(shell TZ=UTC git log --first-parent --max-count=1 \
@@ -81,15 +81,15 @@
 
 ## docs                   : make the docs
 docs: FORCE
 	cd docs && $(MAKE) html
 
 ## clean                  : clean up all temporary / machine-generated files
 clean: check-python3 FORCE
-	rm -f ${MODULE}/*.pyc tests/*.pyc *.so ${MODULE}/*.so
+	rm -f ${MODULE}/*.pyc tests/*.pyc *.so ${MODULE}/*.so cwltool/cwlprov/*.so
 	rm -Rf ${MODULE}/__pycache__/
 	python setup.py clean --all || true
 	rm -Rf .coverage
 	rm -f diff-cover.html
 
 # Linting and code style related targets
 ## sort_import            : sorting imports using isort: https://github.com/timothycrosley/isort
@@ -173,15 +173,15 @@
 	sloccount $^
 
 list-author-emails:
 	@echo 'name, E-Mail Address'
 	@git log --format='%aN,%aE' | sort -u | grep -v 'root'
 
 mypy3: mypy
-mypy: $(filter-out setup.py gittagger.py,$(PYSOURCES))
+mypy: $(PYSOURCES)
 	if ! test -f $(shell python -c 'import ruamel.yaml; import os.path; print(os.path.dirname(ruamel.yaml.__file__))')/py.typed ; \
 	then \
 		rm -Rf mypy-stubs/ruamel/yaml ; \
 		ln -s $(shell python -c 'import ruamel.yaml; import os.path; print(os.path.dirname(ruamel.yaml.__file__))') \
 			mypy-stubs/ruamel/ ; \
 	fi  # if minimally required ruamel.yaml version is 0.15.99 or greater, than the above can be removed
 	MYPYPATH=$$MYPYPATH:mypy-stubs mypy $^
```

### Comparing `cwltool-3.1.20230513155734/PKG-INFO` & `cwltool-3.1.20230526180938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwltool
-Version: 3.1.20230513155734
+Version: 3.1.20230526180938
 Summary: Common workflow language reference implementation
 Home-page: https://github.com/common-workflow-language/cwltool
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 License: UNKNOWN
 Download-URL: https://github.com/common-workflow-language/cwltool
 Description: #############################################################################################
```

### Comparing `cwltool-3.1.20230513155734/README.rst` & `cwltool-3.1.20230526180938/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/argparser.py` & `cwltool-3.1.20230526180938/cwltool/argparser.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/builder.py` & `cwltool-3.1.20230526180938/cwltool/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,24 +18,23 @@
     cast,
 )
 
 from cwl_utils import expression
 from cwl_utils.file_formats import check_format
 from mypy_extensions import mypyc_attr
 from rdflib import Graph
+from ruamel.yaml.comments import CommentedMap
+from ruamel.yaml.representer import RoundTripRepresenter
+from ruamel.yaml.scalarfloat import ScalarFloat
 from schema_salad.avro.schema import Names, Schema, make_avsc_object
 from schema_salad.exceptions import ValidationException
 from schema_salad.sourceline import SourceLine
 from schema_salad.utils import convert_to_dict, json_dumps
 from schema_salad.validate import validate
 
-from ruamel.yaml.comments import CommentedMap
-from ruamel.yaml.representer import RoundTripRepresenter
-from ruamel.yaml.scalarfloat import ScalarFloat
-
 from .errors import WorkflowException
 from .loghandler import _logger
 from .mutation import MutationManager
 from .software_requirements import DependenciesConfiguration
 from .stdfsaccess import StdFsAccess
 from .utils import (
     CONTENT_LIMIT,
@@ -46,16 +45,18 @@
     aslist,
     get_listing,
     normalizeFilesDirs,
     visit_class,
 )
 
 if TYPE_CHECKING:
+    from .cwlprov.provenance_profile import (
+        ProvenanceProfile,  # pylint: disable=unused-import
+    )
     from .pathmapper import PathMapper
-    from .provenance_profile import ProvenanceProfile  # pylint: disable=unused-import
 
 INPUT_OBJ_VOCAB: Dict[str, str] = {
     "Any": "https://w3id.org/cwl/salad#Any",
     "File": "https://w3id.org/cwl/cwl#File",
     "Directory": "https://w3id.org/cwl/cwl#Directory",
 }
```

### Comparing `cwltool-3.1.20230513155734/cwltool/checker.py` & `cwltool-3.1.20230526180938/cwltool/checker.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/command_line_tool.py` & `cwltool-3.1.20230526180938/cwltool/command_line_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,23 +29,22 @@
     Type,
     Union,
     cast,
 )
 
 import shellescape
 from mypy_extensions import mypyc_attr
+from ruamel.yaml.comments import CommentedMap, CommentedSeq
 from schema_salad.avro.schema import Schema
 from schema_salad.exceptions import ValidationException
 from schema_salad.ref_resolver import file_uri, uri_file_path
 from schema_salad.sourceline import SourceLine
 from schema_salad.utils import json_dumps
 from schema_salad.validate import validate_ex
 
-from ruamel.yaml.comments import CommentedMap, CommentedSeq
-
 from .builder import (
     INPUT_OBJ_VOCAB,
     Builder,
     content_limit_respected_read_bytes,
     substitute,
 )
 from .context import LoadingContext, RuntimeContext, getdefault
@@ -83,15 +82,17 @@
     shared_file_lock,
     trim_listing,
     upgrade_lock,
     visit_class,
 )
 
 if TYPE_CHECKING:
-    from .provenance_profile import ProvenanceProfile  # pylint: disable=unused-import
+    from .cwlprov.provenance_profile import (
+        ProvenanceProfile,  # pylint: disable=unused-import
+    )
 
 
 class PathCheckingMode(Enum):
     """
     What characters are allowed in path names.
 
     We have the strict (default) mode and the relaxed mode.
```

### Comparing `cwltool-3.1.20230513155734/cwltool/context.py` & `cwltool-3.1.20230526180938/cwltool/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,34 +14,33 @@
     List,
     Optional,
     TextIO,
     Tuple,
     Union,
 )
 
+from ruamel.yaml.comments import CommentedMap
 from schema_salad.avro.schema import Names
 from schema_salad.ref_resolver import Loader
 from schema_salad.utils import FetcherCallableType
 from typing_extensions import Literal
 
-from ruamel.yaml.comments import CommentedMap
-
 from .mpi import MpiConfig
 from .pathmapper import PathMapper
 from .stdfsaccess import StdFsAccess
 from .utils import DEFAULT_TMP_PREFIX, CWLObjectType, HasReqsHints, ResolverType
 
 if TYPE_CHECKING:
     from cwl_utils.parser.cwl_v1_2 import LoadingOptions
 
     from .builder import Builder
+    from .cwlprov.provenance_profile import ProvenanceProfile
+    from .cwlprov.ro import ResearchObject
     from .mutation import MutationManager
     from .process import Process
-    from .provenance import ResearchObject
-    from .provenance_profile import ProvenanceProfile
     from .secrets import SecretStore
     from .software_requirements import DependenciesConfiguration
 
 
 class ContextBase:
     """Shared kwargs based initilizer for :py:class:`RuntimeContext` and :py:class:`LoadingContext`."""
```

### Comparing `cwltool-3.1.20230513155734/cwltool/cuda.py` & `cwltool-3.1.20230526180938/cwltool/cuda.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/cwlrdf.py` & `cwltool-3.1.20230526180938/cwltool/cwlrdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import urllib
 from codecs import StreamWriter
 from typing import IO, Any, Dict, Iterator, Optional, TextIO, Union, cast
 
 from rdflib import Graph
 from rdflib.query import ResultRow
+from ruamel.yaml.comments import CommentedMap
 from schema_salad.jsonld_context import makerdf
 from schema_salad.utils import ContextType
 
-from ruamel.yaml.comments import CommentedMap
-
 from .cwlviewer import CWLViewer
 from .process import Process
 
 
 def gather(tool: Process, ctx: ContextType) -> Graph:
     g = Graph()
```

### Comparing `cwltool-3.1.20230513155734/cwltool/cwlviewer.py` & `cwltool-3.1.20230526180938/cwltool/cwlviewer.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/docker.py` & `cwltool-3.1.20230526180938/cwltool/docker.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/docker_id.py` & `cwltool-3.1.20230526180938/cwltool/docker_id.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/env_to_stdout.py` & `cwltool-3.1.20230526180938/cwltool/env_to_stdout.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/executors.py` & `cwltool-3.1.20230526180938/cwltool/executors.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 import psutil
 from mypy_extensions import mypyc_attr
 from schema_salad.exceptions import ValidationException
 from schema_salad.sourceline import SourceLine
 
 from .command_line_tool import CallbackJob, ExpressionJob
 from .context import RuntimeContext, getdefault
+from .cwlprov.provenance_profile import ProvenanceProfile
 from .errors import WorkflowException
 from .job import JobBase
 from .loghandler import _logger
 from .mutation import MutationManager
 from .process import Process, cleanIntermediate, relocateOutputs
-from .provenance_profile import ProvenanceProfile
 from .task_queue import TaskQueue
 from .update import ORIGINAL_CWLVERSION
 from .utils import CWLObjectType, JobsType
 from .workflow import Workflow
 from .workflow_job import WorkflowJob, WorkflowJobStep
 
 TMPDIR_LOCK = Lock()
```

### Comparing `cwltool-3.1.20230513155734/cwltool/extensions-v1.1.yml` & `cwltool-3.1.20230526180938/cwltool/extensions-v1.1.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/extensions-v1.2.yml` & `cwltool-3.1.20230526180938/cwltool/extensions-v1.2.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/extensions.yml` & `cwltool-3.1.20230526180938/cwltool/extensions.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/factory.py` & `cwltool-3.1.20230526180938/cwltool/factory.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/flatten.py` & `cwltool-3.1.20230526180938/cwltool/flatten.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/hello.simg` & `cwltool-3.1.20230526180938/cwltool/hello.simg`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/job.py` & `cwltool-3.1.20230526180938/cwltool/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,17 @@
     create_tmp_dir,
     ensure_non_writable,
     ensure_writable,
     processes_to_kill,
 )
 
 if TYPE_CHECKING:
-    from .provenance_profile import ProvenanceProfile  # pylint: disable=unused-import
+    from .cwlprov.provenance_profile import (
+        ProvenanceProfile,  # pylint: disable=unused-import
+    )
 needs_shell_quoting_re = re.compile(r"""(^$|[\s|&;()<>\'"$@])""")
 
 FORCE_SHELLED_POPEN = os.getenv("CWLTOOL_FORCE_SHELL_POPEN", "0") == "1"
 
 SHELL_COMMAND_TEMPLATE = """#!/bin/bash
 python3 "run_job.py" "job.json"
 """
```

### Comparing `cwltool-3.1.20230513155734/cwltool/jshint/jshint.js` & `cwltool-3.1.20230526180938/cwltool/jshint/jshint.js`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/jshint/jshint_wrapper.js` & `cwltool-3.1.20230526180938/cwltool/jshint/jshint_wrapper.js`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/load_tool.py` & `cwltool-3.1.20230526180938/cwltool/load_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,29 +17,28 @@
     Optional,
     Tuple,
     Union,
     cast,
 )
 
 from cwl_utils.parser import cwl_v1_2, cwl_v1_2_utils
+from ruamel.yaml.comments import CommentedMap, CommentedSeq
 from schema_salad.exceptions import ValidationException
 from schema_salad.fetcher import Fetcher
 from schema_salad.ref_resolver import Loader, file_uri
 from schema_salad.schema import validate_doc
 from schema_salad.sourceline import SourceLine, cmap
 from schema_salad.utils import (
     ContextType,
     FetcherCallableType,
     IdxResultType,
     ResolveType,
     json_dumps,
 )
 
-from ruamel.yaml.comments import CommentedMap, CommentedSeq
-
 from . import CWL_CONTENT_TYPES, process, update
 from .context import LoadingContext
 from .errors import GraphTargetMissingException
 from .loghandler import _logger
 from .process import Process, get_schema, shortname
 from .update import ALLUPDATES
 from .utils import CWLObjectType, ResolverType, visit_class
```

### Comparing `cwltool-3.1.20230513155734/cwltool/loghandler.py` & `cwltool-3.1.20230526180938/cwltool/loghandler.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/main.py` & `cwltool-3.1.20230526180938/cwltool/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,33 +29,40 @@
     Tuple,
     Union,
     cast,
 )
 
 import argcomplete
 import coloredlogs
-import pkg_resources  # part of setuptools
+import ruamel.yaml
+from importlib_resources import files
+from ruamel.yaml.comments import CommentedMap, CommentedSeq
+from ruamel.yaml.main import YAML
 from schema_salad.exceptions import ValidationException
 from schema_salad.ref_resolver import Loader, file_uri, uri_file_path
 from schema_salad.sourceline import cmap, strip_dup_lineno
 from schema_salad.utils import (
     ContextType,
     FetcherCallableType,
     json_dump,
     json_dumps,
     yaml_no_ts,
 )
 
-import ruamel.yaml
-from ruamel.yaml.comments import CommentedMap, CommentedSeq
-from ruamel.yaml.main import YAML
-
 from . import CWL_CONTENT_TYPES, workflow
 from .argparser import arg_parser, generate_parser, get_default_args
 from .context import LoadingContext, RuntimeContext, getdefault
+from .cwlprov.ro import ResearchObject  # , WritableBagFile
+from .cwlprov.writablebagfile import (  # change this later
+    WritableBagFile,
+    close_ro,
+    create_job,
+    open_log_file_for_activity,
+    packed_workflow,
+)
 from .cwlrdf import printdot, printrdf
 from .errors import (
     ArgumentException,
     GraphTargetMissingException,
     UnsupportedRequirement,
     WorkflowException,
 )
@@ -81,15 +88,14 @@
     mergedirs,
     scandeps,
     shortname,
     use_custom_schema,
     use_standard_schema,
 )
 from .procgenerator import ProcessGenerator
-from .provenance import ResearchObject, WritableBagFile
 from .resolver import ga4gh_tool_registries, tool_resolver
 from .secrets import SecretStore
 from .software_requirements import (
     DependenciesConfiguration,
     get_container_from_software_requirements,
 )
 from .stdfsaccess import StdFsAccess
@@ -635,20 +641,20 @@
 
 def setup_schema(
     args: argparse.Namespace, custom_schema_callback: Optional[Callable[[], None]]
 ) -> None:
     if custom_schema_callback is not None:
         custom_schema_callback()
     elif args.enable_ext:
-        with pkg_resources.resource_stream(__name__, "extensions.yml") as res:
-            ext10 = res.read().decode("utf-8")
-        with pkg_resources.resource_stream(__name__, "extensions-v1.1.yml") as res:
-            ext11 = res.read().decode("utf-8")
-        with pkg_resources.resource_stream(__name__, "extensions-v1.2.yml") as res:
-            ext12 = res.read().decode("utf-8")
+        with files("cwltool").joinpath("extensions.yml") as res:
+            ext10 = res.read_text("utf-8")
+        with files("cwltool").joinpath("extensions-v1.1.yml") as res:
+            ext11 = res.read_text("utf-8")
+        with files("cwltool").joinpath("extensions-v1.2.yml") as res:
+            ext12 = res.read_text("utf-8")
         use_custom_schema("v1.0", "http://commonwl.org/cwltool", ext10)
         use_custom_schema("v1.1", "http://commonwl.org/cwltool", ext11)
         use_custom_schema("v1.2", "http://commonwl.org/cwltool", ext12)
         use_custom_schema("v1.2.0-dev1", "http://commonwl.org/cwltool", ext11)
         use_custom_schema("v1.2.0-dev2", "http://commonwl.org/cwltool", ext11)
         use_custom_schema("v1.2.0-dev3", "http://commonwl.org/cwltool", ext11)
     else:
@@ -688,15 +694,15 @@
     ro = ResearchObject(
         getdefault(runtimeContext.make_fs_access, StdFsAccess)(""),
         temp_prefix_ro=args.tmpdir_prefix,
         orcid=args.orcid,
         full_name=args.cwl_full_name,
     )
     runtimeContext.research_obj = ro
-    log_file_io = ro.open_log_file_for_activity(ro.engine_uuid)
+    log_file_io = open_log_file_for_activity(ro, ro.engine_uuid)
     prov_log_handler = logging.StreamHandler(log_file_io)
 
     prov_log_handler.setFormatter(ProvLogFormatter())
     _logger.addHandler(prov_log_handler)
     _logger.debug("[provenance] Logging to %s", log_file_io)
     if argsl is not None:
         # Log cwltool command line options to provenance file
@@ -1095,15 +1101,15 @@
             processobj = cast(Union[CommentedMap, CommentedSeq], processobj)
             if args.pack:
                 print(print_pack(loadingContext, uri), file=stdout)
                 return 0
 
             if args.provenance and runtimeContext.research_obj:
                 # Can't really be combined with args.pack at same time
-                runtimeContext.research_obj.packed_workflow(print_pack(loadingContext, uri))
+                packed_workflow(runtimeContext.research_obj, print_pack(loadingContext, uri))
 
             if args.print_pre:
                 json_dump(
                     processobj,
                     stdout,
                     indent=4,
                     sort_keys=True,
@@ -1294,15 +1300,15 @@
 
             (out, status) = real_executor(
                 tool, initialized_job_order_object, runtimeContext, logger=_logger
             )
 
             if out is not None:
                 if runtimeContext.research_obj is not None:
-                    runtimeContext.research_obj.create_job(out, True)
+                    create_job(runtimeContext.research_obj, out, True)
 
                     def remove_at_id(doc: CWLObjectType) -> None:
                         for key in list(doc.keys()):
                             if key == "@id":
                                 del doc[key]
                             else:
                                 value = doc[key]
@@ -1379,15 +1385,17 @@
             and runtimeContext
             and runtimeContext.research_obj
             and workflowobj
             and loadingContext
         ):
             research_obj = runtimeContext.research_obj
             if loadingContext.loader is not None:
-                research_obj.generate_snapshot(prov_deps(workflowobj, loadingContext.loader, uri))
+                research_obj.generate_snapshot(
+                    prov_deps(cast(CWLObjectType, processobj), loadingContext.loader, uri)
+                )
             else:
                 _logger.warning(
                     "Unable to generate provenance snapshot "
                     " due to missing loadingContext.loader."
                 )
             if prov_log_handler is not None:
                 # Stop logging so we won't half-log adding ourself to RO
@@ -1397,15 +1405,15 @@
                 prov_log_handler.flush()
                 # Underlying WritableBagFile will add the tagfile to the manifest
                 if prov_log_stream:
                     prov_log_stream.close()
                 # Why not use prov_log_handler.stream ? That is not part of the
                 # public API for logging.StreamHandler
                 prov_log_handler.close()
-            research_obj.close(args.provenance)
+            close_ro(research_obj, args.provenance)
 
         _logger.removeHandler(stderr_handler)
         _logger.addHandler(defaultStreamHandler)
 
 
 def find_default_container(
     builder: HasReqsHints,
```

### Comparing `cwltool-3.1.20230513155734/cwltool/mpi.py` & `cwltool-3.1.20230526180938/cwltool/mpi.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/mutation.py` & `cwltool-3.1.20230526180938/cwltool/mutation.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/pack.py` & `cwltool-3.1.20230526180938/cwltool/pack.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,18 @@
     MutableSequence,
     Optional,
     Set,
     Union,
     cast,
 )
 
+from ruamel.yaml.comments import CommentedMap, CommentedSeq
 from schema_salad.ref_resolver import Loader, SubLoader
 from schema_salad.utils import ResolveType
 
-from ruamel.yaml.comments import CommentedMap, CommentedSeq
-
 from .context import LoadingContext
 from .load_tool import fetch_document, resolve_and_validate_document
 from .process import shortname, uniquename
 from .update import ORDERED_VERSIONS, ORIGINAL_CWLVERSION, update
 from .utils import CWLObjectType, CWLOutputType
 
 LoadRefType = Callable[[Optional[str], str], ResolveType]
```

### Comparing `cwltool-3.1.20230513155734/cwltool/pathmapper.py` & `cwltool-3.1.20230526180938/cwltool/pathmapper.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/process.py` & `cwltool-3.1.20230526180938/cwltool/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,32 +29,31 @@
     Tuple,
     Type,
     Union,
     cast,
 )
 
 from cwl_utils import expression
+from importlib_resources import files
 from mypy_extensions import mypyc_attr
-from pkg_resources import resource_stream
 from rdflib import Graph
+from ruamel.yaml.comments import CommentedMap, CommentedSeq
 from schema_salad.avro.schema import (
     Names,
     Schema,
     SchemaParseException,
     make_avsc_object,
 )
 from schema_salad.exceptions import ValidationException
 from schema_salad.ref_resolver import Loader, file_uri, uri_file_path
 from schema_salad.schema import load_schema, make_avro_schema, make_valid_avro
 from schema_salad.sourceline import SourceLine, strip_dup_lineno
 from schema_salad.utils import convert_to_dict
 from schema_salad.validate import avro_type_name, validate_ex
 
-from ruamel.yaml.comments import CommentedMap, CommentedSeq
-
 from .builder import INPUT_OBJ_VOCAB, Builder
 from .context import LoadingContext, RuntimeContext, getdefault
 from .errors import UnsupportedRequirement, WorkflowException
 from .loghandler import _logger
 from .mpi import MPIRequirementName
 from .pathmapper import MapperEnt, PathMapper
 from .secrets import SecretStore
@@ -76,15 +75,15 @@
     normalizeFilesDirs,
     random_outdir,
     visit_class,
 )
 from .validate_js import validate_js_expressions
 
 if TYPE_CHECKING:
-    from .provenance_profile import ProvenanceProfile
+    from .cwlprov.provenance_profile import ProvenanceProfile
 
 
 class LogAsDebugFilter(logging.Filter):
     def __init__(self, name: str, parent: logging.Logger) -> None:
         """Initialize."""
         name = str(name)
         super().__init__(name)
@@ -191,30 +190,27 @@
 
     cache: Dict[str, Union[str, Graph, bool]] = {}
     version = version.split("#")[-1]
     if ".dev" in version:
         version = ".".join(version.split(".")[:-1])
     for f in cwl_files:
         try:
-            res = resource_stream(__name__, f"schemas/{version}/{f}")
-            cache["https://w3id.org/cwl/" + f] = res.read().decode("UTF-8")
-            res.close()
+            with files("cwltool").joinpath(f"schemas/{version}/{f}") as res:
+                cache["https://w3id.org/cwl/" + f] = res.read_text("UTF-8")
         except OSError:
             pass
 
     for f in salad_files:
         try:
-            res = resource_stream(
-                __name__,
+            with files("cwltool").joinpath(
                 f"schemas/{version}/salad/schema_salad/metaschema/{f}",
-            )
-            cache["https://w3id.org/cwl/salad/schema_salad/metaschema/" + f] = res.read().decode(
-                "UTF-8"
-            )
-            res.close()
+            ) as res:
+                cache["https://w3id.org/cwl/salad/schema_salad/metaschema/" + f] = res.read_text(
+                    "UTF-8"
+                )
         except OSError:
             pass
 
     if version in custom_schemas:
         cache[custom_schemas[version][0]] = custom_schemas[version][1]
         SCHEMA_CACHE[version] = load_schema(custom_schemas[version][0], cache=cache)
     else:
```

### Comparing `cwltool-3.1.20230513155734/cwltool/procgenerator.py` & `cwltool-3.1.20230526180938/cwltool/procgenerator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import copy
 from typing import Dict, Optional, Tuple, cast
 
+from ruamel.yaml.comments import CommentedMap
 from schema_salad.exceptions import ValidationException
 from schema_salad.sourceline import indent
 
-from ruamel.yaml.comments import CommentedMap
-
 from .context import LoadingContext, RuntimeContext
 from .errors import WorkflowException
 from .load_tool import load_tool
 from .loghandler import _logger
 from .process import Process, shortname
 from .utils import CWLObjectType, JobsGeneratorType, OutputCallbackType
```

### Comparing `cwltool-3.1.20230513155734/cwltool/provenance.py` & `cwltool-3.1.20230526180938/cwltool/cwlprov/ro.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,46 @@
-"""
-Stores Research Object including provenance.
+"""Stores class definition of ResearchObject and WritableBagFile."""
 
-See :doc:`/CWLProv`
-"""
-
-import copy
 import datetime
 import hashlib
 import os
-
-try:
-    import pwd
-except ImportError:
-    # Guard against `from .provenance import ...` on windows.
-    # See windows_check() in main.py
-    pass
-import re
 import shutil
 import tempfile
 import uuid
-from array import array
-from collections import OrderedDict
-from getpass import getuser
-from io import FileIO, TextIOWrapper
-from mmap import mmap
 from pathlib import Path, PurePosixPath
 from typing import (
     IO,
     Any,
-    BinaryIO,
-    Callable,
     Dict,
     List,
     MutableMapping,
     MutableSequence,
     Optional,
     Set,
     Tuple,
     Union,
     cast,
 )
 
 import prov.model as provM
 from prov.model import PROV, ProvDocument
-from schema_salad.utils import json_dumps
-from typing_extensions import TypedDict
 
-from .loghandler import _logger
+from ..loghandler import _logger
+from ..stdfsaccess import StdFsAccess
+from ..utils import (
+    CWLObjectType,
+    CWLOutputType,
+    create_tmp_dir,
+    local_path,
+    posix_path,
+    versionstring,
+)
+from . import Aggregate, Annotation, AuthoredBy, _valid_orcid, _whoami, checksum_copy
 from .provenance_constants import (
     ACCOUNT_UUID,
-    CWLPROV,
     CWLPROV_VERSION,
     DATA,
     ENCODING,
     FOAF,
     LOGS,
     METADATA,
     ORCID,
@@ -64,212 +51,14 @@
     SNAPSHOT,
     TEXT_PLAIN,
     USER_UUID,
     UUID,
     WORKFLOW,
     Hasher,
 )
-from .stdfsaccess import StdFsAccess
-from .utils import (
-    CWLObjectType,
-    CWLOutputType,
-    create_tmp_dir,
-    local_path,
-    posix_path,
-    versionstring,
-)
-
-
-def _whoami() -> Tuple[str, str]:
-    """Return the current operating system account as (username, fullname)."""
-    username = getuser()
-    try:
-        fullname = pwd.getpwuid(os.getuid())[4].split(",")[0]
-    except (KeyError, IndexError):
-        fullname = username
-
-    return (username, fullname)
-
-
-class WritableBagFile(FileIO):
-    """Writes files in research object."""
-
-    def __init__(self, research_object: "ResearchObject", rel_path: str) -> None:
-        """Initialize an ROBagIt."""
-        self.research_object = research_object
-        if Path(rel_path).is_absolute():
-            raise ValueError("rel_path must be relative: %s" % rel_path)
-        self.rel_path = rel_path
-        self.hashes = {
-            SHA1: hashlib.sha1(),  # nosec
-            SHA256: hashlib.sha256(),
-            SHA512: hashlib.sha512(),
-        }
-        # Open file in Research Object folder
-        path = os.path.abspath(os.path.join(research_object.folder, local_path(rel_path)))
-        if not path.startswith(os.path.abspath(research_object.folder)):
-            raise ValueError("Path is outside Research Object: %s" % path)
-        _logger.debug("[provenance] Creating WritableBagFile at %s.", path)
-        super().__init__(path, mode="w")
-
-    def write(self, b: Any) -> int:
-        """Write some content to the Bag."""
-        real_b = b if isinstance(b, (bytes, mmap, array)) else b.encode("utf-8")
-        total = 0
-        length = len(real_b)
-        while total < length:
-            ret = super().write(real_b)
-            if ret:
-                total += ret
-        for val in self.hashes.values():
-            # print("Updating hasher %s ", val)
-            val.update(real_b)
-        return total
-
-    def close(self) -> None:
-        # FIXME: Convert below block to a ResearchObject method?
-        if self.rel_path.startswith("data/"):
-            self.research_object.bagged_size[self.rel_path] = self.tell()
-        else:
-            self.research_object.tagfiles.add(self.rel_path)
-
-        super().close()
-        # { "sha1": "f572d396fae9206628714fb2ce00f72e94f2258f" }
-        checksums = {}
-        for name in self.hashes:
-            checksums[name] = self.hashes[name].hexdigest().lower()
-        self.research_object.add_to_manifest(self.rel_path, checksums)
-
-    # To simplify our hash calculation we won't support
-    # seeking, reading or truncating, as we can't do
-    # similar seeks in the current hash.
-    # TODO: Support these? At the expense of invalidating
-    # the current hash, then having to recalculate at close()
-    def seekable(self) -> bool:
-        return False
-
-    def readable(self) -> bool:
-        return False
-
-    def truncate(self, size: Optional[int] = None) -> int:
-        # FIXME: This breaks contract IOBase,
-        # as it means we would have to recalculate the hash
-        if size is not None:
-            raise OSError("WritableBagFile can't truncate")
-        return self.tell()
-
-
-def _check_mod_11_2(numeric_string: str) -> bool:
-    """
-    Validate numeric_string for its MOD-11-2 checksum.
-
-    Any "-" in the numeric_string are ignored.
-
-    The last digit of numeric_string is assumed to be the checksum, 0-9 or X.
-
-    See ISO/IEC 7064:2003 and
-    https://support.orcid.org/knowledgebase/articles/116780-structure-of-the-orcid-identifier
-    """
-    # Strip -
-    nums = numeric_string.replace("-", "")
-    total = 0
-    # skip last (check)digit
-    for num in nums[:-1]:
-        digit = int(num)
-        total = (total + digit) * 2
-    remainder = total % 11
-    result = (12 - remainder) % 11
-    if result == 10:
-        checkdigit = "X"
-    else:
-        checkdigit = str(result)
-    # Compare against last digit or X
-    return nums[-1].upper() == checkdigit
-
-
-def _valid_orcid(orcid: Optional[str]) -> str:
-    """
-    Ensure orcid is a valid ORCID identifier.
-
-    The string must be equivalent to one of these forms:
-
-    0000-0002-1825-0097
-    orcid.org/0000-0002-1825-0097
-    http://orcid.org/0000-0002-1825-0097
-    https://orcid.org/0000-0002-1825-0097
-
-    If the ORCID number or prefix is invalid, a ValueError is raised.
-
-    The returned ORCID string is always in the form of:
-    https://orcid.org/0000-0002-1825-0097
-    """
-    if orcid is None or not orcid:
-        raise ValueError("ORCID cannot be unspecified")
-    # Liberal in what we consume, e.g. ORCID.org/0000-0002-1825-009x
-    orcid = orcid.lower()
-    match = re.match(
-        # Note: concatenated r"" r"" below so we can add comments to pattern
-        # Optional hostname, with or without protocol
-        r"(http://orcid\.org/|https://orcid\.org/|orcid\.org/)?"
-        # alternative pattern, but probably messier
-        # r"^((https?://)?orcid.org/)?"
-        # ORCID number is always 4x4 numerical digits,
-        # but last digit (modulus 11 checksum)
-        # can also be X (but we made it lowercase above).
-        # e.g. 0000-0002-1825-0097
-        # or   0000-0002-1694-233x
-        r"(?P<orcid>(\d{4}-\d{4}-\d{4}-\d{3}[0-9x]))$",
-        orcid,
-    )
-
-    help_url = (
-        "https://support.orcid.org/knowledgebase/articles/"
-        "116780-structure-of-the-orcid-identifier"
-    )
-    if not match:
-        raise ValueError(f"Invalid ORCID: {orcid}\n{help_url}")
-
-    # Conservative in what we produce:
-    # a) Ensure any checksum digit is uppercase
-    orcid_num = match.group("orcid").upper()
-    # b) ..and correct
-    if not _check_mod_11_2(orcid_num):
-        raise ValueError(f"Invalid ORCID checksum: {orcid_num}\n{help_url}")
-
-    # c) Re-add the official prefix https://orcid.org/
-    return "https://orcid.org/%s" % orcid_num
-
-
-Annotation = TypedDict(
-    "Annotation",
-    {
-        "uri": str,
-        "about": str,
-        "content": Optional[Union[str, List[str]]],
-        "oa:motivatedBy": Dict[str, str],
-    },
-)
-Aggregate = TypedDict(
-    "Aggregate",
-    {
-        "uri": Optional[str],
-        "bundledAs": Optional[Dict[str, Any]],
-        "mediatype": Optional[str],
-        "conformsTo": Optional[Union[str, List[str]]],
-        "createdOn": Optional[str],
-        "createdBy": Optional[Dict[str, str]],
-    },
-    total=False,
-)
-# Aggregate.bundledAs is actually type Aggregate, but cyclic definitions are not supported
-AuthoredBy = TypedDict(
-    "AuthoredBy",
-    {"orcid": Optional[str], "name": Optional[str], "uri": Optional[str]},
-    total=False,
-)
 
 
 class ResearchObject:
     """CWLProv Research Object."""
 
     def __init__(
         self,
@@ -289,21 +78,20 @@
         self.tagfiles: Set[str] = set()
         self._file_provenance: Dict[str, Aggregate] = {}
         self._external_aggregates: List[Aggregate] = []
         self.annotations: List[Annotation] = []
         self._content_types: Dict[str, str] = {}
         self.fsaccess = fsaccess
         # These should be replaced by generate_prov_doc when workflow/run IDs are known:
-        self.engine_uuid = "urn:uuid:%s" % uuid.uuid4()
+        self.engine_uuid = f"urn:uuid:{uuid.uuid4()}"
         self.ro_uuid = uuid.uuid4()
-        self.base_uri = "arcp://uuid,%s/" % self.ro_uuid
-        self.cwltool_version = "cwltool %s" % versionstring().split()[-1]
-        ##
-        self.relativised_input_object: CWLObjectType = {}
+        self.base_uri = f"arcp://uuid,{self.ro_uuid}/"
+        self.cwltool_version = f"cwltool {versionstring().split()[-1]}"
         self.has_manifest = False
+        self.relativised_input_object: CWLObjectType = {}
 
         self._initialize()
         _logger.debug("[provenance] Temporary research object: %s", self.folder)
 
     def self_check(self) -> None:
         """Raise ValueError if this RO is closed."""
         if self.closed:
@@ -332,36 +120,15 @@
         """Write fixed bagit header."""
         self.self_check()
         bagit = os.path.join(self.folder, "bagit.txt")
         # encoding: always UTF-8 (although ASCII would suffice here)
         with open(bagit, "w", encoding=ENCODING, newline="\n") as bag_it_file:
             # TODO: \n or \r\n ?
             bag_it_file.write("BagIt-Version: 0.97\n")
-            bag_it_file.write("Tag-File-Character-Encoding: %s\n" % ENCODING)
-
-    def open_log_file_for_activity(self, uuid_uri: str) -> Union[TextIOWrapper, WritableBagFile]:
-        """Begin the per-activity log."""
-        self.self_check()
-        # Ensure valid UUID for safe filenames
-        activity_uuid = uuid.UUID(uuid_uri)
-        if activity_uuid.urn == self.engine_uuid:
-            # It's the engine aka cwltool!
-            name = "engine"
-        else:
-            name = "activity"
-        p = os.path.join(LOGS, f"{name}.{activity_uuid}.txt")
-        _logger.debug(f"[provenance] Opening log file for {name}: {p}")
-        self.add_annotation(activity_uuid.urn, [p], CWLPROV["log"].uri)
-        return self.write_bag_file(p)
-
-    def _finalize(self) -> None:
-        self._write_ro_manifest()
-        self._write_bag_info()
-        if not self.has_manifest:
-            (Path(self.folder) / "manifest-sha1.txt").touch()
+            bag_it_file.write(f"Tag-File-Character-Encoding: {ENCODING}\n")
 
     def user_provenance(self, document: ProvDocument) -> None:
         """Add the user provenance."""
         self.self_check()
         (username, fullname) = _whoami()
 
         if not self.full_name:
@@ -394,27 +161,14 @@
         #   (which again is launched by any of the above)
         #
         # We can't tell in which way, but ultimately we're still
         # acting in behalf of that user (even if we might
         # get their name wrong!)
         document.actedOnBehalfOf(account, user)
 
-    def write_bag_file(
-        self, path: str, encoding: Optional[str] = ENCODING
-    ) -> Union[TextIOWrapper, WritableBagFile]:
-        """Write the bag file into our research object."""
-        self.self_check()
-        # For some reason below throws BlockingIOError
-        # fp = BufferedWriter(WritableBagFile(self, path))
-        bag_file = WritableBagFile(self, path)
-        if encoding is not None:
-            # encoding: match Tag-File-Character-Encoding: UTF-8
-            return TextIOWrapper(cast(BinaryIO, bag_file), encoding=encoding, newline="\n")
-        return bag_file
-
     def add_tagfile(self, path: str, timestamp: Optional[datetime.datetime] = None) -> None:
         """Add tag files to our research object."""
         self.self_check()
         checksums = {}
         # Read file to calculate its checksum
         if os.path.isdir(path):
             return
@@ -449,29 +203,29 @@
     def _ro_aggregates(self) -> List[Aggregate]:
         """Gather dictionary of files to be added to the manifest."""
 
         def guess_mediatype(
             rel_path: str,
         ) -> Tuple[Optional[str], Optional[Union[str, List[str]]]]:
             """Return the mediatypes."""
-            media_types: Dict[str, str] = {
+            media_types: Dict[Union[str, None], str] = {
                 # Adapted from
                 # https://w3id.org/bundle/2014-11-05/#media-types
                 "txt": TEXT_PLAIN,
                 "ttl": 'text/turtle; charset="UTF-8"',
                 "rdf": "application/rdf+xml",
                 "json": "application/json",
                 "jsonld": "application/ld+json",
                 "xml": "application/xml",
                 ##
                 "cwl": 'text/x+yaml; charset="UTF-8"',
                 "provn": 'text/provenance-notation; charset="UTF-8"',
                 "nt": "application/n-triples",
             }
-            conforms_to: Dict[str, str] = {
+            conforms_to: Dict[Union[str, None], str] = {
                 "provn": "http://www.w3.org/TR/2013/REC-prov-n-20130430/",
                 "cwl": "https://w3id.org/cwl/",
             }
 
             prov_conforms_to: Dict[str, str] = {
                 "provn": "http://www.w3.org/TR/2013/REC-prov-n-20130430/",
                 "rdf": "http://www.w3.org/TR/2013/REC-prov-o-20130430/",
@@ -483,60 +237,55 @@
             }
 
             extension: Optional[str] = rel_path.rsplit(".", 1)[-1].lower()
             if extension == rel_path:
                 # No ".", no extension
                 extension = None
 
-            mediatype = None  # type: Optional[str]
-            conformsTo = None  # type: Optional[Union[str, List[str]]]
-            if extension in media_types:
-                mediatype = media_types[extension]
-
-            if extension in conforms_to:
-                # TODO: Open CWL file to read its declared "cwlVersion", e.g.
-                # cwlVersion = "v1.0"
-                conformsTo = conforms_to[extension]
+            mediatype: Optional[str] = media_types.get(extension, None)
+            conformsTo: Optional[Union[str, List[str]]] = conforms_to.get(extension, None)
+            # TODO: Open CWL file to read its declared "cwlVersion", e.g.
+            # cwlVersion = "v1.0"
 
             if rel_path.startswith(posix_path(PROVENANCE)) and extension in prov_conforms_to:
                 if ".cwlprov" in rel_path:
                     # Our own!
                     conformsTo = [
                         prov_conforms_to[extension],
                         CWLPROV_VERSION,
                     ]
                 else:
                     # Some other PROV
                     # TODO: Recognize ProvOne etc.
                     conformsTo = prov_conforms_to[extension]
             return (mediatype, conformsTo)
 
-        aggregates = []  # type: List[Aggregate]
+        aggregates: List[Aggregate] = []
         for path in self.bagged_size.keys():
             temp_path = PurePosixPath(path)
             folder = temp_path.parent
             filename = temp_path.name
 
             # NOTE: Here we end up aggregating the abstract
             # data items by their sha1 hash, so that it matches
             # the entity() in the prov files.
 
             # TODO: Change to nih:sha-256; hashes
             #  https://tools.ietf.org/html/rfc6920#section-7
-            aggregate_dict = {
+            aggregate_dict: Aggregate = {
                 "uri": "urn:hash::sha1:" + filename,
                 "bundledAs": {
                     # The arcp URI is suitable ORE proxy; local to this Research Object.
                     # (as long as we don't also aggregate it by relative path!)
                     "uri": self.base_uri + path,
                     # relate it to the data/ path
-                    "folder": "/%s/" % folder,
+                    "folder": f"/{folder}/",
                     "filename": filename,
                 },
-            }  # type: Aggregate
+            }
             if path in self._file_provenance:
                 # Made by workflow run, merge captured provenance
                 bundledAs = aggregate_dict["bundledAs"]
                 if bundledAs:
                     bundledAs.update(self._file_provenance[path])
                 else:
                     aggregate_dict["bundledAs"] = cast(
@@ -561,19 +310,19 @@
                 # aggregate it.
                 continue
 
             # These are local paths like metadata/provenance - but
             # we need to relativize them for our current directory for
             # as we are saved in metadata/manifest.json
             mediatype, conformsTo = guess_mediatype(path)
-            rel_aggregates = {
+            rel_aggregates: Aggregate = {
                 "uri": str(Path(os.pardir) / path),
                 "mediatype": mediatype,
                 "conformsTo": conformsTo,
-            }  # type: Aggregate
+            }
 
             if path in self._file_provenance:
                 # Propagate file provenance (e.g. timestamp)
                 rel_aggregates.update(self._file_provenance[path])
             elif not path.startswith(SNAPSHOT):
                 # make new timestamp?
                 (
@@ -581,40 +330,39 @@
                     rel_aggregates["createdBy"],
                 ) = self._self_made()
             aggregates.append(rel_aggregates)
         aggregates.extend(self._external_aggregates)
         return aggregates
 
     def add_uri(self, uri: str, timestamp: Optional[datetime.datetime] = None) -> Aggregate:
-        """Create and store an aggreate for the given URI."""
         self.self_check()
-        aggr = {"uri": uri}  # type: Aggregate
+        aggr: Aggregate = {"uri": uri}
         aggr["createdOn"], aggr["createdBy"] = self._self_made(timestamp=timestamp)
         self._external_aggregates.append(aggr)
         return aggr
 
     def add_annotation(
         self, about: str, content: List[str], motivated_by: str = "oa:describing"
     ) -> str:
         """Cheap URI relativize for current directory and /."""
         self.self_check()
         curr = self.base_uri + METADATA + "/"
         content = [c.replace(curr, "").replace(self.base_uri, "../") for c in content]
         uri = uuid.uuid4().urn
-        ann = {
+        ann: Annotation = {
             "uri": uri,
             "about": about,
             "content": content,
             "oa:motivatedBy": {"@id": motivated_by},
-        }  # type: Annotation
+        }
         self.annotations.append(ann)
         return uri
 
     def _ro_annotations(self) -> List[Annotation]:
-        annotations = []  # type: List[Annotation]
+        annotations: List[Annotation] = []
         annotations.append(
             {
                 "uri": uuid.uuid4().urn,
                 "about": self.ro_uuid.urn,
                 "content": "/",
                 # https://www.w3.org/TR/annotation-vocab/#named-individuals
                 "oa:motivatedBy": {"@id": "oa:describing"},
@@ -660,74 +408,26 @@
             }
         )
         # Add user-added annotations at end
         annotations.extend(self.annotations)
         return annotations
 
     def _authored_by(self) -> Optional[AuthoredBy]:
-        authored_by = {}  # type: AuthoredBy
+        authored_by: AuthoredBy = {}
         if self.orcid:
             authored_by["orcid"] = self.orcid
         if self.full_name:
             authored_by["name"] = self.full_name
             if not self.orcid:
                 authored_by["uri"] = USER_UUID
 
         if authored_by:
             return authored_by
         return None
 
-    def _write_ro_manifest(self) -> None:
-        # Does not have to be this order, but it's nice to be consistent
-        filename = "manifest.json"
-        createdOn, createdBy = self._self_made()
-        manifest = OrderedDict(
-            {
-                "@context": [
-                    {"@base": f"{self.base_uri}{posix_path(METADATA)}/"},
-                    "https://w3id.org/bundle/context",
-                ],
-                "id": "/",
-                "conformsTo": CWLPROV_VERSION,
-                "manifest": filename,
-                "createdOn": createdOn,
-                "createdBy": createdBy,
-                "authoredBy": self._authored_by(),
-                "aggregates": self._ro_aggregates(),
-                "annotations": self._ro_annotations(),
-            }
-        )
-
-        json_manifest = json_dumps(manifest, indent=4, ensure_ascii=False)
-        rel_path = str(PurePosixPath(METADATA) / filename)
-        json_manifest += "\n"
-        with self.write_bag_file(rel_path) as manifest_file:
-            manifest_file.write(json_manifest)
-
-    def _write_bag_info(self) -> None:
-        with self.write_bag_file("bag-info.txt") as info_file:
-            info_file.write("Bag-Software-Agent: %s\n" % self.cwltool_version)
-            # FIXME: require sha-512 of payload to comply with profile?
-            # FIXME: Update profile
-            info_file.write("BagIt-Profile-Identifier: https://w3id.org/ro/bagit/profile\n")
-            info_file.write("Bagging-Date: %s\n" % datetime.date.today().isoformat())
-            info_file.write("External-Description: Research Object of CWL workflow run\n")
-            if self.full_name:
-                info_file.write("Contact-Name: %s\n" % self.full_name)
-
-            # NOTE: We can't use the urn:uuid:{UUID} of the workflow run (a prov:Activity)
-            # as identifier for the RO/bagit (a prov:Entity). However the arcp base URI is good.
-            info_file.write("External-Identifier: %s\n" % self.base_uri)
-
-            # Calculate size of data/ (assuming no external fetch.txt files)
-            total_size = sum(self.bagged_size.values())
-            num_files = len(self.bagged_size)
-            info_file.write("Payload-Oxum: %d.%d\n" % (total_size, num_files))
-        _logger.debug("[provenance] Generated bagit metadata: %s", self.folder)
-
     def generate_snapshot(self, prov_dep: CWLObjectType) -> None:
         """Copy all of the CWL files to the snapshot/ directory."""
         self.self_check()
         for key, value in prov_dep.items():
             if key == "location" and cast(str, value).split("/")[-1]:
                 location = cast(str, value)
                 filename = location.split("/")[-1]
@@ -752,23 +452,14 @@
             elif key in ("secondaryFiles", "listing"):
                 for files in cast(MutableSequence[CWLObjectType], value):
                     if isinstance(files, MutableMapping):
                         self.generate_snapshot(files)
             else:
                 pass
 
-    def packed_workflow(self, packed: str) -> None:
-        """Pack CWL description to generate re-runnable CWL object in RO."""
-        self.self_check()
-        rel_path = str(PurePosixPath(WORKFLOW) / "packed.cwl")
-        # Write as binary
-        with self.write_bag_file(rel_path, encoding=None) as write_pack:
-            write_pack.write(packed)
-        _logger.debug("[provenance] Added packed workflow: %s", rel_path)
-
     def has_data_file(self, sha1hash: str) -> bool:
         """Confirm the presence of the given file in the RO."""
         folder = os.path.join(self.folder, DATA, sha1hash[0:2])
         hash_path = os.path.join(folder, sha1hash)
         return os.path.isfile(hash_path)
 
     def add_data_file(
@@ -824,15 +515,15 @@
             {"uri": self.engine_uuid, "name": self.cwltool_version},
         )
 
     def add_to_manifest(self, rel_path: str, checksums: Dict[str, str]) -> None:
         """Add files to the research object manifest."""
         self.self_check()
         if PurePosixPath(rel_path).is_absolute():
-            raise ValueError("rel_path must be relative: %s" % rel_path)
+            raise ValueError(f"rel_path must be relative: {rel_path}")
 
         if os.path.commonprefix(["data/", rel_path]) == "data/":
             # payload file, go to manifest
             manifest = "manifest"
             self.has_manifest = True
         else:
             # metadata file, go to tag manifest
@@ -847,15 +538,15 @@
             with open(manifestpath, "a", encoding=ENCODING, newline="\n") as checksum_file:
                 line = f"{hash_value}  {rel_path}\n"
                 _logger.debug("[provenance] Added to %s: %s", manifestpath, line)
                 checksum_file.write(line)
 
     def _add_to_bagit(self, rel_path: str, **checksums: str) -> None:
         if PurePosixPath(rel_path).is_absolute():
-            raise ValueError("rel_path must be relative: %s" % rel_path)
+            raise ValueError(f"rel_path must be relative: {rel_path}")
         lpath = os.path.join(self.folder, local_path(rel_path))
         if not os.path.exists(lpath):
             raise OSError(f"File {rel_path} does not exist within RO: {lpath}")
 
         if rel_path in self.bagged_size:
             # Already added, assume checksum OK
             return
@@ -866,65 +557,31 @@
             checksums = dict(checksums)
             with open(lpath, "rb") as file_path:
                 # FIXME: Need sha-256 / sha-512 as well for Research Object BagIt profile?
                 checksums[SHA1] = checksum_copy(file_path, hasher=hashlib.sha1)
 
         self.add_to_manifest(rel_path, checksums)
 
-    def create_job(self, builder_job: CWLObjectType, is_output: bool = False) -> CWLObjectType:
-        # TODO customise the file
-        """Generate the new job object with RO specific relative paths."""
-        copied = copy.deepcopy(builder_job)
-        relativised_input_objecttemp = {}  # type: CWLObjectType
-        self._relativise_files(copied)
-
-        def jdefault(o: Any) -> Dict[Any, Any]:
-            return dict(o)
-
-        if is_output:
-            rel_path = PurePosixPath(WORKFLOW) / "primary-output.json"
-        else:
-            rel_path = PurePosixPath(WORKFLOW) / "primary-job.json"
-        j = json_dumps(copied, indent=4, ensure_ascii=False, default=jdefault)
-        with self.write_bag_file(str(rel_path)) as file_path:
-            file_path.write(j + "\n")
-        _logger.debug("[provenance] Generated customised job file: %s", rel_path)
-        # Generate dictionary with keys as workflow level input IDs and values
-        # as
-        # 1) for files the relativised location containing hash
-        # 2) for other attributes, the actual value.
-        for key, value in copied.items():
-            if isinstance(value, MutableMapping):
-                if value.get("class") in ("File", "Directory"):
-                    relativised_input_objecttemp[key] = value
-            else:
-                relativised_input_objecttemp[key] = value
-        self.relativised_input_object.update(
-            {k: v for k, v in relativised_input_objecttemp.items() if v}
-        )
-        return self.relativised_input_object
-
     def _relativise_files(
         self,
         structure: Union[CWLObjectType, CWLOutputType, MutableSequence[CWLObjectType]],
     ) -> None:
         """Save any file objects into the RO and update the local paths."""
         # Base case - we found a File we need to update
         _logger.debug("[provenance] Relativising: %s", structure)
 
         if isinstance(structure, MutableMapping):
             if structure.get("class") == "File":
-                relative_path = None  # type: Optional[Union[str, PurePosixPath]]
+                relative_path: Optional[Union[str, PurePosixPath]] = None
                 if "checksum" in structure:
                     raw_checksum = cast(str, structure["checksum"])
                     alg, checksum = raw_checksum.split("$")
                     if alg != SHA1:
                         raise TypeError(
-                            "Only SHA1 CWL checksums are currently supported: "
-                            "{}".format(structure)
+                            f"Only SHA1 CWL checksums are currently supported: {structure}"
                         )
                     if self.has_data_file(checksum):
                         prefix = checksum[0:2]
                         relative_path = PurePosixPath("data") / prefix / checksum
 
                 if not (relative_path is not None and "location" in structure):
                     # Register in RO; but why was this not picked
@@ -951,69 +608,7 @@
                     pass
             return
 
         if isinstance(structure, MutableSequence):
             for obj in structure:
                 # Recurse and rewrite any nested File objects
                 self._relativise_files(cast(CWLOutputType, obj))
-
-    def close(self, save_to: Optional[str] = None) -> None:
-        """Close the Research Object, optionally saving to specified folder.
-
-        Closing will remove any temporary files used by this research object.
-        After calling this method, this ResearchObject instance can no longer
-        be used, except for no-op calls to .close().
-
-        The 'saveTo' folder should not exist - if it does, it will be deleted.
-
-        It is safe to call this function multiple times without the
-        'saveTo' argument, e.g. within a try..finally block to
-        ensure the temporary files of this Research Object are removed.
-        """
-        if save_to is None:
-            if not self.closed:
-                _logger.debug("[provenance] Deleting temporary %s", self.folder)
-                shutil.rmtree(self.folder, ignore_errors=True)
-        else:
-            save_to = os.path.abspath(save_to)
-            _logger.info("[provenance] Finalizing Research Object")
-            self._finalize()  # write manifest etc.
-            # TODO: Write as archive (.zip or .tar) based on extension?
-
-            if os.path.isdir(save_to):
-                _logger.info("[provenance] Deleting existing %s", save_to)
-                shutil.rmtree(save_to)
-            shutil.move(self.folder, save_to)
-            _logger.info("[provenance] Research Object saved to %s", save_to)
-            self.folder = save_to
-        self.closed = True
-
-
-def checksum_copy(
-    src_file: IO[Any],
-    dst_file: Optional[IO[Any]] = None,
-    hasher: Callable[[], "hashlib._Hash"] = Hasher,
-    buffersize: int = 1024 * 1024,
-) -> str:
-    """Compute checksums while copying a file."""
-    # TODO: Use hashlib.new(Hasher_str) instead?
-    checksum = hasher()
-    contents = src_file.read(buffersize)
-    if dst_file and hasattr(dst_file, "name") and hasattr(src_file, "name"):
-        temp_location = os.path.join(os.path.dirname(dst_file.name), str(uuid.uuid4()))
-        try:
-            os.rename(dst_file.name, temp_location)
-            os.link(src_file.name, dst_file.name)
-            dst_file = None
-            os.unlink(temp_location)
-        except OSError:
-            pass
-        if os.path.exists(temp_location):
-            os.rename(temp_location, dst_file.name)  # type: ignore
-    while contents != b"":
-        if dst_file is not None:
-            dst_file.write(contents)
-        checksum.update(contents)
-        contents = src_file.read(buffersize)
-    if dst_file is not None:
-        dst_file.flush()
-    return checksum.hexdigest().lower()
```

### Comparing `cwltool-3.1.20230513155734/cwltool/provenance_constants.py` & `cwltool-3.1.20230526180938/cwltool/cwlprov/provenance_constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 SCHEMA = Namespace("schema", "http://schema.org/")
 CWLPROV = Namespace("cwlprov", "https://w3id.org/cwl/prov#")
 ORCID = Namespace("orcid", "https://orcid.org/")
 UUID = Namespace("id", "urn:uuid:")
 
 # BagIt and YAML always use UTF-8
 ENCODING = "UTF-8"
-TEXT_PLAIN = 'text/plain; charset="%s"' % ENCODING
+TEXT_PLAIN = f"text/plain; charset={ENCODING!r}"
 
 # sha1, compatible with the File type's "checksum" field
 # e.g. "checksum" = "sha1$47a013e660d408619d894b20806b1d5086aab03b"
 # See ./cwltool/schemas/v1.0/Process.yml
 Hasher = hashlib.sha1
 SHA1 = "sha1"
 SHA256 = "sha256"
```

### Comparing `cwltool-3.1.20230513155734/cwltool/provenance_profile.py` & `cwltool-3.1.20230526180938/cwltool/cwlprov/provenance_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,21 @@
     cast,
 )
 
 from prov.identifier import Identifier, QualifiedName
 from prov.model import PROV, PROV_LABEL, PROV_TYPE, PROV_VALUE, ProvDocument, ProvEntity
 from schema_salad.sourceline import SourceLine
 
-from .errors import WorkflowException
-from .job import CommandLineJob, JobBase
-from .loghandler import _logger
-from .process import Process, shortname
+from ..errors import WorkflowException
+from ..job import CommandLineJob, JobBase
+from ..loghandler import _logger
+from ..process import Process, shortname
+from ..stdfsaccess import StdFsAccess
+from ..utils import CWLObjectType, JobsType, get_listing, posix_path, versionstring
+from ..workflow_job import WorkflowJob
 from .provenance_constants import (
     ACCOUNT_UUID,
     CWLPROV,
     ENCODING,
     FOAF,
     METADATA,
     ORE,
@@ -42,20 +45,18 @@
     SHA256,
     TEXT_PLAIN,
     UUID,
     WF4EVER,
     WFDESC,
     WFPROV,
 )
-from .stdfsaccess import StdFsAccess
-from .utils import CWLObjectType, JobsType, get_listing, posix_path, versionstring
-from .workflow_job import WorkflowJob
+from .writablebagfile import create_job, write_bag_file  # change this later
 
 if TYPE_CHECKING:
-    from .provenance import ResearchObject
+    from .ro import ResearchObject
 
 
 def copy_job_order(job: Union[Process, JobsType], job_order_object: CWLObjectType) -> CWLObjectType:
     """Create copy of job object for provenance."""
     if not isinstance(job, WorkflowJob):
         # direct command line tool execution
         return job_order_object
@@ -110,18 +111,15 @@
             _logger.debug("[provenance] Creator Full name: %s", self.full_name)
         self.workflow_run_uuid = run_uuid or uuid.uuid4()
         self.workflow_run_uri = self.workflow_run_uuid.urn
         self.generate_prov_doc()
 
     def __str__(self) -> str:
         """Represent this Provenvance profile as a string."""
-        return "ProvenanceProfile <{}> in <{}>".format(
-            self.workflow_run_uri,
-            self.research_object,
-        )
+        return f"ProvenanceProfile <{self.workflow_run_uri}> in <{self.research_object}>"
 
     def generate_prov_doc(self) -> Tuple[str, ProvDocument]:
         """Add basic namespaces."""
 
         def host_provenance(document: ProvDocument) -> None:
             """Record host provenance."""
             document.add_namespace(CWLPROV)
@@ -136,15 +134,15 @@
                 {
                     PROV_TYPE: FOAF["OnlineAccount"],
                     "prov:location": hostname,
                     CWLPROV["hostname"]: hostname,
                 },
             )
 
-        self.cwltool_version = "cwltool %s" % versionstring().split()[-1]
+        self.cwltool_version = f"cwltool {versionstring().split()[-1]}"
         self.document.add_namespace("wfprov", "http://purl.org/wf4ever/wfprov#")
         # document.add_namespace('prov', 'http://www.w3.org/ns/prov#')
         self.document.add_namespace("wfdesc", "http://purl.org/wf4ever/wfdesc#")
         # TODO: Make this ontology. For now only has cwlprov:image
         self.document.add_namespace("cwlprov", "https://w3id.org/cwl/prov#")
         self.document.add_namespace("foaf", "http://xmlns.com/foaf/0.1/")
         self.document.add_namespace("schema", "http://schema.org/")
@@ -236,15 +234,15 @@
     ) -> None:
         """Evaluate the nature of job."""
         if not hasattr(process, "steps"):
             # record provenance of independent commandline tool executions
             self.prospective_prov(job)
             customised_job = copy_job_order(job, job_order_object)
             self.used_artefacts(customised_job, self.workflow_run_uri)
-            research_obj.create_job(customised_job)
+            create_job(research_obj, customised_job)
         elif hasattr(job, "workflow"):
             # record provenance of workflow executions
             self.prospective_prov(job)
             customised_job = copy_job_order(job, job_order_object)
             self.used_artefacts(customised_job, self.workflow_run_uri)
 
     def record_process_start(
@@ -456,15 +454,15 @@
         ore_doc = ProvDocument()
         ore_doc.add_namespace(ORE)
         ore_doc.add_namespace(RO)
         ore_doc.add_namespace(UUID)
         ore_doc.add_bundle(dir_bundle)
         ore_doc = ore_doc.flattened()
         ore_doc_path = str(PurePosixPath(METADATA, ore_doc_fn))
-        with self.research_object.write_bag_file(ore_doc_path) as provenance_file:
+        with write_bag_file(self.research_object, ore_doc_path) as provenance_file:
             ore_doc.serialize(provenance_file, format="rdf", rdf_format="turtle")
         self.research_object.add_annotation(dir_id, [ore_doc_fn], ORE["isDescribedBy"].uri)
 
         if is_empty:
             # Empty directory
             coll.add_asserted_type(PROV["EmptyCollection"])
             coll.add_asserted_type(PROV["EmptyDictionary"])
@@ -473,15 +471,15 @@
 
     def declare_string(self, value: str) -> Tuple[ProvEntity, str]:
         """Save as string in UTF-8."""
         byte_s = BytesIO(str(value).encode(ENCODING))
         data_file = self.research_object.add_data_file(byte_s, content_type=TEXT_PLAIN)
         checksum = PurePosixPath(data_file).name
         # FIXME: Don't naively assume add_data_file uses hash in filename!
-        data_id = "data:%s" % PurePosixPath(data_file).stem
+        data_id = f"data:{PurePosixPath(data_file).stem}"
         entity = self.document.entity(
             data_id, {PROV_TYPE: WFPROV["Artifact"], PROV_VALUE: str(value)}
         )
         return entity, checksum
 
     def declare_artefact(self, value: Any) -> ProvEntity:
         """Create data artefact entities for all file objects."""
@@ -505,15 +503,15 @@
             return entity
 
         if isinstance(value, bytes):
             # If we got here then we must be in Python 3
             byte_s = BytesIO(value)
             data_file = self.research_object.add_data_file(byte_s)
             # FIXME: Don't naively assume add_data_file uses hash in filename!
-            data_id = "data:%s" % PurePosixPath(data_file).stem
+            data_id = f"data:{PurePosixPath(data_file).stem}"
             return self.document.entity(
                 data_id,
                 {PROV_TYPE: WFPROV["Artifact"], PROV_VALUE: str(value)},
             )
 
         if isinstance(value, MutableMapping):
             if "@id" in value:
@@ -650,15 +648,15 @@
             for output, value in final_output.items():
                 entity = self.declare_artefact(value)
                 if name is not None:
                     name = urllib.parse.quote(str(name), safe=":/,#")
                     # FIXME: Probably not "main" in nested workflows
                     role = self.wf_ns[f"main/{name}/{output}"]
                 else:
-                    role = self.wf_ns["main/%s" % output]
+                    role = self.wf_ns[f"main/{output}"]
 
                 if not process_run_id:
                     process_run_id = self.workflow_run_uri
 
                 self.document.wasGeneratedBy(
                     entity, process_run_id, timestamp, None, {"prov:role": role}
                 )
@@ -734,44 +732,44 @@
 
         # TODO: Also support other profiles than CWLProv, e.g. ProvOne
 
         # list of prov identifiers of provenance files
         prov_ids = []
 
         # https://www.w3.org/TR/prov-xml/
-        with self.research_object.write_bag_file(basename + ".xml") as provenance_file:
+        with write_bag_file(self.research_object, basename + ".xml") as provenance_file:
             self.document.serialize(provenance_file, format="xml", indent=4)
             prov_ids.append(self.provenance_ns[filename + ".xml"])
 
         # https://www.w3.org/TR/prov-n/
-        with self.research_object.write_bag_file(basename + ".provn") as provenance_file:
+        with write_bag_file(self.research_object, basename + ".provn") as provenance_file:
             self.document.serialize(provenance_file, format="provn", indent=2)
             prov_ids.append(self.provenance_ns[filename + ".provn"])
 
         # https://www.w3.org/Submission/prov-json/
-        with self.research_object.write_bag_file(basename + ".json") as provenance_file:
+        with write_bag_file(self.research_object, basename + ".json") as provenance_file:
             self.document.serialize(provenance_file, format="json", indent=2)
             prov_ids.append(self.provenance_ns[filename + ".json"])
 
         # "rdf" aka https://www.w3.org/TR/prov-o/
         # which can be serialized to ttl/nt/jsonld (and more!)
 
         # https://www.w3.org/TR/turtle/
-        with self.research_object.write_bag_file(basename + ".ttl") as provenance_file:
+        with write_bag_file(self.research_object, basename + ".ttl") as provenance_file:
             self.document.serialize(provenance_file, format="rdf", rdf_format="turtle")
             prov_ids.append(self.provenance_ns[filename + ".ttl"])
 
         # https://www.w3.org/TR/n-triples/
-        with self.research_object.write_bag_file(basename + ".nt") as provenance_file:
+        with write_bag_file(self.research_object, basename + ".nt") as provenance_file:
             self.document.serialize(provenance_file, format="rdf", rdf_format="ntriples")
             prov_ids.append(self.provenance_ns[filename + ".nt"])
 
         # https://www.w3.org/TR/json-ld/
         # TODO: Use a nice JSON-LD context
         # see also https://eprints.soton.ac.uk/395985/
         # 404 Not Found on https://provenance.ecs.soton.ac.uk/prov.jsonld :(
-        with self.research_object.write_bag_file(basename + ".jsonld") as provenance_file:
+        with write_bag_file(self.research_object, basename + ".jsonld") as provenance_file:
             self.document.serialize(provenance_file, format="rdf", rdf_format="json-ld")
             prov_ids.append(self.provenance_ns[filename + ".jsonld"])
 
         _logger.debug("[provenance] added provenance: %s", prov_ids)
         return prov_ids
```

### Comparing `cwltool-3.1.20230513155734/cwltool/rdfqueries/get_inner_edges.sparql` & `cwltool-3.1.20230526180938/cwltool/rdfqueries/get_inner_edges.sparql`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/rdfqueries/get_input_edges.sparql` & `cwltool-3.1.20230526180938/cwltool/rdfqueries/get_input_edges.sparql`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/rdfqueries/get_output_edges.sparql` & `cwltool-3.1.20230526180938/cwltool/rdfqueries/get_output_edges.sparql`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/rdfqueries/get_root.sparql` & `cwltool-3.1.20230526180938/cwltool/rdfqueries/get_root.sparql`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/resolver.py` & `cwltool-3.1.20230526180938/cwltool/resolver.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/run_job.py` & `cwltool-3.1.20230526180938/cwltool/run_job.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/CommandLineTool.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/Process.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/README.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/README.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/Workflow.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/concepts.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/contrib.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/intro.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/invocation.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/CODE_OF_CONDUCT.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/CONFORMANCE_TESTS.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/CONFORMANCE_TESTS.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/CommandLineTool.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/Process.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/Workflow.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/concepts.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/contrib.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/index.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/intro.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/invocation.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/CommandLineTool.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/Process.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/Workflow.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/concepts.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/contrib.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/intro.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/invocation.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/CODE_OF_CONDUCT.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/CONFORMANCE_TESTS.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/CONFORMANCE_TESTS.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/CommandLineTool.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/Operation.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/Process.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/Workflow.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/concepts.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/contrib.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/index.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/intro.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/invocation.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/CommandLineTool.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/Operation.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/Process.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/Workflow.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/concepts.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/contrib.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/intro.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/invocation.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/CommandLineTool.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/Operation.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/Process.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/Workflow.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/concepts.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/contrib.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/index.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/intro.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/invocation.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/CODE_OF_CONDUCT.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/CONFORMANCE_TESTS.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/CONFORMANCE_TESTS.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/CommandLineTool.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/Operation.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/Process.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/Workflow.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/concepts.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/contrib.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/index.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/intro.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/invocation.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/CODE_OF_CONDUCT.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/CONFORMANCE_TESTS.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/CONFORMANCE_TESTS.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/CommandLineTool.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/Operation.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/Process.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/Workflow.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/concepts.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/contrib.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/index.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/intro.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/invocation.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20230526180938/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/secrets.py` & `cwltool-3.1.20230526180938/cwltool/secrets.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/singularity.py` & `cwltool-3.1.20230526180938/cwltool/singularity.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/singularity_utils.py` & `cwltool-3.1.20230526180938/cwltool/singularity_utils.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/software_requirements.py` & `cwltool-3.1.20230526180938/cwltool/software_requirements.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/stdfsaccess.py` & `cwltool-3.1.20230526180938/cwltool/stdfsaccess.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/subgraph.py` & `cwltool-3.1.20230526180938/cwltool/subgraph.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/task_queue.py` & `cwltool-3.1.20230526180938/cwltool/task_queue.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/udocker.py` & `cwltool-3.1.20230526180938/cwltool/udocker.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/cwltool/update.py` & `cwltool-3.1.20230526180938/cwltool/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,19 @@
     MutableSequence,
     Optional,
     Tuple,
     Union,
     cast,
 )
 
+from ruamel.yaml.comments import CommentedMap, CommentedSeq
 from schema_salad.exceptions import ValidationException
 from schema_salad.ref_resolver import Loader
 from schema_salad.sourceline import SourceLine
 
-from ruamel.yaml.comments import CommentedMap, CommentedSeq
-
 from .loghandler import _logger
 from .utils import CWLObjectType, CWLOutputType, aslist, visit_class, visit_field
 
 
 def v1_1to1_2(
     doc: CommentedMap, loader: Loader, baseuri: str
 ) -> Tuple[CommentedMap, str]:  # pylint: disable=unused-argument
```

### Comparing `cwltool-3.1.20230513155734/cwltool/utils.py` & `cwltool-3.1.20230526180938/cwltool/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,23 +32,27 @@
     Optional,
     Set,
     Tuple,
     Union,
     cast,
 )
 
-import pkg_resources
 import requests
 from cachecontrol import CacheControl
 from cachecontrol.caches import FileCache
 from mypy_extensions import TypedDict, mypyc_attr
 from schema_salad.exceptions import ValidationException
 from schema_salad.ref_resolver import Loader
 from typing_extensions import Deque, Literal
 
+if sys.version_info >= (3, 8):
+    import importlib.metadata as importlib_metadata
+else:
+    import importlib_metadata
+
 if TYPE_CHECKING:
     from .command_line_tool import CallbackJob, ExpressionJob
     from .job import CommandLineJob, JobBase
     from .stdfsaccess import StdFsAccess
     from .workflow_job import WorkflowJob
 
 __random_outdir: Optional[str] = None
@@ -110,17 +114,17 @@
 StepType = CWLObjectType  # WorkflowStep
 
 LoadListingType = Union[Literal["no_listing"], Literal["shallow_listing"], Literal["deep_listing"]]
 
 
 def versionstring() -> str:
     """Version of CWLtool used to execute the workflow."""
-    pkg = pkg_resources.require("cwltool")
+    pkg = importlib_metadata.version("cwltool")
     if pkg:
-        return f"{sys.argv[0]} {pkg[0].version}"
+        return f"{sys.argv[0]} {pkg}"
     return "{} {}".format(sys.argv[0], "unknown version")
 
 
 def aslist(thing: Any) -> MutableSequence[Any]:
     """Wrap any non-MutableSequence/list in a list."""
     if isinstance(thing, MutableSequence):
         return thing
```

### Comparing `cwltool-3.1.20230513155734/cwltool/validate_js.py` & `cwltool-3.1.20230526180938/cwltool/validate_js.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,28 +14,27 @@
     Union,
     cast,
 )
 
 from cwl_utils.errors import SubstitutionError
 from cwl_utils.expression import scanner as scan_expression
 from cwl_utils.sandboxjs import code_fragment_to_js, exec_js_process
-from pkg_resources import resource_stream
+from importlib_resources import files
+from ruamel.yaml.comments import CommentedMap, CommentedSeq
 from schema_salad.avro.schema import (
     ArraySchema,
     EnumSchema,
     RecordSchema,
     Schema,
     UnionSchema,
 )
 from schema_salad.sourceline import SourceLine
 from schema_salad.utils import json_dumps
 from schema_salad.validate import validate_ex
 
-from ruamel.yaml.comments import CommentedMap, CommentedSeq
-
 from .errors import WorkflowException
 from .loghandler import _logger
 
 
 def is_expression(tool: Any, schema: Optional[Schema]) -> bool:
     """Test a field/schema combo to see if it is a CWL Expression."""
     return (
@@ -147,23 +146,23 @@
                 "W104",
                 "W119",  # using ES6 features
             ],
             "strict": "implied",
             "esversion": 5,
         }
 
-    with resource_stream(__name__, "jshint/jshint.js") as res:
+    with files("cwltool").joinpath("jshint/jshint.js") as res:
         # NOTE: we need a global variable for lodash (which jshint depends on)
-        jshint_functions_text = "var global = this;" + res.read().decode("utf-8")
+        jshint_functions_text = "var global = this;" + res.read_text("utf-8")
 
-    with resource_stream(__name__, "jshint/jshint_wrapper.js") as res2:
+    with files("cwltool").joinpath("jshint/jshint_wrapper.js") as res2:
         # NOTE: we need to assign to ob, as the expression {validateJS: validateJS} as an expression
         # is interpreted as a block with a label `validateJS`
         jshint_functions_text += (
-            "\n" + res2.read().decode("utf-8") + "\nvar ob = {validateJS: validateJS}; ob"
+            "\n" + res2.read_text("utf-8") + "\nvar ob = {validateJS: validateJS}; ob"
         )
 
     returncode, stdout, stderr = exec_js_process(
         "validateJS(%s)" % json_dumps({"code": js_text, "options": options, "globals": globals}),
         timeout=eval_timeout,
         context=jshint_functions_text,
         container_engine=container_engine,
```

### Comparing `cwltool-3.1.20230513155734/cwltool/workflow.py` & `cwltool-3.1.20230526180938/cwltool/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,27 @@
     MutableSequence,
     Optional,
     Union,
     cast,
 )
 from uuid import UUID
 
+from ruamel.yaml.comments import CommentedMap
 from schema_salad.exceptions import ValidationException
 from schema_salad.sourceline import SourceLine, indent
 
-from ruamel.yaml.comments import CommentedMap
-
 from . import command_line_tool, context, procgenerator
 from .checker import circular_dependency_checker, loop_checker, static_checker
 from .context import LoadingContext, RuntimeContext, getdefault
+from .cwlprov.provenance_profile import ProvenanceProfile
+from .cwlprov.writablebagfile import create_job
 from .errors import WorkflowException
 from .load_tool import load_tool
 from .loghandler import _logger
 from .process import Process, get_overrides, shortname
-from .provenance_profile import ProvenanceProfile
 from .utils import (
     CWLObjectType,
     CWLOutputType,
     JobsGeneratorType,
     OutputCallbackType,
     StepType,
     aslist,
@@ -159,15 +159,15 @@
     ) -> JobsGeneratorType:
         builder = self._init_job(job_order, runtimeContext)
 
         if runtimeContext.research_obj is not None:
             if runtimeContext.toplevel:
                 # Record primary-job.json
                 runtimeContext.research_obj.fsaccess = runtimeContext.make_fs_access("")
-                runtimeContext.research_obj.create_job(builder.job)
+                create_job(runtimeContext.research_obj, builder.job)
 
         job = WorkflowJob(self, runtimeContext)
         yield job
 
         runtimeContext = runtimeContext.copy()
         runtimeContext.part_of = "workflow %s" % job.name
         runtimeContext.toplevel = False
```

### Comparing `cwltool-3.1.20230513155734/cwltool/workflow_job.py` & `cwltool-3.1.20230526180938/cwltool/workflow_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     WorkflowStateItem,
     adjustDirObjs,
     aslist,
     get_listing,
 )
 
 if TYPE_CHECKING:
-    from .provenance_profile import ProvenanceProfile
+    from .cwlprov.provenance_profile import ProvenanceProfile
     from .workflow import Workflow, WorkflowStep
 
 
 class WorkflowJobStep:
     """Generated for each step in Workflow.steps()."""
 
     def __init__(self, step: "WorkflowStep") -> None:
```

### Comparing `cwltool-3.1.20230513155734/cwltool.egg-info/PKG-INFO` & `cwltool-3.1.20230526180938/cwltool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwltool
-Version: 3.1.20230513155734
+Version: 3.1.20230526180938
 Summary: Common workflow language reference implementation
 Home-page: https://github.com/common-workflow-language/cwltool
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 License: UNKNOWN
 Download-URL: https://github.com/common-workflow-language/cwltool
 Description: #############################################################################################
```

### Comparing `cwltool-3.1.20230513155734/cwltool.egg-info/SOURCES.txt` & `cwltool-3.1.20230526180938/cwltool.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,14 @@
 cwltool/main.py
 cwltool/mpi.py
 cwltool/mutation.py
 cwltool/pack.py
 cwltool/pathmapper.py
 cwltool/process.py
 cwltool/procgenerator.py
-cwltool/provenance.py
-cwltool/provenance_constants.py
-cwltool/provenance_profile.py
 cwltool/py.typed
 cwltool/resolver.py
 cwltool/run_job.py
 cwltool/secrets.py
 cwltool/singularity.py
 cwltool/singularity_utils.py
 cwltool/software_requirements.py
@@ -68,14 +65,19 @@
 cwltool.egg-info/PKG-INFO
 cwltool.egg-info/SOURCES.txt
 cwltool.egg-info/dependency_links.txt
 cwltool.egg-info/entry_points.txt
 cwltool.egg-info/requires.txt
 cwltool.egg-info/top_level.txt
 cwltool.egg-info/zip-safe
+cwltool/cwlprov/__init__.py
+cwltool/cwlprov/provenance_constants.py
+cwltool/cwlprov/provenance_profile.py
+cwltool/cwlprov/ro.py
+cwltool/cwlprov/writablebagfile.py
 cwltool/jshint/jshint.js
 cwltool/jshint/jshint_wrapper.js
 cwltool/rdfqueries/get_inner_edges.sparql
 cwltool/rdfqueries/get_input_edges.sparql
 cwltool/rdfqueries/get_output_edges.sparql
 cwltool/rdfqueries/get_root.sparql
 cwltool/schemas/v1.0/CommandLineTool-standalone.yml
@@ -441,14 +443,16 @@
 mypy-stubs/graphviz/__init__.pyi
 mypy-stubs/graphviz/_compat.pyi
 mypy-stubs/graphviz/backend.pyi
 mypy-stubs/graphviz/dot.pyi
 mypy-stubs/graphviz/files.pyi
 mypy-stubs/graphviz/lang.pyi
 mypy-stubs/graphviz/tools.pyi
+mypy-stubs/importlib_metadata/__init__.pyi
+mypy-stubs/importlib_metadata/_meta.pyi
 mypy-stubs/prov/__init__.pyi
 mypy-stubs/prov/constants.py
 mypy-stubs/prov/dot.pyi
 mypy-stubs/prov/graph.pyi
 mypy-stubs/prov/identifier.pyi
 mypy-stubs/prov/model.pyi
 mypy-stubs/prov/serializers/provjson.pyi
@@ -800,14 +804,15 @@
 tests/wf/packed_no_main.cwl
 tests/wf/paramref_arguments_roundtrip.cwl
 tests/wf/paramref_arguments_self.cwl
 tests/wf/parseInt-tool.cwl
 tests/wf/record_outputeval.cwl
 tests/wf/resreq_expr_float_v1_0.cwl
 tests/wf/resreq_expr_float_v1_2.cwl
+tests/wf/revsort-job-shortcut.json
 tests/wf/revsort-job.json
 tests/wf/revsort.cwl
 tests/wf/revsort_datetime.cwl
 tests/wf/revsort_step_bad_schema.cwl
 tests/wf/revtool.cwl
 tests/wf/revtool_bad_schema.cwl
 tests/wf/scatter-job2.json
```

### Comparing `cwltool-3.1.20230513155734/gittaggers.py` & `cwltool-3.1.20230526180938/gittaggers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 import subprocess
+import sys
 import time
-import pkg_resources
+
+if sys.version_info >= (3, 8):
+    import importlib.metadata as importlib_metadata
+else:
+    import importlib_metadata
+
+from typing import Any
+
 from setuptools.command.egg_info import egg_info
 
-SETUPTOOLS_VER = pkg_resources.get_distribution(
-    "setuptools").version.split('.')
+SETUPTOOLS_VER = importlib_metadata.version("setuptools").split(".")
+
+RECENT_SETUPTOOLS = (
+    int(SETUPTOOLS_VER[0]) > 40
+    or (int(SETUPTOOLS_VER[0]) == 40 and int(SETUPTOOLS_VER[1]) > 0)
+    or (int(SETUPTOOLS_VER[0]) == 40 and int(SETUPTOOLS_VER[1]) == 0 and int(SETUPTOOLS_VER[2]) > 0)
+)
 
-RECENT_SETUPTOOLS = int(SETUPTOOLS_VER[0]) > 40 or (
-    int(SETUPTOOLS_VER[0]) == 40 and int(SETUPTOOLS_VER[1]) > 0) or (
-        int(SETUPTOOLS_VER[0]) == 40 and int(SETUPTOOLS_VER[1]) == 0 and
-        int(SETUPTOOLS_VER[2]) > 0)
 
 class EggInfoFromGit(egg_info):
     """Tag the build with git commit timestamp.
 
     If a build tag has already been set (e.g., "egg_info -b", building
     from source package), leave it alone.
     """
 
-    def git_timestamp_tag(self):
+    def git_timestamp_tag(self) -> str:
         gitinfo = subprocess.check_output(
-            ['git', 'log', '--first-parent', '--max-count=1',
-             '--format=format:%ct', '.']).strip()
-        return time.strftime('.%Y%m%d%H%M%S', time.gmtime(int(gitinfo)))
+            ["git", "log", "--first-parent", "--max-count=1", "--format=format:%ct", "."]
+        ).strip()
+        return time.strftime(".%Y%m%d%H%M%S", time.gmtime(int(gitinfo)))
 
-    def tags(self):
+    def tags(self) -> Any:
         if self.tag_build is None:
             try:
                 self.tag_build = self.git_timestamp_tag()
             except subprocess.CalledProcessError:
                 pass
-        return egg_info.tags(self)
+        return egg_info.tags(self)  # type: ignore[no-untyped-call]
 
     if RECENT_SETUPTOOLS:
         vtags = property(tags)
```

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/arcp/parse.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/arcp/parse.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/argcomplete/__init__.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/argcomplete/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/bagit.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/bagit.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/cachecontrol/caches/file_cache.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/cachecontrol/caches/file_cache.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/graphviz/dot.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/graphviz/dot.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/graphviz/files.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/graphviz/files.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/graphviz/lang.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/graphviz/lang.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/mistune.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/mistune.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/prov/constants.py` & `cwltool-3.1.20230526180938/mypy-stubs/prov/constants.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/prov/dot.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/prov/dot.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/prov/graph.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/prov/graph.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/prov/identifier.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/prov/identifier.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/prov/model.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/prov/model.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     @property
     def namespaces(self) -> Set[Namespace]: ...
     @property
     def default_ns_uri(self) -> str | None: ...
     @property
     def document(self) -> ProvDocument | None: ...
     @property
-    def identifier(self) -> str | None: ...
+    def identifier(self) -> str | None | QualifiedName: ...
     @property
     def records(self) -> List[ProvRecord]: ...
     def set_default_namespace(self, uri: Namespace) -> None: ...
     def get_default_namespace(self) -> Namespace: ...
     def add_namespace(
         self, namespace_or_prefix: Namespace | str, uri: str | None = ...
     ) -> Namespace: ...
```

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/prov/serializers/provjson.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/prov/serializers/provjson.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/prov/serializers/provrdf.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/prov/serializers/provrdf.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/prov/serializers/provxml.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/prov/serializers/provxml.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/pydot.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/pydot.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/__init__.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/collection.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/collection.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/graph.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/graph.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_CSVW.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_CSVW.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_DCAT.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_DCAT.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_DCTERMS.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_DCTERMS.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_DOAP.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_DOAP.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_FOAF.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_FOAF.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_ODRL2.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_ODRL2.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_ORG.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_ORG.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_OWL.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_OWL.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_PROV.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_PROV.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_QB.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_QB.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_RDF.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_RDF.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_RDFS.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_RDFS.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_SDO.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_SDO.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_SH.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_SH.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_SKOS.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_SKOS.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_SOSA.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_SOSA.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_SSN.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_SSN.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_TIME.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_TIME.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_VOID.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_VOID.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/_XSD.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/_XSD.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/namespace/__init__.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/namespace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/paths.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/paths.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/query.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/query.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/resource.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/resource.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/rdflib/term.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/rdflib/term.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/subprocess.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/subprocess.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/mypy-stubs/urllib/parse.pyi` & `cwltool-3.1.20230526180938/mypy-stubs/urllib/parse.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/setup.py` & `cwltool-3.1.20230526180938/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 """Setup for the reference implementation of the CWL standards."""
 import os
 import sys
 import warnings
+from typing import Type
 
 import setuptools.command.egg_info as egg_info_cmd
 from setuptools import setup
 
 if os.name == "nt":
     warnings.warn(
         "The CWL reference runner (cwltool) no longer supports running "
@@ -23,15 +24,15 @@
 
 SETUP_DIR = os.path.dirname(__file__)
 README = os.path.join(SETUP_DIR, "README.rst")
 
 try:
     import gittaggers
 
-    Tagger = gittaggers.EggInfoFromGit
+    Tagger: Type[egg_info_cmd.egg_info] = gittaggers.EggInfoFromGit
 except ImportError:
     Tagger = egg_info_cmd.egg_info
 
 NEEDS_PYTEST = {"pytest", "test", "ptr"}.intersection(sys.argv)
 PYTEST_RUNNER = ["pytest-runner", "pytest-cov"] if NEEDS_PYTEST else []
 USE_MYPYC = False
 # To compile with mypyc, a mypyc checkout must be present on the PYTHONPATH
@@ -63,28 +64,32 @@
         # "cwltool/__main__.py",
         "cwltool/main.py",
         "cwltool/mutation.py",
         "cwltool/pack.py",
         "cwltool/pathmapper.py",
         "cwltool/process.py",
         "cwltool/procgenerator.py",
-        # "cwltool/provenance.py",  # WritableBag is having issues
+        # "cwltool/cwlprov/__init__.py",
+        "cwltool/cwlprov/provenance_constants.py",
+        "cwltool/cwlprov/provenance_profile.py",
+        "cwltool/cwlprov/ro.py",
+        # "cwltool/cwlprov/writablebagfile.py",  # WritableBag is having issues
         "cwltool/resolver.py",
         "cwltool/secrets.py",
         "cwltool/singularity.py",
         "cwltool/software_requirements.py",
         # "cwltool/stdfsaccess.py",  # StdFsAccess needs to be subclassable
         "cwltool/subgraph.py",
         "cwltool/update.py",
         "cwltool/utils.py",
         "cwltool/validate_js.py",
         "cwltool/workflow.py",
     ]
 
-    from mypyc.build import mypycify
+    from mypyc.build import mypycify  # type: ignore[import]
 
     opt_level = os.getenv("MYPYC_OPT_LEVEL", "3")
     ext_modules = mypycify(mypyc_targets, opt_level=opt_level)
 else:
     ext_modules = []
 
 setup(
@@ -96,22 +101,22 @@
     author="Common workflow language working group",
     author_email="common-workflow-language@googlegroups.com",
     url="https://github.com/common-workflow-language/cwltool",
     download_url="https://github.com/common-workflow-language/cwltool",
     ext_modules=ext_modules,
     # platforms='',  # empty as is conveyed by the classifier below
     # license='',  # empty as is conveyed by the classifier below
-    packages=["cwltool", "cwltool.tests"],
+    packages=["cwltool", "cwltool.tests", "cwltool.cwlprov"],
     package_dir={"cwltool.tests": "tests"},
     include_package_data=True,
     install_requires=[
         "setuptools",
         "requests >= 2.6.1",  # >= 2.6.1 to workaround
         # https://github.com/ionrock/cachecontrol/issues/137
-        "ruamel.yaml >= 0.15, < 0.17.27",
+        "ruamel.yaml >= 0.15, < 0.17.28",
         "rdflib >= 4.2.2, < 6.4.0",
         "rdflib >= 4.2.2, < 6.0.0;python_version<='3.6'",
         "shellescape >= 3.4.1, < 3.9",
         "schema-salad >= 8.4, < 9",
         "mypy-extensions",
         "psutil >= 5.6.6",
         "prov == 1.5.1",
```

### Comparing `cwltool-3.1.20230513155734/tests/2.fasta` & `cwltool-3.1.20230526180938/tests/2.fasta`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/bundle-context.jsonld` & `cwltool-3.1.20230526180938/tests/bundle-context.jsonld`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/checker_wf/broken-wf.cwl` & `cwltool-3.1.20230526180938/tests/checker_wf/broken-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/checker_wf/broken-wf2.cwl` & `cwltool-3.1.20230526180938/tests/checker_wf/broken-wf2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/checker_wf/broken-wf3.cwl` & `cwltool-3.1.20230526180938/tests/checker_wf/broken-wf3.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/checker_wf/circ-dep-wf.cwl` & `cwltool-3.1.20230526180938/tests/checker_wf/circ-dep-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/checker_wf/circ-dep-wf2.cwl` & `cwltool-3.1.20230526180938/tests/checker_wf/circ-dep-wf2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/checker_wf/functional-wf.cwl` & `cwltool-3.1.20230526180938/tests/checker_wf/functional-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/cwl-conformance/cwltool-conftest.py` & `cwltool-3.1.20230526180938/tests/cwl-conformance/cwltool-conftest.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/echo-badposition-expr.cwl` & `cwltool-3.1.20230526180938/tests/echo-badposition-expr.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/echo-position-expr.cwl` & `cwltool-3.1.20230526180938/tests/echo-position-expr.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/input_deps/docker-array-secondaryfiles.cwl` & `cwltool-3.1.20230526180938/tests/input_deps/docker-array-secondaryfiles.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/input_deps/ref.fasta` & `cwltool-3.1.20230526180938/tests/input_deps/ref.fasta`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/input_deps/ref2.fasta` & `cwltool-3.1.20230526180938/tests/input_deps/ref2.fasta`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/all-output-loop-no-iteration.cwl` & `cwltool-3.1.20230526180938/tests/loop/all-output-loop-no-iteration.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/all-output-loop.cwl` & `cwltool-3.1.20230526180938/tests/loop/all-output-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/default-value-loop.cwl` & `cwltool-3.1.20230526180938/tests/loop/default-value-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/invalid-loop-command-line-tool.cwl` & `cwltool-3.1.20230526180938/tests/loop/invalid-loop-command-line-tool.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/invalid-loop-hint.cwl` & `cwltool-3.1.20230526180938/tests/loop/invalid-loop-hint.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/invalid-loop-scatter.cwl` & `cwltool-3.1.20230526180938/tests/loop/invalid-loop-scatter.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/invalid-loop-when.cwl` & `cwltool-3.1.20230526180938/tests/loop/invalid-loop-when.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/invalid-loop-workflow.cwl` & `cwltool-3.1.20230526180938/tests/loop/invalid-loop-workflow.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/invalid-multi-source-loop-no-requirement.cwl` & `cwltool-3.1.20230526180938/tests/loop/invalid-multi-source-loop-no-requirement.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/invalid-no-loopWhen.cwl` & `cwltool-3.1.20230526180938/tests/loop/invalid-no-loopWhen.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/invalid-non-boolean-loopWhen.cwl` & `cwltool-3.1.20230526180938/tests/loop/invalid-non-boolean-loopWhen.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/invalid-value-from-loop-no-requirement.cwl` & `cwltool-3.1.20230526180938/tests/loop/invalid-value-from-loop-no-requirement.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/loop-inside-loop-all.cwl` & `cwltool-3.1.20230526180938/tests/loop/loop-inside-loop-all.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/loop-inside-loop.cwl` & `cwltool-3.1.20230526180938/tests/loop/loop-inside-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/loop-inside-scatter.cwl` & `cwltool-3.1.20230526180938/tests/loop/loop-inside-scatter.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/multi-source-loop.cwl` & `cwltool-3.1.20230526180938/tests/loop/multi-source-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/single-var-loop-no-iteration.cwl` & `cwltool-3.1.20230526180938/tests/loop/single-var-loop-no-iteration.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/single-var-loop.cwl` & `cwltool-3.1.20230526180938/tests/loop/single-var-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/two-vars-loop-2.cwl` & `cwltool-3.1.20230526180938/tests/loop/two-vars-loop-2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/two-vars-loop.cwl` & `cwltool-3.1.20230526180938/tests/loop/two-vars-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/loop/value-from-loop.cwl` & `cwltool-3.1.20230526180938/tests/loop/value-from-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/random_lines.cwl` & `cwltool-3.1.20230526180938/tests/random_lines.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/random_lines_mapping.cwl` & `cwltool-3.1.20230526180938/tests/random_lines_mapping.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/scatter_numbers.cwl` & `cwltool-3.1.20230526180938/tests/scatter_numbers.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/secondary-files-bad.cwl` & `cwltool-3.1.20230526180938/tests/secondary-files-bad.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/secondary-files.cwl` & `cwltool-3.1.20230526180938/tests/secondary-files.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/seqtk_seq_wrong_name.cwl` & `cwltool-3.1.20230526180938/tests/seqtk_seq_wrong_name.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/count-lines1-wf.cwl` & `cwltool-3.1.20230526180938/tests/subgraph/count-lines1-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/count-lines17-wf.cwl.json` & `cwltool-3.1.20230526180938/tests/subgraph/count-lines17-wf.cwl.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/env-wf2_subwf-packed.cwl` & `cwltool-3.1.20230526180938/tests/subgraph/env-wf2_subwf-packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/extract_count_output.json` & `cwltool-3.1.20230526180938/tests/subgraph/extract_count_output.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/extract_file1.json` & `cwltool-3.1.20230526180938/tests/subgraph/extract_file1.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/extract_file2.json` & `cwltool-3.1.20230526180938/tests/subgraph/extract_file2.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/extract_file3.json` & `cwltool-3.1.20230526180938/tests/subgraph/extract_file3.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/extract_output3.json` & `cwltool-3.1.20230526180938/tests/subgraph/extract_output3.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/extract_output4.json` & `cwltool-3.1.20230526180938/tests/subgraph/extract_output4.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/extract_output5.json` & `cwltool-3.1.20230526180938/tests/subgraph/extract_output5.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/extract_step1.json` & `cwltool-3.1.20230526180938/tests/subgraph/extract_step1.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/extract_step2.json` & `cwltool-3.1.20230526180938/tests/subgraph/extract_step2.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/extract_step2_1432.json` & `cwltool-3.1.20230526180938/tests/subgraph/extract_step2_1432.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/extract_step3.json` & `cwltool-3.1.20230526180938/tests/subgraph/extract_step3.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/extract_step4.json` & `cwltool-3.1.20230526180938/tests/subgraph/extract_step4.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/extract_step5.json` & `cwltool-3.1.20230526180938/tests/subgraph/extract_step5.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/single_step1.json` & `cwltool-3.1.20230526180938/tests/subgraph/single_step1.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/single_step2.json` & `cwltool-3.1.20230526180938/tests/subgraph/single_step2.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/single_step3.json` & `cwltool-3.1.20230526180938/tests/subgraph/single_step3.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/single_step4.json` & `cwltool-3.1.20230526180938/tests/subgraph/single_step4.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/single_step5.json` & `cwltool-3.1.20230526180938/tests/subgraph/single_step5.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/steplevel-resreq.cwl` & `cwltool-3.1.20230526180938/tests/subgraph/steplevel-resreq.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/subgraph/timelimit2-wf.cwl` & `cwltool-3.1.20230526180938/tests/subgraph/timelimit2-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_anon_types.py` & `cwltool-3.1.20230526180938/tests/test_anon_types.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import cast
 
 import pytest
+from ruamel.yaml.comments import CommentedMap
 from schema_salad.sourceline import cmap
 
 from cwltool.command_line_tool import CommandLineTool
 from cwltool.context import LoadingContext
-from ruamel.yaml.comments import CommentedMap
 
 snippet = cast(
     CommentedMap,
     cmap(
         [
             {
                 "cwlVersion": "v1.0",
```

### Comparing `cwltool-3.1.20230513155734/tests/test_bad_outputs_wf.cwl` & `cwltool-3.1.20230526180938/tests/test_bad_outputs_wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_conditionals.py` & `cwltool-3.1.20230526180938/tests/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_content_type.py` & `cwltool-3.1.20230526180938/tests/test_content_type.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_context.py` & `cwltool-3.1.20230526180938/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_cuda.py` & `cwltool-3.1.20230526180938/tests/test_cuda.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_default_path.py` & `cwltool-3.1.20230526180938/tests/test_default_path.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_dependencies.py` & `cwltool-3.1.20230526180938/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_docker.py` & `cwltool-3.1.20230526180938/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_docker_paths_with_colons.py` & `cwltool-3.1.20230526180938/tests/test_docker_paths_with_colons.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_empty_input.py` & `cwltool-3.1.20230526180938/tests/test_empty_input.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_environment.py` & `cwltool-3.1.20230526180938/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_examples.py` & `cwltool-3.1.20230526180938/tests/test_examples.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 from typing import Any, Dict, List, Union, cast
 
 import cwl_utils.expression as expr
 import pydot
 import pytest
 from cwl_utils.errors import JavascriptException
 from cwl_utils.sandboxjs import param_re
+from ruamel.yaml.comments import CommentedMap, CommentedSeq
 from schema_salad.exceptions import ValidationException
 
 import cwltool.checker
 import cwltool.factory
 import cwltool.pathmapper
 import cwltool.process
 import cwltool.workflow
 from cwltool.checker import can_assign_src_to_sink
 from cwltool.context import RuntimeContext
 from cwltool.errors import WorkflowException
 from cwltool.main import main
 from cwltool.process import CWL_IANA
 from cwltool.utils import CWLObjectType, dedup
-from ruamel.yaml.comments import CommentedMap, CommentedSeq
 
 from .util import get_data, get_main_output, needs_docker, working_directory
 
 sys.argv = [""]
 
 expression_match = [
     ("(foo)", True),
```

### Comparing `cwltool-3.1.20230513155734/tests/test_ext.py` & `cwltool-3.1.20230526180938/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_fetch.py` & `cwltool-3.1.20230526180938/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_http_input.py` & `cwltool-3.1.20230526180938/tests/test_http_input.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_input_deps.py` & `cwltool-3.1.20230526180938/tests/test_input_deps.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_iwdr.py` & `cwltool-3.1.20230526180938/tests/test_iwdr.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_js_sandbox.py` & `cwltool-3.1.20230526180938/tests/test_js_sandbox.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_load_tool.py` & `cwltool-3.1.20230526180938/tests/test_load_tool.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_loop.py` & `cwltool-3.1.20230526180938/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_make_template.py` & `cwltool-3.1.20230526180938/tests/test_make_template.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_misc_cli.py` & `cwltool-3.1.20230526180938/tests/test_misc_cli.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_mpi.py` & `cwltool-3.1.20230526180938/tests/test_mpi.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 import sys
 from io import StringIO
 from pathlib import Path
 from typing import Any, Generator, List, MutableMapping, Optional, Tuple
 
 import pkg_resources
 import pytest
+from ruamel.yaml.comments import CommentedMap, CommentedSeq
 from schema_salad.avro.schema import Names
 from schema_salad.utils import yaml_no_ts
 
 import cwltool.load_tool
 import cwltool.singularity
 import cwltool.udocker
 from cwltool.command_line_tool import CommandLineTool
 from cwltool.context import LoadingContext, RuntimeContext
 from cwltool.main import main
 from cwltool.mpi import MpiConfig, MPIRequirementName
-from ruamel.yaml.comments import CommentedMap, CommentedSeq
 
 from .util import get_data, working_directory
 
 
 def test_mpi_conf_defaults() -> None:
     mpi = MpiConfig()
     assert mpi.runner == "mpirun"
```

### Comparing `cwltool-3.1.20230513155734/tests/test_override.py` & `cwltool-3.1.20230526180938/tests/test_override.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_pack.py` & `cwltool-3.1.20230526180938/tests/test_pack.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_parallel.py` & `cwltool-3.1.20230526180938/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_path_checks.py` & `cwltool-3.1.20230526180938/tests/test_path_checks.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import urllib.parse
 from io import BytesIO
 from pathlib import Path
 from typing import IO, Any, List, cast
 
 import pytest
+from ruamel.yaml.comments import CommentedMap
 from schema_salad.sourceline import cmap
 
 from cwltool.command_line_tool import CommandLineTool
 from cwltool.context import LoadingContext, RuntimeContext
 from cwltool.main import main
 from cwltool.stdfsaccess import StdFsAccess
 from cwltool.update import INTERNAL_VERSION
 from cwltool.utils import CWLObjectType
-from ruamel.yaml.comments import CommentedMap
 
 from .util import needs_docker
 
 script = """
 #!/usr/bin/env cwl-runner
 cwlVersion: v1.0
 class: CommandLineTool
```

### Comparing `cwltool-3.1.20230513155734/tests/test_pathmapper.py` & `cwltool-3.1.20230526180938/tests/test_pathmapper.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_procgenerator.py` & `cwltool-3.1.20230526180938/tests/test_procgenerator.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_provenance.py` & `cwltool-3.1.20230526180938/tests/test_provenance.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 import arcp
 import bagit
 import pytest
 from rdflib import Graph, Namespace, URIRef
 from rdflib.namespace import DC, DCTERMS, RDF
 from rdflib.term import Literal
 
-from cwltool import provenance, provenance_constants
+import cwltool.cwlprov as provenance
+from cwltool.cwlprov import provenance_constants
+from cwltool.cwlprov.ro import ResearchObject
+from cwltool.cwlprov.writablebagfile import close_ro, write_bag_file
 from cwltool.main import main
-from cwltool.provenance import ResearchObject
 from cwltool.stdfsaccess import StdFsAccess
 
 from .util import get_data, needs_docker, working_directory
 
 # RDF namespaces we'll query for later
 ORE = Namespace("http://www.openarchives.org/ore/terms/")
 PROV = Namespace("http://www.w3.org/ns/prov#")
@@ -78,14 +80,27 @@
         get_data("tests/wf/revsort-job.json"),
     )
     check_output_object(folder)
     check_provenance(folder)
 
 
 @needs_docker
+def test_revsort_workflow_shortcut(tmp_path: Path) -> None:
+    """Confirm that using 'cwl:tool' shortcut still snapshots the CWL files."""
+    folder = cwltool(
+        tmp_path,
+        get_data("tests/wf/revsort-job-shortcut.json"),
+    )
+    check_output_object(folder)
+    check_provenance(folder)
+    assert not (folder / "snapshot" / "revsort-job-shortcut.json").exists()
+    assert len(list((folder / "snapshot").iterdir())) == 4
+
+
+@needs_docker
 def test_nested_workflow(tmp_path: Path) -> None:
     check_provenance(cwltool(tmp_path, get_data("tests/wf/nested.cwl")), nested=True)
 
 
 @needs_docker
 def test_secondary_files_implicit(tmp_path: Path) -> None:
     file1 = tmp_path / "foo1.txt"
@@ -590,29 +605,29 @@
             assert str(prim_basename) == f"{prim_nameroot}{prim_nameext}"
 
 
 @pytest.fixture
 def research_object(tmp_path: Path) -> Generator[ResearchObject, None, None]:
     re_ob = ResearchObject(StdFsAccess(str(tmp_path / "ro")), temp_prefix_ro=str(tmp_path / "tmp"))
     yield re_ob
-    re_ob.close()
+    close_ro(re_ob)
 
 
 def test_absolute_path_fails(research_object: ResearchObject) -> None:
     with pytest.raises(ValueError):
-        research_object.write_bag_file("/absolute/path/fails")
+        write_bag_file(research_object, "/absolute/path/fails")
 
 
 def test_climboutfails(research_object: ResearchObject) -> None:
     with pytest.raises(ValueError):
-        research_object.write_bag_file("../../outside-ro")
+        write_bag_file(research_object, "../../outside-ro")
 
 
 def test_writable_string(research_object: ResearchObject) -> None:
-    with research_object.write_bag_file("file.txt") as fh:
+    with write_bag_file(research_object, "file.txt") as fh:
         assert fh.writable()
         fh.write("Hello\n")
 
     sha1 = os.path.join(research_object.folder, "tagmanifest-sha1.txt")
     assert os.path.isfile(sha1)
 
     with open(sha1, encoding="UTF-8") as sha_file:
@@ -636,55 +651,55 @@
     )
 
     sha512 = os.path.join(research_object.folder, "tagmanifest-sha512.txt")
     assert os.path.isfile(sha512)
 
 
 def test_writable_unicode_string(research_object: ResearchObject) -> None:
-    with research_object.write_bag_file("file.txt") as fh:
+    with write_bag_file(research_object, "file.txt") as fh:
         assert fh.writable()
         fh.write("Here is a snowman: \u2603 \n")
 
 
 def test_writable_bytes(research_object: ResearchObject) -> None:
     string = "Here is a snowman: \u2603 \n".encode()
-    with research_object.write_bag_file("file.txt", encoding=None) as fh:
+    with write_bag_file(research_object, "file.txt", encoding=None) as fh:
         fh.write(string)  # type: ignore
 
 
 def test_data(research_object: ResearchObject) -> None:
-    with research_object.write_bag_file("data/file.txt") as fh:
+    with write_bag_file(research_object, "data/file.txt") as fh:
         assert fh.writable()
         fh.write("Hello\n")
 
     # Because this is under data/ it should add to manifest
     # rather than tagmanifest
     sha1 = os.path.join(research_object.folder, "manifest-sha1.txt")
     assert os.path.isfile(sha1)
     with open(sha1, encoding="UTF-8") as fh2:
         stripped_sha = fh2.readline().strip()
         assert stripped_sha.endswith("data/file.txt")
 
 
 def test_not_seekable(research_object: ResearchObject) -> None:
-    with research_object.write_bag_file("file.txt") as fh:
+    with write_bag_file(research_object, "file.txt") as fh:
         assert not fh.seekable()
         with pytest.raises(OSError):
             fh.seek(0)
 
 
 def test_not_readable(research_object: ResearchObject) -> None:
-    with research_object.write_bag_file("file.txt") as fh:
+    with write_bag_file(research_object, "file.txt") as fh:
         assert not fh.readable()
         with pytest.raises(OSError):
             fh.read()
 
 
 def test_truncate_fails(research_object: ResearchObject) -> None:
-    with research_object.write_bag_file("file.txt") as fh:
+    with write_bag_file(research_object, "file.txt") as fh:
         fh.write("Hello there")
         fh.truncate()  # OK as we're always at end
         # Will fail because the checksum can't rewind
         with pytest.raises(OSError):
             fh.truncate(0)
```

### Comparing `cwltool-3.1.20230513155734/tests/test_rdfprint.py` & `cwltool-3.1.20230526180938/tests/test_rdfprint.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_recursive_validation.py` & `cwltool-3.1.20230526180938/tests/test_recursive_validation.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_relocate.py` & `cwltool-3.1.20230526180938/tests/test_relocate.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_secrets.py` & `cwltool-3.1.20230526180938/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_singularity.py` & `cwltool-3.1.20230526180938/tests/test_singularity.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_singularity_versions.py` & `cwltool-3.1.20230526180938/tests/test_singularity_versions.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_stdout_stderr_log_dir.py` & `cwltool-3.1.20230526180938/tests/test_stdout_stderr_log_dir.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_streaming.py` & `cwltool-3.1.20230526180938/tests/test_streaming.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Test that files marked as 'streamable' when 'streaming_allowed' can be named pipes."""
 import os
 from pathlib import Path
 from typing import cast
 
 import pytest
+from ruamel.yaml.comments import CommentedMap
 from schema_salad.sourceline import cmap
 
 from cwltool.command_line_tool import CommandLineTool
 from cwltool.context import LoadingContext, RuntimeContext
 from cwltool.errors import WorkflowException
 from cwltool.job import JobBase
 from cwltool.update import INTERNAL_VERSION, ORIGINAL_CWLVERSION
 from cwltool.utils import CWLObjectType
-from ruamel.yaml.comments import CommentedMap
 
 from .util import get_data
 
 toolpath_object = cast(
     CommentedMap,
     cmap(
         {
```

### Comparing `cwltool-3.1.20230513155734/tests/test_subclass_mypyc.py` & `cwltool-3.1.20230526180938/tests/test_subclass_mypyc.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 Especially if those classes are (or become) compiled with mypyc.
 """
 
 import pickle
 
 import pytest
+from ruamel.yaml.comments import CommentedMap
 from schema_salad.avro import schema
 
 from cwltool.builder import Builder
 from cwltool.command_line_tool import CommandLineTool, ExpressionTool
 from cwltool.context import LoadingContext, RuntimeContext
 from cwltool.stdfsaccess import StdFsAccess
 from cwltool.update import INTERNAL_VERSION
-from ruamel.yaml.comments import CommentedMap
 
 from .test_anon_types import snippet
 
 
 @pytest.mark.parametrize("snippet", snippet)
 def test_subclass_CLT(snippet: CommentedMap) -> None:
     """We can subclass CommandLineTool."""
```

### Comparing `cwltool-3.1.20230513155734/tests/test_subgraph.py` & `cwltool-3.1.20230526180938/tests/test_subgraph.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_target.py` & `cwltool-3.1.20230526180938/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_tmpdir.py` & `cwltool-3.1.20230526180938/tests/test_tmpdir.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 import re
 import subprocess
 import sys
 from pathlib import Path
 from typing import List, cast
 
 import pytest
+from ruamel.yaml.comments import CommentedMap
 from schema_salad.avro import schema
 from schema_salad.sourceline import cmap
 
 from cwltool.builder import Builder
 from cwltool.command_line_tool import CommandLineTool
 from cwltool.context import LoadingContext, RuntimeContext
 from cwltool.docker import DockerCommandLineJob
 from cwltool.job import JobBase
 from cwltool.main import main
 from cwltool.pathmapper import MapperEnt
 from cwltool.stdfsaccess import StdFsAccess
 from cwltool.update import INTERNAL_VERSION, ORIGINAL_CWLVERSION
 from cwltool.utils import create_tmp_dir
-from ruamel.yaml.comments import CommentedMap
 
 from .util import get_data, get_main_output, needs_docker
 
 
 def test_docker_commandLineTool_job_tmpdir_prefix(tmp_path: Path) -> None:
     """Test that docker enabled CommandLineTool respects temp directory directives."""
     loading_context = LoadingContext(
```

### Comparing `cwltool-3.1.20230513155734/tests/test_toolargparse.py` & `cwltool-3.1.20230526180938/tests/test_toolargparse.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_trs.py` & `cwltool-3.1.20230526180938/tests/test_trs.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_udocker.py` & `cwltool-3.1.20230526180938/tests/test_udocker.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_validate.py` & `cwltool-3.1.20230526180938/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_validate_js.py` & `cwltool-3.1.20230526180938/tests/test_validate_js.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/test_windows_warning.py` & `cwltool-3.1.20230526180938/tests/test_windows_warning.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/trs/Dockstore.cwl` & `cwltool-3.1.20230526180938/tests/trs/Dockstore.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/trs/md5sum-tool.cwl` & `cwltool-3.1.20230526180938/tests/trs/md5sum-tool.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/utf_doc_example.cwl` & `cwltool-3.1.20230526180938/tests/utf_doc_example.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/util.py` & `cwltool-3.1.20230526180938/tests/util.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/910.cwl` & `cwltool-3.1.20230526180938/tests/wf/910.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/bad_formattest.cwl` & `cwltool-3.1.20230526180938/tests/wf/bad_formattest.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/bad_formattest2.cwl` & `cwltool-3.1.20230526180938/tests/wf/bad_formattest2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/conflict.cwl` & `cwltool-3.1.20230526180938/tests/wf/conflict.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/directory.cwl` & `cwltool-3.1.20230526180938/tests/wf/directory.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/double-nested.cwl` & `cwltool-3.1.20230526180938/tests/wf/double-nested.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/echo.cwl` & `cwltool-3.1.20230526180938/tests/wf/echo.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/expect_iwd-passthrough1_packed.cwl` & `cwltool-3.1.20230526180938/tests/wf/expect_iwd-passthrough1_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/expect_packed.cwl` & `cwltool-3.1.20230526180938/tests/wf/expect_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/expect_revsort_datetime_packed.cwl` & `cwltool-3.1.20230526180938/tests/wf/expect_revsort_datetime_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/expect_trick_packed.cwl` & `cwltool-3.1.20230526180938/tests/wf/expect_trick_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/floats_small_and_large.cwl` & `cwltool-3.1.20230526180938/tests/wf/floats_small_and_large.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/generator/pytoolgen.cwl` & `cwltool-3.1.20230526180938/tests/wf/generator/pytoolgen.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/hello-workflow-badhints.cwl` & `cwltool-3.1.20230526180938/tests/wf/hello-workflow-badhints.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/hello-workflow-badhints2.cwl` & `cwltool-3.1.20230526180938/tests/wf/hello-workflow-badhints2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/hello-workflow.cwl` & `cwltool-3.1.20230526180938/tests/wf/hello-workflow.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/iwd-passthrough1.cwl` & `cwltool-3.1.20230526180938/tests/wf/iwd-passthrough1.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/iwdr-passthrough-successive.cwl` & `cwltool-3.1.20230526180938/tests/wf/iwdr-passthrough-successive.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/iwdr_permutations.cwl` & `cwltool-3.1.20230526180938/tests/wf/iwdr_permutations.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/iwdr_permutations_nocontainer.cwl` & `cwltool-3.1.20230526180938/tests/wf/iwdr_permutations_nocontainer.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/missing_cwlVersion.cwl` & `cwltool-3.1.20230526180938/tests/wf/missing_cwlVersion.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/mpi_expr.cwl` & `cwltool-3.1.20230526180938/tests/wf/mpi_expr.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/mpi_simple_wf.cwl` & `cwltool-3.1.20230526180938/tests/wf/mpi_simple_wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/nested.cwl` & `cwltool-3.1.20230526180938/tests/wf/nested.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/operation/expect_operation-single_packed.cwl` & `cwltool-3.1.20230526180938/tests/wf/operation/expect_operation-single_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/operation/operation-single.cwl` & `cwltool-3.1.20230526180938/tests/wf/operation/operation-single.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/packed-with-loadlisting.cwl` & `cwltool-3.1.20230526180938/tests/wf/packed-with-loadlisting.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/packed_no_main.cwl` & `cwltool-3.1.20230526180938/tests/wf/packed_no_main.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/paramref_arguments_roundtrip.cwl` & `cwltool-3.1.20230526180938/tests/wf/paramref_arguments_roundtrip.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/paramref_arguments_self.cwl` & `cwltool-3.1.20230526180938/tests/wf/paramref_arguments_self.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/record_outputeval.cwl` & `cwltool-3.1.20230526180938/tests/wf/record_outputeval.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/revsort.cwl` & `cwltool-3.1.20230526180938/tests/wf/revsort.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/revsort_datetime.cwl` & `cwltool-3.1.20230526180938/tests/wf/revsort_datetime.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/revsort_step_bad_schema.cwl` & `cwltool-3.1.20230526180938/tests/wf/revsort_step_bad_schema.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/revtool.cwl` & `cwltool-3.1.20230526180938/tests/wf/revtool.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/revtool_bad_schema.cwl` & `cwltool-3.1.20230526180938/tests/wf/revtool_bad_schema.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/scatter-wf4.cwl` & `cwltool-3.1.20230526180938/tests/wf/scatter-wf4.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/scatter-wf4.json` & `cwltool-3.1.20230526180938/tests/wf/scatter-wf4.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/scatter2.cwl` & `cwltool-3.1.20230526180938/tests/wf/scatter2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/scatter2_subwf.cwl` & `cwltool-3.1.20230526180938/tests/wf/scatter2_subwf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/scatterfail.cwl` & `cwltool-3.1.20230526180938/tests/wf/scatterfail.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/schemadef-bug-1473.cwl` & `cwltool-3.1.20230526180938/tests/wf/schemadef-bug-1473.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/sec-wf-out.cwl` & `cwltool-3.1.20230526180938/tests/wf/sec-wf-out.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/sorttool.cwl` & `cwltool-3.1.20230526180938/tests/wf/sorttool.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/three_step_color.cwl` & `cwltool-3.1.20230526180938/tests/wf/three_step_color.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/trick_revsort.cwl` & `cwltool-3.1.20230526180938/tests/wf/trick_revsort.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/updateval_inplace.cwl` & `cwltool-3.1.20230526180938/tests/wf/updateval_inplace.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/wffail.cwl` & `cwltool-3.1.20230526180938/tests/wf/wffail.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/whale.txt` & `cwltool-3.1.20230526180938/tests/wf/whale.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tests/wf/wrong_cwlVersion.cwl` & `cwltool-3.1.20230526180938/tests/wf/wrong_cwlVersion.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230513155734/tox.ini` & `cwltool-3.1.20230526180938/tox.ini`

 * *Files identical despite different names*

