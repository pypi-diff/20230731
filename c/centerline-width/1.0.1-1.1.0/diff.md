# Comparing `tmp/centerline-width-1.0.1.tar.gz` & `tmp/centerline-width-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/centerline-width-1.0.1.tar", last modified: Fri Jul 21 21:24:06 2023, max compression
+gzip compressed data, was "dist/centerline-width-1.1.0.tar", last modified: Mon Jul 31 06:52:33 2023, max compression
```

## Comparing `centerline-width-1.0.1.tar` & `centerline-width-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-21 21:24:06.287201 centerline-width-1.0.1/
--rw-rw-r--   0 user      (1000) user      (1000)    46218 2023-07-21 21:24:06.287201 centerline-width-1.0.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    40212 2023-07-13 19:32:57.000000 centerline-width-1.0.1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-21 21:24:06.279201 centerline-width-1.0.1/centerline_width/
--rw-rw-r--   0 user      (1000) user      (1000)     1632 2023-06-23 06:05:21.000000 centerline-width-1.0.1/centerline_width/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    26135 2023-06-26 21:50:27.000000 centerline-width-1.0.1/centerline_width/centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)    16829 2023-06-26 21:48:17.000000 centerline-width-1.0.1/centerline_width/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-1.0.1/centerline_width/getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)     9312 2023-07-12 06:10:05.000000 centerline-width-1.0.1/centerline_width/plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-1.0.1/centerline_width/preprocessing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-21 21:24:06.287201 centerline-width-1.0.1/centerline_width/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)    13693 2023-06-26 21:49:08.000000 centerline-width-1.0.1/centerline_width/pytests/test_centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-1.0.1/centerline_width/pytests/test_getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)    12990 2023-06-24 07:23:37.000000 centerline-width-1.0.1/centerline_width/pytests/test_plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-1.0.1/centerline_width/pytests/test_preprocessing.py
--rw-rw-r--   0 user      (1000) user      (1000)     5105 2023-06-24 07:13:29.000000 centerline-width-1.0.1/centerline_width/pytests/test_riverCenterlineClass.py
--rw-rw-r--   0 user      (1000) user      (1000)     6510 2023-06-26 21:49:56.000000 centerline-width-1.0.1/centerline_width/riverCenterlineClass.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-21 21:24:06.279201 centerline-width-1.0.1/centerline_width.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    46218 2023-07-21 21:24:06.000000 centerline-width-1.0.1/centerline_width.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      700 2023-07-21 21:24:06.000000 centerline-width-1.0.1/centerline_width.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-21 21:24:06.000000 centerline-width-1.0.1/centerline_width.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      160 2023-07-21 21:24:06.000000 centerline-width-1.0.1/centerline_width.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-07-21 21:24:06.000000 centerline-width-1.0.1/centerline_width.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-21 21:24:06.287201 centerline-width-1.0.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1846 2023-07-21 21:22:06.000000 centerline-width-1.0.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 06:52:33.573910 centerline-width-1.1.0/
+-rw-rw-r--   0 user      (1000) user      (1000)    53316 2023-07-31 06:52:33.573910 centerline-width-1.1.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    46958 2023-07-31 06:34:46.000000 centerline-width-1.1.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 06:52:33.569910 centerline-width-1.1.0/centerline_width/
+-rw-rw-r--   0 user      (1000) user      (1000)     1949 2023-07-28 21:06:35.000000 centerline-width-1.1.0/centerline_width/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    28929 2023-07-28 21:33:59.000000 centerline-width-1.1.0/centerline_width/centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19456 2023-07-28 21:35:26.000000 centerline-width-1.1.0/centerline_width/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-1.1.0/centerline_width/getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13110 2023-07-28 21:27:12.000000 centerline-width-1.1.0/centerline_width/plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-1.1.0/centerline_width/preprocessing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 06:52:33.573910 centerline-width-1.1.0/centerline_width/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)    17125 2023-07-29 22:22:33.000000 centerline-width-1.1.0/centerline_width/pytests/test_centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-1.1.0/centerline_width/pytests/test_getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15156 2023-07-29 22:17:03.000000 centerline-width-1.1.0/centerline_width/pytests/test_plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-1.1.0/centerline_width/pytests/test_preprocessing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5105 2023-06-24 07:13:29.000000 centerline-width-1.1.0/centerline_width/pytests/test_riverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3486 2023-07-28 21:11:22.000000 centerline-width-1.1.0/centerline_width/relativeDistance.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9334 2023-07-28 21:36:14.000000 centerline-width-1.1.0/centerline_width/riverCenterlineClass.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 06:52:33.569910 centerline-width-1.1.0/centerline_width.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    53316 2023-07-31 06:52:33.000000 centerline-width-1.1.0/centerline_width.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      737 2023-07-31 06:52:33.000000 centerline-width-1.1.0/centerline_width.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-31 06:52:33.000000 centerline-width-1.1.0/centerline_width.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      160 2023-07-31 06:52:33.000000 centerline-width-1.1.0/centerline_width.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-07-31 06:52:33.000000 centerline-width-1.1.0/centerline_width.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-31 06:52:33.573910 centerline-width-1.1.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1846 2023-07-31 06:41:29.000000 centerline-width-1.1.0/setup.py
```

### Comparing `centerline-width-1.0.1/PKG-INFO` & `centerline-width-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.0.1.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.1.0.tar.gz
 Description: # Centerline-Width
          <p align="center">
           <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
@@ -225,125 +225,155 @@
         * centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
         * centerlineEqualDistance (list of tuples): List of the latitude and longitude coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
         * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
         * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
         * centerlineLength (float): Length of the centerline of the river (in km)
         * rightBankLength (float): Length of the right bank of the river (in km)
         * leftBankLength (float): Length of the left bank of the river (in km)
+        * centerlineVoronoiRelative (list of tuples): List of the relative distance coordinates of the centerline generated by Voronoi diagrams
+        * centerlineEqualDistanceRelative (list of tuples): List of the relative distance coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
+        * centerlineEvenlySpacedRelative (list of tuples): List of the relative distance coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
+        * centerlineSmoothedRelative (list of tuples): List of the relative distance coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
         
         **Object (class) additional attributes:**
         
         * river_name (string): name of object, set to the csv_data string
-        * left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
-        * right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
+        * left_bank_coordinates (list of tuples): list of latitude/longtiude coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
+        * right_bank_coordinates (list of tuples) list of latitude/longitude coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
+        * left_bank_relative_coordinates (list of tuples): list of relative distances coordaintes of the left bank, measured as the distance in meters from the first point on the left bank (`[(x, y), (x, y)]`)
+        * right_bank_relative_coordinates (list of tuples): list of relative distances coordaintes of the right bank, measured as the distance in meters from the first point on the left bank (`[(x, y), (x, y)]`)
         * df_len (int): Length of the data frame of the csv data (spliced by the optional_cutoff)
         * equal_distance (int): Distance between points (in meters) used in centerlineEqualDistance, defaults to points every 10 meters
         * ellipsoid (string): Built-in ellipsoid definition of Earth to determine how degrees are converted to meters used by centerlineEqualDistance, defaults to "WGS84"
-        * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate riverbank (used to define an inside and an outside of the river)
-        * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
-        * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
+        * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate the latitude/longtiude coordinate riverbank (used to define an inside and an outside of the river)
+        * bank_polygon_relative (Shapley Polygon): Multi-sided polygon generated to encapsulate the relative distance coordinate riverbank (used to define an inside and an outside of the river)
+        * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon for the latitude/longitude coordinate system
+        * top_bank_relative (Shapley Linestring): Linestring that represents the top of the river/polygon for the relative distance coordinate system
+        * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon for the latitude/longitude coordinate system
+        * bottom_bank_relative (Shapley Linestring): Linestring that represents the bottom of the river/polygon for the relative distance coordinate system
         * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
+        * starting_node_relative (tuple): Tuple of the starting position (relative distance x and relative distance y) of the centerline path
         * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
-        * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
+        * ending_node_relative (tuple): Tuple of the end position (relative distance x and relative distance y) of the centerline path
+        * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks of the latitude/longitude coordinate system
+        * bank_voronoi_relative (scipy Voronoi object): Voronoi generated by left/right banks of the relative distance coordinate system
         * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
         * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
+        * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Relative Distance X position to ending Relative Distance X position)
+        * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Relative Distance Y position to ending Relative Distance Y position)
         * interpolate_data (boolean): if interpolating between existing data, defaults to False
         * interpolate_n (int): specifies how many additional points will be added between points along the riverbank when interpolating data, defaults to 5
         * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the length of the data frame (df_len)
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         ```
         
-        ### Return Latitude/Longitude Coordinates of Centerline
-        Return the latitude/longitude coordinates in units of decimal-degrees of the centerline based on the left and right banks
+        ### Coordinates of Centerline
+        Return the coordinates of the centerline based on the left and right banks with either `Decimal Degree` (latitude/longtiude) or `Relative Distance` (meters)
         
         **Types of Centerlines**
         
         There are four types of centerline coordinates formed from the riverbank data
         
         - **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline.png)
         - **Equal Distance Centerline**: centerline based on Voronoi centerline but each point is equally spaced out from the previous (in meters) and takes into account the radius of the Earth to convert degrees to meters (example below: `equal_distance=10`)
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_centerline.png)
         - **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points (example: `interpolate_n_centerpoints=200`)
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline.png)
         - **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline.png)
         
+        By default, coordinates are formed in `Decimal Degrees`, but can be set to `Relative Distance`. Relative Distance measures the distance (in meters) of a point from the first point on the left bank
+        
         Centerline coordinates are formed by the Voronoi vertices
         ```
         river_object.centerlineVoronoi
         ```
+        | river_object.centerlineVoronoi | river_object.centerlineVoronoiRelative |
+        | ------------- | ------------- |
+        | ![centerlineVoronoi+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline.png) | ![centerlineVoronoiRelative+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline_relative.png) |
         
         Centerline coordinates are formed by Equally Distanced vertices, set by `equal_distance`
         ```
         river_object.centerlineEqualDistance
         ```
+        | river_object.centerlineEqualDistance | river_object.centerlineEqualDistanceRelative |
+        | ------------- | ------------- |
+        | ![centerlineEqualDistance+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_centerline.png) | ![centerlineEqualDistanceRelative+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_centerline_relative.png) |
         
         Centerline coordinates are formed by Evenly Spaced vertices, set by `interpolate_n_centerpoints`
         ```
         river_object.centerlineEvenlySpaced
         ```
+        | river_object.centerlineEvenlySpaced | river_object.centerlineEvenlySpacedRelative |
+        | ------------- | ------------- |
+        | ![centerlineEvenlySpaced+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline.png) | ![centerlineEvenlySpacedRelative+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline_relative.png) |
         
         Centerline coordinates are formed from Smoothed vertices
         ```
         river_object.centerlineSmoothed
         ```
+        | river_object.centerlineSmoothed | river_object.centerlineSmoothedRelative |
+        | ------------- | ------------- |
+        | ![centerlineEvenlySpaced+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline.png) | ![centerlineEvenlySpacedRelative+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline_relative.png) |
         
         Example:
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_centerline_coordinates = river_object.centerlineVoronoi
         ```
         Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
         
         ### Save Centerline Coordinates to a .CSV File
         Save the centerline coordinates to a csv file with columns for latitude and longitude. This is the file format for a table of (latitude,longitude) pairs accepted to import back into Google Earth Pro.
         
         ```
-        saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
+        saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi", coordinate_type="Decimal Degrees")
         ```
         * **[REQUIRED]** save_to_csv (string): CSV filename, requires a .csv extension
         * [OPTIONAL] centerline_type (string): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
