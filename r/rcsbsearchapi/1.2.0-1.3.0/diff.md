# Comparing `tmp/rcsbsearchapi-1.2.0.tar.gz` & `tmp/rcsbsearchapi-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsbsearchapi-1.2.0.tar", last modified: Thu Jul 20 15:05:48 2023, max compression
+gzip compressed data, was "rcsbsearchapi-1.3.0.tar", last modified: Mon Jul 31 16:18:51 2023, max compression
```

## Comparing `rcsbsearchapi-1.2.0.tar` & `rcsbsearchapi-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-20 15:05:48.641083 rcsbsearchapi-1.2.0/
--rw-r--r--   0 vsts      (1001) docker     (122)     1543 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    12444 2023-07-20 15:05:48.641083 rcsbsearchapi-1.2.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    11548 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-20 15:05:48.637082 rcsbsearchapi-1.2.0/rcsbsearchapi/
--rw-r--r--   0 vsts      (1001) docker     (122)     1720 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/rcsbsearchapi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      774 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/rcsbsearchapi/const.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-20 15:05:48.641083 rcsbsearchapi-1.2.0/rcsbsearchapi/resources/
--rw-r--r--   0 vsts      (1001) docker     (122)   173785 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/rcsbsearchapi/resources/chemical_schema.json
--rw-r--r--   0 vsts      (1001) docker     (122)  1290883 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/rcsbsearchapi/resources/metadata_schema.json
--rw-r--r--   0 vsts      (1001) docker     (122)     5766 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/rcsbsearchapi/schema.py
--rw-r--r--   0 vsts      (1001) docker     (122)    37888 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/rcsbsearchapi/search.py
--rw-r--r--   0 vsts      (1001) docker     (122)      568 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/rcsbsearchapi/update_schema.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-20 15:05:48.637082 rcsbsearchapi-1.2.0/rcsbsearchapi.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    12444 2023-07-20 15:05:48.000000 rcsbsearchapi-1.2.0/rcsbsearchapi.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      543 2023-07-20 15:05:48.000000 rcsbsearchapi-1.2.0/rcsbsearchapi.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-20 15:05:48.000000 rcsbsearchapi-1.2.0/rcsbsearchapi.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-20 15:05:16.000000 rcsbsearchapi-1.2.0/rcsbsearchapi.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      165 2023-07-20 15:05:48.000000 rcsbsearchapi-1.2.0/rcsbsearchapi.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       14 2023-07-20 15:05:48.000000 rcsbsearchapi-1.2.0/rcsbsearchapi.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       23 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-07-20 15:05:48.641083 rcsbsearchapi-1.2.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     2572 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-20 15:05:48.641083 rcsbsearchapi-1.2.0/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)     2881 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/tests/testschema.py
--rw-r--r--   0 vsts      (1001) docker     (122)    25332 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/tests/testsearch.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-31 16:18:51.334364 rcsbsearchapi-1.3.0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1543 2023-07-31 16:17:48.000000 rcsbsearchapi-1.3.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-07-31 16:17:48.000000 rcsbsearchapi-1.3.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    15684 2023-07-31 16:18:51.334364 rcsbsearchapi-1.3.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    14788 2023-07-31 16:17:48.000000 rcsbsearchapi-1.3.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-31 16:18:51.330364 rcsbsearchapi-1.3.0/rcsbsearchapi/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1720 2023-07-31 16:17:48.000000 rcsbsearchapi-1.3.0/rcsbsearchapi/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      934 2023-07-31 16:17:48.000000 rcsbsearchapi-1.3.0/rcsbsearchapi/const.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-31 16:18:51.334364 rcsbsearchapi-1.3.0/rcsbsearchapi/resources/
+-rw-r--r--   0 vsts      (1001) docker     (122)   173785 2023-07-31 16:17:48.000000 rcsbsearchapi-1.3.0/rcsbsearchapi/resources/chemical_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (122)  1290883 2023-07-31 16:17:48.000000 rcsbsearchapi-1.3.0/rcsbsearchapi/resources/metadata_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (122)     5766 2023-07-31 16:17:48.000000 rcsbsearchapi-1.3.0/rcsbsearchapi/schema.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    41394 2023-07-31 16:17:48.000000 rcsbsearchapi-1.3.0/rcsbsearchapi/search.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      568 2023-07-31 16:17:48.000000 rcsbsearchapi-1.3.0/rcsbsearchapi/update_schema.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-31 16:18:51.334364 rcsbsearchapi-1.3.0/rcsbsearchapi.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    15684 2023-07-31 16:18:51.000000 rcsbsearchapi-1.3.0/rcsbsearchapi.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      543 2023-07-31 16:18:51.000000 rcsbsearchapi-1.3.0/rcsbsearchapi.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-31 16:18:51.000000 rcsbsearchapi-1.3.0/rcsbsearchapi.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-31 16:18:06.000000 rcsbsearchapi-1.3.0/rcsbsearchapi.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      165 2023-07-31 16:18:51.000000 rcsbsearchapi-1.3.0/rcsbsearchapi.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       14 2023-07-31 16:18:51.000000 rcsbsearchapi-1.3.0/rcsbsearchapi.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       23 2023-07-31 16:17:48.000000 rcsbsearchapi-1.3.0/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-07-31 16:18:51.338364 rcsbsearchapi-1.3.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     2572 2023-07-31 16:17:48.000000 rcsbsearchapi-1.3.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-31 16:18:51.334364 rcsbsearchapi-1.3.0/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2881 2023-07-31 16:17:48.000000 rcsbsearchapi-1.3.0/tests/testschema.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    33669 2023-07-31 16:17:48.000000 rcsbsearchapi-1.3.0/tests/testsearch.py
```

### Comparing `rcsbsearchapi-1.2.0/LICENSE` & `rcsbsearchapi-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsbsearchapi-1.2.0/PKG-INFO` & `rcsbsearchapi-1.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsbsearchapi
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python package interface for the RCSB PDB search API service
 Home-page: https://github.com/rcsb/py-rcsbsearchapi
 Author: Dennis Piehl
 Author-email: dennis.piehl@rcsb.org
 License: BSD 3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -240,26 +240,73 @@
 
 # RNA query: 6C RNA motif
 rna = SeqMotifQuery("CCCCCC", sequence_type="rna")
 print("RNA results:")
 for polyid in rna("polymer_entity"):
     print(polyid)
 ```
+### Structure Similarity Query Example
+
+The PDB archive can be queried using the 3D shape of a protein structure. To perform this query, 3D protein structure data must be provided as an input or parameter, A chain ID or assembly ID must be specified, whether the input structure data should be compared to Assemblies or Polymer Entity Instance (Chains) is required, and defining the search type as either strict or relaxed is required. More information on how Structure Similarity Queries work can be found on the [RCSB PDB Structure Similarity Search](https://www.rcsb.org/docs/search-and-browse/advanced-search/structure-similarity-search) page.
+```python
+from rcsbsearchapi.search import StructSimilarityQuery
+
+# Basic query: querying using entry ID and default values assembly ID "1", operator "strict", and target search space "Assemblies"
+q1 = StructSimilarityQuery(value="4HHB")
+
+# Same example but with parameters explicitly specified
+q1 = StructSimilarityQuery(structure_search_type="entry_id",
+                           value="4HHB",
+                           input_structure_type="assembly_id",
+                           input_option="1",
+                           operator="strict_shape_match",
+                           target_search_space="assembly"
+                           )
+for id in q1("assembly"):
+    print(id)
+```
+Below is a more complex example that utilizes chain ID, relaxed search operator, and polymer entity instance or target search space. Specifying whether the input structure
+type is chain id or assembly id is very important. For example, specifying chain ID as the input structure type but inputting an assembly ID can lead to
+an error.
+```python
+from rcsbsearchapi.search import StructSimilarityQuery
+
+# More complex query with entry ID value "4HHB", chain ID "B", operator "relaxed", and target search space "Chains"
+q2 = StructSimilarityQuery(structure_search_type="entry_id",
+                                   value="4HHB",
+                                   input_structure_type="chain_id",
+                                   input_option="B",
+                                   operator="relaxed_shape_match",
+                                   target_search_space="polymer_entity_instance")
+list(q2())
+```
+Structure similarity queries also allow users to upload a file from their local computer or input a file url from the website to query the PDB archive for similar proteins. The file represents a target protein structure in the file formats "cif", "bcif", "pdb", "cif.gz", or "pdb.gz". If a user wants to use a file url for queries, the user must specify the structure search type, the value (being the url), and the file format of the file. This is also the same case for file upload, except the value is the absolute path leading to the file that is in the local machine. An example for file url is below for 4HHB (hemoglobin).
+```python
+from rcsbsearchapi.search import StructSimilarityQuery
+
+q3 = StructSimilarityQuery("file_url", "https://files.rcsb.org/view/4HHB.cif", input_option="cif")
+
+# If using file upload, an example query would be like below:
+# q3 = StructSimilarityQuery("file_upload", "/absolute/path/to/file.cif", input_option="file format")
+
+list(q3())
+```
+
 ## Supported Features
 
 The following table lists the status of current and planned features.
 
 - [x] Structure and chemical attribute search
   - [x] Attribute Comparison operations
   - [x] Query set operations
   - [x] Attribute `contains`, `in_` (fluent only)
 - [x] Option to include computed structure models (CSMs) in search
 - [x] Sequence search
 - [x] Sequence motif search
-- [ ] Structural search
+- [x] Structure similarity search
 - [ ] Structural motif search
 - [ ] Chemical search
 - [ ] Rich results using the Data API
 
 Contributions are welcome for unchecked items!
 
 ## Installation
```

