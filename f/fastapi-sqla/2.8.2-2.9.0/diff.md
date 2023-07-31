# Comparing `tmp/fastapi_sqla-2.8.2.tar.gz` & `tmp/fastapi_sqla-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_sqla-2.8.2.tar", max compression
+gzip compressed data, was "fastapi_sqla-2.9.0.tar", max compression
```

## Comparing `fastapi_sqla-2.8.2.tar` & `fastapi_sqla-2.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-05-05 20:16:56.369780 fastapi_sqla-2.8.2/LICENSE
--rw-r--r--   0        0        0    13673 2023-05-05 20:16:56.369780 fastapi_sqla-2.8.2/README.md
--rw-r--r--   0        0        0     1466 2023-05-05 20:16:56.369780 fastapi_sqla-2.8.2/fastapi_sqla/__init__.py
--rw-r--r--   0        0        0     5549 2023-05-05 20:16:56.369780 fastapi_sqla-2.8.2/fastapi_sqla/_pytest_plugin.py
--rw-r--r--   0        0        0     6604 2023-05-05 20:16:56.369780 fastapi_sqla-2.8.2/fastapi_sqla/asyncio_support.py
--rw-r--r--   0        0        0      855 2023-05-05 20:16:56.369780 fastapi_sqla-2.8.2/fastapi_sqla/aws_aurora_support.py
--rw-r--r--   0        0        0     1106 2023-05-05 20:16:56.369780 fastapi_sqla-2.8.2/fastapi_sqla/aws_rds_iam_support.py
--rw-r--r--   0        0        0        0 2023-05-05 20:16:56.369780 fastapi_sqla-2.8.2/fastapi_sqla/py.typed
--rw-r--r--   0        0        0    10317 2023-05-05 20:16:56.369780 fastapi_sqla-2.8.2/fastapi_sqla/sqla.py
--rw-r--r--   0        0        0     5013 2023-05-05 20:16:56.369780 fastapi_sqla-2.8.2/pyproject.toml
--rw-r--r--   0        0        0    15870 1970-01-01 00:00:00.000000 fastapi_sqla-2.8.2/setup.py
--rw-r--r--   0        0        0    16960 1970-01-01 00:00:00.000000 fastapi_sqla-2.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-31 13:44:41.972012 fastapi_sqla-2.9.0/LICENSE
+-rw-r--r--   0        0        0    13679 2023-07-31 13:44:41.972012 fastapi_sqla-2.9.0/README.md
+-rw-r--r--   0        0        0     1486 2023-07-31 13:44:41.972012 fastapi_sqla-2.9.0/fastapi_sqla/__init__.py
+-rw-r--r--   0        0        0     5549 2023-07-31 13:44:41.972012 fastapi_sqla-2.9.0/fastapi_sqla/_pytest_plugin.py
+-rw-r--r--   0        0        0     6604 2023-07-31 13:44:41.972012 fastapi_sqla-2.9.0/fastapi_sqla/asyncio_support.py
+-rw-r--r--   0        0        0      838 2023-07-31 13:44:41.972012 fastapi_sqla-2.9.0/fastapi_sqla/aws_aurora_support.py
+-rw-r--r--   0        0        0     1090 2023-07-31 13:44:41.972012 fastapi_sqla-2.9.0/fastapi_sqla/aws_rds_iam_support.py
+-rw-r--r--   0        0        0        0 2023-07-31 13:44:41.972012 fastapi_sqla-2.9.0/fastapi_sqla/py.typed
+-rw-r--r--   0        0        0    10528 2023-07-31 13:44:41.972012 fastapi_sqla-2.9.0/fastapi_sqla/sqla.py
+-rw-r--r--   0        0        0     5134 2023-07-31 13:44:41.976012 fastapi_sqla-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0    15864 1970-01-01 00:00:00.000000 fastapi_sqla-2.9.0/setup.py
+-rw-r--r--   0        0        0    16967 1970-01-01 00:00:00.000000 fastapi_sqla-2.9.0/PKG-INFO
```

### Comparing `fastapi_sqla-2.8.2/LICENSE` & `fastapi_sqla-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_sqla-2.8.2/README.md` & `fastapi_sqla-2.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     if user is None:
         raise HTTPException(404)
     return {"data": user}
 
 
 @app.post("/users", response_model=Item[UserModel])
 def create_user(new_user: UserIn, session: Session = Depends()):
-    user = User(**new_user.dict())
+    user = User(**new_user.model_dump())
     session.add(user)
     try:
         session.flush()
     except IntegrityError:
         raise HTTPException(409, "Email is already taken.")
     return {"data": user}
 ```
```

### Comparing `fastapi_sqla-2.8.2/fastapi_sqla/__init__.py` & `fastapi_sqla-2.9.0/fastapi_sqla/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         "AsyncPaginate",
         "AsyncPagination",
         "AsyncSession",
         "open_async_session",
     ]
     has_asyncio_support = True
 
-except ImportError as err:
+except ImportError as err:  # pragma: no cover
     has_asyncio_support = False
     asyncio_support_err = str(err)
 
 
 def setup(app: FastAPI):
     engine = sqla.new_engine()
```

### Comparing `fastapi_sqla-2.8.2/fastapi_sqla/_pytest_plugin.py` & `fastapi_sqla-2.9.0/fastapi_sqla/_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqla-2.8.2/fastapi_sqla/asyncio_support.py` & `fastapi_sqla-2.9.0/fastapi_sqla/asyncio_support.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqla-2.8.2/fastapi_sqla/aws_aurora_support.py` & `fastapi_sqla-2.9.0/fastapi_sqla/aws_aurora_support.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,28 @@
-from pydantic import BaseSettings
+from os import environ
+
 from sqlalchemy import event
 from sqlalchemy.engine import Engine
 from sqlalchemy.engine.interfaces import ExceptionContext
 
 # Taken from
 # https://www.postgresql.org/docs/current/errcodes-appendix.html#ERRCODES-TABLE
 READONLY_ERROR_CODE = "25006"
 
 
 def setup(engine: Engine):