-        * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)`
-        * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)`
+        * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)` or `<centerline_type> Relative Distance Y (from Latitude) (m)`
+        * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)` or `<centerline_type> Relative Distance X (from Longitude) (m)`
+        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
         ```
         Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
         
         Note: it is best practice to plot the centerline with `plotCenterline()` to ensure that the results saved are as expected
         
         ### Save Centerline Coordinates to a .MAT File
         Save the centerline coordinates to a .mat file with columns for latitude and longitude
         
         ```
-        saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi")
+        saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi", coordinate_type="Decimal Degrees")
         ```
         * **[REQUIRED]** save_to_mat (string): MAT filename, requires a .mat extension
         * [OPTIONAL] centerline_type (string): Centerline type to save to MAT (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
-        * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` (cannot include spaces or special characters)
-        * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` (cannot include spaces or special characters)
+        * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` or `<centerline_type>_Relative_Distance_Y_From_Latitude_m` (cannot include spaces or special characters)
+        * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` or `<centerline_type>_Relative_Distance_X_From_Longitude_m` (cannot include spaces or special characters)
+        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineMAT(save_to_mat="centerline_coordinates.mat", centerline_type="Smoothed")
         ```
         Returns a .mat file with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed_Centerline_Latitude_(Deg), Smoothed_Centerline_Longitude_(Deg)`
         
         Note: it is best practice to plot the centerline with `plotCenterline()` to ensure that the results saved are as expected
         
-        ### Return Length of Centerline
+        ### Length of Centerline
         Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
         ```
         river_object.centerlineLength
         ```
         Length returned in kilometers
         ```python
         import centerline_width
@@ -358,23 +388,25 @@
         ```
         plotCenterline(centerline_type="Voronoi",
         		marker_type="line",
         		centerline_color="black",
         		display_all_possible_paths=False, 
         		plot_title=None, 
         		save_plot_name=None, 
-        		display_voronoi=False)
+        		display_voronoi=False,
+        		coordinate_type="Decimal Degrees")
         ```
         * [OPTIONAL] centerline_type (string): Centerline type graph within river (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
         * [OPTIONAL] marker_type (string): Graph type (not case-sensitive), options: ["Line", "Scatter"], defaults to "Line"
         * [OPTIONAL] centerline_color (string): Color of centerline coordinates on graph (not case-sensitive), options: [matplotlib named colors](https://matplotlib.org/stable/gallery/color/named_colors.html), defaults to "black"
         * [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging), defaults to False
         * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
         * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
         * [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline, defaults to False
+        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.plotCenterline()
         ```
         Output:
@@ -388,23 +420,25 @@
         ```
         plotCenterlineWidth(plot_title=None, 
         		save_plot_name=None, 
         		display_true_centerline=True,
         		transect_span_distance=3,
         		apply_smoothing=False,
         		flag_intersections=True,
-        		remove_intersections=False)
+        		remove_intersections=False,
+        		coordinate_type="Decimal Degrees")
         ```
         * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
         * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
         * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
         * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
         * [OPTIONAL] flag_intersections (boolean): Display intersecting width lines as red in graph, defaults to True
         * [OPTIONAL] remove_intersections (boolean): Remove intersecting lines (but maintain the most width lines as possible) and only return non-intersecting width lines, defaults to False
+        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         
         **apply_smoothing**
         
         apply_smoothing applies a spline to smooth the centerline points created by the Voronoi vertices. This reduces the noise of the slopes and can create width lines that are less susceptible to small changes in the bank
         
         | apply_smoothing=False | apply_smoothing=True |
         | ------------- | ------------- |
@@ -425,14 +459,22 @@
         
         Intersecting lines are flagged in red by default (flag_intersections=True)
         
         | remove_intersections=False | remove_intersections=True |
         | ------------- | ------------- |
         | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
         
+        **coordinate_type**
+        
+        Two options for measuring and displaying coordinates. The two options are "Decimal Degrees" and "Relative Distance". "Decimal Degrees" is the default option that uses the original data coordinate system with latitude/longitude. "Relative Distance" changes the coordinates of each point to be the distance (in meters) from the first point on the left bank
+        
+        | coordinate_type="Decimal Degrees" | remove_intersections="Relative Distance" |
+        | ------------- | ------------- |
+        | ![dd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_decimal_degrees.png) | ![rd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_relative_distance.png)|
+        
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
         ```
         ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
         
@@ -440,19 +482,21 @@
         
         Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width` in meters
         
         ```
         riverWidthFromCenterline(transect_span_distance=3,
         			apply_smoothing=True,
         			remove_intersections=False,
+        			coordinate_type="Decimal Degrees",
         			save_to_csv=None)
         ```
         * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
         * [OPTIONAL] remove_intersections (boolean): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
+        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (km)`)
         
         Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
```

### Comparing `centerline-width-1.0.1/README.md` & `centerline-width-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -217,125 +217,155 @@
 * centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
 * centerlineEqualDistance (list of tuples): List of the latitude and longitude coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
 * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
 * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
 * centerlineLength (float): Length of the centerline of the river (in km)
 * rightBankLength (float): Length of the right bank of the river (in km)
 * leftBankLength (float): Length of the left bank of the river (in km)
+* centerlineVoronoiRelative (list of tuples): List of the relative distance coordinates of the centerline generated by Voronoi diagrams
+* centerlineEqualDistanceRelative (list of tuples): List of the relative distance coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
+* centerlineEvenlySpacedRelative (list of tuples): List of the relative distance coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
+* centerlineSmoothedRelative (list of tuples): List of the relative distance coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
 
 **Object (class) additional attributes:**
 
 * river_name (string): name of object, set to the csv_data string
-* left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
-* right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
+* left_bank_coordinates (list of tuples): list of latitude/longtiude coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
+* right_bank_coordinates (list of tuples) list of latitude/longitude coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
+* left_bank_relative_coordinates (list of tuples): list of relative distances coordaintes of the left bank, measured as the distance in meters from the first point on the left bank (`[(x, y), (x, y)]`)
+* right_bank_relative_coordinates (list of tuples): list of relative distances coordaintes of the right bank, measured as the distance in meters from the first point on the left bank (`[(x, y), (x, y)]`)
 * df_len (int): Length of the data frame of the csv data (spliced by the optional_cutoff)
 * equal_distance (int): Distance between points (in meters) used in centerlineEqualDistance, defaults to points every 10 meters
 * ellipsoid (string): Built-in ellipsoid definition of Earth to determine how degrees are converted to meters used by centerlineEqualDistance, defaults to "WGS84"
-* bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate riverbank (used to define an inside and an outside of the river)
-* top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
-* bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
+* bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate the latitude/longtiude coordinate riverbank (used to define an inside and an outside of the river)
+* bank_polygon_relative (Shapley Polygon): Multi-sided polygon generated to encapsulate the relative distance coordinate riverbank (used to define an inside and an outside of the river)
+* top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon for the latitude/longitude coordinate system
+* top_bank_relative (Shapley Linestring): Linestring that represents the top of the river/polygon for the relative distance coordinate system
+* bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon for the latitude/longitude coordinate system
+* bottom_bank_relative (Shapley Linestring): Linestring that represents the bottom of the river/polygon for the relative distance coordinate system
 * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
+* starting_node_relative (tuple): Tuple of the starting position (relative distance x and relative distance y) of the centerline path
 * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
-* bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
+* ending_node_relative (tuple): Tuple of the end position (relative distance x and relative distance y) of the centerline path
+* bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks of the latitude/longitude coordinate system
+* bank_voronoi_relative (scipy Voronoi object): Voronoi generated by left/right banks of the relative distance coordinate system
 * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
 * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
+* x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Relative Distance X position to ending Relative Distance X position)
+* y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Relative Distance Y position to ending Relative Distance Y position)
 * interpolate_data (boolean): if interpolating between existing data, defaults to False
 * interpolate_n (int): specifies how many additional points will be added between points along the riverbank when interpolating data, defaults to 5
 * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the length of the data frame (df_len)
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 ```
 
-### Return Latitude/Longitude Coordinates of Centerline
-Return the latitude/longitude coordinates in units of decimal-degrees of the centerline based on the left and right banks
+### Coordinates of Centerline
+Return the coordinates of the centerline based on the left and right banks with either `Decimal Degree` (latitude/longtiude) or `Relative Distance` (meters)
 
 **Types of Centerlines**
 
 There are four types of centerline coordinates formed from the riverbank data
 
 - **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline.png)
 - **Equal Distance Centerline**: centerline based on Voronoi centerline but each point is equally spaced out from the previous (in meters) and takes into account the radius of the Earth to convert degrees to meters (example below: `equal_distance=10`)
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_centerline.png)
 - **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points (example: `interpolate_n_centerpoints=200`)
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline.png)
 - **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline.png)
 
+By default, coordinates are formed in `Decimal Degrees`, but can be set to `Relative Distance`. Relative Distance measures the distance (in meters) of a point from the first point on the left bank
+
 Centerline coordinates are formed by the Voronoi vertices
 ```
 river_object.centerlineVoronoi
 ```
+| river_object.centerlineVoronoi | river_object.centerlineVoronoiRelative |
+| ------------- | ------------- |
+| ![centerlineVoronoi+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline.png) | ![centerlineVoronoiRelative+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline_relative.png) |
 
 Centerline coordinates are formed by Equally Distanced vertices, set by `equal_distance`
 ```
 river_object.centerlineEqualDistance
 ```
+| river_object.centerlineEqualDistance | river_object.centerlineEqualDistanceRelative |
+| ------------- | ------------- |
+| ![centerlineEqualDistance+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_centerline.png) | ![centerlineEqualDistanceRelative+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_centerline_relative.png) |
 
 Centerline coordinates are formed by Evenly Spaced vertices, set by `interpolate_n_centerpoints`
 ```
 river_object.centerlineEvenlySpaced
 ```
+| river_object.centerlineEvenlySpaced | river_object.centerlineEvenlySpacedRelative |
+| ------------- | ------------- |
+| ![centerlineEvenlySpaced+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline.png) | ![centerlineEvenlySpacedRelative+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline_relative.png) |
 
 Centerline coordinates are formed from Smoothed vertices
 ```
 river_object.centerlineSmoothed
 ```
+| river_object.centerlineSmoothed | river_object.centerlineSmoothedRelative |
+| ------------- | ------------- |
+| ![centerlineEvenlySpaced+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline.png) | ![centerlineEvenlySpacedRelative+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline_relative.png) |
 
 Example:
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_centerline_coordinates = river_object.centerlineVoronoi
 ```
 Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
 
 ### Save Centerline Coordinates to a .CSV File
 Save the centerline coordinates to a csv file with columns for latitude and longitude. This is the file format for a table of (latitude,longitude) pairs accepted to import back into Google Earth Pro.
 
 ```
-saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
+saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi", coordinate_type="Decimal Degrees")
 ```
 * **[REQUIRED]** save_to_csv (string): CSV filename, requires a .csv extension
 * [OPTIONAL] centerline_type (string): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
