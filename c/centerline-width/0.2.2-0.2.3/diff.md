# Comparing `tmp/centerline-width-0.2.2.tar.gz` & `tmp/centerline-width-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/centerline-width-0.2.2.tar", last modified: Wed May 24 21:12:42 2023, max compression
+gzip compressed data, was "dist/centerline-width-0.2.3.tar", last modified: Fri May 26 07:16:36 2023, max compression
```

## Comparing `centerline-width-0.2.2.tar` & `centerline-width-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 21:12:42.731609 centerline-width-0.2.2/
--rw-rw-r--   0 user      (1000) user      (1000)    31128 2023-05-24 21:12:42.731609 centerline-width-0.2.2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    26334 2023-05-24 21:09:28.000000 centerline-width-0.2.2/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 21:12:42.727609 centerline-width-0.2.2/centerline_width/
--rw-rw-r--   0 user      (1000) user      (1000)     1382 2023-05-23 20:44:39.000000 centerline-width-0.2.2/centerline_width/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    20859 2023-05-24 21:09:07.000000 centerline-width-0.2.2/centerline_width/centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)    10941 2023-05-24 19:30:15.000000 centerline-width-0.2.2/centerline_width/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-0.2.2/centerline_width/getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)     8345 2023-05-24 20:50:36.000000 centerline-width-0.2.2/centerline_width/plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     6750 2023-05-24 20:32:04.000000 centerline-width-0.2.2/centerline_width/preprocessing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 21:12:42.731609 centerline-width-0.2.2/centerline_width/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)     6697 2023-05-17 22:00:19.000000 centerline-width-0.2.2/centerline_width/pytests/test_centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-0.2.2/centerline_width/pytests/test_getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)    11026 2023-05-17 04:31:11.000000 centerline-width-0.2.2/centerline_width/pytests/test_plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-0.2.2/centerline_width/pytests/test_preprocessing.py
--rw-rw-r--   0 user      (1000) user      (1000)     3397 2023-05-19 19:58:39.000000 centerline-width-0.2.2/centerline_width/pytests/test_riverCenterlineClass.py
--rw-rw-r--   0 user      (1000) user      (1000)     4569 2023-05-23 21:32:40.000000 centerline-width-0.2.2/centerline_width/riverCenterlineClass.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 21:12:42.727609 centerline-width-0.2.2/centerline_width.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    31128 2023-05-24 21:12:42.000000 centerline-width-0.2.2/centerline_width.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      700 2023-05-24 21:12:42.000000 centerline-width-0.2.2/centerline_width.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-24 21:12:42.000000 centerline-width-0.2.2/centerline_width.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-24 21:12:42.000000 centerline-width-0.2.2/centerline_width.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-05-24 21:12:42.000000 centerline-width-0.2.2/centerline_width.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-24 21:12:42.731609 centerline-width-0.2.2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1813 2023-05-24 21:04:30.000000 centerline-width-0.2.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-26 07:16:36.414115 centerline-width-0.2.3/
+-rw-rw-r--   0 user      (1000) user      (1000)    33829 2023-05-26 07:16:36.410114 centerline-width-0.2.3/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    28771 2023-05-26 07:15:14.000000 centerline-width-0.2.3/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-26 07:16:36.410114 centerline-width-0.2.3/centerline_width/
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-05-25 22:01:48.000000 centerline-width-0.2.3/centerline_width/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    21536 2023-05-26 06:59:06.000000 centerline-width-0.2.3/centerline_width/centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12386 2023-05-26 06:35:11.000000 centerline-width-0.2.3/centerline_width/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-0.2.3/centerline_width/getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7421 2023-05-26 06:06:57.000000 centerline-width-0.2.3/centerline_width/plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6750 2023-05-24 20:32:04.000000 centerline-width-0.2.3/centerline_width/preprocessing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-26 07:16:36.410114 centerline-width-0.2.3/centerline_width/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)     8687 2023-05-26 06:39:09.000000 centerline-width-0.2.3/centerline_width/pytests/test_centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-0.2.3/centerline_width/pytests/test_getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10312 2023-05-26 06:26:00.000000 centerline-width-0.2.3/centerline_width/pytests/test_plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-0.2.3/centerline_width/pytests/test_preprocessing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3397 2023-05-19 19:58:39.000000 centerline-width-0.2.3/centerline_width/pytests/test_riverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5202 2023-05-26 07:01:19.000000 centerline-width-0.2.3/centerline_width/riverCenterlineClass.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-26 07:16:36.410114 centerline-width-0.2.3/centerline_width.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    33829 2023-05-26 07:16:36.000000 centerline-width-0.2.3/centerline_width.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      700 2023-05-26 07:16:36.000000 centerline-width-0.2.3/centerline_width.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-26 07:16:36.000000 centerline-width-0.2.3/centerline_width.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-26 07:16:36.000000 centerline-width-0.2.3/centerline_width.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-05-26 07:16:36.000000 centerline-width-0.2.3/centerline_width.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-26 07:16:36.414115 centerline-width-0.2.3/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1813 2023-05-26 07:15:41.000000 centerline-width-0.2.3/setup.py
```

### Comparing `centerline-width-0.2.2/PKG-INFO` & `centerline-width-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.2.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.3.tar.gz
 Description: # Centerline-Width
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
         [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
         [![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
         
         Find the centerline and width of rivers based on the latitude and longitude positionss from the right and left bank 
@@ -17,15 +17,18 @@
         * **Convert raw data from Google Earth Pro to CSV**
         	* extractPointsToTextFile()
         	* convertColumnsToCSV()
         * **Find centerline and width of river**
         	* plotCenterline()
         	* plotCenterlineWidth()
         	* riverWidthFromCenterline()
-        	* centerlineLatitudeLongtiude
+        	* saveCenterlineCSV()
+        	* centerlineVoronoi
+        	* centerlineEvenlySpaced
+        	* centerlineSmoothed
         	* centerlineLength
         	* rightBankLength
         	* leftBankLength
         
         | River Outlined in Google Earth Pro | Generated Centerline for the River Bank |
         | ------------- | ------------- |
         | ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
@@ -65,21 +68,23 @@
         river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
         ```
         
         To plot the centerline, run the `plotCenterline()` function from `river_object` created
         ```python
         river_object.plotCenterline()
         ```
-        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_centerline.png)
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_centerline.png)
         
-        To plot the width of the river at intervals along the bank, run `plotCenterlineWidth` (apply_smoothing is optional and defaults to False, but is recommended)
+        To plot the width of the river at intervals along the bank, run `plotCenterlineWidth`
+        
+        While `apply_smoothing`, `remove_intersections`, and `display_true_centerline` are optional, they are recommended to generate a minimal width diagram
         ```python
-        river_object.plotCenterlineWidth(apply_smoothing=True)
+        river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
         ```
-        ![river_coords_width+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_width.png)
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_width.png)
         
         ## Preprocessing
         ### Convert KML files to Text File
         
         Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
         
         ```
@@ -142,15 +147,15 @@
         llat,llon,rlat,rlon
         30.037581,-92.868569,30.037441,-92.867476
         30.037613,-92.868549,30.037448,-92.867474
         30.037648,-92.868546,30.037482,-92.867449
         30.037674,-92.868536,30.037506,-92.867432
         30.037702,-92.868533,30.037525,-92.867430
         ```
-        Output: A csv file `data/river_coords.csv` with the headers llat, llon, rlat, rlon
+        Output: A csv file `data/river_coords.csv` with the headers `llat, llon, rlat, rlon`
         
         ## Centerline and Width
         ### River Object
         First, generate a river object to contain river data and available transformations
         ```
         centerline_width.riverCenterline(csv_data=None,
         				optional_cutoff=None,
@@ -162,15 +167,17 @@
         * [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
         * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
         
         Interpolating is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps dues to the combination of sparse data and a narrow river
         
         Object (class) useful attributes:
         
-        * centerlineLatitudeLongtiude (list of tuples): List of the latitude and longitude coordinates of the centerline
+        * centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
+        * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
+        * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
         * centerlineLength (float): Length of the centerline of the river (in km)
         * rightBankLength (float): Length of the right bank of the river (in km)
         * leftBankLength (float): Length of the left bank of the river (in km)
         
         Object (class) additional atttributes:
         
         * river_name (string): name of object, set to the csv_data string
@@ -182,50 +189,90 @@
         * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
         * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
         * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
         * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
         * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
         * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
         * interpolate_data (bool): if interpolating between existing data, defaults to False
-        * interpolate_n (int): specifies how many additional points will be added when interpolating data, defaults to 5
+        * interpolate_n (int): specifies how many additional points will be added between points along the river bank when interpolating data, defaults to 5
+        * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the the length of the dataframe (df_len)
+        
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         ```
         
         ### Return Latitude/Longitude Coordinates of Centerline
         Return the latitude/longitude coordinates of the centerline based on the left and right banks
+        
+        **Types of Centerlines**
+        There are three types of centerline coordinates formed from the river bank data. Each are built off of eachother and are used to clean and smooth data
+        - **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
+        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/voronoi_centerline.png)
+        - **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
+        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/evenly_spaced_centerline.png)
+        - **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
+        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/smoothed_centerline.png)
+        
+        Centerline coordinates are formed by the Voronoi vertices
+        ```
+        river_object.centerlineVoronoi
+        ```
+        
+        Centerline coordinates are formed by Evenly Spaced Voronoi vertices
+        ```
+        river_object.centerlineEvenlySpaced
+        ```
+        
+        Centerline coordinates are formed from Smoothed Voronoi vertices
         ```
-        river_object.centerlineLatitudeLongtiude
+        river_object.centerlineSmoothed
         ```
-        Centerline coordinates are formed from Voronoi vertices
         
+        Example:
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=15)
-        river_centerline_coordinates = river_object.centerlineLatitudeLongtiude
+        river_centerline_coordinates = river_object.centerlineVoronoi
         ```
         Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
         
+        ### Save Centerline Coordinates to a CSV
+        Save the centerline coordinates to a csv file with columns for latitude and longitude
+        
+        ```
+        saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
+        ```
+        * **[REQUIRED]** save_to_csv (str): CSV filename, requires a .csv extension
+        * [OPTIONAL] centerline_type (str): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed"], defaults to "Voronoi"
+        
+        ```python
+        import centerline_width
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+        river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
+        ```
+        
+        Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
+        
         ### Return Length of Centerline
-        Return the length of the centerline found between the left and right bank
+        Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
         ```
         river_object.centerlineLength
         ```
         Length returned in kilometers
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=550)
         river_centerline_length = river_object.centerlineLength
         ```
         The length of the river centerline returns `215.34700589636674` km
         
         ## Plot Centerline in Matplotlib
-        ### Plot the centerline created from a list of right and left banks with Voronoi vertices
+        Plot the centerline created from a list of right and left banks with Voronoi vertices
         
         ```
         plotCenterline(display_all_possible_paths=False, 
         		plot_title=None, 
         		save_plot_name=None, 
         		display_voronoi=False)
         ```
@@ -236,35 +283,33 @@
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.plotCenterline(display_all_possible_paths=False, display_voronoi=False)
         ```
         Output:
-        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_centerline.png)
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_centerline.png)
         
         ## Plot Centerline Width Lines in Matplotlib
         ### Plot the Centerline Width Lines
         Plot the width of the river based on the centerline
         
         Display Centerline at even intervals from the Voronoi generated centerline
         ```
         plotCenterlineWidth(plot_title=None, 
         		save_plot_name=None, 
         		display_true_centerline=True,
-        		n_interprolate_centerpoints=None,
         		transect_span_distance=3,
         		apply_smoothing=False,
         		flag_intersections=True,
         		remove_intersections=False)
         ```
         * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
         * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
         * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
-        * [OPTIONAL] n_interprolate_centerpoints (int): Recreate centerline coordinates with n evenly spaced points, defaults to the number of rows in the csv file
         * [OPTIONAL] transect_span_distance (int): Sum up n amount of points around a centerpoint to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
         * [OPTIONAL] flag_intersections (bool): Display intersecting width lines as red in graph, defaults to True
         * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to False
         
         **apply_smoothing**
         
@@ -292,42 +337,36 @@
         | remove_intersections=False | remove_intersections=True |
         | ------------- | ------------- |
         | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-        river_object.plotCenterlineWidth(save_plot_name="data/river_coords_width.png",
-        				display_true_centerline=False,
-        				n_interprolate_centerpoints=None,
-        				transect_span_distance=3,
-        				apply_smoothing=True,
-        				flag_intersections=True,
-        				remove_intersections=True)
+        river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
         ```
-        ![river_coords_width+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_width.png)
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_width.png)
         
         ### Return Width of River
         
-        Return the width of the river at each (evenly spaced) centerline coordinate
+        Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width`
         
         ```
-        riverWidthFromCenterline(n_interprolate_centerpoints=None,
-        			transect_span_distance=3,
+        riverWidthFromCenterline(transect_span_distance=3,
         			apply_smoothing=True,
         			remove_intersections=False,
         			units="km",
         			save_to_csv=None)
         ```
-        * [OPTIONAL] n_interprolate_centerpoints (int): Recreate centerline coordinates with n evenly spaced points, defaults to the number of rows in the csv file
         * [OPTIONAL] transect_span_distance (int): Sum up n amount of points around a centerpoint to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
         * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaultsl to True
         * [OPTIONAL] units (string): Units to measure distance, options: ["km" (kilometers), "m" (meters), "mi" (miles), "nmi" (nautical miles), "ft" (feet), "in" (inches), "rad" (radians), "deg" (degrees)], defaults to "km" (kilometers)
-        * [OPTIONAL] save_to_csv (string): Save river width output to a csv file, defaults to None (no file is saved)
+        * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
+        
+        Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordiantes may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
         							apply_smoothing=True,
         							units="km",
@@ -370,19 +409,14 @@
         
         **All vertices:**
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example4.png)
         
         **Vertices that have at least two connections (that would create gaps):**
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example5.png)
         
