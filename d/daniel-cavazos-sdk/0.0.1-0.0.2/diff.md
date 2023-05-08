# Comparing `tmp/daniel-cavazos-sdk-0.0.1.tar.gz` & `tmp/daniel-cavazos-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daniel-cavazos-sdk-0.0.1.tar", last modified: Mon May  8 20:23:44 2023, max compression
+gzip compressed data, was "daniel-cavazos-sdk-0.0.2.tar", last modified: Mon May  8 20:46:51 2023, max compression
```

## Comparing `daniel-cavazos-sdk-0.0.1.tar` & `daniel-cavazos-sdk-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 20:23:44.399475 daniel-cavazos-sdk-0.0.1/
--rw-rw-rw-   0        0        0      381 2023-05-08 20:23:44.399475 daniel-cavazos-sdk-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-08 19:59:18.000000 daniel-cavazos-sdk-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 20:23:44.391476 daniel-cavazos-sdk-0.0.1/daniel_cavazos_sdk.egg-info/
--rw-rw-rw-   0        0        0      381 2023-05-08 20:23:44.000000 daniel-cavazos-sdk-0.0.1/daniel_cavazos_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-08 20:23:44.000000 daniel-cavazos-sdk-0.0.1/daniel_cavazos_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 20:23:44.000000 daniel-cavazos-sdk-0.0.1/daniel_cavazos_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-08 20:23:44.000000 daniel-cavazos-sdk-0.0.1/daniel_cavazos_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 20:23:44.399475 daniel-cavazos-sdk-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      634 2023-05-08 20:05:39.000000 daniel-cavazos-sdk-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:23:44.398475 daniel-cavazos-sdk-0.0.1/the_one_client/
--rw-rw-rw-   0        0        0        0 2023-05-08 20:00:29.000000 daniel-cavazos-sdk-0.0.1/the_one_client/__init__.py
--rw-rw-rw-   0        0        0     2243 2023-05-08 20:19:23.000000 daniel-cavazos-sdk-0.0.1/the_one_client/builder.py
--rw-rw-rw-   0        0        0     1432 2023-05-08 20:21:49.000000 daniel-cavazos-sdk-0.0.1/the_one_client/client.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:46:51.481825 daniel-cavazos-sdk-0.0.2/
+-rw-rw-rw-   0        0        0     2101 2023-05-08 20:46:51.481825 daniel-cavazos-sdk-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1716 2023-05-08 20:46:17.000000 daniel-cavazos-sdk-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 20:46:51.468781 daniel-cavazos-sdk-0.0.2/daniel_cavazos_sdk/
+-rw-rw-rw-   0        0        0        0 2023-05-08 20:00:29.000000 daniel-cavazos-sdk-0.0.2/daniel_cavazos_sdk/__init__.py
+-rw-rw-rw-   0        0        0     2243 2023-05-08 20:19:23.000000 daniel-cavazos-sdk-0.0.2/daniel_cavazos_sdk/builder.py
+-rw-rw-rw-   0        0        0     1210 2023-05-08 20:44:30.000000 daniel-cavazos-sdk-0.0.2/daniel_cavazos_sdk/client.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:46:51.480824 daniel-cavazos-sdk-0.0.2/daniel_cavazos_sdk.egg-info/
+-rw-rw-rw-   0        0        0     2101 2023-05-08 20:46:51.000000 daniel-cavazos-sdk-0.0.2/daniel_cavazos_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-08 20:46:51.000000 daniel-cavazos-sdk-0.0.2/daniel_cavazos_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 20:46:51.000000 daniel-cavazos-sdk-0.0.2/daniel_cavazos_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-08 20:46:51.000000 daniel-cavazos-sdk-0.0.2/daniel_cavazos_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 20:46:51.482826 daniel-cavazos-sdk-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      634 2023-05-08 20:46:30.000000 daniel-cavazos-sdk-0.0.2/setup.py
```

### Comparing `daniel-cavazos-sdk-0.0.1/setup.py` & `daniel-cavazos-sdk-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="daniel-cavazos-sdk",
-    version="0.0.1",
+    version="0.0.2",
     author="Daniel Cavazos",
     author_email="dcaazy@gmail.com",
     description="Accesses The One API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `daniel-cavazos-sdk-0.0.1/the_one_client/builder.py` & `daniel-cavazos-sdk-0.0.2/daniel_cavazos_sdk/builder.py`

 * *Files identical despite different names*

### Comparing `daniel-cavazos-sdk-0.0.1/the_one_client/client.py` & `daniel-cavazos-sdk-0.0.2/daniel_cavazos_sdk/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from .builder import SDKBuilder
+
 class TheOneClient(SDKBuilder):
     """
     A client for The One API that extends the SDKBuilder class.
 
     This class defines methods that interact with The One API to retrieve information
     about movies and quotes from the Lord of the Rings trilogy.
 
@@ -18,24 +20,13 @@
 
     # retrieve all quotes for a specific movie by ID
     quotes = client.get_movie_quotes(id="5cd95395de30eff6ebccde56")
 
     # retrieve a specific quote by ID
     one_ring_quote = client.get_quote(id="5cd96e05de30eff6ebccebce")
     """
-
     host = "https://the-one-api.dev/v2"
     get_movies = SDKBuilder.GET("/movie")
     get_movie = SDKBuilder.GET("/movie/{id}")
-    get_movie_quotes = SDKBuilder.GET(
-
-
-client = TheOneClient(token="eUHAQDqjMHmj4rLHN8eF")
-movies = client.get_movies()
-print(movies)
-movie = client.get_movie(id="5cd95395de30eff6ebccde56")
-print(movie)
-movie_quotes = client.get_movie_quotes(id="5cd95395de30eff6ebccde56")
-print(movie_quotes)
-quotes = client.get_quotes()
-print(quotes)
-quote = client.get_quote(id="5cd96e05de30eff6ebccebce")
+    get_movie_quotes = SDKBuilder.GET("/movie/{id}/quote")
+    get_quotes = SDKBuilder.GET("/quote")
+    get_quote = SDKBuilder.GET("/quote/{id}")
```

