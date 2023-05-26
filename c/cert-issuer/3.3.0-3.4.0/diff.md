# Comparing `tmp/cert-issuer-3.3.0.tar.gz` & `tmp/cert-issuer-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cert-issuer-3.3.0.tar", last modified: Thu Aug 25 15:29:38 2022, max compression
+gzip compressed data, was "cert-issuer-3.4.0.tar", last modified: Fri May 26 13:35:07 2023, max compression
```

## Comparing `cert-issuer-3.3.0.tar` & `cert-issuer-3.4.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-08-25 15:29:38.000000 cert-issuer-3.3.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2138 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-08-25 15:29:38.000000 cert-issuer-3.3.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5773 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/tests/test_connectors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      363 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/tests/test_signer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11817 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/tests/test_proof_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8798 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/tests/test_certificate_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6054 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/tests/test_tx_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3756 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/tests/test_merkle_tree_generator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19187 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-08-25 15:29:38.000000 cert-issuer-3.3.0/cert_issuer/
--rw-rw-r--   0 travis    (2000) travis    (2000)      544 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1306 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/chained_proof_2021.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2689 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/signer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1961 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/proof_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4841 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-08-25 15:29:38.000000 cert-issuer-3.3.0/cert_issuer/models/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5253 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/models/verifiable_credential.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2646 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/models/metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3421 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/models/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2968 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/merkle_tree_generator.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-08-25 15:29:38.000000 cert-issuer-3.3.0/cert_issuer/blockchain_handlers/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-08-25 15:29:38.000000 cert-issuer-3.3.0/cert_issuer/blockchain_handlers/bitcoin/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3031 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/blockchain_handlers/bitcoin/signer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4611 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/blockchain_handlers/bitcoin/transaction_handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4805 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/blockchain_handlers/bitcoin/tx_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10248 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/blockchain_handlers/bitcoin/connectors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3595 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/blockchain_handlers/bitcoin/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-08-25 15:29:38.000000 cert-issuer-3.3.0/cert_issuer/blockchain_handlers/ethereum/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1508 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/blockchain_handlers/ethereum/signer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3947 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/blockchain_handlers/ethereum/transaction_handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1085 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/blockchain_handlers/ethereum/tx_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13044 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/blockchain_handlers/ethereum/connectors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3133 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/blockchain_handlers/ethereum/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/blockchain_handlers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1352 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/issuer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      793 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/normalization_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5688 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/certificate_handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1590 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/issue_certificates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1079 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2022-08-25 15:29:37.000000 cert-issuer-3.3.0/cert_issuer/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8688 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/cert_issuer/config.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-08-25 15:29:38.000000 cert-issuer-3.3.0/cert_issuer.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2022-08-25 15:29:38.000000 cert-issuer-3.3.0/cert_issuer.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1629 2022-08-25 15:29:38.000000 cert-issuer-3.3.0/cert_issuer.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    19526 2022-08-25 15:29:38.000000 cert-issuer-3.3.0/cert_issuer.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      250 2022-08-25 15:29:38.000000 cert-issuer-3.3.0/cert_issuer.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2022-08-25 15:29:38.000000 cert-issuer-3.3.0/cert_issuer.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-08-25 15:29:38.000000 cert-issuer-3.3.0/cert_issuer.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    19526 2022-08-25 15:29:38.000000 cert-issuer-3.3.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/ethereum_requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      250 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       25 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/bitcoin_requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      309 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/conf_regtest.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)      134 2022-08-25 15:29:38.000000 cert-issuer-3.3.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1096 2022-08-25 15:29:02.000000 cert-issuer-3.3.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      502 2022-08-25 15:29:37.000000 cert-issuer-3.3.0/CHANGELOG.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-26 13:35:07.939885 cert-issuer-3.4.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      934 2023-05-26 13:35:05.000000 cert-issuer-3.4.0/CHANGELOG.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1096 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       43 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19777 2023-05-26 13:35:07.939885 cert-issuer-3.4.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19438 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       25 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/bitcoin_requirements.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-26 13:35:07.935884 cert-issuer-3.4.0/cert_issuer/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2023-05-26 13:35:05.000000 cert-issuer-3.4.0/cert_issuer/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      544 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/__main__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-26 13:35:07.935884 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-26 13:35:07.935884 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3595 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10248 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/connectors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3031 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/signer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4611 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/transaction_handlers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4805 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/tx_utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-26 13:35:07.939885 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3624 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13037 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/connectors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/signer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4233 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/transaction_handlers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1210 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/tx_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5688 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/certificate_handlers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1306 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/chained_proof_2021.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9143 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1079 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4841 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1590 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/issue_certificates.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1352 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/issuer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2968 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/merkle_tree_generator.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-26 13:35:07.939885 cert-issuer-3.4.0/cert_issuer/models/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3421 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/models/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2646 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/models/metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5857 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/models/verifiable_credential.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      793 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/normalization_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1961 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/proof_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2689 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/signer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       73 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-26 13:35:07.935884 cert-issuer-3.4.0/cert_issuer.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19777 2023-05-26 13:35:07.000000 cert-issuer-3.4.0/cert_issuer.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1629 2023-05-26 13:35:07.000000 cert-issuer-3.4.0/cert_issuer.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-26 13:35:07.000000 cert-issuer-3.4.0/cert_issuer.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2023-05-26 13:35:07.000000 cert-issuer-3.4.0/cert_issuer.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      266 2023-05-26 13:35:07.000000 cert-issuer-3.4.0/cert_issuer.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       18 2023-05-26 13:35:07.000000 cert-issuer-3.4.0/cert_issuer.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      309 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/conf_regtest.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)       25 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/ethereum_requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      265 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      134 2023-05-26 13:35:07.939885 cert-issuer-3.4.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2138 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-26 13:35:07.939885 cert-issuer-3.4.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8798 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/tests/test_certificate_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5773 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/tests/test_connectors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3756 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/tests/test_merkle_tree_generator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11817 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/tests/test_proof_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      363 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/tests/test_signer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6054 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/tests/test_tx_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cert-issuer-3.3.0/setup.py` & `cert-issuer-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/tests/test_connectors.py` & `cert-issuer-3.4.0/tests/test_connectors.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/tests/test_proof_handler.py` & `cert-issuer-3.4.0/tests/test_proof_handler.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/tests/test_certificate_handler.py` & `cert-issuer-3.4.0/tests/test_certificate_handler.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/tests/test_tx_utils.py` & `cert-issuer-3.4.0/tests/test_tx_utils.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/tests/test_merkle_tree_generator.py` & `cert-issuer-3.4.0/tests/test_merkle_tree_generator.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/README.md` & `cert-issuer-3.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: cert-issuer
+Version: 3.4.0
+Summary: Issues blockchain certificates using the Bitcoin blockchain
+Home-page: https://github.com/blockchain-certificates/cert-issuer
+Author: Blockcerts
+Author-email: info@blockcerts.org
+License: MIT
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Verifiable Credential Compliance result](https://badgen.net/badge/Verifiable%20Credentials%20v1/compliant/green?icon=https://www.w3.org/Icons/WWW/w3c_home_nb-v.svg)](https://github.com/blockchain-certificates/cert-issuer/vc-compliance-report.html)
 [![Build Status](https://travis-ci.org/blockchain-certificates/cert-issuer.svg?branch=master)](https://travis-ci.org/blockchain-certificates/cert-issuer)
 [![PyPI version](https://badge.fury.io/py/cert-issuer.svg)](https://badge.fury.io/py/cert-issuer)
 
 # cert-issuer
 
 The cert-issuer project issues blockchain certificates by creating a transaction from the issuing institution to the
 recipient on the Bitcoin or Ethereum blockchains. That transaction includes the hash of the certificate itself.
@@ -422,7 +435,9 @@
       file not found
 #include <openssl/aes.h>
 ```
 
 # Contact
 
 Contact us at [the Blockcerts community forum](http://community.blockcerts.org/).
+
+
```

### Comparing `cert-issuer-3.3.0/cert_issuer/__main__.py` & `cert-issuer-3.4.0/cert_issuer/__main__.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/chained_proof_2021.py` & `cert-issuer-3.4.0/cert_issuer/chained_proof_2021.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/signer.py` & `cert-issuer-3.4.0/cert_issuer/signer.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/proof_handler.py` & `cert-issuer-3.4.0/cert_issuer/proof_handler.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/helpers.py` & `cert-issuer-3.4.0/cert_issuer/helpers.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/models/verifiable_credential.py` & `cert-issuer-3.4.0/cert_issuer/models/verifiable_credential.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import logging
 from urllib.parse import urlparse
 from cert_schema import ContextUrls
 
 # TODO: move the v3 checks to cert-schema
 def validate_RFC3339_date (date):
     return re.match('^[1-9]\d{3}-\d{2}-\d{2}[Tt\s]\d{2}:\d{2}:\d{2}(?:\.\d{3})?((?:[+-]\d{2}:\d{2})|[Zz])$', date)
 
@@ -38,23 +39,37 @@
     if not isinstance(context, list):
         raise ValueError('`@context` property must be an array')
     if context[0] != vc_context_url:
         raise ValueError('First @context declared must be {}, was given {}'.format(vc_context_url, context[0]))
     if len(type) > 1 and len(context) == 1:
         raise ValueError('A more specific type: {}, was detected, yet no context seems provided for that type'.format(type[1]))
     if context[-1] not in blockcerts_valid_context_url:
-        raise ValueError('Last @context declared must be one of valid blockcerts context url, preferably {}, was given {}'.format(blockcerts_valid_context_url[-1]), context[-1])
+        logging.warning("""
+           Last `@context` is not blockcerts' context. It is not a critical issue but some issues have come up at times
+           because of some properties of a different context overwriting blockcerts' taxonomy. Check this property
+           again in case of verification issue.
+           """)
 
     pass
 
 def validate_credential_subject (credential_subject):
     pass
 
 def validate_issuer (certificate_issuer):
-    if not is_valid_url(certificate_issuer) and not is_valid_url(certificate_issuer['id']):
+    has_error = False
+    if isinstance(certificate_issuer, str) and not is_valid_url(certificate_issuer):
+        has_error = True
+
+    if isinstance(certificate_issuer, dict) and not is_valid_url(certificate_issuer['id']):
+        has_error = True
+
+    if isinstance(certificate_issuer, list):
+        has_error = True
+        
+    if has_error:
         raise ValueError('`issuer` property must be a URL string or an object with an `id` property containing a URL string')
     pass
 
 def validate_date_RFC3339_string_format (date, property_name):
     error_message = '`{}` property must be a valid RFC3339 string.'.format(property_name)
     if not isinstance(date, str):
         error_message += ' `{}` value is not a string'.format(date)
@@ -70,27 +85,31 @@
     pass
 
 def validate_expiration_date (certificate_expiration_date):
     validate_date_RFC3339_string_format(certificate_expiration_date, 'expirationDate')
     pass
 
 def validate_credential_status (certificate_credential_status):
-    try:
-        validate_url(certificate_credential_status['id'])
-    except KeyError:
-        raise ValueError('credentialStatus.id must be defined')
-    except ValueError:
-        raise ValueError('credentialStatus.id must be a valid URL')
+    if not isinstance(certificate_credential_status, list):
+        certificate_credential_status = [certificate_credential_status]
 
-    try:
-        isinstance(certificate_credential_status['type'], str)
-    except KeyError:
-        raise ValueError('credentialStatus.type must be defined')
-    except:
-        raise ValueError('credentialStatus.type must be a string')
+    for status in certificate_credential_status:
+        try:
+            validate_url(status['id'])
+        except KeyError:
+            raise ValueError('credentialStatus.id must be defined')
+        except ValueError:
+            raise ValueError('credentialStatus.id must be a valid URL')
+
+        try:
+            isinstance(status['type'], str)
+        except KeyError:
+            raise ValueError('credentialStatus.type must be defined')
+        except:
+            raise ValueError('credentialStatus.type must be a string')
     pass
 
 def verify_credential(certificate_metadata):
     try:
         # if undefined will throw KeyError
         validate_credential_subject(certificate_metadata['credentialSubject'])
     except:
```

### Comparing `cert-issuer-3.3.0/cert_issuer/models/metadata.py` & `cert-issuer-3.4.0/cert_issuer/models/metadata.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/models/__init__.py` & `cert-issuer-3.4.0/cert_issuer/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/merkle_tree_generator.py` & `cert-issuer-3.4.0/cert_issuer/merkle_tree_generator.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/blockchain_handlers/bitcoin/signer.py` & `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/signer.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/blockchain_handlers/bitcoin/transaction_handlers.py` & `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/transaction_handlers.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/blockchain_handlers/bitcoin/tx_utils.py` & `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/tx_utils.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/blockchain_handlers/bitcoin/connectors.py` & `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/connectors.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/blockchain_handlers/bitcoin/__init__.py` & `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/__init__.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/blockchain_handlers/ethereum/signer.py` & `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/signer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import rlp
-from ethereum import transactions
-from ethereum.utils import encode_hex
+import web3
+from eth_utils import to_hex
 
 from cert_issuer.errors import UnableToSignTxError
 from cert_issuer.models import Signer
 
 
 class EthereumSigner(Signer):
     def __init__(self, ethereum_chain):
@@ -24,16 +23,17 @@
     # wif = unencrypted private key as string in the first line of the supplied private key file
     def sign_message(self, wif, message_to_sign):
         pass
 
     def sign_transaction(self, wif, transaction_to_sign):
         ##try to sign the transaction.
 
-        if isinstance(transaction_to_sign, transactions.Transaction):
+        if isinstance(transaction_to_sign, dict):
             try:
-                raw_tx = rlp.encode(transaction_to_sign.sign(wif, self.netcode))
-                raw_tx_hex = encode_hex(raw_tx)
+                transaction_to_sign['chainId'] = self.netcode
+                raw_tx = web3.Account.sign_transaction(transaction_to_sign, wif)['rawTransaction']
+                raw_tx_hex = to_hex(raw_tx)
                 return raw_tx_hex
             except Exception as msg:
                 return {'error': True, 'message': msg}
         else:
-            raise UnableToSignTxError('You are trying to sign a non transaction type')
+            raise UnableToSignTxError('"sign_transaction()" expects a dict representing an unsigned transaction with fields such as "gas", "to", "data", etc. run "$ python cert_issuer -h" for more information on transaction configuration.')
```

### Comparing `cert-issuer-3.3.0/cert_issuer/blockchain_handlers/ethereum/transaction_handlers.py` & `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/transaction_handlers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,84 @@
 import logging
 
-from pycoin.serialize import b2h
+from web3 import Web3
+from eth_utils import to_hex, remove_0x_prefix
 
 from cert_issuer.errors import InsufficientFundsError
 from cert_issuer.blockchain_handlers.ethereum import tx_utils
 from cert_issuer.models import TransactionHandler
 from cert_issuer.signer import FinalizableSigner
 
 
 # as the transaction format in Ethereum is different, the abstracted TransactionCreator doesn't satisfy
 class EthereumTransactionCreator(object):
     def estimate_cost_for_certificate_batch(self):
         pass
 
     def create_transaction(self, tx_cost_constants, issuing_address, nonce, to_address, blockchain_bytes):
+        max_priority_fee_per_gas = tx_cost_constants.get_max_priority_fee_per_gas()
         gasprice = tx_cost_constants.get_gas_price()
         gaslimit = tx_cost_constants.get_gas_limit()
 
         transaction = tx_utils.create_ethereum_trx(
-            issuing_address,
             nonce,
             to_address,
             blockchain_bytes,
+            max_priority_fee_per_gas,
             gasprice,
             gaslimit)
 
         return transaction
 
 
 class EthereumTransactionHandler(TransactionHandler):
-    def __init__(self, connector, tx_cost_constants, secret_manager, issuing_address, prepared_inputs=None,
+    def __init__(self, connector, nonce, tx_cost_constants, secret_manager, issuing_address, prepared_inputs=None,
                  transaction_creator=EthereumTransactionCreator()):
         self.connector = connector
+        self.nonce = nonce
         self.tx_cost_constants = tx_cost_constants
         self.secret_manager = secret_manager
-        self.issuing_address = issuing_address
+        self.issuing_address = Web3.toChecksumAddress(issuing_address)
         # input transactions are not needed for Ether
         self.prepared_inputs = prepared_inputs
         self.transaction_creator = transaction_creator
 
     def ensure_balance(self):
         # testing etherscan api wrapper
         self.balance = self.connector.get_balance(self.issuing_address)
 
         # for now transaction cost will be a constant: (25000 gas estimate times 20Gwei gasprice) from tx_utils
         # can later be calculated inside EthereumTransaction_creator
         transaction_cost = self.tx_cost_constants.get_recommended_max_cost()
-        logging.info('Total cost will be %d wei', transaction_cost)
+        logging.info('Total cost will be no more than %d wei', transaction_cost)
 
         if transaction_cost > self.balance:
             error_message = 'Please add {} wei to the address {}'.format(
                 transaction_cost - self.balance, self.issuing_address)
             logging.error(error_message)
             raise InsufficientFundsError(error_message)
 
     def issue_transaction(self, blockchain_bytes):
-        eth_data_field = b2h(blockchain_bytes)
+        eth_data_field = remove_0x_prefix(to_hex(blockchain_bytes))
         prepared_tx = self.create_transaction(blockchain_bytes)
         signed_tx = self.sign_transaction(prepared_tx)
         self.verify_transaction(signed_tx, eth_data_field)
         txid = self.broadcast_transaction(signed_tx)
         return txid
 
     def create_transaction(self, blockchain_bytes):
         if self.balance:
             # it is assumed here that the address has sufficient funds, as the ensure_balance has just been checked
-            nonce = self.connector.get_address_nonce(self.issuing_address)
+            nonce = self.nonce or self.connector.get_address_nonce(self.issuing_address)
+            logging.info("NONCE IS %d", nonce)
             # Transactions in the first iteration will be send to burn address
-            toaddress = '0xdeaddeaddeaddeaddeaddeaddeaddeaddeaddead'
-            tx = self.transaction_creator.create_transaction(self.tx_cost_constants, self.issuing_address, nonce,
+            toaddress = Web3.toChecksumAddress('0xdeaddeaddeaddeaddeaddeaddeaddeaddeaddead')
+            prepared_tx = self.transaction_creator.create_transaction(self.tx_cost_constants, self.issuing_address, nonce,
                                                              toaddress, blockchain_bytes)
 
-            prepared_tx = tx
             return prepared_tx
         else:
             raise InsufficientFundsError('Not sufficient ether to spend at: %s', self.issuing_address)
 
     def sign_transaction(self, prepared_tx):
         # stubbed from BitcoinTransactionHandler
         with FinalizableSigner(self.secret_manager) as signer:
```

### Comparing `cert-issuer-3.3.0/cert_issuer/blockchain_handlers/ethereum/tx_utils.py` & `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/tx_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 import logging
 
 from cert_issuer.errors import UnverifiedTransactionError
 
 
-def create_ethereum_trx(issuing_address, nonce, to_address, blockchain_bytes, gasprice, gaslimit):
+def create_ethereum_trx(nonce, to_address, blockchain_bytes, max_priority_fee_per_gas, gasprice, gaslimit):
     # the actual value transfer is 0 in the Ethereum implementation
-    from ethereum.transactions import Transaction
     value = 0
-    tx = Transaction(nonce=nonce, gasprice=gasprice, startgas=gaslimit, to=to_address, value=value,
-                     data=blockchain_bytes)
+    tx = dict(
+        nonce=nonce,
+        gas=gaslimit,
+        to=to_address,
+        value=value,
+        data=blockchain_bytes)
+    if max_priority_fee_per_gas:
+        tx['maxFeePerGas'] = gasprice
+        tx['maxPriorityFeePerGas'] = max_priority_fee_per_gas
+    else:
+        tx['gasPrice'] = gasprice
     return tx
 
 
 def verify_eth_transaction(signed_hextx, eth_data_field):
     """
     Verify ethDataField field in transaction
     :param signed_hextx:
```

### Comparing `cert-issuer-3.3.0/cert_issuer/blockchain_handlers/ethereum/connectors.py` & `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/connectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 class EthereumRPCProvider(object):
     def __init__(self, ethereum_url):
         self.ethereum_url = ethereum_url
         self.w3 = Web3(HTTPProvider(ethereum_url))
 
     def broadcast_tx(self, tx):
         logging.info('Broadcasting transaction with EthereumRPCProvider')
-        response = self.w3.eth.sendRawTransaction("0x" + tx).hex()
+        response = self.w3.eth.sendRawTransaction(tx).hex()
         return response
 
     def get_balance(self, address):
         """
         Returns the balance in Wei.
         """
         response = self.w3.eth.getBalance(account=address, block_identifier="latest")
```

### Comparing `cert-issuer-3.3.0/cert_issuer/issuer.py` & `cert-issuer-3.4.0/cert_issuer/issuer.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/normalization_handler.py` & `cert-issuer-3.4.0/cert_issuer/normalization_handler.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/certificate_handlers.py` & `cert-issuer-3.4.0/cert_issuer/certificate_handlers.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/issue_certificates.py` & `cert-issuer-3.4.0/cert_issuer/issue_certificates.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/errors.py` & `cert-issuer-3.4.0/cert_issuer/errors.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer/config.py` & `cert-issuer-3.4.0/cert_issuer/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     logger.addHandler(handler)
 
 
 # restructured arguments to put the chain specific arguments together.
 def add_arguments(p):
     p.add('-c', '--my-config', required=False, env_var='CONFIG_FILE',
           is_config_file=True, help='config file path')
-    p.add_argument('--issuing_address', required=True, help='issuing address', env_var='ISSUING_ADDRESS')
-    p.add_argument('--verification_method', required=True, help='Verification method for the Linked Data Proof', env_var='VERIFICATION_METHOD')
+    p.add_argument('--issuing_address', required=False, help='issuing address', env_var='ISSUING_ADDRESS')
+    p.add_argument('--verification_method', required=False, help='Verification method for the Linked Data Proof', env_var='VERIFICATION_METHOD')
     p.add_argument('--usb_name', required=True, help='usb path to key_file', env_var='USB_NAME')
     p.add_argument('--key_file', required=True,
                    help='name of file on USB containing private key', env_var='KEY_FILE')
     p.add_argument('--unsigned_certificates_dir', default=os.path.join(DATA_PATH, 'unsigned_certificates'),
                    help='Default path to data directory storing unsigned certs', env_var='UNSIGNED_CERTIFICATES_DIR')
     p.add_argument('--signed_certificates_dir', default=os.path.join(DATA_PATH, 'signed_certificates'),
                    help='Default path to data directory storing signed certs', env_var='SIGNED_CERTIFICATES_DIR')
@@ -65,16 +65,20 @@
     p.add_argument('--satoshi_per_byte', default=250,
                    type=int, help='Satoshi per byte', env_var='SATOSHI_PER_BYTE')
     p.add_argument('--bitcoind', dest='bitcoind', default=False, action='store_true',
                    help='Use bitcoind connectors.', env_var='BITCOIND')
     p.add_argument('--no_bitcoind', dest='bitcoind', default=True, action='store_false',
                    help='Default; do not use bitcoind connectors; use APIs instead', env_var='NO_BITCOIND')
     # ethereum arguments
+    p.add_argument('--nonce', default=0, type=int,
+                   help='sets nonce of ETH transaction. useful if you run your own transaction management system.', env_var='NONCE')
+    p.add_argument('--max_priority_fee_per_gas', default=0, type=int,
+                   help='decide the priority fee per gas spent for EIP-1559-compliant transactions (in wei, the smallest ETH unit)', env_var='MAX_PRIORITY_FEE_PER_GAS')
     p.add_argument('--gas_price', default=20000000000, type=int,
-                   help='decide the price per gas spent (in wei (smallest ETH unit))', env_var='GAS_PRICE')
+                   help='decide the price per gas spent. sets max_fee_per_gas for EIP-1559-compliant transactions.', env_var='GAS_PRICE')
     p.add_argument('--gas_limit', default=25000, type=int,
                    help='decide on the maximum spendable gas. gas_limit < 25000 might not be sufficient', env_var='GAS_LIMIT')
     p.add_argument('--etherscan_api_token', default=None, type=str,
                    help='The API token of the Etherscan broadcaster', env_var='ETHERSCAN_API_TOKEN')
     p.add_argument('--ethereum_rpc_url', default=None, type=str,
                    help='The URL of an Ethereum main net RPC node - useful in the case of third-party full node vendors.',
                    env_var='ETHEREUM_RPC_URL')
```

### Comparing `cert-issuer-3.3.0/cert_issuer.egg-info/SOURCES.txt` & `cert-issuer-3.4.0/cert_issuer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.3.0/cert_issuer.egg-info/PKG-INFO` & `cert-issuer-3.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,8 @@
-Metadata-Version: 2.1
-Name: cert-issuer
-Version: 3.3.0
-Summary: Issues blockchain certificates using the Bitcoin blockchain
-Home-page: https://github.com/blockchain-certificates/cert-issuer
-Author: Blockcerts
-Author-email: info@blockcerts.org
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
+[![Verifiable Credential Compliance result](https://badgen.net/badge/Verifiable%20Credentials%20v1/compliant/green?icon=https://www.w3.org/Icons/WWW/w3c_home_nb-v.svg)](https://github.com/blockchain-certificates/cert-issuer/vc-compliance-report.html)
 [![Build Status](https://travis-ci.org/blockchain-certificates/cert-issuer.svg?branch=master)](https://travis-ci.org/blockchain-certificates/cert-issuer)
 [![PyPI version](https://badge.fury.io/py/cert-issuer.svg)](https://badge.fury.io/py/cert-issuer)
 
 # cert-issuer
 
 The cert-issuer project issues blockchain certificates by creating a transaction from the issuing institution to the
 recipient on the Bitcoin or Ethereum blockchains. That transaction includes the hash of the certificate itself.
@@ -434,9 +423,7 @@
       file not found
 #include <openssl/aes.h>
 ```
 
 # Contact
 
 Contact us at [the Blockcerts community forum](http://community.blockcerts.org/).
-
-
```

### Comparing `cert-issuer-3.3.0/PKG-INFO` & `cert-issuer-3.4.0/cert_issuer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: cert-issuer
-Version: 3.3.0
+Version: 3.4.0
 Summary: Issues blockchain certificates using the Bitcoin blockchain
 Home-page: https://github.com/blockchain-certificates/cert-issuer
 Author: Blockcerts
 Author-email: info@blockcerts.org
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Verifiable Credential Compliance result](https://badgen.net/badge/Verifiable%20Credentials%20v1/compliant/green?icon=https://www.w3.org/Icons/WWW/w3c_home_nb-v.svg)](https://github.com/blockchain-certificates/cert-issuer/vc-compliance-report.html)
 [![Build Status](https://travis-ci.org/blockchain-certificates/cert-issuer.svg?branch=master)](https://travis-ci.org/blockchain-certificates/cert-issuer)
 [![PyPI version](https://badge.fury.io/py/cert-issuer.svg)](https://badge.fury.io/py/cert-issuer)
 
 # cert-issuer
 
 The cert-issuer project issues blockchain certificates by creating a transaction from the issuing institution to the
 recipient on the Bitcoin or Ethereum blockchains. That transaction includes the hash of the certificate itself.
```

### Comparing `cert-issuer-3.3.0/LICENSE` & `cert-issuer-3.4.0/LICENSE`

 * *Files identical despite different names*

