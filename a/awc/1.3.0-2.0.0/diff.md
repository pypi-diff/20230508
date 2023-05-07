# Comparing `tmp/awc-1.3.0-py2.py3-none-any.whl.zip` & `tmp/awc-2.0.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 23896 bytes, number of entries: 16
--rw-r--r--  2.0 unx     6843 b- defN 23-May-06 23:15 awc/__init__.py
+Zip file size: 23907 bytes, number of entries: 16
+-rw-r--r--  2.0 unx     6843 b- defN 23-May-07 23:41 awc/__init__.py
 -rw-r--r--  2.0 unx      678 b- defN 23-Apr-11 16:56 awc/__main__.py
--rw-r--r--  2.0 unx     6039 b- defN 23-May-06 22:49 awc/api.py
+-rw-r--r--  2.0 unx     6030 b- defN 23-May-07 23:42 awc/api.py
 -rw-r--r--  2.0 unx      305 b- defN 23-Apr-12 22:27 awc/const.py
 -rw-r--r--  2.0 unx     1479 b- defN 23-Apr-15 21:04 awc/exc.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 12:49 awc/py.typed
 -rw-r--r--  2.0 unx     1383 b- defN 23-Apr-13 14:54 awc/util.py
 -rw-r--r--  2.0 unx      614 b- defN 23-Apr-12 22:27 awc/wrn.py
--rw-r--r--  2.0 unx     4660 b- defN 23-May-06 22:53 awc/sql/__init__.py
--rw-r--r--  2.0 unx     3453 b- defN 23-May-06 23:12 awc/sql/helpers.py
--rw-------  2.0 unx    35107 b- defN 23-May-06 23:16 awc-1.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3812 b- defN 23-May-06 23:16 awc-1.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-06 23:16 awc-1.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-May-06 23:16 awc-1.3.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 19:04 awc-1.3.0.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1145 b- defN 23-May-06 23:16 awc-1.3.0.dist-info/RECORD
-16 files, 65633 bytes uncompressed, 22060 bytes compressed:  66.4%
+-rw-r--r--  2.0 unx     4715 b- defN 23-May-07 23:39 awc/sql/__init__.py
+-rw-r--r--  2.0 unx     3461 b- defN 23-May-07 23:41 awc/sql/helpers.py
+-rw-------  2.0 unx    35107 b- defN 23-May-07 23:47 awc-2.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3812 b- defN 23-May-07 23:47 awc-2.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-07 23:47 awc-2.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-May-07 23:47 awc-2.0.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 19:04 awc-2.0.0.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1145 b- defN 23-May-07 23:47 awc-2.0.0.dist-info/RECORD
+16 files, 65687 bytes uncompressed, 22071 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -24,26 +24,26 @@
 
 Filename: awc/sql/__init__.py
 Comment: 
 
 Filename: awc/sql/helpers.py
 Comment: 
 
-Filename: awc-1.3.0.dist-info/LICENSE
+Filename: awc-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: awc-1.3.0.dist-info/METADATA
+Filename: awc-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: awc-1.3.0.dist-info/WHEEL
+Filename: awc-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: awc-1.3.0.dist-info/top_level.txt
+Filename: awc-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: awc-1.3.0.dist-info/zip-safe
+Filename: awc-2.0.0.dist-info/zip-safe
 Comment: 
 
-Filename: awc-1.3.0.dist-info/RECORD
+Filename: awc-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awc/__init__.py

```diff
@@ -7,15 +7,15 @@
 from functools import wraps
 
 import requests
 from furl import furl  # type: ignore
 
 from . import const, exc, util
 
-__version__: typing.Final[str] = "1.3.0"
+__version__: typing.Final[str] = "2.0.0"
 
 
 class Awc:
     """ari-web comments interface
 
     this is where all API requests begin, you must
     pass an instance of this object to every api wrapper
```

## awc/api.py

```diff
@@ -178,21 +178,21 @@
 def applied(awc: Awc) -> bool:
     """returns your application status ( `True` if applied / accepted )
 
     awc: awc.Awc -- the awc.Awc instance to work on"""
     return util.resp_to_bool(awc.get(api="applied").text)
 
 
-def anon(awc: Awc, content: str) -> requests.Response:
+def anon(awc: Awc, content: str) -> str:
     """send message to server anonymously
 
     awc: awc.Awc -- the awc.Awc instance to work on
     content: str -- the reason why youre applying
 
     return requests.Response -- the id of the message"""
 
     return awc.post(
         api="anon",
         data={
             "content": util.truncate(content, const.MAX_CONTENT_LEN),
         },
-    )
+    ).text
```

## awc/sql/__init__.py

```diff
@@ -141,14 +141,15 @@
     """anonymous message table"""
 
     tname: str = "anon"
     t: pypika.Table = pypika.Table(tname)
 
     cid: pypika.Column = t.cid  # type: ignore
     content: pypika.Column = t.content  # type: ignore
+    headers: pypika.Column = t.headers  # type: ignore
 
 
 def sql(query: pypika.queries.QueryBuilder) -> str:
     """return an sql query"""
     return query.get_sql()
```

