# Comparing `tmp/fal_serverless-0.6.30.tar.gz` & `tmp/fal_serverless-0.6.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal_serverless-0.6.30.tar", max compression
+gzip compressed data, was "fal_serverless-0.6.31.tar", max compression
```

## Comparing `fal_serverless-0.6.30.tar` & `fal_serverless-0.6.31.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        0 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/README.md
--rw-r--r--   0        0        0      998 2023-05-04 21:44:00.928261 fal_serverless-0.6.30/pyproject.toml
--rw-r--r--   0        0        0      335 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/__init__.py
--rw-r--r--   0        0        0    17406 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/api.py
--rw-r--r--   0        0        0     2390 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/auth/__init__.py
--rw-r--r--   0        0        0     5292 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/auth/auth0.py
--rw-r--r--   0        0        0     1786 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/auth/local.py
--rw-r--r--   0        0        0    11653 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/cli.py
--rw-r--r--   0        0        0      132 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/console/__init__.py
--rw-r--r--   0        0        0      108 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/console/icons.py
--rw-r--r--   0        0        0      485 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/console/ux.py
--rw-r--r--   0        0        0      172 2023-05-04 21:43:52.340291 fal_serverless-0.6.30/src/fal_serverless/env.py
--rw-r--r--   0        0        0      938 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/exceptions/__init__.py
--rw-r--r--   0        0        0      412 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/exceptions/_base.py
--rw-r--r--   0        0        0      353 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/exceptions/auth.py
--rw-r--r--   0        0        0     1435 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/exceptions/handlers.py
--rw-r--r--   0        0        0      326 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/flags.py
--rw-r--r--   0        0        0     1649 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/logging/__init__.py
--rw-r--r--   0        0        0     2574 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/logging/datadog.py
--rw-r--r--   0        0        0     1534 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/logging/isolate.py
--rw-r--r--   0        0        0      386 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/logging/style.py
--rw-r--r--   0        0        0     1785 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/logging/trace.py
--rw-r--r--   0        0        0      643 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/logging/user.py
--rw-r--r--   0        0        0    15210 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/sdk.py
--rw-r--r--   0        0        0     4368 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/sync.py
--rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 fal_serverless-0.6.30/setup.py
--rw-r--r--   0        0        0     1396 1970-01-01 00:00:00.000000 fal_serverless-0.6.30/PKG-INFO
+-rw-r--r--   0        0        0      213 2023-05-08 12:43:58.060579 fal_serverless-0.6.31/README.md
+-rw-r--r--   0        0        0      998 2023-05-08 12:44:13.456756 fal_serverless-0.6.31/pyproject.toml
+-rw-r--r--   0        0        0      335 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/__init__.py
+-rw-r--r--   0        0        0    17406 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/api.py
+-rw-r--r--   0        0        0     2532 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/auth/__init__.py
+-rw-r--r--   0        0        0     5027 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/auth/auth0.py
+-rw-r--r--   0        0        0     1786 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/auth/local.py
+-rw-r--r--   0        0        0    12772 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/cli.py
+-rw-r--r--   0        0        0      132 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/console/__init__.py
+-rw-r--r--   0        0        0      108 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/console/icons.py
+-rw-r--r--   0        0        0      485 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/console/ux.py
+-rw-r--r--   0        0        0      172 2023-05-08 12:44:07.892691 fal_serverless-0.6.31/src/fal_serverless/env.py
+-rw-r--r--   0        0        0      938 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/exceptions/__init__.py
+-rw-r--r--   0        0        0      412 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/exceptions/_base.py
+-rw-r--r--   0        0        0      353 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/exceptions/auth.py
+-rw-r--r--   0        0        0     1435 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/exceptions/handlers.py
+-rw-r--r--   0        0        0      326 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/flags.py
+-rw-r--r--   0        0        0     1649 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/logging/__init__.py
+-rw-r--r--   0        0        0     2574 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/logging/datadog.py
+-rw-r--r--   0        0        0     2122 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/logging/isolate.py
+-rw-r--r--   0        0        0      386 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/logging/style.py
+-rw-r--r--   0        0        0     1785 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/logging/trace.py
+-rw-r--r--   0        0        0      643 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/logging/user.py
+-rw-r--r--   0        0        0    15210 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/sdk.py
+-rw-r--r--   0        0        0     5335 2023-05-08 12:43:58.064579 fal_serverless-0.6.31/src/fal_serverless/sync.py
+-rw-r--r--   0        0        0     1779 1970-01-01 00:00:00.000000 fal_serverless-0.6.31/setup.py
+-rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 fal_serverless-0.6.31/PKG-INFO
```

### Comparing `fal_serverless-0.6.30/pyproject.toml` & `fal_serverless-0.6.31/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fal_serverless"
-version = "0.6.30"
+version = "0.6.31"
 description = "fal Serverless is an easy-to-use Serverless Python Framework"
 authors = ["Features & Labels <hello@fal.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 auth0-python = "^4.1.0"
```

### Comparing `fal_serverless-0.6.30/src/fal_serverless/api.py` & `fal_serverless-0.6.31/src/fal_serverless/api.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.30/src/fal_serverless/auth/__init__.py` & `fal_serverless-0.6.31/src/fal_serverless/auth/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,27 +19,32 @@
     if refresh_token is None:
         raise click.ClickException(message="You're not logged in")
     auth0.revoke(refresh_token)
     local.delete_token()
     console.print(f"{CHECK_ICON} Logged out of [cyan bold]fal Serverless[/]. Bye!")
 
 
-def _fetch_access_token() -> str:
+def refresh():
+    _fetch_access_token(refresh=True)
+    console.print(f"{CHECK_ICON} Refreshed access token")
+
+
+def _fetch_access_token(refresh=False) -> str:
     """
     Load the refresh token, request a new access_token (refreshing the refresh token)
     and return the access_token.
     """
     # We need to lock both read and write access because we could be reading a soon invalid refresh_token
     with local.lock_token():
         refresh_token, access_token = local.load_token()
 
         if refresh_token is None:
             raise UnauthenticatedException()
 
-        if access_token is not None:
+        if access_token is not None and not refresh:
             try:
                 auth0.validate_access_token(access_token)
                 return access_token
             except:
                 # access_token expired, will refresh
                 pass
```

### Comparing `fal_serverless-0.6.30/src/fal_serverless/auth/auth0.py` & `fal_serverless-0.6.31/src/fal_serverless/auth/auth0.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from auth0.authentication.token_verifier import (
     AsymmetricSignatureVerifier,
     TokenVerifier,
 )
 from fal_serverless.console import console
 from fal_serverless.console.icons import CHECK_ICON
 from fal_serverless.console.ux import get_browser
-from rich.prompt import Confirm
 
 AUTH0_DOMAIN = "auth.fal.ai"
 AUTH0_JWKS_URL = f"https://{AUTH0_DOMAIN}/.well-known/jwks.json"
 AUTH0_ALGORITHMS = ["RS256"]
 AUTH0_ISSUER = f"https://{AUTH0_DOMAIN}/"
 AUTH0_FAL_API_AUDIENCE_ID = "fal-cloud"
 AUTH0_CLIENT_ID = "TwXR51Vz8JbY8GUUMy6EyuVR0fTO7N4N"
@@ -41,34 +40,30 @@
 
     device_code_data = device_code_response.json()
     device_user_code = device_code_data["user_code"]
     device_confirmation_url = device_code_data["verification_uri_complete"]
 
     browser = get_browser()
     console.print()
-    if browser is None:
+
+    if browser is not None and click.confirm(
+        "Open browser automatically ('no' to show URL)?", default=True, err=True
+    ):
+        browser.open_new_tab(device_confirmation_url)
+    else:
         console.print(
             f"1. On your computer or mobile device navigate to: {device_confirmation_url}"
         )
         console.print(
-            f"2. Confirm it shows the following code: [markdown.code]{device_user_code}[/]\n"
+            f"2. Confirm it shows the following code: [markdown.code]{device_user_code}[/]"
         )
-    else:
-        console.print(
-            f"Once the page loads, confirm it shows the following code: [markdown.code]{device_user_code}[/]"
-        )
-        Confirm.get_input(
-            console=console,
-            prompt="A browser will open with the login page when you [bold]Press Enter...[/]",
-            password=True,
-        )
-        # This is needed to suppress the ResourceWarning emitted
-        # when the process is waiting for user confirmation
-        warnings.filterwarnings("ignore", category=ResourceWarning)
-        browser.open_new_tab(device_confirmation_url)
+
+    # This is needed to suppress the ResourceWarning emitted
+    # when the process is waiting for user confirmation
+    warnings.filterwarnings("ignore", category=ResourceWarning)
 
     token_payload = {
         "grant_type": "urn:ietf:params:oauth:grant-type:device_code",
         "device_code": device_code_data["device_code"],
         "client_id": AUTH0_CLIENT_ID,
     }
```

### Comparing `fal_serverless-0.6.30/src/fal_serverless/auth/local.py` & `fal_serverless-0.6.31/src/fal_serverless/auth/local.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.30/src/fal_serverless/cli.py` & `fal_serverless-0.6.31/src/fal_serverless/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
+import datetime
+import operator
 from sys import argv
 from uuid import uuid4
 
 import click
 import fal_serverless.auth as auth
 from fal_serverless import api, sdk
 from fal_serverless.console import console
 from fal_serverless.exceptions import ApplicationExceptionHandler
 from fal_serverless.logging import get_logger, set_debug_logging
 from fal_serverless.logging.isolate import IsolateLogPrinter
 from fal_serverless.logging.trace import get_tracer
+from fal_serverless.sync import list_children, parse_logs
 from rich.table import Table
 
 DEFAULT_HOST = "api.alpha.fal.ai"
 HOST_ENVVAR = "FAL_HOST"
 
 DEFAULT_PORT = "443"
 PORT_ENVVAR = "FAL_PORT"
@@ -96,14 +99,19 @@
 
 
 @auth_cli.command(name="logout")
 def auth_logout():
     auth.logout()
 
 
+@auth_cli.command(name="refresh")
+def auth_refresh():
+    auth.refresh()
+
+
 @auth_cli.command(name="hello", hidden=True)
 def auth_test():
     """
     To test auth.
     """
     print(f"Hello, {auth.USER.info['name']} - '{auth.USER.info['sub']}'")
 
@@ -253,14 +261,39 @@
     cron_id = client.schedule(
         func=isolated_function.func, cron=cron_string, options=isolated_function.options
     )
     if cron_id:
         console.print(cron_id)
 
 
+@function_cli.command("logs")
+@click.argument("url", required=True)
+@click.argument("call_id", required=True)
+@click.pass_obj
+def get_logs(client: api.FalServerlessHost, url: str, call_id: str):
+    logs = parse_logs(f"/data/logs/gateway/{url}/{call_id}")
+    log_printer = IsolateLogPrinter(debug=True)
+    for log in logs:
+        log_printer.print_dict(log)
+
+
+@function_cli.command("calls")
+@click.argument("url", required=True)
+@click.pass_obj
+def get_function_call_ids(client: api.FalServerlessHost, url: str):
+    # This will only return a list calls that we have logs for.
+    calls = list_children(f"/data/logs/gateway/{url}")
+    calls.sort(key=operator.itemgetter("updated_time"))
+    for call in calls:
+        name = call["name"].split(".")[0]
+        timestamp = datetime.datetime.fromtimestamp(call["updated_time"])
+        timestamp_str = timestamp.strftime("%Y-%m-%d %H:%M:%S.%f")[:-3]
+        console.print(f"{timestamp_str}: {name}")
+
+
 ##### Crons group #####
 @cli.group("crons")
 @click.option("--host", default=DEFAULT_HOST, envvar=HOST_ENVVAR)
 @click.option("--port", default=DEFAULT_PORT, envvar=PORT_ENVVAR, hidden=True)
 @click.pass_context
 def crons_cli(ctx, host: str, port: str):
     ctx.obj = api.FalServerlessHost(f"{host}:{port}")
```

### Comparing `fal_serverless-0.6.30/src/fal_serverless/exceptions/__init__.py` & `fal_serverless-0.6.31/src/fal_serverless/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.30/src/fal_serverless/exceptions/handlers.py` & `fal_serverless-0.6.31/src/fal_serverless/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.30/src/fal_serverless/logging/__init__.py` & `fal_serverless-0.6.31/src/fal_serverless/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.30/src/fal_serverless/logging/datadog.py` & `fal_serverless-0.6.31/src/fal_serverless/logging/datadog.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.30/src/fal_serverless/logging/trace.py` & `fal_serverless-0.6.31/src/fal_serverless/logging/trace.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.30/src/fal_serverless/logging/user.py` & `fal_serverless-0.6.31/src/fal_serverless/logging/user.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.30/src/fal_serverless/sdk.py` & `fal_serverless-0.6.31/src/fal_serverless/sdk.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.30/src/fal_serverless/sync.py` & `fal_serverless-0.6.31/src/fal_serverless/sync.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import hashlib
 import os
 import shutil
 import zipfile
+from typing import Any
 
 from pathspec import PathSpec
 
 from .api import isolated
 
 CHUNK_SIZE = 1024 * 1024 * 10  # 10 MB
 
@@ -44,14 +45,51 @@
 @isolated()
 def _clear_destination_file(destination_path):
     os.makedirs("/data/sync", exist_ok=True)
     with open(destination_path, "wb") as f:
         f.truncate(0)
 
 
+@isolated()
+def list_children(parent_directory: str) -> list[dict]:
+    items: list[dict] = []
+
+    if not os.path.exists(parent_directory):
+        return items
+
+    for file_name in os.listdir(parent_directory):
+        file_path = os.path.join(parent_directory, file_name)
+
+        created_time = os.path.getctime(file_path)
+        updated_time = os.path.getmtime(file_path)
+
+        items.append(
+            {
+                "name": file_name,
+                "created_time": created_time,
+                "updated_time": updated_time,
+                "is_file": os.path.isfile(file_path),
+            }
+        )
+
+    return items
+
+
+@isolated()
+def parse_logs(file_path: str) -> Any:
+    import json
+
+    if os.path.exists(file_path):
+        with open(file_path) as f:
+            lines = f.readlines()
+            parsed = [json.loads(line) for line in lines]
+            return [log for sub in parsed for log in sub]
+    return []
+
+
 def _upload_file(source_path: str, destination_path: str) -> None:
     file_size = os.path.getsize(source_path)
     total_chunks = (file_size // CHUNK_SIZE) + (1 if file_size % CHUNK_SIZE else 0)
 
     # Clear the destination file
     _clear_destination_file(destination_path)
     for chunk_number in range(total_chunks):
```

### Comparing `fal_serverless-0.6.30/setup.py` & `fal_serverless-0.6.31/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 {':python_version < "3.10"': ['importlib-metadata>=4.4']}
 
 entry_points = \
 {'console_scripts': ['fal-serverless = fal_serverless.cli:cli']}
 
 setup_kwargs = {
     'name': 'fal-serverless',
-    'version': '0.6.30',
+    'version': '0.6.31',
     'description': 'fal Serverless is an easy-to-use Serverless Python Framework',
-    'long_description': '',
+    'long_description': '# fal-serverless\n\nLibrary to run, serve or schedule your Python functions in the cloud with any machine type you may need.\n\nCheck out to the [docs](https://docs.fal.ai/fal-serverless/quickstart) for more details.\n',
     'author': 'Features & Labels',
     'author_email': 'hello@fal.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `fal_serverless-0.6.30/PKG-INFO` & `fal_serverless-0.6.31/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fal-serverless
-Version: 0.6.30
+Version: 0.6.31
 Summary: fal Serverless is an easy-to-use Serverless Python Framework
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -28,8 +28,13 @@
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: structlog (>=22.3.0,<23.0.0)
 Requires-Dist: typing-extensions (==4.4)
 Description-Content-Type: text/markdown
 
+# fal-serverless
+
+Library to run, serve or schedule your Python functions in the cloud with any machine type you may need.
+
+Check out to the [docs](https://docs.fal.ai/fal-serverless/quickstart) for more details.
```

