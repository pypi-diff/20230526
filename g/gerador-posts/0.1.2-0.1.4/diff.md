# Comparing `tmp/gerador_posts-0.1.2.tar.gz` & `tmp/gerador_posts-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerador_posts-0.1.2.tar", last modified: Fri May 26 13:01:35 2023, max compression
+gzip compressed data, was "gerador_posts-0.1.4.tar", last modified: Fri May 26 14:57:44 2023, max compression
```

## Comparing `gerador_posts-0.1.2.tar` & `gerador_posts-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ufpe      (1000) ufpe      (1000)        0 2023-05-26 13:01:35.979340 gerador_posts-0.1.2/
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)     1076 2023-05-25 13:15:36.000000 gerador_posts-0.1.2/LICENSE
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)     1386 2023-05-26 13:01:35.979340 gerador_posts-0.1.2/PKG-INFO
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)     1001 2023-05-26 12:55:14.000000 gerador_posts-0.1.2/README.md
-drwxrwxr-x   0 ufpe      (1000) ufpe      (1000)        0 2023-05-26 13:01:35.979340 gerador_posts-0.1.2/gerador_posts/
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)        0 2023-05-25 17:56:44.000000 gerador_posts-0.1.2/gerador_posts/__init__.py
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)       86 2023-05-25 19:58:03.000000 gerador_posts-0.1.2/gerador_posts/__main__.py
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)     1189 2023-05-25 17:08:30.000000 gerador_posts-0.1.2/gerador_posts/configuracao.py
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)      420 2023-05-26 12:57:07.000000 gerador_posts-0.1.2/gerador_posts/gerador_posts.py
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)      831 2023-05-25 18:29:15.000000 gerador_posts-0.1.2/gerador_posts/tratar_dados.py
-drwxrwxr-x   0 ufpe      (1000) ufpe      (1000)        0 2023-05-26 13:01:35.979340 gerador_posts-0.1.2/gerador_posts.egg-info/
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)     1386 2023-05-26 13:01:35.000000 gerador_posts-0.1.2/gerador_posts.egg-info/PKG-INFO
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)      429 2023-05-26 13:01:35.000000 gerador_posts-0.1.2/gerador_posts.egg-info/SOURCES.txt
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)        1 2023-05-26 13:01:35.000000 gerador_posts-0.1.2/gerador_posts.egg-info/dependency_links.txt
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)       74 2023-05-26 13:01:35.000000 gerador_posts-0.1.2/gerador_posts.egg-info/entry_points.txt
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)        1 2023-05-25 19:32:41.000000 gerador_posts-0.1.2/gerador_posts.egg-info/not-zip-safe
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)       44 2023-05-26 13:01:35.000000 gerador_posts-0.1.2/gerador_posts.egg-info/requires.txt
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)       14 2023-05-26 13:01:35.000000 gerador_posts-0.1.2/gerador_posts.egg-info/top_level.txt
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)       38 2023-05-26 13:01:35.979340 gerador_posts-0.1.2/setup.cfg
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)     1032 2023-05-26 12:59:44.000000 gerador_posts-0.1.2/setup.py
+drwxrwxr-x   0 ufpe      (1000) ufpe      (1000)        0 2023-05-26 14:57:44.783451 gerador_posts-0.1.4/
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)     1076 2023-05-26 14:45:00.000000 gerador_posts-0.1.4/LICENSE
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)     1712 2023-05-26 14:57:44.783451 gerador_posts-0.1.4/PKG-INFO
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)     1302 2023-05-26 14:47:30.000000 gerador_posts-0.1.4/README.md
+drwxrwxr-x   0 ufpe      (1000) ufpe      (1000)        0 2023-05-26 14:57:44.783451 gerador_posts-0.1.4/gerador_posts/
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)        0 2023-05-26 14:45:00.000000 gerador_posts-0.1.4/gerador_posts/__init__.py
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)       86 2023-05-26 14:45:00.000000 gerador_posts-0.1.4/gerador_posts/__main__.py
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)     1189 2023-05-26 14:45:00.000000 gerador_posts-0.1.4/gerador_posts/configuracao.py
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)      420 2023-05-26 14:45:00.000000 gerador_posts-0.1.4/gerador_posts/gerador_posts.py
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)      831 2023-05-26 14:45:00.000000 gerador_posts-0.1.4/gerador_posts/tratar_dados.py
+drwxrwxr-x   0 ufpe      (1000) ufpe      (1000)        0 2023-05-26 14:57:44.783451 gerador_posts-0.1.4/gerador_posts.egg-info/
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)     1712 2023-05-26 14:57:44.000000 gerador_posts-0.1.4/gerador_posts.egg-info/PKG-INFO
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)      429 2023-05-26 14:57:44.000000 gerador_posts-0.1.4/gerador_posts.egg-info/SOURCES.txt
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)        1 2023-05-26 14:57:44.000000 gerador_posts-0.1.4/gerador_posts.egg-info/dependency_links.txt
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)       74 2023-05-26 14:57:44.000000 gerador_posts-0.1.4/gerador_posts.egg-info/entry_points.txt
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)        1 2023-05-26 14:57:44.000000 gerador_posts-0.1.4/gerador_posts.egg-info/not-zip-safe
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)       44 2023-05-26 14:57:44.000000 gerador_posts-0.1.4/gerador_posts.egg-info/requires.txt
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)       14 2023-05-26 14:57:44.000000 gerador_posts-0.1.4/gerador_posts.egg-info/top_level.txt
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)       38 2023-05-26 14:57:44.783451 gerador_posts-0.1.4/setup.cfg
+-rw-rw-r--   0 ufpe      (1000) ufpe      (1000)      899 2023-05-26 14:51:56.000000 gerador_posts-0.1.4/setup.py
```

### Comparing `gerador_posts-0.1.2/LICENSE` & `gerador_posts-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gerador_posts-0.1.2/PKG-INFO` & `gerador_posts-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 Metadata-Version: 2.1
 Name: gerador_posts