-        ### Types of Centerlines
-        - Voronoi centerline: centerline generated from where Voronoi vertices intersect within the river
-        - Evenly Spaced Centerline: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
-        - Smoothed Centerline: centerline generated from the evenly spaced centerline but smoothed by a b-spline
-        
         ## Debugging, Error Handling, and Edge Cases
         ### Wide Start/End of River
         If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example3.png)
         Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red) that sits along the longest path
         
         ### Invalid Polygon
@@ -422,15 +456,14 @@
         | interpolate_data = False | interpolate_data = True |
         | ------------- | ------------- |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
         
         The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
         
         ## Developer Notes: Tech Debt and Bug Fixes
-        * conversion of centerline lat-lon to meters
         * Fix legend overlapping on graph, replace doc_examples that have an overlapping
         * Verify that smoothing filter option does not produce a line that goes outside of the polygon
         
         ## Citations
         Based on work written in R (Golly et al. 2017):
         
         >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
```

### Comparing `centerline-width-0.2.2/README.md` & `centerline-width-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 * **Convert raw data from Google Earth Pro to CSV**
 	* extractPointsToTextFile()
 	* convertColumnsToCSV()
 * **Find centerline and width of river**
 	* plotCenterline()
 	* plotCenterlineWidth()
 	* riverWidthFromCenterline()
-	* centerlineLatitudeLongtiude
+	* saveCenterlineCSV()
+	* centerlineVoronoi
+	* centerlineEvenlySpaced
+	* centerlineSmoothed
 	* centerlineLength
 	* rightBankLength
 	* leftBankLength
 
 | River Outlined in Google Earth Pro | Generated Centerline for the River Bank |
 | ------------- | ------------- |
 | ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
@@ -57,21 +60,23 @@
 river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
 ```
 
 To plot the centerline, run the `plotCenterline()` function from `river_object` created
 ```python
 river_object.plotCenterline()
 ```
-![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_centerline.png)
+![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_centerline.png)
 
-To plot the width of the river at intervals along the bank, run `plotCenterlineWidth` (apply_smoothing is optional and defaults to False, but is recommended)
+To plot the width of the river at intervals along the bank, run `plotCenterlineWidth`
+
+While `apply_smoothing`, `remove_intersections`, and `display_true_centerline` are optional, they are recommended to generate a minimal width diagram
 ```python
