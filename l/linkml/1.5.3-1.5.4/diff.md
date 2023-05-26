# Comparing `tmp/linkml-1.5.3.tar.gz` & `tmp/linkml-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml-1.5.3.tar", max compression
+gzip compressed data, was "linkml-1.5.4.tar", max compression
```

## Comparing `linkml-1.5.3.tar` & `linkml-1.5.4.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     6555 2023-05-23 20:25:52.064652 linkml-1.5.3/LICENSE
--rw-r--r--   0        0        0     1369 2023-05-23 20:25:52.064652 linkml-1.5.3/README.md
--rw-r--r--   0        0        0     3227 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/__init__.py
--rw-r--r--   0        0        0      326 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/_version.py
--rw-r--r--   0        0        0    51005 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/PythonGenNotes.md
--rw-r--r--   0        0        0     4158 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/README.md
--rw-r--r--   0        0        0      616 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/common/__init__.py
--rw-r--r--   0        0        0     2040 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/common/type_designators.py
--rw-r--r--   0        0        0     3118 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/csvgen.py
--rw-r--r--   0        0        0     2873 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/docgen/class.md.jinja2
--rw-r--r--   0        0        0     2682 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/docgen/class_diagram.md.jinja2
--rw-r--r--   0        0        0     1321 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/docgen/common_metadata.md.jinja2
--rw-r--r--   0        0        0     1018 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/docgen/enum.md.jinja2
--rw-r--r--   0        0        0     1190 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/docgen/index.md.jinja2
--rw-r--r--   0        0        0      501 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/docgen/index.tex.jinja2
--rw-r--r--   0        0        0       70 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/docgen/schema.md.jinja2
--rw-r--r--   0        0        0     2557 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/docgen/slot.md.jinja2
--rw-r--r--   0        0        0     1704 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/docgen/subset.md.jinja2
--rw-r--r--   0        0        0      635 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/docgen/type.md.jinja2
--rw-r--r--   0        0        0    32663 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/docgen.py
--rw-r--r--   0        0        0     5112 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/dotgen.py
--rw-r--r--   0        0        0    10913 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/erdiagramgen.py
--rw-r--r--   0        0        0     6894 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/excelgen.py
--rw-r--r--   0        0        0     6393 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/golanggen.py
--rw-r--r--   0        0        0     3575 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/golrgen.py
--rw-r--r--   0        0        0     2347 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/graphqlgen.py
--rw-r--r--   0        0        0      444 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/javagen/example_template.java.jinja2
--rw-r--r--   0        0        0     1737 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/javagen/java_record_template.jinja2
--rw-r--r--   0        0        0     5499 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/javagen.py
--rw-r--r--   0        0        0     8821 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/jsonldcontextgen.py
--rw-r--r--   0        0        0     7952 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/jsonldgen.py
--rw-r--r--   0        0        0    21688 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/jsonschemagen.py
--rw-r--r--   0        0        0     3555 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/linkmlgen.py
--rw-r--r--   0        0        0    34422 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/markdowngen.py
--rw-r--r--   0        0        0     6532 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/namespacegen.py
--rw-r--r--   0        0        0     7831 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/oocodegen.py
--rw-r--r--   0        0        0    27365 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/owlgen.py
--rw-r--r--   0        0        0     4911 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/prefixmapgen.py
--rw-r--r--   0        0        0     9811 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/projectgen.py
--rw-r--r--   0        0        0     2443 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/protogen.py
--rw-r--r--   0        0        0    22150 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/pydanticgen.py
--rw-r--r--   0        0        0    50389 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/pythongen.py
--rw-r--r--   0        0        0     2825 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/rdfgen.py
--rw-r--r--   0        0        0     5621 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/shaclgen.py
--rw-r--r--   0        0        0     9547 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/shexgen.py
--rw-r--r--   0        0        0     6632 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/sparqlgen.py
--rw-r--r--   0        0        0      166 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2575 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py
--rw-r--r--   0        0        0     1625 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py
--rw-r--r--   0        0        0     9334 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/sqlalchemygen.py
--rw-r--r--   0        0        0    18626 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/sqlddlgen.py
--rw-r--r--   0        0        0    11387 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/sqltablegen.py
--rw-r--r--   0        0        0     7177 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/sssomgen.py
--rw-r--r--   0        0        0     1788 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/string_template.md
--rw-r--r--   0        0        0     3020 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/summarygen.py
--rw-r--r--   0        0        0     4760 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/terminusdbgen.py
--rw-r--r--   0        0        0     6094 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/typescriptgen.py
--rw-r--r--   0        0        0     1746 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/yamlgen.py
--rw-r--r--   0        0        0    13311 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/yumlgen.py
--rw-r--r--   0        0        0        0 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/__init__.py
--rw-r--r--   0        0        0     4323 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/cli.py
--rw-r--r--   0        0        0      292 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/config/datamodel/.linkmllint.yaml
--rw-r--r--   0        0        0        0 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/config/datamodel/__init__.py
--rw-r--r--   0        0        0    17711 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/config/datamodel/config.py
--rw-r--r--   0        0        0     6980 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/config/datamodel/config.yaml
--rw-r--r--   0        0        0      540 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/config/default.yaml
--rw-r--r--   0        0        0      198 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/config/recommended.yaml
--rw-r--r--   0        0        0      269 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/formatters/__init__.py
--rw-r--r--   0        0        0      518 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/formatters/formatter.py
--rw-r--r--   0        0        0      767 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/formatters/json_formatter.py
--rw-r--r--   0        0        0     2605 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/formatters/markdown_formatter.py
--rw-r--r--   0        0        0     2085 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/formatters/terminal_formatter.py
--rw-r--r--   0        0        0      871 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/formatters/tsv_formatter.py
--rw-r--r--   0        0        0     5004 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/linter.py
--rw-r--r--   0        0        0    11649 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/rules.py
--rw-r--r--   0        0        0       55 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/reporting/__init__.py
--rw-r--r--   0        0        0     9189 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/reporting/model.py
--rw-r--r--   0        0        0        0 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/transformers/__init__.py
--rw-r--r--   0        0        0    18594 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/transformers/relmodel_transformer.py
--rw-r--r--   0        0        0     5455 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/transformers/schema_renamer.py
--rw-r--r--   0        0        0        0 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/utils/__init__.py
--rw-r--r--   0        0        0     6463 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/utils/converter.py
--rw-r--r--   0        0        0     4384 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/datautils.py
--rw-r--r--   0        0        0      490 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/datavalidator.py
--rw-r--r--   0        0        0     6999 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/execute_tutorial.py
--rw-r--r--   0        0        0    39737 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/generator.py
--rw-r--r--   0        0        0      445 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/helpers.py
--rw-r--r--   0        0        0     5773 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/ifabsent_functions.py
--rw-r--r--   0        0        0     9498 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/mergeutils.py
--rw-r--r--   0        0        0     4560 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/rawloader.py
--rw-r--r--   0        0        0     9065 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/schema_builder.py
--rw-r--r--   0        0        0    13464 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/schema_fixer.py
--rw-r--r--   0        0        0    48537 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/schemaloader.py
--rw-r--r--   0        0        0    19733 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/schemasynopsis.py
--rw-r--r--   0        0        0    16297 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/sqlutils.py
--rw-r--r--   0        0        0     2395 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/typereferences.py
--rw-r--r--   0        0        0     1514 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/validation.py
--rw-r--r--   0        0        0      140 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/validators/__init__.py
--rw-r--r--   0        0        0     6255 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/validators/jsonschemavalidator.py
--rw-r--r--   0        0        0     4873 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/validators/sparqlvalidator.py
--rw-r--r--   0        0        0        0 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/workspaces/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/workspaces/datamodel/__init__.py
--rw-r--r--   0        0        0    15641 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/workspaces/datamodel/workspaces.py
--rw-r--r--   0        0        0     4233 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/workspaces/datamodel/workspaces.yaml
--rw-r--r--   0        0        0    11912 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/workspaces/example_runner.py
--rw-r--r--   0        0        0     4973 2023-05-23 20:26:21.032995 linkml-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     6700 1970-01-01 00:00:00.000000 linkml-1.5.3/setup.py
--rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 linkml-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     6555 2023-05-26 20:00:09.694554 linkml-1.5.4/LICENSE
+-rw-r--r--   0        0        0     1369 2023-05-26 20:00:09.694554 linkml-1.5.4/README.md
+-rw-r--r--   0        0        0     3227 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/__init__.py
+-rw-r--r--   0        0        0      326 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/_version.py
+-rw-r--r--   0        0        0    51005 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/PythonGenNotes.md
+-rw-r--r--   0        0        0     4158 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/README.md
+-rw-r--r--   0        0        0      616 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/common/__init__.py
+-rw-r--r--   0        0        0     2040 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/common/type_designators.py
+-rw-r--r--   0        0        0     3118 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/csvgen.py
+-rw-r--r--   0        0        0     2873 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/class.md.jinja2
+-rw-r--r--   0        0        0     2682 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/class_diagram.md.jinja2
+-rw-r--r--   0        0        0     1321 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/common_metadata.md.jinja2
+-rw-r--r--   0        0        0     1018 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/enum.md.jinja2
+-rw-r--r--   0        0        0     1466 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/index.md.jinja2
+-rw-r--r--   0        0        0      501 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/index.tex.jinja2
+-rw-r--r--   0        0        0       70 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/schema.md.jinja2
+-rw-r--r--   0        0        0     2557 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/slot.md.jinja2
+-rw-r--r--   0        0        0     1704 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/subset.md.jinja2
+-rw-r--r--   0        0        0      635 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/type.md.jinja2
+-rw-r--r--   0        0        0    32994 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen.py
+-rw-r--r--   0        0        0     5112 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/dotgen.py
+-rw-r--r--   0        0        0    10913 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/erdiagramgen.py
+-rw-r--r--   0        0        0     6894 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/excelgen.py
+-rw-r--r--   0        0        0     6393 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/golanggen.py
+-rw-r--r--   0        0        0     3575 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/golrgen.py
+-rw-r--r--   0        0        0     2347 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/graphqlgen.py
+-rw-r--r--   0        0        0      444 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/javagen/example_template.java.jinja2
+-rw-r--r--   0        0        0     1737 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/javagen/java_record_template.jinja2
+-rw-r--r--   0        0        0     5499 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/javagen.py
+-rw-r--r--   0        0        0     8821 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/jsonldcontextgen.py
+-rw-r--r--   0        0        0     7952 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/jsonldgen.py
+-rw-r--r--   0        0        0    21688 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/jsonschemagen.py
+-rw-r--r--   0        0        0     3555 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/linkmlgen.py
+-rw-r--r--   0        0        0    34422 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/markdowngen.py
+-rw-r--r--   0        0        0     6532 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/namespacegen.py
+-rw-r--r--   0        0        0     7831 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/oocodegen.py
+-rw-r--r--   0        0        0    27365 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/owlgen.py
+-rw-r--r--   0        0        0     4911 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/prefixmapgen.py
+-rw-r--r--   0        0        0     9811 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/projectgen.py
+-rw-r--r--   0        0        0     2443 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/protogen.py
+-rw-r--r--   0        0        0    22150 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/pydanticgen.py
+-rw-r--r--   0        0        0    50389 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/pythongen.py
+-rw-r--r--   0        0        0     2825 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/rdfgen.py
+-rw-r--r--   0        0        0     5621 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/shaclgen.py
+-rw-r--r--   0        0        0     9547 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/shexgen.py
+-rw-r--r--   0        0        0     6632 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/sparqlgen.py
+-rw-r--r--   0        0        0      166 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2575 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py
+-rw-r--r--   0        0        0     1625 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py
+-rw-r--r--   0        0        0     9334 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/sqlalchemygen.py
+-rw-r--r--   0        0        0    18626 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/sqlddlgen.py
+-rw-r--r--   0        0        0    11387 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/sqltablegen.py
+-rw-r--r--   0        0        0     7177 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/sssomgen.py
+-rw-r--r--   0        0        0     1788 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/string_template.md
+-rw-r--r--   0        0        0     3020 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/summarygen.py
+-rw-r--r--   0        0        0     4760 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/terminusdbgen.py
+-rw-r--r--   0        0        0     6094 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/typescriptgen.py
+-rw-r--r--   0        0        0     1746 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/yamlgen.py
+-rw-r--r--   0        0        0    13311 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/yumlgen.py
+-rw-r--r--   0        0        0        0 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/__init__.py
+-rw-r--r--   0        0        0     4323 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/cli.py
+-rw-r--r--   0        0        0      292 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/config/datamodel/.linkmllint.yaml
+-rw-r--r--   0        0        0        0 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/config/datamodel/__init__.py
+-rw-r--r--   0        0        0    17711 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/config/datamodel/config.py
+-rw-r--r--   0        0        0     6980 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/config/datamodel/config.yaml
+-rw-r--r--   0        0        0      540 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/config/default.yaml
+-rw-r--r--   0        0        0      198 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/config/recommended.yaml
+-rw-r--r--   0        0        0      269 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/formatters/__init__.py
+-rw-r--r--   0        0        0      518 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/formatters/formatter.py
+-rw-r--r--   0        0        0      767 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/formatters/json_formatter.py
+-rw-r--r--   0        0        0     2605 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/formatters/markdown_formatter.py
+-rw-r--r--   0        0        0     2085 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/formatters/terminal_formatter.py
+-rw-r--r--   0        0        0      871 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/formatters/tsv_formatter.py
+-rw-r--r--   0        0        0     5004 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/linter.py
+-rw-r--r--   0        0        0    11649 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/rules.py
+-rw-r--r--   0        0        0       55 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/reporting/__init__.py
+-rw-r--r--   0        0        0     9189 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/reporting/model.py
+-rw-r--r--   0        0        0        0 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/transformers/__init__.py
+-rw-r--r--   0        0        0    18594 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/transformers/relmodel_transformer.py
+-rw-r--r--   0        0        0     5455 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/transformers/schema_renamer.py
+-rw-r--r--   0        0        0        0 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/__init__.py
+-rw-r--r--   0        0        0     6463 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/converter.py
+-rw-r--r--   0        0        0     4384 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/datautils.py
+-rw-r--r--   0        0        0      490 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/datavalidator.py
+-rw-r--r--   0        0        0     6999 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/execute_tutorial.py
+-rw-r--r--   0        0        0    39737 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/generator.py
+-rw-r--r--   0        0        0      445 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/helpers.py
+-rw-r--r--   0        0        0     5773 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/ifabsent_functions.py
+-rw-r--r--   0        0        0     9498 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/mergeutils.py
+-rw-r--r--   0        0        0     4560 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/rawloader.py
+-rw-r--r--   0        0        0     9065 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/schema_builder.py
+-rw-r--r--   0        0        0    13464 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/schema_fixer.py
+-rw-r--r--   0        0        0    48537 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/schemaloader.py
+-rw-r--r--   0        0        0    19733 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/schemasynopsis.py
+-rw-r--r--   0        0        0    16297 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/sqlutils.py
+-rw-r--r--   0        0        0     2395 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/typereferences.py
+-rw-r--r--   0        0        0     1514 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/validation.py
+-rw-r--r--   0        0        0      140 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/validators/__init__.py
+-rw-r--r--   0        0        0     6255 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/validators/jsonschemavalidator.py
+-rw-r--r--   0        0        0     4873 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/validators/sparqlvalidator.py
+-rw-r--r--   0        0        0        0 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/workspaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 20:00:09.722554 linkml-1.5.4/linkml/workspaces/datamodel/__init__.py
+-rw-r--r--   0        0        0    15641 2023-05-26 20:00:09.722554 linkml-1.5.4/linkml/workspaces/datamodel/workspaces.py
+-rw-r--r--   0        0        0     4233 2023-05-26 20:00:09.722554 linkml-1.5.4/linkml/workspaces/datamodel/workspaces.yaml
+-rw-r--r--   0        0        0    11912 2023-05-26 20:00:09.722554 linkml-1.5.4/linkml/workspaces/example_runner.py
+-rw-r--r--   0        0        0     4973 2023-05-26 20:00:40.366927 linkml-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     6700 1970-01-01 00:00:00.000000 linkml-1.5.4/setup.py
+-rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 linkml-1.5.4/PKG-INFO
```

### Comparing `linkml-1.5.3/LICENSE` & `linkml-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/README.md` & `linkml-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/__init__.py` & `linkml-1.5.4/linkml/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/PythonGenNotes.md` & `linkml-1.5.4/linkml/generators/PythonGenNotes.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/README.md` & `linkml-1.5.4/linkml/generators/README.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/__init__.py` & `linkml-1.5.4/linkml/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/common/type_designators.py` & `linkml-1.5.4/linkml/generators/common/type_designators.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/csvgen.py` & `linkml-1.5.4/linkml/generators/csvgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/docgen/class.md.jinja2` & `linkml-1.5.4/linkml/generators/docgen/class.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/docgen/class_diagram.md.jinja2` & `linkml-1.5.4/linkml/generators/docgen/class_diagram.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/docgen/common_metadata.md.jinja2` & `linkml-1.5.4/linkml/generators/docgen/common_metadata.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/docgen/enum.md.jinja2` & `linkml-1.5.4/linkml/generators/docgen/enum.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/docgen/index.md.jinja2` & `linkml-1.5.4/linkml/generators/docgen/subset.md.jinja2`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,65 @@
-# {% if schema.title %}{{ schema.title }}{% else %}{{ schema.name }}{% endif %}
+# Subset: {{ gen.name(element) }}
 
-{{ schema.description }}
+{%- if header -%}
+{{header}}
+{%- endif -%}
+
+{% if element.description %}
+{% set element_description_lines = element.description.split('\n') %}
+{% for element_description_line in element_description_lines %}
+_{{ element_description_line }}_
+{% endfor %}
+{% endif %}
 
-URI: {{ schema.id }}
-Name: {{ schema.name }}
+URI: {{ gen.uri_link(element) }}
 
-{% if include_top_level_diagram %}
 
-## Schema Diagram
+{% include "common_metadata.md.jinja2" %}
 
-```{{ gen.mermaid_directive() }}
-{{ gen.mermaid_diagram() }}
-```
-{% endif %}
-
-## Classes
+## Classes in subset
 
 | Class | Description |
 | --- | --- |
 {% for c in gen.all_class_objects()|sort(attribute=sort_by) -%}
+{%- if element.name in c.in_subset -%}
 | {{gen.link(c)}} | {{c.description|enshorten}} |
+{% endif -%}
+{% endfor %}
+
+{% for c in gen.all_class_objects()|sort(attribute=sort_by) -%}
+{%- if element.name in c.in_subset -%}
+### {{ gen.name(c) }}
+
+{{c.description}}
+
+| Name | Cardinality and Range  | Description  |
+| ---  | ---  | --- |
+{% for s in gen.class_induced_slots(c.name)|sort(attribute=sort_by) -%}
+{% if element.name in s.in_subset or element.name in schemaview.get_slot(s.name).in_subset -%}
+| {{gen.link(s)}} | {{ gen.cardinality(s) }} <br/> {{gen.link(s.range)}}  | {{s.description|enshorten}} {% if s.identifier %}**identifier**{% endif %}  |
+{% endif -%}
 {% endfor %}
 
-## Slots
+{% endif -%}
+{% endfor %}
+
+## Slots in subset
 
 | Slot | Description |
 | --- | --- |
 {% for s in gen.all_slot_objects()|sort(attribute=sort_by) -%}
+{%- if element.name in s.in_subset -%}
 | {{gen.link(s)}} | {{s.description|enshorten}} |
+{% endif -%}
 {% endfor %}
 
-## Enumerations
+## Enumerations in subset
 
 | Enumeration | Description |
 | --- | --- |
-{% for e in gen.all_enum_objects()|sort(attribute=sort_by) -%}
+{% for e in schemaview.all_enums().values()|sort(attribute='name') -%}
+{%- if element.name in e.in_subset -%}
 | {{gen.link(e)}} | {{e.description|enshorten}} |
+{% endif -%}
 {% endfor %}
 
-## Types
-
-| Type | Description |
-| --- | --- |
-{% for t in gen.all_type_objects()|sort(attribute=sort_by) -%}
-| {{gen.link(t)}} | {{t.description|enshorten}} |
-{% endfor %}
-
-## Subsets
-
-| Subset | Description |
-| --- | --- |
-{% for ss in schemaview.all_subsets().values()|sort(attribute='name') -%}
-| {{gen.link(ss)}} | {{ss.description|enshorten}} |
-{% endfor %}
```

