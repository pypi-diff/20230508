# Comparing `tmp/scrapy-poet-0.8.0.tar.gz` & `tmp/scrapy-poet-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-poet-0.8.0.tar", last modified: Tue Jan 24 12:36:02 2023, max compression
+gzip compressed data, was "scrapy-poet-0.9.0.tar", last modified: Fri Feb 17 02:34:35 2023, max compression
```

## Comparing `scrapy-poet-0.8.0.tar` & `scrapy-poet-0.9.0.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 12:36:02.709028 scrapy-poet-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-01-24 12:36:02.709028 scrapy-poet-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 12:36:02.705028 scrapy-poet-0.8.0/scrapy_poet/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/scrapy_poet/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/scrapy_poet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/scrapy_poet/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/scrapy_poet/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/scrapy_poet/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/scrapy_poet/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/scrapy_poet/downloadermiddlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)    15952 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/scrapy_poet/injection.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/scrapy_poet/injection_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/scrapy_poet/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/scrapy_poet/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/scrapy_poet/page_input_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/scrapy_poet/spidermiddlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/scrapy_poet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 12:36:02.705028 scrapy-poet-0.8.0/scrapy_poet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-01-24 12:36:02.000000 scrapy-poet-0.8.0/scrapy_poet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-01-24 12:36:02.000000 scrapy-poet-0.8.0/scrapy_poet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 12:36:02.000000 scrapy-poet-0.8.0/scrapy_poet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-24 12:36:02.000000 scrapy-poet-0.8.0/scrapy_poet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-24 12:36:02.000000 scrapy-poet-0.8.0/scrapy_poet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-24 12:36:02.000000 scrapy-poet-0.8.0/scrapy_poet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 12:36:02.709028 scrapy-poet-0.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1588 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 12:36:02.709028 scrapy-poet-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/mockserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 12:36:02.709028 scrapy-poet-0.8.0/tests/po_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/po_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/test_callback_for.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    20173 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16110 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/test_injection.py
--rw-r--r--   0 runner    (1001) docker     (123)    15564 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/test_page_input_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/test_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/test_response_required_logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/test_retries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/test_scrapy_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-01-24 12:35:54.000000 scrapy-poet-0.8.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:34:35.123965 scrapy-poet-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-02-17 02:34:35.123965 scrapy-poet-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:34:35.119965 scrapy-poet-0.9.0/scrapy_poet/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/scrapy_poet/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/scrapy_poet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/scrapy_poet/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/scrapy_poet/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/scrapy_poet/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/scrapy_poet/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/scrapy_poet/downloadermiddlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/scrapy_poet/injection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/scrapy_poet/injection_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/scrapy_poet/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15547 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/scrapy_poet/page_input_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/scrapy_poet/spidermiddlewares.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:34:35.123965 scrapy-poet-0.9.0/scrapy_poet/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/scrapy_poet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/scrapy_poet/utils/mockserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/scrapy_poet/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:34:35.119965 scrapy-poet-0.9.0/scrapy_poet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-02-17 02:34:35.000000 scrapy-poet-0.9.0/scrapy_poet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-17 02:34:35.000000 scrapy-poet-0.9.0/scrapy_poet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 02:34:35.000000 scrapy-poet-0.9.0/scrapy_poet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-17 02:34:35.000000 scrapy-poet-0.9.0/scrapy_poet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-17 02:34:35.000000 scrapy-poet-0.9.0/scrapy_poet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-17 02:34:35.000000 scrapy-poet-0.9.0/scrapy_poet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 02:34:35.123965 scrapy-poet-0.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1588 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:34:35.123965 scrapy-poet-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/tests/test_callback_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22947 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15877 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/tests/test_injection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/tests/test_page_input_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/tests/test_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12595 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/tests/test_response_required_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/tests/test_retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/tests/test_scrapy_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53722 2023-02-17 02:34:22.000000 scrapy-poet-0.9.0/tests/test_web_poet_rules.py
```

### Comparing `scrapy-poet-0.8.0/LICENSE` & `scrapy-poet-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-poet-0.8.0/PKG-INFO` & `scrapy-poet-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-poet
-Version: 0.8.0
+Version: 0.9.0
 Summary: Page Object pattern for Scrapy
 Home-page: https://github.com/scrapinghub/scrapy-poet
 Author: Mikhail Korobov
 Author-email: kmike84@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `scrapy-poet-0.8.0/README.rst` & `scrapy-poet-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `scrapy-poet-0.8.0/scrapy_poet/api.py` & `scrapy-poet-0.9.0/scrapy_poet/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,41 +4,44 @@
 from scrapy.http import Request, Response
 from web_poet.pages import ItemPage
 
 _CALLBACK_FOR_MARKER = "__scrapy_poet_callback"
 
 
 class DummyResponse(Response):
-    """This class is returned by the ``InjectionMiddleware`` when it detects
-    that the download could be skipped. It inherits from Scrapy ``Response``
-    and signals and stores the URL and references the original ``Request``.
+    """This class is returned by the
+    :class:`~.InjectionMiddleware` when it detects that the download could be
+    skipped. It inherits from :class:`scrapy.http.Response` and signals and
+    stores the URL and references the original :class:`scrapy.Request
+    <scrapy.http.Request>`.
 
     If you want to skip downloads, you can type annotate your parse method
     with this class.
 
     .. code-block:: python
 
         def parse(self, response: DummyResponse):
             pass
 
-    If there's no Page Input that depends on a Scrapy ``Response``, the
-    ``InjectionMiddleware`` is going to skip download and provide a
-    ``DummyResponse`` to your parser instead.
+    If there's no Page Input that depends on a :class:`scrapy.http.Response`, the
+    :class:`~.InjectionMiddleware` is going to skip download and provide a
+    :class:`~.DummyResponse` to your parser instead.
     """
 
     def __init__(self, url: str, request=Optional[Request]):
         super().__init__(url=url, request=request)
 
 
-def callback_for(page_cls: Type[ItemPage]) -> Callable:
-    """Create a callback for an :class:`web_poet.pages.ItemPage` subclass.
+def callback_for(page_or_item_cls: Type) -> Callable:
+    """Create a callback for an :class:`web_poet.ItemPage <web_poet.pages.ItemPage>`
+    subclass or an item class.
 
     The generated callback returns the output of the
-    ``ItemPage.to_item()`` method, i.e. extracts a single item
-    from a web page, using a Page Object.
+    :meth:`to_item <web_poet.pages.ItemPage.to_item>` method, i.e. extracts a single
+    item from a web page, using a Page Object.
 
     This helper allows to reduce the boilerplate when working
     with Page Objects. For example, instead of this:
 
     .. code-block:: python
 
         class BooksSpider(scrapy.Spider):
@@ -63,15 +66,16 @@
             def parse(self, response):
                 links = response.css(".image_container a")
                 yield from response.follow_all(links, self.parse_book)
 
             parse_book = callback_for(BookPage)
 
     It also supports producing an async generator callable if the Page Objects's
-    ``to_item()`` method is a coroutine which uses the ``async/await`` syntax.
+    :meth:`to_item <web_poet.pages.ItemPage.to_item>` method is a coroutine
+    which uses the ``async/await`` syntax.
 
     So if we have the following:
 
     .. code-block:: python
 
         class BooksSpider(scrapy.Spider):
             name = "books"
@@ -100,28 +104,32 @@
 
     The generated callback could be used as a spider instance method or passed
     as an inline/anonymous argument. Make sure to define it as a spider
     attribute (as shown in the example above) if you're planning to use
     disk queues, because in this case Scrapy is able to serialize
     your request object.
     """
-    if not issubclass(page_cls, ItemPage):
-        raise TypeError(f"{page_cls.__name__} should be a subclass of ItemPage.")
-
     # When the callback is used as an instance method of the spider, it expects
     # to receive 'self' as its first argument. When used as a simple inline
     # function, it expects to receive a response as its first argument.
     #
     # To avoid a TypeError, we need to receive a list of unnamed arguments and
     # a dict of named arguments after our injectable.
