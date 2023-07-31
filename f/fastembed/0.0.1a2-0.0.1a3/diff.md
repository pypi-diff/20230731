# Comparing `tmp/fastembed-0.0.1a2.tar.gz` & `tmp/fastembed-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastembed-0.0.1a2.tar", max compression
+gzip compressed data, was "fastembed-0.0.1a3.tar", max compression
```

## Comparing `fastembed-0.0.1a2.tar` & `fastembed-0.0.1a3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-07-14 05:55:44.593141 fastembed-0.0.1a2/LICENSE
--rw-r--r--   0        0        0     1376 2023-07-17 09:27:57.029707 fastembed-0.0.1a2/README.md
--rw-r--r--   0        0        0      882 2023-07-14 05:55:44.593496 fastembed-0.0.1a2/fastembed/embedding.py
--rw-r--r--   0        0        0      623 2023-07-17 09:28:52.510023 fastembed-0.0.1a2/fastembed/qdrant_client.py
--rw-r--r--   0        0        0     5787 2023-07-14 05:55:44.593784 fastembed-0.0.1a2/fastembed/qdrant_mixin.py
--rw-r--r--   0        0        0      965 2023-07-17 09:30:25.246186 fastembed-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0     2283 1970-01-01 00:00:00.000000 fastembed-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-14 05:55:44.593141 fastembed-0.0.1a3/LICENSE
+-rw-r--r--   0        0        0     1376 2023-07-17 09:27:57.029707 fastembed-0.0.1a3/README.md
+-rw-r--r--   0        0        0     8552 2023-07-31 11:11:50.584066 fastembed-0.0.1a3/fastembed/embedding.py
+-rw-r--r--   0        0        0      623 2023-07-17 09:28:52.510023 fastembed-0.0.1a3/fastembed/qdrant_client.py
+-rw-r--r--   0        0        0     5759 2023-07-31 10:50:29.497648 fastembed-0.0.1a3/fastembed/qdrant_mixin.py
+-rw-r--r--   0        0        0     1026 2023-07-31 11:17:57.302561 fastembed-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 fastembed-0.0.1a3/PKG-INFO
```

### Comparing `fastembed-0.0.1a2/LICENSE` & `fastembed-0.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastembed-0.0.1a2/README.md` & `fastembed-0.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `fastembed-0.0.1a2/fastembed/qdrant_client.py` & `fastembed-0.0.1a3/fastembed/qdrant_client.py`

 * *Files identical despite different names*

### Comparing `fastembed-0.0.1a2/fastembed/qdrant_mixin.py` & `fastembed-0.0.1a3/fastembed/qdrant_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import uuid
 from typing import Any, Dict, Generator, List, Optional
 
 from pydantic import BaseModel
 from qdrant_client.models import Distance, PointStruct, SearchParams, VectorParams
 
-from .embedding import Embedding, SentenceTransformersEmbedding
+from .embedding import DefaultEmbedding, Embedding
 
 
 class QueryResponse(BaseModel):
     ids: List[str]
     embeddings: Optional[List[List[float]]]
     metadatas: List[Dict[str, Any]]
     distances: List[float]
@@ -43,24 +43,24 @@
 
     def upsert_docs(
         self,
         collection_name: str,
         docs: Dict[str, List[Any]],
         batch_size: int = 512,
         wait: bool = True,
-        embedding_model: Embedding = SentenceTransformersEmbedding(),
+        embedding_model: Embedding = DefaultEmbedding(),
         **kwargs,
     ) -> None:
         """
         Args:
             collection_name (str): _description_
             docs (Dict[str, List[Any]]): _description_
             batch_size (int, optional): _description_. Defaults to 512.
             wait (bool, optional): _description_. Defaults to True.
-            embedding_model (Embedding, optional): Defaults to SentenceTransformersEmbedding.
+            embedding_model (Embedding, optional): Defaults to DefaultEmbedding() with all-MiniLM-L6-v2.
         """
 
         # Iterate over documents and metadatas in batches
         for batch_docs, batch_metadatas in zip(
             self.batch_iterable(docs["documents"], batch_size),
             self.batch_iterable(docs["metadatas"], batch_size),
         ):
@@ -86,15 +86,15 @@
         self,
         collection_name: str,
         query_texts: List[str],
         n_results: int = 2,
         batch_size: int = 512,
         query_filter: Optional[Dict[str, Any]] = None,
         search_params: SearchParams = SearchParams(hnsw_ef=128, exact=False),
-        embedding_model: Embedding = SentenceTransformersEmbedding(),
+        embedding_model: Embedding = DefaultEmbedding(),
         **kwargs,
     ) -> List[QueryResponse]:
         """
         Search for documents in a collection.
 
         Args:
             collection_name (str): _description_
```

### Comparing `fastembed-0.0.1a2/pyproject.toml` & `fastembed-0.0.1a3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [tool.poetry]
 name = "fastembed"
-version = "0.0.1.alpha2"
+version = "0.0.1.alpha3"
 description = "Fast embedding alternative to Sentence transformers"
 authors = ["NirantK <nirant.bits@gmail.com>"]
 license = "Apache License"
 readme = "README.md"
 packages = [{include = "fastembed"}]
 homepage = "https://github.com/qdrant/qdrant-client"
 repository = "https://github.com/qdrant/qdrant-client"
 keywords = ["vector", "embedding", "neural", "search", "qdrant"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<3.12"
 onnxruntime = "^1.15.1"
 sentence-transformers = "^2.2.2"
+tqdm = "^4.65.0"
+requests = "^2.31.0"
+tokenizers = "^0.13.3"
 
 [tool.poetry.dev-dependencies]
 ruff = "^0.0.277"
 isort = "^5.12.0"
 black = "^23.7.0"
 pre-commit = "^3.3.3"
```

### Comparing `fastembed-0.0.1a2/PKG-INFO` & `fastembed-0.0.1a3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastembed
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: Fast embedding alternative to Sentence transformers
 Home-page: https://github.com/qdrant/qdrant-client
 License: Apache License
 Keywords: vector,embedding,neural,search,qdrant
 Author: NirantK
 Author-email: nirant.bits@gmail.com
 Requires-Python: >=3.8.0,<3.12
@@ -12,15 +12,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: onnxruntime (>=1.15.1,<2.0.0)
 Requires-Dist: onnxruntime-silicon (>=1.15.0,<2.0.0) ; sys_platform == "darwin"
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
+Requires-Dist: tokenizers (>=0.13.3,<0.14.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/qdrant/qdrant-client
 Description-Content-Type: text/markdown
 
 # FastEmbed Library
 
 FastEmbed is a Python library that provides convenient methods for indexing and searching text documents using Qdrant, a high-dimensional vector indexing and search system.
```

