# Comparing `tmp/pysnc-1.1.3.tar.gz` & `tmp/pysnc-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysnc-1.1.3.tar", max compression
+gzip compressed data, was "pysnc-1.1.4.tar", max compression
```

## Comparing `pysnc-1.1.3.tar` & `pysnc-1.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1052 2023-04-27 21:10:59.586770 pysnc-1.1.3/LICENSE
--rw-r--r--   0        0        0     1590 2023-04-27 21:10:59.586770 pysnc-1.1.3/README.md
--rw-r--r--   0        0        0      984 2023-04-27 21:10:59.586770 pysnc-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      129 2023-04-27 21:10:59.586770 pysnc-1.1.3/pysnc/__init__.py
--rw-r--r--   0        0        0       98 2023-04-27 21:10:59.586770 pysnc-1.1.3/pysnc/__version__.py
--rw-r--r--   0        0        0     8875 2023-04-27 21:10:59.586770 pysnc-1.1.3/pysnc/attachment.py
--rw-r--r--   0        0        0     3778 2023-04-27 21:10:59.590770 pysnc-1.1.3/pysnc/auth.py
--rw-r--r--   0        0        0    15712 2023-04-27 21:10:59.590770 pysnc-1.1.3/pysnc/client.py
--rw-r--r--   0        0        0     1002 2023-04-27 21:10:59.590770 pysnc-1.1.3/pysnc/exceptions.py
--rw-r--r--   0        0        0     3809 2023-04-27 21:10:59.590770 pysnc-1.1.3/pysnc/query.py
--rw-r--r--   0        0        0    37242 2023-04-27 21:10:59.590770 pysnc-1.1.3/pysnc/record.py
--rw-r--r--   0        0        0      846 2023-04-27 21:10:59.590770 pysnc-1.1.3/pysnc/utils.py
--rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 pysnc-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-05-08 21:40:28.445381 pysnc-1.1.4/LICENSE
+-rw-r--r--   0        0        0     1590 2023-05-08 21:40:28.445381 pysnc-1.1.4/README.md
+-rw-r--r--   0        0        0     1056 2023-05-08 21:40:28.445381 pysnc-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/__init__.py
+-rw-r--r--   0        0        0       98 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/__version__.py
+-rw-r--r--   0        0        0     9386 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/attachment.py
+-rw-r--r--   0        0        0     3757 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/auth.py
+-rw-r--r--   0        0        0    15815 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/client.py
+-rw-r--r--   0        0        0     1002 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/exceptions.py
+-rw-r--r--   0        0        0     3867 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/query.py
+-rw-r--r--   0        0        0    37895 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/record.py
+-rw-r--r--   0        0        0      846 2023-05-08 21:40:28.445381 pysnc-1.1.4/pysnc/utils.py
+-rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 pysnc-1.1.4/PKG-INFO
```

### Comparing `pysnc-1.1.3/LICENSE` & `pysnc-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.3/README.md` & `pysnc-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.3/pyproject.toml` & `pysnc-1.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysnc"
-version = "1.1.3"
+version = "1.1.4"
 description = "Python SNC (REST) API"
 authors = ["Matthew Gill <matthew.gill@servicenow.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ServiceNow/PySNC"
 documentation = "https://servicenow.github.io/PySNC/"
 keywords = ["servicenow", "snc"]
@@ -15,24 +15,27 @@
     'Programming Language :: Python :: 3.7',
     'Operating System :: OS Independent',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = ">=2.8.1"
-six = ">=1.10.0"
 requests-oauthlib = { version = ">=1.2.0", optional = true}
 
 [tool.poetry.extras]
 oauth = ["requests-oauthlib"]
 
 [tool.poetry.group.dev.dependencies]
 requests-oauthlib = ">=1.2.0"
 pytest = "^7.3.1"
 python-dotenv = "^1.0.0"
+mypy = "^1.2.0"
+types-requests = "^2.29.0.0"
+types-oauthlib = "^3.2.0.7"
+jake = "^3.0.0"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pysnc-1.1.3/pysnc/attachment.py` & `pysnc-1.1.4/pysnc/attachment.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import traceback
 import logging
 from tempfile import SpooledTemporaryFile
 from pathlib import Path
+from typing import List, Optional
+
+from .record import GlideElement
 from .query import *
 from .exceptions import *
 
 
 class Attachment:
     MAX_MEM_SIZE = 0xFFFF
 
@@ -106,38 +109,38 @@
 
         with self._client.attachment_api.get_file(self.sys_id) as r:
             for chunk in r.iter_content(chunk_size):
                 tf.write(chunk)
         tf.seek(0)
         return tf
 
-    def write_to(self, path, chunk_size=512):
+    def write_to(self, path, chunk_size=512) -> Path:
         """
         Write the attachment to the given path - if the path is a directory the file_name will be used
         """
         assert self._current(), "Cannot read nothing, iterate the attachment"
         p = Path(path)
         # if we specify a dir, auto set the filename
         if p.is_dir():
             p = p / self.file_name
         with open(p, 'wb') as f:
             with self._client.attachment_api.get_file(self.sys_id) as r:
                 for chunk in r.iter_content(chunk_size):
                     f.write(chunk)
         return p
 
-    def read(self):
+    def read(self) -> bytes:
         """
         Read the entire attachment
         :return: b''
         """
         assert self._current(), "Cannot read nothing, iterate the attachment"
         return self._client.attachment_api.get_file(self.sys_id, stream=False).content
 
-    def readlines(self, encoding='UTF-8', delimiter='\n'):
+    def readlines(self, encoding='UTF-8', delimiter='\n') -> List[str]:
         """
         Read the attachment, as text, decoding by default as UTF-8, splitting by the delimiter.
         :param encoding: encoding to use, defaults to UTF-8
         :param delimiter: what to split by, defualt \n
         :return: list
         """
         return self.read().decode(encoding).split(delimiter)
@@ -161,24 +164,29 @@
                 raise RequestException(
                     'Maximum execution time exceeded. Lower batch size (< %s).' % self.__batch_size)
             else:
                 traceback.print_exc()
                 self._log.debug(response.text)
                 raise e
 
+    def _transform_result(self, result):
+        for key, value in result.items():
+            result[key] = GlideElement(key, value, parent_record=self)
+        return result
+
     def get(self, sys_id: str) -> bool:
         """
         Get a single record, accepting two values. If one value is passed, assumed to be sys_id. If two values are
         passed in, the first value is the column name to be used. Can return multiple records.
 
         :param sys_id: the id of the attachment
         :return: ``True`` or ``False`` based on success
         """
         try:
-            response = self._client.attachment_api.get(self, sys_id)
+            response = self._client.attachment_api.get(sys_id)
         except NotFoundException:
             return False
         self.__results = [self._transform_result(response.json()['result'])]
         if len(self.__results) > 0:
             self.__current = 0
             self.__total = len(self.__results)
             return True
@@ -186,15 +194,15 @@
 
     def delete(self):
         response = self._client.attachment_api.delete(self.sys_id)
         code = response.status_code
         if code != 204:
             raise RequestException(response.text)
 
-    def add_query(self, name, value, second_value=None):
+    def add_query(self, name, value, second_value=None) -> QueryCondition:
         """
         Add a query to a record. For example::
 
             add_query('active', 'true')
 
         Which will create the query ``active=true``. If we specify the second_value::
 
@@ -227,19 +235,24 @@
             * DOES NOT CONTAIN
             * INSTANCEOF
 
         :param str second_value: optional, if specified then ``value`` is expected to be an operator
         """
         return self.__query.add_query(name, value, second_value)
 
-    def add_attachment(self, table_sys_id, file_name, file, content_type=None, encryption_context=None):
+    def add_attachment(self, table_sys_id, file_name, file, content_type=None, encryption_context=None) -> str:
         r = self._client.attachment_api.upload_file(file_name, self._table, table_sys_id, file, content_type,
                                              encryption_context)
-        print(r.status_code)
-        print(r.text)
+        # Location header contains the attachment URL
+        return r.headers['Location']
+
+    def get_link(self) -> Optional[str]:
+        if self._current():
+            return f"{self._client.instance}/api/now/v1/attachment/{self.sys_id}/file"
+        return None
 
     def _get_value(self, item, key='value'):
         obj = self._current()
         if item in obj:
             o = obj[item]
             if isinstance(o, dict):
                 return o[key]
```

### Comparing `pysnc-1.1.3/pysnc/auth.py` & `pysnc-1.1.4/pysnc/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import requests
 import time
 from requests.auth import AuthBase
-from urllib3.util import parse_url, Url
+from urllib3.util import parse_url
 from .exceptions import *
-from .utils import get_instance
 
 JWT_GRANT_TYPE = 'urn:ietf:params:oauth:grant-type:jwt-bearer'
 
 
 class ServiceNowFlow:
     def authenticate(self, instance: str) -> requests.Session:
         raise AuthenticationException('authenticate not implemented')
@@ -39,15 +38,15 @@
 
     def authenticate(self, instance: str) -> requests.Session:
         """
         Designed to be called by ServiceNowClient - internal method.
         """
         try:
             from oauthlib.oauth2 import LegacyApplicationClient
-            from requests_oauthlib import OAuth2Session
+            from requests_oauthlib import OAuth2Session  # type: ignore
 
             oauth = OAuth2Session(client=LegacyApplicationClient(client_id=self.client_id),
                                   auto_refresh_url=self.authorization_url(instance),
                                   auto_refresh_kwargs=dict(client_id=self.client_id, client_secret=self.__secret))
             oauth.fetch_token(token_url=self.authorization_url(instance),
                               username=self.__username, password=self.__password, client_id=self.client_id,
                               client_secret=self.__secret)
```

### Comparing `pysnc-1.1.3/pysnc/client.py` & `pysnc-1.1.4/pysnc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from io import BytesIO
 
 import requests
 from requests.auth import AuthBase
 import re
 import logging
 import base64
-from typing import Callable, Any
+from typing import Callable, no_type_check
 
 from requests.cookies import MockRequest, MockResponse
 from requests.structures import CaseInsensitiveDict
 from requests.utils import get_encoding_from_headers
 
 from .exceptions import *
 from .record import GlideRecord
@@ -123,15 +123,15 @@
         self._client = client
 
     @property
     def session(self):
         return self._client.session
 
     # noinspection PyMethodMayBeStatic
-    def _set_params(self, record: GlideRecord=None):
+    def _set_params(self, record=None):
         params = {} if record is None else record._parameters()
         if 'sysparm_display_value' not in params:
             params['sysparm_display_value'] = 'all'
         params['sysparm_exclude_reference_link'] = 'true'  # Scratch it!
         params['sysparm_suppress_pagination_header'] = 'true'  # Required for large queries
         return params
 
@@ -301,51 +301,52 @@
         self.__request_id += 1
         return self.__request_id
 
     def _add_request(self, request: requests.Request, hook: Callable):
         prepared = request.prepare()
         request_id = str(id(prepared))
         headers = [{'name': k, 'value': v} for (k,v) in prepared.headers.items()]
-        relative_url = prepared.url[prepared.url.index('/', 8):] ## slice from the first non https:// slash
+        relative_url = prepared.url[prepared.url.index('/', 8):]  # type: ignore ## slice from the first non https:// slash
 
         now_request = {
             'id': request_id,
             'method': prepared.method,
             'url': relative_url,
             'headers': headers,
             #'exclude_response_headers': False
         }
         if prepared.body:
-            now_request['body'] = base64.b64encode(prepared.body).decode()
+            now_request['body'] = base64.b64encode(prepared.body).decode()  # type: ignore ## could theoretically do us dirty
         self.__hooks[request_id] = hook
         self.__stored_requests[request_id] = prepared
         self.__requests.append(now_request)
 
+    @no_type_check
     def _transform_response(self, req: requests.PreparedRequest, serviced_request) -> requests.Response:
         # modeled after requests.adapters.HttpAdapter.build_response
         response = requests.Response()
         response.status_code = serviced_request['status_code']
         headers = {k: v for (k, v) in [(e['name'], e['value']) for e in serviced_request.get("headers", [])]}
         response.headers = CaseInsensitiveDict(headers)
         response.encoding = get_encoding_from_headers(response.headers)
 
         body = base64.b64decode(serviced_request.get('body', ''))
         response.raw = BytesIO(body)
 
         if isinstance(req.url, bytes):
             response.url = req.url.decode("utf-8")
         else:
-            response.url = req.url
+            response.url = req.url  # type: ignore
 
         # cookies - kinda hack an adapter in
         req = MockRequest(req)
         res = MockResponse(MockHeaders(headers))
         response.cookies.extract_cookies(res, req)
 
-        response.req = req
+        response.request = req
         # response.connection = None
 
         return response
 
     def execute(self):
         bid = self._next_id()
         body = {
```

### Comparing `pysnc-1.1.3/pysnc/exceptions.py` & `pysnc-1.1.4/pysnc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.3/pysnc/query.py` & `pysnc-1.1.4/pysnc/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,16 @@
 class JoinQuery(Query):
     def __init__(self, table, join_table, primary_field=None, join_table_field=None):
         super(self.__class__, self).__init__(table)
         self._join_table = join_table
         self._primary_field = primary_field
         self._join_table_field = join_table_field
 
-    def generate_query(self) -> str:
-        query = super(self.__class__, self).generate_query()
+    def generate_query(self, encoded_query=None, order_by=None) -> str:
+        query = super(self.__class__, self).generate_query(encoded_query, order_by)
         primary = self._primary_field if self._primary_field else "sys_id"
         secondary = self._join_table_field if self._join_table_field else "sys_id"
         res = "JOIN{table}.{primary}={j_table}.{secondary}".format(
             table=self._table,
             primary=primary,
             j_table=self._join_table,
             secondary=secondary
```

### Comparing `pysnc-1.1.3/pysnc/record.py` & `pysnc-1.1.4/pysnc/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import logging
 import copy
 import traceback
 from requests import Request
-from six import string_types
 from collections import OrderedDict
 from datetime import datetime, timezone
-from typing import Any, Union, List
+from typing import Any, Union, List, Optional, TYPE_CHECKING
 
 from .query import *
 from .exceptions import *
-from .attachment import Attachment
 
 TIMESTAMP_FORMAT = "%Y-%m-%d %H:%M:%S%z"
 
+if TYPE_CHECKING:  # for mypy
+    from .client import ServiceNowClient
+    from .attachment import Attachment
 
 class GlideElement(object):
     """
     Object backing the value/display values of a given record entry.
     """
     def __init__(self, name: str, value=None, display_value=None, parent_record=None):
         self._name = name
@@ -213,32 +214,32 @@
     The GlideRecord object. Normally instantiated via convenience method :func:`pysnc.ServiceNowClient.GlideRecord`.
     This object allows us to interact with a specific table via the table rest api.
 
     :param ServiceNowClient client: We need to know which instance we're connecting to
     :param str table: The table are we going to access
     :param int batch_size: Batch size (items returned per HTTP request). Default is ``500``.
     """
-    def __init__(self, client, table: str, batch_size=500):
+    def __init__(self, client: 'ServiceNowClient', table: str, batch_size=500):
         self._log = logging.getLogger(__name__)
         self._client = client
-        self.__table = table
-        self.__is_iter = False
-        self.__batch_size = batch_size
-        self.__query = Query(table)
-        self.__encoded_query = None
-        self.__results = []
-        self.__current = -1
-        self.__field_limits = None
-        self.__view = None
-        self.__total = None
-        self.__limit = None
-        self.__page = -1
-        self.__order = None
-        self.__is_new_record = False
-        self.__display_value = 'all'
+        self.__table: str = table
+        self.__is_iter: bool = False
+        self.__batch_size: int = batch_size
+        self.__query: Query = Query(table)
+        self.__encoded_query: Optional[str] = None
+        self.__results: list = []
+        self.__current: int = -1
+        self.__field_limits: Optional[List[str]] = None
+        self.__view: Optional[str] = None
+        self.__total: Optional[int] = None
+        self.__limit: Optional[int] = None
+        self.__page: int = -1
+        self.__order: Optional[str] = None
+        self.__is_new_record: bool = False
+        self.__display_value: Union[bool, str] = 'all'
 
     def _clear_query(self):
         self.__query = Query(self.__table)
 
     def _parameters(self):
         ret = dict(
             sysparm_query=self.__query.generate_query(encoded_query=self.__encoded_query, order_by=self.__order)
@@ -295,15 +296,15 @@
         Glide compatable method.
 
         :return: the total
         """
         return self.__total if self.__total is not None else 0
 
     @property
-    def fields(self) -> List[str]:
+    def fields(self) -> Union[List[str], None]:
         """
         :return: Fields in which this record will query OR has queried
         """
         if self.__field_limits:
             return self.__field_limits
         c = self._current()
         if c:
@@ -314,15 +315,15 @@
         return None
 
     @fields.setter
     def fields(self, fields: Union[str, List[str]]):
         """
         Set the fields to query, in CSV string format or as a list
         """
-        if isinstance(fields, string_types):
+        if isinstance(fields, str):
             fields = fields.split(',')
         self.__field_limits = fields
 
     @property
     def view(self):
         """
         :return: The current view
@@ -330,15 +331,15 @@
         return self.__view
 
     @view.setter
     def view(self, view):
         self.__view = view
 
     @property
-    def limit(self) -> int:
+    def limit(self) -> Optional[int]:
         """
         :return: Query number limit
         """
         return self.__limit
 
     @limit.setter
     def limit(self, count: int):
@@ -369,14 +370,15 @@
     @location.setter
     def location(self, location: int):
         """
         Set the current location
 
         :param location: the location to be at
         """
+        assert self.__total is not None, 'no location to be had when we have no query'
         assert -1 <= location < self.__total
         self.__current = location
 
     @property
     def display_value(self):
         return self.__display_value
 
@@ -522,15 +524,15 @@
                 return True
             return False
         else:
             self.add_query(name, value)
             self.query()
             return self.next()
 
-    def insert(self) -> str:
+    def insert(self) -> Optional[str]:
         """
         Insert a new record.
 
         :return: The ``sys_id`` of the record created or ``None``
         :raise:
             :AuthenticationException: If we do not have rights
             :InsertException: For any other failure reason
@@ -546,15 +548,15 @@
             return None
         elif code == 401:
             raise AuthenticationException(response.json()['error'])
         else:
             rjson = response.json()
             raise InsertException(rjson['error'] if 'error' in rjson else f"{code} response on insert -- expected 201", status_code=code)
 
-    def update(self) -> str:
+    def update(self) -> Optional[str]:
         """
         Update the current record.
 
         :return: The ``sys_id`` on success or ``None``
         :raise:
             :AuthenticationException: If we do not have rights
             :UpdateException: For any other failure reason
@@ -599,15 +601,15 @@
         :return: ``True`` on success
         :raise:
             :AuthenticationException: If we do not have rights
             :DeleteException: For any other failure reason
         """
         if self.__total is None:
             if not self.__field_limits:
-                self.fields = 'sys_id'  # all we need...
+                self.fields = 'sys_id'  # type: ignore  ## all we need...
             self.query()
 
         allRecordsWereDeleted = True
         def handle(response):
             nonlocal  allRecordsWereDeleted
             if response.status_code != 204:
                 allRecordsWereDeleted = False
@@ -661,15 +663,15 @@
         :return: The field value or ``None``
         """
         assert field, 'cannot get the display value for the entire record, as the API does not tell us what that is'
         return self._get_value(field, 'display_value')
 
     def get_element(self, field) -> GlideElement:
         """
-        Return the backing GlideElement for the given field. This is the only method to directly access this element.
+        Return the backing GlideElement for the given field. This is the only method to directly access this element.gr2.serialize()
 
         :param str field: The Field
         :return: The GlideElement class or ``None``
         """
         c = self._current()
         if c is None:
             raise NoRecordException('cannot get a value from nothing, did you forget to call next() or initialize()?')
@@ -682,15 +684,18 @@
         :param str field: The field
         :param value: The Value
         """
         c = self._current()
         if c is None:
             raise NoRecordException('cannot get a value from nothing, did you forget to call next() or initialize()?')
         if field not in c:
-            c[field] = GlideElement(field, value, parent_record=self)
+            if isinstance(value, GlideElement):
+                c[field] = GlideElement(field, value.get_value(), value.get_display_value(), parent_record=self)
+            else:
+                c[field] = GlideElement(field, value, parent_record=self)
         else:
             c[field].set_value(value)
 
     def set_display_value(self, field, value):
         """
         Set the display value for a field.
 
@@ -718,20 +723,19 @@
         obj = self._current()
         stack = '&sysparm_stack=%s_list.do?sysparm_query=active=true' % self.__table
         if no_stack:
             stack = ''
         id = self.sys_id if obj else 'null'
         return "{}/{}.do?sys_id={}{}".format(ins, self.__table, id, stack)
 
-    def get_link_list(self) -> str:
+    def get_link_list(self) -> Optional[str]:
         """
         Generate a full URL to for the current query.
 
         :return: The full URL to the record query
-        :rtype: str
         """
         ins = self._client.instance
         sysparm_query = self.get_encoded_query()
         url = "{}/{}_list.do".format(ins, self.__table)
         # Using `requests` as to be py2/3 agnostic and to encode the URL properly.
         return Request('GET', url, params=dict(sysparm_query=sysparm_query)).prepare().url
 
@@ -745,15 +749,15 @@
 
     def get_unique_name(self) -> str:
         """
         always give us the sys_id
         """
         return self.get_value('sys_id')
 
-    def get_attachments(self) -> Attachment:
+    def get_attachments(self) -> 'Attachment':
         """
         Get the attachments for the current record or the current table
 
         :return: A list of attachments
         :rtype: :class:`pysnc.Attachment`
         """
         attachment = self._client.Attachment(self.__table)
@@ -763,15 +767,15 @@
         return attachment
 
     def add_attachment(self, file_name, file, content_type=None, encryption_context=None):
         if self._current() is None:
             raise NoRecordException('cannot add attachment to nothing, did you forget to call next() or initialize()?')
 
         attachment = self._client.Attachment(self.__table)
-        attachment.add_attachment(self.sys_id, file_name, file, content_type, encryption_context)
+        return attachment.add_attachment(self.sys_id, file_name, file, content_type, encryption_context)
 
     def add_active_query(self) -> QueryCondition:
         """
         Equivilant to the following::
 
            add_query('active', 'true')
 
@@ -863,15 +867,15 @@
            add_query(field, '', 'ISNOTEMPTY')
 
         :param str field: The field to validate
         """
         return self.__query.add_not_null_query(field)
 
     def _serialize(self, record, display_value, fields=None, changes_only=False):
-        if isinstance(display_value, string_types):
+        if isinstance(display_value, str):
             v_type = 'both'
         else:
             v_type = 'display_value' if display_value else 'value'
 
         def compress(obj):
             ret = dict()
             if not obj:
@@ -892,15 +896,15 @@
                     ret[key] = value.get_value()
             return ret
 
         return compress(record)
 
     def serialize(self, display_value=False, fields=None, fmt=None, changes_only=False) -> Any:
         """
-        Turn current record into a dict
+        Turn current record into a dictGlideRecord(None, 'incident')
 
         :param display_value: ``True``, ``False``, or ``'both'``
         :param list fields: Fields to serialize. Defaults to all fields.
         :param str fmt: None or ``pandas``. Defaults to None
         :param changes_only: Do we want to serialize only the fields we've modified?
         :return: dict representation
         """
@@ -1019,15 +1023,15 @@
 
         :return: ``True`` or ``False`` based on success
         """
         l = len(self.__results)
         if l > 0 and self.__current+1 < l:
             self.__current = self.__current + 1
             if self.__is_iter:
-                return self
+                return self  # type: ignore  # this typing is internal only
             return True
         if self.__total and self.__total > 0 and \
                 (self.__current+1) < self.__total and \
                 self.__total > len(self.__results) and \
                 _recursive is False:
             if self.__limit:
                 if self.__current+1 < self.__limit:
```

### Comparing `pysnc-1.1.3/pysnc/utils.py` & `pysnc-1.1.4/pysnc/utils.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.3/PKG-INFO` & `pysnc-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysnc
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python SNC (REST) API
 Home-page: https://github.com/ServiceNow/PySNC
 License: MIT
 Keywords: servicenow,snc
 Author: Matthew Gill
 Author-email: matthew.gill@servicenow.com
 Requires-Python: >=3.8,<4.0
@@ -18,15 +18,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: oauth
 Requires-Dist: requests (>=2.8.1)
 Requires-Dist: requests-oauthlib (>=1.2.0) ; extra == "oauth"
-Requires-Dist: six (>=1.10.0)
 Project-URL: Documentation, https://servicenow.github.io/PySNC/
 Project-URL: Repository, https://github.com/ServiceNow/PySNC
 Description-Content-Type: text/markdown
 
 # ServiceNow Python API
 
 **What:**
```