-    def parse(*args, page: page_cls, **kwargs):  # type: ignore
-        yield page.to_item()  # type: ignore
+    if issubclass(page_or_item_cls, ItemPage):
+
+        def parse(*args, page: page_or_item_cls, **kwargs):  # type: ignore
+            yield page.to_item()  # type: ignore
+
+        async def async_parse(*args, page: page_or_item_cls, **kwargs):  # type: ignore
+            yield await page.to_item()  # type: ignore
+
+        if iscoroutinefunction(page_or_item_cls.to_item):
+            setattr(async_parse, _CALLBACK_FOR_MARKER, True)
+            return async_parse
 
-    async def async_parse(*args, page: page_cls, **kwargs):  # type: ignore
-        yield await page.to_item()  # type: ignore
+    else:
 
-    if iscoroutinefunction(page_cls.to_item):
-        setattr(async_parse, _CALLBACK_FOR_MARKER, True)
-        return async_parse
+        def parse(*args, item: page_or_item_cls, **kwargs):  # type:ignore
+            yield item
 
     setattr(parse, _CALLBACK_FOR_MARKER, True)
     return parse
```

### Comparing `scrapy-poet-0.8.0/scrapy_poet/cache.py` & `scrapy-poet-0.9.0/scrapy_poet/cache.py`

 * *Files identical despite different names*

### Comparing `scrapy-poet-0.8.0/scrapy_poet/commands.py` & `scrapy-poet-0.9.0/scrapy_poet/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 class SavingInjectionMiddleware(InjectionMiddleware):
     def __init__(self, crawler: Crawler) -> None:
         super().__init__(crawler)
         self.injector = SavingInjector(
             crawler,
             default_providers=DEFAULT_PROVIDERS,
-            overrides_registry=self.overrides_registry,
+            registry=self.registry,
         )
 
 
 def spider_for(injectable: Type[ItemPage]) -> Type[scrapy.Spider]:
     class InjectableSpider(scrapy.Spider):
         name = "injectable"
         url = None
@@ -81,20 +81,22 @@
         if not issubclass(cls, ItemPage):
             raise UsageError(f"Error: {type_name} is not a descendant of ItemPage")
 
         spider_cls = spider_for(cls)
         self.settings["ITEM_PIPELINES"][SavingPipeline] = 100
         self.settings["DOWNLOADER_MIDDLEWARES"][SavingInjectionMiddleware] = 543
 
-        frozen_time = datetime.datetime.now(datetime.timezone.utc)
+        frozen_time = datetime.datetime.now(datetime.timezone.utc).replace(
+            microsecond=0
+        )
         with time_machine.travel(frozen_time):
             self.crawler_process.crawl(spider_cls, url=url)
             self.crawler_process.start()
 
         deps = saved_dependencies
         item = saved_items[0]
         meta = {
-            "frozen_time": frozen_time.isoformat(),
+            "frozen_time": frozen_time.isoformat(timespec="seconds"),
         }
         basedir = Path(self.settings.get("SCRAPY_POET_TESTS_DIR", "fixtures"))
         fixture = Fixture.save(basedir / type_name, inputs=deps, item=item, meta=meta)
         print(f"\nThe test fixture has been written to {fixture.path}.")
```

### Comparing `scrapy-poet-0.8.0/scrapy_poet/downloader.py` & `scrapy-poet-0.9.0/scrapy_poet/downloader.py`

 * *Files identical despite different names*

### Comparing `scrapy-poet-0.8.0/scrapy_poet/downloadermiddlewares.py` & `scrapy-poet-0.9.0/scrapy_poet/downloadermiddlewares.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,37 +6,39 @@
 import logging
 import warnings
 from typing import Generator, Optional, Type, TypeVar
 
 from scrapy import Spider, signals
 from scrapy.crawler import Crawler
 from scrapy.http import Request, Response
-from scrapy.utils.misc import create_instance, load_object
 from twisted.internet.defer import Deferred, inlineCallbacks
+from web_poet import RulesRegistry
 
 from .api import DummyResponse
 from .injection import Injector
-from .overrides import OverridesRegistry
 from .page_input_providers import (
     HttpClientProvider,
     HttpResponseProvider,
+    ItemProvider,
     PageParamsProvider,
     RequestUrlProvider,
     ResponseUrlProvider,
 )
+from .utils import create_registry_instance, is_min_scrapy_version
 
 logger = logging.getLogger(__name__)
 
 
 DEFAULT_PROVIDERS = {
     HttpResponseProvider: 500,
     HttpClientProvider: 600,
     PageParamsProvider: 700,
     RequestUrlProvider: 800,
     ResponseUrlProvider: 900,
+    ItemProvider: 1000,
 }
 
 InjectionMiddlewareTV = TypeVar("InjectionMiddlewareTV", bound="InjectionMiddleware")
 
 
 class InjectionMiddleware:
     """This is a Downloader Middleware that's supposed to:
@@ -44,23 +46,19 @@
     * check if request downloads could be skipped
     * inject dependencies before request callbacks are executed
     """
 
     def __init__(self, crawler: Crawler) -> None:
         """Initialize the middleware"""
         self.crawler = crawler
-        settings = self.crawler.settings
-        registry_cls = load_object(
-            settings.get("SCRAPY_POET_OVERRIDES_REGISTRY", OverridesRegistry)
-        )
-        self.overrides_registry = create_instance(registry_cls, settings, crawler)
+        self.registry = create_registry_instance(RulesRegistry, crawler)
         self.injector = Injector(
             crawler,
             default_providers=DEFAULT_PROVIDERS,
-            overrides_registry=self.overrides_registry,
+            registry=self.registry,
         )
 
     @classmethod
     def from_crawler(
         cls: Type[InjectionMiddlewareTV], crawler: Crawler
     ) -> InjectionMiddlewareTV:
         o = cls(crawler)
@@ -70,35 +68,42 @@
     def spider_closed(self, spider: Spider) -> None:
         self.injector.close()
 
     def process_request(
         self, request: Request, spider: Spider
     ) -> Optional[DummyResponse]:
         """This method checks if the request is really needed and if its
-        download could be skipped by trying to infer if a ``Response``
+        download could be skipped by trying to infer if a :class:`scrapy.http.Response`
         is going to be used by the callback or a Page Input.
 
-        If the ``Response`` can be ignored, a ``utils.DummyResponse`` object is
-        returned on its place. This ``DummyResponse`` is linked to the original
-        ``Request`` instance.
+        If the :class:`scrapy.http.Response` can be ignored, a
+        :class:`~.DummyResponse` instance is returned on its place. This
+        :class:`~.DummyResponse` is linked to the original :class:`scrapy.Request
+        <scrapy.http.Request>` instance.
 
         With this behavior, we're able to optimize spider executions avoiding
         unnecessary downloads. That could be the case when the callback is
         actually using another source like external APIs such as Zyte's
         AutoExtract.
         """
         if self.injector.is_scrapy_response_required(request):
             return None
 
         logger.debug(f"Using DummyResponse instead of downloading {request}")
         self.crawler.stats.inc_value("scrapy_poet/dummy_response_count")
         return DummyResponse(url=request.url, request=request)
 
     def _skip_dependency_creation(self, request: Request, spider: Spider) -> bool:
-        """See: https://github.com/scrapinghub/scrapy-poet/issues/48"""
+        """See:
+
+        * https://github.com/scrapinghub/scrapy-poet/issues/48  — scrapy <  2.8
+        * https://github.com/scrapinghub/scrapy-poet/issues/118 — scrapy >= 2.8
+        """
+        if is_min_scrapy_version("2.8.0"):
+            return False
 
         # No need to skip if the callback doesn't default to the parse() method
         if request.callback is not None:
             return False
 
         # If the Request.cb_kwargs possess all of the cb dependencies, then no
         # warning message should be issued.