-river_object.plotCenterlineWidth(apply_smoothing=True)
+river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
 ```
-![river_coords_width+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_width.png)
+![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_width.png)
 
 ## Preprocessing
 ### Convert KML files to Text File
 
 Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
 
 ```
@@ -134,15 +139,15 @@
 llat,llon,rlat,rlon
 30.037581,-92.868569,30.037441,-92.867476
 30.037613,-92.868549,30.037448,-92.867474
 30.037648,-92.868546,30.037482,-92.867449
 30.037674,-92.868536,30.037506,-92.867432
 30.037702,-92.868533,30.037525,-92.867430
 ```
-Output: A csv file `data/river_coords.csv` with the headers llat, llon, rlat, rlon
+Output: A csv file `data/river_coords.csv` with the headers `llat, llon, rlat, rlon`
 
 ## Centerline and Width
 ### River Object
 First, generate a river object to contain river data and available transformations
 ```
 centerline_width.riverCenterline(csv_data=None,
 				optional_cutoff=None,
@@ -154,15 +159,17 @@
 * [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
 * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
 
 Interpolating is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps dues to the combination of sparse data and a narrow river
 
 Object (class) useful attributes:
 
-* centerlineLatitudeLongtiude (list of tuples): List of the latitude and longitude coordinates of the centerline
+* centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
+* centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
+* centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
 * centerlineLength (float): Length of the centerline of the river (in km)
 * rightBankLength (float): Length of the right bank of the river (in km)
 * leftBankLength (float): Length of the left bank of the river (in km)
 
 Object (class) additional atttributes:
 
 * river_name (string): name of object, set to the csv_data string
@@ -174,50 +181,90 @@
 * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
 * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
 * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
 * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
 * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
 * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
 * interpolate_data (bool): if interpolating between existing data, defaults to False
-* interpolate_n (int): specifies how many additional points will be added when interpolating data, defaults to 5
+* interpolate_n (int): specifies how many additional points will be added between points along the river bank when interpolating data, defaults to 5
+* interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the the length of the dataframe (df_len)
+
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 ```
 
 ### Return Latitude/Longitude Coordinates of Centerline
 Return the latitude/longitude coordinates of the centerline based on the left and right banks
+
+**Types of Centerlines**
+There are three types of centerline coordinates formed from the river bank data. Each are built off of eachother and are used to clean and smooth data
+- **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
+![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/voronoi_centerline.png)
+- **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
+![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/evenly_spaced_centerline.png)
+- **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
+![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/smoothed_centerline.png)
+
+Centerline coordinates are formed by the Voronoi vertices
+```
+river_object.centerlineVoronoi
+```
+
+Centerline coordinates are formed by Evenly Spaced Voronoi vertices
+```
+river_object.centerlineEvenlySpaced
+```
+
+Centerline coordinates are formed from Smoothed Voronoi vertices
 ```
-river_object.centerlineLatitudeLongtiude
+river_object.centerlineSmoothed
 ```
-Centerline coordinates are formed from Voronoi vertices
 
+Example:
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=15)
-river_centerline_coordinates = river_object.centerlineLatitudeLongtiude
+river_centerline_coordinates = river_object.centerlineVoronoi
 ```
 Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
 
+### Save Centerline Coordinates to a CSV
+Save the centerline coordinates to a csv file with columns for latitude and longitude
+
+```
+saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
+```
+* **[REQUIRED]** save_to_csv (str): CSV filename, requires a .csv extension
+* [OPTIONAL] centerline_type (str): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed"], defaults to "Voronoi"
+
+```python
+import centerline_width
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
+```
+
+Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
+
 ### Return Length of Centerline
-Return the length of the centerline found between the left and right bank
+Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
 ```
 river_object.centerlineLength
 ```
 Length returned in kilometers
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=550)
 river_centerline_length = river_object.centerlineLength
 ```
 The length of the river centerline returns `215.34700589636674` km
 
 ## Plot Centerline in Matplotlib
-### Plot the centerline created from a list of right and left banks with Voronoi vertices
+Plot the centerline created from a list of right and left banks with Voronoi vertices
 
 ```
 plotCenterline(display_all_possible_paths=False, 
 		plot_title=None, 
 		save_plot_name=None, 
 		display_voronoi=False)
 ```
@@ -228,35 +275,33 @@
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.plotCenterline(display_all_possible_paths=False, display_voronoi=False)
 ```
 Output:
-![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_centerline.png)
+![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_centerline.png)
 
 ## Plot Centerline Width Lines in Matplotlib
 ### Plot the Centerline Width Lines
 Plot the width of the river based on the centerline
 
 Display Centerline at even intervals from the Voronoi generated centerline
 ```
 plotCenterlineWidth(plot_title=None, 
 		save_plot_name=None, 
 		display_true_centerline=True,
-		n_interprolate_centerpoints=None,
 		transect_span_distance=3,
 		apply_smoothing=False,
 		flag_intersections=True,
 		remove_intersections=False)
 ```
 * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
 * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
 * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
-* [OPTIONAL] n_interprolate_centerpoints (int): Recreate centerline coordinates with n evenly spaced points, defaults to the number of rows in the csv file
 * [OPTIONAL] transect_span_distance (int): Sum up n amount of points around a centerpoint to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
 * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
 * [OPTIONAL] flag_intersections (bool): Display intersecting width lines as red in graph, defaults to True
 * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to False
 
 **apply_smoothing**
 
@@ -284,42 +329,36 @@
 | remove_intersections=False | remove_intersections=True |
 | ------------- | ------------- |
 | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-river_object.plotCenterlineWidth(save_plot_name="data/river_coords_width.png",
-				display_true_centerline=False,
-				n_interprolate_centerpoints=None,
-				transect_span_distance=3,
-				apply_smoothing=True,
-				flag_intersections=True,
-				remove_intersections=True)
+river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
 ```
-![river_coords_width+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_width.png)
+![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_width.png)
 
 ### Return Width of River
 
-Return the width of the river at each (evenly spaced) centerline coordinate
+Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width`
 
 ```
-riverWidthFromCenterline(n_interprolate_centerpoints=None,
-			transect_span_distance=3,
+riverWidthFromCenterline(transect_span_distance=3,
 			apply_smoothing=True,
 			remove_intersections=False,
 			units="km",
 			save_to_csv=None)
 ```
-* [OPTIONAL] n_interprolate_centerpoints (int): Recreate centerline coordinates with n evenly spaced points, defaults to the number of rows in the csv file
 * [OPTIONAL] transect_span_distance (int): Sum up n amount of points around a centerpoint to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
 * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
 * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaultsl to True
 * [OPTIONAL] units (string): Units to measure distance, options: ["km" (kilometers), "m" (meters), "mi" (miles), "nmi" (nautical miles), "ft" (feet), "in" (inches), "rad" (radians), "deg" (degrees)], defaults to "km" (kilometers)
-* [OPTIONAL] save_to_csv (string): Save river width output to a csv file, defaults to None (no file is saved)
+* [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
+
+Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordiantes may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
 							apply_smoothing=True,
 							units="km",
@@ -362,19 +401,14 @@
 
 **All vertices:**
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example4.png)
 
 **Vertices that have at least two connections (that would create gaps):**
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example5.png)
 
-### Types of Centerlines
-- Voronoi centerline: centerline generated from where Voronoi vertices intersect within the river
-- Evenly Spaced Centerline: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
-- Smoothed Centerline: centerline generated from the evenly spaced centerline but smoothed by a b-spline
-
 ## Debugging, Error Handling, and Edge Cases
 ### Wide Start/End of River
 If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example3.png)
 Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red) that sits along the longest path
 
 ### Invalid Polygon
@@ -414,15 +448,14 @@
 | interpolate_data = False | interpolate_data = True |
 | ------------- | ------------- |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
 
 The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
 
 ## Developer Notes: Tech Debt and Bug Fixes
-* conversion of centerline lat-lon to meters
 * Fix legend overlapping on graph, replace doc_examples that have an overlapping
 * Verify that smoothing filter option does not produce a line that goes outside of the polygon
 
 ## Citations
 Based on work written in R (Golly et al. 2017):
 
 >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