### Comparing `rcsbsearchapi-1.2.0/README.md` & `rcsbsearchapi-1.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -214,26 +214,73 @@
 
 # RNA query: 6C RNA motif
 rna = SeqMotifQuery("CCCCCC", sequence_type="rna")
 print("RNA results:")
 for polyid in rna("polymer_entity"):
     print(polyid)
 ```
+### Structure Similarity Query Example
+
+The PDB archive can be queried using the 3D shape of a protein structure. To perform this query, 3D protein structure data must be provided as an input or parameter, A chain ID or assembly ID must be specified, whether the input structure data should be compared to Assemblies or Polymer Entity Instance (Chains) is required, and defining the search type as either strict or relaxed is required. More information on how Structure Similarity Queries work can be found on the [RCSB PDB Structure Similarity Search](https://www.rcsb.org/docs/search-and-browse/advanced-search/structure-similarity-search) page.
+```python
+from rcsbsearchapi.search import StructSimilarityQuery
+
+# Basic query: querying using entry ID and default values assembly ID "1", operator "strict", and target search space "Assemblies"
+q1 = StructSimilarityQuery(value="4HHB")
+
+# Same example but with parameters explicitly specified
+q1 = StructSimilarityQuery(structure_search_type="entry_id",
+                           value="4HHB",
+                           input_structure_type="assembly_id",
+                           input_option="1",
+                           operator="strict_shape_match",
+                           target_search_space="assembly"
+                           )
+for id in q1("assembly"):
+    print(id)
+```
+Below is a more complex example that utilizes chain ID, relaxed search operator, and polymer entity instance or target search space. Specifying whether the input structure
+type is chain id or assembly id is very important. For example, specifying chain ID as the input structure type but inputting an assembly ID can lead to
+an error.
+```python
+from rcsbsearchapi.search import StructSimilarityQuery
+
+# More complex query with entry ID value "4HHB", chain ID "B", operator "relaxed", and target search space "Chains"
+q2 = StructSimilarityQuery(structure_search_type="entry_id",
+                                   value="4HHB",
+                                   input_structure_type="chain_id",
+                                   input_option="B",
+                                   operator="relaxed_shape_match",
+                                   target_search_space="polymer_entity_instance")
+list(q2())
+```
+Structure similarity queries also allow users to upload a file from their local computer or input a file url from the website to query the PDB archive for similar proteins. The file represents a target protein structure in the file formats "cif", "bcif", "pdb", "cif.gz", or "pdb.gz". If a user wants to use a file url for queries, the user must specify the structure search type, the value (being the url), and the file format of the file. This is also the same case for file upload, except the value is the absolute path leading to the file that is in the local machine. An example for file url is below for 4HHB (hemoglobin).
+```python
+from rcsbsearchapi.search import StructSimilarityQuery
+
+q3 = StructSimilarityQuery("file_url", "https://files.rcsb.org/view/4HHB.cif", input_option="cif")
+
+# If using file upload, an example query would be like below:
+# q3 = StructSimilarityQuery("file_upload", "/absolute/path/to/file.cif", input_option="file format")
+
+list(q3())
+```
+
 ## Supported Features
 
 The following table lists the status of current and planned features.
 
 - [x] Structure and chemical attribute search
   - [x] Attribute Comparison operations
   - [x] Query set operations
   - [x] Attribute `contains`, `in_` (fluent only)
 - [x] Option to include computed structure models (CSMs) in search
 - [x] Sequence search
 - [x] Sequence motif search
-- [ ] Structural search
+- [x] Structure similarity search
 - [ ] Structural motif search
 - [ ] Chemical search
 - [ ] Rich results using the Data API
 
 Contributions are welcome for unchecked items!
 
 ## Installation
```

