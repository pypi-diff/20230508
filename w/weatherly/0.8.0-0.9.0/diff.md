# Comparing `tmp/weatherly-0.8.0.tar.gz` & `tmp/weatherly-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weatherly-0.8.0.tar", last modified: Sat May  6 11:20:26 2023, max compression
+gzip compressed data, was "weatherly-0.9.0.tar", last modified: Sat May  6 12:25:40 2023, max compression
```

## Comparing `weatherly-0.8.0.tar` & `weatherly-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 11:20:26.522344 weatherly-0.8.0/
--rw-rw-rw-   0        0        0     1097 2023-04-15 14:32:24.000000 weatherly-0.8.0/LICENSE
--rw-rw-rw-   0        0        0     3574 2023-05-06 11:20:26.519347 weatherly-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     2500 2023-05-06 11:06:37.000000 weatherly-0.8.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-06 11:20:26.522344 weatherly-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     2024 2023-05-02 14:16:37.000000 weatherly-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:20:26.468378 weatherly-0.8.0/weatherly/
--rw-rw-rw-   0        0        0      817 2023-05-06 11:15:22.000000 weatherly-0.8.0/weatherly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:20:26.514397 weatherly-0.8.0/weatherly/api/
--rw-rw-rw-   0        0        0     1257 2023-05-02 14:16:37.000000 weatherly-0.8.0/weatherly/api/__init__.py
--rw-rw-rw-   0        0        0    26795 2023-05-06 11:06:37.000000 weatherly-0.8.0/weatherly/api/client.py
--rw-rw-rw-   0        0        0     2742 2023-04-24 06:52:08.000000 weatherly-0.8.0/weatherly/api/core.py
--rw-rw-rw-   0        0        0     5346 2023-05-06 11:06:37.000000 weatherly-0.8.0/weatherly/enums.py
--rw-rw-rw-   0        0        0     4035 2023-05-02 14:16:37.000000 weatherly-0.8.0/weatherly/errors.py
--rw-rw-rw-   0        0        0    43189 2023-05-06 11:06:37.000000 weatherly-0.8.0/weatherly/responses.py
--rw-rw-rw-   0        0        0     2894 2023-05-02 14:16:37.000000 weatherly-0.8.0/weatherly/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:20:26.500357 weatherly-0.8.0/weatherly.egg-info/
--rw-rw-rw-   0        0        0     3574 2023-05-06 11:20:26.000000 weatherly-0.8.0/weatherly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-05-06 11:20:26.000000 weatherly-0.8.0/weatherly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 11:20:26.000000 weatherly-0.8.0/weatherly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-05-06 11:20:26.000000 weatherly-0.8.0/weatherly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-06 11:20:26.000000 weatherly-0.8.0/weatherly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 12:25:40.086676 weatherly-0.9.0/
+-rw-rw-rw-   0        0        0     1097 2023-04-15 14:32:24.000000 weatherly-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0     3574 2023-05-06 12:25:40.082678 weatherly-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2500 2023-05-06 11:06:37.000000 weatherly-0.9.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-06 12:25:40.090673 weatherly-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     2024 2023-05-02 14:16:37.000000 weatherly-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:25:40.032709 weatherly-0.9.0/weatherly/
+-rw-rw-rw-   0        0        0      817 2023-05-06 12:22:54.000000 weatherly-0.9.0/weatherly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:25:40.077682 weatherly-0.9.0/weatherly/api/
+-rw-rw-rw-   0        0        0     1257 2023-05-02 14:16:37.000000 weatherly-0.9.0/weatherly/api/__init__.py
+-rw-rw-rw-   0        0        0    29714 2023-05-06 12:15:04.000000 weatherly-0.9.0/weatherly/api/client.py
+-rw-rw-rw-   0        0        0     2742 2023-04-24 06:52:08.000000 weatherly-0.9.0/weatherly/api/core.py
+-rw-rw-rw-   0        0        0     5346 2023-05-06 11:06:37.000000 weatherly-0.9.0/weatherly/enums.py
+-rw-rw-rw-   0        0        0     4035 2023-05-02 14:16:37.000000 weatherly-0.9.0/weatherly/errors.py
+-rw-rw-rw-   0        0        0    43189 2023-05-06 11:06:37.000000 weatherly-0.9.0/weatherly/responses.py
+-rw-rw-rw-   0        0        0     2894 2023-05-02 14:16:37.000000 weatherly-0.9.0/weatherly/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:25:40.066688 weatherly-0.9.0/weatherly.egg-info/
+-rw-rw-rw-   0        0        0     3574 2023-05-06 12:25:39.000000 weatherly-0.9.0/weatherly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-05-06 12:25:39.000000 weatherly-0.9.0/weatherly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 12:25:39.000000 weatherly-0.9.0/weatherly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-05-06 12:25:39.000000 weatherly-0.9.0/weatherly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-06 12:25:39.000000 weatherly-0.9.0/weatherly.egg-info/top_level.txt
```

### Comparing `weatherly-0.8.0/LICENSE` & `weatherly-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weatherly-0.8.0/PKG-INFO` & `weatherly-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weatherly
-Version: 0.8.0
+Version: 0.9.0
 Summary: A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more...
 Home-page: https://github.com/konradsic/weatherly
 Author: konradsic
 License: MIT
 Project-URL: Issues, https://github.com/konradsic/weatherly/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `weatherly-0.8.0/README.rst` & `weatherly-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `weatherly-0.8.0/setup.py` & `weatherly-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.8.0/weatherly/__init__.py` & `weatherly-0.9.0/weatherly/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 :license: MIT license, see LICENSE for details
 """
 
 __title__ = 'weatherly'
 __author__ = 'konradsic'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023-present konradsic'
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 from typing import NamedTuple, Literal
 
 from .api import *
 from .errors import *
 from .enums import *
 from .responses import *
@@ -25,10 +25,10 @@
 
 class VersionInfo(NamedTuple):
     major: int
     minor: int
     micro: int
     release_type: Literal['alpha', 'beta', 'candidate', 'final']
     
-version_info = VersionInfo(major=0, minor=8, micro=0, release_type='final')
+version_info = VersionInfo(major=0, minor=9, micro=0, release_type='final')
 
 del NamedTuple, Literal, VersionInfo
```

### Comparing `weatherly-0.8.0/weatherly/api/__init__.py` & `weatherly-0.9.0/weatherly/api/__init__.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.8.0/weatherly/api/client.py` & `weatherly-0.9.0/weatherly/api/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,27 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import datetime
-from typing import Any, Dict, List, Literal, Optional, Union
+import inspect
+import traceback
+from typing import (
+    Any, 
+    Dict, 
+    List, 
+    Literal, 
+    Optional, 
+    Union, 
+    Callable, 
+    TypeVar,
+    ParamSpec
+)
 
 from .. import utils as utils
 from ..enums import Languages
 from ..errors import (AccessDenied, APIKeyDisabled, APILimitExceeded,
                       InternalApplicationError, InvalidAPIKey, InvalidDate,
                       NoLocationFound, WeatherAPIException)
 from ..responses import (AstronomicalData, CurrentWeatherData, ForecastData,
@@ -37,14 +49,17 @@
 WEATHERAPI_BASE_URL = "https://api.weatherapi.com/v1/"
 BOOL_REPLACE = {True: "yes", False: "no"}
 
 __all__ = (
     "Client",
 )
 
+T = TypeVar("T")
+P = ParamSpec("P")
+
 class Client(BaseAPIClient):
     """
     A WeatherAPI.com client for fetching various weather information
 
     Parameters
     ----------
     api_key: :class:`str`