```

### Comparing `centerline-width-0.2.2/centerline_width/__init__.py` & `centerline-width-0.2.3/centerline_width/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 from .centerline import centerlinePath
 from .centerline import networkXGraphShortestPath
 from .centerline import centerlineLength
 from .centerline import evenlySpacedCenterline
 from .centerline import smoothedCoordinates
 from .centerline import riverWidthFromCenterlineCoordinates
 from .centerline import riverWidthFromCenterline
+from .centerline import saveCenterlineCSV
 
 # plotDiagrams.py function calls
 from .plotDiagrams import plotCenterline
 from .plotDiagrams import plotCenterlineWidth
 
 # error_handling.py function calls
 from .error_handling import errrorHandlingConvertColumnsToCSV
 from .error_handling import errorHandlingPlotCenterline
 from .error_handling import errorHandlingPlotCenterlineWidth
 from .error_handling import errorHandlingRiverWidthFromCenterline
+from .error_handling import errorHandlingSaveCenterlineCSV
 from .error_handling import errorHandlingExtractPointsToTextFile
 from .error_handling import errorHandlingRiverCenterlineClass
```

### Comparing `centerline-width-0.2.2/centerline_width/centerline.py` & `centerline-width-0.2.3/centerline_width/centerline.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 		logger.critical("\nCRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.")
 		shortest_path_points = None
 	else:
 		shortest_path_points = networkXGraphShortestPath(nx_graphs, starting_node, ending_node)
 
 	return starting_node, ending_node, x_ridge_point, y_ridge_point, shortest_path_points
 
-def evenlySpacedCenterline(centerline_coordinates=None, number_of_fixed_points=10):
+def evenlySpacedCenterline(centerline_coordinates=None, number_of_fixed_points=None):
 	# Interpolate to evenly space points along the centerline coordinates (effectively smoothing with fewer points)
 	if centerline_coordinates is None:
 		return None
 
 	centerline_line = LineString(centerline_coordinates)
 
 	# Splitting into a fixed number of points
@@ -299,67 +299,61 @@
 			del right_width_coordinates[centerline_coord]
 			del left_width_coordinates[centerline_coord]
 		logger.info("[SUCCESS] Intersection lines removed")
 
 	return right_width_coordinates, left_width_coordinates, num_intersection_coordinates
 
 def riverWidthFromCenterline(river_object=None,
-							n_interprolate_centerpoints=None,
 							transect_span_distance=3,
 							apply_smoothing=True,
 							remove_intersections=False,
 							units="km",
 							save_to_csv=None):
 	# Return river width: centerline and width at centerline
 	# Width is measured to the bank, relative to the center point (normal of the centerline)
 	# { [centerline latitude, centerline longitude] : widthValue }
 
 	centerline_width.errorHandlingRiverWidthFromCenterline(river_object=river_object,
-															n_interprolate_centerpoints=n_interprolate_centerpoints,
 															transect_span_distance=transect_span_distance,
 															apply_smoothing=apply_smoothing,
 															remove_intersections=remove_intersections,
 															units=units,
 															save_to_csv=save_to_csv)
 
-	if n_interprolate_centerpoints is None:
-		# if plotting width, but n_interprolate_centerpoints is undefined, set to the size of the dataframe
-		n_interprolate_centerpoints = river_object.df_len
-
-	if river_object.centerlineLatitudeLongtiude is None:
+	if river_object.centerlineVoronoi is None:
 		logger.critical("\nCRITICAL ERROR, unable to find width without a valid centerline")
 		return None
 
 	# recreate the centerline with evenly spaced points
-	defined_centerline_coordinates = centerline_width.evenlySpacedCenterline(centerline_coordinates=river_object.centerlineLatitudeLongtiude,
-																			number_of_fixed_points=n_interprolate_centerpoints)
+	defined_centerline_coordinates = centerline_width.evenlySpacedCenterline(centerline_coordinates=river_object.centerlineVoronoi,
+																			number_of_fixed_points=river_object.interpolate_n_centerpoints)
 	if apply_smoothing:
-		defined_centerline_coordinates = centerline_width.smoothedCoordinates(centerline_coordinates=river_object.centerlineLatitudeLongtiude,
-																				interprolate_num=n_interprolate_centerpoints)
+		defined_centerline_coordinates = centerline_width.smoothedCoordinates(centerline_coordinates=river_object.centerlineVoronoi,
+																				interprolate_num=river_object.interpolate_n_centerpoints)
 	# if using smoothing, replace left/right coordinates with the smoothed variation
 	right_width_coord, left_width_coord, _ = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object, 
-																									centerline_coordinates=defined_centerline_coordinates,
-																									transect_span_distance=transect_span_distance,
-																									remove_intersections=remove_intersections)
+																								centerline_coordinates=defined_centerline_coordinates,
+																								transect_span_distance=transect_span_distance,
+																								remove_intersections=remove_intersections)
 
 	width_dict = {}
 	for centerline_coord, _ in right_width_coord.items():
 		# store the haversine distance between the lat/lon position of the right/left bank
 		lon1, lat1 = right_width_coord[centerline_coord]
 		lon2, lat2 = left_width_coord[centerline_coord]
 		haversine_distance_between_right_and_left = haversine((lat1, lon1), (lat2, lon2), unit=units)
 		width_dict[centerline_coord] = haversine_distance_between_right_and_left
 
 	# Save width dictionary to a csv file (Latitude, Longtiude, Width)
 	if save_to_csv:
 		with open(save_to_csv, "w") as csv_file_output:
 			writer = csv.writer(csv_file_output)
-			writer.writerow(["Centerline Latitude (°)", "Centerline Longitude (°)", "Width ({0})".format(units)])
+			writer.writerow(["Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width ({0})".format(units)])
 			for coordinate_key, width_value in width_dict.items():
-				writer.writerow([coordinate_key[0], coordinate_key[1], width_value])
+				writer.writerow([coordinate_key[1], coordinate_key[0], width_value])
 
 	return width_dict
 
 def centerlineLength(centerline_coordinates=None):
 	# Return the length/distance for all the centerline coordaintes in km
 	total_length = 0
 	previous_pair = None
@@ -371,7 +365,22 @@
 			previous_pair = xy_pair
 		else:
 			lon1, lon2 = previous_pair[0], xy_pair[0]
 			lat1, lat2 = previous_pair[1], xy_pair[1]
 			distance_to_add = haversine((lat1, lon1), (lat2, lon2), unit="km")
 			total_length += distance_to_add
 	return total_length
+
+def saveCenterlineCSV(river_object=None, save_to_csv=None, centerline_type="Voronoi"):
+	# Save Centerline Coordinates generated by Voronoi Diagram to CSV
+	centerline_width.errorHandlingSaveCenterlineCSV(river_object=river_object, save_to_csv=save_to_csv, centerline_type=centerline_type)
+	centerline_type = centerline_type.title()
+
+	if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoi
+	if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
+	if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothed
+
+	with open(save_to_csv, "w") as csv_file_output:
+		writer = csv.writer(csv_file_output)
+		writer.writerow(["{0} Centerline Latitude (Deg)".format(centerline_type), "{0} Centerline Longitude (Deg)".format(centerline_type)])
+		for latitude_longitude in centerline_coordinates_by_type:
+			writer.writerow([latitude_longitude[1], latitude_longitude[0]])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `centerline-width-0.2.2/centerline_width/error_handling.py` & `centerline-width-0.2.3/centerline_width/error_handling.py`

 * *Files 15% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 		logger.critical("\nCRITICAL ERROR, [display_voronoi]: Must be a bool, current type = '{0}'".format(type(display_voronoi)))
 		exit()
 
 def errorHandlingPlotCenterlineWidth(river_object=None,
 									plot_title=None,
 									save_plot_name=None,
 									display_true_centerline=None,
-									n_interprolate_centerpoints=None,
 									transect_span_distance=None,
 									apply_smoothing=None,
 									flag_intersections=None,
 									remove_intersections=None):
 	# Error handling for plotCenterlineWidth()
 	if river_object is None:
 		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
