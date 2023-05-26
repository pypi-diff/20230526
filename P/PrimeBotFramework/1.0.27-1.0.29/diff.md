# Comparing `tmp/PrimeBotFramework-1.0.27.tar.gz` & `tmp/PrimeBotFramework-1.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-yvgw175j/PrimeBotFramework-1.0.27.tar", last modified: Fri May 26 16:58:57 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-l5_6bmd5/PrimeBotFramework-1.0.29.tar", last modified: Fri May 26 17:21:26 2023, max compression
```

## Comparing `PrimeBotFramework-1.0.27.tar` & `PrimeBotFramework-1.0.29.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 16:58:57.006805 PrimeBotFramework-1.0.27/
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-05-26 16:58:57.010805 PrimeBotFramework-1.0.27/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 16:58:57.006805 PrimeBotFramework-1.0.27/PrimeBot/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 16:58:57.006805 PrimeBotFramework-1.0.27/PrimeBot/B2E/
--rw-rw-rw-   0 root         (0) root         (0)     4028 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/PrimeBot/B2E/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 16:58:57.006805 PrimeBotFramework-1.0.27/PrimeBot/Cnab750V1/
--rw-rw-rw-   0 root         (0) root         (0)    10035 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/PrimeBot/Cnab750V1/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 16:58:57.006805 PrimeBotFramework-1.0.27/PrimeBot/CpfCnpj/
--rw-rw-rw-   0 root         (0) root         (0)     1963 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/PrimeBot/CpfCnpj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/PrimeBot/CpfCnpj/api_codes.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/PrimeBot/CpfCnpj/model.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 16:58:57.006805 PrimeBotFramework-1.0.27/PrimeBot/D4Sign/
--rw-rw-rw-   0 root         (0) root         (0)     2600 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/PrimeBot/D4Sign/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 16:58:57.006805 PrimeBotFramework-1.0.27/PrimeBot/DeathByCaptcha/
--rw-rw-rw-   0 root         (0) root         (0)     2822 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/PrimeBot/DeathByCaptcha/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 16:58:57.006805 PrimeBotFramework-1.0.27/PrimeBot/Documents/
--rw-rw-rw-   0 root         (0) root         (0)     1098 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/PrimeBot/Documents/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 16:58:57.006805 PrimeBotFramework-1.0.27/PrimeBot/Elastic/
--rw-rw-rw-   0 root         (0) root         (0)     1239 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/PrimeBot/Elastic/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 16:58:57.006805 PrimeBotFramework-1.0.27/PrimeBot/ExchangeGraph/
--rw-rw-rw-   0 root         (0) root         (0)     8987 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/PrimeBot/ExchangeGraph/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 16:58:57.006805 PrimeBotFramework-1.0.27/PrimeBot/IntegracaoSendGrid/
--rw-rw-rw-   0 root         (0) root         (0)     4251 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/PrimeBot/IntegracaoSendGrid/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 16:58:57.006805 PrimeBotFramework-1.0.27/PrimeBot/ListenerECS/
--rw-rw-rw-   0 root         (0) root         (0)     4096 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/PrimeBot/ListenerECS/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 16:58:57.006805 PrimeBotFramework-1.0.27/PrimeBot/Mongo/
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/PrimeBot/Mongo/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 16:58:57.006805 PrimeBotFramework-1.0.27/PrimeBot/OracleDB/
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/PrimeBot/OracleDB/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 16:58:57.006805 PrimeBotFramework-1.0.27/PrimeBot/Vault/
--rw-rw-rw-   0 root         (0) root         (0)     2740 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/PrimeBot/Vault/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/PrimeBot/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 16:58:57.010805 PrimeBotFramework-1.0.27/PrimeBotFramework.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-05-26 16:58:56.000000 PrimeBotFramework-1.0.27/PrimeBotFramework.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      709 2023-05-26 16:58:57.000000 PrimeBotFramework-1.0.27/PrimeBotFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-26 16:58:56.000000 PrimeBotFramework-1.0.27/PrimeBotFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-26 16:58:56.000000 PrimeBotFramework-1.0.27/PrimeBotFramework.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-26 16:58:56.000000 PrimeBotFramework-1.0.27/PrimeBotFramework.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-26 16:58:57.010805 PrimeBotFramework-1.0.27/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-05-26 16:58:47.000000 PrimeBotFramework-1.0.27/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/B2E/
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/B2E/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/Cnab750/
+-rw-rw-rw-   0 root         (0) root         (0)    10033 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/Cnab750/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/CpfCnpj/
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/CpfCnpj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/CpfCnpj/api_codes.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/CpfCnpj/model.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/D4Sign/
+-rw-rw-rw-   0 root         (0) root         (0)     2600 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/D4Sign/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/DeathByCaptcha/
+-rw-rw-rw-   0 root         (0) root         (0)     2822 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/DeathByCaptcha/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/Documents/
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/Documents/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/Elastic/
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/Elastic/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/ExchangeGraph/
+-rw-rw-rw-   0 root         (0) root         (0)     8987 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/ExchangeGraph/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/IntegracaoSendGrid/
+-rw-rw-rw-   0 root         (0) root         (0)     4251 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/IntegracaoSendGrid/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/ListenerECS/
+-rw-rw-rw-   0 root         (0) root         (0)     4096 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/ListenerECS/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/Mongo/
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/Mongo/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/OracleDB/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/OracleDB/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/Vault/
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/Vault/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBotFramework.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-05-26 17:21:26.000000 PrimeBotFramework-1.0.29/PrimeBotFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      707 2023-05-26 17:21:26.000000 PrimeBotFramework-1.0.29/PrimeBotFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-26 17:21:26.000000 PrimeBotFramework-1.0.29/PrimeBotFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-26 17:21:26.000000 PrimeBotFramework-1.0.29/PrimeBotFramework.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-26 17:21:26.000000 PrimeBotFramework-1.0.29/PrimeBotFramework.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-26 17:21:26.865454 PrimeBotFramework-1.0.29/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/setup.py
```

### Comparing `PrimeBotFramework-1.0.27/PKG-INFO` & `PrimeBotFramework-1.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.27
+Version: 1.0.29
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PrimeBotFramework-1.0.27/PrimeBot/B2E/__init__.py` & `PrimeBotFramework-1.0.29/PrimeBot/B2E/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.27/PrimeBot/Cnab750V1/__init__.py` & `PrimeBotFramework-1.0.29/PrimeBot/Cnab750/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-class Cnab750V1():
+class Cnab750():
     """
         Métodos de leitura de dados do CNAB 750 - Pagamentos Instantâneos
     """
 
     def retornar_arquivos_diretorio(self, caminho_diretorio: str) -> list:
         """Retorna os arquivos de um diretorio
```

### Comparing `PrimeBotFramework-1.0.27/PrimeBot/CpfCnpj/__init__.py` & `PrimeBotFramework-1.0.29/PrimeBot/CpfCnpj/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.27/PrimeBot/CpfCnpj/api_codes.py` & `PrimeBotFramework-1.0.29/PrimeBot/CpfCnpj/api_codes.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.27/PrimeBot/D4Sign/__init__.py` & `PrimeBotFramework-1.0.29/PrimeBot/D4Sign/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.27/PrimeBot/DeathByCaptcha/__init__.py` & `PrimeBotFramework-1.0.29/PrimeBot/DeathByCaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.27/PrimeBot/Documents/__init__.py` & `PrimeBotFramework-1.0.29/PrimeBot/Documents/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.27/PrimeBot/Elastic/__init__.py` & `PrimeBotFramework-1.0.29/PrimeBot/Elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.27/PrimeBot/ExchangeGraph/__init__.py` & `PrimeBotFramework-1.0.29/PrimeBot/ExchangeGraph/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.27/PrimeBot/IntegracaoSendGrid/__init__.py` & `PrimeBotFramework-1.0.29/PrimeBot/IntegracaoSendGrid/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.27/PrimeBot/ListenerECS/__init__.py` & `PrimeBotFramework-1.0.29/PrimeBot/ListenerECS/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.27/PrimeBot/OracleDB/__init__.py` & `PrimeBotFramework-1.0.29/PrimeBot/OracleDB/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.27/PrimeBot/Vault/__init__.py` & `PrimeBotFramework-1.0.29/PrimeBot/Vault/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.27/PrimeBotFramework.egg-info/PKG-INFO` & `PrimeBotFramework-1.0.29/PrimeBotFramework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.27
+Version: 1.0.29
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PrimeBotFramework-1.0.27/PrimeBotFramework.egg-info/SOURCES.txt` & `PrimeBotFramework-1.0.29/PrimeBotFramework.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 PKG-INFO
 setup.cfg
 setup.py
 PrimeBot/__init__.py
 PrimeBot/B2E/__init__.py
-PrimeBot/Cnab750V1/__init__.py
+PrimeBot/Cnab750/__init__.py
 PrimeBot/CpfCnpj/__init__.py
 PrimeBot/CpfCnpj/api_codes.py
 PrimeBot/CpfCnpj/model.py
 PrimeBot/D4Sign/__init__.py
 PrimeBot/DeathByCaptcha/__init__.py
 PrimeBot/Documents/__init__.py
 PrimeBot/Elastic/__init__.py
```

### Comparing `PrimeBotFramework-1.0.27/setup.py` & `PrimeBotFramework-1.0.29/setup.py`

 * *Files identical despite different names*

