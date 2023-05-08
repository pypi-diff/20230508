# Comparing `tmp/senabase-starterpack-0.1.6.tar.gz` & `tmp/senabase-starterpack-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "senabase-starterpack-0.1.6.tar", last modified: Mon Mar 13 12:37:18 2023, max compression
+gzip compressed data, was "senabase-starterpack-0.1.7.tar", last modified: Mon May  8 08:40:27 2023, max compression
```

## Comparing `senabase-starterpack-0.1.6.tar` & `senabase-starterpack-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dongobie   (501) staff       (20)        0 2023-03-13 12:37:18.819537 senabase-starterpack-0.1.6/
--rw-r--r--   0 dongobie   (501) staff       (20)     1069 2023-01-27 10:15:26.000000 senabase-starterpack-0.1.6/LICENSE
--rw-r--r--   0 dongobie   (501) staff       (20)     1131 2023-03-13 12:37:18.819369 senabase-starterpack-0.1.6/PKG-INFO
--rw-r--r--   0 dongobie   (501) staff       (20)      827 2023-03-13 12:31:29.000000 senabase-starterpack-0.1.6/README.md
-drwxr-xr-x   0 dongobie   (501) staff       (20)        0 2023-03-13 12:37:18.818337 senabase-starterpack-0.1.6/senabase/
--rw-r--r--   0 dongobie   (501) staff       (20)        0 2022-12-08 20:57:22.000000 senabase-starterpack-0.1.6/senabase/__init__.py
-drwxr-xr-x   0 dongobie   (501) staff       (20)        0 2023-03-13 12:37:18.818637 senabase-starterpack-0.1.6/senabase/starterpack/
--rw-r--r--   0 dongobie   (501) staff       (20)        0 2023-03-13 12:17:16.000000 senabase-starterpack-0.1.6/senabase/starterpack/__init__.py
--rw-r--r--   0 dongobie   (501) staff       (20)     1320 2023-03-13 12:17:52.000000 senabase-starterpack-0.1.6/senabase/starterpack/database.py
--rw-r--r--   0 dongobie   (501) staff       (20)     1833 2023-03-13 12:25:58.000000 senabase-starterpack-0.1.6/senabase/starterpack/log.py
-drwxr-xr-x   0 dongobie   (501) staff       (20)        0 2023-03-13 12:37:18.819188 senabase-starterpack-0.1.6/senabase_starterpack.egg-info/
--rw-r--r--   0 dongobie   (501) staff       (20)     1131 2023-03-13 12:37:18.000000 senabase-starterpack-0.1.6/senabase_starterpack.egg-info/PKG-INFO
--rw-r--r--   0 dongobie   (501) staff       (20)      360 2023-03-13 12:37:18.000000 senabase-starterpack-0.1.6/senabase_starterpack.egg-info/SOURCES.txt
--rw-r--r--   0 dongobie   (501) staff       (20)        1 2023-03-13 12:37:18.000000 senabase-starterpack-0.1.6/senabase_starterpack.egg-info/dependency_links.txt
--rw-r--r--   0 dongobie   (501) staff       (20)       35 2023-03-13 12:37:18.000000 senabase-starterpack-0.1.6/senabase_starterpack.egg-info/requires.txt
--rw-r--r--   0 dongobie   (501) staff       (20)        9 2023-03-13 12:37:18.000000 senabase-starterpack-0.1.6/senabase_starterpack.egg-info/top_level.txt
--rw-r--r--   0 dongobie   (501) staff       (20)       38 2023-03-13 12:37:18.819588 senabase-starterpack-0.1.6/setup.cfg
--rw-r--r--   0 dongobie   (501) staff       (20)      694 2023-03-13 11:22:53.000000 senabase-starterpack-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 08:40:27.496457 senabase-starterpack-0.1.7/
+-rw-rw-rw-   0        0        0     1090 2023-05-07 23:47:08.000000 senabase-starterpack-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     1188 2023-05-08 08:40:27.495459 senabase-starterpack-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      875 2023-05-07 23:47:08.000000 senabase-starterpack-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 08:40:27.488460 senabase-starterpack-0.1.7/senabase/
+-rw-rw-rw-   0        0        0        0 2023-05-07 23:47:08.000000 senabase-starterpack-0.1.7/senabase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 08:40:27.490465 senabase-starterpack-0.1.7/senabase/starterpack/
+-rw-rw-rw-   0        0        0        0 2023-05-07 23:47:08.000000 senabase-starterpack-0.1.7/senabase/starterpack/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-05-08 00:34:12.000000 senabase-starterpack-0.1.7/senabase/starterpack/database.py
+-rw-rw-rw-   0        0        0     1886 2023-05-07 23:47:08.000000 senabase-starterpack-0.1.7/senabase/starterpack/log.py
+drwxrwxrwx   0        0        0        0 2023-05-08 08:40:27.494457 senabase-starterpack-0.1.7/senabase_starterpack.egg-info/
+-rw-rw-rw-   0        0        0     1188 2023-05-08 08:40:27.000000 senabase-starterpack-0.1.7/senabase_starterpack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-05-08 08:40:27.000000 senabase-starterpack-0.1.7/senabase_starterpack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 08:40:27.000000 senabase-starterpack-0.1.7/senabase_starterpack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-08 08:40:27.000000 senabase-starterpack-0.1.7/senabase_starterpack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 08:40:27.000000 senabase-starterpack-0.1.7/senabase_starterpack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 08:40:27.496457 senabase-starterpack-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      711 2023-05-08 08:40:23.000000 senabase-starterpack-0.1.7/setup.py
```

### Comparing `senabase-starterpack-0.1.6/LICENSE` & `senabase-starterpack-0.1.7/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Jungkyu Park
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Jungkyu Park
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `senabase-starterpack-0.1.6/PKG-INFO` & `senabase-starterpack-0.1.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-Metadata-Version: 2.1
-Name: senabase-starterpack
-Version: 0.1.6
-Summary: senabase starterpack library
-Home-page: https://github.com/parkssie/senabase-starterpack
-Author: Jungkyu Park
-Author-email: parkssie@gmail.com
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# senabase-starterpack
-
-senabase-starterpack is personal library for fast prototyping.
-
-## Installation
-
-Use `pip` to download it from [PyPI](https://pypi.org/project/senabase-starterpack/)
-
-```shell
-$ pip install senabase-starterpack
-```
-
-The minimum required versions of the respective tools are:
-
-```
-psycopg2-binary>=2.9.*
-pyyaml>=6.*
-```
-
-## Example
-
-### PostgreSQLHandler
-
-Postgresql starterpack
-
-```python
-from senabase.starterpack.database import PostgreSQLHandler
-
-pgh = PostgreSQLHandler()
-pgh.configure('127.0.0.1', 5432, 'postgres', 'userid', 'userpassword')
-
-q1 = 'select now()'
-rs = pgh.get(q1)
-```
-
-### log
-
-Logging starterpack
-
-```python
-from senabase.starterpack.log import SimpleLogger
-
-log = SimpleLogger()
-log.configure('proto')
-
-log.i('Information')
-log.d('Debug')
-log.e(Exception('Example exception'))
-```
+Metadata-Version: 2.1
+Name: senabase-starterpack
+Version: 0.1.7
+Summary: senabase starterpack library
+Home-page: https://github.com/parkssie/senabase-starterpack
+Author: Jungkyu Park
+Author-email: parkssie@me.com
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# senabase-starterpack
+
+senabase-starterpack is personal library for fast prototyping.
+
+## Installation
+
+Use `pip` to download it from [PyPI](https://pypi.org/project/senabase-starterpack/)
+
+```shell
+$ pip install senabase-starterpack
+```
+
+The minimum required versions of the respective tools are:
+
+```
+psycopg2-binary>=2.9.*
+pyyaml>=6.*
+```
+
+## Example
+
+### PostgreSQLHandler
+
+Postgresql starterpack
+
+```python
+from senabase.starterpack.database import PostgreSQLHandler
+
+pgh = PostgreSQLHandler()
+pgh.configure('127.0.0.1', 5432, 'postgres', 'userid', 'userpassword')
+
+q1 = 'select now()'
+rs = pgh.get(q1)
+```
+
+### log
+
+Logging starterpack
+
+```python
+from senabase.starterpack.log import SimpleLogger
+
+log = SimpleLogger()
+log.configure('proto')
+
+log.i('Information')
+log.d('Debug')
+log.e(Exception('Example exception'))
+```
```

