# Comparing `tmp/codechain-0.0.3.tar.gz` & `tmp/codechain-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codechain-0.0.3.tar", last modified: Thu Jul 27 12:40:46 2023, max compression
+gzip compressed data, was "codechain-0.0.4.tar", last modified: Mon Jul 31 17:31:26 2023, max compression
```

## Comparing `codechain-0.0.3.tar` & `codechain-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-27 12:40:46.519209 codechain-0.0.3/
--rw-r--r--   0 james      (501) staff       (20)     1587 2023-07-27 12:40:46.519078 codechain-0.0.3/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1011 2023-07-27 11:41:19.000000 codechain-0.0.3/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-27 12:40:46.518159 codechain-0.0.3/codechain/
--rw-r--r--   0 james      (501) staff       (20)       69 2023-07-27 01:45:29.000000 codechain-0.0.3/codechain/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      861 2023-07-27 01:45:31.000000 codechain-0.0.3/codechain/evaluation.py
--rw-r--r--   0 james      (501) staff       (20)     3409 2023-07-27 12:37:01.000000 codechain-0.0.3/codechain/generation.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-27 12:40:46.518912 codechain-0.0.3/codechain.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     1587 2023-07-27 12:40:46.000000 codechain-0.0.3/codechain.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      252 2023-07-27 12:40:46.000000 codechain-0.0.3/codechain.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-07-27 12:40:46.000000 codechain-0.0.3/codechain.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       10 2023-07-27 12:40:46.000000 codechain-0.0.3/codechain.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       10 2023-07-27 12:40:46.000000 codechain-0.0.3/codechain.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-07-27 12:40:46.519245 codechain-0.0.3/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1066 2023-07-27 12:40:15.000000 codechain-0.0.3/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-31 17:31:26.589179 codechain-0.0.4/
+-rw-r--r--   0 james      (501) staff       (20)     1587 2023-07-31 17:31:26.589038 codechain-0.0.4/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1011 2023-07-27 11:41:19.000000 codechain-0.0.4/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-31 17:31:26.587963 codechain-0.0.4/codechain/
+-rw-r--r--   0 james      (501) staff       (20)       69 2023-07-27 01:45:29.000000 codechain-0.0.4/codechain/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      948 2023-07-27 16:35:20.000000 codechain-0.0.4/codechain/evaluation.py
+-rw-r--r--   0 james      (501) staff       (20)     3416 2023-07-27 16:38:54.000000 codechain-0.0.4/codechain/generation.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-31 17:31:26.588834 codechain-0.0.4/codechain.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     1587 2023-07-31 17:31:26.000000 codechain-0.0.4/codechain.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      252 2023-07-31 17:31:26.000000 codechain-0.0.4/codechain.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-07-31 17:31:26.000000 codechain-0.0.4/codechain.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       10 2023-07-31 17:31:26.000000 codechain-0.0.4/codechain.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       10 2023-07-31 17:31:26.000000 codechain-0.0.4/codechain.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-07-31 17:31:26.589217 codechain-0.0.4/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1066 2023-07-31 16:04:44.000000 codechain-0.0.4/setup.py
```

### Comparing `codechain-0.0.3/PKG-INFO` & `codechain-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codechain
-Version: 0.0.3
+Version: 0.0.4
 Summary: Code generation with LLMs
 Author: James Murdza
 Author-email: <james@jamesmurdza.com>
 Project-URL: Source, https://github.com/jamesmurdza/codechain
 Keywords: python,llms,codegen,code generation
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `codechain-0.0.3/README.md` & `codechain-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `codechain-0.0.3/codechain/evaluation.py` & `codechain-0.0.4/codechain/evaluation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from typing import Optional
 
 from langsmith.evaluation import RunEvaluator, EvaluationResult
 from langsmith.schemas import Run, Example
-
-from human_eval.execution import check_correctness
-from human_eval.data import read_problems
-
-problems = read_problems()
-
 class HumanEvalEvaluator(RunEvaluator):
     """ This is a wrapper around the HumanEval evaluator. """
 
+    def __init__(self):
+
+        from human_eval.data import read_problems
+        
+        self.problems = read_problems()
+
     def evaluate_run(self, run: Run, example: Optional[Example] = None) -> EvaluationResult:
+
+        from human_eval.execution import check_correctness
+
         print("Evaluating " + run.inputs["task_id"])
-        problem = problems[run.inputs["task_id"]]
+        problem = HumanEvalEvaluator.self.problems[run.inputs["task_id"]]
         solution = run.outputs["output"]
 
         # The HumanEval evaluator, which runs the Python code against unit tests
         result = check_correctness(problem, solution, 5)
 
         return EvaluationResult(
             key = "Correctness",
```

### Comparing `codechain-0.0.3/codechain/generation.py` & `codechain-0.0.4/codechain/generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict
 
 from langchain.chains import LLMChain, SimpleSequentialChain, SequentialChain, TransformChain
 from langchain.prompts import PromptTemplate
-from langchain.schema import BaseLanguageModel
+from langchain.base_language import BaseLanguageModel
 import re
 
 class CodeChain(SimpleSequentialChain):
     """ Chain that generates code from a prompt. """
     
     @staticmethod
     async def extract_code(inputs: dict) -> dict:
```

### Comparing `codechain-0.0.3/codechain.egg-info/PKG-INFO` & `codechain-0.0.4/codechain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codechain
-Version: 0.0.3
+Version: 0.0.4
 Summary: Code generation with LLMs
 Author: James Murdza
 Author-email: <james@jamesmurdza.com>
 Project-URL: Source, https://github.com/jamesmurdza/codechain
 Keywords: python,llms,codegen,code generation
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `codechain-0.0.3/setup.py` & `codechain-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Code generation with LLMs'
 
 # Setting up
 setup(
     name="codechain",
     version=VERSION,
     author="James Murdza",
```