## awc/sql/helpers.py

```diff
@@ -98,23 +98,23 @@
                 Comment.author: censoring,
                 Comment.content: censoring,
             },
         )
     ]
 
 
-def get_anon_msg(cid: int) -> typing.List[pypika.queries.QueryBuilder]:
+def get_anon_msg(ip: str) -> typing.List[pypika.queries.QueryBuilder]:
     """get an anonymous message by id
 
-    cid: int -- content id
+    ip: str -- content id ( ip )
 
     return typing.List[pypika.queries.QueryBuilder] -- the queries"""
-    return [AnonMsg.select(AnonMsg.cid == cid, AnonMsg.content)]  # type: ignore
+    return [AnonMsg.select(AnonMsg.cid == ip, AnonMsg.content)]  # type: ignore
 
 
-def del_anon_msg(cid: int) -> typing.List[pypika.queries.QueryBuilder]:
+def del_anon_msg(ip: str) -> typing.List[pypika.queries.QueryBuilder]:
     """delete an anonymous message by id
 
-    cid: int -- content id
+    ip: str -- content id ( ip )
 
     return typing.List[pypika.queries.QueryBuilder] -- the queries"""
-    return [delete(AnonMsg.query(AnonMsg.cid == cid))]  # type: ignore
+    return [delete(AnonMsg.query(AnonMsg.cid == ip))]  # type: ignore
```

## Comparing `awc-1.3.0.dist-info/LICENSE` & `awc-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awc-1.3.0.dist-info/METADATA` & `awc-2.0.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awc
-Version: 1.3.0
+Version: 2.0.0
 Summary: wrapper for ari-web comments API
 Home-page: https://ari-web.xyz/gh/awc
 Author: Ari Archer
 Author-email: ari.web.xyz@gmail.com
 License: GPLv3+
 Keywords: http,http-client,comments,api,wrapper,https
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `awc-1.3.0.dist-info/RECORD` & `awc-2.0.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-awc/__init__.py,sha256=OkwHBCETpuVmwur9pMKvu_Lz8zQTgLc0FO6q6wqBWmo,6843
+awc/__init__.py,sha256=5uLQwp_swIDpjtoVmFW9JDQ8hDx3MY_R7V4a0lrF7KA,6843
 awc/__main__.py,sha256=d1UfoKcH5bl9qoqWowmcARIitWbbGsasAZfq8RHHsE4,678
-awc/api.py,sha256=Ike6z5oGmWd_gzdZ099B4OsSmn8K43oWrQew5plGGyA,6039
+awc/api.py,sha256=f02eIZdXfOZo9f-f7YhN1Rhcz4a55KAzxRfTIxSrzTg,6030
 awc/const.py,sha256=0ctjO9muVRU7kBkqF9LjcgwvP4baLum63UUOxTE1oLw,305
 awc/exc.py,sha256=kGwH4_a8C1EpYx3PvoBXyWiiW451YbHsKi_JGtnsiuk,1479
 awc/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 awc/util.py,sha256=u9-_per8iyglLx9dVfQKJBdSEFZq2-5aymE7XDjoJ0o,1383
 awc/wrn.py,sha256=K84cpt9OdHQi76vhgMsWFbl8rIN_sH6EkOGptZOUWmQ,614
-awc/sql/__init__.py,sha256=jQn-2p7E3-dEfOEOIK7TQ3exmGR7pWa8Lj-XkGP37ZI,4660
-awc/sql/helpers.py,sha256=azK2eyKk49VWqEfuLWgwSOVZrz85kySNxxxy6PJO9TA,3453
-awc-1.3.0.dist-info/LICENSE,sha256=nqVIZAIjniFxpDnU4HMUA3KRZ8mFA_JpXMNFVQTHlVI,35107
-awc-1.3.0.dist-info/METADATA,sha256=ay5Mt5MfOW5c2wd0FaIE3g13xYcu-K41b7InjOTURHk,3812
-awc-1.3.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-awc-1.3.0.dist-info/top_level.txt,sha256=Xj3P9OwultDU5KrAvJbWKuD3ki2LWL6tSfbMPu28Hck,4
-awc-1.3.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-awc-1.3.0.dist-info/RECORD,,
+awc/sql/__init__.py,sha256=HmoZ5tZkUYCcfQYWVpFqFOfE9nC9-zyXqbU95MAYGNU,4715
+awc/sql/helpers.py,sha256=RpvZjgSj2-ZidZCR9vPQhpRWKJkeBgcTLWYz0i-jc34,3461
+awc-2.0.0.dist-info/LICENSE,sha256=nqVIZAIjniFxpDnU4HMUA3KRZ8mFA_JpXMNFVQTHlVI,35107
+awc-2.0.0.dist-info/METADATA,sha256=5to-Bt5mPPu_mbF8MItG4L3KggHrXktokNHB2IfuVA8,3812
+awc-2.0.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+awc-2.0.0.dist-info/top_level.txt,sha256=Xj3P9OwultDU5KrAvJbWKuD3ki2LWL6tSfbMPu28Hck,4
+awc-2.0.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+awc-2.0.0.dist-info/RECORD,,
```

