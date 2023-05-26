# Comparing `tmp/jupyter_ai_magics-0.7.2.tar.gz` & `tmp/jupyter_ai_magics-0.7.3.tar.gz`

## Comparing `jupyter_ai_magics-0.7.2.tar` & `jupyter_ai_magics-0.7.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/setup.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/_version.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/aliases.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/embedding_providers.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/exception.py
--rw-r--r--   0        0        0    14995 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/magics.py
--rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/providers.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/tests/__init__.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/LICENSE
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/README.md
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/setup.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/_version.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/aliases.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/embedding_providers.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/exception.py
+-rw-r--r--   0        0        0    14995 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/magics.py
+-rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/providers.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/tests/__init__.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/LICENSE
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/README.md
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/PKG-INFO
```

### Comparing `jupyter_ai_magics-0.7.2/package.json` & `jupyter_ai_magics-0.7.3/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.7.3'"}*

```diff
@@ -16,9 +16,9 @@
         "type": "git",
         "url": "https://github.com/jupyterlab/jupyter-ai.git"
     },
     "scripts": {
         "dev-install": "pip install -e \".[all]\"",
         "dev-uninstall": "pip uninstall jupyter_ai_magics -y"
     },
-    "version": "0.7.2"
+    "version": "0.7.3"
 }
```

### Comparing `jupyter_ai_magics-0.7.2/jupyter_ai_magics/__init__.py` & `jupyter_ai_magics-0.7.3/jupyter_ai_magics/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.2/jupyter_ai_magics/embedding_providers.py` & `jupyter_ai_magics-0.7.3/jupyter_ai_magics/embedding_providers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.2/jupyter_ai_magics/exception.py` & `jupyter_ai_magics-0.7.3/jupyter_ai_magics/exception.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.2/jupyter_ai_magics/magics.py` & `jupyter_ai_magics-0.7.3/jupyter_ai_magics/magics.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.2/jupyter_ai_magics/providers.py` & `jupyter_ai_magics-0.7.3/jupyter_ai_magics/providers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.2/jupyter_ai_magics/utils.py` & `jupyter_ai_magics-0.7.3/jupyter_ai_magics/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.2/.gitignore` & `jupyter_ai_magics-0.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.2/LICENSE` & `jupyter_ai_magics-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.2/pyproject.toml` & `jupyter_ai_magics-0.7.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 requires = ["hatchling>=1.4.0", "hatch-nodejs-version"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyter_ai_magics"
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Framework :: Jupyter",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 dependencies = [
     "ipython",
     "pydantic",
     "importlib_metadata~=5.2.0",
-    "langchain==0.0.158"
+    "langchain==0.0.159",
+    "typing_extensions==4.5.0"
 ]
 
 [project.optional-dependencies]
 test = [
     "coverage",
     "pytest",
     "pytest-asyncio",
```

### Comparing `jupyter_ai_magics-0.7.2/PKG-INFO` & `jupyter_ai_magics-0.7.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai_magics
-Version: 0.7.2
+Version: 0.7.3
 Summary: Jupyter AI magics Python package. Not published on NPM.
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -36,24 +36,24 @@
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
 Classifier: Framework :: Jupyter
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: importlib-metadata~=5.2.0
 Requires-Dist: ipython
-Requires-Dist: langchain==0.0.158
+Requires-Dist: langchain==0.0.159
 Requires-Dist: pydantic
+Requires-Dist: typing-extensions==4.5.0
 Provides-Extra: all
 Requires-Dist: ai21; extra == 'all'
 Requires-Dist: anthropic; extra == 'all'
 Requires-Dist: boto3; extra == 'all'
 Requires-Dist: cohere; extra == 'all'
 Requires-Dist: huggingface-hub; extra == 'all'
 Requires-Dist: ipywidgets; extra == 'all'
```

