# Comparing `tmp/aidriver-0.1.tar.gz` & `tmp/aidriver-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aidriver-0.1.tar", last modified: Sun Jul 30 13:37:27 2023, max compression
+gzip compressed data, was "aidriver-0.1.1.tar", last modified: Mon Jul 31 21:33:28 2023, max compression
```

## Comparing `aidriver-0.1.tar` & `aidriver-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,43 @@
-drwxr-xr-x   0 jphillips  (1000) jphillips  (1000)        0 2023-07-30 13:37:27.740042 aidriver-0.1/
--rw-r--r--   0 jphillips  (1000) jphillips  (1000)      304 2023-07-30 12:25:48.000000 aidriver-0.1/.envtemplate
--rw-r--r--   0 jphillips  (1000) jphillips  (1000)      727 2023-07-30 12:47:26.000000 aidriver-0.1/Dockerfile
--rw-r--r--   0 jphillips  (1000) jphillips  (1000)      109 2023-07-30 13:37:27.740042 aidriver-0.1/PKG-INFO
-drwxr-xr-x   0 jphillips  (1000) jphillips  (1000)        0 2023-07-30 13:37:27.730041 aidriver-0.1/ai_driver/
--rw-r--r--   0 jphillips  (1000) jphillips  (1000)     4785 2023-07-30 13:06:32.000000 aidriver-0.1/ai_driver/main.py
-drwxr-xr-x   0 jphillips  (1000) jphillips  (1000)        0 2023-07-30 13:37:27.730041 aidriver-0.1/ai_driver/tests/
-drwxr-xr-x   0 jphillips  (1000) jphillips  (1000)        0 2023-07-30 13:37:27.730041 aidriver-0.1/ai_driver/tests/test_data/
--rw-r--r--   0 jphillips  (1000) jphillips  (1000)  2869842 2023-07-30 12:27:38.000000 aidriver-0.1/ai_driver/tests/test_data/PlayerDnDBasicRules_v0.2_PrintFriendly.pdf
--rw-r--r--   0 jphillips  (1000) jphillips  (1000)     1048 2023-07-30 13:10:32.000000 aidriver-0.1/ai_driver/tests/test_main.py
-drwxr-xr-x   0 jphillips  (1000) jphillips  (1000)        0 2023-07-30 13:37:27.740042 aidriver-0.1/aidriver.egg-info/
--rw-r--r--   0 jphillips  (1000) jphillips  (1000)      109 2023-07-30 13:37:27.000000 aidriver-0.1/aidriver.egg-info/PKG-INFO
--rw-r--r--   0 jphillips  (1000) jphillips  (1000)      376 2023-07-30 13:37:27.000000 aidriver-0.1/aidriver.egg-info/SOURCES.txt
--rw-r--r--   0 jphillips  (1000) jphillips  (1000)        1 2023-07-30 13:37:27.000000 aidriver-0.1/aidriver.egg-info/dependency_links.txt
--rw-r--r--   0 jphillips  (1000) jphillips  (1000)      367 2023-07-30 13:37:27.000000 aidriver-0.1/aidriver.egg-info/requires.txt
--rw-r--r--   0 jphillips  (1000) jphillips  (1000)       10 2023-07-30 13:37:27.000000 aidriver-0.1/aidriver.egg-info/top_level.txt
-drwxr-xr-x   0 jphillips  (1000) jphillips  (1000)        0 2023-07-30 13:37:27.740042 aidriver-0.1/data/
--rw-r--r--   0 jphillips  (1000) jphillips  (1000)  2869842 2023-07-30 13:10:05.000000 aidriver-0.1/data/PlayerDnDBasicRules_v0.2_PrintFriendly.pdf
--rw-r--r--   0 jphillips  (1000) jphillips  (1000)      149 2023-07-30 12:48:55.000000 aidriver-0.1/data/README.md
--rw-r--r--   0 jphillips  (1000) jphillips  (1000)     1073 2023-07-30 13:01:41.000000 aidriver-0.1/pyproject.toml
--rw-r--r--   0 jphillips  (1000) jphillips  (1000)       38 2023-07-30 13:37:27.740042 aidriver-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:33:28.120289 aidriver-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-31 21:33:06.000000 aidriver-0.1.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-31 21:33:06.000000 aidriver-0.1.1/.envtemplate
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-31 21:33:06.000000 aidriver-0.1.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 21:33:28.120289 aidriver-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:33:28.112289 aidriver-0.1.1/ai_driver/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/instruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/langsmith_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:33:28.112289 aidriver-0.1.1/ai_driver/local_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/local_llm/ggml_llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/local_llm/ggml_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/local_llm/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/local_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/qa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:33:28.112289 aidriver-0.1.1/ai_driver/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/scripts/download_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/scripts/init_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:33:28.112289 aidriver-0.1.1/ai_driver/scripts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/scripts/tests/test_download_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:33:28.112289 aidriver-0.1.1/ai_driver/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/tests/local_loader_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/tests/qa_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:33:28.112289 aidriver-0.1.1/ai_driver/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2869842 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/tests/test_data/PlayerDnDBasicRules_v0.2_PrintFriendly.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:33:28.116289 aidriver-0.1.1/ai_driver/vector_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/vector_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/vector_storage/faiss_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-31 21:33:06.000000 aidriver-0.1.1/ai_driver/vector_storage/pinecone_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:33:28.116289 aidriver-0.1.1/aidriver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 21:33:28.000000 aidriver-0.1.1/aidriver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-31 21:33:28.000000 aidriver-0.1.1/aidriver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:33:28.000000 aidriver-0.1.1/aidriver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-31 21:33:28.000000 aidriver-0.1.1/aidriver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 21:33:28.000000 aidriver-0.1.1/aidriver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:33:28.116289 aidriver-0.1.1/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-31 21:33:06.000000 aidriver-0.1.1/config/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:33:28.120289 aidriver-0.1.1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2869842 2023-07-31 21:33:06.000000 aidriver-0.1.1/data/PlayerDnDBasicRules_v0.2_PrintFriendly.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-31 21:33:06.000000 aidriver-0.1.1/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-31 21:33:06.000000 aidriver-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-31 21:33:28.120289 aidriver-0.1.1/setup.cfg
```

### Comparing `aidriver-0.1/ai_driver/tests/test_data/PlayerDnDBasicRules_v0.2_PrintFriendly.pdf` & `aidriver-0.1.1/ai_driver/tests/test_data/PlayerDnDBasicRules_v0.2_PrintFriendly.pdf`

 * *Files identical despite different names*

### Comparing `aidriver-0.1/ai_driver/tests/test_main.py` & `aidriver-0.1.1/ai_driver/tests/local_loader_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-from main import embed_FAISS_from_documents, load, split
+from ai_driver.local_loader import load, split
 import pytest
 import os
 import shutil
 