### Comparing `senabase-starterpack-0.1.6/README.md` & `senabase-starterpack-0.1.7/senabase_starterpack.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,60 @@
-# senabase-starterpack
-
-senabase-starterpack is personal library for fast prototyping.
-
-## Installation
-
-Use `pip` to download it from [PyPI](https://pypi.org/project/senabase-starterpack/)
-
-```shell
-$ pip install senabase-starterpack
-```
-
-The minimum required versions of the respective tools are:
-
-```
-psycopg2-binary>=2.9.*
-pyyaml>=6.*
-```
-
-## Example
-
-### PostgreSQLHandler
-
-Postgresql starterpack
-
-```python
-from senabase.starterpack.database import PostgreSQLHandler
-
-pgh = PostgreSQLHandler()
-pgh.configure('127.0.0.1', 5432, 'postgres', 'userid', 'userpassword')
-
-q1 = 'select now()'
-rs = pgh.get(q1)
-```
-
-### log
-
-Logging starterpack
-
-```python
-from senabase.starterpack.log import SimpleLogger
-
-log = SimpleLogger()
-log.configure('proto')
-
-log.i('Information')
-log.d('Debug')
-log.e(Exception('Example exception'))
-```
+Metadata-Version: 2.1
+Name: senabase-starterpack
+Version: 0.1.7
+Summary: senabase starterpack library
+Home-page: https://github.com/parkssie/senabase-starterpack
+Author: Jungkyu Park
+Author-email: parkssie@me.com
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# senabase-starterpack
+
+senabase-starterpack is personal library for fast prototyping.
+
+## Installation
+
+Use `pip` to download it from [PyPI](https://pypi.org/project/senabase-starterpack/)
+
+```shell
+$ pip install senabase-starterpack
+```
+
+The minimum required versions of the respective tools are:
+
+```
+psycopg2-binary>=2.9.*
+pyyaml>=6.*
+```
+
+## Example
+
+### PostgreSQLHandler
+
+Postgresql starterpack
+
+```python
+from senabase.starterpack.database import PostgreSQLHandler
+
+pgh = PostgreSQLHandler()
+pgh.configure('127.0.0.1', 5432, 'postgres', 'userid', 'userpassword')
+
+q1 = 'select now()'
+rs = pgh.get(q1)
+```
+
+### log
+
+Logging starterpack
+
+```python
+from senabase.starterpack.log import SimpleLogger
+
+log = SimpleLogger()
+log.configure('proto')
+
+log.i('Information')
+log.d('Debug')
+log.e(Exception('Example exception'))
+```
```