@@ -113,35 +118,33 @@
             return True
 
         return False
 
     @inlineCallbacks
     def process_response(
         self, request: Request, response: Response, spider: Spider
-    ) -> Generator[Deferred[object], object, Response]:
-        """This method fills ``request.cb_kwargs`` with instances for
-        the required Page Objects found in the callback signature.
-
-        In other words, this method instantiates all ``Injectable``
-        subclasses declared as request callback arguments and
-        any other parameter with a ``PageObjectInputProvider`` configured for
-        its type.
-
-        If there's a collision between an already set ``cb_kwargs``
-        and an injectable attribute,
-        the user-defined ``cb_kwargs`` takes precedence.
+    ) -> Generator[Deferred, object, Response]:
+        """This method fills :attr:`scrapy.Request.cb_kwargs
+        <scrapy.http.Request.cb_kwargs>` with instances for the required Page
+        Objects found in the callback signature.
+
+        In other words, this method instantiates all :class:`web_poet.Injectable
+        <web_poet.pages.Injectable>` subclasses declared as request callback
+        arguments and any other parameter with a :class:`~.PageObjectInputProvider`
+        configured for its type.
         """
         if self._skip_dependency_creation(request, spider):
             warnings.warn(
                 "A request has been encountered with callback=None which "
                 "defaults to the parse() method. On such cases, annotated "
                 "dependencies in the parse() method won't be built by "
                 "scrapy-poet. However, if the request has callback=parse, "
                 "the annotated dependencies will be built.\n\n"
-                "See the Pitfalls doc for more info."
+                "See the Pitfalls doc for more info.",
+                stacklevel=2,
             )
             return response
 
         # Find out the dependencies
         final_kwargs = yield from self.injector.build_callback_dependencies(
             request,
             response,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scrapy-poet-0.8.0/scrapy_poet/injection.py` & `scrapy-poet-0.9.0/scrapy_poet/injection.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 from scrapy import Request, Spider
 from scrapy.crawler import Crawler
 from scrapy.http import Response
 from scrapy.settings import Settings
 from scrapy.statscollectors import StatsCollector
 from scrapy.utils.conf import build_component_list
 from scrapy.utils.defer import maybeDeferred_coro
-from scrapy.utils.misc import create_instance, load_object
+from scrapy.utils.misc import load_object
 from twisted.internet.defer import inlineCallbacks
+from web_poet import RulesRegistry
 from web_poet.pages import is_injectable
 
 from scrapy_poet.api import _CALLBACK_FOR_MARKER, DummyResponse
 from scrapy_poet.cache import SqlitedictCache
 from scrapy_poet.injection_errors import (
     InjectionError,
     NonCallableProviderError,
     UndeclaredProvidedTypeError,
 )
-from scrapy_poet.overrides import OverridesRegistry, OverridesRegistryBase
 from scrapy_poet.page_input_providers import PageObjectInputProvider
+from scrapy_poet.utils import is_min_scrapy_version
 
-from .utils import get_scrapy_data_path
+from .utils import create_registry_instance, get_scrapy_data_path
 
 logger = logging.getLogger(__name__)
 
 
 class Injector:
     """
     Keep all the logic required to do dependency injection in Scrapy callbacks.
@@ -39,30 +40,30 @@
     """
 
     def __init__(
         self,
         crawler: Crawler,
         *,
         default_providers: Optional[Mapping] = None,
-        overrides_registry: Optional[OverridesRegistryBase] = None,
+        registry: Optional[RulesRegistry] = None,
     ):
         self.crawler = crawler
         self.spider = crawler.spider
-        self.overrides_registry = overrides_registry or OverridesRegistry()
+        self.registry = registry or RulesRegistry()
         self.load_providers(default_providers)
         self.init_cache()
 
     def load_providers(self, default_providers: Optional[Mapping] = None):  # noqa: D102
         providers_dict = {
             **(default_providers or {}),
             **self.crawler.settings.getdict("SCRAPY_POET_PROVIDERS"),
         }
         provider_classes = build_component_list(providers_dict)
         logger.info(f"Loading providers:\n {pprint.pformat(provider_classes)}")
-        self.providers = [load_object(cls)(self.crawler) for cls in provider_classes]
+        self.providers = [load_object(cls)(self) for cls in provider_classes]
         check_all_providers_are_callable(self.providers)
         # Caching whether each provider requires the scrapy response
         self.is_provider_requiring_scrapy_response = {
             provider: is_provider_requiring_scrapy_response(provider)
             for provider in self.providers
         }
         # Caching the function for faster execution
@@ -116,15 +117,16 @@
                 if provider.is_provided(cls):
                     result.add(provider)
 
         return result
 
     def is_scrapy_response_required(self, request: Request):
         """
-        Check whether the request's response is going to be used.
+        Check whether Scrapy's :class:`~scrapy.http.Request`'s
+        :class:`~scrapy.http.Response` is going to be used.
         """
         callback = get_callback(request, self.spider)
         if is_callback_requiring_scrapy_response(callback, request.callback):
             return True
 
         for provider in self.discover_callback_providers(request):
             if self.is_provider_requiring_scrapy_response[provider]:
@@ -135,15 +137,18 @@
     def build_plan(self, request: Request) -> andi.Plan:
         """Create a plan for building the dependencies required by the callback"""
         callback = get_callback(request, self.spider)
         return andi.plan(
             callback,
             is_injectable=is_injectable,
             externally_provided=self.is_class_provided_by_any_provider,
-            overrides=self.overrides_registry.overrides_for(request).get,
+            # Ignore the type since andi.plan expects overrides to be
+            # Callable[[Callable], Optional[Callable]] but the registry
+            # returns the typing for ``dict.get()`` method.
+            overrides=self.registry.overrides_for(request.url).get,  # type: ignore[arg-type]
         )
 
     @inlineCallbacks
     def build_instances(self, request: Request, response: Response, plan: andi.Plan):
         """Build the instances dict from a plan including external dependencies."""
         # First we build the external dependencies using the providers
         instances = yield from self.build_instances_from_providers(
@@ -263,15 +268,15 @@
     providers: List[PageObjectInputProvider],
 ) -> Callable[[Callable], bool]:
     """
     Return a function of type ``Callable[[Type], bool]`` that return
     True if the given type is provided by any of the registered providers.
 
     The attribute ``provided_classes`` from each provided is used.
-    This attribute can be a ``set`` or a ``Callable``. All sets are
+    This attribute can be a :class:`set` or a ``Callable``. All sets are
     joined together for efficiency.
     """
     sets_of_types: Set[Callable] = set()  # caching all sets found
     individual_is_callable: List[Callable[[Callable], bool]] = [
         sets_of_types.__contains__
     ]
     for provider in providers:
@@ -294,30 +299,32 @@
                 return True
         return False
 
     return is_provided_fn
 
 
 def get_callback(request, spider):
-    """Get ``request.callback`` of a :class:`scrapy.Request`"""
+    """Get the :attr:`scrapy.Request.callback <scrapy.http.Request.callback>` of
+    a :class:`scrapy.Request <scrapy.http.Request>`.
+    """
     if request.callback is None:
         return getattr(spider, "parse")  # noqa: B009
     return request.callback
 
 
 _unset = object()
 
 
 def is_callback_requiring_scrapy_response(
     callback: Callable, raw_callback: Any = _unset
 ) -> bool:
     """
     Check whether the request's callback method requires the response.
     Basically, it won't be required if the response argument in the
