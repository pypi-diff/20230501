# Comparing `tmp/coredb_pgmq_python-0.2.0.tar.gz` & `tmp/coredb_pgmq_python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coredb_pgmq_python-0.2.0.tar", max compression
+gzip compressed data, was "coredb_pgmq_python-0.2.1.tar", max compression
```

## Comparing `coredb_pgmq_python-0.2.0.tar` & `coredb_pgmq_python-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1510 2023-04-25 14:35:45.630453 coredb_pgmq_python-0.2.0/README.md
--rw-r--r--   0        0        0      106 2023-04-25 14:35:45.630453 coredb_pgmq_python-0.2.0/coredb_pgmq_python/__init__.py
--rw-r--r--   0        0        0     3532 2023-04-25 14:35:45.630453 coredb_pgmq_python-0.2.0/coredb_pgmq_python/queue.py
--rw-r--r--   0        0        0     1015 2023-04-25 14:35:45.630453 coredb_pgmq_python-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 coredb_pgmq_python-0.2.0/setup.py
--rw-r--r--   0        0        0     2425 1970-01-01 00:00:00.000000 coredb_pgmq_python-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1510 2023-05-01 16:40:17.818132 coredb_pgmq_python-0.2.1/README.md
+-rw-r--r--   0        0        0      106 2023-05-01 16:40:17.818132 coredb_pgmq_python-0.2.1/coredb_pgmq_python/__init__.py
+-rw-r--r--   0        0        0     3532 2023-05-01 16:40:17.818132 coredb_pgmq_python-0.2.1/coredb_pgmq_python/queue.py
+-rw-r--r--   0        0        0     1029 2023-05-01 16:40:17.818132 coredb_pgmq_python-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 coredb_pgmq_python-0.2.1/setup.py
+-rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 coredb_pgmq_python-0.2.1/PKG-INFO
```

### Comparing `coredb_pgmq_python-0.2.0/README.md` & `coredb_pgmq_python-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `coredb_pgmq_python-0.2.0/coredb_pgmq_python/queue.py` & `coredb_pgmq_python-0.2.1/coredb_pgmq_python/queue.py`

 * *Files identical despite different names*

### Comparing `coredb_pgmq_python-0.2.0/pyproject.toml` & `coredb_pgmq_python-0.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 [tool.poetry]
 name = "coredb-pgmq-python"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python client for the PGMQ Postgres extension."
 authors = ["Adam Hendel <adam@coredb.io>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "coredb_pgmq_python"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/CoreDB-io/coredb"
-"Repository" = "https://github.com/CoreDB-io/coredb/tree/main/extensions/pgmq/coredb-pgmq-python"
-"Documentation" = "https://github.com/CoreDB-io/coredb/tree/main/extensions/pgmq/coredb-pgmq-python"
+"Repository" = "https://github.com/CoreDB-io/coredb/tree/main/pgmq/coredb-pgmq-python"
+"Documentation" = "https://github.com/CoreDB-io/coredb/tree/main/pgmq/coredb-pgmq-python"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 psycopg = {extras = ["binary", "pool"], version = "^3.1.8"}
 pydantic = "^1.10.7"
 orjson = "^3.8.10"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "1.1.1"
+pandas = "^2.0.1"
 pytest = "^7.3.0"
 debugpy = "^1.6.7"
 black = "^23.3.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
+numpy = "^1.24.3"
 
 [tool.black]
 line-length = 120
 target-version = ['py311', 'py310', 'py39']
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `coredb_pgmq_python-0.2.0/setup.py` & `coredb_pgmq_python-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['orjson>=3.8.10,<4.0.0',
  'psycopg[binary,pool]>=3.1.8,<4.0.0',
  'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'coredb-pgmq-python',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Python client for the PGMQ Postgres extension.',
     'long_description': '# Coredb\'s Python Client for PGMQ\n\n## Installation\n\nInstall with `pip` from pypi.org\n\n```bash\npip install coredb-pgmq-python\n```\n\nDependencies:\n\nPostgres running the [CoreDB PGMQ extension](https://github.com/CoreDB-io/coredb/tree/main/extensions/pgmq).\n\n## Usage\n\n## Start a Postgres Instance with the CoreDB extension installed\n\n```bash\ndocker run -d --name postgres -e POSTGRES_PASSWORD=postgres -p 5432:5432 quay.io/coredb/pgmq-pg:latest\n```\n\nInitialize a connection to Postgres\n\n```python\n\nfrom coredb_pgmq_python import PGMQueue, Message\n\nqueue = PGMQueue(host="0.0.0.0")\n```\n\nCreate a queue (or a partitioned queue)\n\n```python\nqueue.create_queue("my_queue")\n# queue.create_partitioned_queue("my_partitioned_queue", partition_size=10000)\n```\n\n\nSend a message\n\n```python\nmsg_id: int = queue.send("my_queue", {"hello": "world"})\n```\n\nRead a message, set it invisible for 30 seconds.\n\n```python\nread_message: Message = queue.read("my_queue", vt=10)\nprint(read_message)\n```\n\nArchive the message after we\'re done with it. Archived messages are moved to an archive table.\n\n```python\narchived: bool = queue.archive("my_queue", read_message.msg_id)\n```\n\nDelete a message completely.\n\n```python\nmsg_id: int = queue.send("my_queue", {"hello": "world"})\nread_message: Message = queue.read("my_queue")\ndeleted: bool = queue.delete("my_queue", read_message.msg_id)\n```\n\nPop a message, deleting it and reading it in one transaction.\n\n```python\npopped_message: Message = queue.pop("my_queue")\nprint(popped_message)\n```\n',
     'author': 'Adam Hendel',
     'author_email': 'adam@coredb.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `coredb_pgmq_python-0.2.0/PKG-INFO` & `coredb_pgmq_python-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: coredb-pgmq-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python client for the PGMQ Postgres extension.
 License: Apache 2.0
 Author: Adam Hendel
 Author-email: adam@coredb.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: orjson (>=3.8.10,<4.0.0)
 Requires-Dist: psycopg[binary,pool] (>=3.1.8,<4.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Project-URL: Documentation, https://github.com/CoreDB-io/coredb/tree/main/extensions/pgmq/coredb-pgmq-python
+Project-URL: Documentation, https://github.com/CoreDB-io/coredb/tree/main/pgmq/coredb-pgmq-python
 Project-URL: Homepage, https://github.com/CoreDB-io/coredb
-Project-URL: Repository, https://github.com/CoreDB-io/coredb/tree/main/extensions/pgmq/coredb-pgmq-python
+Project-URL: Repository, https://github.com/CoreDB-io/coredb/tree/main/pgmq/coredb-pgmq-python
 Description-Content-Type: text/markdown
 
 # Coredb's Python Client for PGMQ
 
 ## Installation
 
 Install with `pip` from pypi.org
```

