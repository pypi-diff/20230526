# Comparing `tmp/pycatsearch-5.1.4.tar.gz` & `tmp/pycatsearch-5.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatsearch-5.1.4.tar", last modified: Tue May 23 06:51:47 2023, max compression
+gzip compressed data, was "pycatsearch-5.1.5.tar", last modified: Fri May 26 10:59:25 2023, max compression
```

## Comparing `pycatsearch-5.1.4.tar` & `pycatsearch-5.1.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:47.988060 pycatsearch-5.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:47.984060 pycatsearch-5.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:47.984060 pycatsearch-5.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-05-23 06:51:47.988060 pycatsearch-5.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:51:47.988060 pycatsearch-5.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:47.984060 pycatsearch-5.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:47.988060 pycatsearch-5.1.4/src/pycatsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 06:51:47.000000 pycatsearch-5.1.4/src/pycatsearch/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/async_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/catalog_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:47.988060 pycatsearch-5.1.4/src/pycatsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/download_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/float_spinbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/frequency_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/menu_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/selectable_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/substance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/substances_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/titled_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    40971 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/waiting_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)    23913 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:47.988060 pycatsearch-5.1.4/src/pycatsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-05-23 06:51:47.000000 pycatsearch-5.1.4/src/pycatsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-23 06:51:47.000000 pycatsearch-5.1.4/src/pycatsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:51:47.000000 pycatsearch-5.1.4/src/pycatsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-23 06:51:47.000000 pycatsearch-5.1.4/src/pycatsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:51:47.000000 pycatsearch-5.1.4/src/pycatsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 06:51:47.000000 pycatsearch-5.1.4/src/pycatsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:59:25.743520 pycatsearch-5.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:59:25.735520 pycatsearch-5.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:59:25.739520 pycatsearch-5.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-05-26 10:59:25.743520 pycatsearch-5.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 10:59:25.743520 pycatsearch-5.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:59:25.735520 pycatsearch-5.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:59:25.739520 pycatsearch-5.1.5/src/pycatsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 10:59:25.000000 pycatsearch-5.1.5/src/pycatsearch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/async_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/catalog_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:59:25.743520 pycatsearch-5.1.5/src/pycatsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/download_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/float_spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/frequency_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/menu_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/selectable_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/substance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/substances_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/titled_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41570 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/waiting_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24830 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:59:25.739520 pycatsearch-5.1.5/src/pycatsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-05-26 10:59:25.000000 pycatsearch-5.1.5/src/pycatsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 10:59:25.000000 pycatsearch-5.1.5/src/pycatsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:59:25.000000 pycatsearch-5.1.5/src/pycatsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-26 10:59:25.000000 pycatsearch-5.1.5/src/pycatsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 10:59:25.000000 pycatsearch-5.1.5/src/pycatsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 10:59:25.000000 pycatsearch-5.1.5/src/pycatsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/updater.py
```

### Comparing `pycatsearch-5.1.4/.github/workflows/publish-to-pypi.yml` & `pycatsearch-5.1.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/LICENSE.md` & `pycatsearch-5.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/PKG-INFO` & `pycatsearch-5.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.4
+Version: 5.1.5
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
```

### Comparing `pycatsearch-5.1.4/README.md` & `pycatsearch-5.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/main.py` & `pycatsearch-5.1.5/main.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/pyproject.toml` & `pycatsearch-5.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/setup.py` & `pycatsearch-5.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/src/pycatsearch/__init__.py` & `pycatsearch-5.1.5/src/pycatsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/src/pycatsearch/async_downloader.py` & `pycatsearch-5.1.5/src/pycatsearch/async_downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,23 +153,29 @@
                                 if within(_catalog_entry.frequency, self._frequency_limits)]
                     }
 
                 species: list[dict[str, int | str]] = await get_species()
                 self._tasks = [asyncio.create_task(get_substance_catalog(_e)) for _e in species]
                 catalog: list[dict[str, int | str | list[dict[str, float]]]] = []
                 species_count: Final[int] = len(species)
+                skipped_count: int = 0
                 catalog_entry: dict[str, int | str | list[dict[str, float]]]
                 future_entry_index: int
                 future_entry: asyncio.Future[dict[str, int | str | list[dict[str, float]]]]
                 for future_entry_index, future_entry in enumerate(asyncio.as_completed(self._tasks), start=1):
                     catalog_entry = await future_entry
                     if catalog_entry and LINES in catalog_entry and catalog_entry[LINES]:
                         catalog.append(catalog_entry)
+                    else:
+                        skipped_count += 1
                     if self._state_queue is not None:
-                        self._state_queue.put((len(catalog), species_count - future_entry_index))
+                        self._state_queue.put((len(catalog), species_count - future_entry_index - skipped_count))
+
+            if self._state_queue is not None:
+                self._state_queue.put((len(catalog), 0))
 
             return catalog
 
         with suppress(RuntimeError):  # it might be “cannot schedule new futures after shutdown”
             self._catalog = asyncio.run(async_get_catalog())
