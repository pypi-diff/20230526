# Comparing `tmp/laminci-0.5.3.tar.gz` & `tmp/laminci-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laminci-0.5.3.tar", last modified: Mon Apr 10 14:59:34 2023, max compression
+gzip compressed data, was "laminci-0.6.0.tar", last modified: Fri May 26 16:19:43 2023, max compression
```

## Comparing `laminci-0.5.3.tar` & `laminci-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.5.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.5.3/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.5.3/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.5.3/.gitignore
--rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.5.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.5.3/README.md
--rw-r--r--   0        0        0     2711 2023-04-10 14:59:15.965346 laminci-0.5.3/docs/changelog.md
--rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.5.3/docs/guide/index.md
--rw-r--r--   0        0        0     1415 2023-02-23 20:46:33.157438 laminci-0.5.3/docs/guide/quickstart.ipynb
--rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.5.3/docs/index.md
--rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.5.3/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
--rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.5.3/docs/notes/index.md
--rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.5.3/lamin-project.yaml
--rw-r--r--   0        0        0      378 2023-04-10 14:59:01.991275 laminci-0.5.3/laminci/__init__.py
--rw-r--r--   0        0        0     1413 2023-04-10 14:58:46.731399 laminci-0.5.3/laminci/_artifacts.py
--rw-r--r--   0        0        0     1794 2023-03-25 16:54:29.619400 laminci-0.5.3/laminci/_db.py
--rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.5.3/laminci/_docs.py
--rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.5.3/laminci/_env.py
--rw-r--r--   0        0        0     2423 2023-04-10 13:41:42.840205 laminci-0.5.3/laminci/_nox.py
--rw-r--r--   0        0        0      134 2023-02-23 21:55:02.625676 laminci-0.5.3/laminci/db.py
--rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.5.3/laminci/nox.py
--rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.5.3/noxfile.py
--rw-r--r--   0        0        0      694 2023-03-09 14:11:55.514326 laminci-0.5.3/pyproject.toml
--rw-r--r--   0        0        0       27 2023-02-23 21:02:08.742721 laminci-0.5.3/tests/test_base.py
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 laminci-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.6.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.6.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.6.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.6.0/README.md
+-rw-r--r--   0        0        0     3052 2023-05-26 16:19:25.148581 laminci-0.6.0/docs/changelog.md
+-rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.6.0/docs/guide/index.md
+-rw-r--r--   0        0        0     1415 2023-05-26 15:57:31.631988 laminci-0.6.0/docs/guide/quickstart.ipynb
+-rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.6.0/docs/index.md
+-rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.6.0/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
+-rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.6.0/docs/notes/index.md
+-rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.6.0/lamin-project.yaml
+-rw-r--r--   0        0        0      378 2023-05-26 16:18:33.421862 laminci-0.6.0/laminci/__init__.py
+-rw-r--r--   0        0        0     2122 2023-05-26 16:17:30.304228 laminci-0.6.0/laminci/_artifacts.py
+-rw-r--r--   0        0        0     1358 2023-05-26 16:17:30.304517 laminci-0.6.0/laminci/_db.py
+-rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.6.0/laminci/_docs.py
+-rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.6.0/laminci/_env.py
+-rw-r--r--   0        0        0     2423 2023-04-10 13:41:42.840205 laminci-0.6.0/laminci/_nox.py
+-rw-r--r--   0        0        0       81 2023-05-26 16:17:30.304774 laminci-0.6.0/laminci/db.py
+-rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.6.0/laminci/nox.py
+-rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.6.0/noxfile.py
+-rw-r--r--   0        0        0      694 2023-03-09 14:11:55.514326 laminci-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-05-26 16:17:30.304991 laminci-0.6.0/tests/test_artifacts.py
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 laminci-0.6.0/PKG-INFO
```

### Comparing `laminci-0.5.3/.github/workflows/build.yml` & `laminci-0.6.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.5.3/.github/workflows/latest-changes.yml` & `laminci-0.6.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.5.3/.gitignore` & `laminci-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `laminci-0.5.3/.pre-commit-config.yaml` & `laminci-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `laminci-0.5.3/docs/changelog.md` & `laminci-0.6.0/docs/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+✨ Add aws cli based way of pushing a docs artifact | [20](https://github.com/laminlabs/laminci/pull/20) | [falexwolf](https://github.com/falexwolf) | 2023-05-26 | 0.6.0
+🚸 Allow passing version to `setup_local_test_postgres` | [19](https://github.com/laminlabs/laminci/pull/19) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
 🚸 Close current instance before uploading docs artifacts | [17](https://github.com/laminlabs/laminci/pull/17) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.3
 🚸 Add support for environments | [16](https://github.com/laminlabs/laminci/pull/16) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.1
 ⬆️ Upgrade to new replace API | [15](https://github.com/laminlabs/laminci/pull/15) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.0
 ♻️ Replace `lndb` with `lamin` | [14](https://github.com/laminlabs/laminci/pull/14) | [falexwolf](https://github.com/falexwolf) | 2023-03-29 | 0.4.2
 🚸 Replace git checkout with git switch | [13](https://github.com/laminlabs/laminci/pull/13) | [falexwolf](https://github.com/falexwolf) | 2023-03-27 | 0.4.1
 ⬆️ Upgrade to LaminDB v0.35 | [12](https://github.com/laminlabs/laminci/pull/12) | [falexwolf](https://github.com/falexwolf) | 2023-03-26 | 0.4.0
 🚚 Rename `upload_docs_dir` to `upload_docs_artifact` |  | 2023-03-21 | 0.3.4
```

### Comparing `laminci-0.5.3/docs/guide/quickstart.ipynb` & `laminci-0.6.0/docs/guide/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.5.3/docs/notes/YYYY-MM-DD-my-design-choice.ipynb` & `laminci-0.6.0/docs/notes/YYYY-MM-DD-my-design-choice.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.5.3/laminci/_artifacts.py` & `laminci-0.6.0/laminci/_artifacts.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
+import warnings
 from pathlib import Path
+from subprocess import run
 from zipfile import ZipFile
 
 from lamin_logger import logger
 
 from ._env import get_package_name
 
 
@@ -13,34 +15,62 @@
         for f in Path("./docs").glob("**/*"):
             if ".ipynb_checkpoints" in str(f):
                 continue
             if f.suffix in {".md", ".ipynb", ".png", ".jpg", ".svg"}:
                 zf.write(f, f.relative_to("./docs"))  # add at root level
 
 
-def upload_docs_artifact() -> None:
-    # this is super ugly but necessary right now
-    # we might need to close the current instance as it might be corrupted
-    import lndb
-
-    lndb.close()
-
-    import lamindb as ln
-
-    if "GITHUB_EVENT_NAME" in os.environ and os.environ["GITHUB_EVENT_NAME"] != "push":
-        logger.info("Only upload docs artifact for push event.")
-        return None
+def zip_docs():
     package_name = get_package_name()
     zip_filename = f"{package_name}_docs.zip"
     zip_docs_dir(zip_filename)
+    return package_name, zip_filename
+
+
+def upload_docs_artifact_aws() -> None:
+    package_name, zip_filename = zip_docs()
+    run(
+        f"aws s3 cp {zip_filename} s3://lamin-site-assets/docs/{zip_filename}",
+        shell=True,
+    )
+
+
+def upload_docs_artifact_lamindb() -> None:
+    package_name, zip_filename = zip_docs()
+
+    import lamindb as ln
 
     ln.setup.load("testuser1/lamin-site-assets", migrate=True)
 
     transform = ln.add(ln.Transform, name=f"CI {package_name}")
     ln.track(transform=transform)
 
     file = ln.select(ln.File, key=f"docs/{zip_filename}").one_or_none()
     if file is not None:
         file.replace(zip_filename)
     else:
         file = ln.File(zip_filename, key=f"docs/{zip_filename}")
     ln.add(file)
+
+
+def upload_docs_artifact(aws: bool = False) -> None:
+    if "GITHUB_EVENT_NAME" in os.environ and os.environ["GITHUB_EVENT_NAME"] != "push":
+        logger.info("Only upload docs artifact for push event.")
+        return None
+
+    if aws:
+        upload_docs_artifact_aws()
+    else:
+        try:
+            # this is super ugly but necessary right now
+            # we might need to close the current instance as it might be corrupted
+            import lndb
+
+            lndb.close()
+
+            import lamindb as ln  # noqa
+
+            upload_docs_artifact_lamindb()
+
+        except ImportError:
+            warnings.warn("Fall back to AWS")
+            upload_docs_artifact_aws()
```

### Comparing `laminci-0.5.3/laminci/_db.py` & `laminci-0.6.0/laminci/_db.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 from pathlib import Path
-from subprocess import PIPE, run
+from subprocess import run
+from typing import Optional
 
 from lamin_logger import logger
 
 
 def setup_local_test_sqlite_file(src_settings, return_dir: bool = False):
     path = src_settings._sqlite_file_local
     new_stem = path.stem + "_test"
@@ -15,39 +16,27 @@
     tgt_sqlite_file.parent.mkdir(exist_ok=True)
     if tgt_sqlite_file.exists():
         tgt_sqlite_file.unlink()
     tgt_db = f"sqlite:///{tgt_sqlite_file}"
     return tgt_db
 
 
-def setup_local_test_postgres(name: str = "pgtest"):
+def setup_local_test_postgres(name: str = "pgtest", version: Optional[str] = None):
+    if version is not None:
+        version = ":{version}"
+    else:
+        version = ""
     process = run(
         f"docker run --name {name} -e POSTGRES_PASSWORD=pwd"
-        f" -e POSTGRES_DB={name} -d -p 5432:5432 postgres",  # noqa
+        f" -e POSTGRES_DB={name} -d -p 5432:5432 postgres{version}",  # noqa
         shell=True,
     )
     if process.returncode == 0:
         logger.info(
             "Created Postgres test instance:"
             f" 'postgresql://postgres:pwd@0.0.0.0:5432/{name}'\nIt runs in docker"
             f" container '{name}'"
         )
     else:
         raise RuntimeError("Failed to set up postgres test instance.")
     time.sleep(2)
     return f"postgresql://postgres:pwd@0.0.0.0:5432/{name}"
-
-
-def setup_local_test_postgres_supabase():
-    process = run(
-        f"""supabase start | grep 'anon key'|cut -f2 -d ":" | sed -e 's/^[[:space:]]*//'""",  # noqa
-        shell=True,
-        stdout=PIPE,
-    )
-    anon_key = process.stdout.decode("UTF-8").replace("\n", "")
-    open(".supabase_local_anon_key", "w").write(anon_key)
-    if process.returncode == 0:
-        logger.info("Created Supabase test instance.")
-    else:
-        raise RuntimeError("Failed to set up Supabase test instance.")
-    time.sleep(2)
-    return "postgresql://postgres:postgres@localhost:54322/postgres"
```

### Comparing `laminci-0.5.3/laminci/_env.py` & `laminci-0.6.0/laminci/_env.py`

 * *Files identical despite different names*

### Comparing `laminci-0.5.3/laminci/_nox.py` & `laminci-0.6.0/laminci/_nox.py`

 * *Files identical despite different names*

### Comparing `laminci-0.5.3/pyproject.toml` & `laminci-0.6.0/pyproject.toml`

 * *Files identical despite different names*