-    callback is annotated with ``DummyResponse``
+    callback is annotated with :class:`~.DummyResponse`.
     """
     if getattr(callback, _CALLBACK_FOR_MARKER, False) is True:
         # The callback_for function was used to create this callback.
         return False
 
     signature = inspect.signature(callback)
     first_parameter_key = next(iter(signature.parameters))
@@ -329,15 +336,16 @@
 
     if first_parameter.annotation is first_parameter.empty:
         # There's no type annotation, so we're probably using response here.
         return True
 
     if issubclass(first_parameter.annotation, DummyResponse):
         # See: https://github.com/scrapinghub/scrapy-poet/issues/48
-        if raw_callback is None:
+        # See: https://github.com/scrapinghub/scrapy-poet/issues/118
+        if raw_callback is None and not is_min_scrapy_version("2.8.0"):
             warnings.warn(
                 "A request has been encountered with callback=None which "
                 "defaults to the parse() method. If the parse() method is "
                 "annotated with scrapy_poet.DummyResponse (or its subclasses), "
                 "we're assuming this isn't intended and would simply ignore "
                 "this annotation.\n\n"
                 "See the Pitfalls doc for more info."
@@ -358,15 +366,17 @@
     Crawler,
     Settings,
     StatsCollector,
 }
 
 
 def is_provider_requiring_scrapy_response(provider):
-    """Check whether injectable provider makes use of a valid Response."""
+    """Check whether injectable provider makes use of a valid
+    :class:`scrapy.http.Response`.
+    """
     plan = andi.plan(
         provider.__call__,
         is_injectable=is_injectable,
         externally_provided=SCRAPY_PROVIDED_CLASSES,
     )
     for possible_type, _ in plan.dependencies:
         if issubclass(possible_type, Response):
@@ -374,15 +384,15 @@
 
     return False
 
 
 def get_injector_for_testing(
     providers: Mapping,
     additional_settings: Optional[Dict] = None,
-    overrides_registry: Optional[OverridesRegistryBase] = None,
+    registry: Optional[RulesRegistry] = None,
 ) -> Injector:
     """
     Return an :class:`Injector` using a fake crawler.
     Useful for testing providers
     """
 
     class MySpider(Spider):
@@ -392,23 +402,23 @@
         {**(additional_settings or {}), "SCRAPY_POET_PROVIDERS": providers}
     )
     crawler = Crawler(MySpider)
     crawler.settings = settings
     spider = MySpider()
     spider.settings = settings
     crawler.spider = spider
-    if not overrides_registry:
-        overrides_registry = create_instance(OverridesRegistry, settings, crawler)
-    return Injector(crawler, overrides_registry=overrides_registry)
+    if not registry:
+        registry = create_registry_instance(RulesRegistry, crawler)
+    return Injector(crawler, registry=registry)
 
 
 def get_response_for_testing(callback: Callable) -> Response:
     """
-    Return a response with fake content with the configured callback.
-    It is useful for testing providers.
+    Return a :class:`scrapy.http.Response` with fake content with the configured
+    callback. It is useful for testing providers.
     """
     url = "http://example.com"
     html = """
         <html>
             <body>
                 <div class="breadcrumbs">
                     <a href="/food">Food</a> /
```

### Comparing `scrapy-poet-0.8.0/scrapy_poet.egg-info/PKG-INFO` & `scrapy-poet-0.9.0/scrapy_poet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-poet
-Version: 0.8.0
+Version: 0.9.0
 Summary: Page Object pattern for Scrapy
 Home-page: https://github.com/scrapinghub/scrapy-poet
 Author: Mikhail Korobov
 Author-email: kmike84@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `scrapy-poet-0.8.0/scrapy_poet.egg-info/SOURCES.txt` & `scrapy-poet-0.9.0/scrapy_poet.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,34 +9,33 @@
 scrapy_poet/cache.py
 scrapy_poet/commands.py
 scrapy_poet/downloader.py
 scrapy_poet/downloadermiddlewares.py
 scrapy_poet/injection.py
 scrapy_poet/injection_errors.py
 scrapy_poet/middleware.py
-scrapy_poet/overrides.py
 scrapy_poet/page_input_providers.py
 scrapy_poet/spidermiddlewares.py
-scrapy_poet/utils.py
 scrapy_poet.egg-info/PKG-INFO
 scrapy_poet.egg-info/SOURCES.txt
 scrapy_poet.egg-info/dependency_links.txt
 scrapy_poet.egg-info/entry_points.txt
 scrapy_poet.egg-info/requires.txt
 scrapy_poet.egg-info/top_level.txt
+scrapy_poet/utils/__init__.py
+scrapy_poet/utils/mockserver.py
+scrapy_poet/utils/testing.py
 tests/__init__.py
 tests/conftest.py
-tests/mockserver.py
 tests/test_cache.py
 tests/test_callback_for.py
 tests/test_commands.py
 tests/test_downloader.py
 tests/test_injection.py
 tests/test_middleware.py
 tests/test_page_input_providers.py
 tests/test_providers.py
 tests/test_response_required_logic.py
 tests/test_retries.py
 tests/test_scrapy_dependencies.py
 tests/test_utils.py
-tests/utils.py
-tests/po_lib/__init__.py
+tests/test_web_poet_rules.py
```

### Comparing `scrapy-poet-0.8.0/setup.py` & `scrapy-poet-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `scrapy-poet-0.8.0/tests/mockserver.py` & `scrapy-poet-0.9.0/scrapy_poet/utils/mockserver.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def __enter__(self):
         self.proc = Popen(
             [
                 sys.executable,
                 "-u",
                 "-m",
-                "tests.mockserver",
+                "scrapy_poet.utils.mockserver",
                 self.resource,
                 "--port",
                 str(self.port),
             ],
             stdout=PIPE,
         )
         self.proc.stdout.readline()
```

### Comparing `scrapy-poet-0.8.0/tests/test_cache.py` & `scrapy-poet-0.9.0/tests/test_cache.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from tempfile import NamedTemporaryFile
 
 from pytest_twisted import inlineCallbacks
 from scrapy import Request, Spider
 from web_poet import WebPage, field
 
-from .mockserver import MockServer
-from .utils import EchoResource, make_crawler
+from scrapy_poet.utils.mockserver import MockServer
+from scrapy_poet.utils.testing import EchoResource, make_crawler
 
 
 @inlineCallbacks
 def test_cache_no_errors(caplog) -> None:
     with NamedTemporaryFile() as cache_file:
         with MockServer(EchoResource) as server:
```

### Comparing `scrapy-poet-0.8.0/tests/test_callback_for.py` & `scrapy-poet-0.9.0/tests/test_callback_for.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,20 +123,7 @@
     cb = callback_for(FakeItemPageAsync)
     request = scrapy.Request("http://example.com/", callback=cb)
     with pytest.raises(ValueError) as exc:
         request.to_dict(spider=spider)
 
     msg = f"Function {cb} is not an instance method in: {spider}"
     assert str(exc.value) == msg
-
-
-def test_invalid_subclass():
-    """Classes should inherit from ItemPage."""
-
-    class MyClass(object):
-        pass
-
-    with pytest.raises(TypeError) as exc:
-        callback_for(MyClass)
-
-    msg = "MyClass should be a subclass of ItemPage."
-    assert str(exc.value) == msg
```

### Comparing `scrapy-poet-0.8.0/tests/test_downloader.py` & `scrapy-poet-0.9.0/tests/test_downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 from scrapy.exceptions import IgnoreRequest
 from web_poet import HttpClient
 from web_poet.exceptions import HttpError, HttpRequestError, HttpResponseError
 from web_poet.pages import WebPage
 
 from scrapy_poet import DummyResponse
 from scrapy_poet.downloader import create_scrapy_downloader
-from scrapy_poet.utils import http_request_to_scrapy_request
-from tests.utils import (
+from scrapy_poet.utils import http_request_to_scrapy_request, is_min_scrapy_version
+from scrapy_poet.utils.mockserver import MockServer
+from scrapy_poet.utils.testing import (
     AsyncMock,
     DelayedResource,
     EchoResource,
-    MockServer,
     StatusResource,
     make_crawler,
 )
 
 
 @pytest.fixture
 def scrapy_downloader() -> Callable:
@@ -430,19 +430,19 @@
         "DOWNLOADER_MIDDLEWARES": {
             "scrapy_poet.InjectionMiddleware": 543,
         },
     }
 
 
 # See: https://github.com/scrapinghub/scrapy-poet/issues/48
-def _assert_warning_messages(record, index: Optional[List] = None):
+def _assert_warning_messages(
+    record, index: Optional[List] = None, not_existing: bool = False
+):
     index = index or [0, 1]
 
-    assert len(index) == len(record.list), "Differing number of warnings"
-
     expected_warnings = [
         # From injection.py:
         "A request has been encountered with callback=None which "
         "defaults to the parse() method. If the parse() method is "
         "annotated with scrapy_poet.DummyResponse (or its subclasses), "
         "we're assuming this isn't intended and would simply ignore "
         "this annotation.\n\n"
@@ -452,18 +452,31 @@
         "defaults to the parse() method. On such cases, annotated "
         "dependencies in the parse() method won't be built by "
         "scrapy-poet. However, if the request has callback=parse, "
         "the annotated dependencies will be built.\n\n"
         "See the Pitfalls doc for more info.",
     ]
 