### Comparing `rcsbsearchapi-1.2.0/rcsbsearchapi/__init__.py` & `rcsbsearchapi-1.3.0/rcsbsearchapi/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """RCSB PDB Search API"""
 from typing import TYPE_CHECKING, Any, List
 
 from .search import Terminal  # noqa: F401
 from .search import Attr, Group, Query, Session, TextQuery, Value
 
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 
 
 # loading rcsb_attributes can cause errors, so load it lazily
 if TYPE_CHECKING:
     from .schema import SchemaGroup
```

### Comparing `rcsbsearchapi-1.2.0/rcsbsearchapi/const.py` & `rcsbsearchapi-1.3.0/rcsbsearchapi/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,10 +6,13 @@
 SEARCH_SCHEMA_URL = "https://search.rcsb.org/schema/search/request/json-schema-rcsb_search_query.json"
 SEARCH_OPENAPI_SCHEMA_URL = "https://search.rcsb.org/openapi.json"
 STRUCTURE_ATTRIBUTE_SEARCH_SERVICE = "text"
 CHEMICAL_ATTRIBUTE_SEARCH_SERVICE = "text_chem"
 FULL_TEXT_SEARCH_SERVICE = "full_text"
 SEQUENCE_SEARCH_SERVICE = "sequence"
 SEQMOTIF_SEARCH_SERVICE = "seqmotif"
+STRUCT_SIM_SEARCH_SERVICE = "structure"
 SEQUENCE_SEARCH_MIN_NUM_OF_RESIDUES = 25
 SEQMOTIF_SEARCH_MIN_CHARACTERS = 2
 RCSB_SEARCH_API_QUERY_URL = "https://search.rcsb.org/rcsbsearch/v2/query"
