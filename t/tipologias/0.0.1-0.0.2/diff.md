# Comparing `tmp/tipologias-0.0.1.tar.gz` & `tmp/tipologias-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tipologias-0.0.1.tar", last modified: Mon May 22 19:02:53 2023, max compression
+gzip compressed data, was "tipologias-0.0.2.tar", last modified: Fri May 26 11:55:45 2023, max compression
```

## Comparing `tipologias-0.0.1.tar` & `tipologias-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 19:02:53.407135 tipologias-0.0.1/
--rw-rw-rw-   0        0        0     1511 2023-05-22 15:06:17.000000 tipologias-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      719 2023-05-22 19:02:53.406134 tipologias-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       85 2023-05-22 15:07:16.000000 tipologias-0.0.1/README.md
--rw-rw-rw-   0        0        0     1557 2023-05-22 19:02:39.000000 tipologias-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-22 19:02:53.408135 tipologias-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-22 19:02:53.380135 tipologias-0.0.1/tests/
--rw-rw-rw-   0        0        0      372 2023-05-22 18:28:51.000000 tipologias-0.0.1/tests/test_socio_comum.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:02:53.383136 tipologias-0.0.1/tipologias/
--rw-rw-rw-   0        0        0        0 2023-05-22 14:54:23.000000 tipologias-0.0.1/tipologias/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:02:53.400135 tipologias-0.0.1/tipologias/core/
--rw-rw-rw-   0        0        0        0 2023-05-22 14:54:23.000000 tipologias-0.0.1/tipologias/core/__init__.py
--rw-rw-rw-   0        0        0     1269 2023-05-02 19:14:25.000000 tipologias-0.0.1/tipologias/core/base.py
--rw-rw-rw-   0        0        0     2635 2023-05-22 18:04:22.000000 tipologias-0.0.1/tipologias/core/socios_comum.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:02:53.404133 tipologias-0.0.1/tipologias/queries/
--rw-rw-rw-   0        0        0        0 2023-05-22 18:30:01.000000 tipologias-0.0.1/tipologias/queries/__init__.py
--rw-rw-rw-   0        0        0      728 2023-05-22 17:44:30.000000 tipologias-0.0.1/tipologias/queries/socios.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:02:53.394134 tipologias-0.0.1/tipologias.egg-info/
--rw-rw-rw-   0        0        0      719 2023-05-22 19:02:53.000000 tipologias-0.0.1/tipologias.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-05-22 19:02:53.000000 tipologias-0.0.1/tipologias.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 19:02:53.000000 tipologias-0.0.1/tipologias.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2023-05-22 19:02:53.000000 tipologias-0.0.1/tipologias.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 19:02:53.000000 tipologias-0.0.1/tipologias.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 11:55:45.738488 tipologias-0.0.2/
+-rw-rw-rw-   0        0        0     1511 2023-05-22 15:06:17.000000 tipologias-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      719 2023-05-26 11:55:45.737491 tipologias-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2023-05-22 15:07:16.000000 tipologias-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1704 2023-05-26 11:55:32.000000 tipologias-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 11:55:45.739490 tipologias-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 11:55:45.705488 tipologias-0.0.2/tipologias/
+-rw-rw-rw-   0        0        0        0 2023-05-22 14:54:23.000000 tipologias-0.0.2/tipologias/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:55:45.723489 tipologias-0.0.2/tipologias/core/
+-rw-rw-rw-   0        0        0        0 2023-05-22 14:54:23.000000 tipologias-0.0.2/tipologias/core/__init__.py
+-rw-rw-rw-   0        0        0     2229 2023-05-25 21:32:07.000000 tipologias-0.0.2/tipologias/core/base.py
+-rw-rw-rw-   0        0        0      571 2023-05-25 18:20:51.000000 tipologias-0.0.2/tipologias/core/participante_pregao.py
+-rw-rw-rw-   0        0        0     2110 2023-05-25 17:49:26.000000 tipologias-0.0.2/tipologias/core/socios_comum.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:55:45.729491 tipologias-0.0.2/tipologias/queries/
+-rw-rw-rw-   0        0        0        0 2023-05-22 18:30:01.000000 tipologias-0.0.2/tipologias/queries/__init__.py
+-rw-rw-rw-   0        0        0      374 2023-05-25 17:31:57.000000 tipologias-0.0.2/tipologias/queries/pregao.py
+-rw-rw-rw-   0        0        0      720 2023-05-25 17:46:26.000000 tipologias-0.0.2/tipologias/queries/socios.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:55:45.735491 tipologias-0.0.2/tipologias/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-22 18:30:01.000000 tipologias-0.0.2/tipologias/utils/__init__.py
+-rw-rw-rw-   0        0        0     1381 2023-05-25 21:31:33.000000 tipologias-0.0.2/tipologias/utils/asynchronous.py
+-rw-rw-rw-   0        0        0     3035 2023-05-26 11:28:00.000000 tipologias-0.0.2/tipologias/utils/padastools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:55:45.715489 tipologias-0.0.2/tipologias.egg-info/
+-rw-rw-rw-   0        0        0      719 2023-05-26 11:55:45.000000 tipologias-0.0.2/tipologias.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      529 2023-05-26 11:55:45.000000 tipologias-0.0.2/tipologias.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 11:55:45.000000 tipologias-0.0.2/tipologias.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      170 2023-05-26 11:55:45.000000 tipologias-0.0.2/tipologias.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 11:55:45.000000 tipologias-0.0.2/tipologias.egg-info/top_level.txt
```

### Comparing `tipologias-0.0.1/LICENSE` & `tipologias-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tipologias-0.0.1/PKG-INFO` & `tipologias-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tipologias
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pacote de tipologias para trilhas de auditoria do TCMRIO
 Author-email: Marciel Barcellos <marciel.barcellos@tcmrio.tc.br>, Nicolau Rodrigues <nicolau.rodrigues@tcmrio.tc.br>
 Project-URL: source, https://gitlab.com/tcmrj/tipologias
 Project-URL: Bug Tracker, https://gitlab.com/tcmrj/tipologias/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tipologias-0.0.1/pyproject.toml` & `tipologias-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tipologias"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Marciel Barcellos", email="marciel.barcellos@tcmrio.tc.br" },
   { name="Nicolau Rodrigues", email="nicolau.rodrigues@tcmrio.tc.br" },
 ]
 description = "Pacote de tipologias para trilhas de auditoria do TCMRIO"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -20,15 +20,16 @@
 
 dependencies = [
   'pandas == 1.5.3',
   'openpyxl == 3.1.2',
 ]
 
 [project.optional-dependencies]
