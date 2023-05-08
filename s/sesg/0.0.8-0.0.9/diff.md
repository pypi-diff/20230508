# Comparing `tmp/sesg-0.0.8.tar.gz` & `tmp/sesg-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sesg-0.0.8.tar", max compression
+gzip compressed data, was "sesg-0.0.9.tar", max compression
```

## Comparing `sesg-0.0.8.tar` & `sesg-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35148 2023-04-17 17:41:20.988197 sesg-0.0.8/LICENSE
--rw-r--r--   0        0        0      478 2023-04-17 17:33:48.160350 sesg-0.0.8/README.md
--rw-r--r--   0        0        0     2801 2023-04-19 01:47:34.815214 sesg-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-17 15:18:13.051151 sesg-0.0.8/src/sesg/__init__.py
--rw-r--r--   0        0        0     8127 2023-04-17 21:13:02.702530 sesg-0.0.8/src/sesg/graph.py
--rw-r--r--   0        0        0     6744 2023-04-17 14:56:33.924330 sesg-0.0.8/src/sesg/metrics.py
--rw-r--r--   0        0        0      173 2023-04-18 04:38:35.955358 sesg-0.0.8/src/sesg/scopus/__init__.py
--rw-r--r--   0        0        0     7656 2023-04-19 01:47:30.231256 sesg-0.0.8/src/sesg/scopus/api.py
--rw-r--r--   0        0        0     6080 2023-04-18 12:05:40.816197 sesg-0.0.8/src/sesg/scopus/client.py
--rw-r--r--   0        0        0    16416 2023-04-18 03:04:34.582222 sesg-0.0.8/src/sesg/scopus_client.py
--rw-r--r--   0        0        0    13843 2023-04-18 03:31:52.519891 sesg-0.0.8/src/sesg/search_string.py
--rw-r--r--   0        0        0     7659 2023-04-17 15:00:57.692606 sesg-0.0.8/src/sesg/snowballing.py
--rw-r--r--   0        0        0     6042 2023-04-18 16:47:52.299822 sesg-0.0.8/src/sesg/topic_extraction.py
--rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 sesg-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-04-17 17:41:20.988197 sesg-0.0.9/LICENSE
+-rw-r--r--   0        0        0      478 2023-04-17 17:33:48.160350 sesg-0.0.9/README.md
+-rw-r--r--   0        0        0     2801 2023-04-19 16:37:24.181123 sesg-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-17 15:18:13.051151 sesg-0.0.9/src/sesg/__init__.py
+-rw-r--r--   0        0        0     8127 2023-04-17 21:13:02.702530 sesg-0.0.9/src/sesg/graph.py
+-rw-r--r--   0        0        0     6744 2023-04-17 14:56:33.924330 sesg-0.0.9/src/sesg/metrics.py
+-rw-r--r--   0        0        0      631 2023-04-19 16:32:22.203556 sesg-0.0.9/src/sesg/scopus/__init__.py
+-rw-r--r--   0        0        0     8441 2023-04-19 14:45:57.217851 sesg-0.0.9/src/sesg/scopus/api.py
+-rw-r--r--   0        0        0     7159 2023-04-19 16:36:19.116652 sesg-0.0.9/src/sesg/scopus/client.py
+-rw-r--r--   0        0        0    16416 2023-04-18 03:04:34.582222 sesg-0.0.9/src/sesg/scopus_client.py
+-rw-r--r--   0        0        0    13843 2023-04-18 03:31:52.519891 sesg-0.0.9/src/sesg/search_string.py
+-rw-r--r--   0        0        0     7659 2023-04-17 15:00:57.692606 sesg-0.0.9/src/sesg/snowballing.py
+-rw-r--r--   0        0        0     6042 2023-04-18 16:47:52.299822 sesg-0.0.9/src/sesg/topic_extraction.py
+-rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 sesg-0.0.9/PKG-INFO
```

### Comparing `sesg-0.0.8/LICENSE` & `sesg-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sesg-0.0.8/pyproject.toml` & `sesg-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sesg"
-version = "0.0.8"
+version = "0.0.9"
 description = "SeSG is a tool developed to help Systematic Literature Review researchers, specifically at the step of building a search string."
 authors = ["Demetrius Panovitch <demetrius.mp789@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
   {include = "sesg", from = "src"}
 ]
