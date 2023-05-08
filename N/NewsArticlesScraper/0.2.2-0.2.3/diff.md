# Comparing `tmp/NewsArticlesScraper-0.2.2.tar.gz` & `tmp/NewsArticlesScraper-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NewsArticlesScraper-0.2.2.tar", last modified: Sun Apr 23 16:14:29 2023, max compression
+gzip compressed data, was "NewsArticlesScraper-0.2.3.tar", last modified: Mon May  8 19:41:37 2023, max compression
```

## Comparing `NewsArticlesScraper-0.2.2.tar` & `NewsArticlesScraper-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 16:14:29.823987 NewsArticlesScraper-0.2.2/
-drwxrwxrwx   0        0        0        0 2023-04-23 16:14:29.803987 NewsArticlesScraper-0.2.2/NewsArticlesScraper/
--rw-rw-rw-   0        0        0    13787 2023-04-23 16:14:17.000000 NewsArticlesScraper-0.2.2/NewsArticlesScraper/Scrapers.py
--rw-rw-rw-   0        0        0       64 2023-02-14 20:15:57.000000 NewsArticlesScraper-0.2.2/NewsArticlesScraper/__init__.py
--rw-rw-rw-   0        0        0     1074 2023-04-23 16:12:20.000000 NewsArticlesScraper-0.2.2/NewsArticlesScraper/test.py
-drwxrwxrwx   0        0        0        0 2023-04-23 16:14:29.822486 NewsArticlesScraper-0.2.2/NewsArticlesScraper.egg-info/
--rw-rw-rw-   0        0        0      648 2023-04-23 16:14:29.000000 NewsArticlesScraper-0.2.2/NewsArticlesScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-04-23 16:14:29.000000 NewsArticlesScraper-0.2.2/NewsArticlesScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 16:14:29.000000 NewsArticlesScraper-0.2.2/NewsArticlesScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-23 16:14:29.000000 NewsArticlesScraper-0.2.2/NewsArticlesScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-23 16:14:29.000000 NewsArticlesScraper-0.2.2/NewsArticlesScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      648 2023-04-23 16:14:29.823486 NewsArticlesScraper-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-14 20:04:13.000000 NewsArticlesScraper-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-23 16:14:29.823987 NewsArticlesScraper-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      996 2023-04-23 16:14:17.000000 NewsArticlesScraper-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 19:41:37.781732 NewsArticlesScraper-0.2.3/
+drwxrwxrwx   0        0        0        0 2023-05-08 19:41:37.762231 NewsArticlesScraper-0.2.3/NewsArticlesScraper/
+-rw-rw-rw-   0        0        0    13964 2023-05-08 18:46:27.000000 NewsArticlesScraper-0.2.3/NewsArticlesScraper/Scrapers.py
+-rw-rw-rw-   0        0        0       64 2023-02-14 20:15:57.000000 NewsArticlesScraper-0.2.3/NewsArticlesScraper/__init__.py
+-rw-rw-rw-   0        0        0     1074 2023-04-23 16:12:20.000000 NewsArticlesScraper-0.2.3/NewsArticlesScraper/test.py
+drwxrwxrwx   0        0        0        0 2023-05-08 19:41:37.780231 NewsArticlesScraper-0.2.3/NewsArticlesScraper.egg-info/
+-rw-rw-rw-   0        0        0      648 2023-05-08 19:41:37.000000 NewsArticlesScraper-0.2.3/NewsArticlesScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-08 19:41:37.000000 NewsArticlesScraper-0.2.3/NewsArticlesScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 19:41:37.000000 NewsArticlesScraper-0.2.3/NewsArticlesScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-05-08 19:41:37.000000 NewsArticlesScraper-0.2.3/NewsArticlesScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-08 19:41:37.000000 NewsArticlesScraper-0.2.3/NewsArticlesScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      648 2023-05-08 19:41:37.781232 NewsArticlesScraper-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-02-14 20:04:13.000000 NewsArticlesScraper-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 19:41:37.782233 NewsArticlesScraper-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      996 2023-05-08 19:40:59.000000 NewsArticlesScraper-0.2.3/setup.py
```

### Comparing `NewsArticlesScraper-0.2.2/NewsArticlesScraper/Scrapers.py` & `NewsArticlesScraper-0.2.3/NewsArticlesScraper/Scrapers.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
         # 'JOBDIR': './News/CNBCJobs',
         'REQUEST_FINGERPRINTER_IMPLEMENTATION': '2.7',
         'DOWNLOADER_MIDDLEWARES': {
             'scrapy.downloadermiddlewares.useragent.UserAgentMiddleware': None,
             'scrapy_user_agents.middlewares.RandomUserAgentMiddleware': 400,
         },
         'RANDOM_UA_TYPE': "random",
