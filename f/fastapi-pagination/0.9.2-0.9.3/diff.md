# Comparing `tmp/fastapi-pagination-0.9.2.tar.gz` & `tmp/fastapi-pagination-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-pagination-0.9.2.tar", max compression
+gzip compressed data, was "fastapi-pagination-0.9.3.tar", max compression
```

## Comparing `fastapi-pagination-0.9.2.tar` & `fastapi-pagination-0.9.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1070 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/LICENSE
--rw-r--r--   0        0        0     2017 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/README.md
--rw-r--r--   0        0        0      461 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/__init__.py
--rw-r--r--   0        0        0     3986 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/api.py
--rw-r--r--   0        0        0     2512 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/bases.py
--rw-r--r--   0        0        0     1126 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/default.py
--rw-r--r--   0        0        0        0 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/ext/__init__.py
--rw-r--r--   0        0        0      851 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/ext/async_sqlalchemy.py
--rw-r--r--   0        0        0      961 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/ext/async_sqlmodel.py
--rw-r--r--   0        0        0      784 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/ext/asyncpg.py
--rw-r--r--   0        0        0      793 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/ext/databases.py
--rw-r--r--   0        0        0      733 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/ext/django.py
--rw-r--r--   0        0        0      787 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/ext/gino.py
--rw-r--r--   0        0        0      855 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/ext/mongoengine.py
--rw-r--r--   0        0        0     1713 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/ext/motor.py
--rw-r--r--   0        0        0      855 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/ext/orm.py
--rw-r--r--   0        0        0      620 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/ext/ormar.py
--rw-r--r--   0        0        0      967 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/ext/piccolo.py
--rw-r--r--   0        0        0        0 2022-04-09 14:07:24.721331 fastapi-pagination-0.9.2/fastapi_pagination/ext/py.typed
--rw-r--r--   0        0        0      870 2022-04-09 14:07:24.725331 fastapi-pagination-0.9.2/fastapi_pagination/ext/sqlalchemy.py
--rw-r--r--   0        0        0      783 2022-04-09 14:07:24.725331 fastapi-pagination-0.9.2/fastapi_pagination/ext/sqlalchemy_future.py
--rw-r--r--   0        0        0      857 2022-04-09 14:07:24.725331 fastapi-pagination-0.9.2/fastapi_pagination/ext/sqlmodel.py
--rw-r--r--   0        0        0     1147 2022-04-09 14:07:24.725331 fastapi-pagination-0.9.2/fastapi_pagination/ext/tortoise.py
--rw-r--r--   0        0        0     1083 2022-04-09 14:07:24.725331 fastapi-pagination-0.9.2/fastapi_pagination/iterables.py
--rw-r--r--   0        0        0     1201 2022-04-09 14:07:24.725331 fastapi-pagination-0.9.2/fastapi_pagination/limit_offset.py
--rw-r--r--   0        0        0       69 2022-04-09 14:07:24.725331 fastapi-pagination-0.9.2/fastapi_pagination/links/__init__.py
--rw-r--r--   0        0        0     1165 2022-04-09 14:07:24.725331 fastapi-pagination-0.9.2/fastapi_pagination/links/bases.py
--rw-r--r--   0        0        0      832 2022-04-09 14:07:24.725331 fastapi-pagination-0.9.2/fastapi_pagination/links/default.py
--rw-r--r--   0        0        0     1193 2022-04-09 14:07:24.725331 fastapi-pagination-0.9.2/fastapi_pagination/links/limmit_offset.py
--rw-r--r--   0        0        0      614 2022-04-09 14:07:24.725331 fastapi-pagination-0.9.2/fastapi_pagination/paginator.py
--rw-r--r--   0        0        0        0 2022-04-09 14:07:24.725331 fastapi-pagination-0.9.2/fastapi_pagination/py.typed
--rw-r--r--   0        0        0     2816 2022-04-09 14:07:24.725331 fastapi-pagination-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     3897 2022-04-09 14:07:33.785299 fastapi-pagination-0.9.2/setup.py
--rw-r--r--   0        0        0     4186 2022-04-09 14:07:33.785698 fastapi-pagination-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-04-16 13:55:31.768361 fastapi-pagination-0.9.3/LICENSE
+-rw-r--r--   0        0        0     2017 2022-04-16 13:55:31.768361 fastapi-pagination-0.9.3/README.md
+-rw-r--r--   0        0        0      461 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/__init__.py
+-rw-r--r--   0        0        0     4036 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/api.py
+-rw-r--r--   0        0        0     2512 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/bases.py
+-rw-r--r--   0        0        0     1126 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/default.py
+-rw-r--r--   0        0        0        0 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/__init__.py
+-rw-r--r--   0        0        0      851 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/async_sqlalchemy.py
+-rw-r--r--   0        0        0      961 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/async_sqlmodel.py
+-rw-r--r--   0        0        0      784 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/asyncpg.py
+-rw-r--r--   0        0        0      793 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/databases.py
+-rw-r--r--   0        0        0      733 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/django.py
+-rw-r--r--   0        0        0      787 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/gino.py
+-rw-r--r--   0        0        0      855 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/mongoengine.py
+-rw-r--r--   0        0        0     1713 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/motor.py
+-rw-r--r--   0        0        0      855 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/orm.py
+-rw-r--r--   0        0        0      620 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/ormar.py
+-rw-r--r--   0        0        0      967 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/piccolo.py
+-rw-r--r--   0        0        0        0 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/py.typed
+-rw-r--r--   0        0        0      870 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/sqlalchemy.py
+-rw-r--r--   0        0        0      783 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/sqlalchemy_future.py
+-rw-r--r--   0        0        0      857 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/sqlmodel.py
+-rw-r--r--   0        0        0     1147 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/ext/tortoise.py
+-rw-r--r--   0        0        0     1083 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/iterables.py
+-rw-r--r--   0        0        0     1201 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/limit_offset.py
+-rw-r--r--   0        0        0       69 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/links/__init__.py
+-rw-r--r--   0        0        0     1165 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/links/bases.py
+-rw-r--r--   0        0        0      832 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/links/default.py
+-rw-r--r--   0        0        0     1193 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/links/limmit_offset.py
+-rw-r--r--   0        0        0      614 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/paginator.py
+-rw-r--r--   0        0        0        0 2022-04-16 13:55:31.772361 fastapi-pagination-0.9.3/fastapi_pagination/py.typed
+-rw-r--r--   0        0        0     2816 2022-04-16 13:55:31.776361 fastapi-pagination-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     3897 2022-04-16 13:55:44.942903 fastapi-pagination-0.9.3/setup.py
+-rw-r--r--   0        0        0     4186 2022-04-16 13:55:44.943358 fastapi-pagination-0.9.3/PKG-INFO
```

### Comparing `fastapi-pagination-0.9.2/LICENSE` & `fastapi-pagination-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/README.md` & `fastapi-pagination-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/api.py` & `fastapi-pagination-0.9.3/fastapi_pagination/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import inspect
-from contextlib import contextmanager
+from contextlib import contextmanager, suppress
 from contextvars import ContextVar
 from typing import (
     Any,
     AsyncIterator,
     Callable,
     ContextManager,
     Iterator,
@@ -64,15 +64,17 @@
 
 def _ctx_var_with_reset(var: ContextVar, value: Any) -> ContextManager[None]:
     token = var.set(value)
 
     @contextmanager
     def _reset_ctx() -> Iterator[None]:
         yield
-        var.reset(token)
+
+        with suppress(ValueError):
+            var.reset(token)
 
     return _reset_ctx()
 
 
 def set_page(page: Type[AbstractPage]) -> ContextManager[None]:
     return _ctx_var_with_reset(page_type, page)
```

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/bases.py` & `fastapi-pagination-0.9.3/fastapi_pagination/bases.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/default.py` & `fastapi-pagination-0.9.3/fastapi_pagination/default.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/ext/async_sqlalchemy.py` & `fastapi-pagination-0.9.3/fastapi_pagination/ext/async_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/ext/async_sqlmodel.py` & `fastapi-pagination-0.9.3/fastapi_pagination/ext/async_sqlmodel.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/ext/asyncpg.py` & `fastapi-pagination-0.9.3/fastapi_pagination/ext/asyncpg.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/ext/databases.py` & `fastapi-pagination-0.9.3/fastapi_pagination/ext/databases.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/ext/django.py` & `fastapi-pagination-0.9.3/fastapi_pagination/ext/django.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/ext/gino.py` & `fastapi-pagination-0.9.3/fastapi_pagination/ext/gino.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/ext/mongoengine.py` & `fastapi-pagination-0.9.3/fastapi_pagination/ext/mongoengine.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/ext/motor.py` & `fastapi-pagination-0.9.3/fastapi_pagination/ext/motor.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/ext/orm.py` & `fastapi-pagination-0.9.3/fastapi_pagination/ext/orm.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/ext/ormar.py` & `fastapi-pagination-0.9.3/fastapi_pagination/ext/ormar.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/ext/piccolo.py` & `fastapi-pagination-0.9.3/fastapi_pagination/ext/piccolo.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/ext/sqlalchemy.py` & `fastapi-pagination-0.9.3/fastapi_pagination/ext/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/ext/sqlalchemy_future.py` & `fastapi-pagination-0.9.3/fastapi_pagination/ext/sqlalchemy_future.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/ext/sqlmodel.py` & `fastapi-pagination-0.9.3/fastapi_pagination/ext/sqlmodel.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/ext/tortoise.py` & `fastapi-pagination-0.9.3/fastapi_pagination/ext/tortoise.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/iterables.py` & `fastapi-pagination-0.9.3/fastapi_pagination/iterables.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/limit_offset.py` & `fastapi-pagination-0.9.3/fastapi_pagination/limit_offset.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/links/bases.py` & `fastapi-pagination-0.9.3/fastapi_pagination/links/bases.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/links/default.py` & `fastapi-pagination-0.9.3/fastapi_pagination/links/default.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/links/limmit_offset.py` & `fastapi-pagination-0.9.3/fastapi_pagination/links/limmit_offset.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/fastapi_pagination/paginator.py` & `fastapi-pagination-0.9.3/fastapi_pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-0.9.2/pyproject.toml` & `fastapi-pagination-0.9.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-pagination"
-version = "0.9.2"
+version = "0.9.3"
 description = "FastAPI pagination"
 authors = [
     "Yurii Karabas <1998uriyyo@gmail.com>",
 ]
 
 license = "MIT"
 readme = "README.md"
@@ -25,15 +25,15 @@
 pydantic = ">=1.7.2"
 fastapi = ">=0.61.2"
 gino = { version = ">=1.0.1", extras = ["starlette"], optional = true }
 SQLAlchemy = { version = ">=1.3.20", optional = true }
 databases = { version = ">=0.4.0", extras = ["postgresql", "sqlite", "mysql"], optional = true }
 orm = { version = ">=0.1.5", optional = true }
 typesystem = { version = "^0.2.0", optional = true }
-tortoise-orm = { version = ">=0.16.18,<0.19.0", extras = ["asyncpg", "aiomysql", "aiosqlite"], optional = true }
+tortoise-orm = { version = ">=0.16.18,<0.20.0", extras = ["asyncpg", "aiomysql", "aiosqlite"], optional = true }
 asyncpg = { version = ">=0.24.0", optional = true }
 ormar = { version = ">=0.10.5", optional = true}
 Django = { version = "<3.3.0", optional = true}
 piccolo = { version = ">=0.29,<0.35", optional = true}
 motor =  { version = "^2.5.1", optional = true }
 
 # sqlmodel = { version = "^0.0.4", optional = true} Should be uncommented when gino will support sqlalchemy 1.4
```

### Comparing `fastapi-pagination-0.9.2/setup.py` & `fastapi-pagination-0.9.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,40 +9,40 @@
 
 install_requires = \
 ['fastapi>=0.61.2', 'pydantic>=1.7.2']
 
 extras_require = \
 {'all': ['gino[starlette]>=1.0.1',
          'SQLAlchemy>=1.3.20',
-         'databases[postgresql,sqlite,mysql]>=0.4.0',
+         'databases[postgresql,mysql,sqlite]>=0.4.0',
          'orm>=0.1.5',
-         'tortoise-orm[asyncpg,aiomysql,aiosqlite]>=0.16.18,<0.19.0',
+         'tortoise-orm[aiomysql,asyncpg,aiosqlite]>=0.16.18,<0.20.0',
          'asyncpg>=0.24.0',
          'ormar>=0.10.5',
          'Django<3.3.0',
          'piccolo>=0.29,<0.35',
          'motor>=2.5.1,<3.0.0',
          'mongoengine>=0.23.1,<0.25.0'],
  'asyncpg': ['SQLAlchemy>=1.3.20', 'asyncpg>=0.24.0'],
- 'databases': ['databases[postgresql,sqlite,mysql]>=0.4.0'],
- 'django': ['databases[postgresql,sqlite,mysql]>=0.4.0', 'Django<3.3.0'],
+ 'databases': ['databases[postgresql,mysql,sqlite]>=0.4.0'],
+ 'django': ['databases[postgresql,mysql,sqlite]>=0.4.0', 'Django<3.3.0'],
  'gino': ['gino[starlette]>=1.0.1', 'SQLAlchemy>=1.3.20'],
  'mongoengine': ['mongoengine>=0.23.1,<0.25.0'],
  'motor': ['motor>=2.5.1,<3.0.0'],
- 'orm': ['databases[postgresql,sqlite,mysql]>=0.4.0',
+ 'orm': ['databases[postgresql,mysql,sqlite]>=0.4.0',
          'orm>=0.1.5',
          'typesystem>=0.2.0,<0.3.0'],
  'ormar': ['ormar>=0.10.5'],
  'piccolo': ['piccolo>=0.29,<0.35'],
  'sqlalchemy': ['SQLAlchemy>=1.3.20'],
- 'tortoise': ['tortoise-orm[asyncpg,aiomysql,aiosqlite]>=0.16.18,<0.19.0']}
+ 'tortoise': ['tortoise-orm[aiomysql,asyncpg,aiosqlite]>=0.16.18,<0.20.0']}
 
 setup_kwargs = {
     'name': 'fastapi-pagination',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'FastAPI pagination',
     'long_description': "# FastAPI Pagination\n\n[![License](https://img.shields.io/badge/License-MIT-lightgrey)](/LICENSE)\n[![codecov](https://github.com/uriyyo/fastapi-pagination/workflows/Test/badge.svg)](https://github.com/uriyyo/fastapi-pagination/actions)\n[![codecov](https://codecov.io/gh/uriyyo/fastapi-pagination/branch/main/graph/badge.svg?token=QqIqDQ7FZi)](https://codecov.io/gh/uriyyo/fastapi-pagination)\n[![Downloads](https://pepy.tech/badge/fastapi-pagination)](https://pepy.tech/project/fastapi-pagination)\n[![PYPI](https://img.shields.io/pypi/v/fastapi-pagination)](https://pypi.org/project/fastapi-pagination/)\n[![PYPI](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Support me on Patreon](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Duriyyo%26type%3Dpatrons&style=flat)](https://patreon.com/uriyyo)\n\n## Installation\n\n```bash\n# Basic version\npip install fastapi-pagination\n\n# All available integrations\npip install fastapi-pagination[all]\n```\n\nAvailable integrations:\n\n* [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy)\n* [gino](https://github.com/python-gino/gino)\n* [databases](https://github.com/encode/databases)\n* [ormar](http://github.com/collerek/ormar)\n* [orm](https://github.com/encode/orm)\n* [tortoise](https://github.com/tortoise/tortoise-orm)\n* [django](https://github.com/django/django)\n* [piccolo](https://github.com/piccolo-orm/piccolo)\n* [sqlmodel](https://github.com/tiangolo/sqlmodel)\n* [motor](https://github.com/mongodb/motor)\n* [mongoengine](https://github.com/MongoEngine/mongoengine)\n\n## Example\n\n```python\nfrom fastapi import FastAPI\nfrom pydantic import BaseModel\n\nfrom fastapi_pagination import Page, add_pagination, paginate\n\napp = FastAPI()\n\n\nclass User(BaseModel):\n    name: str\n    surname: str\n\n\nusers = [\n    User(name='Yurii', surname='Karabas'),\n    # ...\n]\n\n\n@app.get('/users', response_model=Page[User])\nasync def get_users():\n    return paginate(users)\n\n\nadd_pagination(app)\n```\n",
     'author': 'Yurii Karabas',
     'author_email': '1998uriyyo@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/uriyyo/fastapi-pagination',
```

### Comparing `fastapi-pagination-0.9.2/PKG-INFO` & `fastapi-pagination-0.9.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-pagination
-Version: 0.9.2
+Version: 0.9.3
 Summary: FastAPI pagination
 Home-page: https://github.com/uriyyo/fastapi-pagination
 License: MIT
 Author: Yurii Karabas
 Author-email: 1998uriyyo@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -27,24 +27,24 @@
 Provides-Extra: ormar
 Provides-Extra: piccolo
 Provides-Extra: sqlalchemy
 Provides-Extra: tortoise
 Requires-Dist: Django (<3.3.0); extra == "django" or extra == "all"
 Requires-Dist: SQLAlchemy (>=1.3.20); extra == "gino" or extra == "sqlalchemy" or extra == "asyncpg" or extra == "all"
 Requires-Dist: asyncpg (>=0.24.0); extra == "asyncpg" or extra == "all"
-Requires-Dist: databases[postgresql,sqlite,mysql] (>=0.4.0); extra == "databases" or extra == "orm" or extra == "django" or extra == "all"
+Requires-Dist: databases[postgresql,mysql,sqlite] (>=0.4.0); extra == "databases" or extra == "orm" or extra == "django" or extra == "all"
 Requires-Dist: fastapi (>=0.61.2)
 Requires-Dist: gino[starlette] (>=1.0.1); extra == "gino" or extra == "all"
 Requires-Dist: mongoengine (>=0.23.1,<0.25.0); extra == "mongoengine" or extra == "all"
 Requires-Dist: motor (>=2.5.1,<3.0.0); extra == "motor" or extra == "all"
 Requires-Dist: orm (>=0.1.5); extra == "orm" or extra == "all"
 Requires-Dist: ormar (>=0.10.5); extra == "ormar" or extra == "all"
 Requires-Dist: piccolo (>=0.29,<0.35); extra == "piccolo" or extra == "all"
 Requires-Dist: pydantic (>=1.7.2)
-Requires-Dist: tortoise-orm[asyncpg,aiomysql,aiosqlite] (>=0.16.18,<0.19.0); extra == "tortoise" or extra == "all"
+Requires-Dist: tortoise-orm[aiomysql,asyncpg,aiosqlite] (>=0.16.18,<0.20.0); extra == "tortoise" or extra == "all"
 Requires-Dist: typesystem (>=0.2.0,<0.3.0); extra == "orm"
 Project-URL: Repository, https://github.com/uriyyo/fastapi-pagination
 Description-Content-Type: text/markdown
 
 # FastAPI Pagination
 
 [![License](https://img.shields.io/badge/License-MIT-lightgrey)](/LICENSE)
```