```

### Comparing `sesg-0.0.8/src/sesg/graph.py` & `sesg-0.0.9/src/sesg/graph.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.8/src/sesg/metrics.py` & `sesg-0.0.9/src/sesg/metrics.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.8/src/sesg/scopus/api.py` & `sesg-0.0.9/src/sesg/scopus/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,55 +25,65 @@
 
 
 @dataclass
 class SuccessResponse:
     """A successfull Scopus Response
 
     Args:
-        number_of_results (int): Number of results for this query.
+        number_of_results (int): Number of results for this query. Notice that even if it displays more than 5000 results, Scopus will limit to retrieve only 5000.
         number_of_pages (int): Number of pages that needs to be fetched to get all results. Limited to 200 due to Scopus API 5000 entries limit.
-        current_page (int): Current page being fetched.
+        current_page (int): Current page being fetched. Starts at 1, being at most 200.
         entries (List[Entry]): Studies returned from the API.
     """  # noqa: E501
 
     @dataclass
     class Entry:
         """A study entry returned from the API.
 
         Args:
             title (str): The title of the study.
+            cited_by_count (Optional[int]): How many studies cites this one.
         """
 
         title: str
+        cited_by_count: Optional[int]
 
     number_of_results: int
     number_of_pages: int
     current_page: int
     entries: List[Entry]
 
 
 class TimeoutError(Exception):
     """The request took too long."""
 
 
 class APIKeyExpiredError(Exception):
-    """The API key is expired, meaning it has been used over 20000 times in less than a week"""  # noqa: E501
+    """The API key is expired, meaning it has been used over 20000 times in less than a week.
+
+    Args:
+        resets_at (Optional[datetime]): Datetime object represents when the API key will be resetted.
+    """  # noqa: E501
 
     resets_at: Optional[datetime]
 
     def __init__(
         self,
         *,
         resets_at: Optional[datetime] = None,
     ) -> None:
         self.resets_at = resets_at
 
 
 class PayloadTooLargeError(Exception):
-    """The response has a status code of 400 or 413. Probably the search string is too long."""  # noqa: E501
+    """The response has a status code of 413. Probably the search string is too long."""  # noqa: E501
+
+
+class BadRequestError(Exception):
+    """The response has a status code of 400."""  # noqa: E501
 
 
 def _api_key_is_expired(
     *,
     response: httpx.Response,
 ) -> bool:
     """Checks if a Scopus API key is expired, given the response of a Scopus Request.
@@ -194,26 +204,27 @@
 ) -> SuccessResponse:
     """Parses a Scopus API response.
 
     Args:
         response (httpx.Response): A Scopus API response.
 
     Returns:
-        A SuccessResponse instance
+        A SuccessResponse instance.
     """  # noqa: E501
     json = response.json()
 
     number_of_results = int(json["search-results"]["opensearch:totalResults"])
     start_index = int(json["search-results"]["opensearch:startIndex"])
     current_page = math.floor(start_index / 25) + 1
     number_of_pages = min(math.ceil(number_of_results / 25), 200)
 
     entries = [
         SuccessResponse.Entry(
             title=entry["dc:title"],
+            cited_by_count=entry.get("citedby-count", None),
         )
         for entry in json["search-results"]["entry"]
         if "dc:title" in entry
     ]
 
     return SuccessResponse(
         number_of_results=number_of_results,
@@ -229,24 +240,31 @@
     query: str,
     timeout: float,
     page: int,
 ) -> AsyncIterator[SuccessResponse]:
     """Performs Scopus API calls, in a manner that will return
     all available results, which is at most 5000.
 