@@ -139,46 +154,86 @@
             elif code == 2006: raise InvalidAPIKey(status, code, msg)
             elif code == 2007: raise APILimitExceeded(status, code, msg)
             elif code == 2008: raise APIKeyDisabled(status, code, msg)
             elif code == 2009: raise AccessDenied(status, code, msg)
             elif code == 9999: raise InternalApplicationError(status, code, msg)
             else: raise WeatherAPIException(status, code, msg)
 
+        full_url = str(self.url + endpoint + utils.parse_kwargs_to_urlargs({**self.default_options, **final_options}))
+        self.on_api_call_successful(full_url, resp[1])
         return resp
     
-    def event(self):
+    def on_error(self, func: str, exc: Exception) -> None:
+        """Default implementation of error handling in this client.
+        
+        Parameters
+        ---------------
+        func: :class:`str`
+            Name of function that raised an error
+        exc: :exc:`Exception`
+            Exception that was caught during func callback
+        """
+        print(f"Exception occured during \"{func}\":\n\n{traceback.format_exc()}")
+    
+    def on_api_call_successful(self, request, result):
+        """An event function called when an API call was successful.
+        
+        Default client implementation of this event is null i.e. does nothing.
+        
+        Parameters
+        --------------
+        request: :class:`str`
+            A request string e.g. https://api.weatherapi.com/v1/some-request&param=value
+        result: :external:py:class:`requests.Response`
+            Result as an requests object
+        """
+        pass
+    
+    def event(self, func: Callable[P, T]) -> Callable[P, T]:
         """A decorator that turns a function into an event. For example
 
         .. code:: python
 
             import weatherly
             client = weatherly.Client(api_key=...)
 
             @client.event
             def on_error(payload):
                 print(f"An error occured! Payload: {payload}")
         
         In the example above, by adding ``@client.event`` the ``on_error`` function has turned into an error handler function
+        
+        .. danger::
+        
+            The function **SHOULD NOT** be a coroutine function!
         """