-* [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)`
-* [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)`
+* [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)` or `<centerline_type> Relative Distance Y (from Latitude) (m)`
+* [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)` or `<centerline_type> Relative Distance X (from Longitude) (m)`
+* [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
 ```
 Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
 
 Note: it is best practice to plot the centerline with `plotCenterline()` to ensure that the results saved are as expected
 
 ### Save Centerline Coordinates to a .MAT File
 Save the centerline coordinates to a .mat file with columns for latitude and longitude
 
 ```
-saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi")
+saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi", coordinate_type="Decimal Degrees")
 ```
 * **[REQUIRED]** save_to_mat (string): MAT filename, requires a .mat extension
 * [OPTIONAL] centerline_type (string): Centerline type to save to MAT (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
-* [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` (cannot include spaces or special characters)
-* [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` (cannot include spaces or special characters)
+* [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` or `<centerline_type>_Relative_Distance_Y_From_Latitude_m` (cannot include spaces or special characters)
+* [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` or `<centerline_type>_Relative_Distance_X_From_Longitude_m` (cannot include spaces or special characters)
+* [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.saveCenterlineMAT(save_to_mat="centerline_coordinates.mat", centerline_type="Smoothed")
 ```
 Returns a .mat file with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed_Centerline_Latitude_(Deg), Smoothed_Centerline_Longitude_(Deg)`
 
 Note: it is best practice to plot the centerline with `plotCenterline()` to ensure that the results saved are as expected
 
-### Return Length of Centerline
+### Length of Centerline
 Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
 ```
 river_object.centerlineLength
 ```
 Length returned in kilometers
 ```python
 import centerline_width
@@ -350,23 +380,25 @@
 ```
 plotCenterline(centerline_type="Voronoi",
 		marker_type="line",
 		centerline_color="black",
 		display_all_possible_paths=False, 
 		plot_title=None, 
 		save_plot_name=None, 
-		display_voronoi=False)
+		display_voronoi=False,
+		coordinate_type="Decimal Degrees")
 ```
 * [OPTIONAL] centerline_type (string): Centerline type graph within river (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
 * [OPTIONAL] marker_type (string): Graph type (not case-sensitive), options: ["Line", "Scatter"], defaults to "Line"
 * [OPTIONAL] centerline_color (string): Color of centerline coordinates on graph (not case-sensitive), options: [matplotlib named colors](https://matplotlib.org/stable/gallery/color/named_colors.html), defaults to "black"
 * [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging), defaults to False
 * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
 * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
 * [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline, defaults to False
+* [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.plotCenterline()
 ```
 Output:
@@ -380,23 +412,25 @@
 ```
 plotCenterlineWidth(plot_title=None, 
 		save_plot_name=None, 
 		display_true_centerline=True,
 		transect_span_distance=3,
 		apply_smoothing=False,
 		flag_intersections=True,
-		remove_intersections=False)
+		remove_intersections=False,
+		coordinate_type="Decimal Degrees")
 ```
 * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
 * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
 * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
 * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
 * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
 * [OPTIONAL] flag_intersections (boolean): Display intersecting width lines as red in graph, defaults to True
 * [OPTIONAL] remove_intersections (boolean): Remove intersecting lines (but maintain the most width lines as possible) and only return non-intersecting width lines, defaults to False
+* [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
 
 **apply_smoothing**
 
 apply_smoothing applies a spline to smooth the centerline points created by the Voronoi vertices. This reduces the noise of the slopes and can create width lines that are less susceptible to small changes in the bank
 
 | apply_smoothing=False | apply_smoothing=True |
 | ------------- | ------------- |
@@ -417,14 +451,22 @@
 
 Intersecting lines are flagged in red by default (flag_intersections=True)
 
 | remove_intersections=False | remove_intersections=True |
 | ------------- | ------------- |
 | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
 
+**coordinate_type**
+
+Two options for measuring and displaying coordinates. The two options are "Decimal Degrees" and "Relative Distance". "Decimal Degrees" is the default option that uses the original data coordinate system with latitude/longitude. "Relative Distance" changes the coordinates of each point to be the distance (in meters) from the first point on the left bank
+
+| coordinate_type="Decimal Degrees" | remove_intersections="Relative Distance" |
+| ------------- | ------------- |
+| ![dd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_decimal_degrees.png) | ![rd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_relative_distance.png)|
+
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
 ```
 ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
 
@@ -432,19 +474,21 @@
 
 Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width` in meters
 
 ```
 riverWidthFromCenterline(transect_span_distance=3,
 			apply_smoothing=True,
 			remove_intersections=False,
+			coordinate_type="Decimal Degrees",
 			save_to_csv=None)
 ```
 * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
 * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
 * [OPTIONAL] remove_intersections (boolean): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
+* [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
 * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (km)`)
 
 Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
```

### Comparing `centerline-width-1.0.1/centerline_width/__init__.py` & `centerline-width-1.1.0/centerline_width/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 from .preprocessing import generateVoronoi
 from .preprocessing import pointsFromVoronoi
 from .preprocessing import interpolateBetweenPoints
 
 # riverObject.py function calls
 from .riverCenterlineClass import riverCenterline
 
+# relativeDistance.py function calls
+from .relativeDistance import relativeSingleCoordinate
+from .relativeDistance import relativeBankCoordinates
+from .relativeDistance import relativeCenterlineCoordinates
+from .relativeDistance import relativeRidgeCoordinates
+from .relativeDistance import relativeWidthCoordinates
+
 # centerline.py function calls
 from .centerline import centerlinePath
 from .centerline import networkXGraphShortestPath
 from .centerline import centerlineLength
 from .centerline import equalDistanceCenterline
 from .centerline import evenlySpacedCenterline
 from .centerline import smoothedCoordinates
```

### Comparing `centerline-width-1.0.1/centerline_width/centerline.py` & `centerline-width-1.1.0/centerline_width/centerline.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,14 +198,15 @@
 
 	return smoothed_coordinates
 
 def riverWidthFromCenterlineCoordinates(river_object=None,
 										centerline_coordinates=None,
 										transect_span_distance=3,
 										remove_intersections=False,
+										coordinate_type="Decimal Degrees",
 										save_to_csv=None):
 	# Return the left/right coordinates of width centerlines
 	right_width_coordinates = {}
 	left_width_coordinates = {}
 	num_intersection_coordinates = {}
 	x = []
 	y = []
@@ -228,24 +229,26 @@
 			normal_of_slope = -1 / slope_avg
 			middle_of_list = len(group_points) // 2 # set centerline point to be the middle point being averaged
 			centerline_slope[group_points[middle_of_list]] = normal_of_slope
 
 	def intersectsTopOrBottomOfBank(point1, point2):
 		# returns True/False if the points lie on the 'false' top/bottom of the river
 		points_intersect_false_edges = False
+
 		# avoiding floating point precession errors when determining if point lies within the line
 		# if point is within a small distance of a line it is considered to intersect
 		if river_object.top_bank.distance(point1) < 1e-8 or river_object.bottom_bank.distance(point1) < 1e-8:
 			points_intersect_false_edges = True
 		if river_object.top_bank.distance(point2) < 1e-8 or river_object.bottom_bank.distance(point2) < 1e-8:
 			points_intersect_false_edges = True
 		return points_intersect_false_edges
 
 	# Generate a list of lines from the centerline point with its normal
 	logger.info("[PROCESSING] Calculating and positioning width lines, may takes a few minutes...")
+
 	min_x, min_y, max_x, max_y = river_object.bank_polygon.bounds
 	for centerline_point, slope in centerline_slope.items():
 		# draw a max line that extends the entire distance of the available space, will be trimmed below to just within polygon
 		left_y = slope * (min_x - centerline_point[0]) + centerline_point[1]
 		right_y = slope * (max_x - centerline_point[0]) + centerline_point[1]
 
 		# Save the points where they intersect the polygon
@@ -343,25 +346,29 @@
 
 	return right_width_coordinates, left_width_coordinates, num_intersection_coordinates
 
 def riverWidthFromCenterline(river_object=None,
 							transect_span_distance=3,
 							apply_smoothing=True,
 							remove_intersections=False,
+							coordinate_type="Decimal Degrees",
 							save_to_csv=None):
 	# Return river width: centerline and width at centerline
 	# Width is measured to the bank, relative to the center point (normal of the centerline)
 	# { [centerline latitude, centerline longitude] : widthValue }
 
 	centerline_width.errorHandlingRiverWidthFromCenterline(river_object=river_object,
 															transect_span_distance=transect_span_distance,
 															apply_smoothing=apply_smoothing,
 															remove_intersections=remove_intersections,
+															coordinate_type=coordinate_type,
 															save_to_csv=save_to_csv)
 
+	coordinate_type = coordinate_type.title()
+
 	if river_object.centerlineVoronoi is None:
 		logger.critical("\nCRITICAL ERROR, unable to find width without a valid centerline")
 		return None
 
 	# recreate the centerline with evenly spaced points
 	defined_centerline_coordinates = centerline_width.evenlySpacedCenterline(centerline_coordinates=river_object.centerlineVoronoi,
 																			number_of_fixed_points=river_object.interpolate_n_centerpoints)
@@ -382,19 +389,29 @@
 	for centerline_coord, _ in right_width_coord.items():
 		# store the distance between the lat/lon position of the right/left bank
 		lon1, lat1 = right_width_coord[centerline_coord]
 		lon2, lat2 = left_width_coord[centerline_coord]
 		_, _, distance_between_right_and_left_m = geodesic.inv(lon1, lat1, lon2, lat2)
 		width_dict[centerline_coord] = distance_between_right_and_left_m/1000
 
+	# Set headers and conver to Relative Distance if needed
+	if coordinate_type == "Decimal Degrees":
+		latitude_header= "Centerline Latitude (Deg)"
+		longitude_header = "Centerline Longitude (Deg)"
+	if coordinate_type == "Relative Distance":
+		latitude_header= "Relative Distance Y (from Latitude) (m)"
+		longitude_header = "Relative Distance X (from Longitude) (m)"
+		# Convert from Decimal Degrees to Relative Distance
+		width_dict = centerline_width.relativeWidthCoordinates(river_object.left_bank_coordinates[0], width_dict, river_object.ellipsoid)
+
 	# Save width dictionary to a csv file (Latitude, Longtiude, Width)
 	if save_to_csv:
 		with open(save_to_csv, "w") as csv_file_output:
 			writer = csv.writer(csv_file_output)
-			writer.writerow(["Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (km)"])
+			writer.writerow([latitude_header,longitude_header, "Width (km)"])
 			for coordinate_key, width_value in width_dict.items():
 				writer.writerow([coordinate_key[1], coordinate_key[0], width_value])
 
 	return width_dict
 
 def centerlineLength(centerline_coordinates=None, ellipsoid="WGS84"):
 	# Return the length/distance for all the centerline coordinates in km
@@ -411,61 +428,99 @@
 		else:
 			lon1, lon2 = previous_pair[0], xy_pair[0]
 			lat1, lat2 = previous_pair[1], xy_pair[1]
 			_, _, distance_between_meters = geodesic.inv(lon1, lat1, lon2, lat2)
 			total_length += distance_between_meters
 	return total_length/1000
 
-def saveCenterlineCSV(river_object=None, save_to_csv=None, latitude_header=None, longitude_header=None, centerline_type="Voronoi"):
+def saveCenterlineCSV(river_object=None,
+					save_to_csv=None,
+					latitude_header=None,
+					longitude_header=None,
+					centerline_type="Voronoi",
+					coordinate_type="Decimal Degrees"):
 	# Save Centerline Coordinates generated by Voronoi Diagram to .CSV
 	centerline_width.errorHandlingSaveCenterlineCSV(river_object=river_object,
 													save_to_csv=save_to_csv, 
 													latitude_header=latitude_header,
 													longitude_header=longitude_header,
-													centerline_type=centerline_type)
+													centerline_type=centerline_type,
+													coordinate_type=coordinate_type)
 	centerline_type = centerline_type.title()
+	coordinate_type = coordinate_type.title()
 
-	if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoi
-	if centerline_type == "Equal Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistance
-	if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
-	if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothed
-
-	if latitude_header is None:
-		latitude_header = "{0} Centerline Latitude (Deg)".format(centerline_type)
-	if longitude_header is None:
-		longitude_header = "{0} Centerline Longitude (Deg)".format(centerline_type)
+	if coordinate_type == "Decimal Degrees":
+		if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoi
+		if centerline_type == "Equal Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistance
+		if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
+		if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothed
+	if coordinate_type == "Relative Distance":
+		if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoiRelative
+		if centerline_type == "Equal Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistanceRelative
+		if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpacedRelative
+		if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothedRelative
+
+	if coordinate_type == "Decimal Degrees":
+		if latitude_header is None:
+			latitude_header = "{0} Centerline Latitude (Deg)".format(centerline_type)
+		if longitude_header is None:
+			longitude_header = "{0} Centerline Longitude (Deg)".format(centerline_type)
+	if coordinate_type == "Relative Distance":
+		if latitude_header is None:
+			latitude_header = "{0} Relative Distance Y (from Latitude) (m)".format(centerline_type)
+		if longitude_header is None:
+			longitude_header = "{0} Relative Distance X (from Longitude) (m)".format(centerline_type)
 
 	with open(save_to_csv, "w") as csv_file_output:
 		writer = csv.writer(csv_file_output)
 		writer.writerow([latitude_header, longitude_header])
 		if centerline_coordinates_by_type is not None:
 			for latitude_longitude in centerline_coordinates_by_type:
 				writer.writerow([latitude_longitude[1], latitude_longitude[0]])
 		else:
 			logger.warn("\nWARNING, no {0} centerline coordinates found, {1} file generated will be empty".format(centerline_type, save_to_csv))
 
-def saveCenterlineMAT(river_object=None, save_to_mat=None, latitude_header=None, longitude_header=None, centerline_type="Voronoi"):
+def saveCenterlineMAT(river_object=None,
+					save_to_mat=None,
+					latitude_header=None,
+					longitude_header=None,
+					centerline_type="Voronoi",
+					coordinate_type="Decimal Degrees"):
 	# Save Centerline Coordinates generated by Voronoi Diagram to .MAT
 	centerline_width.errorHandlingSaveCenterlineMAT(river_object=river_object,
 													save_to_mat=save_to_mat, 
 													latitude_header=latitude_header,
 													longitude_header=longitude_header,
-													centerline_type=centerline_type)
+													centerline_type=centerline_type,
+													coordinate_type=coordinate_type)
 	centerline_type = centerline_type.title()
+	coordinate_type = coordinate_type.title()
 
-	if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoi
-	if centerline_type == "Equal Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistance
-	if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
-	if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothed
+	if coordinate_type == "Decimal Degrees":
+		if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoi
+		if centerline_type == "Equal Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistance
+		if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
+		if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothed
+	if coordinate_type == "Relative Distance":
+		if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoiRelative
+		if centerline_type == "Equal Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistanceRelative
+		if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpacedRelative
+		if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothedRelative
 
 	# .mat files do not allow for spaces or special characters in the header
-	if latitude_header is None:
-		latitude_header = "{0}_Centerline_Latitude_Deg".format(centerline_type.replace(" ", "_"))
-	if longitude_header is None:
-		longitude_header = "{0}_Centerline_Longitude_Deg".format(centerline_type.replace(" ", "_"))
+	if coordinate_type == "Decimal Degrees":
+		if latitude_header is None:
+			latitude_header = "{0}_Centerline_Latitude_Deg".format(centerline_type.replace(" ", "_"))
+		if longitude_header is None:
+			longitude_header = "{0}_Centerline_Longitude_Deg".format(centerline_type.replace(" ", "_"))
+	if coordinate_type == "Relative Distance":
+		if latitude_header is None:
+			latitude_header = "{0}_Relative_Distance_Y_From_Latitude_m".format(centerline_type.replace(" ", "_"))
+		if longitude_header is None:
+			longitude_header = "{0}_Relative_Distance_X_From_Longitude_m".format(centerline_type.replace(" ", "_"))		
 
 	latitude_lst = []
 	longtiude_lst = []
 
 	if centerline_coordinates_by_type is not None:
 		for latitude_longitude in centerline_coordinates_by_type:
 			longtiude_lst.append(latitude_longitude[0])
```

### Comparing `centerline-width-1.0.1/centerline_width/error_handling.py` & `centerline-width-1.1.0/centerline_width/error_handling.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 def errorHandlingPlotCenterline(river_object=None,
 								centerline_type=None,
 								marker_type=None,
 								centerline_color=None,
 								display_all_possible_paths=None,
 								plot_title=None,
 								save_plot_name=None,
-								display_voronoi=None):
+								display_voronoi=None,
+								coordinate_type=None):
 	# Error handling for plotCenterline()
 	if river_object is None:
 		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
 		exit()
 	else:
 		if not isinstance(river_object, centerline_width.riverCenterline):
 			logger.critical("\nCRITICAL ERROR, [river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{0}'".format(type(river_object)))
@@ -88,22 +89,32 @@
 		logger.critical("\nCRITICAL ERROR, [save_plot_name]: Must be a str, current type = '{0}'".format(type(save_plot_name)))
 		exit()
 
 	if type(display_voronoi) != bool:
 		logger.critical("\nCRITICAL ERROR, [display_voronoi]: Must be a bool, current type = '{0}'".format(type(display_voronoi)))
 		exit()
 
+	if type(coordinate_type) != str:
+		logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(type(coordinate_type)))
+		exit()
+	else:
+		coordinate_type_options = ["Decimal Degrees", "Relative Distance"]
+		if coordinate_type.title() not in coordinate_type_options:
+			logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be an available option in {0}, current option = '{1}'".format(coordinate_type_options, coordinate_type))
+			exit()
+
 def errorHandlingPlotCenterlineWidth(river_object=None,
 									plot_title=None,
 									save_plot_name=None,
 									display_true_centerline=None,
 									transect_span_distance=None,
 									apply_smoothing=None,
 									flag_intersections=None,
-									remove_intersections=None):
+									remove_intersections=None,
+									coordinate_type=None):
 	# Error handling for plotCenterlineWidth()
 	if river_object is None:
 		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
 		exit()
 	else:
 		if not isinstance(river_object, centerline_width.riverCenterline):
 			logger.critical("\nCRITICAL ERROR, [river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{0}'".format(type(river_object)))