+UPLOAD_URL = "https://user-upload.rcsb.org/v1/putMultipart"
+RETURN_UP_URL = "https://user-upload.rcsb.org/v1/download/"
```

### Comparing `rcsbsearchapi-1.2.0/rcsbsearchapi/resources/chemical_schema.json` & `rcsbsearchapi-1.3.0/rcsbsearchapi/resources/chemical_schema.json`

 * *Files identical despite different names*

### Comparing `rcsbsearchapi-1.2.0/rcsbsearchapi/resources/metadata_schema.json` & `rcsbsearchapi-1.3.0/rcsbsearchapi/resources/metadata_schema.json`

 * *Files identical despite different names*

### Comparing `rcsbsearchapi-1.2.0/rcsbsearchapi/schema.py` & `rcsbsearchapi-1.3.0/rcsbsearchapi/schema.py`

 * *Files identical despite different names*

### Comparing `rcsbsearchapi-1.2.0/rcsbsearchapi/search.py` & `rcsbsearchapi-1.3.0/rcsbsearchapi/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,29 +25,33 @@
     TypeVar,
     Union,
     overload,
 )
 
 import requests
 from .const import STRUCTURE_ATTRIBUTE_SEARCH_SERVICE, REQUESTS_PER_SECOND, FULL_TEXT_SEARCH_SERVICE, SEQUENCE_SEARCH_SERVICE, SEQUENCE_SEARCH_MIN_NUM_OF_RESIDUES