+    !!! note
+
+        Notice that the exceptions on the **Raises**
+        section occurs during iteration time, not at function call time.
+
     Args:
         api_key (str): Valid Scopus API key.
         query (str): Query to search for.
         timeout (int): How long to wait for the request to complete.
         page (int): Page where to start the search.
 
     Raises:
         TimeoutError: If the request takes longer than the given `timeout`.
         APIKeyExpiredError: If the response has a header indicating that the API Key is expired.
-        PayloadTooLargeError: If the response status code is 413. Indicates that the search string is too large.
+        PayloadTooLargeError: If the response status code is 413. Probably indicates that the search string is too large.
+        BadRequestError: If the response status code is 400. Probably indicates that the search string is too large.
+
 
     Yields:
         Async iterator that yields each page found.
     """  # noqa: E501
     client = httpx.AsyncClient()
 
     first_request = _create_request(
```

### Comparing `sesg-0.0.8/src/sesg/scopus/client.py` & `sesg-0.0.9/src/sesg/scopus/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,33 +5,55 @@
 The client is optimized to scrape the maximum number of pages that are available from Scopus API,
 which is 5000, for normal users, at the maximum speed possible.
 
 We use [`aiometer`](https://github.com/florimondmanca/aiometer),
 and [`httpx`](https://github.com/projectdiscovery/httpx) to achieve this goal.
 """  # noqa: E501
 
-from typing import AsyncIterator, List, Union
+from dataclasses import dataclass
+from datetime import datetime
+from typing import AsyncIterator, List, Optional, Union
 
 from . import api
 
 
 class OutOfAPIKeysError(Exception):
     """Used all API keys available."""
 
 
-class ExceededTimeoutRetries(Exception):
+class ExceededTimeoutRetriesError(Exception):
     """Exceeded the number of timeout retries in a row."""
 
 
+@dataclass
 class APIKeyExpiredResponse:
-    """Represents an API key expired response from the [`ScopusClient`][sesg.scopus.client.ScopusClient]"""  # noqa: E501
+    """Represents an API key expired response from the [`ScopusClient`][sesg.scopus.client.ScopusClient]
+
+    Args:
+        api_key (str): The expired API key.
+        api_key_index (int): The index of the expired API key on the list of API keys passed to [`ScopusClient`][sesg.scopus.client.ScopusClient].
+        resets_at (Optional[datetime]): Datetime object represents when the API key will be resetted.
+    """  # noqa: E501
+
+    api_key: str
+    api_key_index: int
+    resets_at: Optional[datetime]
 
 
+@dataclass
 class TimeoutResponse:
