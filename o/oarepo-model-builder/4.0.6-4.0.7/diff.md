# Comparing `tmp/oarepo-model-builder-4.0.6.tar.gz` & `tmp/oarepo-model-builder-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-4.0.6.tar", last modified: Thu May 25 12:14:06 2023, max compression
+gzip compressed data, was "oarepo-model-builder-4.0.7.tar", last modified: Fri May 26 10:23:01 2023, max compression
```

## Comparing `oarepo-model-builder-4.0.6.tar` & `oarepo-model-builder-4.0.7.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.944024 oarepo-model-builder-4.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 12:14:06.944024 oarepo-model-builder-4.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.892024 oarepo-model-builder-4.0.6/oarepo_model_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.896024 oarepo-model-builder-4.0.6/oarepo_model_builder/builders/
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builders/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builders/json_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builders/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builders/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builders/model_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builders/pyproject_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builders/python.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builders/python_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builders/setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builders/setup_py.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.896024 oarepo-model-builder-4.0.6/oarepo_model_builder/builders/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builders/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builders/templates/setup.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builders/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.896024 oarepo-model-builder-4.0.6/oarepo_model_builder/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/builtin_models/invenio.json
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.896024 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.896024 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.900024 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/facets/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/facets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/facets/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/facets/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/facets/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/facets/object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.900024 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/object.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.904024 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/blueprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/model_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/record_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/search_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.904024 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/containers/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/containers/array.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/containers/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/containers/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/containers/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/primitive_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/generate_doc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.912024 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_api_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_app_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_pid_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_resource_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_search_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_ui_marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_ui_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_script_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.916024 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/api_views.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/app_views.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/ext.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/imports.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/invenio_record_facets.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/marshmallow.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/permissions.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/pid_provider.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/proxies.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/record_dumper.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/resource.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/resource_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/service.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/service_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/ui_serializer.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/version.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.916024 oarepo-model-builder-4.0.6/oarepo_model_builder/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/merger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.924024 oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/json_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/python.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.924024 oarepo-model-builder-4.0.6/oarepo_model_builder/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/profiles/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/profiles/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.928024 oarepo-model-builder-4.0.6/oarepo_model_builder/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/settings/opensearch.json
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/settings/python.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.928024 oarepo-model-builder-4.0.6/oarepo_model_builder/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.932024 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/absolute_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/camelcase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.932024 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/cst/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/cst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/cst/call.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/cst/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/cst/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/cst/indented_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/cst/mergers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/cst/simple_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/deepmerge.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/facet_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/import_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/python_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/utils/verbose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.936024 oarepo-model-builder-4.0.6/oarepo_model_builder/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/validation/extensibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/validation/model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/oarepo_model_builder/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.892024 oarepo-model-builder-4.0.6/oarepo_model_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 12:14:06.000000 oarepo-model-builder-4.0.6/oarepo_model_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-05-25 12:14:06.000000 oarepo-model-builder-4.0.6/oarepo_model_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:14:06.000000 oarepo-model-builder-4.0.6/oarepo_model_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-25 12:14:06.000000 oarepo-model-builder-4.0.6/oarepo_model_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-25 12:14:06.000000 oarepo-model-builder-4.0.6/oarepo_model_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 12:14:06.000000 oarepo-model-builder-4.0.6/oarepo_model_builder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-25 12:14:06.944024 oarepo-model-builder-4.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:14:06.944024 oarepo-model-builder-4.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/faker_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/multilang.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_builder_from_entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_cfg_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_datatype_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_datatype_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_empty_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)   396304 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_extend.py
--rw-r--r--   0 runner    (1001) docker     (123)    28951 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_fulltext_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_jsonchema_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_mapping_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_marshmallow_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_marshmallow_ui_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    23543 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_model_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_overwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_pid_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_plugin_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_python_mergers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_sample_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_schema_props.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_search_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_simple_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_template_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_type_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-25 12:12:57.000000 oarepo-model-builder-4.0.6/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.165020 oarepo-model-builder-4.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-26 10:23:01.165020 oarepo-model-builder-4.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.137019 oarepo-model-builder-4.0.7/oarepo_model_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.141020 oarepo-model-builder-4.0.7/oarepo_model_builder/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builders/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builders/json_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builders/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builders/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builders/model_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builders/pyproject_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builders/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builders/python_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builders/setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builders/setup_py.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.141020 oarepo-model-builder-4.0.7/oarepo_model_builder/builders/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builders/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builders/templates/setup.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builders/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.141020 oarepo-model-builder-4.0.7/oarepo_model_builder/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/builtin_models/invenio.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.141020 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.141020 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.141020 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/facets/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/facets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/facets/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/facets/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/facets/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/facets/object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.145020 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.145020 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/model_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/record_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/search_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.149020 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/containers/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/containers/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/containers/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/containers/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/primitive_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/generate_doc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.153020 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_api_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_app_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_pid_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_resource_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_search_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_ui_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_ui_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_script_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.153020 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/api_views.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/app_views.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/ext.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/imports.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/invenio_record_facets.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/marshmallow.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/permissions.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/pid_provider.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/proxies.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/record_dumper.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/resource.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/resource_config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/service.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/service_config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/ui_serializer.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/version.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.153020 oarepo-model-builder-4.0.7/oarepo_model_builder/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/merger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.157020 oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/json_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.157020 oarepo-model-builder-4.0.7/oarepo_model_builder/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/profiles/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/profiles/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.157020 oarepo-model-builder-4.0.7/oarepo_model_builder/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/settings/opensearch.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/settings/python.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.157020 oarepo-model-builder-4.0.7/oarepo_model_builder/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.157020 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/absolute_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/camelcase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.161020 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/cst/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/cst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/cst/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/cst/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/cst/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/cst/indented_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/cst/mergers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/cst/simple_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/deepmerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/facet_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/import_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/python_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/utils/verbose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.161020 oarepo-model-builder-4.0.7/oarepo_model_builder/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/validation/extensibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/validation/model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/oarepo_model_builder/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.137019 oarepo-model-builder-4.0.7/oarepo_model_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-26 10:23:01.000000 oarepo-model-builder-4.0.7/oarepo_model_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-05-26 10:23:01.000000 oarepo-model-builder-4.0.7/oarepo_model_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:23:01.000000 oarepo-model-builder-4.0.7/oarepo_model_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-26 10:23:01.000000 oarepo-model-builder-4.0.7/oarepo_model_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-26 10:23:01.000000 oarepo-model-builder-4.0.7/oarepo_model_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 10:23:01.000000 oarepo-model-builder-4.0.7/oarepo_model_builder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-26 10:23:01.165020 oarepo-model-builder-4.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:23:01.165020 oarepo-model-builder-4.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/faker_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/multilang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_builder_from_entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_cfg_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_datatype_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_datatype_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_empty_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)   396304 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29556 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_fulltext_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_jsonchema_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_mapping_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_marshmallow_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_marshmallow_ui_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23543 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_model_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_overwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_pid_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_plugin_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_python_mergers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_sample_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_schema_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_search_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_simple_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_template_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_type_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-26 10:22:16.000000 oarepo-model-builder-4.0.7/tests/utils.py
```

### Comparing `oarepo-model-builder-4.0.6/LICENSE` & `oarepo-model-builder-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/PKG-INFO` & `oarepo-model-builder-4.0.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder
-Version: 4.0.6
+Version: 4.0.7
 Summary: A utility library that generates OARepo required data model files from a JSON specification file
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo model builder
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/builder.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/builders/__init__.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/builders/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 
     def build_children(self, parent_node):
         for child in parent_node.children.items():
             self._build_node_internal(child)
 
     def build_node(self, datatype: DataType):
         "Intended to be overriden in children"
