# Comparing `tmp/geodatacrawler-0.1.2.tar.gz` & `tmp/geodatacrawler-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodatacrawler-0.1.2.tar", max compression
+gzip compressed data, was "geodatacrawler-1.1.0.tar", max compression
```

## Comparing `geodatacrawler-0.1.2.tar` & `geodatacrawler-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0     1096 2023-06-20 07:37:01.011896 geodatacrawler-0.1.2/LICENSE
--rwxr-xr-x   0        0        0     5036 2023-06-22 07:00:12.921422 geodatacrawler-0.1.2/README.md
--rwxr-xr-x   0        0        0       23 2023-06-20 07:37:01.153896 geodatacrawler-0.1.2/geodatacrawler/__init__.py
--rwxr-xr-x   0        0        0      220 2023-06-20 07:37:01.153896 geodatacrawler-0.1.2/geodatacrawler/etl.py
--rwxr-xr-x   0        0        0    16594 2023-06-20 07:37:01.154895 geodatacrawler-0.1.2/geodatacrawler/mapfile.py
--rwxr-xr-x   0        0        0    30096 2023-07-06 08:48:38.498475 geodatacrawler-0.1.2/geodatacrawler/metadata.py
--rwxr-xr-x   0        0        0     7379 2023-06-20 07:37:01.156897 geodatacrawler-0.1.2/geodatacrawler/schemas/iso19139/__init__.py
--rwxr-xr-x   0        0        0     3603 2023-06-22 07:00:12.939812 geodatacrawler-0.1.2/geodatacrawler/schemas/iso19139/contact.j2
--rwxr-xr-x   0        0        0    21854 2023-06-22 07:00:12.941435 geodatacrawler-0.1.2/geodatacrawler/schemas/iso19139/main.j2
--rwxr-xr-x   0        0        0      307 2023-07-06 08:28:47.933795 geodatacrawler-0.1.2/geodatacrawler/templates/PGM.tpl
--rwxr-xr-x   0        0        0       21 2023-06-20 07:37:01.159894 geodatacrawler-0.1.2/geodatacrawler/templates/__init__.py
--rwxr-xr-x   0        0        0      118 2023-06-20 07:37:01.160911 geodatacrawler-0.1.2/geodatacrawler/templates/class-line.tpl
--rwxr-xr-x   0        0        0      118 2023-06-20 07:37:01.161895 geodatacrawler-0.1.2/geodatacrawler/templates/class-point.tpl
--rwxr-xr-x   0        0        0      137 2023-06-20 07:37:01.161895 geodatacrawler-0.1.2/geodatacrawler/templates/class-polygon.tpl
--rwxr-xr-x   0        0        0     6622 2023-06-20 07:37:01.162898 geodatacrawler-0.1.2/geodatacrawler/templates/class-raster.tpl
--rwxr-xr-x   0        0        0     2112 2023-06-20 07:37:01.163900 geodatacrawler-0.1.2/geodatacrawler/templates/csv.j2
--rwxr-xr-x   0        0        0     2860 2023-06-20 07:37:01.164899 geodatacrawler-0.1.2/geodatacrawler/templates/default.map
--rwxr-xr-x   0        0        0    12288 2023-06-20 07:37:01.164899 geodatacrawler-0.1.2/geodatacrawler/templates/index.sqlite
--rwxr-xr-x   0        0        0      722 2023-06-20 07:37:01.165896 geodatacrawler-0.1.2/geodatacrawler/templates/layer.tpl
--rwxr-xr-x   0        0        0     6686 2023-06-20 07:37:01.166897 geodatacrawler-0.1.2/geodatacrawler/upload.py
--rwxr-xr-x   0        0        0    17081 2023-06-20 07:37:01.167895 geodatacrawler-0.1.2/geodatacrawler/upload_wosis.py
--rwxr-xr-x   0        0        0    21760 2023-07-04 11:48:26.220044 geodatacrawler-0.1.2/geodatacrawler/utils.py
--rwxr-xr-x   0        0        0     1031 2023-07-31 12:33:42.239832 geodatacrawler-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6133 1970-01-01 00:00:00.000000 geodatacrawler-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1096 2023-06-20 07:37:01.011896 geodatacrawler-1.1.0/LICENSE
+-rwxr-xr-x   0        0        0     3756 2023-07-31 14:47:49.815210 geodatacrawler-1.1.0/README.md
+-rwxr-xr-x   0        0        0       23 2023-06-20 07:37:01.153896 geodatacrawler-1.1.0/geodatacrawler/__init__.py
+-rwxr-xr-x   0        0        0      220 2023-06-20 07:37:01.153896 geodatacrawler-1.1.0/geodatacrawler/etl.py
+-rwxr-xr-x   0        0        0    16594 2023-06-20 07:37:01.154895 geodatacrawler-1.1.0/geodatacrawler/mapfile.py
+-rwxr-xr-x   0        0        0    30113 2023-07-31 14:47:41.294665 geodatacrawler-1.1.0/geodatacrawler/metadata.py
+-rwxr-xr-x   0        0        0     7379 2023-06-20 07:37:01.156897 geodatacrawler-1.1.0/geodatacrawler/schemas/iso19139/__init__.py
+-rwxr-xr-x   0        0        0     3603 2023-07-31 12:57:52.922404 geodatacrawler-1.1.0/geodatacrawler/schemas/iso19139/contact.j2
+-rwxr-xr-x   0        0        0    21854 2023-07-31 12:57:52.930840 geodatacrawler-1.1.0/geodatacrawler/schemas/iso19139/main.j2
+-rwxr-xr-x   0        0        0      307 2023-07-31 12:57:52.942960 geodatacrawler-1.1.0/geodatacrawler/templates/PGM.tpl
+-rwxr-xr-x   0        0        0       21 2023-06-20 07:37:01.159894 geodatacrawler-1.1.0/geodatacrawler/templates/__init__.py
+-rwxr-xr-x   0        0        0      118 2023-06-20 07:37:01.160911 geodatacrawler-1.1.0/geodatacrawler/templates/class-line.tpl
+-rwxr-xr-x   0        0        0      118 2023-06-20 07:37:01.161895 geodatacrawler-1.1.0/geodatacrawler/templates/class-point.tpl
+-rwxr-xr-x   0        0        0      137 2023-06-20 07:37:01.161895 geodatacrawler-1.1.0/geodatacrawler/templates/class-polygon.tpl
+-rwxr-xr-x   0        0        0     6622 2023-06-20 07:37:01.162898 geodatacrawler-1.1.0/geodatacrawler/templates/class-raster.tpl
+-rwxr-xr-x   0        0        0     2112 2023-06-20 07:37:01.163900 geodatacrawler-1.1.0/geodatacrawler/templates/csv.j2
+-rwxr-xr-x   0        0        0     2860 2023-06-20 07:37:01.164899 geodatacrawler-1.1.0/geodatacrawler/templates/default.map
+-rwxr-xr-x   0        0        0    12288 2023-06-20 07:37:01.164899 geodatacrawler-1.1.0/geodatacrawler/templates/index.sqlite
+-rwxr-xr-x   0        0        0      722 2023-06-20 07:37:01.165896 geodatacrawler-1.1.0/geodatacrawler/templates/layer.tpl
+-rwxr-xr-x   0        0        0     6686 2023-06-20 07:37:01.166897 geodatacrawler-1.1.0/geodatacrawler/upload.py
+-rwxr-xr-x   0        0        0    17081 2023-06-20 07:37:01.167895 geodatacrawler-1.1.0/geodatacrawler/upload_wosis.py
+-rwxr-xr-x   0        0        0    21760 2023-07-31 12:57:52.959935 geodatacrawler-1.1.0/geodatacrawler/utils.py
+-rwxr-xr-x   0        0        0     1031 2023-07-31 14:48:01.437700 geodatacrawler-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4890 1970-01-01 00:00:00.000000 geodatacrawler-1.1.0/PKG-INFO
```

### Comparing `geodatacrawler-0.1.2/LICENSE` & `geodatacrawler-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.2/README.md` & `geodatacrawler-1.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,84 @@
 # pyGeoDataCrawler
 
