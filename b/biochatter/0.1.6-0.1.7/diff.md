# Comparing `tmp/biochatter-0.1.6.tar.gz` & `tmp/biochatter-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biochatter-0.1.6.tar", max compression
+gzip compressed data, was "biochatter-0.1.7.tar", max compression
```

## Comparing `biochatter-0.1.6.tar` & `biochatter-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-06-13 11:08:28.958016 biochatter-0.1.6/LICENSE
--rw-r--r--   0        0        0      453 2023-06-28 13:22:29.968048 biochatter-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-06-13 11:09:32.282374 biochatter-0.1.6/biochatter/__init__.py
--rw-r--r--   0        0        0     2672 2023-06-16 16:39:33.107276 biochatter-0.1.6/biochatter/_stats.py
--rw-r--r--   0        0        0    18302 2023-07-07 08:35:59.679816 biochatter-0.1.6/biochatter/llm_connect.py
--rw-r--r--   0        0        0     5922 2023-07-19 11:17:00.987814 biochatter-0.1.6/biochatter/podcast.py
--rw-r--r--   0        0        0     7150 2023-07-19 11:48:37.917691 biochatter-0.1.6/biochatter/vectorstore.py
--rw-r--r--   0        0        0      765 2023-07-19 11:48:37.919179 biochatter-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1475 1970-01-01 00:00:00.000000 biochatter-0.1.6/setup.py
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 biochatter-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-13 11:08:28.958016 biochatter-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1670 2023-07-27 11:53:21.701606 biochatter-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 11:09:32.282374 biochatter-0.1.7/biochatter/__init__.py
+-rw-r--r--   0        0        0     2672 2023-06-16 16:39:33.107276 biochatter-0.1.7/biochatter/_stats.py
+-rw-r--r--   0        0        0    18628 2023-07-31 16:02:01.952939 biochatter-0.1.7/biochatter/llm_connect.py
+-rw-r--r--   0        0        0     5922 2023-07-19 11:17:00.987814 biochatter-0.1.7/biochatter/podcast.py
+-rw-r--r--   0        0        0     8432 2023-07-27 11:53:21.702371 biochatter-0.1.7/biochatter/vectorstore.py
+-rw-r--r--   0        0        0     6158 2023-07-27 11:53:21.702650 biochatter-0.1.7/biochatter/vectorstore_host.py
+-rw-r--r--   0        0        0      788 2023-07-31 16:07:08.882683 biochatter-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2730 1970-01-01 00:00:00.000000 biochatter-0.1.7/setup.py
+-rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 biochatter-0.1.7/PKG-INFO
```

### Comparing `biochatter-0.1.6/LICENSE` & `biochatter-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `biochatter-0.1.6/biochatter/_stats.py` & `biochatter-0.1.7/biochatter/_stats.py`

 * *Files identical despite different names*

### Comparing `biochatter-0.1.6/biochatter/llm_connect.py` & `biochatter-0.1.7/biochatter/llm_connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,20 +148,20 @@
         self.data_input_tool = df
 
         for tool_name in self.prompts["tool_prompts"]:
             if tool_name in input_file_name:
                 msg = self.prompts["tool_prompts"][tool_name].format(df=df)
                 self.append_system_message(msg)
 
-    def query(self, text: str):
+    def query(self, text: str, collection_name: Optional[str] = None):
         self.append_user_message(text)
 
         if self.docsum:
             if self.docsum.use_prompt:
-                self._inject_context(text)
+                self._inject_context(text, collection_name)
 
         msg, token_usage = self._primary_query()
 
         if not token_usage:
             # indicates error
             return (msg, token_usage, None)
 
@@ -209,15 +209,15 @@
     def _primary_query(self, text: str):
         pass
 
     @abstractmethod
     def _correct_response(self, msg: str):
         pass
 
-    def _inject_context(self, text: str):
+    def _inject_context(self, text: str, collection_name: Optional[str] = None):
         """
         Inject the context into the prompt from vector database similarity
         search. Finds the most similar n text fragments and adds them to the
         message history object for usage in the next prompt. Uses the document
         summarisation prompt set to inject the context. The ultimate prompt
         should include the placeholder for the statements, `{statements}` (used
         for formatting the string).
@@ -240,22 +240,24 @@
         if st:
             with st.spinner(sim_msg):
                 statements = [
                     doc.page_content
                     for doc in self.docsum.similarity_search(
                         text,
                         self.docsum.n_results,
+                        collection_name,
                     )
                 ]
         else:
             statements = [
                 doc.page_content
                 for doc in self.docsum.similarity_search(
                     text,
                     self.docsum.n_results,
+                    collection_name,
                 )
             ]
 
         prompts = self.prompts["docsum_prompts"]
         if statements:
             self.current_statements = statements
             for i, prompt in enumerate(prompts):
@@ -527,14 +529,20 @@
             test = self.chat.generate([[HumanMessage(content="Hello")]])
 
             return True
 
         except openai.error.AuthenticationError as e:
             return False
 
+    def _update_usage_stats(self, model: str, token_usage: dict):
+        """
+        We do not track usage stats for Azure.
+        """
+        return
+
 
 class BloomConversation(Conversation):
     def __init__(
         self,
         model_name: str,
         prompts: dict,
         split_correction: bool,
```

### Comparing `biochatter-0.1.6/biochatter/podcast.py` & `biochatter-0.1.7/biochatter/podcast.py`

 * *Files identical despite different names*

### Comparing `biochatter-0.1.6/pyproject.toml` & `biochatter-0.1.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biochatter"
-version = "0.1.6"
+version = "0.1.7"
 description = "Backend library for conversational AI in biomedicine"
 authors = ["Sebastian Lobentanzer <sebastian.lobentanzer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
@@ -20,14 +20,14 @@
 streamlit = { version = "^1.23.1", optional = true }
 gTTS = { version = "^2.3.2", optional = true }
 
 [tool.poetry.extras]
 streamlit = ["streamlit"]
 podcast = ["gTTS"]
 
-
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
+bump2version = "^1.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