-Version: 0.1.2
-Summary: Gerador de posts baseado em templates e dados 
+Version: 0.1.4
+Summary: Gerador de posts baseado em templates e arquivos de dados (csv e yaml).
 Home-page: https://github.com/cecivieira/gerador-posts
 Author: Ana Cecília Vieira
 Author-email: cecivieira@gmail.com
 License: MIT
 Keywords: jinja2,yaml,templates
 Platform: UNKNOWN
 Requires-Python: >=3.10.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Gerador de posts
-Gerador de posts baseado em templates e dados armazenados em arquivo csv.
+Gerador de posts baseado em templates e dados armazenados em arquivos de dados (csv e yaml).
 
 Essa aplicação surgiu da necessidade de gerar textos a partir de um template, cujos dados deveriam ser coletados de um arquivo .csv e .yaml. Então, é isso que esse programa faz: ler dados de um arquivo .csv, outros dados de um arquivo .yaml e preenche um ou mais templates.
 
 ## Instalação
 
 ```bash
 (.venv) $ pip install gerador-posts
 ```
 
 ## Uso
 
-1. Crie os dados:
+1. Crie os arquivos de dados:
     1. Crie a pasta `./dados`;
     1. Dentro dessa pasta, crie dois arquivos de dados: `links.csv` e `variaveis.yaml` (os arquivos devem ter exatamente esses títulos).
-1. Crie os templates:
+1. Escreva os templates:
     1. Crie a pasta `./posts_templates`;
-    1. Dentro dessa pasta você pode criar quantos templates desejar, em qualquer formato de arquivo. (para inserir dados no template use a sintaxe do Jinja2).
+    1. Dentro dessa pasta você pode criar quantos templates desejar, em qualquer formato de arquivo. (para inserir os dados no template use a sintaxe do Jinja2).
 1. Crie a pasta aonde os posts prontos serão armazenados: `./posts_prontos`;
 1. Execute o pacote:
     ```bash
     (.venv) $ gerar-posts
     ```