-    config = Config()
+    lc_environ = {k.lower(): v for k, v in environ.items()}
+    aws_aurora_enabled = lc_environ.get("fastapi_sqla_aws_aurora_enabled") == "true"
 
-    if not config.aws_aurora_enabled:
+    if not aws_aurora_enabled:
         return
 
     event.listen(engine, "handle_error", disconnect_on_readonly_error)
 
 
 def disconnect_on_readonly_error(context: ExceptionContext):
     if context.is_disconnect:
         return
 
     error_code = getattr(context.original_exception, "pgcode", None)
     if error_code == READONLY_ERROR_CODE:
         context.is_disconnect = True  # type: ignore
-
-
-class Config(BaseSettings):
-    aws_aurora_enabled: bool = False
-
-    class Config:
-        env_prefix = "fastapi_sqla_"
```

### Comparing `fastapi_sqla-2.8.2/fastapi_sqla/aws_rds_iam_support.py` & `fastapi_sqla-2.9.0/fastapi_sqla/aws_rds_iam_support.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
+from os import environ
+
 try:
     import boto3
 
     boto3_installed = True
 except ImportError as err:
     boto3_installed = False
     boto3_installed_err = str(err)
 
 from functools import lru_cache
 
-from pydantic import BaseSettings
 from sqlalchemy import event
 
 
 def setup(engine):
-    config = Config()
+    lc_environ = {k.lower(): v for k, v in environ.items()}
+    aws_rds_iam_enabled = lc_environ.get("fastapi_sqla_aws_rds_iam_enabled") == "true"
 
-    if config.aws_rds_iam_enabled:
+    if aws_rds_iam_enabled:
         assert boto3_installed, boto3_installed_err
         # Cache the client at startup
         get_rds_client()
         event.listen(engine, "do_connect", set_connection_token)
 
 
 @lru_cache
@@ -34,14 +36,7 @@
     return token
 
 
 def set_connection_token(dialect, conn_rec, cargs, cparams):
     cparams["password"] = get_authentication_token(
         host=cparams["host"], port=cparams.get("port", 5432), user=cparams["user"]
     )
-
-
-class Config(BaseSettings):
-    aws_rds_iam_enabled: bool = False
-
-    class Config:
-        env_prefix = "fastapi_sqla_"
```

### Comparing `fastapi_sqla-2.8.2/fastapi_sqla/sqla.py` & `fastapi_sqla-2.9.0/fastapi_sqla/sqla.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Generic, Iterator, Optional, TypeVar, Union, cast
 
 import structlog
 from fastapi import Depends, Query, Request
 from fastapi.concurrency import contextmanager_in_threadpool
 from fastapi.responses import PlainTextResponse
 from pydantic import BaseModel, Field
-from pydantic.generics import GenericModel
+from pydantic import __version__ as pydantic_version
 from sqlalchemy import engine_from_config, text
 from sqlalchemy.engine import Engine
 from sqlalchemy.ext.declarative import DeferredReflection
 from sqlalchemy.orm import Query as LegacyQuery
 from sqlalchemy.orm.session import Session as SqlaSession
 from sqlalchemy.orm.session import sessionmaker
 from sqlalchemy.sql import Select, func, select
@@ -25,14 +25,21 @@
 try:
     from sqlalchemy.orm import DeclarativeBase
 except ImportError:
     from sqlalchemy.ext.declarative import declarative_base
 
     DeclarativeBase = declarative_base()  # type: ignore
 
+major, _, _ = [int(v) for v in pydantic_version.split(".")]
+is_pydantic2 = major == 2
+if is_pydantic2:
+    GenericModel = BaseModel
+
+else:
+    from pydantic.generics import GenericModel  # type:ignore
 
 logger = structlog.get_logger(__name__)
 
 _SESSION_KEY = "fastapi_sqla_session"
 
 _Session = sessionmaker()