```

### Comparing `pycatsearch-5.1.4/src/pycatsearch/catalog.py` & `pycatsearch-5.1.5/src/pycatsearch/catalog.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/src/pycatsearch/catalog_entry.py` & `pycatsearch-5.1.5/src/pycatsearch/catalog_entry.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/src/pycatsearch/downloader.py` & `pycatsearch-5.1.5/src/pycatsearch/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,23 +164,29 @@
                         for _catalog_entry in catalog_entries
                         if within(_catalog_entry.frequency, self._frequency_limits)]
             }
 
         species: list[dict[str, int | str]] = get_species()
         catalog: list[dict[str, int | str | list[dict[str, float]]]] = []
         species_count: Final[int] = len(species)
+        skipped_count: int = 0
         catalog_entry: dict[str, int | str | list[dict[str, float]]]
         entry_index: int
         _e: dict[str, int | str]
         for entry_index, _e in enumerate(species):
             catalog_entry = get_substance_catalog(_e)
             if catalog_entry and LINES in catalog_entry and catalog_entry[LINES]:
                 catalog.append(catalog_entry)
+            else:
+                skipped_count += 1
             if self._state_queue is not None:
-                self._state_queue.put((len(catalog), species_count - entry_index))
+                self._state_queue.put((len(catalog), species_count - entry_index - skipped_count))
+
+        if self._state_queue is not None:
+            self._state_queue.put((len(catalog), 0))
 
         self._catalog = catalog
 
 
 def get_catalog(frequency_limits: tuple[float, float] = (-inf, inf)) \
         -> list[dict[str, int | str | list[dict[str, float]]]]:
     """
```

### Comparing `pycatsearch-5.1.4/src/pycatsearch/gui/catalog_info.py` & `pycatsearch-5.1.5/src/pycatsearch/gui/catalog_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/src/pycatsearch/gui/download_dialog.py` & `pycatsearch-5.1.5/src/pycatsearch/gui/download_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
         if self.progress_page.downloader is not None and self.progress_page.downloader.is_alive():
             self.progress_page.downloader.join(0.1)
 
         if exit_code == QDialog.DialogCode.Accepted and self.catalog:
             _formats: dict[tuple[str, ...], str] = {
                 tuple(all_cases('.json.gz')): self.tr('JSON with GZip compression', 'file type'),
                 tuple(all_cases('.json.bz2')): self.tr('JSON with Bzip2 compression', 'file type'),
-                tuple(*all_cases('.json.xz'), *all_cases('.json.lzma')):
+                (*all_cases('.json.xz'), *all_cases('.json.lzma')):
                     self.tr('JSON with LZMA2 compression', 'file type'),
                 tuple(all_cases('.json')): self.tr('JSON', 'file type'),
             }
             save_file_name: str
             save_file_name, _ = self._get_save_file_name(formats=_formats, caption=self.tr('Save As...'))
             if not save_file_name:
                 return
```

### Comparing `pycatsearch-5.1.4/src/pycatsearch/gui/float_spinbox.py` & `pycatsearch-5.1.5/src/pycatsearch/gui/float_spinbox.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/src/pycatsearch/gui/frequency_box.py` & `pycatsearch-5.1.5/src/pycatsearch/gui/frequency_box.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/src/pycatsearch/gui/menu_bar.py` & `pycatsearch-5.1.5/src/pycatsearch/gui/menu_bar.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,90 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
+from contextlib import suppress
+from typing import Any
+
 from qtpy.QtGui import QIcon
 from qtpy.QtWidgets import QAction, QMenu, QMenuBar, QStyle, QWidget
 
 __all__ = ['MenuBar']
 
 
 class MenuBar(QMenuBar):
     def __init__(self, parent: QWidget | None = None) -> None:
         super().__init__(parent)
-        self.menu_file: QMenu = QMenu(self.tr('&File'), self)
-        self.menu_help: QMenu = QMenu(self.tr('&Help'), self)
-        self.menu_edit: QMenu = QMenu(self.tr('&Edit'), self)
-        self.menu_columns: QMenu = QMenu(self.tr('&Columns'), self)
-        self.menu_copy_only: QMenu = QMenu(self.tr('Copy &Only'), self.menu_edit)
-        self.action_load: QAction = QAction(
-            QIcon.fromTheme('document-open', self.style().standardIcon(QStyle.StandardPixmap.SP_DialogOpenButton)),
-            self.tr('&Load Catalog...'),
-            self.menu_file)
-        self.action_reload: QAction = QAction(
-            QIcon.fromTheme('document-revert', self.style().standardIcon(QStyle.StandardPixmap.SP_BrowserReload)),
-            self.tr('&Reload Catalogs'),
-            self.menu_file)
-        self.action_download_catalog: QAction = QAction(self.tr('&Download Catalog...'), self.menu_file)
-        self.action_preferences: QAction = QAction(self.tr('&Preferences...'), self.menu_file)
-        self.action_quit: QAction = QAction(QIcon.fromTheme('application-exit'), self.tr('&Quit'),
-                                            self.menu_file)
-        self.action_check_updates: QAction = QAction(self.tr('Check for Updates...'), self.menu_help)
-        self.action_about_catalogs: QAction = QAction(
-            QIcon.fromTheme('help-about', self.style().standardIcon(QStyle.StandardPixmap.SP_FileDialogInfoView)),
-            self.tr('About Catalogs...'),
-            self.menu_help)
-        self.action_about: QAction = QAction(
-            QIcon.fromTheme('help-about', self.style().standardIcon(QStyle.StandardPixmap.SP_FileDialogInfoView)),
-            self.tr('&About...'),
-            self.menu_help)
-        self.action_about_qt: QAction = QAction(self.style().standardIcon(QStyle.StandardPixmap.SP_TitleBarMenuButton),
-                                                self.tr('About &Qt...'), self.menu_help)
-        self.action_copy: QAction = QAction(QIcon.fromTheme('edit-copy'), self.tr('Co&py Selection'),
-                                            self.menu_edit)
-        self.action_clear: QAction = QAction(
-            QIcon.fromTheme('edit-clear', self.style().standardIcon(QStyle.StandardPixmap.SP_DialogResetButton)),
-            self.tr('&Clear Results'),
-            self.menu_edit)
-        self.action_select_all: QAction = QAction(QIcon.fromTheme('edit-select-all'), self.tr('&Select All'),
-                                                  self.menu_edit)
-        self.action_copy_name: QAction = QAction(self.tr('&Substance Name'), self.menu_copy_only)
-        self.action_copy_frequency: QAction = QAction(self.tr('&Frequency'), self.menu_copy_only)
-        self.action_copy_intensity: QAction = QAction(self.tr('&Intensity'), self.menu_copy_only)
-        self.action_copy_lower_state_energy: QAction = QAction(self.menu_copy_only.tr('&Lower State Energy'),
-                                                               self.menu_copy_only)
-        self.action_show_frequency: QAction = QAction(self.tr('&Frequency'), self.menu_columns)
-        self.action_show_intensity: QAction = QAction(self.tr('&Intensity'), self.menu_columns)
-        self.action_show_lower_state_energy: QAction = QAction(self.tr('&Lower State Energy'),
-                                                               self.menu_columns)
-        self.action_substance_info: QAction = QAction(self.tr('Substance &Info'), self.menu_edit)
-
-        self.action_preferences.setMenuRole(QAction.MenuRole.PreferencesRole)
-        self.action_quit.setMenuRole(QAction.MenuRole.QuitRole)
-        self.action_about.setMenuRole(QAction.MenuRole.AboutRole)
-        self.action_about_qt.setMenuRole(QAction.MenuRole.AboutQtRole)
-        self.menu_file.addAction(self.action_load)
-        self.menu_file.addAction(self.action_reload)
+        self.menu_file: QMenu = self.addMenu(self.tr('&File'))
+        self.action_load: QAction = self.menu_file.addAction(
+            self._icon('document-open', 'mdi6.folder-open', standard_pixmap=QStyle.StandardPixmap.SP_DialogOpenButton),
+            self.tr('&Load Catalog...'))
+        self.action_reload: QAction = self.menu_file.addAction(
+            self._icon('document-revert', 'mdi6.reload', standard_pixmap=QStyle.StandardPixmap.SP_BrowserReload),
+            self.tr('&Reload Catalogs'))
         self.menu_file.addSeparator()
-        self.menu_file.addAction(self.action_download_catalog)
+        self.action_download_catalog: QAction = self.menu_file.addAction(
+            self._icon('network-receive', 'mdi6.download'),
+            self.tr('&Download Catalog...'))
         self.menu_file.addSeparator()
-        self.menu_file.addAction(self.action_preferences)
+        self.action_preferences: QAction = self.menu_file.addAction(
+            self._icon('preferences-other', 'mdi6.application-settings'),
+            self.tr('&Preferences...'))
         self.menu_file.addSeparator()
-        self.menu_file.addAction(self.action_quit)
-        self.menu_help.addAction(self.action_check_updates)
-        self.menu_help.addSeparator()
-        self.menu_help.addAction(self.action_about_catalogs)
-        self.menu_help.addAction(self.action_about)
-        self.menu_help.addAction(self.action_about_qt)
-        self.menu_copy_only.addAction(self.action_copy_name)
-        self.menu_copy_only.addAction(self.action_copy_frequency)
-        self.menu_copy_only.addAction(self.action_copy_intensity)
-        self.menu_copy_only.addAction(self.action_copy_lower_state_energy)
-        self.menu_edit.addAction(self.action_clear)
+        self.action_quit: QAction = self.menu_file.addAction(
+            self._icon('application-exit', 'mdi6.exit-run', standard_pixmap=QStyle.StandardPixmap.SP_DialogCloseButton),
+            self.tr('&Quit'))
+
+        self.menu_edit: QMenu = self.addMenu(self.tr('&Edit'))
+        self.action_clear: QAction = self.menu_edit.addAction(
+            self._icon('edit-clear', 'mdi6.broom', standard_pixmap=QStyle.StandardPixmap.SP_DialogResetButton),
+            self.tr('&Clear Results'))
         self.menu_edit.addSeparator()
-        self.menu_edit.addAction(self.menu_copy_only.menuAction())
-        self.menu_edit.addAction(self.action_copy)
+        self.menu_copy_only: QMenu = self.menu_edit.addMenu(self.tr('Copy &Only'))
+        self.action_copy_name: QAction = self.menu_copy_only.addAction(self.tr('&Substance Name'))
+        self.action_copy_frequency: QAction = self.menu_copy_only.addAction(self.tr('&Frequency'))
+        self.action_copy_intensity: QAction = self.menu_copy_only.addAction(self.tr('&Intensity'))
+        self.action_copy_lower_state_energy: QAction = self.menu_copy_only.addAction(
+            self.menu_copy_only.tr('&Lower State Energy'))
+        self.action_copy: QAction = self.menu_edit.addAction(
+            self._icon('edit-copy', 'mdi6.content-copy'),
+            self.tr('Co&py Selection'))
         self.menu_edit.addSeparator()
-        self.menu_edit.addAction(self.action_select_all)
+        self.action_select_all: QAction = self.menu_edit.addAction(
+            self._icon('edit-select-all', 'mdi6.select-all'),
+            self.tr('&Select All'))
         self.menu_edit.addSeparator()
-        self.menu_edit.addAction(self.action_substance_info)
-        self.menu_columns.addAction(self.action_show_frequency)
-        self.menu_columns.addAction(self.action_show_intensity)
-        self.menu_columns.addAction(self.action_show_lower_state_energy)
-        self.addAction(self.menu_file.menuAction())
-        self.addAction(self.menu_edit.menuAction())
-        self.addAction(self.menu_columns.menuAction())
-        self.addAction(self.menu_help.menuAction())
+        self.action_substance_info: QAction = self.menu_edit.addAction(
+            self._icon('dialog-information', 'mdi6.flask-empty-outline', 'mdi6.information-variant',
+                       options=[{}, {'scale_factor': 0.5}]),
+            self.tr('Substance &Info'))
+
+        self.menu_columns: QMenu = self.addMenu(self.tr('&Columns'))
+        self.action_show_frequency: QAction = self.menu_columns.addAction(self.tr('&Frequency'))
+        self.action_show_intensity: QAction = self.menu_columns.addAction(self.tr('&Intensity'))
+        self.action_show_lower_state_energy: QAction = self.menu_columns.addAction(self.tr('&Lower State Energy'))
+
+        self.menu_help: QMenu = self.addMenu(self.tr('&Help'))
+        self.action_check_updates: QAction = self.menu_help.addAction(
+            self._icon('application-update', 'mdi6.update'),
+            self.tr('Check for Updates...'))
+        self.menu_help.addSeparator()
+        self.action_about_catalogs: QAction = self.menu_help.addAction(
+            self._icon('document-properties', 'mdi6.information'),
+            self.tr('About Catalogs...'))
+        self.action_about: QAction = self.menu_help.addAction(
+            self._icon('help-about', 'mdi6.help', standard_pixmap=QStyle.StandardPixmap.SP_FileDialogInfoView),
+            self.tr('&About...'))
+        self.action_about_qt: QAction = self.menu_help.addAction(
+            self.style().standardIcon(QStyle.StandardPixmap.SP_TitleBarMenuButton),
+            self.tr('About &Qt...'))
+
+        self.action_preferences.setMenuRole(QAction.MenuRole.PreferencesRole)
+        self.action_quit.setMenuRole(QAction.MenuRole.QuitRole)
+        self.action_about.setMenuRole(QAction.MenuRole.AboutRole)
+        self.action_about_qt.setMenuRole(QAction.MenuRole.AboutQtRole)
 
         self.action_load.setShortcut('Ctrl+L')
         self.action_quit.setShortcut('Ctrl+Q')
         self.action_about.setShortcut('F1')
         self.action_preferences.setShortcut('Ctrl+,')
         self.action_copy.setShortcut('Ctrl+C')
         self.action_select_all.setShortcut('Ctrl+A')
@@ -105,7 +93,24 @@
         self.action_copy_frequency.setShortcut('Ctrl+Shift+C, F')
         self.action_copy_intensity.setShortcut('Ctrl+Shift+C, I')
         self.action_copy_lower_state_energy.setShortcut('Ctrl+Shift+C, E')
         self.action_substance_info.setShortcut('Ctrl+I')
         self.action_show_frequency.setCheckable(True)
         self.action_show_intensity.setCheckable(True)
         self.action_show_lower_state_energy.setCheckable(True)
+
+    def _icon(self, theme_name: str, *qta_name: str,
+              standard_pixmap: QStyle.StandardPixmap | None = None,
+              **qta_specs: Any) -> QIcon:
+        if theme_name and QIcon.hasThemeIcon(theme_name):
+            return QIcon.fromTheme(theme_name)
+
+        if qta_name:
+            with suppress(ImportError, Exception):
+                import qtawesome as qta
+
+                return qta.icon(*qta_name, **qta_specs)  # might raise an `Exception` if the icon is not in the font
+
+        if standard_pixmap is not None:
+            return self.style().standardIcon(standard_pixmap)
+
+        return QIcon()
```

### Comparing `pycatsearch-5.1.4/src/pycatsearch/gui/settings.py` & `pycatsearch-5.1.5/src/pycatsearch/gui/settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,34 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import os
-from typing import Any, Callable, Final
+from typing import Any, Callable, Final, Hashable, Iterable, NamedTuple
 
-from qtpy.QtCore import QSettings
+from qtpy.QtCore import QObject, QSettings
 
 from ..utils import *
 
 __all__ = ['Settings']
 
 
 class Settings(QSettings):
     """ convenient internal representation of the application settings """
-    FREQUENCY_UNITS: Final[list[str]] = ['MHz', 'GHz', 'cm⁻¹', 'nm']
-    INTENSITY_UNITS: Final[list[str]] = ['lg(nm² × MHz)', 'nm² × MHz', 'lg(cm / molecule)', 'cm / molecule']
-    ENERGY_UNITS: Final[list[str]] = ['cm⁻¹', 'meV', 'J']
-    TEMPERATURE_UNITS: Final[list[str]] = ['K', '°C']
-    LINE_ENDS: Final[list[str]] = [r'Line Feed (\n)', r'Carriage Return (\r)', r'CR+LF (\r\n)', r'LF+CR (\n\r)']
-    _LINE_ENDS: Final[list[str]] = ['\n', '\r', '\r\n', '\n\r']
-    CSV_SEPARATORS: Final[list[str]] = [r'comma (,)', r'tab (\t)', r'semicolon (;)', r'space ( )']
-    _CSV_SEPARATORS: Final[list[str]] = [',', '\t', ';', ' ']
-
-    DIALOG: dict[str, dict[str, tuple[Any, ...]]] = {
-        'When the program starts': {
-            'Load catalogs': ('load_last_catalogs',),
-            'Check for update': ('check_updates',),
-        },
-        'Display': {
-            'Allow rich text in formulas': ('rich_text_in_formulas',),
-        },
-        'Search': {
-            'Timeout:': (slice(1, 99), (' sec',), 'timeout',),
-        },
-        'Units': {
-            'Frequency:': (FREQUENCY_UNITS, 'frequency_unit'),
-            'Intensity:': (INTENSITY_UNITS, 'intensity_unit'),
-            'Energy:': (ENERGY_UNITS, 'energy_unit'),
-            'Temperature:': (TEMPERATURE_UNITS, 'temperature_unit'),
-        },
-        'Export': {
-            'With units': ('with_units',),
-            'Line ending:': (LINE_ENDS, _LINE_ENDS, 'line_end'),
-            'CSV separator:': (CSV_SEPARATORS, _CSV_SEPARATORS, 'csv_separator'),
-        }
-    }
+
+    class CallbackOnly(NamedTuple):
+        callback: str
+
+    class SpinboxAndCallback(NamedTuple):
+        range: slice
+        prefix_and_suffix: tuple[str, str]
+        callback: str
+
+    class ComboboxAndCallback(NamedTuple):
+        combobox_data: Iterable[str] | dict[Hashable, str]
+        callback: str
 
     TO_MHZ: Final[list[Callable[[float], float]]] = [lambda x: x, ghz_to_mhz, rec_cm_to_mhz, nm_to_mhz]
     FROM_MHZ: Final[list[Callable[[float], float]]] = [lambda x: x, mhz_to_ghz, mhz_to_rec_cm, mhz_to_nm]
 
     TO_LOG10_SQ_NM_MHZ: Final[list[Callable[[float], float]]] = [
         lambda x: x,
         sq_nm_mhz_to_log10_sq_nm_mhz,
@@ -72,16 +52,66 @@
         rec_cm_to_meV,
         rec_cm_to_j
     ]
 
     TO_K: Final[list[Callable[[float], float]]] = [lambda x: x, lambda x: x + 273.15]
     FROM_K: Final[list[Callable[[float], float]]] = [lambda x: x, lambda x: x - 273.15]
 
-    def __init__(self, *args: Any) -> None:
-        super().__init__(*args)
+    def __init__(self, organization: str, application: str, parent: QObject | None = None) -> None:
+        super().__init__(organization, application, parent)
+
+        # for some reason, the dicts are not being translated when used as class variables
+        self.LINE_ENDS: Final[dict[str, str]] = {
+            '\n': self.tr(r'Line Feed (\n)'),
+            '\r': self.tr(r'Carriage Return (\r)'),
+            '\r\n': self.tr(r'CR+LF (\r\n)'),
+            '\n\r': self.tr(r'LF+CR (\n\r)')
+        }
+        self.CSV_SEPARATORS: Final[dict[str, str]] = {
+            ',': self.tr(r'comma (,)'),
+            '\t': self.tr(r'tab (\t)'),
+            ';': self.tr(r'semicolon (;)'),
+            ' ': self.tr(r'space ( )')
+        }
+        self.FREQUENCY_UNITS: Final[list[str]] = [self.tr('MHz'), self.tr('GHz'), self.tr('cm⁻¹'), self.tr('nm')]
+        self.INTENSITY_UNITS: Final[list[str]] = [self.tr('lg(nm² × MHz)'), self.tr('nm² × MHz'),
+                                                  self.tr('lg(cm / molecule)'), self.tr('cm / molecule')]
+        self.ENERGY_UNITS: Final[list[str]] = [self.tr('cm⁻¹'), self.tr('meV'), self.tr('J')]
+        self.TEMPERATURE_UNITS: Final[list[str]] = [self.tr('K'), self.tr('°C')]
+
+    @property
+    def dialog(self) -> (dict[(str
+                               | tuple[str, tuple[str, ...]]
+                               | tuple[str, tuple[str, ...], tuple[tuple[str, Any], ...]]),
+                              dict[str, (Settings.CallbackOnly
+                                         | Settings.SpinboxAndCallback
+                                         | Settings.ComboboxAndCallback)]]):
+        return {
+            (self.tr('When the program starts'), ('mdi6.rocket-launch',)): {
+                self.tr('Load catalogs'): Settings.CallbackOnly('load_last_catalogs'),
+                self.tr('Check for update'): Settings.CallbackOnly('check_updates'),
+            },
+            (self.tr('Display'), ('mdi6.binoculars',)): {
+                self.tr('Allow rich text in formulas'): Settings.CallbackOnly('rich_text_in_formulas'),
+            },
+            (self.tr('Search'), ('mdi6.table-search',)): {
+                self.tr('Timeout:'): Settings.SpinboxAndCallback(slice(1, 99), ('', 'sec'), 'timeout'),
+            },
+            (self.tr('Units'), ('mdi6.pencil-ruler',)): {
+                self.tr('Frequency:'): Settings.ComboboxAndCallback(self.FREQUENCY_UNITS, 'frequency_unit'),
+                self.tr('Intensity:'): Settings.ComboboxAndCallback(self.INTENSITY_UNITS, 'intensity_unit'),
+                self.tr('Energy:'): Settings.ComboboxAndCallback(self.ENERGY_UNITS, 'energy_unit'),
+                self.tr('Temperature:'): Settings.ComboboxAndCallback(self.TEMPERATURE_UNITS, 'temperature_unit'),
+            },
+            (self.tr('Export'), ('mdi6.file-export',)): {
+                self.tr('With units'): Settings.CallbackOnly('with_units'),
+                self.tr('Line ending:'): Settings.ComboboxAndCallback(self.LINE_ENDS, 'line_end'),
+                self.tr('CSV separator:'): Settings.ComboboxAndCallback(self.CSV_SEPARATORS, 'csv_separator'),
+            }
+        }
 
     @property
     def frequency_unit(self) -> int:
         self.beginGroup('frequency')
         v: int = self.value('unit', 0, int)
         self.endGroup()
         return v
@@ -261,35 +291,35 @@
         self.beginGroup('display')
         self.setValue('richTextInFormulas', new_value)
         self.endGroup()
 
     @property
     def line_end(self) -> str:
         self.beginGroup('export')
-        v: int = self.value('lineEnd', self._LINE_ENDS.index(os.linesep), int)
+        v: int = self.value('lineEnd', list(self.LINE_ENDS.keys()).index(os.linesep), int)
         self.endGroup()
-        return self._LINE_ENDS[v]
+        return list(self.LINE_ENDS.keys())[v]
 
     @line_end.setter
     def line_end(self, new_value: str) -> None:
         self.beginGroup('export')
-        self.setValue('lineEnd', self._LINE_ENDS.index(new_value))
+        self.setValue('lineEnd', list(self.LINE_ENDS.keys()).index(new_value))
         self.endGroup()
 
     @property
     def csv_separator(self) -> str:
         self.beginGroup('export')
-        v: int = self.value('csvSeparator', self._CSV_SEPARATORS.index('\t'), int)
+        v: int = self.value('csvSeparator', list(self.CSV_SEPARATORS.keys()).index('\t'), int)
         self.endGroup()
-        return self._CSV_SEPARATORS[v]
+        return list(self.CSV_SEPARATORS.keys())[v]
 
     @csv_separator.setter
     def csv_separator(self, new_value: str) -> None:
         self.beginGroup('export')
-        self.setValue('csvSeparator', self._CSV_SEPARATORS.index(new_value))
+        self.setValue('csvSeparator', list(self.CSV_SEPARATORS.keys()).index(new_value))
         self.endGroup()
 
     @property
     def with_units(self) -> bool:
         self.beginGroup('export')
         v: bool = self.value('withUnits', True, bool)
         self.endGroup()
@@ -309,7 +339,20 @@
         return v
 
     @timeout.setter
     def timeout(self, new_value: float) -> None:
         self.beginGroup('search')
         self.setValue('timeout', new_value)
         self.endGroup()
+
+    @property
+    def ignored_version(self) -> str:
+        self.beginGroup('update')
+        v: str = self.value('ignoredVersion', '', str)
+        self.endGroup()
+        return v
+
+    @ignored_version.setter
+    def ignored_version(self, new_value: str) -> None:
+        self.beginGroup('update')
+        self.setValue('ignoredVersion', new_value)
+        self.endGroup()
```

### Comparing `pycatsearch-5.1.4/src/pycatsearch/gui/substance_info.py` & `pycatsearch-5.1.5/src/pycatsearch/gui/substance_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/src/pycatsearch/gui/substances_box.py` & `pycatsearch-5.1.5/src/pycatsearch/gui/substances_box.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/src/pycatsearch/gui/titled_list_widget.py` & `pycatsearch-5.1.5/src/pycatsearch/gui/titled_list_widget.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/src/pycatsearch/gui/ui.py` & `pycatsearch-5.1.5/src/pycatsearch/gui/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -419,22 +419,27 @@
         self.menu_bar.action_clear.triggered.connect(self._on_action_clear_triggered)
 
         if not self.catalog.is_empty:
             self.box_frequency.set_frequency_limits(self.catalog.min_frequency, self.catalog.max_frequency)
 
         if self.settings.check_updates:
             _latest_release: ReleaseInfo = latest_release()
-            if _latest_release and _latest_release.version > __version__:
+            if (_latest_release
+                    and _latest_release.version != self.settings.ignored_version
+                    and _latest_release.version > __version__):
                 res: QMessageBox.StandardButton = QMessageBox.question(
                     self, self.tr('Release Info'),
                     self.tr('Version {release.version} published {release.pub_date} is available. '
                             'Would you like to get the update? '
-                            'The app will try to restart.').format(release=_latest_release))
+                            'The app will try to restart.').format(release=_latest_release),
+                    QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No | QMessageBox.StandardButton.Ignore)
                 if res == QMessageBox.StandardButton.Yes:
                     update_with_pip()
+                elif res == QMessageBox.StandardButton.Ignore:
+                    self.settings.ignored_version = _latest_release.version
 
     def closeEvent(self, event: QCloseEvent) -> None:
         self.save_settings()
         event.accept()
 
     def load_catalog(self, *catalog_file_names: str) -> bool:
         self.setDisabled(True)
@@ -498,16 +503,16 @@
         return filename, _filter
 
     @Slot()
     def _on_action_load_triggered(self) -> None:
         self.status_bar.showMessage(self.tr('Select a catalog file to load.'))
         new_catalog_file_names: list[str]
         _formats: dict[tuple[str, ...], str] = {
-            tuple(*all_cases('.json.gz'), *all_cases('.json.bz2'),
-                  *all_cases('.json.xz'), *all_cases('.json.lzma')): self.tr('Compressed JSON', 'file type'),
+            (*all_cases('.json.gz'), *all_cases('.json.bz2'),
+             *all_cases('.json.xz'), *all_cases('.json.lzma')): self.tr('Compressed JSON', 'file type'),
             tuple(all_cases('.json')): self.tr('JSON', 'file type'),
         }
         new_catalog_file_names, _ = self.get_open_file_names(formats=_formats,
                                                              caption=self.tr('Load Catalog'),
                                                              directory=(*self.catalog.sources, '')[0])
 
         if new_catalog_file_names:
@@ -657,17 +662,20 @@
         if not _latest_release:
             QMessageBox.warning(self, self.tr('Release Info'), self.tr('Update check failed.'))
         elif _latest_release.version > __version__:
             res: QMessageBox.StandardButton = QMessageBox.question(
                 self, self.tr('Release Info'),
                 self.tr('Version {release.version} published {release.pub_date} is available. '
                         'Would you like to get the update? '
-                        'The app will try to restart.').format(release=_latest_release))
+                        'The app will try to restart.').format(release=_latest_release),
+                QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No | QMessageBox.StandardButton.Ignore)
             if res == QMessageBox.StandardButton.Yes:
                 update_with_pip()
+            elif res == QMessageBox.StandardButton.Ignore:
+                self.settings.ignored_version = _latest_release.version
         else:
             QMessageBox.information(self, self.tr('Release Info'), self.tr('You are using the latest version.'))
 
     @Slot()
     def _on_action_about_catalogs_triggered(self) -> None:
         if self.catalog:
             ci: CatalogInfo = CatalogInfo(self.catalog, self)
```

### Comparing `pycatsearch-5.1.4/src/pycatsearch/gui/waiting_screen.py` & `pycatsearch-5.1.5/src/pycatsearch/gui/waiting_screen.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/src/pycatsearch/utils.py` & `pycatsearch-5.1.5/src/pycatsearch/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,15 +163,16 @@
 
     last_i_1: int
     last_i_2: int
     i_1: int = 0
     i_2: int = 0
 
     if key is None:
-        key = lambda _: _
+        def key(value: _AnyType) -> SupportsLessAndEqual:
+            return value
 
     while i_1 < len(sorted_items_1) and i_2 < len(sorted_items_2):
         last_i_1 = i_1
         while (i_1 < len(sorted_items_1) and i_2 < len(sorted_items_2)
                and key(sorted_items_1[i_1]) <= key(sorted_items_2[i_2])):
             i_1 += 1
         if last_i_1 < i_1:
@@ -216,15 +217,17 @@
                   key: Callable[[_AnyType], SupportsLessAndEqual] | None = None,
                   maybe_equal: bool = False) -> int:
     from operator import lt, le
 
     if not items:
         raise ValueError('Empty sequence provided')
     if key is None:
-        key = lambda _: _
+        def key(value: _AnyType) -> SupportsLessAndEqual:
+            return value
+
     less: Callable[[SupportsLessAndEqual, SupportsLessAndEqual], bool] = le if maybe_equal else lt
     if not less(key(items[0]), threshold):
         return -1
     if less(key(items[-1]), threshold):
         return len(items)
     i: int = 0
     j: int = len(items) - 1
@@ -595,18 +598,40 @@
     def __init__(self, version: str = '', pub_date: str = '') -> None:
         self.version: str = version
         self.pub_date: str = pub_date
 
     def __bool__(self) -> bool:
         return bool(self.version) and bool(self.pub_date)
 
-    def __gt__(self, other: str) -> bool:
-        self_as_tuple: tuple[int | str, ...] = tuple(int(i) if i.isdigit() else i for i in self.version.split('.'))
-        other_as_tuple: tuple[int | str, ...] = tuple(int(i) if i.isdigit() else i for i in other.split('.'))
-        return self_as_tuple > other_as_tuple
+    def __lt__(self, other: str | ReleaseInfo) -> bool:
+        if isinstance(other, str):
+            other = ReleaseInfo(version=other)
+        i: str
+        j: str
+        for i, j in itertools.zip_longest(self.version.replace('-', '.').split('.'),
+                                          other.version.replace('-', '.').split('.'), fillvalue=''):
+            if i == j:
+                continue
+            if i.isdigit() and j.isdigit():
+                return int(i) < int(j)
+            else:
+                i_digits: str = ''.join(itertools.takewhile(str.isdigit, i))
+                j_digits: str = ''.join(itertools.takewhile(str.isdigit, j))
+                if i_digits != j_digits:
+                    if i_digits and j_digits:
+                        return int(i_digits) < int(j_digits)
+                    else:
+                        return i_digits < j_digits
+                return i < j
+        return False
+
+    def __eq__(self, other: str | ReleaseInfo) -> bool:
+        if isinstance(other, str):
+            other = ReleaseInfo(version=other)
+        return self.version == other.version
 
 
 def latest_release() -> ReleaseInfo:
     import urllib.request
     import xml.dom.minidom as dom
     from http.client import HTTPResponse
     from xml.dom.minicompat import NodeList
```

### Comparing `pycatsearch-5.1.4/src/pycatsearch.egg-info/PKG-INFO` & `pycatsearch-5.1.5/src/pycatsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.4
+Version: 5.1.5
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
```

### Comparing `pycatsearch-5.1.4/src/pycatsearch.egg-info/SOURCES.txt` & `pycatsearch-5.1.5/src/pycatsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.4/updater.py` & `pycatsearch-5.1.5/updater.py`

 * *Files identical despite different names*