@@ -92,23 +91,14 @@
 		logger.critical("\nCRITICAL ERROR, [save_plot_name]: Must be a str, current type = '{0}'".format(type(save_plot_name)))
 		exit()
 
 	if type(display_true_centerline) != bool:
 		logger.critical("\nCRITICAL ERROR, [display_true_centerline]: Must be a bool, current type = '{0}'".format(type(display_true_centerline)))
 		exit()
 
-	if n_interprolate_centerpoints is not None:
-		if type(n_interprolate_centerpoints) != int:
-			logger.critical("\nCRITICAL ERROR, [n_interprolate_centerpoints]: Must be a int, current type = '{0}'".format(type(n_interprolate_centerpoints)))
-			exit()
-		else:
-			if n_interprolate_centerpoints < 2:
-				logger.critical("\nCRITICAL ERROR, [n_interprolate_centerpoints]: Must be a greater than 1, currently = '{0}'".format(n_interprolate_centerpoints))
-				exit()
-
 	if type(transect_span_distance) != int:
 		logger.critical("\nCRITICAL ERROR, [transect_span_distance]: Must be a int, current type = '{0}'".format(type(transect_span_distance)))
 		exit()
 	else:
 		if transect_span_distance < 3:
 			logger.critical("\nCRITICAL ERROR, [transect_span_distance]: Must be a greater than 2 to find the slope between at least two points, currently = '{0}'".format(transect_span_distance))
 			exit()
@@ -124,34 +114,28 @@
 
 	if type(remove_intersections) != bool:
 		logger.critical("\nCRITICAL ERROR, [remove_intersections]: Must be a bool, current type = '{0}'".format(type(remove_intersections)))
 		exit()
 
 ## Error Handling: centerline.py
 def errorHandlingRiverWidthFromCenterline(river_object=None,
-										n_interprolate_centerpoints=None,
 										transect_span_distance=None,
 										apply_smoothing=None,
 										remove_intersections=None,
 										units=None,
 										save_to_csv=None):
 	# Error Handling for riverWidthFromCenterline()
 	if river_object is None:
 		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
 		exit()
 	else:
 		if not isinstance(river_object, centerline_width.riverCenterline):
 			logger.critical("\nCRITICAL ERROR, [river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{0}'".format(type(river_object)))
 			exit()
 
-	if n_interprolate_centerpoints is not None:
-		if type(n_interprolate_centerpoints) != int:
-			logger.critical("\nCRITICAL ERROR, [n_interprolate_centerpoints]: Must be a int, current type = '{0}'".format(type(n_interprolate_centerpoints)))
-			exit()
-
 	if transect_span_distance is not None:
 		if type(transect_span_distance) != int:
 			logger.critical("\nCRITICAL ERROR, [transect_span_distance]: Must be a int, current type = '{0}'".format(type(transect_span_distance)))
 			exit()
 		else:
 			if transect_span_distance < 3:
 				logger.critical("\nCRITICAL ERROR, [transect_span_distance]: Must be greater than 2, currently = '{0}'".format(transect_span_distance))
@@ -170,17 +154,52 @@
 			logger.critical("\nCRITICAL ERROR, [units]: Must be a str, current type = '{0}'".format(type(units)))
 			exit()
 	else:
 		if units not in units_options:
 			logger.critical("\nCRITICAL ERROR, [units]: Must be an option available ({0}), current given option = '{1}'".format(units_options, units))
 			exit()
 
-	if save_to_csv is not None and type(save_to_csv) != str:
+	if save_to_csv is not None:
+		if type(save_to_csv) != str:
+			logger.critical("\nCRITICAL ERROR, [save_to_csv]: Must be a str, current type = '{0}'".format(type(save_to_csv)))
+			exit()
+		if not save_to_csv.lower().endswith(".csv"):
+			logger.critical("\nCRITICAL ERROR, [save_to_csv]: Extension must be a .csv file, current extension = '{0}'".format(save_to_csv.split(".")[1]))
+			exit()
+
+def errorHandlingSaveCenterlineCSV(river_object=None, save_to_csv=None, centerline_type=None):
+	# Error Handling for saveCenterlineCSV()
+	if river_object is None:
+		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
+		exit()
+	else:
+		if not isinstance(river_object, centerline_width.riverCenterline):
+			logger.critical("\nCRITICAL ERROR, [river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{0}'".format(type(river_object)))
+			exit()
+
+	if save_to_csv is None:
+		logger.critical("\nCRITICAL ERROR, [save_to_csv]: Requires csv filename")
+		exit()
+	else:
+		if type(save_to_csv) != str:
 			logger.critical("\nCRITICAL ERROR, [save_to_csv]: Must be a str, current type = '{0}'".format(type(save_to_csv)))
 			exit()
+		else:
+			if not save_to_csv.lower().endswith(".csv"):
+				logger.critical("\nCRITICAL ERROR, [save_to_csv]: Extension must be a .csv file, current extension = '{0}'".format(save_to_csv.split(".")[1]))
+				exit()
+
+	centerline_type_options = ["Voronoi", "Evenly Spaced", "Smoothed"]
+	if type(centerline_type) != str:
+		logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be a str, current type = '{0}'".format(type(centerline_type)))
+		exit()
+	else:
+		if centerline_type.title() not in centerline_type_options:
+			logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be an available option in {0}, current option = '{1}'".format(centerline_type_options, centerline_type))
+			exit()
 
 # Error Handling: getCoordinatesKML.py
 def errorHandlingExtractPointsToTextFile(left_kml=None, right_kml=None, text_output_name=None):
 	# Error Handling for extractPointsToTextFile()
 	if left_kml is None:
 		logger.critical("\nCRITICAL ERROR, [left_kml]: Requires left_kml file")
 		exit()
@@ -212,15 +231,19 @@
 		exit()
 	else:
 		if type(text_output_name) != str:
 			logger.critical("\nCRITICAL ERROR, [text_output_name]: Must be a str, current type = '{0}'".format(type(text_output_name)))
 			exit()
 
 ## Error Handling: riverCenterlineClass.py
-def errorHandlingRiverCenterlineClass(csv_data=None, optional_cutoff=None, interpolate_data=None, interpolate_n=None):
+def errorHandlingRiverCenterlineClass(csv_data=None,
+									optional_cutoff=None,
+									interpolate_data=None,
+									interpolate_n=None,
+									interpolate_n_centerpoints=None):
 	# Error Handling for riverCenterlineClass()
 	if csv_data is None:
 		logger.critical("\nCRITICAL ERROR, [csv_data]: Requires csv_data location")
 		exit()
 	else:
 		if type(csv_data) != str and not isinstance(csv_data, StringIO): 
 			# StringIO accounts for testing against a StringIO instead of a CSV (used in pytests)
@@ -237,7 +260,16 @@
 		exit()
 
 	if type(interpolate_n) != int:
 		logger.critical("\nCRITICAL ERROR, [interpolate_n]: Must be a int, current type = '{0}'".format(type(interpolate_n)))
 		exit()
 		if interpolate_n > 15:
 			logger.warn("WARNING, [interpolate_n]: Setting interpolate_n above 15 will cause the code to execute exponentially slower")
+
+	if interpolate_n_centerpoints is not None:
+		if type(interpolate_n_centerpoints) != int:
+			logger.critical("\nCRITICAL ERROR, [interpolate_n_centerpoints]: Must be a int, current type = '{0}'".format(type(interpolate_n_centerpoints)))
+			exit()
+		else:
+			if interpolate_n_centerpoints < 2:
+				logger.critical("\nCRITICAL ERROR, [interpolate_n_centerpoints]: Must be a greater than 1, currently = '{0}'".format(interpolate_n_centerpoints))
+				exit()
```

### Comparing `centerline-width-0.2.2/centerline_width/getCoordinatesKML.py` & `centerline-width-0.2.3/centerline_width/getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.2/centerline_width/plotDiagrams.py` & `centerline-width-0.2.3/centerline_width/plotDiagrams.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ## Logging set up for .INFO
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 stream_handler = logging.StreamHandler()
 logger.addHandler(stream_handler)
 
