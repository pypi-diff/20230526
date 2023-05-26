# Comparing `tmp/policyuniverse-1.5.1.20230523.tar.gz` & `tmp/policyuniverse-1.5.1.20230526.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "policyuniverse-1.5.1.20230523.tar", last modified: Tue May 23 17:55:07 2023, max compression
+gzip compressed data, was "policyuniverse-1.5.1.20230526.tar", last modified: Fri May 26 15:39:15 2023, max compression
```

## Comparing `policyuniverse-1.5.1.20230523.tar` & `policyuniverse-1.5.1.20230526.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:07.906948 policyuniverse-1.5.1.20230523/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 17:54:52.000000 policyuniverse-1.5.1.20230523/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 17:54:52.000000 policyuniverse-1.5.1.20230523/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-05-23 17:55:07.906948 policyuniverse-1.5.1.20230523/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-23 17:54:52.000000 policyuniverse-1.5.1.20230523/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:07.906948 policyuniverse-1.5.1.20230523/policyuniverse/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-23 17:54:52.000000 policyuniverse-1.5.1.20230523/policyuniverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-23 17:54:52.000000 policyuniverse-1.5.1.20230523/policyuniverse/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-23 17:54:52.000000 policyuniverse-1.5.1.20230523/policyuniverse/action_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-23 17:54:52.000000 policyuniverse-1.5.1.20230523/policyuniverse/arn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-23 17:54:52.000000 policyuniverse-1.5.1.20230523/policyuniverse/common.py
--rw-r--r--   0 runner    (1001) docker     (123)  7768930 2023-05-23 17:54:52.000000 policyuniverse-1.5.1.20230523/policyuniverse/data.json
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-23 17:54:52.000000 policyuniverse-1.5.1.20230523/policyuniverse/expander_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-23 17:54:52.000000 policyuniverse-1.5.1.20230523/policyuniverse/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-23 17:54:52.000000 policyuniverse-1.5.1.20230523/policyuniverse/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-05-23 17:54:52.000000 policyuniverse-1.5.1.20230523/policyuniverse/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:07.906948 policyuniverse-1.5.1.20230523/policyuniverse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-05-23 17:55:07.000000 policyuniverse-1.5.1.20230523/policyuniverse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-23 17:55:07.000000 policyuniverse-1.5.1.20230523/policyuniverse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:55:07.000000 policyuniverse-1.5.1.20230523/policyuniverse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:55:07.000000 policyuniverse-1.5.1.20230523/policyuniverse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-23 17:55:07.000000 policyuniverse-1.5.1.20230523/policyuniverse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 17:55:07.000000 policyuniverse-1.5.1.20230523/policyuniverse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-23 17:55:07.906948 policyuniverse-1.5.1.20230523/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-23 17:54:52.000000 policyuniverse-1.5.1.20230523/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:39:15.496235 policyuniverse-1.5.1.20230526/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-05-26 15:39:15.496235 policyuniverse-1.5.1.20230526/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:39:15.496235 policyuniverse-1.5.1.20230526/policyuniverse/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/action_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/arn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7791087 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/expander_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/policyuniverse/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:39:15.496235 policyuniverse-1.5.1.20230526/policyuniverse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-05-26 15:39:15.000000 policyuniverse-1.5.1.20230526/policyuniverse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-26 15:39:15.000000 policyuniverse-1.5.1.20230526/policyuniverse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:39:15.000000 policyuniverse-1.5.1.20230526/policyuniverse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:39:15.000000 policyuniverse-1.5.1.20230526/policyuniverse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-26 15:39:15.000000 policyuniverse-1.5.1.20230526/policyuniverse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 15:39:15.000000 policyuniverse-1.5.1.20230526/policyuniverse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-26 15:39:15.496235 policyuniverse-1.5.1.20230526/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-26 15:39:02.000000 policyuniverse-1.5.1.20230526/setup.py
```

### Comparing `policyuniverse-1.5.1.20230523/LICENSE` & `policyuniverse-1.5.1.20230526/LICENSE`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230523/PKG-INFO` & `policyuniverse-1.5.1.20230526/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyuniverse
-Version: 1.5.1.20230523
+Version: 1.5.1.20230526
 Summary: Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.
 Home-page: https://github.com/Netflix-Skunkworks/policyuniverse
 Author: Patrick Kelley
 Author-email: patrickbarrettkelley@gmail.com
 Keywords: iam,arn,action_groups,condition,policy,statement,wildcard
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
```