-        pass
 
 
 TEMPLATES = {
     "setup_py": "templates/setup.py.jinja2",
 }
 
 __all__ = [
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/builders/extend.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/builders/extend.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/builders/json_base.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/builders/json_base.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/builders/jsonschema.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/builders/jsonschema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/builders/mapping.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/builders/mapping.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/builders/model_saver.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/builders/model_saver.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/builders/python.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/builders/python.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,8 +17,7 @@
         )
 
     def class_to_path(self, class_name):
         return self.module_to_path(package_name(class_name))
 
     def build_node(self, datatype):
         "intended to be overridden in children"
-        pass
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/builders/python_structure.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/builders/python_structure.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/builders/setup_cfg.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/builders/setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/builders/utils.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/builders/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/builtin_models/invenio.json` & `oarepo-model-builder-4.0.7/oarepo_model_builder/builtin_models/invenio.json`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/cli.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/__init__.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     IntegerDataType,
 )
 from .strings import StringDataType  # noqa , just for export
 from .strings import (  # noqa
     FulltextDataType,
     FulltextKeywordDataType,
     KeywordDataType,
-    StringDataType,
     URLDataType,
     UUIDDataType,
 )
 
 DEFAULT_DATATYPES = [
     IntegerDataType,
     FloatDataType,
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/__init__.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from .enum import EnumComponent
-
-from .facets import (
-    ArrayFacetsComponent,
-    NestedFacetsComponent,
-    ObjectFacetsComponent,
-    RegularFacetsComponent,
-)
-
+from .facets.array import ArrayFacetsComponent
+from .facets.field import RegularFacetsComponent
+from .facets.nested import NestedFacetsComponent
+from .facets.object import ObjectFacetsComponent
 from .marshmallow import (
     ArrayMarshmallowComponent,
     ObjectMarshmallowComponent,
     RegularMarshmallowComponent,
     UIArrayMarshmallowComponent,
     UIMarshmallowComponent,
     UIObjectMarshmallowComponent,
@@ -74,9 +70,8 @@
     DefaultsModelComponent,
     ProxyModelComponent,
     PluginsModelComponent,
     ObjectFacetsComponent,
     NestedFacetsComponent,
     RegularFacetsComponent,
     ArrayFacetsComponent,
-
 ]
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/enum.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/enum.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/facets/field.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/facets/field.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import marshmallow as ma
 from marshmallow import fields
 
 from oarepo_model_builder.datatypes import datatypes
-from oarepo_model_builder.utils.facet_helpers import facet_name
+from oarepo_model_builder.utils.facet_helpers import facet_name, flatten
 from oarepo_model_builder.validation.utils import ImportSchema
 
 from ...datatypes import DataTypeComponent
+from . import FacetDefinition
 
 
 class FacetsSchema(ma.Schema):
     class Meta:
         unknown = ma.RAISE
 
     searchable = ma.fields.Bool(required=False)
@@ -27,52 +28,53 @@
 
     class ModelSchema(ma.Schema):
         facets = ma.fields.Nested(
             FacetsSchema,
             required=False,
         )
 
-    def build_facets(self, datatype, facets, facet_definition=None, searchable=True):
-        facet_section = datatype.section_facets
-        if not facet_section.config == {}:
-            _path = datatype.path
-            if "keyword" in datatype.section_facets.config:
-                _path = _path + ".keyword"
-            if "path" in facet_section.config:
-                path = _path + "." + facet_section.config["path"]
-
-            else:
-                path = _path
-            key = facet_section.config.get("key", facet_name(_path))
-            label = facet_section.config.get(
-                "label", f'{_path.replace(".", "/")}.label'
-            )
-            facet_searchable = facet_section.config.get("searchable", searchable)
-            imports = facet_section.config.get("imports", [])
-            arguments = facet_section.config.get("args", [])
-            arguments_string = ",".join(arguments)
-            if arguments_string != "":
-                arguments_string = "," + arguments_string
-            field = facet_section.config.get(
-                "field",
-                datatype.section_facets.config["facet_class"]
-                + f'(field="{path}", label =_("{label}") {arguments_string} '
-                + ")",
-            )
-            facet_definition = {
-                "path": key,
-                "class": field,
-                "facet_searchable": facet_searchable,
-                "imports": imports,
-            }
-        datatypes.call_components(
-            datatype.parent,
-            "build_definition",
-            facets=facets,
-            facet_definition=facet_definition,
-            searchable=searchable,
+    def facet_path(self, datatype, facet_section):
+        _path = datatype.path
+        if "path" in facet_section:
+            path = _path + "." + facet_section["path"]
+        else:
+            path = _path
+        return path
+
+    def process_facets(self, datatype, section, **__kwargs):
+        # create the facet definition
+        facet_section = section.config
+
+        path = self.facet_path(datatype, facet_section)
+        facet_definition = FacetDefinition(
+            path=facet_section.get("key", facet_name(datatype.path)),
+            dot_path=datatype.path,
+            searchable=facet_section.get("searchable"),
+            imports=facet_section.get("imports", []),
+        )
+
+        # set the field on the definition
+        label = facet_section.get("label", f'{datatype.path.replace(".", "/")}.label')
+        facet_definition.set_field(
+            facet_section,
+            arguments=[
+                f"field={repr(path)}",
+                f"label =_({repr(label)})",
+                *facet_section.get("args", []),
+            ],
         )
 
-    def create_definition(self, config, datatype):
-        return {
-            datatype.path: config["facet_class"] + f'(field="{datatype.path}"' + ")"
-        }
+        # if there is indeed a facet here, process via parents
+        if facet_definition.field:
+            facets = flatten(
+                datatypes.call_components(
+                    datatype.parent,
+                    "build_facet_definition",
+                    facet_definition=facet_definition,
+                )
+            )
+        else:
+            facets = []
+
+        # and store it on the element
+        section.config["facets"] = facets
+        return section
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/facets/object.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/facets/array.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,23 @@
-from oarepo_model_builder.datatypes import ObjectDataType, datatypes
+from oarepo_model_builder.datatypes import ArrayDataType, datatypes
+from oarepo_model_builder.utils.facet_helpers import flatten
 
+from . import FacetDefinition
 from .field import RegularFacetsComponent
 
 
-class ObjectFacetsComponent(RegularFacetsComponent):
-    eligible_datatypes = [ObjectDataType]
+class ArrayFacetsComponent(RegularFacetsComponent):
+    eligible_datatypes = [ArrayDataType]
 
-    def build_definition(
-        self, datatype, facets, facet_definition=None, searchable=True
+    def build_facet_definition(
+        self,
+        datatype,
+        facet_definition: FacetDefinition,
     ):
-        if datatype.key is not None:
-            facet_section = datatype.section_facets.config
-            if facet_section != {}:
-                facet_searchable = facet_section.get("searchable", "")
-                if facet_definition:
-                    imports = facet_section.get("imports", [])
-                    facet_definition["imports"].extend(imports)
-                    fs = facet_definition.get("facet_searchable", "")
-                    if fs != "" and facet_searchable != "" and fs != facet_searchable:
-                        facet_definition["facet_searchable"] = facet_searchable
-        datatypes.call_components(
-            datatype.parent,
-            "build_definition",
-            facets=facets,
-            facet_definition=facet_definition,
-            searchable=searchable,
+        facet_definition.update(datatype.section_facets.config)
+        return flatten(
+            datatypes.call_components(
+                datatype.parent,
+                "build_facet_definition",
+                facet_definition=facet_definition,
+            )
         )
-
-    def build_facets(self, datatype, facets, facet_definition=None, searchable=True):
-        pass
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/__init__.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/array.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/array.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import List
 
-
 from oarepo_model_builder.datatypes.containers.array import ArrayDataType
 from oarepo_model_builder.datatypes.datatypes import DataType, Section, datatypes
 
 from .field import RegularMarshmallowComponent, RegularMarshmallowComponentMixin
 from .graph import MarshmallowField
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/field.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/field.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/graph.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import dataclasses
 from typing import List, Optional, Set
 
+from oarepo_model_builder.validation import InvalidModelException
+
 from ....utils.python_name import base_name, package_name
 from ...datatypes import Import
-from oarepo_model_builder.validation import InvalidModelException
 
 
 @dataclasses.dataclass
 class MarshmallowField:
     key: str
     definition: str
     imports: List[Import] = dataclasses.field(default_factory=list)
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/object.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/object.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/__init__.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/app.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/app.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/blueprints.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/blueprints.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/defaults.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/defaults.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/jsonschema.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/jsonschema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/mapping.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/mapping.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/marshmallow.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/marshmallow.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/model_saver.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/model_saver.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/permissions.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/permissions.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/pid.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/pid.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/plugins.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/plugins.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/proxy.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/proxy.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/record.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/record.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/record_dumper.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/record_dumper.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/record_metadata.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/record_metadata.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/resource.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/sample.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/sample.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/search_options.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/search_options.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/service.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/service.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/ui.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Dict
 
 import marshmallow as ma
 
 from oarepo_model_builder.datatypes import ModelDataType
 from oarepo_model_builder.utils.python_name import parent_module
 from oarepo_model_builder.validation.utils import ImportSchema
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/model/utils.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/model/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/sample.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/sample.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/components/ui.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/components/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/containers/array.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/containers/array.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,17 +13,14 @@
         }
     }
     marshmallow = {
         "field-class": "ma_fields.List",
     }
     json_schema = {"type": "array"}
 
-    facets = {"facet_class": "TermsFacet"}
-
-
     class ModelSchema(DataType.ModelSchema):
         items = fields.Nested(FieldSchema)
         uniqueItems = fields.Boolean(required=False)
         minItems = fields.Integer(required=False)
         maxItems = fields.Integer(required=False)
 
     def prepare(self, context):
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/containers/object.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/containers/object.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/datatypes.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import dataclasses
 import json
 from collections.abc import Mapping
 from functools import cached_property, lru_cache
-from typing import Any, Dict, List, Type, Union, Optional
+from typing import Any, Dict, List, Optional, Type, Union
 
 import importlib_metadata
 import marshmallow as ma
 from marshmallow import fields
 
 from ..utils.deepmerge import deepmerge
 from ..utils.import_class import import_class
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/dates.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/dates.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from .datatypes import DataType
 
 
 class BaseDateDataType(DataType):
-
     marshmallow = {"field-class": "ma_fields.String"}
 
     facets = {
         "facet_class": "DateTimeFacet",
         "imports": [{"import": "oarepo_runtime.facets.date.DateTimeFacet"}],
     }
 
 
-
 class DateDataType(BaseDateDataType):
     model_type = "date"
     ui = {
         "marshmallow": {
             "field-class": "l10n.LocalizedDate",
             "imports": [
                 {"import": "oarepo_runtime.ui.marshmallow", "alias": "l10n"}  # NOSONAR
@@ -41,15 +39,18 @@
         }
     }
     marshmallow = {
         "field-class": "ma_fields.String",
         "validators": ["validate_date('%H:%M:%S')"],
         "imports": [{"import": "oarepo_runtime.validation.validate_date"}],
     }
-    mapping = {"type": "date", "format": "strict_time||strict_time_no_millis||basic_time||basic_time_no_millis"}
+    mapping = {
+        "type": "date",
+        "format": "strict_time||strict_time_no_millis||basic_time||basic_time_no_millis",
+    }
     json_schema = {"type": "string", "format": "time"}
 
 
 class DateTimeDataType(BaseDateDataType):
     model_type = "datetime"
 
     ui = {
@@ -59,15 +60,18 @@
         }
     }
     marshmallow = {
         "field-class": "ma_fields.String",
         "validators": ["validate_datetime"],
         "imports": [{"import": "oarepo_runtime.validation.validate_datetime"}],
     }
-    mapping = {"type": "date", "format": "strict_date_time||strict_date_time_no_millis||basic_date_time||basic_date_time_no_millis||basic_date||strict_date"}
+    mapping = {
+        "type": "date",
+        "format": "strict_date_time||strict_date_time_no_millis||basic_date_time||basic_date_time_no_millis||basic_date||strict_date",
+    }
     json_schema = {"type": "string", "format": "date-time"}
 
 
 class EDTFDataType(BaseDateDataType):
     model_type = "edtf"
 
     ui = {
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/model.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/model.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/primitive_types.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/primitive_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
         "facet_class": "TermsFacet",
         "imports": [
             {"import": "invenio_records_resources.services.records.facets.TermsFacet"}
         ],
     }
 
 
-
 class IntegerDataType(NumberDataType):
     model_type = "integer"
 
     ui = {
         "marshmallow": {
             "field-class": "ma_fields.Integer",
         }
@@ -90,8 +89,7 @@
     json_schema = {"type": "boolean"}
     facets = {
         "facet_class": "TermsFacet",
         "imports": [
             {"import": "invenio_records_resources.services.records.facets.TermsFacet"}
         ],
     }
-
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/datatypes/strings.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/datatypes/strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         "facet_class": "TermsFacet",
         "imports": [
             {"import": "invenio_records_resources.services.records.facets.TermsFacet"}
         ],
     }
 
 
-
 class UUIDDataType(StringDataType):
     model_type = "uuid"
     mapping = {"type": "keyword"}
 
 
 class FulltextKeywordDataType(StringDataType):
     model_type = "fulltext+keyword"
@@ -65,18 +64,16 @@
         # "path": "_keyword",
         "imports": [
             {"import": "invenio_records_resources.services.records.facets.TermsFacet"}
         ],
     }
 
 
-
 class URLDataType(StringDataType):
     model_type = "url"
     mapping = {"type": "keyword"}
     facets = {
         "facet_class": "TermsFacet",
         "imports": [
             {"import": "invenio_records_resources.services.records.facets.TermsFacet"}
         ],
     }
-
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/entrypoints.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/entrypoints.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/fs.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/fs.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/generate_doc.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/generate_doc.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/__init__.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_base.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_base.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_marshmallow.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_marshmallow.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_search.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_facets.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,33 @@
+from typing import List
+
 from oarepo_model_builder.datatypes import DataType
 
+from ..datatypes.components.facets import FacetDefinition
 from .invenio_base import InvenioBaseClassPythonBuilder
 
 
 class InvenioRecordSearchFacetsBuilder(InvenioBaseClassPythonBuilder):
-    TYPE = "invenio_record_search"
-    # class_config = "record-search-options-class"
+    TYPE = "invenio_record_facets"
     section = "facets"
     template = "record-facets"
 
     def build_node(self, node: DataType):
         # everything is done in finish
         pass
 
     def finish(self, **extra_kwargs):
-        facets = self.current_model.section_facets.config["facets"]
+        facets: List[FacetDefinition] = []
+        for node in self.current_model.deep_iter():
+            facets.extend(node.section_facets.config["facets"])
         package = self.current_model.definition["facets"]["module"]
-        search_options_data = []
 
         imports = []
         for f in facets:
-            search_options_data.append({f["path"]: f["class"]})
-            if "imports" in f:
-                for i in f["imports"]:
-                    imports.append((i["import"]).rsplit(".", 1))
-
-        imports = list(map(list, set(map(tuple, imports))))
-        imports.sort(key=lambda x: (x[0], x[1]))
+            imports.extend(f.imports)
 
         return super().finish(
             current_package_name=package,
-            search_options_data=search_options_data,
+            facets=facets,
             imports=imports,
             **extra_kwargs,
         )
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_search_options.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_search_options.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+from typing import List
+
+from ..datatypes.components.facets import FacetDefinition
 from .invenio_base import InvenioBaseClassPythonBuilder
 
 
 class InvenioRecordSearchOptionsBuilder(InvenioBaseClassPythonBuilder):
     TYPE = "invenio_record_search_options"
     section = "search-options"
     template = "record-search-options"
 
     def finish(self, **extra_kwargs):
-        facets = self.current_model.section_facets.config["facets"]
+        facets: List[FacetDefinition] = []
+        for node in self.current_model.deep_iter():
+            facets.extend(node.section_facets.config["facets"])
         search_data = []
         for f in facets:
-            search_data.append({f["path"]: "facets." + f["path"]})
+            search_data.append({f.path: "facets." + f.path})
         extra_kwargs["search_data"] = search_data
         super().finish(**extra_kwargs)
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_record_service_config.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_record_service_config.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/invenio_script_sample_data.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/invenio_script_sample_data.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/api_views.py.jinja2` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/api_views.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/app_views.py.jinja2` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/app_views.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/config.py.jinja2` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/config.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/ext.py.jinja2` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/ext.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/marshmallow.py.jinja2` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/marshmallow.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/permissions.py.jinja2` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/permissions.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/record.py.jinja2` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/record.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/resource_config.py.jinja2` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/resource_config.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/invenio/templates/service_config.py.jinja2` & `oarepo-model-builder-4.0.7/oarepo_model_builder/invenio/templates/service_config.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/loaders/__init__.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/merger.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/merger.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/cfg.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/diff.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/diff.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/json.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/json.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/json_stack.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/json_stack.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/python.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/python.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/text.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/text.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/toml.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/toml.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/outputs/yaml.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/outputs/yaml.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/profiles/record.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/profiles/record.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/schema.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/templates/__init__.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/utils/cst/call.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/utils/cst/call.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/utils/cst/collections.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/utils/cst/collections.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/utils/cst/common.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/utils/cst/common.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/utils/cst/indented_nodes.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/utils/cst/indented_nodes.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/utils/cst/mergers.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/utils/cst/mergers.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/utils/cst/simple_nodes.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/utils/cst/simple_nodes.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/utils/deepmerge.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/utils/deepmerge.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/utils/facet_helpers.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/utils/facet_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from .python_name import convert_name_to_python
 
 
+def flatten(list_of_lists):
+    return [x for l in list_of_lists for x in l]
+
+
 def facet_definition(obj):
     key = None
     field = None
     args = None
     path = None
     if "facets" in obj.definition:
         facets = obj.definition["facets"]
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/utils/jinja.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/utils/jinja.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,19 @@
     split_base_name,
     split_package_base_name,
     split_package_name,
 )
 
 
 def sorted_imports(imports):
-    imports = list(sorted(imports, key=lambda x: (x["import"], x.get("alias"))))
+    # make the entries unique
+    imports_dict = {(x["import"], x.get("alias")): x for x in imports}
+    imports = list(imports_dict.values())
+    # sort them
+    imports.sort(key=lambda x: (x["import"], x.get("alias")))
     return imports
 
 
 def to_import_dict(import_object):
     if isinstance(import_object, Import):
         return {"import": import_object.import_path, "alias": import_object.alias}
     return import_object
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/utils/properties.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/utils/properties.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/utils/python_name.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/utils/python_name.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/utils/verbose.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/utils/verbose.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/validation/__init__.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/validation/extensibility.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/validation/extensibility.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/validation/model_validation.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/validation/model_validation.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder/validation/utils.py` & `oarepo-model-builder-4.0.7/oarepo_model_builder/validation/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder.egg-info/PKG-INFO` & `oarepo-model-builder-4.0.7/oarepo_model_builder.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder
-Version: 4.0.6
+Version: 4.0.7
 Summary: A utility library that generates OARepo required data model files from a JSON specification file
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo model builder
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder.egg-info/SOURCES.txt` & `oarepo-model-builder-4.0.7/oarepo_model_builder.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -91,25 +91,25 @@
 oarepo_model_builder/invenio/invenio_base.py
 oarepo_model_builder/invenio/invenio_config.py
 oarepo_model_builder/invenio/invenio_ext.py
 oarepo_model_builder/invenio/invenio_ext_setup_cfg.py
 oarepo_model_builder/invenio/invenio_proxies.py
 oarepo_model_builder/invenio/invenio_record.py
 oarepo_model_builder/invenio/invenio_record_dumper.py
+oarepo_model_builder/invenio/invenio_record_facets.py
 oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py
 oarepo_model_builder/invenio/invenio_record_marshmallow.py
 oarepo_model_builder/invenio/invenio_record_metadata.py
 oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py
 oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py
 oarepo_model_builder/invenio/invenio_record_permissions.py
 oarepo_model_builder/invenio/invenio_record_pid_provider.py
 oarepo_model_builder/invenio/invenio_record_resource.py
 oarepo_model_builder/invenio/invenio_record_resource_config.py
 oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py
-oarepo_model_builder/invenio/invenio_record_search.py
 oarepo_model_builder/invenio/invenio_record_search_options.py
 oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py
 oarepo_model_builder/invenio/invenio_record_service.py
 oarepo_model_builder/invenio/invenio_record_service_config.py
 oarepo_model_builder/invenio/invenio_record_ui_marshmallow.py
 oarepo_model_builder/invenio/invenio_record_ui_serializer.py
 oarepo_model_builder/invenio/invenio_script_sample_data.py
```