-    for idx, result_warning in zip(index, record.list):
-        assert expected_warnings[idx] in str(result_warning.message)
+    expected_warning_found = [False] * len(index)
+
+    for result_warning in record.list:
+        for idx in index:
+            if expected_warnings[idx] in str(result_warning.message):
+                expected_warning_found[idx] = True
+
+    if not not_existing:
+        assert all(expected_warning_found)
+    else:
+        assert not any(expected_warning_found)
 
 
+@pytest.mark.skipif(
+    is_min_scrapy_version("2.8.0"),
+    reason="tests Scrapy < 2.8 before NO_CALLBACK was introduced",
+)
 @inlineCallbacks
 def test_parse_callback_none_dummy_response() -> None:
     """If request.callback == None and the parse() method only has a single
     parameter of ``response: DummyResponse``, then a warning should be issued.
 
     This also means that even if the response is annotated with ``DummyResponse``,
     it's still downloaded as opposed to being skipped.
@@ -484,14 +497,18 @@
         with pytest.warns(UserWarning) as record:
             yield crawler.crawl()
 
     _assert_warning_messages(record, index=[0])
     assert not isinstance(collected["response"], DummyResponse)
 
 
+@pytest.mark.skipif(
+    is_min_scrapy_version("2.8.0"),
+    reason="tests Scrapy < 2.8 before NO_CALLBACK was introduced",
+)
 @inlineCallbacks
 def test_parse_callback_none_response() -> None:
     """Similar to ``test_parse_callback_none_dummy_response()`` but instead of
     ``response: DummyResponse``, it's ``response: scrapy.http.Response``.
 
     No warnings should be issued here.
     """
@@ -504,21 +521,25 @@
             start_urls = [server.root_url]
 
             def parse(self, response: scrapy.http.Response):
                 collected["response"] = response
 
         crawler = make_crawler(TestSpider, {})
 
-        with warnings.catch_warnings(record=True) as warning_msg:
+        with pytest.warns(UserWarning) as record:
             yield crawler.crawl()
 
-    assert not warning_msg
+    _assert_warning_messages(record, not_existing=True)
     assert not isinstance(collected["response"], DummyResponse)
 
 
+@pytest.mark.skipif(
+    is_min_scrapy_version("2.8.0"),
+    reason="tests Scrapy < 2.8 before NO_CALLBACK was introduced",
+)
 @inlineCallbacks
 def test_parse_callback_none_no_annotated_deps() -> None:
     """Similar to ``test_parse_callback_none_dummy_response()`` but there are no
     annotated dependencies.
 
     No warnings should be issued here.
     """
@@ -538,14 +559,18 @@
         with warnings.catch_warnings(record=True) as warning_msg:
             yield crawler.crawl()
 
     assert not warning_msg
     assert isinstance(collected["response"], scrapy.http.Response)
 
 
+@pytest.mark.skipif(
+    is_min_scrapy_version("2.8.0"),
+    reason="tests Scrapy < 2.8 before NO_CALLBACK was introduced",
+)
 @inlineCallbacks
 def test_parse_callback_none_with_deps(caplog) -> None:
     """Same with the ``test_parse_callback_none_dummy_response`` test but it
     confirms that the other dependencies requested by the parse() method isn't
     injected.
 
     Moreover, it results in a TypeError in Scrapy due to the missing argument.
@@ -574,14 +599,18 @@
         expected_msg = (
             "TypeError: test_parse_callback_none_with_deps.<locals>.TestSpider"
             ".parse() missing 1 required positional argument: 'page'"
         )
     assert expected_msg in caplog.text
 
 
+@pytest.mark.skipif(
+    is_min_scrapy_version("2.8.0"),
+    reason="tests Scrapy < 2.8 before NO_CALLBACK was introduced",
+)
 @inlineCallbacks
 def test_parse_callback_none_with_deps_cb_kwargs(caplog) -> None:
     """Same with the ``test_parse_callback_none_with_deps`` but the dep is passed
     via the ``cb_kwargs`` Request parameter.
 
     No warnings should be issued here.
     """
@@ -604,14 +633,18 @@
             yield crawler.crawl()
 
     _assert_warning_messages(record, index=[0])
     assert not caplog.text  # no TypeError caused by missing ``page`` arg.
     assert not isinstance(collected["response"], DummyResponse)
 
 
+@pytest.mark.skipif(
+    is_min_scrapy_version("2.8.0"),
+    reason="tests Scrapy < 2.8 before NO_CALLBACK was introduced",
+)
 @inlineCallbacks
 def test_parse_callback_none_with_deps_cb_kwargs_incomplete(caplog) -> None:
     """Same with the ``test_parse_callback_none_with_deps_cb_kwargs`` but not
     all of the callback dependencies are available in the ``cb_kwargs`` Request
     parameter.
     """
 
@@ -647,7 +680,67 @@
         )
     else:
         expected_msg = (
             "TypeError: test_parse_callback_none_with_deps_cb_kwargs_incomplete."
             "<locals>.TestSpider.parse() missing 1 required positional argument: 'page2'"
         )
     assert expected_msg in caplog.text
+
+
+@pytest.mark.skipif(
+    not is_min_scrapy_version("2.8.0"),
+    reason="NO_CALLBACK not available in Scrapy < 2.8",
+)
+@inlineCallbacks
+def test_parse_callback_NO_CALLBACK(caplog) -> None:
+    """See: https://github.com/scrapinghub/scrapy-poet/issues/118"""
+
+    collected = {}
+
+    with MockServer(EchoResource) as server:
+
+        class TestSpider(BaseSpider):
+            start_urls = [server.root_url]
+
+            def parse(self, response: DummyResponse):
+                collected["response"] = response
+
+        crawler = make_crawler(TestSpider, {})
+
+        with pytest.warns(UserWarning) as record:
+            yield crawler.crawl()
+
+    _assert_warning_messages(record, not_existing=True)
+    assert not caplog.text
+    assert isinstance(collected["response"], DummyResponse)
+
+
+@pytest.mark.skipif(
+    not is_min_scrapy_version("2.8.0"),
+    reason="NO_CALLBACK not available in Scrapy < 2.8",
+)
+@inlineCallbacks
+def test_parse_callback_NO_CALLBACK_with_page_dep(caplog) -> None:
+    """See: https://github.com/scrapinghub/scrapy-poet/issues/118
+
+    Similar to ``test_parse_callback_NO_CALLBACK()`` but with a page object
+    dependency in ``parse()`` callback.
+    """
+
+    collected = {}
+
+    with MockServer(EchoResource) as server:
+
+        class TestSpider(BaseSpider):
+            start_urls = [server.root_url]
+
+            def parse(self, response: DummyResponse, page: BasicPage):
+                collected["response"] = response
+
+        crawler = make_crawler(TestSpider, {})
+
+        with pytest.warns(UserWarning) as record:
+            yield crawler.crawl()
+
+    _assert_warning_messages(record, not_existing=True)
+    assert not caplog.text
+    assert not isinstance(collected["response"], DummyResponse)
```

### Comparing `scrapy-poet-0.8.0/tests/test_injection.py` & `scrapy-poet-0.9.0/tests/test_injection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-import weakref
 from typing import Any, Callable, Sequence, Set
 
 import attr
 import parsel
 import pytest
 from pytest_twisted import inlineCallbacks
 from scrapy import Request
 from scrapy.http import Response
 from url_matcher import Patterns
 from url_matcher.util import get_domain
-from web_poet import Injectable, ItemPage
+from web_poet import Injectable, ItemPage, RulesRegistry
 from web_poet.mixins import ResponseShortcutsMixin
 from web_poet.rules import ApplyRule
 
 from scrapy_poet import (
     CacheDataProviderMixin,
     DummyResponse,
     HttpResponseProvider,
@@ -26,15 +25,14 @@
     is_class_provided_by_any_provider_fn,
 )
 from scrapy_poet.injection_errors import (
     InjectionError,
     NonCallableProviderError,
     UndeclaredProvidedTypeError,
 )