-        raise NotImplementedError
+        if inspect.iscoroutinefunction(func):
+            raise ValueError("Event functions should not be coroutines")
+        
+        # overwrite default client event implementation to user's func
+        setattr(self, func.__name__, func)
+        return func
 
     def set_language(self, lang: Union[str, Languages]) -> Optional[Languages]:
         """Set client's language when requesting data.
         
         Parameters
         -----------
         lang: Union[:class:`str`, :class:`Languages`]
             Language to set. Can be either a string that is lanuage's name or code or a :class:`Languages` enum object.
             
         Returns
         ---------
         Optional[:class:`Languages`]
             An enum class representing the language of the client. Is ``None`` when something went wrong and the language was not set.
         """
-        lang_class = utils.find_language(lang, asobj=True)
+        try:
+            lang_class = utils.find_language(lang, asobj=True)
+        except Exception as exc:
+            self.on_error("set_language", exc)
         if not lang_class:
             return None
 
         self.lang = lang_class 
         return self.lang
 
     def get_current_weather(self, 
@@ -226,18 +281,21 @@
         """
         options = {
             "aqi": aqi or self.aqi,
             "q": query,
             **kwargs
         }
         if lang is not None: options["lang"] = lang
-        resp = self._call_request("current.json", options)
+        try:
+            resp = self._call_request("current.json", options)
 
-        weather = CurrentWeatherData(resp[0], resp[1].status_code, None)
-        return weather
+            weather = CurrentWeatherData(resp[0], resp[1].status_code, None)
+            return weather
+        except Exception as exc:
+            self.on_error("get_current_weather", exc)
 
     def get_locations(self, query: str):
         """Get locations for given query
 
         Parameters
         ---------------
         query: :class:`str`
@@ -261,20 +319,23 @@
         :exc:`AccessDenied`
             Raised when access to given resource was denied
         :exc:`InternalApplicationError`
             Raised when there was a very rare internal application error
         :exc:`WeatherAPIException`
             Raised when something else went wrong, that does not have a specific exception class.
         """
-        resp = self._call_request("search.json",{"q": query})
+        try:
+            resp = self._call_request("search.json",{"q": query})
 
-        locations = []
-        for loc in resp[0]:
-            locations.append(LocationData(loc, resp[1].status_code, None))
-        return locations
+            locations = []
+            for loc in resp[0]:
+                locations.append(LocationData(loc, resp[1].status_code, None))
+            return locations
+        except Exception as exc:
+            self.on_error("get_locations", exc)
 
     def get_forecast_data(
         self,
         query: str, 
         days: int,
         *,
         aqi: Optional[bool] = None,
@@ -327,17 +388,20 @@
             "q": query,
             "alerts": alerts or self.kwargs.get("alerts"),
             "days": days,
             **kwargs
         }
         if lang is not None: options["lang"] = lang
 
-        resp = self._call_request("forecast.json", options)
-        forecast = ForecastData(resp[0], resp[1].status_code, None)
-        return forecast
+        try:
+            resp = self._call_request("forecast.json", options)
+            forecast = ForecastData(resp[0], resp[1].status_code, None)
+            return forecast
+        except Exception as exc:
+            self.on_error("get_forecast_data", exc)
 
     def get_historical_data(
         self,
         query: str,
         date: str,
         *,
         aqi: Optional[bool] = None,
@@ -391,34 +455,36 @@
             "aqi": aqi or self.aqi,
             "q": query,
             "alerts": alerts or self.kwargs.get("alerts"),
             "dt": date,
             **kwargs
         }
         if lang is not None: options["lang"] = lang
-
-        # check if given date is really "historical"
         try:
-            splitted = date.split("-")
-            datetuple = datetime.datetime(
-                int(splitted[0]), 
-                int(splitted[1][1:]) if splitted[1].startswith("0") else int(splitted[1]), 
-                int(splitted[2][1:]) if splitted[2].startswith("0") else int(splitted[2]),
-                0,0)
-            epoch = datetuple.timestamp()
+            # check if given date is really "historical"
+            try:
+                splitted = date.split("-")
+                datetuple = datetime.datetime(
+                    int(splitted[0]), 
+                    int(splitted[1][1:]) if splitted[1].startswith("0") else int(splitted[1]), 
+                    int(splitted[2][1:]) if splitted[2].startswith("0") else int(splitted[2]),
+                    0,0)
+                epoch = datetuple.timestamp()
+            except Exception as exc:
+                raise InvalidDate(f"Failed to convert date {date}: Invalid format") from exc
+
+            now = datetime.datetime.timestamp(datetime.datetime.utcnow())
+
+            if epoch > now: raise InvalidDate("Date should be before current time, switch from History API to Future to use future dates.")
+
+            resp = self._call_request("history.json", options)
+            history = ForecastData(resp[0], resp[1].status_code, None)
+            return history
         except Exception as exc:
-            raise InvalidDate(f"Failed to convert date {date}: Invalid format") from exc
-
-        now = datetime.datetime.timestamp(datetime.datetime.utcnow())
-
-        if epoch > now: raise InvalidDate("Date should be before current time, switch from History API to Future to use future dates.")
-
-        resp = self._call_request("history.json", options)
-        history = ForecastData(resp[0], resp[1].status_code, None)
-        return history
+            self.on_error("get_historical_data", exc)
         
     def get_future_data(
         self,
         query: str,
         date: str,
         *,
         lang: Optional[Union[str, Languages]] = None,
@@ -464,34 +530,37 @@
         """
         options = {
             "q": query,
             "dt": date,
             **kwargs
         }
         if lang is not None: options["lang"] = lang
-
-        # check if given date is really "historical"
+        
         try:
-            splitted = date.split("-")
-            datetuple = datetime.datetime(
-                int(splitted[0]), 
-                int(splitted[1][1:]) if splitted[1].startswith("0") else int(splitted[1]), 
-                int(splitted[2][1:]) if splitted[2].startswith("0") else int(splitted[2]),
-                0,0)
-            epoch = datetuple.timestamp()
+            # check if given date is really "historical"
+            try:
+                splitted = date.split("-")
+                datetuple = datetime.datetime(
+                    int(splitted[0]), 
+                    int(splitted[1][1:]) if splitted[1].startswith("0") else int(splitted[1]), 
+                    int(splitted[2][1:]) if splitted[2].startswith("0") else int(splitted[2]),
+                    0,0)
+                epoch = datetuple.timestamp()
+            except Exception as exc:
+                raise InvalidDate(f"Failed to convert date {date}: Invalid format") from exc
+
+            now = datetime.datetime.timestamp(datetime.datetime.utcnow())
+
+            if epoch < now: raise InvalidDate("Date should be after current time, switch from Future API to History to use past dates.")
+
+            resp = self._call_request("future.json", options)
+            future = FutureData(resp[0], resp[1].status_code, None)
+            return future
         except Exception as exc:
-            raise InvalidDate(f"Failed to convert date {date}: Invalid format") from exc
-
-        now = datetime.datetime.timestamp(datetime.datetime.utcnow())
-
-        if epoch < now: raise InvalidDate("Date should be after current time, switch from Future API to History to use past dates.")
-
-        resp = self._call_request("future.json", options)
-        future = FutureData(resp[0], resp[1].status_code, None)
-        return future
+            self.on_error("get_future_data", exc)
         
     def get_astronomical_data(
         self,
         query: str,
         date: str,
         **kwargs: Dict[str, Any]
     ) -> AstronomicalData:
@@ -529,17 +598,20 @@
             Raised when something else went wrong, that does not have a specific exception class.
         """
         options = {
             "q": query,
             "dt": date,
             **kwargs
         }
-        resp = self._call_request("astronomy.json", options)
-        astro = AstronomicalData(resp[0], resp[1].status_code, None)
-        return astro
+        try:
+            resp = self._call_request("astronomy.json", options)
+            astro = AstronomicalData(resp[0], resp[1].status_code, None)
+            return astro
+        except Exception as exc:
+            self.on_error("get_astronomical_data", exc)
 
     def get_marine_data(
         self,
         query: str,
         *,
         tides: Optional[bool] = None,
         **kwargs: Dict[str, Any]
@@ -578,17 +650,20 @@
             Raised when something else went wrong, that does not have a specific exception class.
         """
         options = {
             "q": query,
             "tides": tides or self.tides,
             **kwargs
         }
-        resp = self._call_request("marine.json", options)
-        marine = MarineData(resp[0], resp[1].status_code, None)
-        return marine
+        try:
+            resp = self._call_request("marine.json", options)
+            marine = MarineData(resp[0], resp[1].status_code, None)
+            return marine
+        except Exception as exc:
+            self.on_error("get_marine_data", exc)
 
     def get_ip_data(
         self,
         ip_address: str,
         **kwargs: Dict[str, Any]
     ) -> IPData:
         """
@@ -623,17 +698,20 @@
         :exc:`WeatherAPIException`
             Raised when something else went wrong, that does not have a specific exception class.
         """
         options = {
             "q": ip_address,
             **kwargs
         }
-        resp = self._call_request("ip.json", options)
-        ip = IPData(resp[0], resp[1].status_code, None)
-        return ip
+        try:
+            resp = self._call_request("ip.json", options)
+            ip = IPData(resp[0], resp[1].status_code, None)
+            return ip
+        except Exception as exc:
+            self.on_error("get_ip_data", exc)
 
     def get_sports_data(
         self,
         query: str,
         **kwargs: Dict[str, Any]
     ) -> SportsData:
         """
@@ -668,19 +746,20 @@
         :exc:`WeatherAPIException`
             Raised when something else went wrong, that does not have a specific exception class.
         """
         options = {
             "q": query,
             **kwargs
         }
-        resp = self._call_request("sports.json", options)
-        sports = SportsData(resp[0], resp[1].status_code, None)
-        return sports
-
-
+        try:
+            resp = self._call_request("sports.json", options)
+            sports = SportsData(resp[0], resp[1].status_code, None)
+            return sports
+        except Exception as exc:
+            self.on_error("get_sports_data", exc)
     
     def __str__(self):
         return f"<{self.__class__.__name__} api_key={self.default_options['key']} lang={self.lang}>"
     
     def __repr__(self):
         return repr(self.__str__())
```

### Comparing `weatherly-0.8.0/weatherly/api/core.py` & `weatherly-0.9.0/weatherly/api/core.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.8.0/weatherly/enums.py` & `weatherly-0.9.0/weatherly/enums.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.8.0/weatherly/errors.py` & `weatherly-0.9.0/weatherly/errors.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.8.0/weatherly/responses.py` & `weatherly-0.9.0/weatherly/responses.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.8.0/weatherly/utils.py` & `weatherly-0.9.0/weatherly/utils.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.8.0/weatherly.egg-info/PKG-INFO` & `weatherly-0.9.0/weatherly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weatherly
-Version: 0.8.0
+Version: 0.9.0
 Summary: A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more...
 Home-page: https://github.com/konradsic/weatherly
 Author: konradsic
 License: MIT
 Project-URL: Issues, https://github.com/konradsic/weatherly/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
```