### Comparing `oarepo-model-builder-4.0.6/oarepo_model_builder.egg-info/entry_points.txt` & `oarepo-model-builder-4.0.7/oarepo_model_builder.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 0100-python_structure = oarepo_model_builder.builders.python_structure:PythonStructureBuilder
 0105-invenio_record_pid_provider = oarepo_model_builder.invenio.invenio_record_pid_provider:InvenioRecordPIDProviderBuilder
 0110-invenio_record = oarepo_model_builder.invenio.invenio_record:InvenioRecordBuilder
 0120-invenio_record_metadata = oarepo_model_builder.invenio.invenio_record_metadata:InvenioRecordMetadataBuilder
 0130-invenio_record_marshmallow = oarepo_model_builder.invenio.invenio_record_marshmallow:InvenioRecordMarshmallowBuilder
 0140-invenio_record_ui_marshmallow = oarepo_model_builder.invenio.invenio_record_ui_marshmallow:InvenioRecordUIMarshmallowBuilder
 0200-invenio_record_permissions = oarepo_model_builder.invenio.invenio_record_permissions:InvenioRecordPermissionsBuilder
-0300-invenio_record_search_facets = oarepo_model_builder.invenio.invenio_record_search:InvenioRecordSearchFacetsBuilder
+0300-invenio_record_search_facets = oarepo_model_builder.invenio.invenio_record_facets:InvenioRecordSearchFacetsBuilder
 0305-invenio_record_search_options = oarepo_model_builder.invenio.invenio_record_search_options:InvenioRecordSearchOptionsBuilder
 0310-invenio_record_service_config = oarepo_model_builder.invenio.invenio_record_service_config:InvenioRecordServiceConfigBuilder
 0320-invenio_record_service = oarepo_model_builder.invenio.invenio_record_service:InvenioRecordServiceBuilder
 0340-invenio_record_dumper = oarepo_model_builder.invenio.invenio_record_dumper:InvenioRecordDumperBuilder
 0400-invenio_record_resource_config = oarepo_model_builder.invenio.invenio_record_resource_config:InvenioRecordResourceConfigBuilder
 0410-invenio_record_resource = oarepo_model_builder.invenio.invenio_record_resource:InvenioRecordResourceBuilder
 0420-invenio_api_views = oarepo_model_builder.invenio.invenio_api_views:InvenioAPIViewsBuilder