```

### Comparing `fastapi_sqla-2.8.2/pyproject.toml` & `fastapi_sqla-2.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-sqla"
-version = "2.8.2"
+version = "2.9.0"
 description = "SQLAlchemy extension for FastAPI with support for pagination, asyncio, and pytest, ready for production."
 authors = [
     "Hadrien David <hadrien.david@dialogue.co>",
     "Victor Repkow <victor.repkow@dialogue.co>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -38,15 +38,15 @@
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 fastapi = ">=0.61"
-pydantic = "<2"
+pydantic = ">=1"
 sqlalchemy = ">=1.3"
 structlog = ">=20"
 
 alembic = { version = "^1.4.3", optional = true}
 asgi_lifespan = { version = "^1.0.1", optional = true}
 asyncpg = {version = "^0.25.0", optional = true}
 black = {version = "^22.8.0", optional = true}
@@ -58,15 +58,15 @@
 pylama = {version = "^8.4.1", optional = true}
 pytest = {version = "^7.2.1", optional = true}
 pytest-asyncio = {version = "^0.19.0", optional = true}
 pytest-cov = { version = "^2.10.1", optional = true}
 tox = {version = "^3.26.0", optional = true}
 boto3 = {version = "^1.24.74", optional = true}
 greenlet = {version = "^1.1.3", optional = true}
-mypy = {version = "^0.991", extras = ["tests"]}
+mypy = {version = "^0.991", extras = ["tests"], optional = true}
 
 [tool.poetry.extras]
 # Test dependencies as extras so they can be set as extras in tox config
 # More info on https://github.com/python-poetry/poetry/issues/1941
 tests = [
     "alembic",
     "asgi_lifespan",
@@ -146,27 +146,31 @@
 
 [tool.coverage.report]
 skip_covered = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-isolated_build = True
-envlist = sqlalchemy{ 1.3, 1.4, 2.0 }-{ asyncpg, noasyncpg }-{aws_rds_iam, noaws_rds_iam }
+envlist = sqlalchemy{ 1.3, 1.4, 2.0 }-{ asyncpg, noasyncpg }-{aws_rds_iam, noaws_rds_iam }-pydantic{ 1.10, 2.0, 2.1 }
 
 [testenv]
 passenv = CI
 deps =
     sqlalchemy1.3: sqlalchemy<1.4
     sqlalchemy1.4: sqlalchemy>=1.4,<2
     sqlalchemy2.0: sqlalchemy>=2
     asyncpg: asyncpg
     aws_rds_iam: boto3
+    pydantic1.10: pydantic<2
+    pydantic2.0: pydantic>1.10,<2.1
+    pydantic2.1: pydantic>=2.1
+
 extras =
     tests
+
 commands = pytest -vv --cov={envsitepackagesdir}/fastapi_sqla --cov-report xml --cov-report html --junitxml=test-reports/pytest/junit.xml
 """
 
 [tool.black]
 exclude = ".mypy_cache|.pytest_cache|.vscode|.eggs|venv"
 --skip-magic-trailing-comma = true
```

### Comparing `fastapi_sqla-2.8.2/setup.py` & `fastapi_sqla-2.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,43 +4,43 @@
 packages = \
 ['fastapi_sqla']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fastapi>=0.61', 'pydantic<2', 'sqlalchemy>=1.3', 'structlog>=20']
+['fastapi>=0.61', 'pydantic>=1', 'sqlalchemy>=1.3', 'structlog>=20']
 
 extras_require = \
-{':extra == "tests"': ['mypy[tests]>=0.991,<0.992'],
- 'asyncpg': ['asyncpg>=0.25.0,<0.26.0'],
+{'asyncpg': ['asyncpg>=0.25.0,<0.26.0'],
  'aws-rds-iam': ['boto3>=1.24.74,<2.0.0'],
  'tests': ['alembic>=1.4.3,<2.0.0',
            'asgi_lifespan>=1.0.1,<2.0.0',
            'black>=22.8.0,<23.0.0',
            'Faker>=14.2.0,<15.0.0',
            'httpx>=0.23.0,<0.24.0',
            'isort>=5.5.3,<6.0.0',
            'pdbpp>=0.10.2,<0.11.0',
            'psycopg2>=2.8.6,<3.0.0',
            'pylama>=8.4.1,<9.0.0',
            'pytest>=7.2.1,<8.0.0',
            'pytest-asyncio>=0.19.0,<0.20.0',
            'pytest-cov>=2.10.1,<3.0.0',
            'tox>=3.26.0,<4.0.0',
-           'greenlet>=1.1.3,<2.0.0']}
+           'greenlet>=1.1.3,<2.0.0',
+           'mypy[tests]>=0.991,<0.992']}
 
 entry_points = \
 {'pytest11': ['fastapi-sqla = fastapi_sqla._pytest_plugin']}
 
 setup_kwargs = {
     'name': 'fastapi-sqla',
-    'version': '2.8.2',
+    'version': '2.9.0',
     'description': 'SQLAlchemy extension for FastAPI with support for pagination, asyncio, and pytest, ready for production.',
-    'long_description': '# Fastapi-SQLA\n\n[![codecov](https://codecov.io/gh/dialoguemd/fastapi-sqla/branch/master/graph/badge.svg?token=BQHLryClIn)](https://codecov.io/gh/dialoguemd/fastapi-sqla)\n[![CircleCI](https://dl.circleci.com/status-badge/img/gh/dialoguemd/fastapi-sqla/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/dialoguemd/fastapi-sqla/tree/master)\n![PyPI](https://img.shields.io/pypi/v/fastapi-sqla)\n[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-brightgreen.svg)](https://conventionalcommits.org)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n\nFastapi-SQLA is an [SQLAlchemy] extension for [FastAPI] easy to setup with support for\npagination, asyncio, and [pytest].\nIt supports SQLAlchemy>=1.3 and is fully compliant with [SQLAlchemy 2.0].\nIt is developped, maintained and used on production by the team at [@dialoguemd] with\nlove from Montreal 🇨🇦.\n\n# Installing\n\nUsing [pip](https://pip.pypa.io/):\n```\npip install fastapi-sqla\n```\n\n# Quick Example\n\nAssuming it runs against a DB with a table `user` with 3 columns, `id`, `name` and\nunique `email`:\n\n```python\n# main.py\nfrom fastapi import Depends, FastAPI, HTTPException\nfrom fastapi_sqla import Base, Item, Page, Paginate, Session, setup\nfrom pydantic import BaseModel, EmailStr\nfrom sqlalchemy import select\nfrom sqlalchemy.exc import IntegrityError\n\napp = FastAPI()\n\nsetup(app)\n\n\nclass User(Base):\n    __tablename__ = "user"\n\n\nclass UserIn(BaseModel):\n    name: str\n    email: EmailStr\n\n\nclass UserModel(UserIn):\n    id: int\n\n    class Config:\n        orm_mode = True\n\n\n@app.get("/users", response_model=Page[UserModel])\ndef list_users(paginate: Paginate = Depends()):\n    return paginate(select(User))\n\n\n@app.get("/users/{user_id}", response_model=Item[UserModel])\ndef get_user(user_id: int, session: Session = Depends()):\n    user = session.get(User, user_id)\n    if user is None:\n        raise HTTPException(404)\n    return {"data": user}\n\n\n@app.post("/users", response_model=Item[UserModel])\ndef create_user(new_user: UserIn, session: Session = Depends()):\n    user = User(**new_user.dict())\n    session.add(user)\n    try:\n        session.flush()\n    except IntegrityError:\n        raise HTTPException(409, "Email is already taken.")\n    return {"data": user}\n```\n\nCreating a db using `sqlite3`:\n```bash\nsqlite3 db.sqlite <<EOF\nCREATE TABLE user (\n    id    INTEGER PRIMARY KEY AUTOINCREMENT,\n    email TEXT NOT NULL,\n    name  TEXT NOT NULL\n);\nCREATE UNIQUE INDEX user_email_idx ON user (email);\nEOF\n```\n\nRunning the app:\n```bash\nsqlalchemy_url=sqlite:///db.sqlite?check_same_thread=false uvicorn main:app\n```\n\n# Configuration\n\n## Environment variables:\n\nThe keys of interest in `os.environ` are prefixed with `sqlalchemy_`.\nEach matching key (after the prefix is stripped) is treated as though it were the\ncorresponding keyword argument to [`sqlalchemy.create_engine`]\ncall.\n\nThe only required key is `sqlalchemy_url`, which provides the database URL, example:\n\n```bash\nexport sqlalchemy_url=postgresql://postgres@localhost\n```\n\n### `asyncio` support using [`asyncpg`]\n\nSQLAlchemy `>= 1.4` supports `asyncio`.\nTo enable `asyncio` support against a Postgres DB, install `asyncpg`:\n\n```bash\npip install asyncpg\n```\n\nAnd define environment variable `sqlalchemy_url` with `postgres+asyncpg` scheme:\n\n```bash\nexport sqlalchemy_url=postgresql+asyncpg://postgres@localhost\n```\n\n## Setup the app:\n\n```python\nimport fastapi_sqla\nfrom fastapi import FastAPI\n\napp = FastAPI()\nfastapi_sqla.setup(app)\n```\n\n# SQLAlchemy\n\n## Adding a new entity class:\n\n```python\nfrom fastapi_sqla import Base\n\n\nclass Entity(Base):\n    __tablename__ = "table-name-in-db"\n```\n\n## Getting an sqla session\n\n### Using dependency injection\n\nUse [FastAPI dependency injection] to get a session as a parameter of a path operation\nfunction.\nSQLAlchemy session is committed before response is returned or rollbacked if any\nexception occurred:\n\n```python\nfrom fastapi import APIRouter, Depends\nfrom fastapi_sqla import Session\nfrom fastapi_sqla.asyncio_support import AsyncSession\n\nrouter = APIRouter()\n\n\n@router.get("/example")\ndef example(session: Session = Depends()):\n    return session.execute("SELECT now()").scalar()\n\n\n@router.get("/async_example")\nasync def async_example(session: AsyncSession = Depends()):\n    return await session.scalar("SELECT now()")\n```\n\n### Using a context manager\n\nWhen needing a session outside of a path operation, like when using\n[FastAPI background tasks], use `fastapi_sqla.open_session` context manager.\nSQLAlchemy session is committed when exiting context or rollbacked if any exception\noccurred:\n\n```python\nfrom fastapi import APIRouter, BackgroundTasks\nfrom fastapi_sqla import open_session\nfrom fastapi_sqla import asyncio_support\n\nrouter = APIRouter()\n\n\n@router.get("/example")\ndef example(bg: BackgroundTasks):\n    bg.add_task(run_bg)\n    bg.add_task(run_async_bg)\n\n\ndef run_bg():\n    with open_session() as session:\n        session.execute("SELECT now()").scalar()\n\n\nasync def run_async_bg():\n    async with asyncio_support.open_session() as session:\n        await session.scalar("SELECT now()")\n```\n\n## Pagination\n\n```python\nfrom fastapi import APIRouter, Depends\nfrom fastapi_sqla import Base, Page, Paginate\nfrom pydantic import BaseModel\nfrom sqlalchemy import select\n\nrouter = APIRouter()\n\n\nclass User(Base):\n    __tablename__ = "user"\n\n\nclass UserModel(BaseModel):\n    id: int\n    name: str\n\n    class Config:\n        orm_mode = True\n\n\n@router.get("/users", response_model=Page[UserModel])\ndef all_users(paginate: Paginate = Depends()):\n    return paginate(select(User))\n```\n\nBy default:\n\n* It returns pages of 10 items, up to 100 items;\n* Total number of items in the collection is queried using [`Query.count`].\n* Response example for `/users?offset=40&limit=10`:\n\n    ```json\n    {\n        "data": [\n            {\n                "id": 41,\n                "name": "Pat Thomas"\n            },\n            {\n                "id": 42,\n                "name": "Mulatu Astatke"\n            }\n        ],\n        "meta": {\n            "offset": 40,\n            "total_items": 42,\n            "total_pages": 5,\n            "page_number": 5\n        }\n    }\n    ```\n\n### Paginating non-scalar results\n\nTo paginate a query which doesn\'t return [scalars], specify `scalars=False` when invoking\n`paginate`:\n\n```python\nfrom fastapi import APIRouter, Depends\nfrom fastapi_sqla import Base, Page, Paginate\nfrom pydantic import BaseModel\nfrom sqlalchemy import func, select\nfrom sqlalchemy.orm import relationship\n\nrouter = APIRouter()\n\n\nclass User(Base):\n    __tablename__ = "user"\n    notes = relationship("Note")\n\n\nclass Note(Base):\n    __tablename__ = "note"\n\n\nclass UserModel(BaseModel):\n    id: int\n    name: str\n    notes_count: int\n\n\n@router.get("/users", response_model=Page[UserModel])\ndef all_users(paginate: Paginate = Depends()):\n    query = (\n        select(User.id, User.name, func.count(Note.id).label("notes_count"))\n        .join(Note)\n        .group_by(User)\n    )\n    return paginate(query, scalars=False)\n```\n\n\n### Customize pagination\n\nYou can customize:\n- Minimum and maximum number of items per pages;\n- How the total number of items in the collection is queried;\n\nTo customize pagination, create a dependency using `fastapi_sqla.Pagination`:\n\n```python\nfrom fastapi import APIRouter, Depends\nfrom fastapi_sqla import Base, Page, Pagination, Session\nfrom pydantic import BaseModel\nfrom sqlalchemy import func, select\n\nrouter = APIRouter()\n\n\nclass User(Base):\n    __tablename__ = "user"\n\n\nclass UserModel(BaseModel):\n    id: int\n    name: str\n\n\ndef query_count(session: Session = Depends()) -> int:\n    return session.execute(select(func.count()).select_from(User)).scalar()\n\n\nPaginate = Pagination(min_page_size=5, max_page_size=500, query_count=query_count)\n\n\n@router.get("/users", response_model=Page[UserModel])\ndef all_users(paginate: Paginate = Depends()):\n    return paginate(select(User))\n```\n\n### Async pagination\n\nWhen using the asyncio support, use the `AsyncPaginate` dependency:\n\n```python\nfrom fastapi import APIRouter, Depends\nfrom fastapi_sqla import Base, Page, AsyncPaginate\nfrom pydantic import BaseModel\nfrom sqlalchemy import select\n\nrouter = APIRouter()\n\n\nclass User(Base):\n    __tablename__ = "user"\n\n\nclass UserModel(BaseModel):\n    id: int\n    name: str\n\n    class Config:\n        orm_mode = True\n\n\n@router.get("/users", response_model=Page[UserModel])\nasync def all_users(paginate: AsyncPaginate = Depends()):\n    return await paginate(select(User))\n```\n\nCustomize pagination by creating a dependency using `fastapi_sqla.AsyncPagination`:\n\n```python\nfrom fastapi import APIRouter, Depends\nfrom fastapi_sqla import Base, Page, AsyncPagination, AsyncSession\nfrom pydantic import BaseModel\nfrom sqlalchemy import func, select\n\nrouter = APIRouter()\n\n\nclass User(Base):\n    __tablename__ = "user"\n\n\nclass UserModel(BaseModel):\n    id: int\n    name: str\n\n\nasync def query_count(session: AsyncSession = Depends()) -> int:\n    result = await session.execute(select(func.count()).select_from(User))\n    return result.scalar()\n\n\nPaginate = AsyncPagination(min_page_size=5, max_page_size=500, query_count=query_count)\n\n\n@router.get("/users", response_model=Page[UserModel])\ndef all_users(paginate: CustomPaginate = Depends()):\n    return await paginate(select(User))\n```\n\n# Pytest fixtures\n\nThis library provides a set of utility fixtures, through its PyTest plugin, which is\nautomatically installed with the library.\n\nBy default, no records are actually written to the database when running tests.\nThere currently is no way to change this behaviour.\n\n## `sqla_modules`\n\nYou must define this fixture, in order for the plugin to reflect table metadata in your\nSQLAlchemy entities. It should just import all of the application\'s modules which contain\nSQLAlchemy models.\n\nExample:\n\n```python\n# tests/conftest.py\nfrom pytest import fixture\n\n\n@fixture\ndef sqla_modules():\n    from app import sqla  # noqa\n```\n\n## `db_url`\n\nThe DB url to use.\n\nWhen `CI` key is set in environment variables, it defaults to using `postgres` as the\nhost name:\n\n```\npostgresql://postgres@postgres/postgres\n```\n\nIn other cases, the host is set to `localhost`:\n\n```\npostgresql://postgres@localhost/postgres\n```\n\nOf course, you can override it by overloading the fixture:\n\n```python\nfrom pytest import fixture\n\n\n@fixture(scope="session")\ndef db_url():\n    return "postgresql://postgres@localhost/test_database"\n```\n\n## `async_sqlalchemy_url`\n\nDB url to use when using `asyncio` support. Defaults to `db_url` fixture with\n`postgresql+asyncpg://` scheme.\n\n\n## `session` & `async_session`\n\nSqla sessions to create db fixture:\n* All changes done at test setup or during the test are rollbacked at test tear down;\n* No record will actually be written in the database;\n* Changes in one regular session need to be committed to be available from other regular\n  sessions;\n* Changes in one async session need to be committed to be available from other async\n  sessions;\n* Changes from regular sessions are not available from `async` session and vice-versa\n  even when committed;\n\nExample:\n```python\nfrom pytest import fixture\n\n\n@fixture\ndef patient(session):\n    from er.sqla import Patient\n    patient = Patient(first_name="Bob", last_name="David")\n    session.add(patient)\n    session.commit()\n    return patient\n\n\n@fixture\nasync def doctor(async_session):\n    from er.sqla import Doctor\n    doctor = Doctor(name="who")\n    async_session.add(doctor)\n    await async_session.commit()\n    return doctor\n```\n\n## `db_migration`\n\nA session scope fixture that runs `alembic upgrade` at test session setup and\n`alembic downgrade` at tear down.\n\nIt depends on `alembic_ini_path` fixture to get the path of `alembic.ini` file.\n\nTo use in a test or test module:\n\n```python\nfrom pytest import mark\n\npytestmark = mark.usefixtures("db_migration")\n```\n\nTo use globally, add to [pytest options]:\n\n ```ini\n [pytest]\n usefixtures =\n     db_migration\n ```\n\nOr depends on it in top-level `conftest.py` and mark it as _auto-used_:\n\n```python\nfrom pytest import fixture\n\n\n@fixture(scope="session", autouse=True)\ndef db_migration(db_migration):\n    pass\n```\n\n## `alembic_ini_path`\n\nIt returns the path of  `alembic.ini` configuration file. By default, it returns\n`./alembic.ini`.\n\n\n# Development\n\n## Prerequisites\n\n- **Python >=3.9**\n- [**Poetry**](https://poetry.eustace.io/) to install package dependencies.\n- A postgres DB reachable at `postgresql://postgres@localhost/postgres`\n\n\n## Setup\n\n```bash\n$ poetry install --extras tests --extras asyncpg --extras aws_rds_iam\n```\n\n## Running tests\n\n```bash\n$ poetry run pytest\n```\n\n#### Runing tests on multiple environments\n\n```bash\n$ poetry run tox\n```\n\n[`sqlalchemy.create_engine`]: https://docs.sqlalchemy.org/en/20/core/engines.html#sqlalchemy.create_engine\n[`Query.count`]: https://docs.sqlalchemy.org/en/20/orm/queryguide/query.html#sqlalchemy.orm.Query.count\n[pytest options]: https://docs.pytest.org/en/stable/reference.html#confval-usefixtures\n[FastAPI]: https://fastapi.tiangolo.com/\n[FastAPI dependency injection]: https://fastapi.tiangolo.com/tutorial/dependencies/\n[FastAPI background tasks]: https://fastapi.tiangolo.com/tutorial/background-tasks/\n[SQLAlchemy]: http://sqlalchemy.org/\n[SQLAlchemy 2.0]: https://docs.sqlalchemy.org/en/20/changelog/migration_20.html\n[`asyncpg`]: https://magicstack.github.io/asyncpg/current/\n[scalars]: https://docs.sqlalchemy.org/en/20/core/connections.html#sqlalchemy.engine.Result.scalars\n[alembic]: https://alembic.sqlalchemy.org/\n[pytest]: https://docs.pytest.org/\n[@dialoguemd]: https://github.com/dialoguemd\n',
+    'long_description': '# Fastapi-SQLA\n\n[![codecov](https://codecov.io/gh/dialoguemd/fastapi-sqla/branch/master/graph/badge.svg?token=BQHLryClIn)](https://codecov.io/gh/dialoguemd/fastapi-sqla)\n[![CircleCI](https://dl.circleci.com/status-badge/img/gh/dialoguemd/fastapi-sqla/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/dialoguemd/fastapi-sqla/tree/master)\n![PyPI](https://img.shields.io/pypi/v/fastapi-sqla)\n[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-brightgreen.svg)](https://conventionalcommits.org)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n\nFastapi-SQLA is an [SQLAlchemy] extension for [FastAPI] easy to setup with support for\npagination, asyncio, and [pytest].\nIt supports SQLAlchemy>=1.3 and is fully compliant with [SQLAlchemy 2.0].\nIt is developped, maintained and used on production by the team at [@dialoguemd] with\nlove from Montreal 🇨🇦.\n\n# Installing\n\nUsing [pip](https://pip.pypa.io/):\n```\npip install fastapi-sqla\n```\n\n# Quick Example\n\nAssuming it runs against a DB with a table `user` with 3 columns, `id`, `name` and\nunique `email`:\n\n```python\n# main.py\nfrom fastapi import Depends, FastAPI, HTTPException\nfrom fastapi_sqla import Base, Item, Page, Paginate, Session, setup\nfrom pydantic import BaseModel, EmailStr\nfrom sqlalchemy import select\nfrom sqlalchemy.exc import IntegrityError\n\napp = FastAPI()\n\nsetup(app)\n\n\nclass User(Base):\n    __tablename__ = "user"\n\n\nclass UserIn(BaseModel):\n    name: str\n    email: EmailStr\n\n\nclass UserModel(UserIn):\n    id: int\n\n    class Config:\n        orm_mode = True\n\n\n@app.get("/users", response_model=Page[UserModel])\ndef list_users(paginate: Paginate = Depends()):\n    return paginate(select(User))\n\n\n@app.get("/users/{user_id}", response_model=Item[UserModel])\ndef get_user(user_id: int, session: Session = Depends()):\n    user = session.get(User, user_id)\n    if user is None:\n        raise HTTPException(404)\n    return {"data": user}\n\n\n@app.post("/users", response_model=Item[UserModel])\ndef create_user(new_user: UserIn, session: Session = Depends()):\n    user = User(**new_user.model_dump())\n    session.add(user)\n    try:\n        session.flush()\n    except IntegrityError:\n        raise HTTPException(409, "Email is already taken.")\n    return {"data": user}\n```\n\nCreating a db using `sqlite3`:\n```bash\nsqlite3 db.sqlite <<EOF\nCREATE TABLE user (\n    id    INTEGER PRIMARY KEY AUTOINCREMENT,\n    email TEXT NOT NULL,\n    name  TEXT NOT NULL\n);\nCREATE UNIQUE INDEX user_email_idx ON user (email);\nEOF\n```\n\nRunning the app:\n```bash\nsqlalchemy_url=sqlite:///db.sqlite?check_same_thread=false uvicorn main:app\n```\n\n# Configuration\n\n## Environment variables:\n\nThe keys of interest in `os.environ` are prefixed with `sqlalchemy_`.\nEach matching key (after the prefix is stripped) is treated as though it were the\ncorresponding keyword argument to [`sqlalchemy.create_engine`]\ncall.\n\nThe only required key is `sqlalchemy_url`, which provides the database URL, example:\n\n```bash\nexport sqlalchemy_url=postgresql://postgres@localhost\n```\n\n### `asyncio` support using [`asyncpg`]\n\nSQLAlchemy `>= 1.4` supports `asyncio`.\nTo enable `asyncio` support against a Postgres DB, install `asyncpg`:\n\n```bash\npip install asyncpg\n```\n\nAnd define environment variable `sqlalchemy_url` with `postgres+asyncpg` scheme:\n\n```bash\nexport sqlalchemy_url=postgresql+asyncpg://postgres@localhost\n```\n\n## Setup the app:\n\n```python\nimport fastapi_sqla\nfrom fastapi import FastAPI\n\napp = FastAPI()\nfastapi_sqla.setup(app)\n```\n\n# SQLAlchemy\n\n## Adding a new entity class:\n\n```python\nfrom fastapi_sqla import Base\n\n\nclass Entity(Base):\n    __tablename__ = "table-name-in-db"\n```\n\n## Getting an sqla session\n\n### Using dependency injection\n\nUse [FastAPI dependency injection] to get a session as a parameter of a path operation\nfunction.\nSQLAlchemy session is committed before response is returned or rollbacked if any\nexception occurred:\n\n```python\nfrom fastapi import APIRouter, Depends\nfrom fastapi_sqla import Session\nfrom fastapi_sqla.asyncio_support import AsyncSession\n\nrouter = APIRouter()\n\n\n@router.get("/example")\ndef example(session: Session = Depends()):\n    return session.execute("SELECT now()").scalar()\n\n\n@router.get("/async_example")\nasync def async_example(session: AsyncSession = Depends()):\n    return await session.scalar("SELECT now()")\n```\n\n### Using a context manager\n\nWhen needing a session outside of a path operation, like when using\n[FastAPI background tasks], use `fastapi_sqla.open_session` context manager.\nSQLAlchemy session is committed when exiting context or rollbacked if any exception\noccurred:\n\n```python\nfrom fastapi import APIRouter, BackgroundTasks\nfrom fastapi_sqla import open_session\nfrom fastapi_sqla import asyncio_support\n\nrouter = APIRouter()\n\n\n@router.get("/example")\ndef example(bg: BackgroundTasks):\n    bg.add_task(run_bg)\n    bg.add_task(run_async_bg)\n\n\ndef run_bg():\n    with open_session() as session:\n        session.execute("SELECT now()").scalar()\n\n\nasync def run_async_bg():\n    async with asyncio_support.open_session() as session:\n        await session.scalar("SELECT now()")\n```\n\n## Pagination\n\n```python\nfrom fastapi import APIRouter, Depends\nfrom fastapi_sqla import Base, Page, Paginate\nfrom pydantic import BaseModel\nfrom sqlalchemy import select\n\nrouter = APIRouter()\n\n\nclass User(Base):\n    __tablename__ = "user"\n\n\nclass UserModel(BaseModel):\n    id: int\n    name: str\n\n    class Config:\n        orm_mode = True\n\n\n@router.get("/users", response_model=Page[UserModel])\ndef all_users(paginate: Paginate = Depends()):\n    return paginate(select(User))\n```\n\nBy default:\n\n* It returns pages of 10 items, up to 100 items;\n* Total number of items in the collection is queried using [`Query.count`].\n* Response example for `/users?offset=40&limit=10`:\n\n    ```json\n    {\n        "data": [\n            {\n                "id": 41,\n                "name": "Pat Thomas"\n            },\n            {\n                "id": 42,\n                "name": "Mulatu Astatke"\n            }\n        ],\n        "meta": {\n            "offset": 40,\n            "total_items": 42,\n            "total_pages": 5,\n            "page_number": 5\n        }\n    }\n    ```\n\n### Paginating non-scalar results\n\nTo paginate a query which doesn\'t return [scalars], specify `scalars=False` when invoking\n`paginate`:\n\n```python\nfrom fastapi import APIRouter, Depends\nfrom fastapi_sqla import Base, Page, Paginate\nfrom pydantic import BaseModel\nfrom sqlalchemy import func, select\nfrom sqlalchemy.orm import relationship\n\nrouter = APIRouter()\n\n\nclass User(Base):\n    __tablename__ = "user"\n    notes = relationship("Note")\n\n\nclass Note(Base):\n    __tablename__ = "note"\n\n\nclass UserModel(BaseModel):\n    id: int\n    name: str\n    notes_count: int\n\n\n@router.get("/users", response_model=Page[UserModel])\ndef all_users(paginate: Paginate = Depends()):\n    query = (\n        select(User.id, User.name, func.count(Note.id).label("notes_count"))\n        .join(Note)\n        .group_by(User)\n    )\n    return paginate(query, scalars=False)\n```\n\n\n### Customize pagination\n\nYou can customize:\n- Minimum and maximum number of items per pages;\n- How the total number of items in the collection is queried;\n\nTo customize pagination, create a dependency using `fastapi_sqla.Pagination`:\n\n```python\nfrom fastapi import APIRouter, Depends\nfrom fastapi_sqla import Base, Page, Pagination, Session\nfrom pydantic import BaseModel\nfrom sqlalchemy import func, select\n\nrouter = APIRouter()\n\n\nclass User(Base):\n    __tablename__ = "user"\n\n\nclass UserModel(BaseModel):\n    id: int\n    name: str\n\n\ndef query_count(session: Session = Depends()) -> int:\n    return session.execute(select(func.count()).select_from(User)).scalar()\n\n\nPaginate = Pagination(min_page_size=5, max_page_size=500, query_count=query_count)\n\n\n@router.get("/users", response_model=Page[UserModel])\ndef all_users(paginate: Paginate = Depends()):\n    return paginate(select(User))\n```\n\n### Async pagination\n\nWhen using the asyncio support, use the `AsyncPaginate` dependency:\n\n```python\nfrom fastapi import APIRouter, Depends\nfrom fastapi_sqla import Base, Page, AsyncPaginate\nfrom pydantic import BaseModel\nfrom sqlalchemy import select\n\nrouter = APIRouter()\n\n\nclass User(Base):\n    __tablename__ = "user"\n\n\nclass UserModel(BaseModel):\n    id: int\n    name: str\n\n    class Config:\n        orm_mode = True\n\n\n@router.get("/users", response_model=Page[UserModel])\nasync def all_users(paginate: AsyncPaginate = Depends()):\n    return await paginate(select(User))\n```\n\nCustomize pagination by creating a dependency using `fastapi_sqla.AsyncPagination`:\n\n```python\nfrom fastapi import APIRouter, Depends\nfrom fastapi_sqla import Base, Page, AsyncPagination, AsyncSession\nfrom pydantic import BaseModel\nfrom sqlalchemy import func, select\n\nrouter = APIRouter()\n\n\nclass User(Base):\n    __tablename__ = "user"\n\n\nclass UserModel(BaseModel):\n    id: int\n    name: str\n\n\nasync def query_count(session: AsyncSession = Depends()) -> int:\n    result = await session.execute(select(func.count()).select_from(User))\n    return result.scalar()\n\n\nPaginate = AsyncPagination(min_page_size=5, max_page_size=500, query_count=query_count)\n\n\n@router.get("/users", response_model=Page[UserModel])\ndef all_users(paginate: CustomPaginate = Depends()):\n    return await paginate(select(User))\n```\n\n# Pytest fixtures\n\nThis library provides a set of utility fixtures, through its PyTest plugin, which is\nautomatically installed with the library.\n\nBy default, no records are actually written to the database when running tests.\nThere currently is no way to change this behaviour.\n\n## `sqla_modules`\n\nYou must define this fixture, in order for the plugin to reflect table metadata in your\nSQLAlchemy entities. It should just import all of the application\'s modules which contain\nSQLAlchemy models.\n\nExample:\n\n```python\n# tests/conftest.py\nfrom pytest import fixture\n\n\n@fixture\ndef sqla_modules():\n    from app import sqla  # noqa\n```\n\n## `db_url`\n\nThe DB url to use.\n\nWhen `CI` key is set in environment variables, it defaults to using `postgres` as the\nhost name:\n\n```\npostgresql://postgres@postgres/postgres\n```\n\nIn other cases, the host is set to `localhost`:\n\n```\npostgresql://postgres@localhost/postgres\n```\n\nOf course, you can override it by overloading the fixture:\n\n```python\nfrom pytest import fixture\n\n\n@fixture(scope="session")\ndef db_url():\n    return "postgresql://postgres@localhost/test_database"\n```\n\n## `async_sqlalchemy_url`\n\nDB url to use when using `asyncio` support. Defaults to `db_url` fixture with\n`postgresql+asyncpg://` scheme.\n\n\n## `session` & `async_session`\n\nSqla sessions to create db fixture:\n* All changes done at test setup or during the test are rollbacked at test tear down;\n* No record will actually be written in the database;\n* Changes in one regular session need to be committed to be available from other regular\n  sessions;\n* Changes in one async session need to be committed to be available from other async\n  sessions;\n* Changes from regular sessions are not available from `async` session and vice-versa\n  even when committed;\n\nExample:\n```python\nfrom pytest import fixture\n\n\n@fixture\ndef patient(session):\n    from er.sqla import Patient\n    patient = Patient(first_name="Bob", last_name="David")\n    session.add(patient)\n    session.commit()\n    return patient\n\n\n@fixture\nasync def doctor(async_session):\n    from er.sqla import Doctor\n    doctor = Doctor(name="who")\n    async_session.add(doctor)\n    await async_session.commit()\n    return doctor\n```\n\n## `db_migration`\n\nA session scope fixture that runs `alembic upgrade` at test session setup and\n`alembic downgrade` at tear down.\n\nIt depends on `alembic_ini_path` fixture to get the path of `alembic.ini` file.\n\nTo use in a test or test module:\n\n```python\nfrom pytest import mark\n\npytestmark = mark.usefixtures("db_migration")\n```\n\nTo use globally, add to [pytest options]:\n\n ```ini\n [pytest]\n usefixtures =\n     db_migration\n ```\n\nOr depends on it in top-level `conftest.py` and mark it as _auto-used_:\n\n```python\nfrom pytest import fixture\n\n\n@fixture(scope="session", autouse=True)\ndef db_migration(db_migration):\n    pass\n```\n\n## `alembic_ini_path`\n\nIt returns the path of  `alembic.ini` configuration file. By default, it returns\n`./alembic.ini`.\n\n\n# Development\n\n## Prerequisites\n\n- **Python >=3.9**\n- [**Poetry**](https://poetry.eustace.io/) to install package dependencies.\n- A postgres DB reachable at `postgresql://postgres@localhost/postgres`\n\n\n## Setup\n\n```bash\n$ poetry install --extras tests --extras asyncpg --extras aws_rds_iam\n```\n\n## Running tests\n\n```bash\n$ poetry run pytest\n```\n\n#### Runing tests on multiple environments\n\n```bash\n$ poetry run tox\n```\n\n[`sqlalchemy.create_engine`]: https://docs.sqlalchemy.org/en/20/core/engines.html#sqlalchemy.create_engine\n[`Query.count`]: https://docs.sqlalchemy.org/en/20/orm/queryguide/query.html#sqlalchemy.orm.Query.count\n[pytest options]: https://docs.pytest.org/en/stable/reference.html#confval-usefixtures\n[FastAPI]: https://fastapi.tiangolo.com/\n[FastAPI dependency injection]: https://fastapi.tiangolo.com/tutorial/dependencies/\n[FastAPI background tasks]: https://fastapi.tiangolo.com/tutorial/background-tasks/\n[SQLAlchemy]: http://sqlalchemy.org/\n[SQLAlchemy 2.0]: https://docs.sqlalchemy.org/en/20/changelog/migration_20.html\n[`asyncpg`]: https://magicstack.github.io/asyncpg/current/\n[scalars]: https://docs.sqlalchemy.org/en/20/core/connections.html#sqlalchemy.engine.Result.scalars\n[alembic]: https://alembic.sqlalchemy.org/\n[pytest]: https://docs.pytest.org/\n[@dialoguemd]: https://github.com/dialoguemd\n',
     'author': 'Hadrien David',
     'author_email': 'hadrien.david@dialogue.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dialoguemd/fastapi-sqla',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fastapi_sqla-2.8.2/PKG-INFO` & `fastapi_sqla-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sqla
-Version: 2.8.2
+Version: 2.9.0
 Summary: SQLAlchemy extension for FastAPI with support for pagination, asyncio, and pytest, ready for production.
 Home-page: https://github.com/dialoguemd/fastapi-sqla
 License: MIT
 Keywords: FastAPI,SQLAlchemy,asyncio,pytest,alembic
 Author: Hadrien David
 Author-email: hadrien.david@dialogue.co
 Requires-Python: >=3.7,<4.0
@@ -52,15 +52,15 @@
 Requires-Dist: fastapi (>=0.61)
 Requires-Dist: greenlet (>=1.1.3,<2.0.0) ; extra == "tests"
 Requires-Dist: httpx (>=0.23.0,<0.24.0) ; extra == "tests"
 Requires-Dist: isort (>=5.5.3,<6.0.0) ; extra == "tests"
 Requires-Dist: mypy[tests] (>=0.991,<0.992) ; extra == "tests"
 Requires-Dist: pdbpp (>=0.10.2,<0.11.0) ; extra == "tests"
 Requires-Dist: psycopg2 (>=2.8.6,<3.0.0) ; extra == "tests"
-Requires-Dist: pydantic (<2)
+Requires-Dist: pydantic (>=1)
 Requires-Dist: pylama (>=8.4.1,<9.0.0) ; extra == "tests"
 Requires-Dist: pytest (>=7.2.1,<8.0.0) ; extra == "tests"
 Requires-Dist: pytest-asyncio (>=0.19.0,<0.20.0) ; extra == "tests"
 Requires-Dist: pytest-cov (>=2.10.1,<3.0.0) ; extra == "tests"
 Requires-Dist: sqlalchemy (>=1.3)
 Requires-Dist: structlog (>=20)
 Requires-Dist: tox (>=3.26.0,<4.0.0) ; extra == "tests"
@@ -134,15 +134,15 @@
     if user is None:
         raise HTTPException(404)
     return {"data": user}
 
 
 @app.post("/users", response_model=Item[UserModel])
 def create_user(new_user: UserIn, session: Session = Depends()):
-    user = User(**new_user.dict())
+    user = User(**new_user.model_dump())
     session.add(user)
     try:
         session.flush()
     except IntegrityError:
         raise HTTPException(409, "Email is already taken.")
     return {"data": user}
 ```
```