-def plotCenterlineBackend(river_object=None):
+def plotCenterlineBackend(river_object=None, display_true_centerline=True):
 	# Shared components between plotCenterline and plotCenterlineWidth
 	fig = plt.figure(figsize=(10,10))
 	ax = fig.add_subplot(111)
 	
 	# Plot River as a Polygon
 	plt.plot(*river_object.bank_polygon.exterior.xy, c="gainsboro")
 	plt.plot(*river_object.top_bank.xy, c="forestgreen")
@@ -37,23 +37,24 @@
 	for i in river_object.left_bank_coordinates:
 		x.append(i[0])
 		y.append(i[1])
 	plt.scatter(x, y, c="orange", s=scatter_plot_size, label="Left Bank")
 
 	# Plot centerline found from NetworkX
 	valid_path_through = False
-	if river_object.centerlineLatitudeLongtiude: # shortest path through points
+	if river_object.centerlineVoronoi: # shortest path through points
 		valid_path_through = True
 		x = []
 		y = []
-		for k, v in river_object.centerlineLatitudeLongtiude:
+		for k, v in river_object.centerlineVoronoi:
 			x.append(k)
 			y.append(v)
-		#plt.scatter(x, y, c="slategray", label="Centerline Coordinates", s=5)
-		plt.plot(*zip(*river_object.centerlineLatitudeLongtiude), c="black", label="Centerline")
+		#plt.scatter(x, y, c="black", label="Centerline Coordinates", s=8)
+		if display_true_centerline:
+			plt.plot(*zip(*river_object.centerlineVoronoi), c="black", label="Centerline")
 
 	# Dynamically assign the starting and ending
 	if river_object.starting_node is not None: # error handling for when data is too small to generate centerline coordiantes
 			plt.scatter(river_object.starting_node[0], river_object.starting_node[1], c="green", label="Starting Node", s=45)
 			plt.scatter(river_object.ending_node[0], river_object.ending_node[1], c="red", label="Ending Node", s=45)
 
 	return fig, ax, valid_path_through
@@ -92,82 +93,65 @@
 	plt.show()
 	if save_plot_name: fig.savefig(save_plot_name)
 
 def plotCenterlineWidth(river_object=None,
 						plot_title=None, 
 						save_plot_name=None, 
 						display_true_centerline=True,
-						n_interprolate_centerpoints=None,
 						transect_span_distance=3,
 						apply_smoothing=False,
 						flag_intersections=True,
 						remove_intersections=False):
 	# Plot Width Lines based on Centerline
 	centerline_width.errorHandlingPlotCenterlineWidth(river_object=river_object,
 													plot_title=plot_title, 
 													save_plot_name=save_plot_name, 
 													display_true_centerline=display_true_centerline,
-													n_interprolate_centerpoints=n_interprolate_centerpoints,
 													transect_span_distance=transect_span_distance,
 													apply_smoothing=apply_smoothing,
 													flag_intersections=flag_intersections,
 													remove_intersections=remove_intersections)
 
-	fig, ax, valid_path_through = plotCenterlineBackend(river_object=river_object)
+	fig, ax, valid_path_through = plotCenterlineBackend(river_object=river_object, display_true_centerline=display_true_centerline)
 
 	# Plot river
-	if n_interprolate_centerpoints is None:
-		# if plotting width, but n_interprolate_centerpoints is undefined, set to the size of the dataframe
-		n_interprolate_centerpoints = river_object.df_len
 
 	# Determine the Width of River
 	number_of_evenly_spaced_points = ""
 
-	if river_object.centerlineLatitudeLongtiude is not None:
-		number_of_evenly_spaced_points = "\nCenterline made of {0} Fixed Points, width lines generated every {1} points".format(n_interprolate_centerpoints, transect_span_distance)
+	if river_object.centerlineVoronoi is not None:
+		number_of_evenly_spaced_points = "\nCenterline made of {0} Fixed Points, width lines generated every {1} points".format(river_object.interpolate_n_centerpoints, transect_span_distance)
 		if river_object.starting_node is not None: # error handling for when data is too small to generate centerline coordiantes
-			# recreate the centerline with evenly spaced points
-			evenly_spaced_centerline_coordinates = centerline_width.evenlySpacedCenterline(centerline_coordinates=river_object.centerlineLatitudeLongtiude,
-																						number_of_fixed_points=n_interprolate_centerpoints)
 			if apply_smoothing:
-				smoothed_centerline_coordinates = centerline_width.smoothedCoordinates(centerline_coordinates=river_object.centerlineLatitudeLongtiude,
-																						interprolate_num=n_interprolate_centerpoints)
 				# if using smoothing, replace left/right coordinates with the smoothed variation
 				right_width_coordinates, left_width_coordinates, num_intersection_coordinates = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object,
-																																					centerline_coordinates=smoothed_centerline_coordinates,
+																																					centerline_coordinates=river_object.centerlineSmoothed,
 																																					transect_span_distance=transect_span_distance,
 																																					remove_intersections=remove_intersections)
 				x = []
 				y = []
-				for k, v in smoothed_centerline_coordinates:
+				for k, v in river_object.centerlineSmoothed:
 					x.append(k)
 					y.append(v)
 				plt.scatter(x, y, c="blue", label="Smoothed Centerline Coordinates", s=5)
-				plt.plot(*zip(*smoothed_centerline_coordinates), "--", c="lightblue", label="Smoothed Centerline")
 			else:
+				# recreate the centerline with evenly spaced points
 				right_width_coordinates, left_width_coordinates, num_intersection_coordinates = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object, 
-																														centerline_coordinates=evenly_spaced_centerline_coordinates,
+																														centerline_coordinates=river_object.centerlineEvenlySpaced,
 																														transect_span_distance=transect_span_distance,
 																														remove_intersections=remove_intersections)
 
-			x = []
-			y = []
-			for k, v in evenly_spaced_centerline_coordinates:
-				x.append(k)
-				y.append(v)
-			#plt.scatter(x, y, c="plum", label="Evenly Spaced Centerline Coordinates", s=20)
+			#x = []
+			#y = []
+			#for k, v in evenly_spaced_centerline_coordinates:
+			#	x.append(k)
+			#	y.append(v)
+			#plt.scatter(x, y, c="plum", label="Evenly Spaced Centerline Coordinates", s=8)
 			#plt.plot(*zip(*evenly_spaced_centerline_coordinates), "--", c="thistle", label="Evenly Spaced Centerline")
 
-			x = []
-			y = []
-			for k, v in right_width_coordinates.items():
-				x.append(k[0])
-				y.append(k[1])
-			plt.scatter(x, y, c="purple", label="Every X Number", s=5)
-
 			for center_coord, edge_coord in right_width_coordinates.items():
 				x_points = (right_width_coordinates[center_coord][0], left_width_coordinates[center_coord][0])
 				y_points = (right_width_coordinates[center_coord][1], left_width_coordinates[center_coord][1])
 				if flag_intersections:
 					if num_intersection_coordinates[center_coord] > 0:
 						if remove_intersections:
 							logger.error("\nERROR: Unable to completely resolve all intersections lines to be removed")
