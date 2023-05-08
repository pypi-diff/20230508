# Comparing `tmp/oauth2-lib-1.2.8.tar.gz` & `tmp/oauth2-lib-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauth2-lib-1.2.8.tar", last modified: Tue May  2 10:55:14 2023, max compression
+gzip compressed data, was "oauth2-lib-1.2.9.tar", last modified: Mon May  8 10:47:38 2023, max compression
```

## Comparing `oauth2-lib-1.2.8.tar` & `oauth2-lib-1.2.9.tar`

### file list

```diff
@@ -1,23 +1,29 @@
--rw-r--r--   0        0        0      363 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/.bumpversion.cfg
--rw-r--r--   0        0        0      550 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0      389 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/.github/workflows/pull-request.yml
--rw-r--r--   0        0        0     1894 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1533 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/.github/workflows/test-package.yml
--rw-r--r--   0        0        0     1103 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/.gitignore
--rw-r--r--   0        0        0     2061 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/LICENSE
--rw-r--r--   0        0        0     1754 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/README.md
--rwxr-xr-x   0        0        0      150 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/fmt_code.sh
--rw-r--r--   0        0        0      671 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/oauth2_lib/__init__.py
--rw-r--r--   0        0        0     7665 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/oauth2_lib/async_api_client.py
--rw-r--r--   0        0        0    15379 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/oauth2_lib/fastapi.py
--rw-r--r--   0        0        0        0 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/oauth2_lib/py.typed
--rw-r--r--   0        0        0     2511 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     1151 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/setup.cfg
--rw-r--r--   0        0        0        0 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/tests/__init__.py
--rw-r--r--   0        0        0     3273 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/tests/conftest.py
--rw-r--r--   0        0        0     7113 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/tests/test_async_api_client.py
--rw-r--r--   0        0        0    13734 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/tests/test_fastapi.py
--rw-r--r--   0        0        0     6570 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/tests/test_opa_decision.py
--rw-r--r--   0        0        0      474 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/tests/test_opa_graphql_decision.py
--rw-r--r--   0        0        0     4589 1970-01-01 00:00:00.000000 oauth2-lib-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0      363 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/.bumpversion.cfg
+-rw-r--r--   0        0        0      550 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0      389 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/.github/workflows/pull-request.yml
+-rw-r--r--   0        0        0     1894 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1533 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/.github/workflows/test-package.yml
+-rw-r--r--   0        0        0     1103 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/.gitignore
+-rw-r--r--   0        0        0     2054 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/LICENSE
+-rw-r--r--   0        0        0     1754 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/README.md
+-rwxr-xr-x   0        0        0      150 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/fmt_code.sh
+-rw-r--r--   0        0        0      671 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/oauth2_lib/__init__.py
+-rw-r--r--   0        0        0     7665 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/oauth2_lib/async_api_client.py
+-rw-r--r--   0        0        0    15651 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/oauth2_lib/fastapi.py
+-rw-r--r--   0        0        0     6112 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/oauth2_lib/graphql_authentication.py
+-rw-r--r--   0        0        0        0 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/oauth2_lib/py.typed
+-rw-r--r--   0        0        0      943 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/oauth2_lib/settings.py
+-rw-r--r--   0        0        0     2546 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1151 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/tests/__init__.py
+-rw-r--r--   0        0        0     3273 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/tests/conftest.py
+-rw-r--r--   0        0        0     2781 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/tests/graphql/conftest.py
+-rw-r--r--   0        0        0     1541 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/tests/graphql/test_authenticated_federated_field.py
+-rw-r--r--   0        0        0     2360 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/tests/graphql/test_authenticated_field.py
+-rw-r--r--   0        0        0     3052 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/tests/graphql/test_authenticated_mutation_field.py
+-rw-r--r--   0        0        0     7113 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/tests/test_async_api_client.py
+-rw-r--r--   0        0        0    13734 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/tests/test_fastapi.py
+-rw-r--r--   0        0        0     6570 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/tests/test_opa_decision.py
+-rw-r--r--   0        0        0     4289 2023-05-08 10:47:33.096831 oauth2-lib-1.2.9/tests/test_opa_graphql_decision.py
+-rw-r--r--   0        0        0     4632 1970-01-01 00:00:00.000000 oauth2-lib-1.2.9/PKG-INFO
```

### Comparing `oauth2-lib-1.2.8/.github/workflows/publish-release.yml` & `oauth2-lib-1.2.9/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.8/.github/workflows/scheduled-build.yml` & `oauth2-lib-1.2.9/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.8/.github/workflows/test-package.yml` & `oauth2-lib-1.2.9/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.8/.gitignore` & `oauth2-lib-1.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.8/.pre-commit-config.yaml` & `oauth2-lib-1.2.9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
       - id: requirements-txt-fixer
       - id: detect-private-key
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies:
-          - flake8-bandit==3.0.0
+          - flake8-bandit
           - flake8-bugbear
           - flake8-comprehensions
           - flake8-docstrings
           - flake8-logging-format
           - flake8-pep3101
           - flake8-print
           - flake8-rst
