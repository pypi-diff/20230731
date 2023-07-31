# Comparing `tmp/tembo_pgmq_python-0.3.0.tar.gz` & `tmp/tembo_pgmq_python-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tembo_pgmq_python-0.3.0.tar", max compression
+gzip compressed data, was "tembo_pgmq_python-0.3.1.tar", max compression
```

## Comparing `tembo_pgmq_python-0.3.0.tar` & `tembo_pgmq_python-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1491 2023-07-13 03:34:35.192602 tembo_pgmq_python-0.3.0/README.md
--rw-r--r--   0        0        0     1168 2023-07-13 03:34:35.192602 tembo_pgmq_python-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      105 2023-07-13 03:34:35.192602 tembo_pgmq_python-0.3.0/tembo_pgmq_python/__init__.py
--rw-r--r--   0        0        0     4651 2023-07-13 03:34:35.192602 tembo_pgmq_python-0.3.0/tembo_pgmq_python/queue.py
--rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 tembo_pgmq_python-0.3.0/setup.py
--rw-r--r--   0        0        0     2389 1970-01-01 00:00:00.000000 tembo_pgmq_python-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1490 2023-07-31 21:05:17.403224 tembo_pgmq_python-0.3.1/README.md
+-rw-r--r--   0        0        0     1168 2023-07-31 21:05:17.403224 tembo_pgmq_python-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      105 2023-07-31 21:05:17.403224 tembo_pgmq_python-0.3.1/tembo_pgmq_python/__init__.py
+-rw-r--r--   0        0        0     4651 2023-07-31 21:05:17.403224 tembo_pgmq_python-0.3.1/tembo_pgmq_python/queue.py
+-rw-r--r--   0        0        0     2277 1970-01-01 00:00:00.000000 tembo_pgmq_python-0.3.1/setup.py
+-rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 tembo_pgmq_python-0.3.1/PKG-INFO
```

### Comparing `tembo_pgmq_python-0.3.0/README.md` & `tembo_pgmq_python-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Postgres running the [Tembo PGMQ extension](https://github.com/tembo-io/tembo/tree/main/pgmq).
 
 ## Usage
 
 ## Start a Postgres Instance with the Tembo extension installed
 
 ```bash
-docker run -d --name postgres -e POSTGRES_PASSWORD=postgres -p 5432:5432 quay.io/coredb/pgmq-pg:latest
+docker run -d --name postgres -e POSTGRES_PASSWORD=postgres -p 5432:5432 quay.io/tembo/pgmq-pg:latest
 ```
 
 Initialize a connection to Postgres
 
 ```python
 from tembo_pgmq_python import PGMQueue, Message
```

### Comparing `tembo_pgmq_python-0.3.0/pyproject.toml` & `tembo_pgmq_python-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tembo-pgmq-python"
-version = "0.3.0"
+version = "0.3.1"
 description = "Python client for the PGMQ Postgres extension."
 authors = ["Adam Hendel <adam@tembo.io>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "tembo_pgmq_python"}]
 
 [tool.poetry.urls]
```

### Comparing `tembo_pgmq_python-0.3.0/tembo_pgmq_python/queue.py` & `tembo_pgmq_python-0.3.1/tembo_pgmq_python/queue.py`

 * *Files identical despite different names*

### Comparing `tembo_pgmq_python-0.3.0/setup.py` & `tembo_pgmq_python-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 install_requires = \
 ['orjson>=3.8.10,<4.0.0',
  'psycopg[binary,pool]>=3.1.8,<4.0.0',
  'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'tembo-pgmq-python',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Python client for the PGMQ Postgres extension.',
-    'long_description': '# Tembo\'s Python Client for PGMQ\n\n## Installation\n\nInstall with `pip` from pypi.org\n\n```bash\npip install tembo-pgmq-python\n```\n\nDependencies:\n\nPostgres running the [Tembo PGMQ extension](https://github.com/tembo-io/tembo/tree/main/pgmq).\n\n## Usage\n\n## Start a Postgres Instance with the Tembo extension installed\n\n```bash\ndocker run -d --name postgres -e POSTGRES_PASSWORD=postgres -p 5432:5432 quay.io/coredb/pgmq-pg:latest\n```\n\nInitialize a connection to Postgres\n\n```python\nfrom tembo_pgmq_python import PGMQueue, Message\n\nqueue = PGMQueue(host="0.0.0.0")\n```\n\nCreate a queue (or a partitioned queue)\n\n```python\nqueue.create_queue("my_queue")\n# queue.create_partitioned_queue("my_partitioned_queue", partition_size=10000)\n```\n\n\nSend a message\n\n```python\nmsg_id: int = queue.send("my_queue", {"hello": "world"})\n```\n\nRead a message, set it invisible for 30 seconds.\n\n```python\nread_message: Message = queue.read("my_queue", vt=10)\nprint(read_message)\n```\n\nArchive the message after we\'re done with it. Archived messages are moved to an archive table.\n\n```python\narchived: bool = queue.archive("my_queue", read_message.msg_id)\n```\n\nDelete a message completely.\n\n```python\nmsg_id: int = queue.send("my_queue", {"hello": "world"})\nread_message: Message = queue.read("my_queue")\ndeleted: bool = queue.delete("my_queue", read_message.msg_id)\n```\n\nPop a message, deleting it and reading it in one transaction.\n\n```python\npopped_message: Message = queue.pop("my_queue")\nprint(popped_message)\n```\n',
+    'long_description': '# Tembo\'s Python Client for PGMQ\n\n## Installation\n\nInstall with `pip` from pypi.org\n\n```bash\npip install tembo-pgmq-python\n```\n\nDependencies:\n\nPostgres running the [Tembo PGMQ extension](https://github.com/tembo-io/tembo/tree/main/pgmq).\n\n## Usage\n\n## Start a Postgres Instance with the Tembo extension installed\n\n```bash\ndocker run -d --name postgres -e POSTGRES_PASSWORD=postgres -p 5432:5432 quay.io/tembo/pgmq-pg:latest\n```\n\nInitialize a connection to Postgres\n\n```python\nfrom tembo_pgmq_python import PGMQueue, Message\n\nqueue = PGMQueue(host="0.0.0.0")\n```\n\nCreate a queue (or a partitioned queue)\n\n```python\nqueue.create_queue("my_queue")\n# queue.create_partitioned_queue("my_partitioned_queue", partition_size=10000)\n```\n\n\nSend a message\n\n```python\nmsg_id: int = queue.send("my_queue", {"hello": "world"})\n```\n\nRead a message, set it invisible for 30 seconds.\n\n```python\nread_message: Message = queue.read("my_queue", vt=10)\nprint(read_message)\n```\n\nArchive the message after we\'re done with it. Archived messages are moved to an archive table.\n\n```python\narchived: bool = queue.archive("my_queue", read_message.msg_id)\n```\n\nDelete a message completely.\n\n```python\nmsg_id: int = queue.send("my_queue", {"hello": "world"})\nread_message: Message = queue.read("my_queue")\ndeleted: bool = queue.delete("my_queue", read_message.msg_id)\n```\n\nPop a message, deleting it and reading it in one transaction.\n\n```python\npopped_message: Message = queue.pop("my_queue")\nprint(popped_message)\n```\n',
     'author': 'Adam Hendel',
     'author_email': 'adam@tembo.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `tembo_pgmq_python-0.3.0/PKG-INFO` & `tembo_pgmq_python-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tembo-pgmq-python
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python client for the PGMQ Postgres extension.
 License: Apache 2.0
 Author: Adam Hendel
 Author-email: adam@tembo.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 Postgres running the [Tembo PGMQ extension](https://github.com/tembo-io/tembo/tree/main/pgmq).
 
 ## Usage
 
 ## Start a Postgres Instance with the Tembo extension installed
 
 ```bash
-docker run -d --name postgres -e POSTGRES_PASSWORD=postgres -p 5432:5432 quay.io/coredb/pgmq-pg:latest
+docker run -d --name postgres -e POSTGRES_PASSWORD=postgres -p 5432:5432 quay.io/tembo/pgmq-pg:latest
 ```
 
 Initialize a connection to Postgres
 
 ```python
 from tembo_pgmq_python import PGMQueue, Message
```