### Comparing `linkml-1.5.3/linkml/generators/docgen/slot.md.jinja2` & `linkml-1.5.4/linkml/generators/docgen/slot.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/docgen/type.md.jinja2` & `linkml-1.5.4/linkml/generators/docgen/type.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/docgen.py` & `linkml-1.5.4/linkml/generators/docgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
     example_runner: ExampleRunner = field(default_factory=lambda: ExampleRunner())
 
     genmeta: bool = field(default_factory=lambda: False)
     gen_classvars: bool = field(default_factory=lambda: True)
     gen_slots: bool = field(default_factory=lambda: True)
     no_types_dir: bool = field(default_factory=lambda: False)
     use_slot_uris: bool = field(default_factory=lambda: False)
+    hierarchical_class_view: bool = field(default_factory=lambda: False)
 
 
     def __post_init__(self):
         dialect = self.dialect
         if dialect is not None:
             # TODO: simplify this
             if isinstance(dialect, str):
@@ -879,20 +880,25 @@
 @click.option("--template-directory", help="Folder in which custom templates are kept")
 @click.option(
     "--use-slot-uris/--no-use-slot-uris",
     default=False,
     help="Use IDs from slot_uri instead of names",
 )
 @click.option(
+    "--hierarchical-class-view/--no-hierarchical-class-view",
+    default=True,
+    help="Render class table on index page in a hierarchically indented view",
+)
+@click.option(
     "--example-directory",
     help="Folder in which example files are found. These are used to make inline examples"
 )
 @click.version_option(__version__, "-V", "--version")
 @click.command()