-from scrapy_poet.overrides import OverridesRegistry
 
 
 def get_provider(classes, content=None):
     class Provider(PageObjectInputProvider):
         provided_classes = classes
         require_response = False
 
@@ -112,20 +110,14 @@
 
         for provider in injector.providers:
             assert (
                 injector.is_provider_requiring_scrapy_response[provider]
                 == provider.require_response
             )
 
-        # Asserting that we are not leaking providers references
-        weak_ref = weakref.ref(injector.providers[0])
-        assert weak_ref()
-        del injector
-        assert weak_ref() is None
-
     def test_non_callable_provider_error(self):
         """Checks that a exception is raised when a provider is not callable"""
 
         class NonCallableProvider(PageObjectInputProvider):
             pass
 
         with pytest.raises(NonCallableProviderError):
@@ -319,22 +311,22 @@
 class TestInjectorOverrides:
     @pytest.mark.parametrize("override_should_happen", [True, False])
     @inlineCallbacks
     def test_overrides(self, providers, override_should_happen):
         domain = "example.com" if override_should_happen else "other-example.com"
         # The request domain is example.com, so overrides shouldn't be applied
         # when we configure them for domain other-example.com
-        overrides = [
-            (domain, PriceInDollarsPO, PricePO),
+        rules = [
+            ApplyRule(Patterns([domain]), use=PriceInDollarsPO, instead_of=PricePO),
             ApplyRule(
                 Patterns([domain]), use=OtherEurDollarRate, instead_of=EurDollarRate
             ),
         ]
-        registry = OverridesRegistry(overrides)
-        injector = get_injector_for_testing(providers, overrides_registry=registry)
+        registry = RulesRegistry(rules=rules)
+        injector = get_injector_for_testing(providers, registry=registry)
 
         def callback(
             response: DummyResponse, price_po: PricePO, rate_po: EurDollarRate
         ):
             pass
 
         response = get_response_for_testing(callback)
```

### Comparing `scrapy-poet-0.8.0/tests/test_middleware.py` & `scrapy-poet-0.9.0/tests/test_middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,26 @@
 from pytest_twisted import inlineCallbacks
 from scrapy import Request, Spider
 from scrapy.http import Response
 from scrapy.utils.log import configure_logging
 from scrapy.utils.test import get_crawler
 from twisted.internet.threads import deferToThread
 from url_matcher.util import get_domain
-from web_poet import default_registry
-from web_poet.page_inputs import HttpResponse, RequestUrl, ResponseUrl
-from web_poet.pages import ItemPage, WebPage
+from web_poet import ApplyRule, HttpResponse, ItemPage, RequestUrl, ResponseUrl, WebPage
 
 from scrapy_poet import DummyResponse, InjectionMiddleware, callback_for
 from scrapy_poet.cache import SqlitedictCache
 from scrapy_poet.page_input_providers import PageObjectInputProvider
-from tests.mockserver import get_ephemeral_port
-from tests.utils import HtmlResource, capture_exceptions, crawl_items, crawl_single_item
+from scrapy_poet.utils.mockserver import get_ephemeral_port
+from scrapy_poet.utils.testing import (
+    HtmlResource,
+    capture_exceptions,
+    crawl_items,
+    crawl_single_item,
+)
 
 
 class ProductHtml(HtmlResource):
     html = """
     <html>
         <div class="breadcrumbs">
             <a href="/food">Food</a> /
@@ -98,29 +101,45 @@
 
 
 @inlineCallbacks
 def test_overrides(settings):
     host = socket.gethostbyname(socket.gethostname())
     domain = get_domain(host)
     port = get_ephemeral_port()
-    settings["SCRAPY_POET_OVERRIDES"] = [
-        (f"{domain}:{port}", OverridenBreadcrumbsExtraction, BreadcrumbsExtraction)
+    settings["SCRAPY_POET_RULES"] = [
+        ApplyRule(
+            f"{domain}:{port}",
+            use=OverridenBreadcrumbsExtraction,
+            instead_of=BreadcrumbsExtraction,
+        )
     ]
     item, url, _ = yield crawl_single_item(
         spider_for(ProductPage), ProductHtml, settings, port=port
     )
     assert item == {
         "url": url,
         "name": "Chocolate",
         "price": "22€",
         "description": "The best chocolate ever",
         "category": "overriden_breadcrumb",
     }
 
 
+def test_deprecation_setting_SCRAPY_POET_OVERRIDES(settings) -> None:
+    settings["SCRAPY_POET_OVERRIDES"] = []
+    crawler = get_crawler(Spider, settings)
+
+    msg = (
+        "The SCRAPY_POET_OVERRIDES setting is deprecated. "
+        "Use SCRAPY_POET_RULES instead."
+    )
+    with pytest.warns(DeprecationWarning, match=msg):
+        InjectionMiddleware(crawler)
+
+
 @attr.s(auto_attribs=True)
 class OptionalAndUnionPage(WebPage):
     breadcrumbs: BreadcrumbsExtraction
     opt_check_1: Optional[BreadcrumbsExtraction]
     opt_check_2: Optional[str]  # str is not Injectable, so None expected here
     union_check_1: Union[BreadcrumbsExtraction, HttpResponse]  # Breadcrumbs is injected
     union_check_2: Union[str, HttpResponse]  # HttpResponse is injected
@@ -218,20 +237,20 @@
 def test_providers(settings, type_):
     item, _, _ = yield crawl_single_item(spider_for(type_), ProductHtml, settings)
     assert item["provided"].msg == "Provided 5!"
     assert item["provided"].response is None
 
 
 @inlineCallbacks
-def test_providers_returning_wrong_classes(settings):
+def test_providers_returning_wrong_classes(settings, caplog):
     """Injection Middleware should raise a runtime error whenever a provider
     returns instances of classes that they're not supposed to provide.
     """
-    with pytest.raises(AssertionError):
-        yield crawl_single_item(spider_for(ExtraClassData), ProductHtml, settings)
+    yield crawl_single_item(spider_for(ExtraClassData), ProductHtml, settings)
+    assert "UndeclaredProvidedTypeError:" in caplog.text
 
 
 class MultiArgsCallbackSpider(scrapy.Spider):
 
     url = None
     custom_settings = {"SCRAPY_POET_PROVIDERS": {WithDeferredProvider: 1}}
 
@@ -464,33 +483,7 @@
 
     spider = has_cache_middleware.crawler.spider
     has_cache_middleware.spider_closed(spider)
     assert mock_sqlitedictcache.mock_calls == [
         mock.call("/tmp/cache", compressed=True),
         mock.call().close(),
     ]
-
-
-@inlineCallbacks
-def test_web_poet_integration(settings):
-    """This tests scrapy-poet's integration with web-poet most especially when
-    populating override settings via:
-
-        from web_poet import default_registry
-
-        SCRAPY_POET_OVERRIDES = default_registry.get_rules()
-    """
-
-    # Only import them in this test scope since they need to be synced with
-    # the URL of the Page Object annotated with @handle_urls.
-    from tests.po_lib import PORT, POOverriden
-
-    # Override rules are defined in `tests/po_lib/__init__.py`.
-    rules = default_registry.get_rules()
-
-    # Converting it to a set removes potential duplicate ApplyRules
-    settings["SCRAPY_POET_OVERRIDES"] = set(rules)
-
-    item, url, _ = yield crawl_single_item(
-        spider_for(POOverriden), ProductHtml, settings, port=PORT
-    )
-    assert item == {"msg": "PO replacement"}
```

### Comparing `scrapy-poet-0.8.0/tests/test_page_input_providers.py` & `scrapy-poet-0.9.0/tests/test_page_input_providers.py`

 * *Files identical despite different names*

### Comparing `scrapy-poet-0.8.0/tests/test_providers.py` & `scrapy-poet-0.9.0/tests/test_providers.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 from typing import Any, Callable, List, Sequence, Set
 from unittest import mock
 
 import attr
 import scrapy
 from pytest_twisted import ensureDeferred, inlineCallbacks
 from scrapy import Request, Spider
-from scrapy.crawler import Crawler
 from scrapy.settings import Settings
 from scrapy.utils.test import get_crawler
 from twisted.python.failure import Failure
 from web_poet import HttpClient, HttpResponse
 
 from scrapy_poet import HttpResponseProvider
+from scrapy_poet.injection import Injector
 from scrapy_poet.page_input_providers import (
     CacheDataProviderMixin,
     HttpClientProvider,
+    ItemProvider,
     PageObjectInputProvider,
     PageParamsProvider,
 )
-from tests.utils import AsyncMock, HtmlResource, crawl_single_item
+from scrapy_poet.utils.testing import AsyncMock, HtmlResource, crawl_single_item
 
 
 class ProductHtml(HtmlResource):
     html = """
     <html>
         <div class="breadcrumbs">
             <a href="/food">Food</a> /
@@ -60,17 +61,17 @@
 
 
 class PriceHtmlDataProvider(PageObjectInputProvider, CacheDataProviderMixin):
 
     name = "price_html"
     provided_classes = {Price, Html}
 
-    def __init__(self, crawler: Crawler):
-        assert isinstance(crawler, Crawler)
-        super().__init__(crawler)
+    def __init__(self, injector: Injector):
+        assert isinstance(injector, Injector)
+        super().__init__(injector)
 
     def __call__(
         self, to_provide, response: scrapy.http.Response, spider: scrapy.Spider
     ):
         assert isinstance(spider, scrapy.Spider)
         ret: List[Any] = []
         if Price in to_provide:
@@ -203,40 +204,43 @@
         Html: Html("Price Html!"),
         "response_data_text": ProductHtml.html,
     }
 
 
 def test_response_data_provider_fingerprint(settings):
     crawler = get_crawler(Spider, settings)