@@ -138,19 +149,29 @@
 		logger.critical("\nCRITICAL ERROR, [flag_intersections]: Must be a bool, current type = '{0}'".format(type(flag_intersections)))
 		exit()
 
 	if type(remove_intersections) != bool:
 		logger.critical("\nCRITICAL ERROR, [remove_intersections]: Must be a bool, current type = '{0}'".format(type(remove_intersections)))
 		exit()
 
+	if type(coordinate_type) != str:
+		logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(type(coordinate_type)))
+		exit()
+	else:
+		coordinate_type_options = ["Decimal Degrees", "Relative Distance"]
+		if coordinate_type.title() not in coordinate_type_options:
+			logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be an available option in {0}, current option = '{1}'".format(coordinate_type_options, coordinate_type))
+			exit()
+
 ## Error Handling: centerline.py
 def errorHandlingRiverWidthFromCenterline(river_object=None,
 										transect_span_distance=None,
 										apply_smoothing=None,
 										remove_intersections=None,
+										coordinate_type=None,
 										save_to_csv=None):
 	# Error Handling for riverWidthFromCenterline()
 	if river_object is None:
 		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
 		exit()
 	else:
 		if not isinstance(river_object, centerline_width.riverCenterline):
@@ -170,23 +191,37 @@
 		logger.critical("\nCRITICAL ERROR, [apply_smoothing]: Must be a bool, current type = '{0}'".format(type(apply_smoothing)))
 		exit()
 
 	if type(remove_intersections) != bool:
 		logger.critical("\nCRITICAL ERROR, [remove_intersections]: Must be a bool, current type = '{0}'".format(type(remove_intersections)))
 		exit()
 
+	if type(coordinate_type) != str:
+		logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(type(coordinate_type)))
+		exit()
+	else:
+		coordinate_type_options = ["Decimal Degrees", "Relative Distance"]
+		if coordinate_type.title() not in coordinate_type_options:
+			logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be an available option in {0}, current option = '{1}'".format(coordinate_type_options, coordinate_type))
+			exit()
+
 	if save_to_csv is not None:
 		if type(save_to_csv) != str:
 			logger.critical("\nCRITICAL ERROR, [save_to_csv]: Must be a str, current type = '{0}'".format(type(save_to_csv)))
 			exit()
 		if not save_to_csv.lower().endswith(".csv"):
 			logger.critical("\nCRITICAL ERROR, [save_to_csv]: Extension must be a .csv file, current extension = '{0}'".format(save_to_csv.split(".")[1]))
 			exit()
 
-def errorHandlingSaveCenterlineCSV(river_object=None, latitude_header=None, longitude_header=None, save_to_csv=None, centerline_type=None):
+def errorHandlingSaveCenterlineCSV(river_object=None,
+								latitude_header=None,
+								longitude_header=None,
+								save_to_csv=None,
+								centerline_type=None,
+								coordinate_type=None):
 	# Error Handling for saveCenterlineCSV()
 	if river_object is None:
 		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
 		exit()
 	else:
 		if not isinstance(river_object, centerline_width.riverCenterline):
 			logger.critical("\nCRITICAL ERROR, [river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{0}'".format(type(river_object)))
@@ -216,15 +251,29 @@
 		logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be a str, current type = '{0}'".format(type(centerline_type)))
 		exit()
 	else:
 		if centerline_type.title() not in centerline_type_options:
 			logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be an available option in {0}, current option = '{1}'".format(centerline_type_options, centerline_type))
 			exit()
 