+
 @pytest.fixture
 def chunks():
     return load(os.path.join(os.path.dirname(__file__), "test_data"), "*.pdf")
-    
+
+
 def test_should_return_empty_list_for_empty_directory():
     empty_dir = os.path.join(os.path.dirname(__file__), "test_data", "empty_dir")
     os.makedirs(empty_dir, exist_ok=True)
     assert load(empty_dir, "*.pdf") == []
     shutil.rmtree(empty_dir)
 
+
 def test_should_return_empty_list_for_no_matching_files():
     assert load(os.path.join(os.path.dirname(__file__), "test_data"), "*.txt") == []
 
+
 def test_should_return_chunks_from_matching_files():
-    assert len(load(os.path.join(os.path.dirname(__file__), "test_data"), "*.pdf")) == 115
+    assert (
+        len(load(os.path.join(os.path.dirname(__file__), "test_data"), "*.pdf")) == 115
+    )
+
 
 def test_should_split_chunks_by_size_and_overlap(chunks):
     chunk_size = 342
     chunk_overlap = 200
 
     texts = split(chunks, chunk_size, chunk_overlap)
-    
+
     ### assert that chunks are not larger than expected
     for doc in texts:
         assert len(doc.page_content) <= chunk_size
-
```

### Comparing `aidriver-0.1/data/PlayerDnDBasicRules_v0.2_PrintFriendly.pdf` & `aidriver-0.1.1/data/PlayerDnDBasicRules_v0.2_PrintFriendly.pdf`

 * *Files identical despite different names*

### Comparing `aidriver-0.1/pyproject.toml` & `aidriver-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -5,52 +5,57 @@
   "setuptools-scm",
   "pytest",
 ]
 
 [project]
 description = "AIDriver"
 name = "aidriver"
-version = "0.1"
+version = "0.1.1"
 dependencies = [
     "requests",
   "python-dotenv",
   "pandas~=2.0.0",
-  "pyarrow==12.0.0",
+  "pyarrow~=12.0.0",
   "debugpy",
   "loguru",
   "httpx",
   "python-dotenv",
   "anyio",
   "openai",
   "faiss-cpu",
   "langchain",
   "langsmith",
   "pypdf",
   "InstructorEmbedding",
   "torch",
   "tdqm",
-  "transformers==4.20.0",
-  "datasets>=2.2.0",
+  "transformers",
+  "datasets",
   "jsonlines",
   "numpy",
-  "scikit_learn>=1.0.2",
+  "scikit_learn",
   "scipy",
-  "sentence_transformers>=2.2.0",
+  "sentence_transformers",
   "rich",
-  "PyPDF2"
+  "PyPDF2",
+  "pinecone-client[grpc]",
+  "python-box",
+  "ctransformers",
+  "uvicorn",
+  "fastapi"
 ]
 
 [tool.pytest.ini_options]
 pythonpath = [
   "ai_driver",
 ]
 
 [tool.setuptools.packages.find]
-include = ["ai_driver"]  # package names should match these glob patterns (["*"] by default)
-exclude = ["data"]  # exclude packages matching these glob patterns (empty by default)
+include = ["ai_driver", "ai_driver.*", "config"]  # package names should match these glob patterns (["*"] by default)
+exclude = ["data", "vectorstore", "artifacts"]  # exclude packages matching these glob patterns (empty by default)
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "trio",
     "pytest-httpx",
 ]
```