-    rdp = HttpResponseProvider(crawler)
+    injector = Injector(crawler)
+    rdp = HttpResponseProvider(injector)
     request = scrapy.http.Request("https://example.com")
 
     # The fingerprint should be readable since it's JSON-encoded.
     fp = rdp.fingerprint(scrapy.http.Response, request)
     assert json.loads(fp)
 
 
 @ensureDeferred
 async def test_http_client_provider(settings):
     crawler = get_crawler(Spider, settings)
     crawler.engine = AsyncMock()
+    injector = Injector(crawler)
 
     with mock.patch(
         "scrapy_poet.page_input_providers.create_scrapy_downloader"
     ) as mock_factory:
-        provider = HttpClientProvider(crawler)
+        provider = HttpClientProvider(injector)
         results = provider(set(), crawler)
         assert isinstance(results[0], HttpClient)
 
     assert results[0]._request_downloader == mock_factory.return_value
 
 
 def test_page_params_provider(settings):
     crawler = get_crawler(Spider, settings)
-    provider = PageParamsProvider(crawler)
+    injector = Injector(crawler)
+    provider = PageParamsProvider(injector)
     request = scrapy.http.Request("https://example.com")
 
     results = provider(set(), request)
 
     assert results[0] == {}
 
     expected_data = {"key": "value"}
@@ -247,7 +251,35 @@
 
     # Check that keys that are invalid Python variable names work.
     expected_data = {1: "a"}
     request.meta.update({"page_params": expected_data})
     results = provider(set(), request)
 
     assert results[0] == expected_data
+
+
+def test_item_provider_cache(settings):
+    """Note that the bulk of the tests for the ``ItemProvider`` alongside the
+    ``Injector`` is tested in ``tests/test_web_poet_rules.py``.
+
+    We'll only test its caching behavior here if its properly garbage collected.
+    """
+
+    crawler = get_crawler(Spider, settings)
+    injector = Injector(crawler)
+    provider = ItemProvider(injector)
+
+    assert len(provider._cached_instances) == 0
+
+    def inside():
+        request = Request("https://example.com")
+        provider.update_cache(request, {Name: Name("test")})
+        assert len(provider._cached_instances) == 1
+
+        cached_instance = provider.get_from_cache(request, Name)
+        assert isinstance(cached_instance, Name)
+
+    # The cache should be empty after the ``inside`` scope has finished which
+    # means that the corresponding ``request`` and the contents under it are
+    # garbage collected.
+    inside()
+    assert len(provider._cached_instances) == 0
```

### Comparing `scrapy-poet-0.8.0/tests/test_response_required_logic.py` & `scrapy-poet-0.9.0/tests/test_response_required_logic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from typing import Any, Dict
 
 import attr
 import pytest
 import scrapy
 from pytest_twisted import inlineCallbacks
 from scrapy.crawler import Crawler
@@ -16,14 +17,21 @@
     is_callback_requiring_scrapy_response,
     is_provider_requiring_scrapy_response,
 )
 from scrapy_poet.page_input_providers import (
     HttpResponseProvider,
     PageObjectInputProvider,
 )
+from scrapy_poet.utils import is_min_scrapy_version
+
+# See: https://github.com/scrapinghub/scrapy-poet/issues/118
+try:
+    from scrapy.http.request import NO_CALLBACK  # available on Scrapy >= 2.8
+except ImportError:
+    NO_CALLBACK = lambda: None  # noqa: E731
 
 
 @attr.s(auto_attribs=True)
 class DummyProductResponse:
 
     data: Dict[str, Any]
 
@@ -180,15 +188,19 @@
     # TextResponse, instead of using the Response type.
     assert is_provider_requiring_scrapy_response(TextProductProvider) is False
     assert is_provider_requiring_scrapy_response(DummyProductProvider) is False
     assert is_provider_requiring_scrapy_response(FakeProductProvider) is False
     assert is_provider_requiring_scrapy_response(StringProductProvider) is False
 
 
-def test_is_callback_using_response():
+@pytest.mark.skipif(
+    is_min_scrapy_version("2.8.0"),
+    reason="tests Scrapy < 2.8 before NO_CALLBACK was introduced",
+)
+def test_is_callback_using_response_for_scrapy28_below() -> None:
     spider = MySpider()
     request = Request("https://example.com", callback=lambda _: _)
     assert is_callback_requiring_scrapy_response(spider.parse, request.callback) is True
     assert (
         is_callback_requiring_scrapy_response(spider.parse2, request.callback) is True
     )
     assert (
@@ -264,19 +276,89 @@
         spider.parse4,
         spider.parse6,
         spider.parse8,
         spider.parse10,
     ):
         with pytest.warns(UserWarning) as record:
             assert (
-                is_callback_requiring_scrapy_response(method, request.callback) is True
+                is_callback_requiring_scrapy_response(method, request.callback) is True  # type: ignore[arg-type]
             )
             assert expected_warning in str(record.list[0].message)
 
 
+@pytest.mark.skipif(
+    not is_min_scrapy_version("2.8.0"),
+    reason="NO_CALLBACK not available in Scrapy < 2.8",
+)
+def test_is_callback_using_response_for_scrapy28_and_above() -> None:
+    spider = MySpider()
+    request_with_callback = Request("https://example.com", callback=lambda _: _)
+    request_no_callback = Request("https://example.com", callback=NO_CALLBACK)
+
+    with warnings.catch_warnings(record=True) as caught_warnings:
+        for request in [request_with_callback, request_no_callback]:
+            assert (
+                is_callback_requiring_scrapy_response(spider.parse, request.callback)
+                is True
+            )
+            assert (
+                is_callback_requiring_scrapy_response(spider.parse2, request.callback)
+                is True
+            )
+            assert (
+                is_callback_requiring_scrapy_response(spider.parse3, request.callback)
+                is False
+            )
+            assert (
+                is_callback_requiring_scrapy_response(spider.parse4, request.callback)
+                is False
+            )
+            assert (
+                is_callback_requiring_scrapy_response(spider.parse5, request.callback)
+                is True
+            )
+            assert (
+                is_callback_requiring_scrapy_response(spider.parse6, request.callback)
+                is False
+            )
+            assert (
+                is_callback_requiring_scrapy_response(spider.parse7, request.callback)
+                is True
+            )
+            assert (
+                is_callback_requiring_scrapy_response(spider.parse8, request.callback)
+                is False
+            )
+            assert (
+                is_callback_requiring_scrapy_response(spider.parse9, request.callback)
+                is True
+            )
+            assert (
+                is_callback_requiring_scrapy_response(spider.parse10, request.callback)
+                is False
+            )
+            assert (
+                is_callback_requiring_scrapy_response(spider.parse11, request.callback)
+                is True
+            )
+            assert (
+                is_callback_requiring_scrapy_response(spider.parse12, request.callback)
+                is True
+            )
+            # Callbacks created with the callback_for function won't make use of
+            # the response, but their providers might use them.
+            assert (
+                is_callback_requiring_scrapy_response(
+                    spider.callback_for_parse, request
+                )
+                is False
+            )
+    assert not caught_warnings
+
+
 @inlineCallbacks
 def test_is_response_going_to_be_used():
     crawler = Crawler(MySpider)
     spider = MySpider()
     crawler.spider = spider
 
     def response(request):