### Comparing `policyuniverse-1.5.1.20230523/README.md` & `policyuniverse-1.5.1.20230526/README.md`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230523/policyuniverse/__init__.py` & `policyuniverse-1.5.1.20230526/policyuniverse/__init__.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230523/policyuniverse/action.py` & `policyuniverse-1.5.1.20230526/policyuniverse/action.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230523/policyuniverse/action_categories.py` & `policyuniverse-1.5.1.20230526/policyuniverse/action_categories.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230523/policyuniverse/arn.py` & `policyuniverse-1.5.1.20230526/policyuniverse/arn.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230523/policyuniverse/common.py` & `policyuniverse-1.5.1.20230526/policyuniverse/common.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230523/policyuniverse/data.json` & `policyuniverse-1.5.1.20230526/policyuniverse/data.json`

 * *Files 0% similar despite different names*

```diff
@@ -8828,14 +8828,40 @@
         "description": "Grants permission to attach a GraphQL API to a custom domain name in AppSync",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_AssociateApi.html"
         }
       },
+      "AssociateMergedGraphqlApi": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to associate a merged API to a source API",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_AssociateMergedGraphqlApi.html"
+        }
+      },
+      "AssociateSourceGraphqlApi": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to associate a source API to a merged API",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_AssociateSourceGraphqlApi.html"
+        }
+      },
       "CreateApiCache": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create an API cache in AppSync",
@@ -9029,14 +9055,27 @@
         "description": "Grants permission to delete a resolver",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_DeleteResolver.html"
         }
       },
+      "DeleteResourcePolicy": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to remove a resource policy",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${ConceptsDocRoot}merge-api.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/devguide/merge-api.html"
+        }
+      },
       "DeleteType": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete a type",
@@ -9055,32 +9094,58 @@
         "description": "Grants permission to detach a GraphQL API to a custom domain name in AppSync",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_DisassociateApi.html"
         }
       },
+      "DisassociateMergedGraphqlApi": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to remove an associated source API from a merged API identified by the source API",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_DisassociateMergedGraphqlApi.html"
+        }
+      },
+      "DisassociateSourceGraphqlApi": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to remove an associated source API from a merged API identified by the merged API",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_DisassociateSourceGraphqlApi.html"
+        }
+      },
       "EvaluateCode": {
         "aws_action_groups": [
-          "ReadWrite",
-          "ReadOnly"
+          "ReadOnly",
+          "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to evaluate code with a runtime and context",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_EvaluateCode.html"
         }
       },
       "EvaluateMappingTemplate": {
         "aws_action_groups": [
-          "ReadWrite",
-          "ReadOnly"
+          "ReadOnly",
+          "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to evaluate template mapping",
         "docs": {
           "api_doc": "",
           "doc_page": "",
@@ -9126,16 +9191,16 @@
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_GetApiCache.html"
         }
       },
       "GetDataSource": {
         "aws_action_groups": [
-          "ReadWrite",
-          "ReadOnly"
+          "ReadOnly",
+          "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve a data source",
         "docs": {
           "api_doc": "",
           "doc_page": "",
@@ -9154,88 +9219,116 @@
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_GetDomainName.html"
         }
       },
       "GetFunction": {
         "aws_action_groups": [
-          "ReadWrite",
-          "ReadOnly"
+          "ReadOnly",
+          "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve a function",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_GetFunction.html"
         }
       },
       "GetGraphqlApi": {
         "aws_action_groups": [
-          "ReadWrite",
-          "ReadOnly"
+          "ReadOnly",
+          "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}"
         ],
         "description": "Grants permission to retrieve a GraphQL API",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_GetGraphqlApi.html"
         }
       },
       "GetIntrospectionSchema": {
         "aws_action_groups": [
-          "ReadWrite",
-          "ReadOnly"
+          "ReadOnly",
+          "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve the introspection schema for a GraphQL API",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_GetIntrospectionSchema.html"
         }
       },
       "GetResolver": {
         "aws_action_groups": [
-          "ReadWrite",
-          "ReadOnly"
+          "ReadOnly",
+          "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve a resolver",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_GetResolver.html"
         }
       },
+      "GetResourcePolicy": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to read a resource policy",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${ConceptsDocRoot}merge-api.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/devguide/merge-api.html"
+        }
+      },
       "GetSchemaCreationStatus": {
         "aws_action_groups": [
-          "ReadWrite",
-          "ReadOnly"
+          "ReadOnly",
+          "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve the current status of a schema creation operation",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_GetSchemaCreationStatus.html"
         }
       },
+      "GetSourceApiAssociation": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to read information about a merged API associated source API",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_GetSourceApiAssociation.html"
+        }
+      },
       "GetType": {
         "aws_action_groups": [
-          "ReadWrite",
-          "ReadOnly"
+          "ReadOnly",
+          "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve a type",
         "docs": {
           "api_doc": "",
           "doc_page": "",
@@ -9253,32 +9346,32 @@
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}using-your-api.html",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/devguide/using-your-api.html"
         }
       },
       "ListApiKeys": {
         "aws_action_groups": [
-          "ReadWrite",
+          "ListOnly",
           "ReadOnly",
-          "ListOnly"
+          "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list the API keys for a given API",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_ListApiKeys.html"
         }
       },
       "ListDataSources": {
         "aws_action_groups": [
-          "ReadWrite",
+          "ListOnly",
           "ReadOnly",
-          "ListOnly"
+          "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list the data sources for a given API",
         "docs": {
           "api_doc": "",
           "doc_page": "",
@@ -9298,72 +9391,87 @@
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_ListDomainNames.html"
         }
       },
       "ListFunctions": {
         "aws_action_groups": [
-          "ReadWrite",
+          "ListOnly",
           "ReadOnly",
-          "ListOnly"
+          "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list the functions for a given API",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_ListFunctions.html"
         }
       },
       "ListGraphqlApis": {
         "aws_action_groups": [
-          "ReadWrite",
+          "ListOnly",
           "ReadOnly",
-          "ListOnly"
+          "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list GraphQL APIs",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_ListGraphqlApis.html"
         }
       },
       "ListResolvers": {
         "aws_action_groups": [
-          "ReadWrite",
+          "ListOnly",
           "ReadOnly",
-          "ListOnly"
+          "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list the resolvers for a given API and type",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_ListResolvers.html"
         }
       },
       "ListResolversByFunction": {
         "aws_action_groups": [
-          "ReadWrite",
+          "ListOnly",
           "ReadOnly",
-          "ListOnly"
+          "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list the resolvers that are associated with a specific function",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_ListResolversByFunction.html"
         }
       },
+      "ListSourceApiAssociations": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list source APIs associated to a given merged API",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_ListSourceApiAssociations.html"
+        }
+      },
       "ListTagsForResource": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [
@@ -9374,53 +9482,107 @@
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_ListTagsForResource.html"
         }
       },
       "ListTypes": {
         "aws_action_groups": [
-          "ReadWrite",
+          "ListOnly",
           "ReadOnly",
-          "ListOnly"
+          "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list the types for a given API",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_ListTypes.html"
         }
       },
+      "ListTypesByAssociation": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list the types for a given merged API and source API association",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_ListTypesByAssociation.html"
+        }
+      },
+      "PutResourcePolicy": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to set a resource policy",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${ConceptsDocRoot}merge-api.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/devguide/merge-api.html"
+        }
+      },
       "SetWebACL": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to set a web ACL",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_SetWebACL.html"
         }
       },
+      "SourceGraphQL": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to send a GraphQL query to a source API of a merged API",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${ConceptsDocRoot}using-your-api.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/devguide/using-your-api.html"
+        }
+      },
       "StartSchemaCreation": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to add a new schema to your GraphQL API. This operation is asynchronous - GetSchemaCreationStatus can show when it has completed",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_StartSchemaCreation.html"
         }
       },
+      "StartSchemaMerge": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to initiate a schema merge for a given merged API and associated source API",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_StartSchemaMerge.html"
+        }
+      },
       "TagResource": {
         "aws_action_groups": [
           "Tagging",
           "ReadWrite"
         ],
         "calculated_action_group": "Tagging",
         "condition_keys": [
@@ -9540,14 +9702,27 @@
         "description": "Grants permission to update a resolver",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_UpdateResolver.html"
         }
       },
+      "UpdateSourceApiAssociation": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update a merged API source API association",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appsync/latest/APIReference/API_UpdateSourceApiAssociation.html"
+        }
+      },
       "UpdateType": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update a type",
@@ -34740,14 +34915,28 @@
         "description": "Grants permission to delete all the scans and related findings from CodeGuru Security by given category",
         "docs": {
           "api_doc": "",
           "doc_page": "${APIReferenceDocPage}",
           "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
         }
       },
+      "GetAccountConfiguration": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve the account level configurations",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${APIReferenceDocPage}",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+        }
+      },
       "GetFindings": {
         "aws_action_groups": [
           "ReadOnly",
           "ListOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
@@ -99756,14 +99945,40 @@
         "description": "Grants permission to list trust anchors",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_ListTrustAnchors.html"
         }
       },
+      "PutNotificationSettings": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to attach notification settings to a trust anchor",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_PutNotificationSettings.html"
+        }
+      },
+      "ResetNotificationSettings": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to reset custom notification settings to IAM Roles Anywhere defined default state",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_ResetNotificationSettings.html"
+        }
+      },
       "TagResource": {
         "aws_action_groups": [
           "ReadWrite",
           "Tagging"
         ],
         "calculated_action_group": "Tagging",
         "condition_keys": [
@@ -100970,15 +101185,15 @@
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/singlesignon/latest/IdentityStoreAPIReference/API_UpdateUser.html"
         }
       }
     },
-    "arn_format": "arn:${Partition}:identitystore::${AwsAccountId}:${ResourceType}/${ResourceId}",
+    "arn_format": "arn:${Partition}:identitystore::${Account}:${ResourceType}/${ResourceId}",
     "arn_regex": "^arn:${Partition}:identitystore:.+",
     "description": "AWS Identity Store",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/singlesignon/latest/IdentityStoreAPIReference/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/singlesignon/latest/IdentityStoreAPIReference/Welcome.html",
@@ -137769,14 +137984,413 @@
       "api_reference_doc_page": "https://docs.aws.amazon.com/mediapackage-vod/latest/apireference/welcome.html",
       "authz_doc_page": "https://docs.aws.amazon.com/mediapackage/latest/ug/setting-up.html#setting-up-create-iam-user",
       "concepts_doc_root": "https://docs.aws.amazon.com/mediapackage/latest/ug/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/mediapackage/latest/ug/"
     },
     "prefix": "mediapackage-vod"
   },
+  "MediaPackage v2": {
+    "actions": {
+      "CreateChannel": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create a channel in a channel group",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_CreateChannel.html"
+        }
+      },
+      "CreateChannelGroup": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create a channel group",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_CreateChannelGroup.html"
+        }
+      },
+      "CreateOriginEndpoint": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create an origin endpoint for a channel",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_CreateOriginEndpoint.html"
+        }
+      },
+      "DeleteChannel": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a channel in a channel group",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_DeleteChannel.html"
+        }
+      },
+      "DeleteChannelGroup": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a channel group",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_DeleteChannelGroup.html"
+        }
+      },
+      "DeleteChannelPolicy": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a resource policy from a channel",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_DeleteChannelPolicy.html"
+        }
+      },
+      "DeleteOriginEndpoint": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete an origin endpoint of a channel",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_DeleteOriginEndpoint.html"
+        }
+      },
+      "DeleteOriginEndpointPolicy": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a resource policy from an origin endpoint",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_DeleteOriginEndpointPolicy.html"
+        }
+      },
+      "GetChannel": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve details of a channel in a channel group",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_GetChannel.html"
+        }
+      },
+      "GetChannelGroup": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve details of a channel group",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_GetChannelGroup.html"
+        }
+      },
+      "GetChannelPolicy": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve a resource policy for a channel",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_GetChannelPolicy.html"
+        }
+      },
+      "GetHeadObject": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to make GetHeadObject requests to MediaPackage",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "API_GetChannelPolicy.html",
+          "doc_page_rel": "API_GetChannelPolicy.html"
+        }
+      },
+      "GetObject": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to make GetObject requests to MediaPackage",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "API_GetChannelPolicy.html",
+          "doc_page_rel": "API_GetChannelPolicy.html"
+        }
+      },
+      "GetOriginEndpoint": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve details of an origin endpoint",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_GetOriginEndpoint.html"
+        }
+      },
+      "GetOriginEndpointPolicy": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve details of a resource policy for an origin endpoint",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_GetOriginEndpointPolicy.html"
+        }
+      },
+      "ListChannelGroups": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list all channel groups for an aws account",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_ListChannelGroups.html"
+        }
+      },
+      "ListChannels": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list all channels in a channel group",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_ListChannels.html"
+        }
+      },
+      "ListOriginEndpoints": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list all origin endpoints of a channel",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_ListOriginEndpoints.html"
+        }
+      },
+      "ListTagsForResource": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to list tags for the specified resource",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_ListTagsForResource.html"
+        }
+      },
+      "PutChannelPolicy": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to attach a resource policy for a channel",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_PutChannelPolicy.html"
+        }
+      },
+      "PutObject": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to make PutObject requests to MediaPackage",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "API_PutChannelPolicy.html",
+          "doc_page_rel": "API_PutChannelPolicy.html"
+        }
+      },
+      "PutOriginEndpointPolicy": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to attach a resource policy to an origin endpoint",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_PutOriginEndpointPolicy.html"
+        }
+      },
+      "TagResource": {
+        "aws_action_groups": [
+          "ReadWrite",
+          "Tagging"
+        ],
+        "calculated_action_group": "Tagging",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to add specified tags to the specified resource",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_TagResource.html"
+        }
+      },
+      "UntagResource": {
+        "aws_action_groups": [
+          "ReadWrite",
+          "Tagging"
+        ],
+        "calculated_action_group": "Tagging",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to remove the specified tags from the specified resource",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_UntagResource.html"
+        }
+      },
+      "UpdateChannel": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update a channel in a channel group",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_UpdateChannel.html"
+        }
+      },
+      "UpdateChannelGroup": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update a channel group",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_UpdateChannelGroup.html"
+        }
+      },
+      "UpdateOriginEndpoint": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update an origin endpoint of a channel",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/API_UpdateOriginEndpoint.html"
+        }
+      }
+    },
+    "arn_format": "arn:${Partition}:mediapackagev2:${Region}:${Account}:${ResourceType}/${ResourceIdentifier}",
+    "arn_regex": "^arn:${Partition}:mediapackagev2:.+",
+    "description": "AWS Elemental MediaPackage V2",
+    "docs": {
+      "actions_doc_root": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/",
+      "api_detail_root": "",
+      "api_doc_root": "",
+      "api_reference_doc_page": "https://docs.aws.amazon.com/mediapackage/latest/APIReference/Welcome.html",
+      "authz_doc_page": "https://docs.aws.amazon.com/mediapackage/latest/userguide/setting-up-iam-permissions.html",
+      "concepts_doc_root": "https://docs.aws.amazon.com/mediapackage/latest/userguide/",
+      "context_keys_doc_root": "https://docs.aws.amazon.com/mediapackage/latest/userguide/"
+    },
+    "prefix": "mediapackagev2"
+  },
   "MediaStore": {
     "actions": {
       "CreateContainer": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -203632,14 +204246,30 @@
         "description": "Grants permission to tag a resource with given key value pairs",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/translate/latest/APIReference/API_TagResource.html"
         }
       },
+      "TranslateDocument": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to translate a document from a source language to a target language",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/translate/latest/APIReference/API_TranslateDocument.html"
+        }
+      },
       "TranslateText": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [
@@ -203689,17 +204319,17 @@
     "arn_regex": "^arn:${Partition}:translate:.+:.+:.+",
     "description": "Amazon Translate",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/translate/latest/APIReference/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/translate/latest/APIReference/API_Operations.html",
-      "authz_doc_page": "https://docs.aws.amazon.com/translate/latest/dg/identity-and-access-management.html",
+      "authz_doc_page": "https://docs.aws.amazon.com/translate/latest/dg/security-iam.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/translate/latest/dg/",
-      "context_keys_doc_root": "https://docs.aws.amazon.com/translate/latest/dg/identity-and-access-management.html"
+      "context_keys_doc_root": "https://docs.aws.amazon.com/translate/latest/dg/security-iam.html"
     },
     "prefix": "translate"
   },
   "Trusted Advisor": {
     "actions": {
       "CreateEngagement": {
         "aws_action_groups": [
```

