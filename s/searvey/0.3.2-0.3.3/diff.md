# Comparing `tmp/searvey-0.3.2-py3-none-any.whl.zip` & `tmp/searvey-0.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 43732 bytes, number of entries: 18
+Zip file size: 43951 bytes, number of entries: 18
 -rw-r--r--  2.0 unx      372 b- defN 80-Jan-01 00:00 searvey/__init__.py
 -rw-r--r--  2.0 unx    35798 b- defN 80-Jan-01 00:00 searvey/coops.py
 -rw-r--r--  2.0 unx     2497 b- defN 80-Jan-01 00:00 searvey/critech.py
 -rw-r--r--  2.0 unx      462 b- defN 80-Jan-01 00:00 searvey/custom_types.py
 -rw-r--r--  2.0 unx     2513 b- defN 80-Jan-01 00:00 searvey/erddap.py
 -rw-r--r--  2.0 unx    12611 b- defN 80-Jan-01 00:00 searvey/ioc.py
 -rw-r--r--  2.0 unx     1389 b- defN 80-Jan-01 00:00 searvey/models.py
 -rw-r--r--  2.0 unx     4405 b- defN 80-Jan-01 00:00 searvey/multi.py
 -rw-r--r--  2.0 unx      975 b- defN 80-Jan-01 00:00 searvey/rate_limit.py
--rw-r--r--  2.0 unx     4969 b- defN 80-Jan-01 00:00 searvey/stations.py
+-rw-r--r--  2.0 unx     5122 b- defN 80-Jan-01 00:00 searvey/stations.py
 -rw-r--r--  2.0 unx     2896 b- defN 80-Jan-01 00:00 searvey/uhslc.py
 -rw-r--r--  2.0 unx     1358 b- defN 80-Jan-01 00:00 searvey/us_states.json
--rw-r--r--  2.0 unx    14917 b- defN 80-Jan-01 00:00 searvey/usgs.py
+-rw-r--r--  2.0 unx    15313 b- defN 80-Jan-01 00:00 searvey/usgs.py
 -rw-r--r--  2.0 unx     4751 b- defN 80-Jan-01 00:00 searvey/utils.py
--rw-r--r--  2.0 unx    35145 b- defN 80-Jan-01 00:00 searvey-0.3.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     4262 b- defN 80-Jan-01 00:00 searvey-0.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 searvey-0.3.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1342 b- defN 16-Jan-01 00:00 searvey-0.3.2.dist-info/RECORD
-18 files, 130750 bytes uncompressed, 41600 bytes compressed:  68.2%
+-rw-r--r--  2.0 unx    35145 b- defN 80-Jan-01 00:00 searvey-0.3.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4051 b- defN 80-Jan-01 00:00 searvey-0.3.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 searvey-0.3.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1342 b- defN 16-Jan-01 00:00 searvey-0.3.3.dist-info/RECORD
+18 files, 131088 bytes uncompressed, 41819 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: searvey/usgs.py
 Comment: 
 
 Filename: searvey/utils.py
 Comment: 
 
-Filename: searvey-0.3.2.dist-info/LICENSE
+Filename: searvey-0.3.3.dist-info/LICENSE
 Comment: 
 
-Filename: searvey-0.3.2.dist-info/METADATA
+Filename: searvey-0.3.3.dist-info/METADATA
 Comment: 
 
-Filename: searvey-0.3.2.dist-info/WHEEL
+Filename: searvey-0.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: searvey-0.3.2.dist-info/RECORD
+Filename: searvey-0.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## searvey/stations.py

```diff
@@ -25,14 +25,18 @@
     "start_date",
     "last_observation",
     "geometry",
 ]
 
 
 class Provider(str, Enum):
+    """
+    An enumeration for ``searvey`` providers.
+    """
+
     ALL: str = "ALL"
     COOPS: str = "COOPS"
     IOC: str = "IOC"
     USGS: str = "USGS"
 
 
 def _get_ioc_stations(
@@ -139,14 +143,17 @@
 
 
 def get_stations(
     activity_threshold: datetime.timedelta = datetime.timedelta(days=3),
     providers: list[Provider] = Provider.ALL,
     region: Polygon | MultiPolygon | None = None,
 ) -> gpd.GeoDataFrame:
+    """
+    Return a ``geopandas.GeoDataFrame`` with metadata from ``providers``.
+    """
     dataframes = []
     if Provider.ALL in providers or Provider.IOC in providers:
         dataframes.append(_get_ioc_stations(activity_threshold=activity_threshold, region=region))
     if Provider.ALL in providers or Provider.COOPS in providers:
         dataframes.append(_get_coops_stations(region=region))
     if Provider.ALL in providers or Provider.USGS in providers:
         dataframes.append(_get_usgs_stations(activity_threshold=activity_threshold, region=region))
```