```

### Comparing `scrapy-poet-0.8.0/tests/test_retries.py` & `scrapy-poet-0.9.0/tests/test_retries.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 from pytest_twisted import inlineCallbacks
 from scrapy import Request, Spider
 from web_poet.exceptions import Retry
 from web_poet.page_inputs.http import HttpResponse
 from web_poet.pages import WebPage
 
-from tests.utils import EchoResource, MockServer, make_crawler
+from scrapy_poet.utils.mockserver import MockServer
+from scrapy_poet.utils.testing import EchoResource, make_crawler
 
 
 class BaseSpider(Spider):
     name = "test_spider"
 
     custom_settings = {
         "DOWNLOADER_MIDDLEWARES": {
```

### Comparing `scrapy-poet-0.8.0/tests/test_scrapy_dependencies.py` & `scrapy-poet-0.9.0/tests/test_scrapy_dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from web_poet.pages import WebPage
 
 from scrapy_poet.injection import SCRAPY_PROVIDED_CLASSES
 from scrapy_poet.page_input_providers import (
     HttpResponseProvider,
     PageObjectInputProvider,
 )
-from tests.utils import HtmlResource, crawl_items, crawl_single_item
+from scrapy_poet.utils.testing import HtmlResource, crawl_items, crawl_single_item
 
 
 class ProductHtml(HtmlResource):
 
     html = """
     <html>
         <div class="breadcrumbs">
```

### Comparing `scrapy-poet-0.8.0/tests/test_utils.py` & `scrapy-poet-0.9.0/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from pathlib import PosixPath
 from unittest import mock
 
 import pytest
+from scrapy import Spider
 from scrapy.http import Request, Response, TextResponse
+from scrapy.utils.test import get_crawler
 from web_poet import HttpRequest, HttpResponse
 
 from scrapy_poet.utils import (
+    create_registry_instance,
     get_scrapy_data_path,
     http_request_to_scrapy_request,
     scrapy_response_to_http_response,
 )
 
 
 @mock.patch("scrapy_poet.utils.os.makedirs")
@@ -168,7 +171,25 @@
 def test_scrapy_response_to_http_response(scrapy_response, http_response):
     result = scrapy_response_to_http_response(scrapy_response)
     assert str(result.url) == str(http_response.url)
     assert result.body == http_response.body
     assert result.status == http_response.status
     assert result.headers == http_response.headers
     assert result._encoding == http_response._encoding
+
+
+@mock.patch("scrapy_poet.utils.consume_modules")
+def test_create_registry_instance_SCRAPY_POET_DISCOVER(mock_consume_modules, settings):
+    settings.set("SCRAPY_POET_RULES", [])
+
+    mock_cls = mock.Mock()
+    fake_crawler = get_crawler(Spider, settings)
+    create_registry_instance(mock_cls, fake_crawler)
+    mock_consume_modules.assert_not_called()
+    mock_cls.assert_called_once_with(rules=[])
+
+    mock_cls = mock.Mock()
+    settings.set("SCRAPY_POET_DISCOVER", ["a.b.c", "x.y"])
+    fake_crawler = get_crawler(Spider, settings)
+    create_registry_instance(mock_cls, fake_crawler)
+    assert mock_consume_modules.call_args_list == [mock.call("a.b.c"), mock.call("x.y")]
+    mock_cls.assert_called_once_with(rules=[])
```

### Comparing `scrapy-poet-0.8.0/tests/utils.py` & `scrapy-poet-0.9.0/scrapy_poet/utils/testing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+from inspect import isasyncgenfunction
 from typing import Dict
 from unittest import mock
 
-from pytest_twisted import inlineCallbacks
+from scrapy import signals
 from scrapy.crawler import Crawler
 from scrapy.exceptions import CloseSpider
+from scrapy.settings import Settings
 from scrapy.utils.python import to_bytes
 from twisted.internet import reactor
+from twisted.internet.defer import inlineCallbacks
 from twisted.internet.task import deferLater
 from twisted.web.resource import Resource
 from twisted.web.server import NOT_DONE_YET
 
-from tests.mockserver import MockServer
+from scrapy_poet.utils.mockserver import MockServer
 
 
 class HtmlResource(Resource):
     isLeaf = True
     content_type = "text/html"
     html = ""
     extra_headers: Dict[str, str] = {}
@@ -87,24 +90,27 @@
 
 
 @inlineCallbacks
 def crawl_single_item(
     spider_cls, resource_cls, settings, spider_kwargs=None, port=None
 ):
     """Run a spider where a single item is expected. Use in combination with
-    ``capture_capture_exceptions`` and ``CollectorPipeline``
+    ``capture_exceptions`` and ``CollectorPipeline``
     """
     items, url, crawler = yield crawl_items(
         spider_cls, resource_cls, settings, spider_kwargs=spider_kwargs, port=port
     )
-    assert len(items) == 1
-    resp = items[0]
-    if "exception" in resp:
-        raise resp["exception"]
-    return resp, url, crawler
+    try:
+        item = items[0]
+    except IndexError:
+        return None, url, crawler
+
+    if isinstance(item, dict) and "exception" in item:
+        raise item["exception"]
+    return item, url, crawler
 
 
 def make_crawler(spider_cls, settings):
     if not getattr(spider_cls, "name", None):
 
         class Spider(spider_cls):
             name = "test_spider"
@@ -120,22 +126,58 @@
         spider.collected_items = []
 
     def process_item(self, item, spider):
         spider.collected_items.append(item)
         return item
 
 
+class InjectedDependenciesCollectorMiddleware:
+    @classmethod
+    def from_crawler(cls, crawler):
+        obj = cls()
+        crawler.signals.connect(obj.spider_opened, signal=signals.spider_opened)
+        return obj
+
+    def spider_opened(self, spider):
+        spider.collected_response_deps = []
+
+    def process_response(self, request, response, spider):
+        spider.collected_response_deps.append(request.cb_kwargs)
+        return response
+
+
+def create_scrapy_settings(request):
+    """Default scrapy-poet settings"""
+    s = dict(
+        # collect scraped items to crawler.spider.collected_items
+        ITEM_PIPELINES={
+            CollectorPipeline: 100,
+        },
+        DOWNLOADER_MIDDLEWARES={
+            # collect injected dependencies to crawler.spider.collected_response_deps
+            InjectedDependenciesCollectorMiddleware: 542,
+            "scrapy_poet.InjectionMiddleware": 543,
+        },
+    )
+    return Settings(s)
+
+
 def capture_exceptions(callback):
     """Wrapper for Scrapy callbacks that captures exceptions within
     the provided callback and yields it under `exception` property. Also
     spider is closed on the first exception."""
 
-    def parse(*args, **kwargs):
+    async def parse(*args, **kwargs):
         try:
-            yield from callback(*args, **kwargs)
+            if isasyncgenfunction(callback):
+                async for x in callback(*args, **kwargs):
+                    yield x
+            else:
+                for x in callback(*args, **kwargs):
+                    yield x
         except Exception as e:
             yield {"exception": e}
             raise CloseSpider("Exception in callback detected")
 
     # Mimic type annotations
     parse.__annotations__ = callback.__annotations__
     return parse
```