### Comparing `policyuniverse-1.5.1.20230523/policyuniverse/expander_minimizer.py` & `policyuniverse-1.5.1.20230526/policyuniverse/expander_minimizer.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230523/policyuniverse/organization.py` & `policyuniverse-1.5.1.20230526/policyuniverse/organization.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230523/policyuniverse/policy.py` & `policyuniverse-1.5.1.20230526/policyuniverse/policy.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230523/policyuniverse/statement.py` & `policyuniverse-1.5.1.20230526/policyuniverse/statement.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230523/policyuniverse.egg-info/PKG-INFO` & `policyuniverse-1.5.1.20230526/policyuniverse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyuniverse
-Version: 1.5.1.20230523
+Version: 1.5.1.20230526
 Summary: Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.
 Home-page: https://github.com/Netflix-Skunkworks/policyuniverse
 Author: Patrick Kelley
 Author-email: patrickbarrettkelley@gmail.com
 Keywords: iam,arn,action_groups,condition,policy,statement,wildcard
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
```

### Comparing `policyuniverse-1.5.1.20230523/policyuniverse.egg-info/SOURCES.txt` & `policyuniverse-1.5.1.20230526/policyuniverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230523/setup.py` & `policyuniverse-1.5.1.20230526/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ROOT = os.path.realpath(os.path.join(os.path.dirname(__file__)))
 
 tests_require = ["pytest", "coveralls", "bandit"]
 dev_require = ["pre-commit", "black"]
 
 setup(
     name="policyuniverse",
-    version="1.5.1.20230523",
+    version="1.5.1.20230526",
     description="Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.",
     long_description=open(os.path.join(ROOT, "README.md")).read(),
     long_description_content_type="text/markdown",
     author="Patrick Kelley",
     author_email="patrickbarrettkelley@gmail.com",
     url="https://github.com/Netflix-Skunkworks/policyuniverse",
     keywords=[
```