-def errorHandlingSaveCenterlineMAT(river_object=None, latitude_header=None, longitude_header=None, save_to_mat=None, centerline_type=None):
+	if type(coordinate_type) != str:
+		logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(type(coordinate_type)))
+		exit()
+	else:
+		coordinate_type_options = ["Decimal Degrees", "Relative Distance"]
+		if coordinate_type.title() not in coordinate_type_options:
+			logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be an available option in {0}, current option = '{1}'".format(coordinate_type_options, coordinate_type))
+			exit()
+
+def errorHandlingSaveCenterlineMAT(river_object=None,
+								latitude_header=None,
+								longitude_header=None,
+								save_to_mat=None,
+								centerline_type=None,
+								coordinate_type=None):
 	# Error Handling for saveCenterlineMAT()
 	if river_object is None:
 		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
 		exit()
 	else:
 		if not isinstance(river_object, centerline_width.riverCenterline):
 			logger.critical("\nCRITICAL ERROR, [river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{0}'".format(type(river_object)))
@@ -262,14 +311,23 @@
 		logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be a str, current type = '{0}'".format(type(centerline_type)))
 		exit()
 	else:
 		if centerline_type.title() not in centerline_type_options:
 			logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be an available option in {0}, current option = '{1}'".format(centerline_type_options, centerline_type))
 			exit()
 
+	if type(coordinate_type) != str:
+		logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(type(coordinate_type)))
+		exit()
+	else:
+		coordinate_type_options = ["Decimal Degrees", "Relative Distance"]
+		if coordinate_type.title() not in coordinate_type_options:
+			logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be an available option in {0}, current option = '{1}'".format(coordinate_type_options, coordinate_type))
+			exit()
+
 # Error Handling: getCoordinatesKML.py
 def errorHandlingExtractPointsToTextFile(left_kml=None, right_kml=None, text_output_name=None):
 	# Error Handling for extractPointsToTextFile()
 	if left_kml is None:
 		logger.critical("\nCRITICAL ERROR, [left_kml]: Requires left_kml file")
 		exit()
 	else:
```

### Comparing `centerline-width-1.0.1/centerline_width/getCoordinatesKML.py` & `centerline-width-1.1.0/centerline_width/getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.1/centerline_width/plotDiagrams.py` & `centerline-width-1.1.0/centerline_width/plotDiagrams.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,57 +15,75 @@
 stream_handler = logging.StreamHandler()
 logger.addHandler(stream_handler)
 
 def plotCenterlineBackend(river_object=None,
 						display_true_centerline=True,
 						centerline_type="Voronoi",
 						marker_type="line",
-						centerline_color="black"):
+						centerline_color="black",
+						coordinate_type=None):
 	# Shared components between plotCenterline and plotCenterlineWidth
 	fig = plt.figure(figsize=(10,10))
 	ax = fig.add_subplot(111)
+	scatter_plot_size = 4
 	
+	coordinate_type = coordinate_type.title()
 	# Plot River as a Polygon
-	plt.plot(*river_object.bank_polygon.exterior.xy, c="gainsboro")
-	plt.plot(*river_object.top_bank.xy, c="forestgreen")
-	plt.plot(*river_object.bottom_bank.xy, c="lightcoral")
+	if coordinate_type == "Decimal Degrees":
+		plt.plot(*river_object.bank_polygon.exterior.xy, c="gainsboro")
+		plt.plot(*river_object.top_bank.xy, c="forestgreen")
+		plt.plot(*river_object.bottom_bank.xy, c="lightcoral")
+	if coordinate_type == "Relative Distance":
+		plt.plot(*river_object.bank_polygon_relative.exterior.xy, c="gainsboro")
+		plt.plot(*river_object.top_bank_relative.xy, c="forestgreen")
+		plt.plot(*river_object.bottom_bank_relative.xy, c="lightcoral")
+
+	# Choose between Decimal Degrees and Relative Distances for X, Y coordinates
+	if coordinate_type == "Decimal Degrees":
+		right_coords =  river_object.right_bank_coordinates
+		left_coords =  river_object.left_bank_coordinates
+	if coordinate_type == "Relative Distance":
+		right_coords =  river_object.right_bank_relative_coordinates
+		left_coords =  river_object.left_bank_relative_coordinates
 
-	scatter_plot_size = 4
-	x = []
-	y = []
-	for i in river_object.right_bank_coordinates: 
-		x.append(i[0])
-		y.append(i[1])
+	x = [i[0] for i in right_coords]
+	y = [i[1] for i in right_coords]
 	plt.scatter(x, y, c="dodgerblue", s=scatter_plot_size, label="Right Bank")
-	x = []
-	y = []
-	for i in river_object.left_bank_coordinates:
-		x.append(i[0])
-		y.append(i[1])
+	x = [i[0] for i in left_coords]
+	y = [i[1] for i in left_coords]
 	plt.scatter(x, y, c="orange", s=scatter_plot_size, label="Left Bank")
 
 	# Plot centerline found from NetworkX
 	valid_path_through = False
 
 	centerline_type = centerline_type.title()
 	marker_type = marker_type.title()
 
+	# Choose btween Decimal Degrees and Centerline Type
 	if centerline_type == "Voronoi": 
-		centerline_coordinates_by_type = river_object.centerlineVoronoi
 		centerline_legend = "Voronoi Centerline Coordinates"
+		if coordinate_type == "Decimal Degrees": centerline_coordinates_by_type = river_object.centerlineVoronoi
+		if coordinate_type == "Relative Distance": centerline_coordinates_by_type = river_object.centerlineVoronoiRelative
+
 	if centerline_type == "Equal Distance": 
-		centerline_coordinates_by_type = river_object.centerlineEqualDistance
 		centerline_legend = "Equal Distance Centerline Coordinates"
+		if coordinate_type == "Decimal Degrees": centerline_coordinates_by_type = river_object.centerlineEqualDistance
+		if coordinate_type == "Relative Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistanceRelative
+
 	if centerline_type == "Evenly Spaced": 
-		centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
 		centerline_legend = "Evenly Spaced Centerline Coordiantes"
+		if coordinate_type == "Decimal Degrees": centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
+		if coordinate_type == "Relative Distance": centerline_coordinates_by_type = river_object.centerlineEvenlySpacedRelative
+
 	if centerline_type == "Smoothed": 
-		centerline_coordinates_by_type = river_object.centerlineSmoothed
 		centerline_legend = "Smoothed Centerlined Coordiantes"
+		if coordinate_type == "Decimal Degrees": centerline_coordinates_by_type = river_object.centerlineSmoothed
+		if coordinate_type == "Relative Distance": centerline_coordinates_by_type = river_object.centerlineSmoothedRelative
 
+	# Plot the centerline coordinates
 	if centerline_coordinates_by_type:
 		valid_path_through = True
 		if display_true_centerline:
 			if marker_type == "Line":
 				plt.plot(*zip(*centerline_coordinates_by_type), c=centerline_color, label=centerline_legend, zorder=10)
 			if marker_type == "Scatter":
 				x = []
@@ -73,112 +91,150 @@
 				for k, v in centerline_coordinates_by_type:
 					x.append(k)
 					y.append(v)
 				plt.scatter(x, y, c=centerline_color, label=centerline_legend, s=8, zorder=10)
 
 	# Dynamically assign the starting and ending
 	if river_object.starting_node is not None: # error handling for when data is too small to generate centerline coordiantes
-		plt.scatter(river_object.starting_node[0], river_object.starting_node[1], c="green", label="Starting Node", s=45)
-		plt.scatter(river_object.ending_node[0], river_object.ending_node[1], c="red", label="Ending Node", s=45)
+		ss = 45 # scatter size
+		if coordinate_type == "Decimal Degrees":
+			plt.scatter(river_object.starting_node[0], river_object.starting_node[1], c="green", label="Starting Node", s=ss)
+			plt.scatter(river_object.ending_node[0], river_object.ending_node[1], c="red", label="Ending Node", s=ss)
+		if coordinate_type == "Relative Distance":
+			plt.scatter(river_object.starting_node_relative[0], river_object.starting_node_relative[1], c="green", label="Starting Node", s=ss)
+			plt.scatter(river_object.ending_node_relative[0], river_object.ending_node_relative[1], c="red", label="Ending Node", s=ss)
 
 	return fig, ax, valid_path_through
 
 def plotCenterline(river_object=None,
 					centerline_type="Voronoi",
 					marker_type="line",
 					centerline_color="black",
 					display_all_possible_paths=False, 
 					plot_title=None, 
 					save_plot_name=None, 
-					display_voronoi=False):
+					display_voronoi=False,
+					coordinate_type="Decimal Degrees"):
 	# Plot Centerline of River
 	centerline_width.errorHandlingPlotCenterline(river_object=river_object,
 												centerline_type=centerline_type,
 												marker_type=marker_type,
 												centerline_color=centerline_color,
 												display_all_possible_paths=display_all_possible_paths,
 												plot_title=plot_title,
 												save_plot_name=save_plot_name,
-												display_voronoi=display_voronoi)
+												display_voronoi=display_voronoi,
+												coordinate_type=coordinate_type)
 
 	fig, ax, valid_path_through = plotCenterlineBackend(river_object=river_object,
 														display_true_centerline=True,
 														centerline_type=centerline_type,
 														marker_type=marker_type,
-														centerline_color=centerline_color)
+														centerline_color=centerline_color,
+														coordinate_type=coordinate_type)
+
+	coordinate_type = coordinate_type.title()
 
 	# Display the Voronoi Diagram
 	if display_voronoi:
-		voronoi_plot_2d(river_object.bank_voronoi, show_points=True, point_size=1, ax=ax)
+		if coordinate_type == "Decimal Degrees":
+			voronoi_plot_2d(river_object.bank_voronoi, show_points=True, point_size=1, ax=ax)
+		if coordinate_type == "Relative Distance":
+			voronoi_plot_2d(river_object.bank_voronoi_relative, show_points=True, point_size=1, ax=ax)
 
 	# Plot all possible paths with text for positions
 	if display_all_possible_paths:
-		for i in range(len(river_object.x_voronoi_ridge_point)):
-			plt.plot(river_object.x_voronoi_ridge_point[i], river_object.y_voronoi_ridge_point[i], 'cyan', linewidth=1, zorder=1)
+		if coordinate_type == "Decimal Degrees":
+			for i in range(len(river_object.x_voronoi_ridge_point)):
+				plt.plot(river_object.x_voronoi_ridge_point[i], river_object.y_voronoi_ridge_point[i], 'cyan', linewidth=1, zorder=1)
+		if coordinate_type == "Relative Distance":
+			for i in range(len(river_object.x_voronoi_ridge_point_relative)):
+				plt.plot(river_object.x_voronoi_ridge_point_relative[i], river_object.y_voronoi_ridge_point_relative[i], 'cyan', linewidth=1, zorder=1)
 
 	# Plot Title, Legends, and Axis Labels
 	if not plot_title:
 		plt.title("River Coordinates: Valid Centerline = {0}, Valid Polygon = {1}, Interpolated = {2}".format(valid_path_through, river_object.bank_polygon.is_valid, river_object.interpolate_data))
 	else:
 		plt.title(plot_title)