-from .const import RCSB_SEARCH_API_QUERY_URL, SEQMOTIF_SEARCH_SERVICE, SEQMOTIF_SEARCH_MIN_CHARACTERS
+from .const import RCSB_SEARCH_API_QUERY_URL, SEQMOTIF_SEARCH_SERVICE, SEQMOTIF_SEARCH_MIN_CHARACTERS, UPLOAD_URL, RETURN_UP_URL, STRUCT_SIM_SEARCH_SERVICE
 
 if sys.version_info > (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 # tqdm is optional
 # Allowed return types for searches. https://search.rcsb.org/#return-type
 ReturnType = Literal[
     "entry", "assembly", "polymer_entity", "non_polymer_entity", "polymer_instance",
     "mol_definition"
 ]
 ReturnContentType = Literal["experimental", "computational"]  # results_content_type parameter list values
 SequenceType = Literal["dna", "rna", "protein"]  # possible sequence types for sequence searching
 SeqMode = Literal["simple", "prosite", "regex"]  # possible sequence motif formats
+StructSimEntryType = Literal["entry_id", "file_url", "file_upload"]  # possible entry types for structure similarity search
+StructSimInputType = Literal["assembly_id", "chain_id"]  # Possible ID choices for structure similarity search
+StructSimSearchSpace = Literal["polymer_entity_instance", "assembly"]  # target search spaces for structure similarity search
+StructSimOperator = Literal["strict_shape_match", "relaxed_shape_match"]  # possible operators for structure similarity search
 TAndOr = Literal["and", "or"]
 # All valid types for Terminal values
 TValue = Union[
     str,
     int,
     float,
     date,
@@ -61,14 +65,28 @@
     Tuple[date, ...],
     Dict[str, Any],
 ]
 # Types valid for numeric operators
 TNumberLike = Union[int, float, date, "Value[int]", "Value[float]", "Value[date]"]
 
 
+def fileUpload(filepath: str, fmt: str = "cif") -> str:
+    """Take a file given by a filepath, and return the
+    corresponding URL to use in a structure search. This URL
+    should then be passed through as part of the value parameter,
+    along with the format of the file. """
+    x = open(filepath, mode='rb')
+    res = requests.post(UPLOAD_URL, files={"file": x, "format": fmt}, timeout=None)
+    try:
+        spec = res.json()["key"]
+    except KeyError:
+        raise TypeError("There was an issue processing the file. Check the file format.")
+    return RETURN_UP_URL + spec
+
+
 class Query(ABC):
     """Base class for all types of queries.
 
     Queries can be combined using set operators:
 
     - `q1 & q2`: Intersection (AND)
     - `q1 | q2`: Union (OR)
@@ -275,18 +293,23 @@
         Args:
             attribute: specify attribute for search (i.e struct.title, exptl.method, rcsb_id)
             operator: specify operation to be done for search (i.e "contains_phrase", "exact_match")
             value: text query
             service: specify what search service (i.e "text", "text_chem")
             negation: logical not
         """
-        super().__init__(params={"attribute": attribute,
-                                 "operator": operator,
-                                 "negation": negation,
-                                 "value": value}, service=service)
+        if value is not None:
+            super().__init__(params={"attribute": attribute,
+                                     "operator": operator,
+                                     "negation": negation,
+                                     "value": value}, service=service)
+        else:
+            super().__init__(params={"attribute": attribute,
+                                     "operator": operator,
+                                     "negation": negation}, service=service)
 
 
 class TextQuery(Terminal):
     """Special case of a Terminal for free-text queries"""
 
     def __init__(self, value: str):
         """Search for the string value anywhere in the text
@@ -318,25 +341,74 @@
                                                                       "identity_cutoff": identity_cutoff,
                                                                       "sequence_type": sequence_type,
                                                                       "value": value
                                                                       })
 
 
 class SeqMotifQuery(Terminal):
-    """Special case of a terminal for protein, DNA, or RNA sequence queries"""
+    """Special case of a terminal for protein, DNA, or RNA sequence motif queries"""
 
     def __init__(self, value: str, pattern_type: Optional[SeqMode] = "simple", sequence_type: Optional[SequenceType] = "protein"):
         if len(value) < SEQMOTIF_SEARCH_MIN_CHARACTERS:
             raise ValueError("The sequence motif must contain at least 2 characters")
         else:
             super().__init__(service=SEQMOTIF_SEARCH_SERVICE, params={"value": value,
                                                                       "pattern_type": pattern_type,
                                                                       "sequence_type": sequence_type})
 
 
+class StructSimilarityQuery(Terminal):
+    """Special case of a terminal for structure similarity queries"""
+
+    def __init__(self, structure_search_type: StructSimEntryType = "entry_id",
+                 value: Optional[str] = None,
+                 input_structure_type: Optional[StructSimInputType] = "assembly_id",
+                 input_option: str = "1",
+                 operator: StructSimOperator = "strict_shape_match",
+                 target_search_space: StructSimSearchSpace = "assembly"
+                 ):
+        if structure_search_type == "entry_id":
+            if input_structure_type == "assembly_id":
+                super().__init__(service=STRUCT_SIM_SEARCH_SERVICE, params={
+                    "operator": operator,
+                    "target_search_space": target_search_space,
+                    "value": {
+                        "entry_id": value,
+                        "assembly_id": input_option
+                    }
+                })
+            elif input_structure_type == "chain_id":
+                super().__init__(service=STRUCT_SIM_SEARCH_SERVICE, params={
+                    "operator": operator,
+                    "target_search_space": target_search_space,
+                    "value": {
+                        "entry_id": value,
+                        "asym_id": input_option
+                    }
+                })
+        elif structure_search_type == "file_url":
+            super().__init__(service=STRUCT_SIM_SEARCH_SERVICE, params={
+                "operator": operator,
+                "target_search_space": target_search_space,
+                "value": {
+                    "url": value,
+                    "format": input_option
+                }
+            })
+        elif structure_search_type == "file_upload":
+            super().__init__(service=STRUCT_SIM_SEARCH_SERVICE, params={
+                "operator": operator,
+                "target_search_space": target_search_space,
+                "value": {
+                    "url": fileUpload(value, input_option),
+                    "format": "bcif"
+                }
+            })
+
+
 @dataclass(frozen=True)
 class Group(Query):
     """AND and OR combinations of queries"""
 
     operator: TAndOr
     nodes: Iterable[Query] = ()
```

### Comparing `rcsbsearchapi-1.2.0/rcsbsearchapi/update_schema.py` & `rcsbsearchapi-1.3.0/rcsbsearchapi/update_schema.py`

 * *Files identical despite different names*

### Comparing `rcsbsearchapi-1.2.0/rcsbsearchapi.egg-info/PKG-INFO` & `rcsbsearchapi-1.3.0/rcsbsearchapi.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsbsearchapi
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python package interface for the RCSB PDB search API service
 Home-page: https://github.com/rcsb/py-rcsbsearchapi
 Author: Dennis Piehl
 Author-email: dennis.piehl@rcsb.org
 License: BSD 3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -240,26 +240,73 @@
 
 # RNA query: 6C RNA motif
 rna = SeqMotifQuery("CCCCCC", sequence_type="rna")
 print("RNA results:")
 for polyid in rna("polymer_entity"):
     print(polyid)
 ```
+### Structure Similarity Query Example
+
+The PDB archive can be queried using the 3D shape of a protein structure. To perform this query, 3D protein structure data must be provided as an input or parameter, A chain ID or assembly ID must be specified, whether the input structure data should be compared to Assemblies or Polymer Entity Instance (Chains) is required, and defining the search type as either strict or relaxed is required. More information on how Structure Similarity Queries work can be found on the [RCSB PDB Structure Similarity Search](https://www.rcsb.org/docs/search-and-browse/advanced-search/structure-similarity-search) page.
+```python
+from rcsbsearchapi.search import StructSimilarityQuery
+
+# Basic query: querying using entry ID and default values assembly ID "1", operator "strict", and target search space "Assemblies"
+q1 = StructSimilarityQuery(value="4HHB")
+
+# Same example but with parameters explicitly specified
+q1 = StructSimilarityQuery(structure_search_type="entry_id",
+                           value="4HHB",
+                           input_structure_type="assembly_id",
+                           input_option="1",
+                           operator="strict_shape_match",
+                           target_search_space="assembly"
+                           )
+for id in q1("assembly"):
+    print(id)
+```
+Below is a more complex example that utilizes chain ID, relaxed search operator, and polymer entity instance or target search space. Specifying whether the input structure
+type is chain id or assembly id is very important. For example, specifying chain ID as the input structure type but inputting an assembly ID can lead to
+an error.
+```python
+from rcsbsearchapi.search import StructSimilarityQuery
+
+# More complex query with entry ID value "4HHB", chain ID "B", operator "relaxed", and target search space "Chains"
+q2 = StructSimilarityQuery(structure_search_type="entry_id",
+                                   value="4HHB",
+                                   input_structure_type="chain_id",
+                                   input_option="B",
+                                   operator="relaxed_shape_match",
+                                   target_search_space="polymer_entity_instance")
+list(q2())
+```
+Structure similarity queries also allow users to upload a file from their local computer or input a file url from the website to query the PDB archive for similar proteins. The file represents a target protein structure in the file formats "cif", "bcif", "pdb", "cif.gz", or "pdb.gz". If a user wants to use a file url for queries, the user must specify the structure search type, the value (being the url), and the file format of the file. This is also the same case for file upload, except the value is the absolute path leading to the file that is in the local machine. An example for file url is below for 4HHB (hemoglobin).
+```python
+from rcsbsearchapi.search import StructSimilarityQuery
+
+q3 = StructSimilarityQuery("file_url", "https://files.rcsb.org/view/4HHB.cif", input_option="cif")
+
+# If using file upload, an example query would be like below:
+# q3 = StructSimilarityQuery("file_upload", "/absolute/path/to/file.cif", input_option="file format")
+
+list(q3())
+```
+
 ## Supported Features
 
 The following table lists the status of current and planned features.
 
 - [x] Structure and chemical attribute search
   - [x] Attribute Comparison operations
   - [x] Query set operations
   - [x] Attribute `contains`, `in_` (fluent only)
 - [x] Option to include computed structure models (CSMs) in search
 - [x] Sequence search
 - [x] Sequence motif search
-- [ ] Structural search
+- [x] Structure similarity search
 - [ ] Structural motif search
 - [ ] Chemical search
 - [ ] Rich results using the Data API
 
 Contributions are welcome for unchecked items!
 
 ## Installation
```

### Comparing `rcsbsearchapi-1.2.0/rcsbsearchapi.egg-info/SOURCES.txt` & `rcsbsearchapi-1.3.0/rcsbsearchapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsbsearchapi-1.2.0/setup.py` & `rcsbsearchapi-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `rcsbsearchapi-1.2.0/tests/testschema.py` & `rcsbsearchapi-1.3.0/tests/testschema.py`

 * *Files identical despite different names*

### Comparing `rcsbsearchapi-1.2.0/tests/testsearch.py` & `rcsbsearchapi-1.3.0/tests/testsearch.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,31 +18,41 @@
 __license__ = "BSD 3-Clause"
 
 import logging
 import platform
 import resource
 import time
 import unittest
+import os
 from itertools import islice
 import requests
-from rcsbsearchapi.const import CHEMICAL_ATTRIBUTE_SEARCH_SERVICE, STRUCTURE_ATTRIBUTE_SEARCH_SERVICE
+from rcsbsearchapi.const import CHEMICAL_ATTRIBUTE_SEARCH_SERVICE, STRUCTURE_ATTRIBUTE_SEARCH_SERVICE, RETURN_UP_URL
 from rcsbsearchapi import Attr, Group, Session, TextQuery, Value
 from rcsbsearchapi import rcsb_attributes as attrs
-from rcsbsearchapi.search import PartialQuery, Terminal, AttributeQuery, SequenceQuery, SeqMotifQuery
+from rcsbsearchapi.search import PartialQuery, Terminal, AttributeQuery, SequenceQuery, SeqMotifQuery, StructSimilarityQuery, fileUpload
 
 
 logging.basicConfig(level=logging.INFO, format="%(asctime)s [%(levelname)s]-%(module)s.%(funcName)s: %(message)s")
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 
 
 class SearchTests(unittest.TestCase):
     def setUp(self):
         self.__startTime = time.time()
         logger.info("Starting %s at %s", self.id(), time.strftime("%Y %m %d %H:%M:%S", time.localtime()))
+        HERE = os.path.abspath(os.path.dirname(__file__))
+        self.__dirPath = os.path.join(HERE, "files")
+        self.__4hhbBcif = os.path.join(self.__dirPath, "4hhb.bcif")
+        self.__4hhbCif = os.path.join(self.__dirPath, "4hhb.cif")
+        self.__4hhbPdb = os.path.join(self.__dirPath, "4hhb.pdb")
+        self.__7n0rPdbGz = os.path.join(self.__dirPath, "7n0r.pdb.gz")
+        self.__7n0rCifGz = os.path.join(self.__dirPath, "7n0r.cif.gz")
+        self.__invalidTxt = os.path.join(self.__dirPath, "invalid.txt")
+        self.__4hhbAssembly1 = os.path.join(self.__dirPath, "4hhb-assembly1.cif.gz")
 
     def tearDown(self):
         unitS = "MB" if platform.system() == "Darwin" else "GB"
         rusageMax = resource.getrusage(resource.RUSAGE_SELF).ru_maxrss
         logger.info("Maximum resident memory size %.4f %s", rusageMax / 10 ** 6, unitS)
         endTime = time.time()
         logger.info("Completed %s at %s (%.4f seconds)", self.id(), time.strftime("%Y %m %d %H:%M:%S", time.localtime()), endTime - self.__startTime)
@@ -548,14 +558,182 @@
             q1 = SeqMotifQuery("AAAA", "nothing", "nothing")  # this should fail
             _ = list(q1())
         except requests.exceptions.HTTPError:
             ok = True
         self.assertTrue(ok)
         logger.info("SeqMotif Query with invalid parameters failed successfully: (%r)", ok)
 
+    def testFileUpload(self):
+        """Test uploading a file. Used for structure queries.
+        As a unique URL is generated each time, the only common
+        denominator is that the return URL contains the file
+        name at the end of it, and that the first part of the
+        URL is the same."""
+
+        hemo = self.__4hhbCif
+        x = fileUpload(hemo)
+        ok = (x[x.rfind("/") + 1:]) == "4hhb.bcif"  # check that end of file name is 4hhb.cif
+        self.assertTrue(ok)
+        logger.info(".cif File Upload check one: (%r)", ok)
+
+        ok = RETURN_UP_URL in x  # check that beginning of URL is formed correctly. This is admittedly rather redundant.
+        self.assertTrue(ok)
+        logger.info(".cif File Upload check two: (%r)", ok)
+
+        zipfile = self.__7n0rCifGz  # gz files should also work by default
+        x = fileUpload(zipfile)
+        ok = (x[x.rfind("/") + 1:]) == "7n0r.bcif"
+        self.assertTrue(ok)
+        logger.info(".cif.gz File Upload check one: (%r)", ok)
+
+        ok = RETURN_UP_URL in x
+        self.assertTrue(ok)
+        logger.info(".cif.gz File Upload check two: (%r)", ok)
+
+        pdbfile = self.__4hhbPdb
+        x = fileUpload(pdbfile, "pdb")  # for non-cif files provide file extension
+        ok = (x[x.rfind("/") + 1:]) == "4hhb.bcif"  # check that end of file name is 4hhb.bcif
+        self.assertTrue(ok)
+        logger.info(".pdb File Upload check one: (%r)", ok)
+
+        ok = RETURN_UP_URL in x
+        self.assertTrue(ok)
+        logger.info(".pdb File Upload check two: (%r)", ok)
+
+        zippdb = self.__7n0rPdbGz  # PDB Zip files should work as well.
+        x = fileUpload(zippdb, "pdb")
+        ok = (x[x.rfind("/") + 1:]) == "7n0r.bcif"
+        self.assertTrue(ok)
+        logger.info(".pdb.gz File Upload check one: (%r)", ok)
+
+        ok = RETURN_UP_URL in x
+        self.assertTrue(ok)
+        logger.info(".pdb.gz File Upload check two: (%r)", ok)
+
+        hemobcif = self.__4hhbBcif
+        x = fileUpload(hemobcif, "bcif")  # must specify that file you are providing is bcif
+        ok = (x[x.rfind("/") + 1:]) == "4hhb.bcif"  # check that end of file name is 4hhb.bcif
+        self.assertTrue(ok)
+        logger.info(".bcif File Upload check one: (%r)", ok)
+
+        ok = RETURN_UP_URL in x  # check that beginning of URL is formed correctly.
+        self.assertTrue(ok)
+        logger.info(".bcif File Upload check two: (%r)", ok)
+
+        hemoAssem = self.__4hhbAssembly1
+        x = fileUpload(hemoAssem)
+        ok = (x[x.rfind("/") + 1:]) == "4hhb-assembly1.bcif"
+        self.assertTrue(ok)
+        logger.info(".cif.gz Assembly File Upload check one: (%r)", ok)
+
+        ok = RETURN_UP_URL in x  # check that beginning of URL is formed correctly.
+        self.assertTrue(ok)
+        logger.info(".cif.gz Assembly File Upload check two: (%r)", ok)
+
+        # test error handling
+
+        invalid = self.__invalidTxt
+        ok = False
+        try:
+            _ = fileUpload(invalid, "bcif")
+        except TypeError:
+            ok = True
+        self.assertTrue(ok)
+        logger.info("invalid query failed successfully: (%r)", ok)
+
+    def testStructSimQuery(self):
+        """Test firing off a structure similarity query"""
+        # Basic query - assembly ID
+        q1 = StructSimilarityQuery(value="4HHB")
+        result = list(q1())
+        ok = len(result) > 0
+        self.assertTrue(ok)
+        logger.info("Basic Structure Similarity query results: result length : (%d), ok : (%r)", len(result), ok)
+
+        # Query with chain ID
+        q2 = StructSimilarityQuery("entry_id", "4HHB", "chain_id", "A", target_search_space="polymer_entity_instance")
+        result = list(q2())
+        ok = len(result) > 0
+        self.assertTrue(ok)
+        logger.info("Query with chain ID results: result length : (%d), ok : (%r)", len(result), ok)
+
+        # Query with file url
+        q3 = StructSimilarityQuery("file_url", "https://files.rcsb.org/view/4HHB.cif", input_option="cif")
+        result = list(q3())
+        ok = len(result) > 0
+        self.assertTrue(ok)
+        logger.info("Query with file url results: result length : (%d), ok : (%r)", len(result), ok)
+
+        # Query with file upload
+        q4 = StructSimilarityQuery("file_upload", self.__4hhbCif, input_option="cif")
+        result = list(q4())
+        ok = len(result) > 0
+        self.assertTrue(ok)
+        logger.info("Query with file upload results: result length : (%d), ok : (%r)", len(result), ok)
+
+        # Query with relaxed operator
+        q5 = StructSimilarityQuery("entry_id", "4HHB", operator="relaxed_shape_match")
+        result = list(q5())
+        ok = len(result) > 0
+        self.assertTrue(ok)
+        logger.info("Query with relaxed operator results: result length : (%d), ok : (%r)", len(result), ok)
+
+        # Query with specifically polymer entity instance search space
+        q6 = StructSimilarityQuery(structure_search_type="entry_id",
+                                   value="4HHB",
+                                   input_structure_type="chain_id",
+                                   input_option="B",
+                                   operator="relaxed_shape_match",
+                                   target_search_space="polymer_entity_instance")
+        result = list(q6())
+        ok = len(result) > 0
+        self.assertTrue(ok)
+        logger.info("Query with polymer entity instance results: result length : (%d), ok : (%r)", len(result), ok)
+
+        # File upload query using 4HHB Assembly 1 - cif zip file
+        q7 = StructSimilarityQuery("file_upload", self.__4hhbAssembly1, input_option="cif")
+        result = list(q7())
+        ok = len(result) > 0
+        self.assertTrue(ok)
+        logger.info("File upload query using 4HHB Assembly 1 cif zip file results : (%d), ok : (%r)", len(result), ok)
+
+        # File upload query using 4HHB PDB file
+        q8 = StructSimilarityQuery("file_upload", self.__4hhbPdb, input_option="pdb")
+        result = list(q8())
+        ok = len(result) > 0
+        self.assertTrue(ok)
+        logger.info("File upload query using 4HHB PDB file results: result length : (%d), ok : (%r)", len(result), ok)
+
+        # File upload query using 4HHB bcif file
+        q9 = StructSimilarityQuery("file_upload", self.__4hhbBcif, input_option="bcif")
+        result = list(q9())
+        ok = len(result) > 0
+        self.assertTrue(ok)
+        logger.info("File upload query using 4HHB bcif file results: result length : (%d), ok : (%r)", len(result), ok)
+
+        # File url query with mmcif file format, relaxed operator, and chains target search space
+        q10 = StructSimilarityQuery("file_url", "https://files.rcsb.org/view/4HHB.cif",
+                                    input_option="cif",
+                                    operator="relaxed_shape_match",
+                                    target_search_space="polymer_entity_instance")
+        result = list(q10())
+        ok = len(result) > 0
+        self.assertTrue(ok)
+        logger.info("File url query using mmcif file format, relaxed, and chains: result length : (%d), ok : (%r)", len(result), ok)
+
+        # File url query with wrong combination of fire url and format (should fail)
+        ok = False
+        try:
+            q11 = StructSimilarityQuery("file_url", "https://files.rcsb.org/view/4HHB.cif", input_option="pdb")
+            result = list(q11())
+        except requests.HTTPError:
+            ok = True
+        self.assertTrue(ok)
+        logger.info("File url query with wrong file format failed successfully : (%r)", ok)
+
 
 def buildSearch():
     suiteSelect = unittest.TestSuite()
     suiteSelect.addTest(SearchTests("testConstruction"))
     suiteSelect.addTest(SearchTests("testLargePagination"))
     suiteSelect.addTest(SearchTests("testOperators"))
     suiteSelect.addTest(SearchTests("testPartialQuery"))
@@ -571,13 +749,15 @@
     suiteSelect.addTest(SearchTests("testIquery"))
     suiteSelect.addTest(SearchTests("testSingleQuery"))
     suiteSelect.addTest(SearchTests("testChemSearch"))
     suiteSelect.addTest(SearchTests("testMismatch"))
     suiteSelect.addTest(SearchTests("testCSMquery"))
     suiteSelect.addTest(SearchTests("testSequenceQuery"))
     suiteSelect.addTest(SearchTests("testSeqMotifQuery"))
+    suiteSelect.addTest(SearchTests("testFileUpload"))
+    suiteSelect.addTest(SearchTests("testStructSimQuery"))
     return suiteSelect
 
 
 if __name__ == "__main__":
     mySuite = buildSearch()
     unittest.TextTestRunner(verbosity=2).run(mySuite)
```