-The tool crawls a data folder, a tree or index file. For each spatial file identified, it will process the file. Extract as many information as possible and store it on a sidecar file. 
+The tool crawls a data folder or tree. For each spatial file identified, it will process the file. Extract as many information as possible and store it on a sidecar metadata file. 
 
-Several options exist for using the results of the index:
+The tool can also look for existing metadata using common conventions. For metadata imports the tool wil use [owslib](https://github.com/geopython/owslib), which supports some metadata formats. 
 
-- The resulting indexed content can be used by [pygeoapi](http://pygeoapi.io) as a backend.
-- Use dashboard software to create visualisations on the indexed content [Apache superset](https://superset.apache.org/)
-- Automated creation of a mapserver mapfile to provide OGC services on top of the spatial files identified
-- Set up an ETL process which triggers conversion of the dataset to an alternative datamodel
+Several options exist for using the results of the generated index:
 
+- The resulting indexed content can be converted to iso19139 or OGCAPI-records and inserted on an instance of pycsw, geonetwork or pygeoapi, to make it searchable.
+- Automated creation of a mapserver mapfile to provide OGC services on top of the spatial files identified.
 
-## Index metadata
+## Installation
 
-The tool looks for existing metadata using common conventions, else it will try to generate the metadata 
-using GDAL/OGR to retrieve details about files. Current backend is SQLite.
+The tool requires GDAL 3.2.2 and pysqlite 0.4.6 to be installed. I recommend to use [conda](https://conda.io/) to install them.
 
-For metadata imports the tool wil use [owslib](https://github.com/geopython/owslib) or [pygeometa](https://github.com/geopython/pygeometa), which supports a some metadata formats. 
+```
+conda create --name pgdc python=3.9 
+conda activate pgdc
+conda install -c conda-forge gdal==3.3.2
+conda install -c conda-forge pysqlite3==0.4.6
+```
 
-Usage (index files recursively from a file folder)
+Then run:
 
 ```
-crawl-metadata --mode=init --dir=/mnt/data [--out-dir=/mnt/mapserver/mapfiles]
+pip install geodatacrawler
+```
+
+## Usage 
+
+The tools are typically called from commandline or a bash script.
+
+### Index metadata
+
+```
+crawl-metadata --mode=init --dir=/myproject/data [--out-dir=/mnt/myoutput]
 ```
 
 Mode explained:
 
 - `init`; creates new metadata for files which do not have it yet (not overwriting)
 - `update`; updates the metadata, merging new content on existing (not creating new)
 - `export`; exports the mcf metadata to xml and stored it in a folder (to be loaded on pycsw) or on a database (todo)
 - `import-csv`; imports a csv of metadata fiels into a series of mcf files, typically combined with a [.j2 file](geodatacrawler/templates/csv.j2) with same name, which `maps` the csv-fields to mcf-fields 
 
-## Minimal metadata
-
-The export utility will merge any yaml file to a index.yaml from a parent folder. This will allow you to create minimal metadata at the detailed level, while providing more generic metadata down the tree. The index.yaml is also used as a configuration for any mapfile creation (service metadata).
-
-## Configuration
+The export utility will merge any yaml file to a index.yml from a parent folder. This will allow you to create minimal metadata at the detailed level, while providing more generic metadata down the tree. The index.yml is also used as a configuration for any mapfile creation (service metadata).
 
 Most parameters are configured from the commandline, check --help to get explanation.
 2 parameters can be set as an environment variable
 
 - pgdc_host is the url on which the data will be hosted in mapserver or a webdav folder.
 - pgdc_schema_path is a physical path to an override of the default iso19139 schema of pygeometa, containing jinja templates to format the exported xml
 
-## Create mapfile
-
+### Create mapfile
 
-The metadata identified can be used to create OGC services exposing the files. Currently the tool creates [mapserver mapfiles](https://www.mapserver.org/mapfile/), which are placed on a output-folder. A configuraton file is expected at the root of the folder to be indexed, if not, it will be created.
+The metadata identified can be used to create OGC services exposing the files. Currently the tool creates [mapserver mapfiles](https://www.mapserver.org/mapfile/), which are placed on a output-folder. A `index.yml` configuraton file is expected at the root of the folder to be indexed, if not, it will be created.
 
 ```
 crawl-mapfile --dir=/mnt/data [--out-dir=/mnt/mapserver/mapfiles]
 ```
 
 A mapserver docker image is available which is able to expose a folder of mapfiles as mapservices, eg http://example.com/{mapfile}?request=getcapabilities&service=wms.
 Idea is that the url to the OGC service will be included in the indexed metadata.
 
-## ETL
-
-Run an ETL process on datasets in a folder structure. This script uses the WOSIS ETL config format and API to trigger the ETL.
-In an initial run, an empty ETL config is generated. In subsequent runs the ETL (updated) config is applied.
+## Development
 
-```
-crawl-etl --dir=/mnt/data [--out-dir=/mnt/data]
-```
-
-## Python Poetry
+### Python Poetry
 
 The project is based on common coding conventions from the python poetry community.
 
-Either run scripts directly
+On the sources, either run scripts directly:
 
 ```
 poetry run crawl-mapfile --dir=/mnt/data
 ```
 
-or run a shell in the poetry env
+or run a shell in the poetry environment:
 
 ```
 poetry shell 
 ```
 
 The GDAL dependency has some installation issue on poetry, see [here](https://stackoverflow.com/a/70986804) for a workaround
 
@@ -85,46 +86,7 @@
 > poetry shell
 >> sudo apt-get install gdal
 >> gdalinfo --version
 GDAL 3.3.2, released 2021/09/01
 >> pip install gdal==3.3.2
 >> exit
 ```
-
-## Docker (used in ci-cd)
-
-In order to synchronise record-loading with record-hosting, we use the isric-pycsw image as a base.
-On top of it python poetry is loaded with the pygeodatacrawler code. this is used as a ci-cd container for example 
-in the lsc-hubs/dataset-inventarisation project
-
-## Sample calls
-
-```
-poetry run crawl-metadata --mode=update --dir=../../ejpsoil/ejpsoildatahub/datasets
-
-poetry run crawl-metadata --mode=import-csv --dir=../../ejpsoil/ejpsoildatahub/datasets --cluster=Country --sep=";" 
-
-poetry run crawl-metadata --mode=export --dir=../../ejpsoil/ejpsoildatahub/datasets --schema= --dir-out=../../ejpsoil/ejpsoildatahub/xml 
-
-```
-
-## Image build
-
-use pycsw image as a base if need also pycsw admin
-
-## WSL-webdav specific
-
-Mount a webdav folder
-
-```
-net use * https://files.example.com
-```
-
-Mount the volume on wsl
-
-```
-sudo mkdir /mnt/z
-sudo mount -t drvfs Z: /mnt/z
-```
-
-## Log
-- june 2023, updated to latest pycsw, this now indexes dist/protocol as format, so terria can filter by 'wms'
```

### Comparing `geodatacrawler-0.1.2/geodatacrawler/mapfile.py` & `geodatacrawler-1.1.0/geodatacrawler/mapfile.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.2/geodatacrawler/metadata.py` & `geodatacrawler-1.1.0/geodatacrawler/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             dir_out = os.path.join(dir_out, db)
             createIndexIfDoesntExist(dir_out)
         elif dbtype == "path":
             if not os.path.exists(dir_out): 
                 print('creating out folder ' + dir_out)
                 os.makedirs(dir_out)
         else:
-            print("postgis not supported")
+            print("Export format "+dbtype+" not supported")
 
     # core metadata gets populated by merging the index.yaml content from parent folders
     initialMetadata = load_default_metadata(mode)
 
     if mode=='import-csv':
         importCsv(dir, dir_out, map, sep, cluster)
     else:
```

### Comparing `geodatacrawler-0.1.2/geodatacrawler/schemas/iso19139/__init__.py` & `geodatacrawler-1.1.0/geodatacrawler/schemas/iso19139/__init__.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.2/geodatacrawler/schemas/iso19139/contact.j2` & `geodatacrawler-1.1.0/geodatacrawler/schemas/iso19139/contact.j2`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.2/geodatacrawler/schemas/iso19139/main.j2` & `geodatacrawler-1.1.0/geodatacrawler/schemas/iso19139/main.j2`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.2/geodatacrawler/templates/class-raster.tpl` & `geodatacrawler-1.1.0/geodatacrawler/templates/class-raster.tpl`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.2/geodatacrawler/templates/csv.j2` & `geodatacrawler-1.1.0/geodatacrawler/templates/csv.j2`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.2/geodatacrawler/templates/default.map` & `geodatacrawler-1.1.0/geodatacrawler/templates/default.map`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.2/geodatacrawler/templates/index.sqlite` & `geodatacrawler-1.1.0/geodatacrawler/templates/index.sqlite`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.2/geodatacrawler/templates/layer.tpl` & `geodatacrawler-1.1.0/geodatacrawler/templates/layer.tpl`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.2/geodatacrawler/upload.py` & `geodatacrawler-1.1.0/geodatacrawler/upload.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.2/geodatacrawler/upload_wosis.py` & `geodatacrawler-1.1.0/geodatacrawler/upload_wosis.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.2/geodatacrawler/utils.py` & `geodatacrawler-1.1.0/geodatacrawler/utils.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.2/pyproject.toml` & `geodatacrawler-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geodatacrawler"
-version = "0.1.2"
+version = "1.1.0"
 license = "MIT"
 description = "a crawler script to extract and author metadata of spatial datasets"
 authors = ["Paul van Genuchten <genuchten@yahoo.com>"]
 readme = "README.md"
 repository = "https://github.com/pvgenuchten/pyGeoDataCrawler"
 packages = [
     { include = "geodatacrawler" },
@@ -12,15 +12,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 PyYAML = "^6.0"
 Fiona = "^1.8.21"
 rasterio = "^1.2.10"
-pysqlite3 = "^0.4.7"
+pysqlite3 = "^0.4.6"
 mappyfile = "^0.9.7"
 GDAL = "3.3.2"
 pyproj = "^3.4.0"
 OWSLib = "^0.27.2"
 pygeometa = "0.13.1"
 pandas = "^1.5.1"
 Jinja2 = "^3.1.2"
```

### Comparing `geodatacrawler-0.1.2/PKG-INFO` & `geodatacrawler-1.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodatacrawler
-Version: 0.1.2
+Version: 1.1.0
 Summary: a crawler script to extract and author metadata of spatial datasets
 Home-page: https://github.com/pvgenuchten/pyGeoDataCrawler
 License: MIT
 Author: Paul van Genuchten
 Author-email: genuchten@yahoo.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,95 +20,96 @@
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: bibtexparser (>=1.4.0,<2.0.0)
 Requires-Dist: jinja2-time (>=0.2.0,<0.3.0)
 Requires-Dist: mappyfile (>=0.9.7,<0.10.0)
 Requires-Dist: pandas (>=1.5.1,<2.0.0)
 Requires-Dist: pygeometa (==0.13.1)
 Requires-Dist: pyproj (>=3.4.0,<4.0.0)
-Requires-Dist: pysqlite3 (>=0.4.7,<0.5.0)
+Requires-Dist: pysqlite3 (>=0.4.6,<0.5.0)
 Requires-Dist: rasterio (>=1.2.10,<2.0.0)
 Project-URL: Repository, https://github.com/pvgenuchten/pyGeoDataCrawler
 Description-Content-Type: text/markdown
 
 # pyGeoDataCrawler
 
-The tool crawls a data folder, a tree or index file. For each spatial file identified, it will process the file. Extract as many information as possible and store it on a sidecar file. 
+The tool crawls a data folder or tree. For each spatial file identified, it will process the file. Extract as many information as possible and store it on a sidecar metadata file. 
 
-Several options exist for using the results of the index:
+The tool can also look for existing metadata using common conventions. For metadata imports the tool wil use [owslib](https://github.com/geopython/owslib), which supports some metadata formats. 
 
-- The resulting indexed content can be used by [pygeoapi](http://pygeoapi.io) as a backend.
-- Use dashboard software to create visualisations on the indexed content [Apache superset](https://superset.apache.org/)
-- Automated creation of a mapserver mapfile to provide OGC services on top of the spatial files identified
-- Set up an ETL process which triggers conversion of the dataset to an alternative datamodel
+Several options exist for using the results of the generated index:
 
+- The resulting indexed content can be converted to iso19139 or OGCAPI-records and inserted on an instance of pycsw, geonetwork or pygeoapi, to make it searchable.
+- Automated creation of a mapserver mapfile to provide OGC services on top of the spatial files identified.
 
-## Index metadata
+## Installation
 
-The tool looks for existing metadata using common conventions, else it will try to generate the metadata 
-using GDAL/OGR to retrieve details about files. Current backend is SQLite.
+The tool requires GDAL 3.2.2 and pysqlite 0.4.6 to be installed. I recommend to use [conda](https://conda.io/) to install them.
 
-For metadata imports the tool wil use [owslib](https://github.com/geopython/owslib) or [pygeometa](https://github.com/geopython/pygeometa), which supports a some metadata formats. 
+```
+conda create --name pgdc python=3.9 
+conda activate pgdc
+conda install -c conda-forge gdal==3.3.2
+conda install -c conda-forge pysqlite3==0.4.6
+```
 
-Usage (index files recursively from a file folder)
+Then run:
 
 ```
-crawl-metadata --mode=init --dir=/mnt/data [--out-dir=/mnt/mapserver/mapfiles]
+pip install geodatacrawler
+```
+
+## Usage 
+
+The tools are typically called from commandline or a bash script.
+
+### Index metadata
+
+```
+crawl-metadata --mode=init --dir=/myproject/data [--out-dir=/mnt/myoutput]
 ```
 
 Mode explained:
 
 - `init`; creates new metadata for files which do not have it yet (not overwriting)
 - `update`; updates the metadata, merging new content on existing (not creating new)
 - `export`; exports the mcf metadata to xml and stored it in a folder (to be loaded on pycsw) or on a database (todo)
 - `import-csv`; imports a csv of metadata fiels into a series of mcf files, typically combined with a [.j2 file](geodatacrawler/templates/csv.j2) with same name, which `maps` the csv-fields to mcf-fields 
 
-## Minimal metadata
-
-The export utility will merge any yaml file to a index.yaml from a parent folder. This will allow you to create minimal metadata at the detailed level, while providing more generic metadata down the tree. The index.yaml is also used as a configuration for any mapfile creation (service metadata).
-
-## Configuration
+The export utility will merge any yaml file to a index.yml from a parent folder. This will allow you to create minimal metadata at the detailed level, while providing more generic metadata down the tree. The index.yml is also used as a configuration for any mapfile creation (service metadata).
 
 Most parameters are configured from the commandline, check --help to get explanation.
 2 parameters can be set as an environment variable
 
 - pgdc_host is the url on which the data will be hosted in mapserver or a webdav folder.
 - pgdc_schema_path is a physical path to an override of the default iso19139 schema of pygeometa, containing jinja templates to format the exported xml
 
-## Create mapfile
-
+### Create mapfile
 
-The metadata identified can be used to create OGC services exposing the files. Currently the tool creates [mapserver mapfiles](https://www.mapserver.org/mapfile/), which are placed on a output-folder. A configuraton file is expected at the root of the folder to be indexed, if not, it will be created.
+The metadata identified can be used to create OGC services exposing the files. Currently the tool creates [mapserver mapfiles](https://www.mapserver.org/mapfile/), which are placed on a output-folder. A `index.yml` configuraton file is expected at the root of the folder to be indexed, if not, it will be created.
 
 ```
 crawl-mapfile --dir=/mnt/data [--out-dir=/mnt/mapserver/mapfiles]
 ```
 
 A mapserver docker image is available which is able to expose a folder of mapfiles as mapservices, eg http://example.com/{mapfile}?request=getcapabilities&service=wms.
 Idea is that the url to the OGC service will be included in the indexed metadata.
 
-## ETL
-
-Run an ETL process on datasets in a folder structure. This script uses the WOSIS ETL config format and API to trigger the ETL.
-In an initial run, an empty ETL config is generated. In subsequent runs the ETL (updated) config is applied.
+## Development
 
-```
-crawl-etl --dir=/mnt/data [--out-dir=/mnt/data]
-```
-
-## Python Poetry
+### Python Poetry
 
 The project is based on common coding conventions from the python poetry community.
 
-Either run scripts directly
+On the sources, either run scripts directly:
 
 ```
 poetry run crawl-mapfile --dir=/mnt/data
 ```
 
-or run a shell in the poetry env
+or run a shell in the poetry environment:
 
 ```
 poetry shell 
 ```
 
 The GDAL dependency has some installation issue on poetry, see [here](https://stackoverflow.com/a/70986804) for a workaround
 
@@ -117,45 +118,7 @@
 >> sudo apt-get install gdal
 >> gdalinfo --version
 GDAL 3.3.2, released 2021/09/01
 >> pip install gdal==3.3.2
 >> exit
 ```
 
-## Docker (used in ci-cd)
-
-In order to synchronise record-loading with record-hosting, we use the isric-pycsw image as a base.
-On top of it python poetry is loaded with the pygeodatacrawler code. this is used as a ci-cd container for example 
-in the lsc-hubs/dataset-inventarisation project
-
-## Sample calls
-
-```
-poetry run crawl-metadata --mode=update --dir=../../ejpsoil/ejpsoildatahub/datasets
-
-poetry run crawl-metadata --mode=import-csv --dir=../../ejpsoil/ejpsoildatahub/datasets --cluster=Country --sep=";" 
-
-poetry run crawl-metadata --mode=export --dir=../../ejpsoil/ejpsoildatahub/datasets --schema= --dir-out=../../ejpsoil/ejpsoildatahub/xml 
-
-```
-
-## Image build
-
-use pycsw image as a base if need also pycsw admin
-
-## WSL-webdav specific
-
-Mount a webdav folder
-
-```
-net use * https://files.example.com
-```
-
-Mount the volume on wsl
-
-```
-sudo mkdir /mnt/z
-sudo mount -t drvfs Z: /mnt/z
-```
-
-## Log
-- june 2023, updated to latest pycsw, this now indexes dist/protocol as format, so terria can filter by 'wms'
```