```

### Comparing `oarepo-model-builder-4.0.6/setup.cfg` & `oarepo-model-builder-4.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder
-version = 4.0.6
+version = 4.0.7
 description = A utility library that generates OARepo required data model files from a JSON specification file
 authors = Miroslav Bauer <bauer@cesnet.cz>, Miroslav Simek <simeki@vscht.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
@@ -101,15 +101,15 @@
 	0100-python_structure  = oarepo_model_builder.builders.python_structure:PythonStructureBuilder
 	0105-invenio_record_pid_provider = oarepo_model_builder.invenio.invenio_record_pid_provider:InvenioRecordPIDProviderBuilder
 	0110-invenio_record  = oarepo_model_builder.invenio.invenio_record:InvenioRecordBuilder
 	0120-invenio_record_metadata  = oarepo_model_builder.invenio.invenio_record_metadata:InvenioRecordMetadataBuilder
 	0130-invenio_record_marshmallow  = oarepo_model_builder.invenio.invenio_record_marshmallow:InvenioRecordMarshmallowBuilder
 	0140-invenio_record_ui_marshmallow  = oarepo_model_builder.invenio.invenio_record_ui_marshmallow:InvenioRecordUIMarshmallowBuilder
 	0200-invenio_record_permissions  = oarepo_model_builder.invenio.invenio_record_permissions:InvenioRecordPermissionsBuilder