-def cli(yamlfile, directory, dialect, template_directory, use_slot_uris, **args):
+def cli(yamlfile, directory, dialect, template_directory, use_slot_uris, hierarchical_class_view, **args):
     """Generate documentation folder from a LinkML YAML schema
 
     Currently a default set of templates for markdown is provided (see the folder linkml/generators/docgen/)
 
     If you specify another format (e.g. html) then you need to provide a template_directory argument, with a template for
     each type of entity inside.
 
@@ -908,14 +914,15 @@
     """
     gen = DocGenerator(
         yamlfile,
         directory=directory,
         dialect=dialect,
         template_directory=template_directory,
         use_slot_uris=use_slot_uris,
+        hierarchical_class_view=hierarchical_class_view,
         **args,
     )
     print(gen.serialize())
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `linkml-1.5.3/linkml/generators/dotgen.py` & `linkml-1.5.4/linkml/generators/dotgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/erdiagramgen.py` & `linkml-1.5.4/linkml/generators/erdiagramgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/excelgen.py` & `linkml-1.5.4/linkml/generators/excelgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/golanggen.py` & `linkml-1.5.4/linkml/generators/golanggen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/golrgen.py` & `linkml-1.5.4/linkml/generators/golrgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/graphqlgen.py` & `linkml-1.5.4/linkml/generators/graphqlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/javagen/java_record_template.jinja2` & `linkml-1.5.4/linkml/generators/javagen/java_record_template.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/javagen.py` & `linkml-1.5.4/linkml/generators/javagen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/jsonldcontextgen.py` & `linkml-1.5.4/linkml/generators/jsonldcontextgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/jsonldgen.py` & `linkml-1.5.4/linkml/generators/jsonldgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/jsonschemagen.py` & `linkml-1.5.4/linkml/generators/jsonschemagen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/linkmlgen.py` & `linkml-1.5.4/linkml/generators/linkmlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/markdowngen.py` & `linkml-1.5.4/linkml/generators/markdowngen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/namespacegen.py` & `linkml-1.5.4/linkml/generators/namespacegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/oocodegen.py` & `linkml-1.5.4/linkml/generators/oocodegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/owlgen.py` & `linkml-1.5.4/linkml/generators/owlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/prefixmapgen.py` & `linkml-1.5.4/linkml/generators/prefixmapgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/projectgen.py` & `linkml-1.5.4/linkml/generators/projectgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/protogen.py` & `linkml-1.5.4/linkml/generators/protogen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/pydanticgen.py` & `linkml-1.5.4/linkml/generators/pydanticgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/pythongen.py` & `linkml-1.5.4/linkml/generators/pythongen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/rdfgen.py` & `linkml-1.5.4/linkml/generators/rdfgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/shaclgen.py` & `linkml-1.5.4/linkml/generators/shaclgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/shexgen.py` & `linkml-1.5.4/linkml/generators/shexgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/sparqlgen.py` & `linkml-1.5.4/linkml/generators/sparqlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py` & `linkml-1.5.4/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py` & `linkml-1.5.4/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/sqlalchemygen.py` & `linkml-1.5.4/linkml/generators/sqlalchemygen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/sqlddlgen.py` & `linkml-1.5.4/linkml/generators/sqlddlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/sqltablegen.py` & `linkml-1.5.4/linkml/generators/sqltablegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/sssomgen.py` & `linkml-1.5.4/linkml/generators/sssomgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/string_template.md` & `linkml-1.5.4/linkml/generators/string_template.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/summarygen.py` & `linkml-1.5.4/linkml/generators/summarygen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/terminusdbgen.py` & `linkml-1.5.4/linkml/generators/terminusdbgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/typescriptgen.py` & `linkml-1.5.4/linkml/generators/typescriptgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/yamlgen.py` & `linkml-1.5.4/linkml/generators/yamlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/generators/yumlgen.py` & `linkml-1.5.4/linkml/generators/yumlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/linter/cli.py` & `linkml-1.5.4/linkml/linter/cli.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/linter/config/datamodel/config.py` & `linkml-1.5.4/linkml/linter/config/datamodel/config.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/linter/config/datamodel/config.yaml` & `linkml-1.5.4/linkml/linter/config/datamodel/config.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/linter/config/default.yaml` & `linkml-1.5.4/linkml/linter/config/default.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/linter/formatters/formatter.py` & `linkml-1.5.4/linkml/linter/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/linter/formatters/json_formatter.py` & `linkml-1.5.4/linkml/linter/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/linter/formatters/markdown_formatter.py` & `linkml-1.5.4/linkml/linter/formatters/markdown_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/linter/formatters/terminal_formatter.py` & `linkml-1.5.4/linkml/linter/formatters/terminal_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/linter/formatters/tsv_formatter.py` & `linkml-1.5.4/linkml/linter/formatters/tsv_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/linter/linter.py` & `linkml-1.5.4/linkml/linter/linter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/linter/rules.py` & `linkml-1.5.4/linkml/linter/rules.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/reporting/model.py` & `linkml-1.5.4/linkml/reporting/model.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/transformers/relmodel_transformer.py` & `linkml-1.5.4/linkml/transformers/relmodel_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/transformers/schema_renamer.py` & `linkml-1.5.4/linkml/transformers/schema_renamer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/utils/converter.py` & `linkml-1.5.4/linkml/utils/converter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/utils/datautils.py` & `linkml-1.5.4/linkml/utils/datautils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/utils/execute_tutorial.py` & `linkml-1.5.4/linkml/utils/execute_tutorial.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/utils/generator.py` & `linkml-1.5.4/linkml/utils/generator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/utils/ifabsent_functions.py` & `linkml-1.5.4/linkml/utils/ifabsent_functions.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/utils/mergeutils.py` & `linkml-1.5.4/linkml/utils/mergeutils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/utils/rawloader.py` & `linkml-1.5.4/linkml/utils/rawloader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/utils/schema_builder.py` & `linkml-1.5.4/linkml/utils/schema_builder.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/utils/schema_fixer.py` & `linkml-1.5.4/linkml/utils/schema_fixer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/utils/schemaloader.py` & `linkml-1.5.4/linkml/utils/schemaloader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/utils/schemasynopsis.py` & `linkml-1.5.4/linkml/utils/schemasynopsis.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/utils/sqlutils.py` & `linkml-1.5.4/linkml/utils/sqlutils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/utils/typereferences.py` & `linkml-1.5.4/linkml/utils/typereferences.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/utils/validation.py` & `linkml-1.5.4/linkml/utils/validation.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/validators/jsonschemavalidator.py` & `linkml-1.5.4/linkml/validators/jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/validators/sparqlvalidator.py` & `linkml-1.5.4/linkml/validators/sparqlvalidator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/workspaces/datamodel/workspaces.py` & `linkml-1.5.4/linkml/workspaces/datamodel/workspaces.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/workspaces/datamodel/workspaces.yaml` & `linkml-1.5.4/linkml/workspaces/datamodel/workspaces.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/linkml/workspaces/example_runner.py` & `linkml-1.5.4/linkml/workspaces/example_runner.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.3/pyproject.toml` & `linkml-1.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml"
-version = "1.5.3"
+version = "1.5.4"
 description = "Linked Open Data Modeling Language"
 authors = [
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harold Solbrig <solbrig@jhu.edu>",
     "Sujay Patil <spatil@lbl.gov>",
     "Harshad Hegde <hhegde@lbl.gov>",
     "Sierra Moxon <smoxon@lbl.gov>",
```