-	plt.xlabel("Longitude (°)")
-	plt.ylabel("Latitude (°)")
+
+	if coordinate_type == "Decimal Degrees":
+		plt.xlabel("Longitude (°)")
+		plt.ylabel("Latitude (°)")
+	if coordinate_type == "Relative Distance":
+		plt.xlabel("Relative Distance X (m)")
+		plt.ylabel("Relative Distance Y (m)")
+
 	plt.legend(loc="upper right")
 	plt.show()
 	if save_plot_name: fig.savefig(save_plot_name)
 
 def plotCenterlineWidth(river_object=None,
 						plot_title=None, 
 						save_plot_name=None, 
 						display_true_centerline=True,
 						transect_span_distance=3,
 						apply_smoothing=False,
 						flag_intersections=True,
-						remove_intersections=False):
+						remove_intersections=False,
+						coordinate_type="Decimal Degrees"):
 	# Plot Width Lines based on Centerline
 	centerline_width.errorHandlingPlotCenterlineWidth(river_object=river_object,
 													plot_title=plot_title, 
 													save_plot_name=save_plot_name, 
 													display_true_centerline=display_true_centerline,
 													transect_span_distance=transect_span_distance,
 													apply_smoothing=apply_smoothing,
 													flag_intersections=flag_intersections,
-													remove_intersections=remove_intersections)
+													remove_intersections=remove_intersections,
+													coordinate_type=coordinate_type)
 
 	fig, ax, valid_path_through = plotCenterlineBackend(river_object=river_object, 
 														display_true_centerline=display_true_centerline,
 														centerline_type="Voronoi",
 														marker_type="line",
-														centerline_color="black")
+														centerline_color="black",
+														coordinate_type=coordinate_type)
 
+	coordinate_type = coordinate_type.title()
 	# Determine the Width of River
 	number_of_evenly_spaced_points = ""
 
 	if river_object.centerlineVoronoi is not None:
 		number_of_evenly_spaced_points = "\nCenterline made of {0} Fixed Points, width lines generated every {1} points".format(river_object.interpolate_n_centerpoints, transect_span_distance)
 		if river_object.starting_node is not None: # error handling for when data is too small to generate centerline coordiantes
+
+			# if using smoothing, replace left/right coordinates with the smoothed variation
 			if apply_smoothing:
-				# if using smoothing, replace left/right coordinates with the smoothed variation
 				right_width_coordinates, left_width_coordinates, num_intersection_coordinates = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object,
 																																					centerline_coordinates=river_object.centerlineSmoothed,
 																																					transect_span_distance=transect_span_distance,
 																																					remove_intersections=remove_intersections)
 				x = []
 				y = []
-				for k, v in river_object.centerlineSmoothed:
+				if coordinate_type == "Decimal Degrees":
+					smoothed_coords = river_object.centerlineSmoothed
+				if coordinate_type == "Relative Distance":
+					smoothed_coords = river_object.centerlineSmoothedRelative
+				for k, v in smoothed_coords:
 					x.append(k)
 					y.append(v)
 				plt.scatter(x, y, c="blue", label="Smoothed Centerline Coordinates", s=5)
 			else:
 				# recreate the centerline with evenly spaced points
 				right_width_coordinates, left_width_coordinates, num_intersection_coordinates = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object, 
 																														centerline_coordinates=river_object.centerlineEvenlySpaced,
 																														transect_span_distance=transect_span_distance,
 																														remove_intersections=remove_intersections)
 
+			if coordinate_type == "Relative Distance":
+				# by default, sets up width with Decimal Degree, convert to Relative Distance
+				right_width_coordinates = centerline_width.relativeWidthCoordinates(river_object.left_bank_coordinates[0], right_width_coordinates, river_object.ellipsoid)
+				left_width_coordinates = centerline_width.relativeWidthCoordinates(river_object.left_bank_coordinates[0], left_width_coordinates, river_object.ellipsoid)
+				num_intersection_coordinates = centerline_width.relativeWidthCoordinates(river_object.left_bank_coordinates[0], num_intersection_coordinates, river_object.ellipsoid)
+
 			invalid_label_added = False # prevent legend for width lines from being generated more than once (because is inside a loop)
 			valid_label_added = False  # prevent legend for width lines from being generated more than once (because is inside a loop)
 			# plot width lines
 			for center_coord, edge_coord in right_width_coordinates.items():
 				x_points = (right_width_coordinates[center_coord][0], left_width_coordinates[center_coord][0])
 				y_points = (right_width_coordinates[center_coord][1], left_width_coordinates[center_coord][1])
 				if flag_intersections:
@@ -204,12 +260,18 @@
 						plt.plot(x_points, y_points, 'green', linewidth=1)
 
 	# Plot Title, Legends, and Axis Labels
 	if not plot_title:
 		plt.title("River Width Coordinates: Valid Centerline = {0}, Valid Polygon = {1}{2}, Interpolated = {3}".format(valid_path_through, river_object.bank_polygon.is_valid, number_of_evenly_spaced_points, river_object.interpolate_data))
 	else:
 		plt.title(plot_title)
-	plt.xlabel("Longitude (°)")
-	plt.ylabel("Latitude (°)")
+
+	if coordinate_type == "Decimal Degrees":
+		plt.xlabel("Longitude (°)")
+		plt.ylabel("Latitude (°)")
+	if coordinate_type == "Relative Distance":
+		plt.xlabel("Relative Distance X (m)")
+		plt.ylabel("Distance Distance Y (m)")
+
 	plt.legend(loc="upper right")
 	plt.show()
 	if save_plot_name: fig.savefig(save_plot_name)
```

### Comparing `centerline-width-1.0.1/centerline_width/preprocessing.py` & `centerline-width-1.1.0/centerline_width/preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.1/centerline_width/pytests/test_centerline.py` & `centerline-width-1.1.0/centerline_width/pytests/test_centerline.py`

 * *Files 10% similar despite different names*

```diff
@@ -97,14 +97,32 @@
 	with pytest.raises(SystemExit):
 		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
 												save_to_csv="filename.txt")
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [save_to_csv]: Extension must be a .csv file, current extension = 'txt'"
 
+def test_riverWidthFromCenterline_coordinateTypeInvalidOption(caplog):
+	with pytest.raises(SystemExit):
+		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
+										coordinate_type="Invalid Option")
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'"
+
+@pytest.mark.parametrize("coordinate_type_name_invalid, coordinate_type_error_output", invalid_non_str_options)
+def test_riverWidthFromCenterline_coordinateTypeInvalidTypes(caplog, coordinate_type_name_invalid, coordinate_type_error_output):
+	with pytest.raises(SystemExit):
+		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
+										coordinate_type=coordinate_type_name_invalid)
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(coordinate_type_error_output)
+
+
 ## saveCenterlineCSV() #####################################################
 def test_saveCenterlineCSV_riverObjectRequired(caplog):
 	with pytest.raises(SystemExit):
 		centerline_width.saveCenterlineCSV(river_object=None)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)"
@@ -158,14 +176,33 @@
 		centerline_width.saveCenterlineCSV(river_object=river_class_example,
 											save_to_csv="testing.csv",
 											centerline_type="not valid")
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [centerline_type]: Must be an available option in ['Voronoi', 'Evenly Spaced', 'Smoothed', 'Equal Distance'], current option = 'not valid'"
 
+def test_saveCenterlineCSV_coordinateTypeInvalidOption(caplog):
+	with pytest.raises(SystemExit):
+		centerline_width.saveCenterlineCSV(river_object=river_class_example,
+										save_to_csv="testing.csv",
+										coordinate_type="Invalid Option")
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'"
+
+@pytest.mark.parametrize("coordinate_type_name_invalid, coordinate_type_error_output", invalid_non_str_options)
+def test_saveCenterlineCSV_coordinateTypeInvalidTypes(caplog, coordinate_type_name_invalid, coordinate_type_error_output):
+	with pytest.raises(SystemExit):
+		centerline_width.saveCenterlineCSV(river_object=river_class_example,
+										save_to_csv="testing.csv",
+										coordinate_type=coordinate_type_name_invalid)
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(coordinate_type_error_output)
+
 ## saveCenterlineMAT() #####################################################
 def test_saveCenterlineMAT_riverObjectRequired(caplog):
 	with pytest.raises(SystemExit):
 		centerline_width.saveCenterlineMAT(river_object=None)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)"
@@ -236,7 +273,26 @@
 	with pytest.raises(SystemExit):
 		centerline_width.saveCenterlineMAT(river_object=river_class_example,
 											save_to_mat="testing.mat",
 											centerline_type="not valid")
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [centerline_type]: Must be an available option in ['Voronoi', 'Evenly Spaced', 'Smoothed', 'Equal Distance'], current option = 'not valid'"
+
+def test_saveCenterlineMAT_coordinateTypeInvalidOption(caplog):
+	with pytest.raises(SystemExit):
+		centerline_width.saveCenterlineMAT(river_object=river_class_example,
+										save_to_mat="testing.mat",
+										coordinate_type="Invalid Option")
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'"
+
+@pytest.mark.parametrize("coordinate_type_name_invalid, coordinate_type_error_output", invalid_non_str_options)
+def test_saveCenterlineMAT_coordinateTypeInvalidTypes(caplog, coordinate_type_name_invalid, coordinate_type_error_output):
+	with pytest.raises(SystemExit):
+		centerline_width.saveCenterlineMAT(river_object=river_class_example,
+										save_to_mat="testing.mat",
+										coordinate_type=coordinate_type_name_invalid)
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(coordinate_type_error_output)
```

### Comparing `centerline-width-1.0.1/centerline_width/pytests/test_getCoordinatesKML.py` & `centerline-width-1.1.0/centerline_width/pytests/test_getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.1/centerline_width/pytests/test_plotDiagrams.py` & `centerline-width-1.1.0/centerline_width/pytests/test_plotDiagrams.py`

 * *Files 12% similar despite different names*

```diff
@@ -133,14 +133,31 @@
 	with pytest.raises(SystemExit):
 		centerline_width.plotCenterline(river_object=river_class_example,
 										display_voronoi=display_voronoi_name_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [display_voronoi]: Must be a bool, current type = '{0}'".format(display_voronoi_error_output)
 
+def test_plotCenterline_coordinateTypeInvalidOption(caplog):
+	with pytest.raises(SystemExit):
+		centerline_width.plotCenterline(river_object=river_class_example,
+										coordinate_type="Invalid Option")
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'"
+
+@pytest.mark.parametrize("coordinate_type_name_invalid, coordinate_type_error_output", invalid_non_str_options)
+def test_plotCenterline_coordinateTypeInvalidTypes(caplog, coordinate_type_name_invalid, coordinate_type_error_output):
+	with pytest.raises(SystemExit):
+		centerline_width.plotCenterline(river_object=river_class_example,
+										coordinate_type=coordinate_type_name_invalid)
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(coordinate_type_error_output)
+
 ## plotCenterlineWidth() #####################################################
 def test_plotCenterlineWidth_riverObjectRequired(caplog):
 	with pytest.raises(SystemExit):
 		centerline_width.plotCenterlineWidth(river_object=None)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)"