-	0300-invenio_record_search_facets  = oarepo_model_builder.invenio.invenio_record_search:InvenioRecordSearchFacetsBuilder
+	0300-invenio_record_search_facets  = oarepo_model_builder.invenio.invenio_record_facets:InvenioRecordSearchFacetsBuilder
 	0305-invenio_record_search_options  = oarepo_model_builder.invenio.invenio_record_search_options:InvenioRecordSearchOptionsBuilder
 	
 	0310-invenio_record_service_config  = oarepo_model_builder.invenio.invenio_record_service_config:InvenioRecordServiceConfigBuilder
 	0320-invenio_record_service  = oarepo_model_builder.invenio.invenio_record_service:InvenioRecordServiceBuilder
 	0340-invenio_record_dumper  = oarepo_model_builder.invenio.invenio_record_dumper:InvenioRecordDumperBuilder
 	0400-invenio_record_resource_config  = oarepo_model_builder.invenio.invenio_record_resource_config:InvenioRecordResourceConfigBuilder
 	0410-invenio_record_resource  = oarepo_model_builder.invenio.invenio_record_resource:InvenioRecordResourceBuilder
```

### Comparing `oarepo-model-builder-4.0.6/tests/multilang.py` & `oarepo-model-builder-4.0.7/tests/multilang.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_builder_from_entrypoints.py` & `oarepo-model-builder-4.0.7/tests/test_builder_from_entrypoints.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_cfg_builders.py` & `oarepo-model-builder-4.0.7/tests/test_cfg_builders.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_datatype_prepare.py` & `oarepo-model-builder-4.0.7/tests/test_datatype_prepare.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_datatype_validator.py` & `oarepo-model-builder-4.0.7/tests/test_datatype_validator.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_dependencies.py` & `oarepo-model-builder-4.0.7/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_empty_metadata.py` & `oarepo-model-builder-4.0.7/tests/test_empty_metadata.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_extend.py` & `oarepo-model-builder-4.0.7/tests/test_extend.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_facets.py` & `oarepo-model-builder-4.0.7/tests/test_facets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
 import re
 
 from oarepo_model_builder.entrypoints import create_builder_from_entrypoints, load_model
 from oarepo_model_builder.fs import InMemoryFileSystem