+1. Feito! Seus posts estão prontos e armazenados na pasta `./posts_prontos`.
+
+## Exemplos
+
+Você pode encontrar alguns exemplos de uso desse pacote em: [https://github.com/cecivieira/gerador-posts-exemplos](https://github.com/cecivieira/gerador-posts-exemplos) .
```

### Comparing `gerador_posts-0.1.2/README.md` & `gerador_posts-0.1.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # Gerador de posts
-Gerador de posts baseado em templates e dados armazenados em arquivo csv.
+Gerador de posts baseado em templates e dados armazenados em arquivos de dados (csv e yaml).
 
 Essa aplicação surgiu da necessidade de gerar textos a partir de um template, cujos dados deveriam ser coletados de um arquivo .csv e .yaml. Então, é isso que esse programa faz: ler dados de um arquivo .csv, outros dados de um arquivo .yaml e preenche um ou mais templates.
 
 ## Instalação
 
 ```bash
 (.venv) $ pip install gerador-posts
 ```
 
 ## Uso
 
-1. Crie os dados:
+1. Crie os arquivos de dados:
     1. Crie a pasta `./dados`;
     1. Dentro dessa pasta, crie dois arquivos de dados: `links.csv` e `variaveis.yaml` (os arquivos devem ter exatamente esses títulos).
-1. Crie os templates:
+1. Escreva os templates:
     1. Crie a pasta `./posts_templates`;
-    1. Dentro dessa pasta você pode criar quantos templates desejar, em qualquer formato de arquivo. (para inserir dados no template use a sintaxe do Jinja2).
+    1. Dentro dessa pasta você pode criar quantos templates desejar, em qualquer formato de arquivo. (para inserir os dados no template use a sintaxe do Jinja2).
 1. Crie a pasta aonde os posts prontos serão armazenados: `./posts_prontos`;
 1. Execute o pacote:
     ```bash
     (.venv) $ gerar-posts
-    ```
+    ```
+1. Feito! Seus posts estão prontos e armazenados na pasta `./posts_prontos`.
+
+## Exemplos
+
+Você pode encontrar alguns exemplos de uso desse pacote em: [https://github.com/cecivieira/gerador-posts-exemplos](https://github.com/cecivieira/gerador-posts-exemplos) .
```

### Comparing `gerador_posts-0.1.2/gerador_posts/configuracao.py` & `gerador_posts-0.1.4/gerador_posts/configuracao.py`

 * *Files identical despite different names*

### Comparing `gerador_posts-0.1.2/gerador_posts/tratar_dados.py` & `gerador_posts-0.1.4/gerador_posts/tratar_dados.py`

 * *Files identical despite different names*

### Comparing `gerador_posts-0.1.2/gerador_posts.egg-info/PKG-INFO` & `gerador_posts-0.1.4/gerador_posts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 Metadata-Version: 2.1
 Name: gerador-posts
-Version: 0.1.2
-Summary: Gerador de posts baseado em templates e dados 
+Version: 0.1.4
+Summary: Gerador de posts baseado em templates e arquivos de dados (csv e yaml).
 Home-page: https://github.com/cecivieira/gerador-posts
 Author: Ana Cecília Vieira
 Author-email: cecivieira@gmail.com
 License: MIT
 Keywords: jinja2,yaml,templates
 Platform: UNKNOWN
 Requires-Python: >=3.10.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Gerador de posts
-Gerador de posts baseado em templates e dados armazenados em arquivo csv.
+Gerador de posts baseado em templates e dados armazenados em arquivos de dados (csv e yaml).
 
 Essa aplicação surgiu da necessidade de gerar textos a partir de um template, cujos dados deveriam ser coletados de um arquivo .csv e .yaml. Então, é isso que esse programa faz: ler dados de um arquivo .csv, outros dados de um arquivo .yaml e preenche um ou mais templates.
 
 ## Instalação
 
 ```bash
 (.venv) $ pip install gerador-posts
 ```
 
 ## Uso
 
-1. Crie os dados:
+1. Crie os arquivos de dados:
     1. Crie a pasta `./dados`;
     1. Dentro dessa pasta, crie dois arquivos de dados: `links.csv` e `variaveis.yaml` (os arquivos devem ter exatamente esses títulos).
-1. Crie os templates:
+1. Escreva os templates:
     1. Crie a pasta `./posts_templates`;
-    1. Dentro dessa pasta você pode criar quantos templates desejar, em qualquer formato de arquivo. (para inserir dados no template use a sintaxe do Jinja2).
+    1. Dentro dessa pasta você pode criar quantos templates desejar, em qualquer formato de arquivo. (para inserir os dados no template use a sintaxe do Jinja2).
 1. Crie a pasta aonde os posts prontos serão armazenados: `./posts_prontos`;
 1. Execute o pacote:
     ```bash
     (.venv) $ gerar-posts
     ```
+1. Feito! Seus posts estão prontos e armazenados na pasta `./posts_prontos`.
+
+## Exemplos
+
+Você pode encontrar alguns exemplos de uso desse pacote em: [https://github.com/cecivieira/gerador-posts-exemplos](https://github.com/cecivieira/gerador-posts-exemplos) .
```