```

### Comparing `centerline-width-0.2.2/centerline_width/preprocessing.py` & `centerline-width-0.2.3/centerline_width/preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.2/centerline_width/pytests/test_getCoordinatesKML.py` & `centerline-width-0.2.3/centerline_width/pytests/test_getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.2/centerline_width/pytests/test_plotDiagrams.py` & `centerline-width-0.2.3/centerline_width/pytests/test_plotDiagrams.py`

 * *Files 9% similar despite different names*

```diff
@@ -133,23 +133,14 @@
 	with pytest.raises(SystemExit):
 		centerline_width.plotCenterlineWidth(river_object=river_class_example,
 											display_true_centerline=display_true_centerline_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [display_true_centerline]: Must be a bool, current type = '{0}'".format(display_true_centerline_error_output)
 
-@pytest.mark.parametrize("n_interprolate_centerpoints_invalid, n_interprolate_centerpoints_error_output", invalid_non_int_options)
-def test_plotCenterlineWidth_nInterprolateCenterpointsInvalidTypes(caplog, n_interprolate_centerpoints_invalid, n_interprolate_centerpoints_error_output):
-	with pytest.raises(SystemExit):
-		centerline_width.plotCenterlineWidth(river_object=river_class_example,
-											n_interprolate_centerpoints=n_interprolate_centerpoints_invalid)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [n_interprolate_centerpoints]: Must be a int, current type = '{0}'".format(n_interprolate_centerpoints_error_output)
-
 @pytest.mark.parametrize("transect_span_distance_invalid, transect_span_distance_error_output", invalid_non_int_options)
 def test_plotCenterlineWidth_transectSpanDistanceInvalidTypes(caplog, transect_span_distance_invalid, transect_span_distance_error_output):
 	with pytest.raises(SystemExit):
 		centerline_width.plotCenterlineWidth(river_object=river_class_example,
 											transect_span_distance=transect_span_distance_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
```

### Comparing `centerline-width-0.2.2/centerline_width/pytests/test_preprocessing.py` & `centerline-width-0.2.3/centerline_width/pytests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.2/centerline_width/pytests/test_riverCenterlineClass.py` & `centerline-width-0.2.3/centerline_width/pytests/test_riverCenterlineClass.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.2/centerline_width/riverCenterlineClass.py` & `centerline-width-0.2.3/centerline_width/riverCenterlineClass.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,28 +3,31 @@
 # External Python libraries (installed via pip install)
 import pandas as pd
 
 # Internal centerline_width reference to access functions, global variables, and error handling
 import centerline_width
 
 class riverCenterline:
-	def __init__(self, csv_data=None, optional_cutoff=None, interpolate_data=False, interpolate_n=5):
+	def __init__(self, csv_data=None, optional_cutoff=None, interpolate_data=False, interpolate_n=5, interpolate_n_centerpoints=None):
 		centerline_width.errorHandlingRiverCenterlineClass(csv_data=csv_data,
 															optional_cutoff=optional_cutoff,
 															interpolate_data=interpolate_data,
-															interpolate_n=interpolate_n)
+															interpolate_n=interpolate_n,
+															interpolate_n_centerpoints=interpolate_n_centerpoints)
 
 		# Description and dataframe
 		self.river_name = csv_data
 		self.interpolate_data = interpolate_data
 		self.interpolate_n = interpolate_n
 		df = pd.read_csv(csv_data)
 		if optional_cutoff:
 			df = df.head(optional_cutoff)
 		self.df_len = len(df)
+		self.interpolate_n_centerpoints = interpolate_n_centerpoints
+		if self.interpolate_n_centerpoints is None: self.interpolate_n_centerpoints = self.df_len
 
 		# Left and Right Coordinates from the given csv data and data cutoff
 		left_bank_coordinates, right_bank_coordinates = centerline_width.leftRightCoordinates(df)
 		if interpolate_data:
 			right_bank_coordinates, left_bank_coordinates = centerline_width.interpolateBetweenPoints(left_bank_coordinates, right_bank_coordinates, interpolate_n)
 		self.left_bank_coordinates = left_bank_coordinates
 		self.right_bank_coordinates = right_bank_coordinates
@@ -43,15 +46,19 @@
 		starting_node, ending_node, x_ridge_point, y_ridge_point, shortest_path_coordinates = centerline_width.centerlinePath(self.bank_voronoi, self.bank_polygon, self.top_bank, self.bottom_bank)
 		self.starting_node = starting_node # starting position for centerline
 		self.ending_node = ending_node # ending position for centerline
 		self.x_voronoi_ridge_point = x_ridge_point # Voronoi x positions
 		self.y_voronoi_ridge_point = y_ridge_point # Voronoi y postions
 
 		# Centerline coordinates
-		self.centerlineLatitudeLongtiude = shortest_path_coordinates
+		self.centerlineVoronoi = shortest_path_coordinates
+		self.centerlineEvenlySpaced = centerline_width.evenlySpacedCenterline(centerline_coordinates=self.centerlineVoronoi,
+																						number_of_fixed_points=self.interpolate_n_centerpoints)
+		self.centerlineSmoothed = centerline_width.smoothedCoordinates(centerline_coordinates=self.centerlineEvenlySpaced,
+																						interprolate_num=self.interpolate_n_centerpoints)
 
 		# Right/Length Bank Length
 		self.rightBankLength = centerline_width.centerlineLength(centerline_coordinates=right_bank_coordinates)
 		self.leftBankLength = centerline_width.centerlineLength(centerline_coordinates=left_bank_coordinates)
 
 		# Centerline length
 		self.centerlineLength = centerline_width.centerlineLength(centerline_coordinates=shortest_path_coordinates)
@@ -67,36 +74,37 @@
 										save_plot_name=save_plot_name, 
 										display_voronoi=display_voronoi)
 
 	def plotCenterlineWidth(self,
 							plot_title=None, 
 							save_plot_name=None, 
 							display_true_centerline=True,
-							n_interprolate_centerpoints=None,
 							transect_span_distance=3,
 							apply_smoothing=False,
 							flag_intersections=True,
 							remove_intersections=False):
 		centerline_width.plotCenterlineWidth(river_object=self,
 											plot_title=plot_title, 
 											save_plot_name=save_plot_name, 
 											display_true_centerline=display_true_centerline,
-											n_interprolate_centerpoints=n_interprolate_centerpoints,
 											transect_span_distance=transect_span_distance,
 											apply_smoothing=apply_smoothing,
 											flag_intersections=flag_intersections,
 											remove_intersections=remove_intersections)
 
 	def riverWidthFromCenterline(self,
-								n_interprolate_centerpoints=None,
 								transect_span_distance=3,
 								apply_smoothing=True,
 								remove_intersections=False,
 								units="km",
 								save_to_csv=None):
 		return centerline_width.riverWidthFromCenterline(river_object=self,
-														n_interprolate_centerpoints=n_interprolate_centerpoints,
 														transect_span_distance=transect_span_distance,
 														apply_smoothing=apply_smoothing,
 														remove_intersections=remove_intersections,
 														units=units,
 														save_to_csv=save_to_csv)