-    """Represents a timed out response from the [`ScopusClient`][sesg.scopus.client.ScopusClient]"""  # noqa: E501
+    """Represents a timed out response from the [`ScopusClient`][sesg.scopus.client.ScopusClient]
+
+    Args:
+        timed_out_page (int): The page where the timeout occured.
+        timeout_retry (int): The current timeout retry attempt for a same request.
+    """  # noqa: E501
+
+    timed_out_page: int
+    timeout_retry: int
 
 
 class ScopusClient:
     """A Scopus API Client with automatic retry on timeout, and automatic
     API key swapping on expiry.
 
     Args:
@@ -72,20 +94,20 @@
     @property
     def current_api_key_index(self) -> int:
         """Index on the list of the current API key being used."""
         return self.__current_api_key_index
 
     @property
     def current_page(self) -> int:
-        """Current page being fetched."""
+        """Current page being fetched. Starts at 1, being at most 200."""
         return self.__current_page
 
     @property
     def current_query(self) -> str:
-        """Current query being searched."""
+        """Current query being used."""
         return self.__current_query
 
     @property
     def api_keys(self) -> List[str]:
         """The Scopus API keys for this client."""
         return self.__api_keys
 
@@ -100,42 +122,53 @@
             query=self.__current_query,
             timeout=self.__timeout,
             page=self.__current_page,
         )
 
     async def __anext__(self):
         try:
-            data = await self.__iterator.__anext__()
+            response = await self.__iterator.__anext__()
 
             self.__current_page += 1
             self.__current_timeout_retry = 0
 
-            return data
+            return response
 
         except api.PayloadTooLargeError as e:
             raise e
 
-        except api.APIKeyExpiredError:
+        except api.APIKeyExpiredError as e:
+            response = APIKeyExpiredResponse(
+                api_key=self.current_api_key,
+                api_key_index=self.current_api_key_index,
+                resets_at=e.resets_at,
+            )
+
             self.__current_timeout_retry = 0
             self.__iterator = self.__restart_iterator_with_current_state()
             self.__current_api_key_index += 1
 
             if self.__current_api_key_index == len(self.__api_keys):
                 raise OutOfAPIKeysError()
 
-            return APIKeyExpiredResponse()
+            return response
 
         except api.TimeoutError:
             if self.__current_timeout_retry == self.__timeout_retries - 1:
-                raise ExceededTimeoutRetries()
+                raise ExceededTimeoutRetriesError()
+
+            response = TimeoutResponse(
+                timed_out_page=self.current_page,
+                timeout_retry=self.current_timeout_retry,
+            )
 
             self.__current_timeout_retry += 1
             self.__iterator = self.__restart_iterator_with_current_state()
 
-            return TimeoutResponse()
+            return response
 
     def __aiter__(self):
         self.__current_page = 0
         self.__current_timeout_retry = 0
         self.__iterator = self.__restart_iterator_with_current_state()
 
         return self
@@ -148,17 +181,28 @@
             api.SuccessResponse,
             APIKeyExpiredResponse,
             TimeoutResponse,
         ]
     ]:
         """Performs Scopus API requests in a timeout-proof, and API key expiry-prof manner.
 
+        !!! note
+
+            Notice that the exceptions on the **Raises**
+            section occurs during iteration time, not at function call time.
+
         Args:
             query (str): The query to search for.
 
+        Raises:
+            ExceededTimeoutRetriesError: If exceeds the number of timeout retries in a row.
+            OutOfAPIKeysError: If used al API keys available.
+            PayloadTooLargeError: If the response status code is 413. Probably indicates that the search string is too large.
+            BadRequestError: If the response status code is 400. Probably indicates that the search string is too large.
+
         Returns:
             An AsyncIterator that yields one of the below:
 
                 - A succesfull response
                 - An API key expired response
                 - A Timed out response
 
@@ -174,23 +218,7 @@
             ...     else:
             ...         # here data is of type `SuccessResponse`
             ...         print(data.entries)
         """  # noqa: E501
         self.__current_query = query
 
         return self.__aiter__()
-
-
-async def m():
-    client = ScopusClient(api_keys=[], timeout=7, timeout_retries=10)
-
-    async for data in client.search("machie"):
-        if isinstance(data, TimeoutResponse):
-            print(f"Timed out on page {client.current_page}")
-
-        elif isinstance(data, APIKeyExpiredResponse):
-            print(
-                f"API Key {client.current_api_key_index + 1} of {len(client.api_keys)} is expired."  # noqa: E501
-            )
-        else:
-            # here data is of type [`SuccessResponse`][sesg.scopus.api.SuccessResponse]
-            print(data.entries)
```

### Comparing `sesg-0.0.8/src/sesg/scopus_client.py` & `sesg-0.0.9/src/sesg/scopus_client.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.8/src/sesg/search_string.py` & `sesg-0.0.9/src/sesg/search_string.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.8/src/sesg/snowballing.py` & `sesg-0.0.9/src/sesg/snowballing.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.8/src/sesg/topic_extraction.py` & `sesg-0.0.9/src/sesg/topic_extraction.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.8/PKG-INFO` & `sesg-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sesg
-Version: 0.0.8
+Version: 0.0.9
 Summary: SeSG is a tool developed to help Systematic Literature Review researchers, specifically at the step of building a search string.
 License: GPL-3.0-only
 Author: Demetrius Panovitch
 Author-email: demetrius.mp789@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