### Comparing `linkml-1.5.3/setup.py` & `linkml-1.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
                      'linkml-sqldb = linkml.utils.sqlutils:main',
                      'linkml-validate = '
                      'linkml.validators.jsonschemavalidator:cli',
                      'run-tutorial = linkml.utils.execute_tutorial:cli']}
 
 setup_kwargs = {
     'name': 'linkml',
-    'version': '1.5.3',
+    'version': '1.5.4',
     'description': 'Linked Open Data Modeling Language',
     'long_description': '[![Pyversions](https://img.shields.io/pypi/pyversions/linkml.svg)](https://pypi.python.org/pypi/linkml)\n![](https://github.com/linkml/linkml/workflows/Build/badge.svg)\n[![PyPi](https://img.shields.io/pypi/v/linkml.svg)](https://pypi.python.org/pypi/linkml)\n[![badge](https://img.shields.io/badge/launch-binder-579ACA.svg)](https://mybinder.org/v2/gh/linkml/linkml/main?filepath=notebooks)\n[![DOI](https://zenodo.org/badge/13996/linkml/linkml.svg)](https://zenodo.org/badge/latestdoi/13996/linkml/linkml)\n[![PyPIDownloadsTotal](https://pepy.tech/badge/linkml)](https://pepy.tech/project/linkml)\n[![PyPIDownloadsMonth](https://img.shields.io/pypi/dm/linkml?logo=PyPI&color=blue)](https://pypi.org/project/linkml)\n[![codecov](https://codecov.io/gh/linkml/linkml/branch/main/graph/badge.svg?token=WNQNG986UN)](https://codecov.io/gh/linkml/linkml)\n\n\n# LinkML - Linked Data Modeling Language\n\nLinkML is a linked data modeling language following object-oriented and ontological principles. LinkML models are typically authored in YAML, and can be converted to other schema representation formats such as JSON or RDF.\n\nThis repo holds the tools for generating and working with LinkML. For the LinkML schema (metamodel), please see https://github.com/linkml/linkml-model\n\nThe complete documentation for LinkML can be found here:\n\n - [linkml.io/linkml](https://linkml.io/linkml)\n',
     'author': 'Chris Mungall',
     'author_email': 'cjmungall@lbl.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://linkml.io/linkml/',
```

### Comparing `linkml-1.5.3/PKG-INFO` & `linkml-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml
-Version: 1.5.3
+Version: 1.5.4
 Summary: Linked Open Data Modeling Language
 Home-page: https://linkml.io/linkml/
 Keywords: schema,linked data,data modeling,rdf,owl,biolink
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.7.6,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