@@ -211,7 +228,24 @@
 def test_plotCenterlineWidth_removeIntersectionsInvalidTypes(caplog, remove_intersections_invalid, remove_intersections_error_output):
 	with pytest.raises(SystemExit):
 		centerline_width.plotCenterlineWidth(river_object=river_class_example,
 											remove_intersections=remove_intersections_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [remove_intersections]: Must be a bool, current type = '{0}'".format(remove_intersections_error_output)
+
+def test_plotCenterlineWidth_coordinateTypeInvalidOption(caplog):
+	with pytest.raises(SystemExit):
+		centerline_width.plotCenterlineWidth(river_object=river_class_example,
+										coordinate_type="Invalid Option")
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'"
+
+@pytest.mark.parametrize("coordinate_type_name_invalid, coordinate_type_error_output", invalid_non_str_options)
+def test_plotCenterlineWidth_coordinateTypeInvalidTypes(caplog, coordinate_type_name_invalid, coordinate_type_error_output):
+	with pytest.raises(SystemExit):
+		centerline_width.plotCenterlineWidth(river_object=river_class_example,
+										coordinate_type=coordinate_type_name_invalid)
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(coordinate_type_error_output)
```

### Comparing `centerline-width-1.0.1/centerline_width/pytests/test_preprocessing.py` & `centerline-width-1.1.0/centerline_width/pytests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.1/centerline_width/pytests/test_riverCenterlineClass.py` & `centerline-width-1.1.0/centerline_width/pytests/test_riverCenterlineClass.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.1/centerline_width/riverCenterlineClass.py` & `centerline-width-1.1.0/centerline_width/riverCenterlineClass.py`

 * *Files 19% similar despite different names*

```diff
@@ -37,36 +37,54 @@
 
 		# Left and Right Coordinates from the given csv data and data cutoff
 		left_bank_coordinates, right_bank_coordinates = centerline_width.leftRightCoordinates(df)
 		if interpolate_data:
 			right_bank_coordinates, left_bank_coordinates = centerline_width.interpolateBetweenPoints(left_bank_coordinates, right_bank_coordinates, interpolate_n)
 		self.left_bank_coordinates = left_bank_coordinates
 		self.right_bank_coordinates = right_bank_coordinates
+		self.left_bank_relative_coordinates, self.right_bank_relative_coordinates = centerline_width.relativeBankCoordinates(self.left_bank_coordinates, self.right_bank_coordinates, self.ellipsoid)
 
 		# Right/Length Bank Length
 		self.rightBankLength = centerline_width.centerlineLength(centerline_coordinates=right_bank_coordinates, ellipsoid=self.ellipsoid)
 		self.leftBankLength = centerline_width.centerlineLength(centerline_coordinates=left_bank_coordinates, ellipsoid=self.ellipsoid)
 
-		# River polygon, position of the top/bottom polygon
+		# Decimal Degrees: River polygon, position of the top/bottom polygon
 		river_bank_polygon, top_bank, bottom_bank = centerline_width.generatePolygon(self.left_bank_coordinates, self.right_bank_coordinates)
 		self.bank_polygon = river_bank_polygon
 		self.top_bank = top_bank
 		self.bottom_bank = bottom_bank
 
-		# Voronoi generated by left/right bank coordinates
+		# Relative Coordinates: River polygon, position of the top/bottom polygon
+		river_bank_polygon, top_bank, bottom_bank = centerline_width.generatePolygon(self.left_bank_relative_coordinates, self.right_bank_relative_coordinates)
+		self.bank_polygon_relative = river_bank_polygon
+		self.top_bank_relative = top_bank
+		self.bottom_bank_relative = bottom_bank
+
+		# Decimal Degrees; Voronoi generated by left/right bank coordinates
 		river_bank_voronoi = centerline_width.generateVoronoi(self.left_bank_coordinates, self.right_bank_coordinates)
 		self.bank_voronoi = river_bank_voronoi
 
-		# All possible paths: starting/ending node, all possible paths (ridges), paths dictionary
+		# Relative Distance; Voronoi generated by left/right bank coordinates
+		river_bank_voronoi = centerline_width.generateVoronoi(self.left_bank_relative_coordinates, self.right_bank_relative_coordinates)
+		self.bank_voronoi_relative = river_bank_voronoi
+
+		# Decimal Degrees all possible paths: starting/ending node, all possible paths (ridges), paths dictionary
 		starting_node, ending_node, x_ridge_point, y_ridge_point, shortest_path_coordinates = centerline_width.centerlinePath(self.bank_voronoi, self.bank_polygon, self.top_bank, self.bottom_bank)
 		self.starting_node = starting_node # starting position for centerline
 		self.ending_node = ending_node # ending position for centerline
 		self.x_voronoi_ridge_point = x_ridge_point # Voronoi x positions
 		self.y_voronoi_ridge_point = y_ridge_point # Voronoi y postions
 
+		# Relative Distances all possible paths: starting/ending node, all possible paths (ridges), paths dictionary
+		self.starting_node_relative = centerline_width.relativeSingleCoordinate(self.left_bank_coordinates[0], self.starting_node, self.ellipsoid) # starting position for centerline
+		self.ending_node_relative = centerline_width.relativeSingleCoordinate(self.left_bank_coordinates[0], self.ending_node, self.ellipsoid) # ending position for centerline
+		x_relative_ridges, y_relative_ridges = centerline_width.relativeRidgeCoordinates(self.left_bank_coordinates[0], self.x_voronoi_ridge_point, self.y_voronoi_ridge_point, self.ellipsoid)
+		self.x_voronoi_ridge_point_relative = x_relative_ridges # Voronoi relative x positions
+		self.y_voronoi_ridge_point_relative = y_relative_ridges # Voronoi relative y postions
+
 		# Voronoi Centerline Coordinates
 		self.centerlineVoronoi = shortest_path_coordinates
 
 		# Centerline length
 		self.centerlineLength = centerline_width.centerlineLength(centerline_coordinates=shortest_path_coordinates, ellipsoid=self.ellipsoid)
 		self.equal_distance = equal_distance
 
@@ -75,75 +93,89 @@
 																				equal_distance=self.equal_distance,
 																				ellipsoid=self.ellipsoid)
 		self.centerlineEvenlySpaced = centerline_width.evenlySpacedCenterline(centerline_coordinates=self.centerlineVoronoi,
 																				number_of_fixed_points=self.interpolate_n_centerpoints)
 		self.centerlineSmoothed = centerline_width.smoothedCoordinates(river_object=self, centerline_coordinates=self.centerlineEvenlySpaced,
 																		interprolate_num=self.interpolate_n_centerpoints)
 
-
+		# Relative Distance from bottom left bank point to each Centerline coordinates
+		self.centerlineVoronoiRelative = centerline_width.relativeCenterlineCoordinates(self.left_bank_coordinates[0], self.centerlineVoronoi, self.ellipsoid)
+		self.centerlineEqualDistanceRelative = centerline_width.relativeCenterlineCoordinates(self.left_bank_coordinates[0], self.centerlineEqualDistance, self.ellipsoid)
+		self.centerlineEvenlySpacedRelative = centerline_width.relativeCenterlineCoordinates(self.left_bank_coordinates[0], self.centerlineEvenlySpaced, self.ellipsoid)
+		self.centerlineSmoothedRelative = centerline_width.relativeCenterlineCoordinates(self.left_bank_coordinates[0], self.centerlineSmoothed, self.ellipsoid)
 
 	def plotCenterline(self,
 						centerline_type="Voronoi",
 						marker_type="line",
 						centerline_color="black",
 						display_all_possible_paths=False,
 						plot_title=None,
 						save_plot_name=None,
-						display_voronoi=False):
+						display_voronoi=False,
+						coordinate_type="Decimal Degrees"):
 		centerline_width.plotCenterline(river_object=self,
 										centerline_type=centerline_type,
 										marker_type=marker_type,
 										centerline_color=centerline_color,
 										display_all_possible_paths=display_all_possible_paths, 
 										plot_title=plot_title, 
 										save_plot_name=save_plot_name, 
-										display_voronoi=display_voronoi)
+										display_voronoi=display_voronoi,
+										coordinate_type=coordinate_type)
 
 	def plotCenterlineWidth(self,
 							plot_title=None, 
 							save_plot_name=None, 
 							display_true_centerline=True,
 							transect_span_distance=3,
 							apply_smoothing=False,
 							flag_intersections=True,
-							remove_intersections=False):
+							remove_intersections=False,
+							coordinate_type="Decimal Degrees"):
 		centerline_width.plotCenterlineWidth(river_object=self,
 											plot_title=plot_title, 
 											save_plot_name=save_plot_name, 
 											display_true_centerline=display_true_centerline,
 											transect_span_distance=transect_span_distance,
 											apply_smoothing=apply_smoothing,
 											flag_intersections=flag_intersections,
-											remove_intersections=remove_intersections)
+											remove_intersections=remove_intersections,
+											coordinate_type=coordinate_type)
 
 	def riverWidthFromCenterline(self,
 								transect_span_distance=3,
 								apply_smoothing=True,
 								remove_intersections=False,
+								coordinate_type="Decimal Degrees",
 								save_to_csv=None):
 		return centerline_width.riverWidthFromCenterline(river_object=self,
 														transect_span_distance=transect_span_distance,
 														apply_smoothing=apply_smoothing,
 														remove_intersections=remove_intersections,
+														coordinate_type=coordinate_type,
 														save_to_csv=save_to_csv)
 
 	def saveCenterlineCSV(self, 
 						save_to_csv=None,
 						latitude_header=None,
 						longitude_header=None, 
-						centerline_type="Voronoi"):
+						centerline_type="Voronoi",
+						coordinate_type="Decimal Degrees"):
 		return centerline_width.saveCenterlineCSV(river_object=self,
 												save_to_csv=save_to_csv,
 												latitude_header=latitude_header, 
 												longitude_header=longitude_header, 
-												centerline_type=centerline_type)
+												centerline_type=centerline_type,
+												coordinate_type=coordinate_type)
 
 	def saveCenterlineMAT(self,
 						save_to_mat=None, 
 						latitude_header=None,
 						longitude_header=None, 
-						centerline_type="Voronoi"):
+						centerline_type="Voronoi",
+						coordinate_type="Decimal Degrees"):
 		return centerline_width.saveCenterlineMAT(river_object=self,
 												save_to_mat=save_to_mat,
 												latitude_header=latitude_header,
 												longitude_header=longitude_header,
-												centerline_type=centerline_type)
+												centerline_type=centerline_type,
+												coordinate_type=coordinate_type)
```

### Comparing `centerline-width-1.0.1/centerline_width.egg-info/PKG-INFO` & `centerline-width-1.1.0/centerline_width.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.0.1.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.1.0.tar.gz
 Description: # Centerline-Width
          <p align="center">
           <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
@@ -225,125 +225,155 @@
         * centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
         * centerlineEqualDistance (list of tuples): List of the latitude and longitude coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
         * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
         * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
         * centerlineLength (float): Length of the centerline of the river (in km)
         * rightBankLength (float): Length of the right bank of the river (in km)
         * leftBankLength (float): Length of the left bank of the river (in km)
+        * centerlineVoronoiRelative (list of tuples): List of the relative distance coordinates of the centerline generated by Voronoi diagrams
+        * centerlineEqualDistanceRelative (list of tuples): List of the relative distance coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
+        * centerlineEvenlySpacedRelative (list of tuples): List of the relative distance coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
+        * centerlineSmoothedRelative (list of tuples): List of the relative distance coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
         
         **Object (class) additional attributes:**
         
         * river_name (string): name of object, set to the csv_data string