+from tests.utils import strip_whitespaces
 
 DUMMY_YAML = "test.yaml"
 
 
 def test_include_invenio():
     schema = load_model(
         "test.yaml",
         model_content={
             "record": {
                 "use": "invenio",
-                "module" : {"qualified": "test"},
+                "module": {"qualified": "test"},
                 "properties": {
                     "jej": {
                         "type": "nested",
                         "properties": {
                             "c": {
                                 "type": "keyword",
                                 "facets": {"path": "cosi"},
@@ -45,17 +46,21 @@
         autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
     builder.build(schema, "record", ["record"], "")
 
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
+    data = (
+        builder.filesystem.open(
+            os.path.join("test", "services", "records", "facets.py")
+        )
+        .read()
+        .replace("'", '"')
+    )
     print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 \"""Facet definitions.\"""
 
@@ -71,15 +76,15 @@
 
 
 
 _schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
 
 
-a_keyword = TermsFacet(field="a.keyword", label=_("a/keyword.label") )
+a = TermsFacet(field="a", label=_("a.label") )
 
 
 
 b = TermsFacet(field="b.cosi", label =_("b.label"))
 
 
 
@@ -134,17 +139,21 @@
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
     builder.build(schema, "record", ["record"], "")
 
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
+    data = (
+        builder.filesystem.open(
+            os.path.join("test", "services", "records", "facets.py")
+        )
+        .read()
+        .replace("'", '"')
+    )
     print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 \"""Facet definitions.\"""
 
@@ -157,15 +166,15 @@
 
 _schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
 b_c = NestedLabeledFacet(path ="b", nested_facet = TermsFacet(field="b.c", label=_("b/c.label") ))
 
 
 
-b_d_keyword = NestedLabeledFacet(path ="b", nested_facet = TermsFacet(field="b.d.keyword", label=_("b/d/keyword.label") ))
+b_d = NestedLabeledFacet(path ="b", nested_facet = TermsFacet(field="b.d", label=_("b/d.label") ))
 
 
 
 b_f_g = NestedLabeledFacet(path ="b", nested_facet = NestedLabeledFacet(path ="b.f", nested_facet = TermsFacet(field="b.f.g", label=_("b/f/g.label") )))
 
 created = DateTimeFacet(field="created", label=_("created.label") )
 
@@ -220,17 +229,21 @@
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
     builder.build(schema, "record", ["record"], "")
 
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
+    data = (
+        builder.filesystem.open(
+            os.path.join("test", "services", "records", "facets.py")
+        )
+        .read()
+        .replace("'", '"')
+    )
     print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
         \"""Facet definitions.\"""
 
@@ -242,15 +255,15 @@
 
 _schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
 b_c = TermsFacet(field="b.c", label=_("b/c.label") )
 
 
 
-b_d_keyword = TermsFacet(field="b.d.keyword", label=_("b/d/keyword.label") )
+b_d = TermsFacet(field="b.d", label=_("b/d.label") )
 
 
 
 b_f_g = TermsFacet(field="b.f.g.cosi", label=_("b/f/g.label") )
 
 created = DateTimeFacet(field="created", label=_("created.label") )
 
@@ -314,17 +327,21 @@
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
     builder.build(schema, "record", ["record"], "")
 
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
+    data = (
+        builder.filesystem.open(
+            os.path.join("test", "services", "records", "facets.py")
+        )
+        .read()
+        .replace("'", '"')
+    )
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
         \"""Facet definitions.\"""
 
 from invenio_search.engine import dsl
@@ -337,27 +354,27 @@
 
 _schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
 b_nes_c = NestedLabeledFacet(path ="b_nes", nested_facet = TermsFacet(field="b_nes.c", label=_("b_nes/c.label") ))
 
 
 
-b_nes_d_keyword = NestedLabeledFacet(path ="b_nes", nested_facet = TermsFacet(field="b_nes.d.keyword", label=_("b_nes/d/keyword.label") ))
+b_nes_d = NestedLabeledFacet(path ="b_nes", nested_facet = TermsFacet(field="b_nes.d", label=_("b_nes/d.label") ))
 
 
 
 b_nes_f_g = NestedLabeledFacet(path ="b_nes", nested_facet = TermsFacet(field="b_nes.f.g", label=_("b_nes/f/g.label") ))
 
 
 
 b_obj_c = TermsFacet(field="b_obj.c", label=_("b_obj/c.label") )
 
 
 
-b_obj_d_keyword = TermsFacet(field="b_obj.d.keyword", label=_("b_obj/d/keyword.label") )
+b_obj_d = TermsFacet(field="b_obj.d", label=_("b_obj/d.label") )
 
 
 
 b_obj_f_g = NestedLabeledFacet(path ="b_obj.f", nested_facet = TermsFacet(field="b_obj.f.g", label=_("b_obj/f/g.label") ))
 
 
 
@@ -397,17 +414,21 @@
         autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
     builder.build(schema, "record", ["record"], "")
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
+    data = (
+        builder.filesystem.open(
+            os.path.join("test", "services", "records", "facets.py")
+        )
+        .read()
+        .replace("'", '"')
+    )
     print(data)
 
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
         \"""Facet definitions.\"""
@@ -420,15 +441,15 @@
 
 _schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
 a = TermsFacet(field="a", label=_("a.label") )
 
 
 
-c_keyword = TermsFacet(field="c.keyword", label=_("c/keyword.label") )
+c = TermsFacet(field="c", label=_("c.label") )
 
 
 
 
 
 
 
@@ -488,17 +509,21 @@
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
     builder.build(schema, "record", ["record"], "")
 
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
+    data = (
+        builder.filesystem.open(
+            os.path.join("test", "services", "records", "facets.py")
+        )
+        .read()
+        .replace("'", '"')
+    )
     print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
  \"""Facet definitions.\"""
 
@@ -572,17 +597,21 @@
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
     builder.build(schema, "record", ["record"], "")
 
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
+    data = (
+        builder.filesystem.open(
+            os.path.join("test", "services", "records", "facets.py")
+        )
+        .read()
+        .replace("'", '"')
+    )
     print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
         \"""Facet definitions.\"""
 
@@ -597,15 +626,15 @@
 
 
 
 created = DateTimeFacet(field="created", label=_("created.label") )
 
 _id = TermsFacet(field="id", label=_("id.label") )
 
-test = NestedLabeledFacet(path ="obj.arr", nested_facet = TermsFacet(field="obj.arr.d.keyword", label=_("obj/arr/d/keyword.label") ))
+test = NestedLabeledFacet(path ="obj.arr", nested_facet = TermsFacet(field="obj.arr.d", label=_("obj/arr/d.label") ))
 
 
 
 obj_arr_e_f = NestedLabeledFacet(path ="obj.arr", nested_facet = TermsFacet(field="obj.arr.e.f", label=_("obj/arr/e/f.label") ))
 
 updated = DateTimeFacet(field="updated", label=_("updated.label") )
 
@@ -655,17 +684,21 @@
         autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
     builder.build(schema, "record", ["record"], "")
 
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
+    data = (
+        builder.filesystem.open(
+            os.path.join("test", "services", "records", "facets.py")
+        )
+        .read()
+        .replace("'", '"')
+    )
     print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 \"""Facet definitions.\"""
 
@@ -745,36 +778,37 @@
         autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
     builder.build(schema, "record", ["record"], "")
 
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
-    print(data)
-    assert re.sub(r"\s", "", data) == re.sub(
-        r"\s",
-        "",
+    data = (
+        builder.filesystem.open(
+            os.path.join("test", "services", "records", "facets.py")
+        )
+        .read()
+        .replace("'", '"')
+    )
+    assert strip_whitespaces(data) == strip_whitespaces(
         """
 \"""Facet definitions.\"""
 
 from invenio_search.engine import dsl
 from flask_babelex import lazy_gettext as _
 
 from invenio_records_resources.services.records.facets import TermsFacet
 from oarepo_runtime.facets.date import DateTimeFacet
 from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
 
 
 _schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
 
-a_keyword = TermsFacet(field="a.keyword", label=_("a/keyword.label") )
+a = TermsFacet(field="a", label=_("a.label") )
 
 
 
 arr_d = NestedLabeledFacet(path ="arr", nested_facet = TermsFacet(field="arr.d", label=_("arr/d.label") ))
 
 
 
@@ -825,17 +859,21 @@
         black=False,
         autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
     builder.build(schema, "record", ["record"], "")
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
+    data = (
+        builder.filesystem.open(
+            os.path.join("test", "services", "records", "facets.py")
+        )
+        .read()
+        .replace("'", '"')
+    )
     print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 \"""Facet definitions.\"""
 
@@ -894,17 +932,21 @@
         autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
     builder.build(schema, "record", ["record"], "")
 
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
+    data = (
+        builder.filesystem.open(
+            os.path.join("test", "services", "records", "facets.py")
+        )
+        .read()
+        .replace("'", '"')
+    )
     print(data)
 
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 \"""Facet definitions.\"""
@@ -967,17 +1009,21 @@
         autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
     builder.build(schema, "record", ["record"], "")
 
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
+    data = (
+        builder.filesystem.open(
+            os.path.join("test", "services", "records", "facets.py")
+        )
+        .read()
+        .replace("'", '"')
+    )
     print(data)
 
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 \"""Facet definitions.\"""
@@ -1039,17 +1085,21 @@
         autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
     builder.build(schema, "record", ["record"], "")
 
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
+    data = (
+        builder.filesystem.open(
+            os.path.join("test", "services", "records", "facets.py")
+        )
+        .read()
+        .replace("'", '"')
+    )
     print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 \"""Facet definitions.\"""
```

### Comparing `oarepo-model-builder-4.0.6/tests/test_fulltext_keyword.py` & `oarepo-model-builder-4.0.7/tests/test_fulltext_keyword.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_jsonchema_builder.py` & `oarepo-model-builder-4.0.7/tests/test_jsonchema_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_loading.py` & `oarepo-model-builder-4.0.7/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_mapping_builder.py` & `oarepo-model-builder-4.0.7/tests/test_mapping_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_marshmallow_builder.py` & `oarepo-model-builder-4.0.7/tests/test_marshmallow_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_marshmallow_ui_builder.py` & `oarepo-model-builder-4.0.7/tests/test_marshmallow_ui_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_merge.py` & `oarepo-model-builder-4.0.7/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_model_saver.py` & `oarepo-model-builder-4.0.7/tests/test_model_saver.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_overwrite.py` & `oarepo-model-builder-4.0.7/tests/test_overwrite.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_pid_provider.py` & `oarepo-model-builder-4.0.7/tests/test_pid_provider.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_plugin_configuration.py` & `oarepo-model-builder-4.0.7/tests/test_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_python_mergers.py` & `oarepo-model-builder-4.0.7/tests/test_python_mergers.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_raw.py` & `oarepo-model-builder-4.0.7/tests/test_raw.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_sample_builder.py` & `oarepo-model-builder-4.0.7/tests/test_sample_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_schema_props.py` & `oarepo-model-builder-4.0.7/tests/test_schema_props.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_search_options.py` & `oarepo-model-builder-4.0.7/tests/test_search_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
-import re
 
 from oarepo_model_builder.entrypoints import create_builder_from_entrypoints, load_model
 from oarepo_model_builder.fs import InMemoryFileSystem
+from tests.utils import strip_whitespaces
 
 DUMMY_YAML = "test.yaml"
 
 
 # def test_sort():
 #     schema = load_model(
 #         DUMMY_YAML,
@@ -91,29 +91,27 @@
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
     builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "search.py")
     ).read()
-    assert re.sub(r"\s", "", data) == re.sub(
-        r"\s",
-        "",
+    assert strip_whitespaces(data) == strip_whitespaces(
         """
 from invenio_records_resources.services import SearchOptions as InvenioSearchOptions
 from flask_babelex import lazy_gettext as _
 from . import facets
 
 
 class TestSearchOptions(InvenioSearchOptions):
     \"""TestRecord search options.\"""
 
     facets = {
         '_schema': facets._schema,
-      'a_keyword': facets.a_keyword,
+      'a': facets.a,
       'b': facets.b,
       'created': facets.created,
       '_id': facets._id,
       'updated': facets.updated,
       
     }
     sort_options = {
```

### Comparing `oarepo-model-builder-4.0.6/tests/test_shortcuts.py` & `oarepo-model-builder-4.0.7/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_simple_builders.py` & `oarepo-model-builder-4.0.7/tests/test_simple_builders.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_type_shortcuts.py` & `oarepo-model-builder-4.0.7/tests/test_type_shortcuts.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/test_validation.py` & `oarepo-model-builder-4.0.7/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.6/tests/utils.py` & `oarepo-model-builder-4.0.7/tests/utils.py`

 * *Files identical despite different names*