+        'RETRY_ENABLED': True,
+        'RETRY_TIMES': 5,
     }
 
     def __init__(self, from_time: datetime.datetime, until_time: datetime.datetime, user_agent=None, **kwargs):
         self.url_stream = "https://api.queryly.com/cnbc/json.aspx?queryly_key=31a35d40a9a64ab3&query=cnbc&endindex={" \
                           "}&batchsize=100&timezoneoffset=-60&sort=date"
         self.from_time = from_time
         self.until_time = until_time
@@ -140,14 +142,16 @@
         'REQUEST_FINGERPRINTER_IMPLEMENTATION': '2.7',
         'DOWNLOAD_TIMEOUT': 300,
         'DOWNLOADER_MIDDLEWARES': {
             'scrapy.downloadermiddlewares.useragent.UserAgentMiddleware': None,
             'scrapy_user_agents.middlewares.RandomUserAgentMiddleware': 400,
         },
         'RANDOM_UA_TYPE': "random",
+        'RETRY_ENABLED': True,
+        'RETRY_TIMES': 5,
     }
 
     def __init__(self, from_time: datetime.datetime, until_time: datetime.datetime, api_key, user_agent=None, **kwargs):
         self.api_key = api_key
         self.from_time = from_time
         self.until_time = until_time
         if (datetime.datetime.now(pytz.timezone("GMT")) - self.until_time).total_seconds() <= 86400:
@@ -248,14 +252,16 @@
         'REQUEST_FINGERPRINTER_IMPLEMENTATION': '2.7',
         'DOWNLOAD_TIMEOUT': 300,
         'DOWNLOADER_MIDDLEWARES': {
             'scrapy.downloadermiddlewares.useragent.UserAgentMiddleware': None,
             'scrapy_user_agents.middlewares.RandomUserAgentMiddleware': 400,
         },
         'RANDOM_UA_TYPE': "random",
+        'RETRY_ENABLED': True,
+        'RETRY_TIMES': 5,
     }
 
     def __init__(self, from_time: datetime.datetime, until_time: datetime.datetime, api_key="test", user_agent=None,
                  **kwargs):
         self.api_key = api_key
         self.from_time = from_time
         self.until_time = until_time
```

### Comparing `NewsArticlesScraper-0.2.2/NewsArticlesScraper/test.py` & `NewsArticlesScraper-0.2.3/NewsArticlesScraper/test.py`

 * *Files identical despite different names*

### Comparing `NewsArticlesScraper-0.2.2/NewsArticlesScraper.egg-info/PKG-INFO` & `NewsArticlesScraper-0.2.3/NewsArticlesScraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2.2
+Version: 0.2.3
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2.2/PKG-INFO` & `NewsArticlesScraper-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2.2
+Version: 0.2.3
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2.2/setup.py` & `NewsArticlesScraper-0.2.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 DESCRIPTION = 'Scraping news articles'
 LONG_DESCRIPTION = 'A package that allows you to scrape news articles from various news sites via scrapy.'
 
 # Setting up
 setup(
     name="NewsArticlesScraper",
     version=VERSION,
```