-        * left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
-        * right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
+        * left_bank_coordinates (list of tuples): list of latitude/longtiude coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
+        * right_bank_coordinates (list of tuples) list of latitude/longitude coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
+        * left_bank_relative_coordinates (list of tuples): list of relative distances coordaintes of the left bank, measured as the distance in meters from the first point on the left bank (`[(x, y), (x, y)]`)
+        * right_bank_relative_coordinates (list of tuples): list of relative distances coordaintes of the right bank, measured as the distance in meters from the first point on the left bank (`[(x, y), (x, y)]`)
         * df_len (int): Length of the data frame of the csv data (spliced by the optional_cutoff)
         * equal_distance (int): Distance between points (in meters) used in centerlineEqualDistance, defaults to points every 10 meters
         * ellipsoid (string): Built-in ellipsoid definition of Earth to determine how degrees are converted to meters used by centerlineEqualDistance, defaults to "WGS84"
-        * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate riverbank (used to define an inside and an outside of the river)
-        * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
-        * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
+        * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate the latitude/longtiude coordinate riverbank (used to define an inside and an outside of the river)
+        * bank_polygon_relative (Shapley Polygon): Multi-sided polygon generated to encapsulate the relative distance coordinate riverbank (used to define an inside and an outside of the river)
+        * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon for the latitude/longitude coordinate system
+        * top_bank_relative (Shapley Linestring): Linestring that represents the top of the river/polygon for the relative distance coordinate system
+        * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon for the latitude/longitude coordinate system
+        * bottom_bank_relative (Shapley Linestring): Linestring that represents the bottom of the river/polygon for the relative distance coordinate system
         * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
+        * starting_node_relative (tuple): Tuple of the starting position (relative distance x and relative distance y) of the centerline path
         * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
-        * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
+        * ending_node_relative (tuple): Tuple of the end position (relative distance x and relative distance y) of the centerline path
+        * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks of the latitude/longitude coordinate system
+        * bank_voronoi_relative (scipy Voronoi object): Voronoi generated by left/right banks of the relative distance coordinate system
         * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
         * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
+        * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Relative Distance X position to ending Relative Distance X position)
+        * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Relative Distance Y position to ending Relative Distance Y position)
         * interpolate_data (boolean): if interpolating between existing data, defaults to False
         * interpolate_n (int): specifies how many additional points will be added between points along the riverbank when interpolating data, defaults to 5
         * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the length of the data frame (df_len)
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         ```
         
-        ### Return Latitude/Longitude Coordinates of Centerline
-        Return the latitude/longitude coordinates in units of decimal-degrees of the centerline based on the left and right banks
+        ### Coordinates of Centerline
+        Return the coordinates of the centerline based on the left and right banks with either `Decimal Degree` (latitude/longtiude) or `Relative Distance` (meters)
         
         **Types of Centerlines**
         
         There are four types of centerline coordinates formed from the riverbank data
         
         - **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline.png)
         - **Equal Distance Centerline**: centerline based on Voronoi centerline but each point is equally spaced out from the previous (in meters) and takes into account the radius of the Earth to convert degrees to meters (example below: `equal_distance=10`)
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_centerline.png)
         - **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points (example: `interpolate_n_centerpoints=200`)
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline.png)
         - **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline.png)
         
+        By default, coordinates are formed in `Decimal Degrees`, but can be set to `Relative Distance`. Relative Distance measures the distance (in meters) of a point from the first point on the left bank
+        
         Centerline coordinates are formed by the Voronoi vertices
         ```
         river_object.centerlineVoronoi
         ```
+        | river_object.centerlineVoronoi | river_object.centerlineVoronoiRelative |
+        | ------------- | ------------- |
+        | ![centerlineVoronoi+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline.png) | ![centerlineVoronoiRelative+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline_relative.png) |
         
         Centerline coordinates are formed by Equally Distanced vertices, set by `equal_distance`
         ```
         river_object.centerlineEqualDistance
         ```
+        | river_object.centerlineEqualDistance | river_object.centerlineEqualDistanceRelative |
+        | ------------- | ------------- |
+        | ![centerlineEqualDistance+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_centerline.png) | ![centerlineEqualDistanceRelative+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_centerline_relative.png) |
         
         Centerline coordinates are formed by Evenly Spaced vertices, set by `interpolate_n_centerpoints`
         ```
         river_object.centerlineEvenlySpaced
         ```
+        | river_object.centerlineEvenlySpaced | river_object.centerlineEvenlySpacedRelative |
+        | ------------- | ------------- |
+        | ![centerlineEvenlySpaced+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline.png) | ![centerlineEvenlySpacedRelative+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline_relative.png) |
         
         Centerline coordinates are formed from Smoothed vertices
         ```
         river_object.centerlineSmoothed
         ```
+        | river_object.centerlineSmoothed | river_object.centerlineSmoothedRelative |
+        | ------------- | ------------- |
+        | ![centerlineEvenlySpaced+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline.png) | ![centerlineEvenlySpacedRelative+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline_relative.png) |
         
         Example:
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_centerline_coordinates = river_object.centerlineVoronoi
         ```
         Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
         
         ### Save Centerline Coordinates to a .CSV File
         Save the centerline coordinates to a csv file with columns for latitude and longitude. This is the file format for a table of (latitude,longitude) pairs accepted to import back into Google Earth Pro.
         
         ```
-        saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
+        saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi", coordinate_type="Decimal Degrees")
         ```
         * **[REQUIRED]** save_to_csv (string): CSV filename, requires a .csv extension
         * [OPTIONAL] centerline_type (string): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
-        * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)`
-        * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)`
+        * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)` or `<centerline_type> Relative Distance Y (from Latitude) (m)`
+        * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)` or `<centerline_type> Relative Distance X (from Longitude) (m)`
+        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
         ```
         Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
         
         Note: it is best practice to plot the centerline with `plotCenterline()` to ensure that the results saved are as expected
         
         ### Save Centerline Coordinates to a .MAT File
         Save the centerline coordinates to a .mat file with columns for latitude and longitude
         
         ```
-        saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi")
+        saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi", coordinate_type="Decimal Degrees")
         ```
         * **[REQUIRED]** save_to_mat (string): MAT filename, requires a .mat extension
         * [OPTIONAL] centerline_type (string): Centerline type to save to MAT (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
-        * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` (cannot include spaces or special characters)
-        * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` (cannot include spaces or special characters)
+        * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` or `<centerline_type>_Relative_Distance_Y_From_Latitude_m` (cannot include spaces or special characters)
+        * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` or `<centerline_type>_Relative_Distance_X_From_Longitude_m` (cannot include spaces or special characters)
+        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineMAT(save_to_mat="centerline_coordinates.mat", centerline_type="Smoothed")
         ```
         Returns a .mat file with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed_Centerline_Latitude_(Deg), Smoothed_Centerline_Longitude_(Deg)`
         
         Note: it is best practice to plot the centerline with `plotCenterline()` to ensure that the results saved are as expected
         
-        ### Return Length of Centerline
+        ### Length of Centerline
         Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
         ```
         river_object.centerlineLength
         ```
         Length returned in kilometers
         ```python
         import centerline_width
@@ -358,23 +388,25 @@
         ```
         plotCenterline(centerline_type="Voronoi",
         		marker_type="line",
         		centerline_color="black",
         		display_all_possible_paths=False, 
         		plot_title=None, 
         		save_plot_name=None, 
-        		display_voronoi=False)
+        		display_voronoi=False,
+        		coordinate_type="Decimal Degrees")
         ```
         * [OPTIONAL] centerline_type (string): Centerline type graph within river (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
         * [OPTIONAL] marker_type (string): Graph type (not case-sensitive), options: ["Line", "Scatter"], defaults to "Line"
         * [OPTIONAL] centerline_color (string): Color of centerline coordinates on graph (not case-sensitive), options: [matplotlib named colors](https://matplotlib.org/stable/gallery/color/named_colors.html), defaults to "black"
         * [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging), defaults to False
         * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
         * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
         * [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline, defaults to False
+        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.plotCenterline()
         ```
         Output:
@@ -388,23 +420,25 @@
         ```
         plotCenterlineWidth(plot_title=None, 
         		save_plot_name=None, 
         		display_true_centerline=True,
         		transect_span_distance=3,
         		apply_smoothing=False,
         		flag_intersections=True,
-        		remove_intersections=False)
+        		remove_intersections=False,
+        		coordinate_type="Decimal Degrees")
         ```
         * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
         * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
         * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
         * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
         * [OPTIONAL] flag_intersections (boolean): Display intersecting width lines as red in graph, defaults to True
         * [OPTIONAL] remove_intersections (boolean): Remove intersecting lines (but maintain the most width lines as possible) and only return non-intersecting width lines, defaults to False
+        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         
         **apply_smoothing**
         
         apply_smoothing applies a spline to smooth the centerline points created by the Voronoi vertices. This reduces the noise of the slopes and can create width lines that are less susceptible to small changes in the bank
         
         | apply_smoothing=False | apply_smoothing=True |
         | ------------- | ------------- |
@@ -425,14 +459,22 @@
         
         Intersecting lines are flagged in red by default (flag_intersections=True)
         
         | remove_intersections=False | remove_intersections=True |
         | ------------- | ------------- |
         | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
         
+        **coordinate_type**
+        
+        Two options for measuring and displaying coordinates. The two options are "Decimal Degrees" and "Relative Distance". "Decimal Degrees" is the default option that uses the original data coordinate system with latitude/longitude. "Relative Distance" changes the coordinates of each point to be the distance (in meters) from the first point on the left bank
+        
+        | coordinate_type="Decimal Degrees" | remove_intersections="Relative Distance" |
+        | ------------- | ------------- |
+        | ![dd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_decimal_degrees.png) | ![rd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_relative_distance.png)|
+        
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
         ```
         ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
         
@@ -440,19 +482,21 @@
         
         Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width` in meters
         
         ```
         riverWidthFromCenterline(transect_span_distance=3,
         			apply_smoothing=True,
         			remove_intersections=False,
+        			coordinate_type="Decimal Degrees",
         			save_to_csv=None)
         ```
         * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
         * [OPTIONAL] remove_intersections (boolean): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
+        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (km)`)
         
         Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
```

### Comparing `centerline-width-1.0.1/centerline_width.egg-info/SOURCES.txt` & `centerline-width-1.1.0/centerline_width.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 setup.py
 centerline_width/__init__.py
 centerline_width/centerline.py
 centerline_width/error_handling.py
 centerline_width/getCoordinatesKML.py
 centerline_width/plotDiagrams.py
 centerline_width/preprocessing.py
+centerline_width/relativeDistance.py
 centerline_width/riverCenterlineClass.py
 centerline_width.egg-info/PKG-INFO
 centerline_width.egg-info/SOURCES.txt
 centerline_width.egg-info/dependency_links.txt
 centerline_width.egg-info/requires.txt
 centerline_width.egg-info/top_level.txt
 centerline_width/pytests/test_centerline.py
```

### Comparing `centerline-width-1.0.1/setup.py` & `centerline-width-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="1.0.1"
+VERSION="1.1.0"
 DESCRIPTION="A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="centerline-width",
```