## searvey/usgs.py

```diff
@@ -9,14 +9,15 @@
 
 We take the return values from `dataretrieval` to be the original data
 """
 from __future__ import annotations
 
 import datetime
 import functools
+import importlib.metadata
 import logging
 import warnings
 from itertools import product
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
@@ -43,14 +44,17 @@
 from .utils import merge_datasets
 from .utils import resolve_date
 from .utils import TODAY
 
 
 logger = logging.getLogger(__name__)
 
+# This will stop working if pandas switches its versioning scheme to CalVer or something...
+_PANDAS_MAJOR_VERSION = int(importlib.metadata.version("pandas").split(".")[0])
+
 # constants
 USGS_OUTPUT_OF_INTEREST = (
     "elevation",  # Overlaps some of the specific codes below
     "flow rate",  # Overlaps some of the specific codes below
     "00065",  # Gage height, feet
     "62614",  # Lake or reservoir water surface elevation above NGVD 1929, feet
     "62615",  # Lake or reservoir water surface elevation above NAVD 1988, feet
@@ -122,29 +126,32 @@
 
 def normalize_usgs_stations(df: pd.DataFrame) -> gpd.GeoDataFrame:
     if df.empty:
         return gpd.GeoDataFrame()
 
     param_dict = _get_usgs_output_info().set_index("parameter_cd").to_dict()
 
-    df.end_date = pd.to_datetime(df.end_date, errors="coerce")
-    df.begin_date = pd.to_datetime(df.begin_date, errors="coerce")
+    to_datetime_kwargs = dict(errors="coerce")
+    if _PANDAS_MAJOR_VERSION >= 2:
+        to_datetime_kwargs["format"] = "mixed"
+    df.end_date = pd.to_datetime(df.end_date, **to_datetime_kwargs)
+    df.begin_date = pd.to_datetime(df.begin_date, **to_datetime_kwargs)
     df["parm_nm"] = [param_dict["parm_nm"].get(i) for i in df.parm_cd.values]
     df["parm_unit"] = [param_dict["parm_unit"].get(i) for i in df.parm_cd.values]
     df = df.dropna(subset="parm_nm")
     # TODO: Should station duplicates (by site_no) be removed?
     gdf = gpd.GeoDataFrame(
         data=df,
         geometry=gpd.points_from_xy(df.dec_long_va, df.dec_lat_va, crs="EPSG:4326"),
     )
     return gdf
 
 
 @functools.lru_cache(maxsize=None)
-def _get_all_usgs_stations() -> gpd.GeoDataFrame:
+def _get_all_usgs_stations(normalize: bool = True) -> gpd.GeoDataFrame:
     """
     Return USGS station metadata for all stations in all the states
 
     :return: ``geopandas.GeoDataFrame`` with the station metadata
     """
 
     # NOTE: multiprocess does NOT keep order
@@ -164,15 +171,16 @@
     )
 
     usgs_stations = functools.reduce(
         # functools.partial(pd.merge, how='outer'),
         lambda i, j: pd.concat([i, j], ignore_index=True),
         (r.result for r in usgs_stations_results if r.result is not None and not r.result.empty),
     )
-    usgs_stations = normalize_usgs_stations(usgs_stations)
+    if normalize:
+        usgs_stations = normalize_usgs_stations(usgs_stations)
 
     return usgs_stations
 
 
 def get_usgs_stations(
     region: Optional[Union[Polygon, MultiPolygon]] = None,
     lon_min: Optional[float] = None,
@@ -202,15 +210,15 @@
         lon_min=lon_min,
         lon_max=lon_max,
         lat_min=lat_min,
         lat_max=lat_max,
         symmetric=True,
     )
 
-    usgs_stations = _get_all_usgs_stations()
+    usgs_stations = _get_all_usgs_stations(normalize=True)
     if region:
         usgs_stations = usgs_stations[usgs_stations.within(region)]
 
     return usgs_stations
 
 
 def normalize_usgs_station_data(df: pd.DataFrame, truncate_seconds: bool) -> pd.DataFrame:
```

