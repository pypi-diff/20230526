# Comparing `tmp/lnschema_lamin1-0.16.3.tar.gz` & `tmp/lnschema_lamin1-0.17a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnschema_lamin1-0.16.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lnschema_lamin1-0.17a1.tar", last modified: Thu May 25 22:09:04 2023, max compression
```

## Comparing `lnschema_lamin1-0.16.3.tar` & `lnschema_lamin1-0.17a1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     3577 2023-05-08 08:17:58.718695 lnschema_lamin1-0.16.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-08 08:17:58.718802 lnschema_lamin1-0.16.3/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-08 08:17:58.718895 lnschema_lamin1-0.16.3/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1416 2023-05-08 08:17:58.718998 lnschema_lamin1-0.16.3/.gitignore
--rw-r--r--   0        0        0     1795 2023-05-08 08:17:58.719108 lnschema_lamin1-0.16.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      154 2023-05-15 15:05:43.656555 lnschema_lamin1-0.16.3/README.md
--rw-r--r--   0        0        0      904 2023-05-23 10:11:29.066166 lnschema_lamin1-0.16.3/docs/changelog.md
--rw-r--r--   0        0        0     5015 2023-05-08 08:17:58.719651 lnschema_lamin1-0.16.3/docs/guide/01-get-started.ipynb
--rw-r--r--   0        0        0     2190 2023-05-08 08:17:58.719754 lnschema_lamin1-0.16.3/docs/guide/02-orms.ipynb
--rw-r--r--   0        0        0     5397 2023-05-15 14:35:07.531917 lnschema_lamin1-0.16.3/docs/guide/10-migrate.ipynb
--rw-r--r--   0        0        0       65 2023-05-08 08:17:58.719916 lnschema_lamin1-0.16.3/docs/guide/index.md
--rw-r--r--   0        0        0      122 2023-05-08 08:17:58.719983 lnschema_lamin1-0.16.3/docs/index.md
--rw-r--r--   0        0        0       63 2023-05-08 08:17:58.720072 lnschema_lamin1-0.16.3/docs/reference.md
--rw-r--r--   0        0        0      163 2023-05-08 08:17:58.720149 lnschema_lamin1-0.16.3/lamin-project.yaml
--rw-r--r--   0        0        0      641 2023-05-23 10:10:40.628983 lnschema_lamin1-0.16.3/lnschema_lamin1/__init__.py
--rw-r--r--   0        0        0     4300 2023-05-23 10:09:49.269416 lnschema_lamin1-0.16.3/lnschema_lamin1/_core.py
--rw-r--r--   0        0        0     3232 2023-05-23 10:09:49.269675 lnschema_lamin1-0.16.3/lnschema_lamin1/_link.py
--rw-r--r--   0        0        0      259 2023-05-15 13:03:26.641873 lnschema_lamin1-0.16.3/lnschema_lamin1/dev/__init__.py
--rw-r--r--   0        0        0      119 2023-05-08 08:17:58.720546 lnschema_lamin1-0.16.3/lnschema_lamin1/dev/_id.py
--rw-r--r--   0        0        0      346 2023-05-15 13:03:26.642051 lnschema_lamin1-0.16.3/lnschema_lamin1/dev/_type.py
--rw-r--r--   0        0        0     1145 2023-05-08 08:17:58.720606 lnschema_lamin1-0.16.3/lnschema_lamin1/dev/_versions.py
--rw-r--r--   0        0        0       31 2023-05-08 08:17:58.720661 lnschema_lamin1-0.16.3/lnschema_lamin1/dev/id.py
--rw-r--r--   0        0        0      156 2023-05-15 13:03:26.642233 lnschema_lamin1-0.16.3/lnschema_lamin1/dev/type.py
--rw-r--r--   0        0        0      426 2023-05-23 10:09:49.269914 lnschema_lamin1-0.16.3/lnschema_lamin1/link.py
--rw-r--r--   0        0        0     1063 2023-05-08 08:17:58.720890 lnschema_lamin1-0.16.3/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py
--rw-r--r--   0        0        0     4097 2023-05-15 15:02:57.367902 lnschema_lamin1-0.16.3/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py
--rw-r--r--   0        0        0     2251 2023-05-23 10:12:25.006468 lnschema_lamin1-0.16.3/lnschema_lamin1/migrations/versions/2023-05-23-f9f58cf3ab38-v0_16_3.py
--rw-r--r--   0        0        0      776 2023-05-08 08:17:58.720978 lnschema_lamin1-0.16.3/noxfile.py
--rw-r--r--   0        0        0      655 2023-05-15 09:56:43.981463 lnschema_lamin1-0.16.3/pyproject.toml
--rw-r--r--   0        0        0      811 2023-05-08 08:17:58.721159 lnschema_lamin1-0.16.3/tests/test_migrations.py
--rw-r--r--   0        0        0      481 2023-05-08 08:17:58.721222 lnschema_lamin1-0.16.3/tests/test_notebooks.py
--rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 lnschema_lamin1-0.16.3/PKG-INFO
+-rw-r--r--   0        0        0     3577 2023-04-22 05:28:10.791442 lnschema_lamin1-0.17a1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-04-22 03:48:17.570277 lnschema_lamin1-0.17a1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-04-22 03:48:17.570464 lnschema_lamin1-0.17a1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1416 2023-04-22 03:51:54.773184 lnschema_lamin1-0.17a1/.gitignore
+-rw-r--r--   0        0        0     1795 2023-04-24 17:49:33.167540 lnschema_lamin1-0.17a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      154 2023-05-25 15:48:48.190697 lnschema_lamin1-0.17a1/README.md
+-rw-r--r--   0        0        0     1069 2023-05-25 21:06:40.200485 lnschema_lamin1-0.17a1/docs/changelog.md
+-rw-r--r--   0        0        0     5015 2023-04-24 17:39:09.187958 lnschema_lamin1-0.17a1/docs/guide/01-get-started.ipynb
+-rw-r--r--   0        0        0     2190 2023-04-24 17:39:09.199540 lnschema_lamin1-0.17a1/docs/guide/02-orms.ipynb
+-rw-r--r--   0        0        0     5397 2023-04-24 17:39:09.201311 lnschema_lamin1-0.17a1/docs/guide/10-migrate.ipynb
+-rw-r--r--   0        0        0       65 2023-04-22 04:06:04.615921 lnschema_lamin1-0.17a1/docs/guide/index.md
+-rw-r--r--   0        0        0      122 2023-04-22 03:48:11.331800 lnschema_lamin1-0.17a1/docs/index.md
+-rw-r--r--   0        0        0       63 2023-04-22 03:51:55.148920 lnschema_lamin1-0.17a1/docs/reference.md
+-rw-r--r--   0        0        0      163 2023-04-22 04:44:31.557229 lnschema_lamin1-0.17a1/lamin-project.yaml
+-rw-r--r--   0        0        0      641 2023-05-25 21:06:29.118991 lnschema_lamin1-0.17a1/lnschema_lamin1/__init__.py
+-rw-r--r--   0        0        0     4310 2023-05-25 21:05:50.419914 lnschema_lamin1-0.17a1/lnschema_lamin1/_core.py
+-rw-r--r--   0        0        0     2902 2023-05-25 21:05:50.420200 lnschema_lamin1-0.17a1/lnschema_lamin1/_link.py
+-rw-r--r--   0        0        0      259 2023-05-25 15:48:48.191950 lnschema_lamin1-0.17a1/lnschema_lamin1/dev/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-22 03:48:17.441295 lnschema_lamin1-0.17a1/lnschema_lamin1/dev/_id.py
+-rw-r--r--   0        0        0      346 2023-05-25 15:48:48.192035 lnschema_lamin1-0.17a1/lnschema_lamin1/dev/_type.py
+-rw-r--r--   0        0        0     1145 2023-04-22 03:56:14.122435 lnschema_lamin1-0.17a1/lnschema_lamin1/dev/_versions.py
+-rw-r--r--   0        0        0       31 2023-04-22 03:48:17.441214 lnschema_lamin1-0.17a1/lnschema_lamin1/dev/id.py
+-rw-r--r--   0        0        0      156 2023-05-25 15:48:48.192133 lnschema_lamin1-0.17a1/lnschema_lamin1/dev/type.py
+-rw-r--r--   0        0        0      426 2023-05-25 15:48:48.192250 lnschema_lamin1-0.17a1/lnschema_lamin1/link.py
+-rw-r--r--   0        0        0     1063 2023-04-24 17:49:33.169471 lnschema_lamin1-0.17a1/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py
+-rw-r--r--   0        0        0     4097 2023-05-25 15:48:48.192371 lnschema_lamin1-0.17a1/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py
+-rw-r--r--   0        0        0     2251 2023-05-25 15:48:48.192464 lnschema_lamin1-0.17a1/lnschema_lamin1/migrations/versions/2023-05-23-f9f58cf3ab38-v0_16_3.py
+-rw-r--r--   0        0        0     4920 2023-05-25 21:05:50.420445 lnschema_lamin1-0.17a1/lnschema_lamin1/migrations/versions/2023-05-25-c3f38ffe9e05-v0_17_0.py
+-rw-r--r--   0        0        0      776 2023-04-24 16:11:06.697345 lnschema_lamin1-0.17a1/noxfile.py
+-rw-r--r--   0        0        0      655 2023-05-25 21:25:20.217756 lnschema_lamin1-0.17a1/pyproject.toml
+-rw-r--r--   0        0        0      811 2023-04-22 04:38:14.658100 lnschema_lamin1-0.17a1/tests/test_migrations.py
+-rw-r--r--   0        0        0      481 2023-04-22 03:48:11.224317 lnschema_lamin1-0.17a1/tests/test_notebooks.py
+-rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 lnschema_lamin1-0.17a1/PKG-INFO
```

### Comparing `lnschema_lamin1-0.16.3/.github/workflows/build.yml` & `lnschema_lamin1-0.17a1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.3/.github/workflows/latest-changes.yml` & `lnschema_lamin1-0.17a1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.3/.gitignore` & `lnschema_lamin1-0.17a1/.gitignore`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.3/.pre-commit-config.yaml` & `lnschema_lamin1-0.17a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.3/docs/changelog.md` & `lnschema_lamin1-0.17a1/docs/changelog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🏗️ Remove SQL-level schema modules | [9](https://github.com/laminlabs/lnschema-lamin1/pull/9) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 | 0.17a1
 🎨 Add `Well` table, File.cell_lines | [8](https://github.com/laminlabs/lnschema-lamin1/pull/8) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-23 | 0.16.3
 💚 Removed treatment relationships | [4](https://github.com/laminlabs/lnschema-lamin1/pull/4) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-15 | 0.16.2
 ✨ Added `Treatment` table | [3](https://github.com/laminlabs/lnschema-lamin1/pull/3) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-15 |
 🚚 Link `CellType` to `File` | [2](https://github.com/laminlabs/lnschema-lamin1/pull/2) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 | 0.16.1
 🎉 Move content from `lnschema-wetlab` here | [1](https://github.com/laminlabs/lnschema-lamin1/pull/1) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.15.1
```