```

### Comparing `oauth2-lib-1.2.8/LICENSE` & `oauth2-lib-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.8/README.md` & `oauth2-lib-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.8/oauth2_lib/__init__.py` & `oauth2-lib-1.2.9/oauth2_lib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the SURF Oauth2 module that interfaces with the oauth2 setup."""
 
-__version__ = "1.2.8"
+__version__ = "1.2.9"
```

### Comparing `oauth2-lib-1.2.8/oauth2_lib/async_api_client.py` & `oauth2-lib-1.2.9/oauth2_lib/async_api_client.py`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.8/oauth2_lib/fastapi.py` & `oauth2-lib-1.2.9/oauth2_lib/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,18 +370,20 @@
 
 def opa_graphql_decision(
     opa_url: str,
     _oidc_security: OIDCUser,
     enabled: bool = True,
     auto_error: bool = True,
     opa_kwargs: Union[Mapping[str, str], None] = None,
+    async_request: Union[AsyncClient, None] = None,
 ) -> Callable[[str, OIDCUserModel], Coroutine[Any, Any, Union[bool, None]]]:
     async def _opa_decision(
         path: str,
         oidc_user: OIDCUserModel = Depends(_oidc_security),
+        async_request_1: Union[AsyncClient, None] = None,
     ) -> Union[bool, None]:
         """
         Check OIDCUserModel against the OPA policy.
 
         This is used as a security module in Graphql projects
         This method will make an async call towards the Policy agent.
 
@@ -396,17 +398,18 @@
                     **oidc_user,
                     "resource": path,
                     "method": "POST",
                 }
             }
 
             logger.debug("Posting input json to Policy agent", input=opa_input)
-
+            client_request = async_request if async_request else async_request_1
+            client_request = client_request if client_request else AsyncClient(http1=True)
             try:
-                result = await AsyncClient(http1=True).post(opa_url, json=opa_input)
+                result = await client_request.post(opa_url, json=opa_input)
             except (NetworkError, TypeError):
                 raise HTTPException(status_code=HTTPStatus.SERVICE_UNAVAILABLE, detail="Policy agent is unavailable")
 
             data = OPAResult.parse_obj(result.json())
 
             resource = opa_input["input"]["resource"]
```

### Comparing `oauth2-lib-1.2.8/pyproject.toml` & `oauth2-lib-1.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     "requests>=2.19.0",
     "structlog>=20.2.0",
     "fastapi>=0.90.1",
     "opentelemetry-distro",
     "httpx[http2]==0.23.0",
     "authlib==1.0.1",
     "pydantic>=1.8.0",
+    "strawberry-graphql>=0.171.1",
 ]
 description-file = "README.md"
 requires-python = ">=3.9"
 
 [tool.flit.metadata.urls]
 Documentation = "https://workfloworchestrator.org/"
```

### Comparing `oauth2-lib-1.2.8/setup.cfg` & `oauth2-lib-1.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.8/tests/conftest.py` & `oauth2-lib-1.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.8/tests/test_async_api_client.py` & `oauth2-lib-1.2.9/tests/test_async_api_client.py`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.8/tests/test_fastapi.py` & `oauth2-lib-1.2.9/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.8/tests/test_opa_decision.py` & `oauth2-lib-1.2.9/tests/test_opa_decision.py`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.8/PKG-INFO` & `oauth2-lib-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauth2-lib
-Version: 1.2.8
+Version: 1.2.9
 Summary: This is the SURF Oauth2 module that interfaces with the oauth2 setup.
 Home-page: https://github.com/workfloworchestrator/oauth2-lib
 Author: SURF
 Author-email: automation-beheer@surf.nl
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -29,14 +29,15 @@
 Requires-Dist: requests>=2.19.0
 Requires-Dist: structlog>=20.2.0
 Requires-Dist: fastapi>=0.90.1
 Requires-Dist: opentelemetry-distro
 Requires-Dist: httpx[http2]==0.23.0
 Requires-Dist: authlib==1.0.1
 Requires-Dist: pydantic>=1.8.0
+Requires-Dist: strawberry-graphql>=0.171.1
 Requires-Dist: bumpversion ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: apache-license-check ; extra == "test"
 Requires-Dist: black ; extra == "test"
 Requires-Dist: flake8 ; extra == "test"
 Requires-Dist: flake8-bandit>=3.0.0 ; extra == "test"
 Requires-Dist: flake8-bugbear ; extra == "test"
```