+
+	def saveCenterlineCSV(self, save_to_csv=None, centerline_type="Voronoi"):
+		return centerline_width.saveCenterlineCSV(river_object=self,
+												save_to_csv=save_to_csv,
+												centerline_type=centerline_type)
```

### Comparing `centerline-width-0.2.2/centerline_width.egg-info/PKG-INFO` & `centerline-width-0.2.3/centerline_width.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.2.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.3.tar.gz
 Description: # Centerline-Width
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
         [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
         [![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
         
         Find the centerline and width of rivers based on the latitude and longitude positionss from the right and left bank 
@@ -17,15 +17,18 @@
         * **Convert raw data from Google Earth Pro to CSV**
         	* extractPointsToTextFile()
         	* convertColumnsToCSV()
         * **Find centerline and width of river**
         	* plotCenterline()
         	* plotCenterlineWidth()
         	* riverWidthFromCenterline()
-        	* centerlineLatitudeLongtiude
+        	* saveCenterlineCSV()
+        	* centerlineVoronoi
+        	* centerlineEvenlySpaced
+        	* centerlineSmoothed
         	* centerlineLength
         	* rightBankLength
         	* leftBankLength
         
         | River Outlined in Google Earth Pro | Generated Centerline for the River Bank |
         | ------------- | ------------- |
         | ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
@@ -65,21 +68,23 @@
         river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
         ```
         
         To plot the centerline, run the `plotCenterline()` function from `river_object` created
         ```python
         river_object.plotCenterline()
         ```
-        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_centerline.png)
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_centerline.png)
         
-        To plot the width of the river at intervals along the bank, run `plotCenterlineWidth` (apply_smoothing is optional and defaults to False, but is recommended)
+        To plot the width of the river at intervals along the bank, run `plotCenterlineWidth`
+        
+        While `apply_smoothing`, `remove_intersections`, and `display_true_centerline` are optional, they are recommended to generate a minimal width diagram
         ```python
-        river_object.plotCenterlineWidth(apply_smoothing=True)
+        river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
         ```
-        ![river_coords_width+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_width.png)
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_width.png)
         
         ## Preprocessing
         ### Convert KML files to Text File
         
         Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
         
         ```
@@ -142,15 +147,15 @@
         llat,llon,rlat,rlon
         30.037581,-92.868569,30.037441,-92.867476
         30.037613,-92.868549,30.037448,-92.867474
         30.037648,-92.868546,30.037482,-92.867449
         30.037674,-92.868536,30.037506,-92.867432
         30.037702,-92.868533,30.037525,-92.867430
         ```
-        Output: A csv file `data/river_coords.csv` with the headers llat, llon, rlat, rlon
+        Output: A csv file `data/river_coords.csv` with the headers `llat, llon, rlat, rlon`
         
         ## Centerline and Width
         ### River Object
         First, generate a river object to contain river data and available transformations
         ```
         centerline_width.riverCenterline(csv_data=None,
         				optional_cutoff=None,
@@ -162,15 +167,17 @@
         * [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
         * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
         
         Interpolating is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps dues to the combination of sparse data and a narrow river
         
         Object (class) useful attributes:
         
-        * centerlineLatitudeLongtiude (list of tuples): List of the latitude and longitude coordinates of the centerline
+        * centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
+        * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
+        * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
         * centerlineLength (float): Length of the centerline of the river (in km)
         * rightBankLength (float): Length of the right bank of the river (in km)
         * leftBankLength (float): Length of the left bank of the river (in km)
         
         Object (class) additional atttributes:
         
         * river_name (string): name of object, set to the csv_data string
@@ -182,50 +189,90 @@
         * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
         * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
         * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
         * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
         * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
         * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
         * interpolate_data (bool): if interpolating between existing data, defaults to False
-        * interpolate_n (int): specifies how many additional points will be added when interpolating data, defaults to 5
+        * interpolate_n (int): specifies how many additional points will be added between points along the river bank when interpolating data, defaults to 5
+        * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the the length of the dataframe (df_len)
+        
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         ```
         
         ### Return Latitude/Longitude Coordinates of Centerline
         Return the latitude/longitude coordinates of the centerline based on the left and right banks
+        
+        **Types of Centerlines**
+        There are three types of centerline coordinates formed from the river bank data. Each are built off of eachother and are used to clean and smooth data
+        - **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
+        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/voronoi_centerline.png)
+        - **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
+        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/evenly_spaced_centerline.png)
+        - **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
+        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/smoothed_centerline.png)
+        
+        Centerline coordinates are formed by the Voronoi vertices
+        ```
+        river_object.centerlineVoronoi
+        ```
+        
+        Centerline coordinates are formed by Evenly Spaced Voronoi vertices
+        ```
+        river_object.centerlineEvenlySpaced
+        ```
+        
+        Centerline coordinates are formed from Smoothed Voronoi vertices
         ```
-        river_object.centerlineLatitudeLongtiude
+        river_object.centerlineSmoothed
         ```
-        Centerline coordinates are formed from Voronoi vertices
         
+        Example:
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=15)
-        river_centerline_coordinates = river_object.centerlineLatitudeLongtiude
+        river_centerline_coordinates = river_object.centerlineVoronoi
         ```
         Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
         
+        ### Save Centerline Coordinates to a CSV
+        Save the centerline coordinates to a csv file with columns for latitude and longitude
+        
+        ```
+        saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
+        ```
+        * **[REQUIRED]** save_to_csv (str): CSV filename, requires a .csv extension
+        * [OPTIONAL] centerline_type (str): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed"], defaults to "Voronoi"
+        
+        ```python
+        import centerline_width
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+        river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
+        ```
+        
+        Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
+        
         ### Return Length of Centerline
-        Return the length of the centerline found between the left and right bank
+        Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
         ```
         river_object.centerlineLength
         ```
         Length returned in kilometers
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=550)
         river_centerline_length = river_object.centerlineLength
         ```
         The length of the river centerline returns `215.34700589636674` km
         
         ## Plot Centerline in Matplotlib
-        ### Plot the centerline created from a list of right and left banks with Voronoi vertices
+        Plot the centerline created from a list of right and left banks with Voronoi vertices
         
         ```
         plotCenterline(display_all_possible_paths=False, 
         		plot_title=None, 
         		save_plot_name=None, 
         		display_voronoi=False)
         ```
@@ -236,35 +283,33 @@
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.plotCenterline(display_all_possible_paths=False, display_voronoi=False)
         ```
         Output:
-        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_centerline.png)
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_centerline.png)
         
         ## Plot Centerline Width Lines in Matplotlib
         ### Plot the Centerline Width Lines
         Plot the width of the river based on the centerline
         
         Display Centerline at even intervals from the Voronoi generated centerline
         ```
         plotCenterlineWidth(plot_title=None, 
         		save_plot_name=None, 
         		display_true_centerline=True,
-        		n_interprolate_centerpoints=None,
         		transect_span_distance=3,
         		apply_smoothing=False,
         		flag_intersections=True,
         		remove_intersections=False)
         ```
         * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
         * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
         * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
-        * [OPTIONAL] n_interprolate_centerpoints (int): Recreate centerline coordinates with n evenly spaced points, defaults to the number of rows in the csv file
         * [OPTIONAL] transect_span_distance (int): Sum up n amount of points around a centerpoint to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
         * [OPTIONAL] flag_intersections (bool): Display intersecting width lines as red in graph, defaults to True
         * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to False
         
         **apply_smoothing**
         
@@ -292,42 +337,36 @@
         | remove_intersections=False | remove_intersections=True |
         | ------------- | ------------- |
         | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
-        river_object.plotCenterlineWidth(save_plot_name="data/river_coords_width.png",
-        				display_true_centerline=False,
-        				n_interprolate_centerpoints=None,
-        				transect_span_distance=3,
-        				apply_smoothing=True,
-        				flag_intersections=True,
-        				remove_intersections=True)
+        river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
         ```
-        ![river_coords_width+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_width.png)
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/river_coords_width.png)
         
         ### Return Width of River
         
-        Return the width of the river at each (evenly spaced) centerline coordinate
+        Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width`
         
         ```
-        riverWidthFromCenterline(n_interprolate_centerpoints=None,
-        			transect_span_distance=3,
+        riverWidthFromCenterline(transect_span_distance=3,
         			apply_smoothing=True,
         			remove_intersections=False,
         			units="km",
         			save_to_csv=None)
         ```
-        * [OPTIONAL] n_interprolate_centerpoints (int): Recreate centerline coordinates with n evenly spaced points, defaults to the number of rows in the csv file
         * [OPTIONAL] transect_span_distance (int): Sum up n amount of points around a centerpoint to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
         * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaultsl to True
         * [OPTIONAL] units (string): Units to measure distance, options: ["km" (kilometers), "m" (meters), "mi" (miles), "nmi" (nautical miles), "ft" (feet), "in" (inches), "rad" (radians), "deg" (degrees)], defaults to "km" (kilometers)
-        * [OPTIONAL] save_to_csv (string): Save river width output to a csv file, defaults to None (no file is saved)
+        * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
+        
+        Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordiantes may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
         							apply_smoothing=True,
         							units="km",
@@ -370,19 +409,14 @@
         
         **All vertices:**
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example4.png)
         
         **Vertices that have at least two connections (that would create gaps):**
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example5.png)
         
-        ### Types of Centerlines
-        - Voronoi centerline: centerline generated from where Voronoi vertices intersect within the river
-        - Evenly Spaced Centerline: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
-        - Smoothed Centerline: centerline generated from the evenly spaced centerline but smoothed by a b-spline
-        
         ## Debugging, Error Handling, and Edge Cases
         ### Wide Start/End of River
         If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example3.png)
         Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red) that sits along the longest path
         
         ### Invalid Polygon
@@ -422,15 +456,14 @@
         | interpolate_data = False | interpolate_data = True |
         | ------------- | ------------- |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
         
         The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
         
         ## Developer Notes: Tech Debt and Bug Fixes
-        * conversion of centerline lat-lon to meters
         * Fix legend overlapping on graph, replace doc_examples that have an overlapping
         * Verify that smoothing filter option does not produce a line that goes outside of the polygon
         
         ## Citations
         Based on work written in R (Golly et al. 2017):
         
         >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
```

### Comparing `centerline-width-0.2.2/centerline_width.egg-info/SOURCES.txt` & `centerline-width-0.2.3/centerline_width.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.2/setup.py` & `centerline-width-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="0.2.2"
+VERSION="0.2.3"
 DESCRIPTION="A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="centerline-width",
```

