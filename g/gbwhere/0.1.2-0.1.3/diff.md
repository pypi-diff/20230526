# Comparing `tmp/gbwhere-0.1.2.tar.gz` & `tmp/gbwhere-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbwhere-0.1.2.tar", max compression
+gzip compressed data, was "gbwhere-0.1.3.tar", max compression
```

## Comparing `gbwhere-0.1.2.tar` & `gbwhere-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1218 2023-05-26 00:05:24.372830 gbwhere-0.1.2/README.md
--rw-r--r--   0        0        0      390 2023-05-26 00:05:49.612660 gbwhere-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      245 2023-05-25 22:20:14.815199 gbwhere-0.1.2/where/cli.py
--rw-r--r--   0        0        0      327 2023-05-25 21:02:29.222307 gbwhere-0.1.2/where/exceptions.py
--rw-r--r--   0        0        0     3494 2023-05-25 22:09:28.355512 gbwhere-0.1.2/where/finder.py
--rw-r--r--   0        0        0     3490 2023-05-25 22:22:17.738380 gbwhere-0.1.2/where/utils.py
--rw-r--r--   0        0        0     1638 1970-01-01 00:00:00.000000 gbwhere-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1184 2023-05-26 00:07:21.780038 gbwhere-0.1.3/README.md
+-rw-r--r--   0        0        0      390 2023-05-26 00:07:29.679985 gbwhere-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      245 2023-05-25 22:20:14.815199 gbwhere-0.1.3/where/cli.py
+-rw-r--r--   0        0        0      327 2023-05-25 21:02:29.222307 gbwhere-0.1.3/where/exceptions.py
+-rw-r--r--   0        0        0     3494 2023-05-25 22:09:28.355512 gbwhere-0.1.3/where/finder.py
+-rw-r--r--   0        0        0     3490 2023-05-25 22:22:17.738380 gbwhere-0.1.3/where/utils.py
+-rw-r--r--   0        0        0     1604 1970-01-01 00:00:00.000000 gbwhere-0.1.3/PKG-INFO
```

### Comparing `gbwhere-0.1.2/README.md` & `gbwhere-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 ## Pré-requisitos
 
 - Python (3.x)
 - pip
 
 ## Instalação
 Tendo Python e o pip em sua máquina, basta executar pip install gbwhere
-https://pypi.org/project/gbwhere/
 
 ## Uso
 Execute o script principal: gbwhere --help.
 Siga as instruções exibidas no console para inserir os critérios de busca desejados.
 Aguarde o processamento e visualize os resultados exibidos.
 
 ## Contribuição
```

### Comparing `gbwhere-0.1.2/where/finder.py` & `gbwhere-0.1.3/where/finder.py`

 * *Files identical despite different names*

### Comparing `gbwhere-0.1.2/where/utils.py` & `gbwhere-0.1.3/where/utils.py`

 * *Files identical despite different names*

### Comparing `gbwhere-0.1.2/PKG-INFO` & `gbwhere-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbwhere
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: rdsgabriel
 Author-email: rdsgabriel.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -25,15 +25,14 @@
 ## Pré-requisitos
 
 - Python (3.x)
 - pip
 
 ## Instalação
 Tendo Python e o pip em sua máquina, basta executar pip install gbwhere
-https://pypi.org/project/gbwhere/
 
 ## Uso
 Execute o script principal: gbwhere --help.
 Siga as instruções exibidas no console para inserir os critérios de busca desejados.
 Aguarde o processamento e visualize os resultados exibidos.
 
 ## Contribuição
```

