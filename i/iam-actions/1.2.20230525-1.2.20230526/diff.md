# Comparing `tmp/iam_actions-1.2.20230525.tar.gz` & `tmp/iam_actions-1.2.20230526.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230525.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230526.tar", max compression
```

## Comparing `iam_actions-1.2.20230525.tar` & `iam_actions-1.2.20230526.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-25 02:27:38.644420 iam_actions-1.2.20230525/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-25 02:27:38.644420 iam_actions-1.2.20230525/README.md
--rw-r--r--   0        0        0      228 2023-05-25 02:27:38.644420 iam_actions-1.2.20230525/iam_actions/__init__.py
--rw-r--r--   0        0        0  4266621 2023-05-25 02:29:36.855195 iam_actions-1.2.20230525/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-25 02:27:38.644420 iam_actions-1.2.20230525/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-25 02:27:38.644420 iam_actions-1.2.20230525/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-25 02:27:38.644420 iam_actions-1.2.20230525/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-25 02:27:38.648420 iam_actions-1.2.20230525/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-25 02:27:38.648420 iam_actions-1.2.20230525/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-25 02:27:38.648420 iam_actions-1.2.20230525/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-25 02:27:38.648420 iam_actions-1.2.20230525/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-25 02:27:38.648420 iam_actions-1.2.20230525/iam_actions/generate/services.py
--rw-r--r--   0        0        0   548309 2023-05-25 02:29:36.855195 iam_actions-1.2.20230525/iam_actions/policies.json
--rw-r--r--   0        0        0   194498 2023-05-25 02:29:36.855195 iam_actions-1.2.20230525/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   531870 2023-05-25 02:29:36.855195 iam_actions-1.2.20230525/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-25 02:29:37.583191 iam_actions-1.2.20230525/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230525/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230525/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/README.md
+-rw-r--r--   0        0        0      228 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4273676 2023-05-26 02:29:01.701737 iam_actions-1.2.20230526/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   549435 2023-05-26 02:29:01.701737 iam_actions-1.2.20230526/iam_actions/policies.json
+-rw-r--r--   0        0        0   194779 2023-05-26 02:29:01.701737 iam_actions-1.2.20230526/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   532983 2023-05-26 02:29:01.701737 iam_actions-1.2.20230526/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-26 02:29:02.685779 iam_actions-1.2.20230526/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230526/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230526/PKG-INFO
```

### Comparing `iam_actions-1.2.20230525/LICENSE` & `iam_actions-1.2.20230526/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230525/README.md` & `iam_actions-1.2.20230526/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230525/iam_actions/actions.json` & `iam_actions-1.2.20230526/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9969451775482479%*

 * *Differences: {"'appsync'": "{'ListTypesByAssociation': {'access_level': 'List', 'description': 'Grants "*

 * *              "permission to list the types for a given merged API and source API association'}, "*

 * *              "'PutResourcePolicy': {'access_level': 'Write', 'description': 'Grants permission to "*

 * *              "set a resource policy'}, 'SourceGraphQL': {'access_level': 'Write', 'description': "*

 * *              "'Grants permission to send a GraphQL query to a source API of a merged API', "*

 * *              "'resources' […]*

```diff
@@ -6866,28 +6866,32 @@
             "description": "Grants permission to attach a GraphQL API to a custom domain name in AppSync",
             "orphan": false,
             "resources": [
                 "domain"
             ]
         },
         "AssociateMergedGraphqlApi": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateMergedGraphqlApi",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to associate a merged API to a source API",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "graphqlapi"
+            ]
         },
         "AssociateSourceGraphqlApi": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateSourceGraphqlApi",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to associate a source API to a merged API",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "graphqlapi"
+            ]
         },
         "CreateApiCache": {
             "access_level": "Write",
             "action": "CreateApiCache",
             "condition_keys": [],
             "description": "Grants permission to create an API cache in AppSync",
             "orphan": false,
@@ -7012,18 +7016,18 @@
             "action": "DeleteResolver",
             "condition_keys": [],
             "description": "Grants permission to delete a resolver",
             "orphan": false,
             "resources": []
         },
         "DeleteResourcePolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteResourcePolicy",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to remove a resource policy",
             "orphan": false,
             "resources": []
         },
         "DeleteType": {
             "access_level": "Write",
             "action": "DeleteType",
             "condition_keys": [],
@@ -7038,28 +7042,32 @@
             "description": "Grants permission to detach a GraphQL API to a custom domain name in AppSync",
             "orphan": false,
             "resources": [
                 "domain"
             ]
         },
         "DisassociateMergedGraphqlApi": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateMergedGraphqlApi",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to remove an associated source API from a merged API identified by the source API",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "mergedApiAssociation"
+            ]
         },
         "DisassociateSourceGraphqlApi": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateSourceGraphqlApi",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to remove an associated source API from a merged API identified by the merged API",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sourceApiAssociation"
+            ]
         },
         "EvaluateCode": {
             "access_level": "Read",
             "action": "EvaluateCode",
             "condition_keys": [],
             "description": "Grants permission to evaluate code with a runtime and context",
             "orphan": false,
@@ -7150,36 +7158,38 @@
             "action": "GetResolver",
             "condition_keys": [],
             "description": "Grants permission to retrieve a resolver",
             "orphan": false,
             "resources": []
         },
         "GetResourcePolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetResourcePolicy",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to read a resource policy",
             "orphan": false,
             "resources": []
         },
         "GetSchemaCreationStatus": {
             "access_level": "Read",
             "action": "GetSchemaCreationStatus",
             "condition_keys": [],
             "description": "Grants permission to retrieve the current status of a schema creation operation",
             "orphan": false,
             "resources": []
         },
         "GetSourceApiAssociation": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetSourceApiAssociation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to read information about a merged API associated source API",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sourceApiAssociation"
+            ]
         },
         "GetType": {
             "access_level": "Read",
             "action": "GetType",
             "condition_keys": [],
             "description": "Grants permission to retrieve a type",
             "orphan": false,
@@ -7249,18 +7259,18 @@
             "action": "ListResolversByFunction",
             "condition_keys": [],
             "description": "Grants permission to list the resolvers that are associated with a specific function",
             "orphan": false,
             "resources": []
         },
         "ListSourceApiAssociations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListSourceApiAssociations",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list source APIs associated to a given merged API",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
             "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [
@@ -7277,60 +7287,65 @@
             "action": "ListTypes",
             "condition_keys": [],
             "description": "Grants permission to list the types for a given API",
             "orphan": false,
             "resources": []
         },
         "ListTypesByAssociation": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListTypesByAssociation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list the types for a given merged API and source API association",
             "orphan": false,
             "resources": []
         },
         "PutResourcePolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PutResourcePolicy",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to set a resource policy",
             "orphan": false,
             "resources": []
         },
         "SetWebACL": {
             "access_level": "Write",
             "action": "SetWebACL",
             "condition_keys": [],
             "description": "Grants permission to set a web ACL",
             "orphan": false,
             "resources": []
         },
         "SourceGraphQL": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "SourceGraphQL",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to send a GraphQL query to a source API of a merged API",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "field",
+                "graphqlapi"
+            ]
         },
         "StartSchemaCreation": {
             "access_level": "Write",
             "action": "StartSchemaCreation",
             "condition_keys": [],
             "description": "Grants permission to add a new schema to your GraphQL API. This operation is asynchronous - GetSchemaCreationStatus can show when it has completed",
             "orphan": false,
             "resources": []
         },
         "StartSchemaMerge": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartSchemaMerge",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to initiate a schema merge for a given merged API and associated source API",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sourceApiAssociation"
+            ]
         },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
@@ -7413,20 +7428,22 @@
             "action": "UpdateResolver",
             "condition_keys": [],
             "description": "Grants permission to update a resolver",
             "orphan": false,
             "resources": []
         },
         "UpdateSourceApiAssociation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateSourceApiAssociation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update a merged API source API association",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sourceApiAssociation"
+            ]
         },
         "UpdateType": {
             "access_level": "Write",
             "action": "UpdateType",
             "condition_keys": [],
             "description": "Grants permission to update a type",
             "orphan": false,
@@ -24859,14 +24876,22 @@
             "access_level": "Undocumented",
             "action": "DeleteScansByCategory",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "GetAccountConfiguration": {
+            "access_level": "Undocumented",
+            "action": "GetAccountConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetFindings": {
             "access_level": "Undocumented",
             "action": "GetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -94975,14 +95000,232 @@
             "description": "Grants permission to update a packaging group in AWS Elemental MediaPackage",
             "orphan": false,
             "resources": [
                 "packaging-groups"
             ]
         }
     },
+    "mediapackagev2": {
+        "CreateChannel": {
+            "access_level": "Undocumented",
+            "action": "CreateChannel",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateChannelGroup": {
+            "access_level": "Undocumented",
+            "action": "CreateChannelGroup",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateOriginEndpoint": {
+            "access_level": "Undocumented",
+            "action": "CreateOriginEndpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteChannel": {
+            "access_level": "Undocumented",
+            "action": "DeleteChannel",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteChannelGroup": {
+            "access_level": "Undocumented",
+            "action": "DeleteChannelGroup",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteChannelPolicy": {
+            "access_level": "Undocumented",
+            "action": "DeleteChannelPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteOriginEndpoint": {
+            "access_level": "Undocumented",
+            "action": "DeleteOriginEndpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteOriginEndpointPolicy": {
+            "access_level": "Undocumented",
+            "action": "DeleteOriginEndpointPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetChannel": {
+            "access_level": "Undocumented",
+            "action": "GetChannel",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetChannelGroup": {
+            "access_level": "Undocumented",
+            "action": "GetChannelGroup",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetChannelPolicy": {
+            "access_level": "Undocumented",
+            "action": "GetChannelPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetHeadObject": {
+            "access_level": "Undocumented",
+            "action": "GetHeadObject",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetObject": {
+            "access_level": "Undocumented",
+            "action": "GetObject",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetOriginEndpoint": {
+            "access_level": "Undocumented",
+            "action": "GetOriginEndpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetOriginEndpointPolicy": {
+            "access_level": "Undocumented",
+            "action": "GetOriginEndpointPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListChannelGroups": {
+            "access_level": "Undocumented",
+            "action": "ListChannelGroups",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListChannels": {
+            "access_level": "Undocumented",
+            "action": "ListChannels",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListOriginEndpoints": {
+            "access_level": "Undocumented",
+            "action": "ListOriginEndpoints",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTagsForResource": {
+            "access_level": "Undocumented",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "PutChannelPolicy": {
+            "access_level": "Undocumented",
+            "action": "PutChannelPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "PutObject": {
+            "access_level": "Undocumented",
+            "action": "PutObject",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "PutOriginEndpointPolicy": {
+            "access_level": "Undocumented",
+            "action": "PutOriginEndpointPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "TagResource": {
+            "access_level": "Undocumented",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateChannel": {
+            "access_level": "Undocumented",
+            "action": "UpdateChannel",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateChannelGroup": {
+            "access_level": "Undocumented",
+            "action": "UpdateChannelGroup",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateOriginEndpoint": {
+            "access_level": "Undocumented",
+            "action": "UpdateOriginEndpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        }
+    },
     "mediastore": {
         "CreateContainer": {
             "access_level": "Write",
             "action": "CreateContainer",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -117317,14 +117560,30 @@
             "access_level": "List",
             "action": "ListTrustAnchors",
             "condition_keys": [],
             "description": "Grants permission to list trust anchors",
             "orphan": false,
             "resources": []
         },
+        "PutNotificationSettings": {
+            "access_level": "Undocumented",
+            "action": "PutNotificationSettings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ResetNotificationSettings": {
+            "access_level": "Undocumented",
+            "action": "ResetNotificationSettings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -144617,20 +144876,22 @@
             "orphan": false,
             "resources": [
                 "parallel-data",
                 "terminology"
             ]
         },
         "TranslateDocument": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "TranslateDocument",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to translate a document from a source language to a target language",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "terminology"
+            ]
         },
         "TranslateText": {
             "access_level": "Read",
             "action": "TranslateText",
             "condition_keys": [],
             "description": "Grants permission to translate text from a source language to a target language",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20230525/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230526/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230525/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230526/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230525/iam_actions/generate/generate.py` & `iam_actions-1.2.20230526/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230525/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230526/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230525/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230526/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230525/iam_actions/generate/services.py` & `iam_actions-1.2.20230526/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230525/iam_actions/policies.json` & `iam_actions-1.2.20230526/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997193697107492%*

 * *Differences: {"'serviceMap'": "{'Amazon CodeGuru Security': {'Actions': {insert: [(4, "*

 * *                 "'GetAccountConfiguration')]}}, 'AWS Identity Store': {'ARNFormat': "*

 * *                 "'arn:aws:identitystore::${Account}:${ResourceType}/${ResourceId}'}, 'AWS "*

 * *                 "Identity and Access Management Roles Anywhere': {'Actions': {insert: [(21, "*

 * *                 "'PutNotificationSettings'), (22, 'ResetNotificationSettings')]}}, 'AWS Elemental "*

 * *                 "MediaPackage V2': OrderedDict([('StringPref […]*

```diff
@@ -3596,14 +3596,54 @@
             "StringPrefix": "mediapackage",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
+        "AWS Elemental MediaPackage V2": {
+            "ARNFormat": "arn:aws:mediapackagev2:${Region}:${Account}:${ResourceType}/${ResourceIdentifier}",
+            "ARNRegex": "^arn:aws:mediapackagev2:.+",
+            "Actions": [
+                "CreateChannel",
+                "CreateChannelGroup",
+                "CreateOriginEndpoint",
+                "DeleteChannel",
+                "DeleteChannelGroup",
+                "DeleteChannelPolicy",
+                "DeleteOriginEndpoint",
+                "DeleteOriginEndpointPolicy",
+                "GetChannel",
+                "GetChannelGroup",
+                "GetChannelPolicy",
+                "GetHeadObject",
+                "GetObject",
+                "GetOriginEndpoint",
+                "GetOriginEndpointPolicy",
+                "ListChannelGroups",
+                "ListChannels",
+                "ListOriginEndpoints",
+                "ListTagsForResource",
+                "PutChannelPolicy",
+                "PutObject",
+                "PutOriginEndpointPolicy",
+                "TagResource",
+                "UntagResource",
+                "UpdateChannel",
+                "UpdateChannelGroup",
+                "UpdateOriginEndpoint"
+            ],
+            "HasResource": true,
+            "StringPrefix": "mediapackagev2",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
+        },
         "AWS Elemental MediaPackage VOD": {
             "ARNFormat": "arn:aws:mediapackage-vod:${Region}:${Account}:${ResourceType}/${ResourceIdentifier}",
             "ARNRegex": "^arn:aws:mediapackage-vod:.+:.+:.+",
             "Actions": [
                 "ConfigureLogs",
                 "CreateAsset",
                 "CreatePackagingConfiguration",
@@ -4557,15 +4597,15 @@
                 "RevokePermissionRequest",
                 "WithdrawPermissionRequest"
             ],
             "HasResource": true,
             "StringPrefix": "iq-permission"
         },
         "AWS Identity Store": {
-            "ARNFormat": "arn:aws:identitystore::${AwsAccountId}:${ResourceType}/${ResourceId}",
+            "ARNFormat": "arn:aws:identitystore::${Account}:${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:identitystore:.+",
             "Actions": [
                 "CreateGroup",
                 "CreateGroupMembership",
                 "CreateUser",
                 "DeleteGroup",
                 "DeleteGroupMembership",
@@ -4829,14 +4869,16 @@
                 "GetTrustAnchor",
                 "ImportCrl",
                 "ListCrls",
                 "ListProfiles",
                 "ListSubjects",
                 "ListTagsForResource",
                 "ListTrustAnchors",
+                "PutNotificationSettings",
+                "ResetNotificationSettings",
                 "TagResource",
                 "UntagResource",
                 "UpdateCrl",
                 "UpdateProfile",
                 "UpdateTrustAnchor"
             ],
             "HasResource": true,
@@ -10902,14 +10944,15 @@
             "ARNFormat": "arn:aws:codeguru-security:${Region}:${Account}:*",
             "ARNRegex": "^arn:aws:codeguru-security:.+:.+:.+",
             "Actions": [
                 "BatchGetFindings",
                 "CreateScan",
                 "CreateUploadUrl",
                 "DeleteScansByCategory",
+                "GetAccountConfiguration",
                 "GetFindings",
                 "GetScan",
                 "ListFindings",
                 "ListScans",
                 "UpdateAccountConfiguration"
             ],
             "HasResource": true,
```

### Comparing `iam_actions-1.2.20230525/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230526/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996875%*

 * *Differences: {"'appsync'": "{'sourceApiAssociation': OrderedDict([('arn_pattern', "*

 * *              "'arn:*:appsync:*:*:apis/*/sourceApiAssociations/*'), ('condition_keys', None)]), "*

 * *              "'mergedApiAssociation': OrderedDict([('arn_pattern', "*

 * *              "'arn:*:appsync:*:*:apis/*/mergedApiAssociations/*'), ('condition_keys', None)])}",*

 * * "'mediapackagev2'": 'OrderedDict()'}*

```diff
@@ -618,14 +618,22 @@
             "arn_pattern": "arn:*:appsync:*:*:apis/*/functions/*",
             "condition_keys": null
         },
         "graphqlapi": {
             "arn_pattern": "arn:*:appsync:*:*:apis/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "mergedApiAssociation": {
+            "arn_pattern": "arn:*:appsync:*:*:apis/*/mergedApiAssociations/*",
+            "condition_keys": null
+        },
+        "sourceApiAssociation": {
+            "arn_pattern": "arn:*:appsync:*:*:apis/*/sourceApiAssociations/*",
+            "condition_keys": null
+        },
         "type": {
             "arn_pattern": "arn:*:appsync:*:*:apis/*/types/*",
             "condition_keys": null
         }
     },
     "aps": {
         "rulegroupsnamespace": {
@@ -4165,14 +4173,15 @@
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "packaging-groups": {
             "arn_pattern": "arn:*:mediapackage-vod:*:*:packaging-groups/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
+    "mediapackagev2": {},
     "mediastore": {
         "container": {
             "arn_pattern": "arn:*:mediastore:*:*:container/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "folder": {
             "arn_pattern": "arn:*:mediastore:*:*:container/*/*",
```

### Comparing `iam_actions-1.2.20230525/iam_actions/services.json` & `iam_actions-1.2.20230526/iam_actions/services.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970866402116403%*

 * *Differences: {"'codeguru-security'": "{'Actions': {insert: [(4, 'GetAccountConfiguration')]}}",*

 * * "'identitystore'": "{'ARNFormats': "*

 * *                    "['arn:aws:identitystore::${Account}:${ResourceType}/${ResourceId}']}",*

 * * "'mediapackagev2'": "OrderedDict([('Actions', ['CreateChannel', 'CreateChannelGroup', "*

 * *                     "'CreateOriginEndpoint', 'DeleteChannel', 'DeleteChannelGroup', "*

 * *                     "'DeleteChannelPolicy', 'DeleteOriginEndpoint', 'DeleteOriginEndpointPolicy', "*

 * *                     " […]*

```diff
@@ -3802,14 +3802,15 @@
             "^arn:aws:codeguru-security:.+:.+:.+"
         ],
         "Actions": [
             "BatchGetFindings",
             "CreateScan",
             "CreateUploadUrl",
             "DeleteScansByCategory",
+            "GetAccountConfiguration",
             "GetFindings",
             "GetScan",
             "ListFindings",
             "ListScans",
             "UpdateAccountConfiguration"
         ],
         "ConditionKeys": [],
@@ -9964,15 +9965,15 @@
         "HasResource": true,
         "ServiceNames": [
             "AWS Identity Sync"
         ]
     },
     "identitystore": {
         "ARNFormats": [
-            "arn:aws:identitystore::${AwsAccountId}:${ResourceType}/${ResourceId}"
+            "arn:aws:identitystore::${Account}:${ResourceType}/${ResourceId}"
         ],
         "ARNRegexes": [
             "^arn:aws:identitystore:.+"
         ],
         "Actions": [
             "CreateGroup",
             "CreateGroupMembership",
@@ -13290,14 +13291,60 @@
             "aws:TagKeys"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Elemental MediaPackage VOD"
         ]
     },
+    "mediapackagev2": {
+        "ARNFormats": [
+            "arn:aws:mediapackagev2:${Region}:${Account}:${ResourceType}/${ResourceIdentifier}"
+        ],
+        "ARNRegexes": [
+            "^arn:aws:mediapackagev2:.+"
+        ],
+        "Actions": [
+            "CreateChannel",
+            "CreateChannelGroup",
+            "CreateOriginEndpoint",
+            "DeleteChannel",
+            "DeleteChannelGroup",
+            "DeleteChannelPolicy",
+            "DeleteOriginEndpoint",
+            "DeleteOriginEndpointPolicy",
+            "GetChannel",
+            "GetChannelGroup",
+            "GetChannelPolicy",
+            "GetHeadObject",
+            "GetObject",
+            "GetOriginEndpoint",
+            "GetOriginEndpointPolicy",
+            "ListChannelGroups",
+            "ListChannels",
+            "ListOriginEndpoints",
+            "ListTagsForResource",
+            "PutChannelPolicy",
+            "PutObject",
+            "PutOriginEndpointPolicy",
+            "TagResource",
+            "UntagResource",
+            "UpdateChannel",
+            "UpdateChannelGroup",
+            "UpdateOriginEndpoint"
+        ],
+        "ConditionKeys": [
+            "aws:RequestTag/${TagKey}",
+            "aws:ResourceTag/${TagKey}",
+            "aws:TagKeys"
+        ],
+        "HasResource": true,
+        "ServiceNames": [
+            "AWS Elemental MediaPackage V2"
+        ]
+    },
     "mediastore": {
         "ARNFormats": [
             "arn:aws:mediastore:${Region}:${Account}:${Resource}"
         ],
         "ARNRegexes": [
             "^arn:aws:mediastore:.+:.+"
         ],
@@ -16492,14 +16539,16 @@
             "GetTrustAnchor",
             "ImportCrl",
             "ListCrls",
             "ListProfiles",
             "ListSubjects",
             "ListTagsForResource",
             "ListTrustAnchors",
+            "PutNotificationSettings",
+            "ResetNotificationSettings",
             "TagResource",
             "UntagResource",
             "UpdateCrl",
             "UpdateProfile",
             "UpdateTrustAnchor"
         ],
         "ConditionKeys": [
```

### Comparing `iam_actions-1.2.20230525/pyproject.toml` & `iam_actions-1.2.20230526/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230525"
+version = "1.2.20230526"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230525/setup.py` & `iam_actions-1.2.20230526/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230525',
+    'version': '1.2.20230526',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230525/PKG-INFO` & `iam_actions-1.2.20230526/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230525
+Version: 1.2.20230526
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

