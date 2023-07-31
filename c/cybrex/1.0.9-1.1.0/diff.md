# Comparing `tmp/cybrex-1.0.9.tar.gz` & `tmp/cybrex-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.0.9.tar", last modified: Sun Jul 23 17:55:39 2023, max compression
+gzip compressed data, was "cybrex-1.1.0.tar", last modified: Mon Jul 31 15:19:32 2023, max compression
```

## Comparing `cybrex-1.0.9.tar` & `cybrex-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-23 17:55:39.759788 cybrex-1.0.9/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.0.9/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)     1479 2023-07-23 17:55:39.759548 cybrex-1.0.9/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)     1203 2023-07-23 17:52:09.000000 cybrex-1.0.9/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-23 17:55:39.757233 cybrex-1.0.9/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.0.9/cybrex/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     4685 2023-07-23 17:55:11.000000 cybrex-1.0.9/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     8231 2023-07-23 17:55:13.000000 cybrex-1.0.9/cybrex/cybrex_ai.py
--rw-r--r--   0 pasha      (501) staff       (20)     3213 2023-07-23 17:55:13.000000 cybrex-1.0.9/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-23 17:55:39.759129 cybrex-1.0.9/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)     1479 2023-07-23 17:55:39.000000 cybrex-1.0.9/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      305 2023-07-23 17:55:39.000000 cybrex-1.0.9/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-23 17:55:39.000000 cybrex-1.0.9/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-23 17:55:39.000000 cybrex-1.0.9/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      182 2023-07-23 17:55:39.000000 cybrex-1.0.9/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-07-23 17:55:39.000000 cybrex-1.0.9/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-07-23 17:55:23.000000 cybrex-1.0.9/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      182 2023-07-19 20:14:47.000000 cybrex-1.0.9/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-23 17:55:39.759935 cybrex-1.0.9/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-31 15:19:32.021487 cybrex-1.1.0/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.1.0/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)    24132 2023-07-31 15:19:32.021141 cybrex-1.1.0/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)    23856 2023-07-23 19:18:23.000000 cybrex-1.1.0/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-31 15:19:32.018583 cybrex-1.1.0/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.1.0/cybrex/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5659 2023-07-31 15:18:57.000000 cybrex-1.1.0/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    11473 2023-07-31 15:18:57.000000 cybrex-1.1.0/cybrex/cybrex_ai.py
+-rw-r--r--   0 pasha      (501) staff       (20)     3213 2023-07-31 15:18:57.000000 cybrex-1.1.0/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-31 15:19:32.020562 cybrex-1.1.0/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)    24132 2023-07-31 15:19:32.000000 cybrex-1.1.0/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      305 2023-07-31 15:19:32.000000 cybrex-1.1.0/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-31 15:19:32.000000 cybrex-1.1.0/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-31 15:19:32.000000 cybrex-1.1.0/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      182 2023-07-31 15:19:32.000000 cybrex-1.1.0/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-07-31 15:19:32.000000 cybrex-1.1.0/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-07-31 15:19:10.000000 cybrex-1.1.0/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      182 2023-07-30 14:20:06.000000 cybrex-1.1.0/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-31 15:19:32.021615 cybrex-1.1.0/setup.cfg
```

### Comparing `cybrex-1.0.9/cybrex/cli.py` & `cybrex-1.1.0/cybrex/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,70 +13,79 @@
     return metadata['doi'] + ': ' + document
 
 
 class CybrexCli:
     def __init__(self):
         self.cybrex = CybrexAI()
 
-    async def semantic_search(self, question: str, top_n: int = 7, summa_documents: int = 9):
+    async def add_all_documents(self):
+        async with self.cybrex as cybrex:
+            async for document in cybrex.geck.get_summa_client().documents('nexus_science'):
+                document = json.loads(document)
+                await self.cybrex.add_documents([document])
+
+    async def dump_texts(self, query: str, output_path: str, n_summa_documents: int = 100):
         """
-        Ask a question about content of document identified by DOI.
+        Store STC text chunks in ZIP archive
 
-        :param question: question to STC
-        :param top_n: number of pieces to return
-        :param summa_documents: the number of documents to extract from Chroma
-            more means more tokens to use and more precision in answer
+        :param query: query to STC
+        :param output_path: where to store result
+        :param n_summa_documents: the number of documents to extract
         """
         async with self.cybrex as cybrex:
-            print(f"{colored('Q', 'green')}: {question}")
-            response = await cybrex.semantic_search(
-                question=question,
-                top_n=top_n,
-                summa_documents=summa_documents
+            print(f"{colored('Q', 'green')}: {query}")
+            await cybrex.dump_texts(
+                query=query,
+                output_path=output_path,
+                n_summa_documents=n_summa_documents
+            )
+
+    async def import_texts(self, input_path: str):
+        """
+        Import binary file with embeddings
+
+        :param input_path:
+        """
+        async with self.cybrex as cybrex:
+            await cybrex.import_texts(
+                input_path=input_path,
             )
-            print(response)
-            snippets = [
-                ' - ' + create_snippet(document, metadata)
-                for (document, metadata) in zip(response['documents'][0], response['metadatas'][0])
-            ]
-            sources = '\n'.join(snippets)
-            print(f"{colored('Sources', 'green')}:\n{sources}")
 
-    async def chat_doc(self, field: str, value: str, question: str, top_n: int = 7):
+    async def chat_doc(self, field: str, value: str, question: str, n_results: int = 7):
         """
         Ask a question about content of document identified by DOI.
 
         :param field: name of the field in document used for selection
         :param value: value of the field in document used for selection
         :param question: Text question to the document
-        :param top_n: the number of documents to extract from Chroma
+        :param n_results: the number of documents to extract from Chroma
             more means more tokens to use and more precision in answer
         """
         async with self.cybrex as cybrex:
             print(f"{colored('Document', 'green')}: {field}:{value}")
             print(f"{colored('Q', 'green')}: {question}")
-            response = await cybrex.chat_document(field, value, question, top_n)
+            response = await cybrex.chat_document(field, value, question, n_results)
             print(f"{colored('A', 'green')}: {response}")
 
-    async def chat_sci(self, question: str, top_n: int = 7, summa_documents: int = 9):
+    async def chat_sci(self, question: str, n_results: int = 7, n_summa_documents: int = 9):
         """
         Ask a question about content of document identified by DOI.
 
         :param question: Text question to the document
-        :param top_n: the number of documents to extract from Chroma
+        :param n_results: the number of documents to extract from Chroma
             more means more tokens to use and more precision in answer
-        :param summa_documents: the number of documents to extract from Chroma
+        :param n_summa_documents: the number of documents to extract from Chroma
             more means more tokens to use and more precision in answer
         """
         async with self.cybrex as cybrex:
             print(f"{colored('Q', 'green')}: {question}")
             response = await cybrex.chat_science(
                 question=question,
-                top_n=top_n,
-                summa_documents=summa_documents,
+                n_results=n_results,
+                n_summa_documents=n_summa_documents,
             )
             print(f"{colored('A', 'green')}: {response['result'].strip()}")
             snippets = [create_snippet(source_document.page_content, source_document.metadata) for source_document in response['source_documents']]
             sources = textwrap.indent('\n'.join(snippets), ' - ')
             print(f"{colored('Sources', 'green')}:\n{sources}")
 
     async def sum_doc(self, field: str, value: str):
@@ -87,32 +96,51 @@
         :param value: value of the field in document used for selection
         """
         async with self.cybrex as cybrex:
             print(f"{colored('Document', 'green')}: {field}:{value}")
             response = await cybrex.summarize_document(field, value)
             print(f"{colored('Summarization', 'green')}: {response}")
 
-    async def add_all_documents(self):
+    async def semantic_search(self, query: str, n_results: int = 7, n_summa_documents: int = 9):
+        """
+        Ask a question about content of document identified by DOI.
+
+        :param query: query to STC
+        :param n_results: number of pieces to return
+        :param n_summa_documents: the number of documents to extract from Chroma
+            more means more tokens to use and more precision in answer
+        """
         async with self.cybrex as cybrex:
-            async for document in cybrex.geck.get_summa_client().documents('nexus_science'):
-                document = json.loads(document)
-                await self.cybrex.add_documents([document])
+            print(f"{colored('Q', 'green')}: {query}")
+            response = await cybrex.semantic_search(
+                query=query,
+                n_results=n_results,
+                n_summa_documents=n_summa_documents
+            )
+            snippets = [
+                ' - ' + create_snippet(document, metadata)
+                for (document, metadata) in zip(response['documents'][0], response['metadatas'][0])
+            ]
+            sources = '\n'.join(snippets)
+            print(f"{colored('Sources', 'green')}:\n{sources}")
 
 
 async def cybrex_cli(debug: bool = False):
     """
     :param debug: add debugging output
     :return:
     """
     logging.basicConfig(stream=sys.stdout, level=logging.INFO if debug else logging.ERROR)
     cybrex_ai = CybrexCli()
     return {
         'add-all-documents': cybrex_ai.add_all_documents,
         'chat-doc': cybrex_ai.chat_doc,
         'chat-sci': cybrex_ai.chat_sci,
+        'dump-texts': cybrex_ai.dump_texts,
+        'import-texts': cybrex_ai.import_texts,
         'semantic-search': cybrex_ai.semantic_search,
         'sum-doc': cybrex_ai.sum_doc,
     }
 
 
 def main():
     fire.Fire(cybrex_cli, name='cybrex')
```

### Comparing `cybrex-1.0.9/cybrex/cybrex_ai.py` & `cybrex-1.1.0/cybrex/cybrex_ai.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,37 @@
+import base64
 import io
+import json
 import logging
 import os.path
 import uuid
+from gzip import GzipFile
 from typing import (
     List,
     Optional,
 )
 
 import chromadb
+import numpy as np
 import pypdf
 import yaml
 from aiokit import AioThing
+from bs4 import BeautifulSoup
 from izihawa_configurator import Configurator
 from izihawa_utils.exceptions import BaseError
 from izihawa_utils.file import mkdir_p
 from langchain.chains import RetrievalQA
 from langchain.chains.summarize import load_summarize_chain
 from langchain.schema import Document
 from langchain.vectorstores import Chroma
 from stc_geck.advices import get_documents_on_topic
 from stc_geck.client import StcGeck
 
 from .models import (
-    OpenAIModel,
+    DefaultModel,
     models_dict,
 )
 
 
 class DocumentNotFoundError(BaseError):
     pass
 
@@ -38,28 +43,32 @@
 def default_config():
     return {
         'ipfs': {
             'http': {
                 'base_url': 'http://127.0.0.1:8080'
             }
         },
-        'model': OpenAIModel.name,
+        'model': DefaultModel.name,
         'summa': {
-            'endpoint': '127.0.0.1:10083'
+            'endpoint': '127.0.0.1:10082'
         },
     }
 
 
 class CybrexAI(AioThing):
     def __init__(
         self,
-        home_path: str = '~/.cybrex',
+        home_path: Optional[str] = None,
         geck: Optional[StcGeck] = None,
     ):
         super().__init__()
+
+        if home_path is None:
+            home_path = os.environ.get("CYBREX_HOME", "~/.cybrex")
+
         self.home_path = os.path.expanduser(home_path)
         if not os.path.exists(self.home_path):
             mkdir_p(self.home_path)
 
         config_path = os.path.join(self.home_path, 'config.yaml')
         if not os.path.exists(config_path):
             with open(config_path, 'w') as f:
@@ -100,138 +109,213 @@
             match primary_link['type']:
                 case 'pdf':
                     pdf_reader = pypdf.PdfReader(io.BytesIO(file_content))
                     return '\n'.join(page.extract_text() for page in pdf_reader.pages)
                 case _:
                     raise RuntimeError("Unsupported extension")
 
-    async def add_documents(self, documents: List[dict], use_only_stored_content: bool = True):
+    async def generate_chunks_from_document(self, document):
+        doi = document['doi']
+        content = await self.resolve_document_content(document)
+        if not content:
+            return
+
+        abstract = document.get('abstract', '')
+
+        logging.getLogger('statbox').info({
+            'action': 'chunking',
+            'doi': doi,
+        })
+
+        extracted_texts = []
+
+        abstract_soup = BeautifulSoup(abstract, features='lxml')
+        content_soup = BeautifulSoup(content, features='lxml')
+
+        for section_id, section in enumerate(list(abstract_soup.children) + list(content_soup.children)):
+            for el in list(section.find_all()):
+                if el.name in {'ref', 'formula', 'math', 'figure'}:
+                    el.extract()
+            text = section.get_text(' ', strip=True)
+            if len(text) < 128:
+                continue
+            extracted_texts.append(text)
+
         metadatas = []
         texts = []
 
+        for chunk_id, chunk in enumerate(self.model.text_splitter.split_text('\n\n'.join(extracted_texts))):
+            if len(chunk) < 128:
+                continue
+            texts.append(chunk)
+            metadatas.append({
+                'doi': doi,
+                'length': len(chunk),
+                'chunk_id': chunk_id,
+            })
+        return metadatas, texts
+
+    async def _get_missing_documents_chunks(self, documents: List[dict], skip_downloading_pdf: bool = True):
+        metadatas = []
+        texts = []
         for document in documents:
             doi = document['doi']
             if self.collection.get(where={'doi': doi})['documents']:
                 logging.getLogger('statbox').info({
                     'action': 'already_stored',
                     'doi': doi,
                 })
                 continue
-            if use_only_stored_content and 'content' not in document:
+            if skip_downloading_pdf and 'content' not in document:
                 logging.getLogger('statbox').info({
                     'action': 'no_content',
                     'doi': doi,
                 })
                 continue
             logging.getLogger('statbox').info({
                 'action': 'retrieve_content',
                 'doi': doi,
             })
-            content = await self.resolve_document_content(document)
-            if not content:
-                continue
-            logging.getLogger('statbox').info({
-                'action': 'chunking',
-                'doi': doi,
-            })
-            index = -1
-            for chunk_id, chunk in enumerate(self.model.text_splitter.split_text(content)):
-                index = content.find(chunk, index + 1)
-                metadata = {
-                    'doi': doi,
-                    'chunk_id': chunk_id,
-                    'start_index': index,
-                    'length': len(chunk),
-                }
-                metadatas.append(metadata)
-                texts.append(chunk)
+            document_metadatas, document_texts = await self.generate_chunks_from_document(document)
+            metadatas.extend(document_metadatas)
+            texts.extend(document_texts)
+        return metadatas, texts
+
+    async def add_documents(self, documents: List[dict], skip_downloading_pdf: bool = True):
+        if not documents:
+            return
+        metadatas, texts = await self._get_missing_documents_chunks(documents, skip_downloading_pdf=skip_downloading_pdf)
         if texts:
             self.collection.upsert(
                 documents=texts,
                 metadatas=metadatas,
                 ids=[str(uuid.uuid1()) for _ in range(len(texts))]
             )
 
-    async def semantic_search(self, question: str, top_n: int = 10, summa_documents: int = 10):
-        await self.add_documents_for_question(question, summa_documents)
-        query_embedding = self.model.embedding_function.embed_query(question)
-        return self.collection.query(
-            query_embeddings=[query_embedding],
-            n_results=top_n,
-            include=['documents', 'metadatas'],
+    async def add_document_by_field_value(self, field, value) -> List[Document]:
+        documents = await self.geck.get_summa_client().search_documents([{
+            'index_alias': 'nexus_science',
+            'collectors': [{'top_docs': {'limit': 1}}],
+            'query': {'term': {'field': field, 'value': value}}
+        }])
+        if not documents:
+            raise DocumentNotFoundError(**{field: value})
+        await self.add_documents(documents)
+        documents = [Document(page_content=text) for text in self.collection.get(where={field: value})['documents']]
+        return documents
+
+    def as_retriever(self, embedding_function=None, **kwargs):
+        chroma = Chroma(
+            client=self.db,
+            collection_name=self.collection_name,
+            persist_directory=self.home_path,
+            embedding_function=embedding_function or self.model.embedding_function,
         )
+        return chroma.as_retriever(**kwargs)
+
+    async def dump_texts(self, query: str, output_path: str, n_summa_documents: int, skip_downloading_pdf: bool = True):
+        documents = await self.keywords_search(query, n_summa_documents=n_summa_documents)
+        metadatas, texts = await self._get_missing_documents_chunks(
+            documents,
+            skip_downloading_pdf=skip_downloading_pdf,
+        )
+        with GzipFile(output_path, mode='wb') as zipper:
+            zipper.writelines([
+                json.dumps({'metadata': metadata, 'text': text}).encode() + b'\n'
+                for metadata, text in zip(metadatas, texts)
+            ])
+
+    async def import_texts(self, input_path: str):
+        metadatas = []
+        texts = []
+        embeddings = []
+        with GzipFile(input_path, mode='rb') as zipper:
+            for line in zipper.readlines():
+                processed_document = json.loads(line)
+                doi = processed_document['metadata']['doi']
+                if self.collection.get(where={'doi': doi})['documents']:
+                    logging.getLogger('statbox').info({
+                        'action': 'already_stored',
+                        'doi': doi,
+                    })
+                    continue
+                metadatas.append(processed_document['metadata'])
+                texts.append(processed_document['text'])
+                embedding = base64.b64decode(processed_document['embedding'])
+                embedding = [n.item() for n in np.frombuffer(embedding, dtype=np.float64)]
+                embeddings.append(embedding)
 
-    async def chat_document(self, field, value, question, top_n: int):
+        if texts:
+            self.collection.upsert(
+                documents=texts,
+                metadatas=metadatas,
+                embeddings=embeddings,
+                ids=[str(uuid.uuid1()) for _ in range(len(texts))]
+            )
+
+    async def chat_document(self, field, value, question, n_results: int):
         await self.add_document_by_field_value(field, value)
-        if top_n > 3:
+        if n_results > 3:
             chain_type = 'map_reduce'
         else:
             chain_type = 'stuff'
         qa = RetrievalQA.from_chain_type(
             llm=self.model.llm,
             chain_type=chain_type,
             retriever=self.as_retriever(
                 search_type='similarity',
                 search_kwargs={
-                    'k': top_n,
+                    'k': n_results,
                     'filter': {
                         field: value,
                     }
                 },
             ),
         )
         result = qa({"query": question})
         return result["result"].strip()
 
-    async def chat_science(self, question, top_n: int, summa_documents: int):
-        await self.add_documents_for_question(question, summa_documents)
+    async def chat_science(self, query: str, n_results: int, n_summa_documents: int):
+        documents = await self.keywords_search(query, n_summa_documents)
+        await self.add_documents(documents)
+
         qa = self.model.get_retrieval_qa(retriever=self.as_retriever(
             search_type='similarity',
             search_kwargs={
-                'k': top_n,
+                'k': n_results,
             },
         ))
-        result = qa({"query": question})
+        result = qa({"query": query})
         return result
 
-    async def summarize_document(self, field, value):
-        documents = await self.add_document_by_field_value(field, value)
-        chain = load_summarize_chain(llm=self.model.llm, chain_type="map_reduce")
-        result = chain.run(documents)
-        return result.strip()
-
-    async def add_document_by_field_value(self, field, value) -> List[Document]:
-        documents = await self.geck.get_summa_client().search_documents([{
-            'index_alias': 'nexus_science',
-            'collectors': [{'top_docs': {'limit': 1}}],
-            'query': {'term': {'field': field, 'value': value}}
-        }])
-        if not documents:
-            raise DocumentNotFoundError(**{field: value})
-        await self.add_documents(documents)
-        documents = [Document(page_content=text) for text in self.collection.get(where={field: value})['documents']]
-        return documents
-
-    async def add_documents_for_question(self, question: str, documents: int):
-        if documents == 0:
-            return
+    async def keywords_search(self, query: str, n_summa_documents: int):
+        if not n_summa_documents:
+            return []
         keywords = self.model.keyword_extractor.extract_keywords(
-            question,
+            query,
             top_n=3,
             keyphrase_ngram_range=(1, 1),
         )
         topic = ' '.join(map(lambda x: x[0], keywords))
         documents = await get_documents_on_topic(
             summa_client=self.geck.get_summa_client(),
             topic=topic,
-            documents=documents,
+            documents=n_summa_documents,
         )
-        return await self.add_documents(documents)
+        return documents
 
-    def as_retriever(self, embedding_function=None, **kwargs):
-        chroma = Chroma(
-            client=self.db,
-            collection_name=self.collection_name,
-            persist_directory=self.home_path,
-            embedding_function=embedding_function or self.model.embedding_function,
+    async def semantic_search(self, query: str, n_results: int = 10, n_summa_documents: int = 10):
+        documents = await self.keywords_search(query, n_summa_documents)
+        await self.add_documents(documents)
+
+        query_embedding = self.model.embedding_function.embed_query(query)
+        return self.collection.query(
+            query_embeddings=[query_embedding],
+            n_results=n_results,
+            include=['documents', 'metadatas'],
         )
-        return chroma.as_retriever(**kwargs)
+
+    async def summarize_document(self, field, value):
+        documents = await self.add_document_by_field_value(field, value)
+        chain = load_summarize_chain(llm=self.model.llm, chain_type="map_reduce")
+        result = chain.run(documents)
+        return result.strip()
```

### Comparing `cybrex-1.0.9/cybrex/models.py` & `cybrex-1.1.0/cybrex/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,18 +37,18 @@
 class BaseModel:
     @lazy
     def keyword_extractor(self):
         return KeyBERT()
 
 
 class DefaultModel(BaseModel):
-    name = 'wizardlm-13b-uncensored_instructor-xl_rcts-2048-256'
+    name = 'wizardlm-13b-uncensored_instructor-xl_rcts-1024-128'
 
     def __init__(self):
-        self.text_splitter = RecursiveCharacterTextSplitter(chunk_size=2048, chunk_overlap=256)
+        self.text_splitter = RecursiveCharacterTextSplitter(chunk_size=1024, chunk_overlap=128)
 
     @lazy
     def llm(self):
         return CTransformers(
             model='TheBloke/WizardLM-13B-uncensored-GGML',
             model_file='wizardLM-13B-Uncensored.ggmlv3.q5_1.bin',
             model_type='llama',
```

### Comparing `cybrex-1.0.9/pyproject.toml` & `cybrex-1.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.0.9"
+version = "1.1.0"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