## Comparing `searvey-0.3.2.dist-info/LICENSE` & `searvey-0.3.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `searvey-0.3.2.dist-info/METADATA` & `searvey-0.3.3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searvey
-Version: 0.3.2
+Version: 0.3.3
 Summary: 
 Home-page: https://github.com/oceanmodeling/searvey.git
 License: GPL-3.0-or-later
 Author: Panos Mavrogiorgos
 Author-email: pmav99@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
@@ -15,34 +15,30 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Dist: Shapely
 Requires-Dist: beautifulsoup4
-Requires-Dist: dataretrieval
+Requires-Dist: dataretrieval (>=1)
 Requires-Dist: erddapy
 Requires-Dist: geopandas
 Requires-Dist: html5lib
 Requires-Dist: limits
 Requires-Dist: lxml
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: tqdm
+Requires-Dist: typing-extensions
 Requires-Dist: xarray
 Project-URL: Repository, https://github.com/oceanmodeling/searvey.git
 Description-Content-Type: text/markdown
 
 # searvey
 
 [![pre-commit.ci](https://results.pre-commit.ci/badge/github/oceanmodeling/searvey/master.svg)](https://results.pre-commit.ci/latest/github/oceanmodeling/searvey/master)
```

## Comparing `searvey-0.3.2.dist-info/RECORD` & `searvey-0.3.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 searvey/critech.py,sha256=rlHWrtAKdFza9N7GMoKltvslqmkmdRdutsbxKIcD7Jg,2497
 searvey/custom_types.py,sha256=H0bQOND1rGkFxr2nLK8Q-Z0YzgebhERfhxv8MNUAiFQ,462
 searvey/erddap.py,sha256=1vZr_D-r3SqK56N65kYgpbAg-6xi3_wFQekw4s8lMeM,2513
 searvey/ioc.py,sha256=O68KB54QVJCjsNIR15MN8AAzKt23KY31Wjjan8EhLR8,12611
 searvey/models.py,sha256=fmRVoh9pnYE9nUzp1n53fkJVWPvJU3E38qmCZn0u5qk,1389
 searvey/multi.py,sha256=0ueJdcyqVpj3PSEhGQkO1UEVl5jBjrdPaOz7NM-lneg,4405
 searvey/rate_limit.py,sha256=DgvKX8Ww1qej2gZrJquoetHi9vSk4ErI6iTYQ3oGTdA,975
-searvey/stations.py,sha256=Sv1CvJYQVOvEkNI2wxAcjiq96tnA2uiZOOdpiKgTMgE,4969
+searvey/stations.py,sha256=nlHO4iu43534t79agbNNWnZDbN13eIw_SJMlob5MN6A,5122
 searvey/uhslc.py,sha256=i4g2O-ie3gj6IPzpsS9ySSbMl9YtU_cGBXs_qoyt1VA,2896
 searvey/us_states.json,sha256=EBZm8uzX4PWgD1kgg2hBR-TEl2QbduSq2tG9sekOywE,1358
-searvey/usgs.py,sha256=NUkmI280SbmvHxN3O1YyGF5TbiKkD65eyuBGAikEOcM,14917
+searvey/usgs.py,sha256=pgwtdgbHX4kdB9likjjFFPnmwAwPrHTodwwcftTrfeE,15313
 searvey/utils.py,sha256=xQ_c6SrfYgOutLo2dV9-neD6I6dT-Xk4sdRctiWVjKY,4751
-searvey-0.3.2.dist-info/LICENSE,sha256=CsWICdCWFNMlGUJiXuxfrxFHw1uyVPns0jZJmzcWkjI,35145
-searvey-0.3.2.dist-info/METADATA,sha256=dlR9sTpg6z7ljM6mu19SEon5iBhH9N8ZYgXNw9_DoPo,4262
-searvey-0.3.2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-searvey-0.3.2.dist-info/RECORD,,
+searvey-0.3.3.dist-info/LICENSE,sha256=CsWICdCWFNMlGUJiXuxfrxFHw1uyVPns0jZJmzcWkjI,35145
+searvey-0.3.3.dist-info/METADATA,sha256=yfv5d1keRwyqmWbRcyIttBiTE8buwBm4q7NOPQYJhCw,4051
+searvey-0.3.3.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+searvey-0.3.3.dist-info/RECORD,,
```