-tests = [ 
+tests = [
+  'anyio == 3.6.2',
   'black == 23.3.0',
   'cryptography == 37.0.4',
   'isort == 5.12.0',
   'pyodbc == 4.0.32',
   'pytest == 7.3.1',
   'python-decouple == 3.6',
   'SQLAlchemy == 1.4.32',
@@ -64,7 +65,14 @@
 '''
 
 [tool.isort]
 profile = "black"
 skip_glob = ["docs/*"]
 multi_line_output = 3
 
+[tool.flake8]
+ignore = ['E231', 'E241']
+per-file-ignores = [
+    '__init__.py:F401',
+]
+max-line-length = 119
+count = true
```

### Comparing `tipologias-0.0.1/tipologias/core/socios_comum.py` & `tipologias-0.0.2/tipologias/core/socios_comum.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,49 @@
 from datetime import datetime
 
-import pandas as pd
-
-from tipologias.core.base import Tipologia
+from tipologias.core.base import BaseTipologia
 from tipologias.queries.socios import Q_LIST_SOCIO_CNPJ
 
 
-class SociosComum(Tipologia):
+class SociosComum(BaseTipologia):
     """Classe que implementa a tipologia SociosComum para analisar a ocorrência de sócios em comum entre cnpjs.
 
     Args:
-        lista_cnpjs (tuple): Uma lista de cnpjs para analisar.
+        cnpj_list (tuple): Uma lista de cnpjs para analisar.
 
     Attributes:
-        lista_cnpjs (tuple): Uma lista de cnpjs para analisar.
+        cnpj_list (tuple): Uma lista de cnpjs para analisar.
         df (pandas.DataFrame): O resultado da análise, armazenado em um DataFrame do pandas.
 
     Methods:
         input_data(): Extrai os dados necessários do banco de dados "big_data_cieg".
         processor(): Processa os dados extraídos e armazena o resultado em um DataFrame.
-        output_data(): Escreve o resultado da análise na tabela "trilhas_resposta_socios_comum" do banco de dados "default".
         execute(): Executa a análise completa.
     """
 
-    def __init__(self, engine, lista_cnpjs: list, data_entrada=None, data_saida=None) -> None:
+    def __init__(self, engine, cnpj_list: list[str], data_entrada=None, data_saida=None) -> None:
         """Inicializa a classe SociosComum com os parâmetros necessários.
 
         Args:
             crtl_analise_pregao_id (int): O ID da análise de pregão associada a essa tipologia.
             lista_pregoes (tuple): Uma lista de números de pregão para analisar.
         """
-        self.engine = engine
-        self.lista_cnpjs = lista_cnpjs
-        self.data_entrada = data_entrada if data_entrada else datetime.now().date()
-        self.data_saida = data_saida if data_saida else datetime.now().date()
-        self.df = None
-        self.processed_data = None
-        self.socios_comum = None
-        self.output_table = "trilhas_resposta_socios_comum"
-
+        self._engine = engine
+        self._cnpj_list = set(cnpj_list)
+        self._data_entrada = data_entrada or datetime.now().date()
+        self._data_saida = data_saida or datetime.now().date()
+        super().__init__(__class__.__name__)
 
     def input_data(self):
         query = Q_LIST_SOCIO_CNPJ.format(
-            lista_cnpjs="','".join(self.lista_cnpjs),
-            data_entrada=self.data_entrada,
-            data_saida=self.data_saida
-        )
-        self.df = pd.read_sql_query(
-            query,
-            self.engine
+            cnpj_list="','".join(self._cnpj_list), data_entrada=self._data_entrada, data_saida=self._data_saida
         )
+        self._df = self._pd.read_sql_query(query, self._engine)
 
     def processor(self):
-        self.socios_comum = pd.DataFrame()
-        for row in self.df.itertuples(name="Socio"):
-            df = self.df.query(
-                f'NUM_CNPJ_EMPRESA != "{row.NUM_CNPJ_EMPRESA}" and (NUM_CPF == "{row.NUM_CPF}" or NUM_CNPJ == "{row.NUM_CNPJ}")'
-            )
-            self.socios_comum = pd.concat([self.socios_comum, df], ignore_index=True)
-
-        self.df = self.socios_comum
-
-    def output_data(self):
-        return self.df
-
-    def execute(self):
-        self.input_data()
-        self.processor()
-        return self.output_data()
+        df_temp = self._pd.DataFrame()
+        for row in self._df.itertuples(name="Socio"):
+            query = f'NUM_CNPJ_EMPRESA != "{row.NUM_CNPJ_EMPRESA}" and (NUM_CPF == "{row.NUM_CPF}" or NUM_CNPJ == "{row.NUM_CNPJ}")'
+            df_query = self._df.query(query)
+            df_temp = self._pd.concat([df_temp, df_query], ignore_index=True)
+
+        self._df = df_temp
```

### Comparing `tipologias-0.0.1/tipologias.egg-info/PKG-INFO` & `tipologias-0.0.2/tipologias.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tipologias
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pacote de tipologias para trilhas de auditoria do TCMRIO
 Author-email: Marciel Barcellos <marciel.barcellos@tcmrio.tc.br>, Nicolau Rodrigues <nicolau.rodrigues@tcmrio.tc.br>
 Project-URL: source, https://gitlab.com/tcmrj/tipologias
 Project-URL: Bug Tracker, https://gitlab.com/tcmrj/tipologias/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