### Comparing `lnschema_lamin1-0.16.3/docs/guide/01-get-started.ipynb` & `lnschema_lamin1-0.17a1/docs/guide/01-get-started.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.3/docs/guide/02-orms.ipynb` & `lnschema_lamin1-0.17a1/docs/guide/02-orms.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.3/docs/guide/10-migrate.ipynb` & `lnschema_lamin1-0.17a1/docs/guide/10-migrate.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.3/lnschema_lamin1/__init__.py` & `lnschema_lamin1-0.17a1/lnschema_lamin1/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,15 +24,15 @@
    link
 
 """
 
 _schema_id = "tvhn"
 _name = "lamin1"
 _migration = "f9f58cf3ab38"
-__version__ = "0.16.3"
+__version__ = "0.17a1"
 
 # prints warning of python versions
 from lamin_logger import py_version_warning
 
 py_version_warning("3.8", "3.10")
```

### Comparing `lnschema_lamin1-0.16.3/lnschema_lamin1/_core.py` & `lnschema_lamin1-0.17a1/lnschema_lamin1/_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,65 +5,68 @@
     ExperimentBase,
     ExperimentTypeBase,
     TechsampleBase,
     TreatmentBase,
 )
 from lnschema_bionty import CellLine, CellType, Disease, Species, Tissue
 from lnschema_core import File
-from lnschema_core.dev.sqlmodel import add_relationship_keys, schema_sqlmodel
+from lnschema_core.dev.sqlmodel import add_relationship_keys, get_orm, schema_sqlmodel
 from sqlalchemy.orm import relationship
 from sqlmodel import Field, Relationship
 
 from lnschema_lamin1.dev import type as tp
 
+from . import __name__ as module_name
 from . import _name as schema_name
 from .link import (
     BiosampleTechsample,
     BiosampleTreatment,
     FileBiosample,
     FileCellLine,
     FileCellType,
     FileExperiment,
     FileTreatment,
     FileWell,
 )
 
-SQLModel, prefix, schema_arg = schema_sqlmodel(schema_name)
+# this is for backward compat
+schema_sqlmodel(schema_name)
+
+# this is the current way
+SQLModel = get_orm(module_name)
+
+
+class ExperimentType(ExperimentTypeBase, table=True):  # type: ignore
+    """Experiment types."""
 
 
 class Experiment(ExperimentBase, table=True):  # type: ignore
     """Experiments."""
 
-    experiment_type_id: str = Field(default=None, foreign_key="lamin1.experiment_type.id", index=True)
+    experiment_type_id: str = Field(default=None, foreign_key=ExperimentType.id, index=True)
     files: File = Relationship(
         back_populates="experiments",
         sa_relationship_kwargs=dict(secondary=FileExperiment.__table__),
     )
 
 
-class ExperimentType(ExperimentTypeBase, table=True):  # type: ignore
-    """Experiment types."""
-
-    __tablename__ = f"{prefix}experiment_type"
-
-
 File.experiments = relationship(Experiment, back_populates="files", secondary=FileExperiment.__table__)
 
 
 class Biosample(BiosampleBase, table=True):  # type: ignore
     """Biological samples that are registered in experiments."""
 
     batch: Optional[str] = None
-    species_id: Optional[str] = Field(default=None, foreign_key="bionty.species.id", index=True)
+    species_id: Optional[str] = Field(default=None, foreign_key=Species.id, index=True)
     species: Species = Relationship()
-    tissue_id: Optional[str] = Field(default=None, foreign_key="bionty.tissue.id", index=True)
+    tissue_id: Optional[str] = Field(default=None, foreign_key=Tissue.id, index=True)
     tissue: Tissue = Relationship()
-    cell_type_id: Optional[str] = Field(default=None, foreign_key="bionty.cell_type.id", index=True)
+    cell_type_id: Optional[str] = Field(default=None, foreign_key=CellType.id, index=True)
     cell_type: CellType = Relationship()
-    disease_id: Optional[str] = Field(default=None, foreign_key="bionty.disease.id", index=True)
+    disease_id: Optional[str] = Field(default=None, foreign_key=Disease.id, index=True)
     disease: Disease = Relationship()
     files: File = Relationship(
         back_populates="biosamples",
         sa_relationship_kwargs=dict(secondary=FileBiosample.__table__),
     )
```

### Comparing `lnschema_lamin1-0.16.3/lnschema_lamin1/_link.py` & `lnschema_lamin1-0.17a1/lnschema_lamin1/_link.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,96 +1,77 @@
-from lnschema_core.dev.sqlmodel import schema_sqlmodel
+from lnschema_core.dev.sqlmodel import get_orm
 from sqlmodel import Field, ForeignKeyConstraint
 
-from . import _name as schema_name
+from . import __name__ as module_name
 
-SQLModel, prefix, schema_arg = schema_sqlmodel(schema_name)
+SQLModel = get_orm(module_name)
 
 
 class ProjectExperiment(SQLModel, table=True):  # type: ignore
     """Links `Project` and `Experiment`."""
 
-    __tablename__ = f"{prefix}project_experiment"
-
-    project_id: str = Field(foreign_key="core.project.id", primary_key=True)
-    experiment_id: str = Field(foreign_key="lamin1.experiment.id", primary_key=True)
+    project_id: str = Field(foreign_key="lnschema_core_project.id", primary_key=True)
+    experiment_id: str = Field(foreign_key="lnschema_lamin1_experiment.id", primary_key=True)
 
 
 class FileExperiment(SQLModel, table=True):  # type: ignore
     """Links for `File` and `Experiment`."""
 
-    __tablename__ = f"{prefix}file_experiment"
-
-    file_id: str = Field(foreign_key="core.file.id", primary_key=True)
-    experiment_id: str = Field(foreign_key="lamin1.experiment.id", primary_key=True)
+    file_id: str = Field(foreign_key="lnschema_core_file.id", primary_key=True)
+    experiment_id: str = Field(foreign_key="lnschema_lamin1_experiment.id", primary_key=True)
 
 
 class FileTreatment(SQLModel, table=True):  # type: ignore
     """Links for `File` and `Treatment`."""
 
-    __tablename__ = f"{prefix}file_treatment"
-
-    file_id: str = Field(foreign_key="core.file.id", primary_key=True)
-    treatment_id: str = Field(foreign_key="lamin1.treatment.id", primary_key=True)
+    file_id: str = Field(foreign_key="lnschema_core_file.id", primary_key=True)
+    treatment_id: str = Field(foreign_key="lnschema_lamin1_treatment.id", primary_key=True)
 
 
 class BiosampleTreatment(SQLModel, table=True):  # type: ignore
     """Links for `Biosample` and `Treatment`."""
 
-    __tablename__ = f"{prefix}biosample_treatment"
-
-    biosample_id: str = Field(foreign_key="lamin1.biosample.id", primary_key=True)
-    treatment_id: str = Field(foreign_key="lamin1.treatment.id", primary_key=True)
+    biosample_id: str = Field(foreign_key="lnschema_lamin1_biosample.id", primary_key=True)
+    treatment_id: str = Field(foreign_key="lnschema_lamin1_treatment.id", primary_key=True)
 
 
 class BiosampleTechsample(SQLModel, table=True):  # type: ignore
     """Links for `Biosample` and `Techsample`."""
 
-    __tablename__ = f"{prefix}biosample_techsample"
-
-    biosample_id: str = Field(foreign_key="lamin1.biosample.id", primary_key=True)
-    techsample_id: str = Field(foreign_key="lamin1.techsample.id", primary_key=True)
+    biosample_id: str = Field(foreign_key="lnschema_lamin1_biosample.id", primary_key=True)
+    techsample_id: str = Field(foreign_key="lnschema_lamin1_techsample.id", primary_key=True)
 
 
 class FileBiosample(SQLModel, table=True):  # type: ignore
     """Links for `File` and `Biosample`."""
 
-    __tablename__ = f"{prefix}file_biosample"
-
-    file_id: str = Field(foreign_key="core.file.id", primary_key=True)
-    biosample_id: str = Field(foreign_key="lamin1.biosample.id", primary_key=True)
+    file_id: str = Field(foreign_key="lnschema_core_file.id", primary_key=True)
+    biosample_id: str = Field(foreign_key="lnschema_lamin1_biosample.id", primary_key=True)
 
 
 class FileCellType(SQLModel, table=True):  # type: ignore
     """Links for `File` and `CellType`."""
 
-    __tablename__ = f"{prefix}file_cell_type"
-
-    file_id: str = Field(foreign_key="core.file.id", primary_key=True)
-    cell_type_id: str = Field(foreign_key="bionty.cell_type.id", primary_key=True)
+    file_id: str = Field(foreign_key="lnschema_core_file.id", primary_key=True)
+    cell_type_id: str = Field(foreign_key="lnschema_bionty_celltype.id", primary_key=True)
 
 
 class FileCellLine(SQLModel, table=True):  # type: ignore
     """Links for `File` and `CellLine`."""
 
-    __tablename__ = f"{prefix}file_cell_line"
-
-    file_id: str = Field(foreign_key="core.file.id", primary_key=True)
-    cell_line_id: str = Field(foreign_key="bionty.cell_line.id", primary_key=True)
+    file_id: str = Field(foreign_key="lnschema_core_file.id", primary_key=True)
+    cell_line_id: str = Field(foreign_key="lnschema_bionty_cellline.id", primary_key=True)
 
 
 class FileWell(SQLModel, table=True):  # type: ignore
     """Links for `File` and `Well`."""
 
-    __tablename__ = f"{prefix}file_well"
-
-    file_id: str = Field(foreign_key="core.file.id", primary_key=True)
+    file_id: str = Field(foreign_key="lnschema_core_file.id", primary_key=True)
     well_row: str = Field(primary_key=True)
     well_column: int = Field(primary_key=True)
 
     __table_args__ = (
         ForeignKeyConstraint(
             ["well_row", "well_column"],
-            ["lamin1.well.row", "lamin1.well.column"],
+            ["lnschema_lamin1_well.row", "lnschema_lamin1_well.column"],
         ),
-        {"schema": schema_arg},
     )
```

### Comparing `lnschema_lamin1-0.16.3/lnschema_lamin1/dev/_versions.py` & `lnschema_lamin1-0.17a1/lnschema_lamin1/dev/_versions.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.3/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py` & `lnschema_lamin1-0.17a1/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.3/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py` & `lnschema_lamin1-0.17a1/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.3/lnschema_lamin1/migrations/versions/2023-05-23-f9f58cf3ab38-v0_16_3.py` & `lnschema_lamin1-0.17a1/lnschema_lamin1/migrations/versions/2023-05-23-f9f58cf3ab38-v0_16_3.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.3/noxfile.py` & `lnschema_lamin1-0.17a1/noxfile.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.3/pyproject.toml` & `lnschema_lamin1-0.17a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.3/tests/test_migrations.py` & `lnschema_lamin1-0.17a1/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.3/PKG-INFO` & `lnschema_lamin1-0.17a1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnschema_lamin1
-Version: 0.16.3
+Version: 0.17a1
 Summary: Lamin's `lamin1` lab schema (`tvhn`).
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lamindb[bionty,biolab]
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "test"
```

