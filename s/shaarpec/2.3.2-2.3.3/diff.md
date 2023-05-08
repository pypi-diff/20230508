# Comparing `tmp/shaarpec-2.3.2.tar.gz` & `tmp/shaarpec-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaarpec-2.3.2.tar", max compression
+gzip compressed data, was "shaarpec-2.3.3.tar", max compression
```

## Comparing `shaarpec-2.3.2.tar` & `shaarpec-2.3.3.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1080 2022-07-19 21:50:58.228912 shaarpec-2.3.2/LICENSE
--rw-r--r--   0        0        0    10581 2023-03-27 13:41:38.160424 shaarpec-2.3.2/README.md
--rw-r--r--   0        0        0     1286 2023-05-02 08:39:32.060980 shaarpec-2.3.2/pyproject.toml
--rw-r--r--   0        0        0       77 2022-07-08 12:22:12.414817 shaarpec-2.3.2/shaarpec/__init__.py
--rw-r--r--   0        0        0    16262 2023-03-27 11:44:05.074127 shaarpec-2.3.2/shaarpec/client.py
--rw-r--r--   0        0        0     1681 2023-05-02 08:39:32.060980 shaarpec-2.3.2/shaarpec/tasks.py
--rw-r--r--   0        0        0      178 2023-01-12 08:38:33.681606 shaarpec-2.3.2/shaarpec/utils.py
--rw-r--r--   0        0        0    12350 1970-01-01 00:00:00.000000 shaarpec-2.3.2/setup.py
--rw-r--r--   0        0        0    12184 1970-01-01 00:00:00.000000 shaarpec-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-07-19 21:50:58.228912 shaarpec-2.3.3/LICENSE
+-rw-r--r--   0        0        0    11309 2023-05-08 11:50:47.491411 shaarpec-2.3.3/README.md
+-rw-r--r--   0        0        0     1287 2023-05-08 11:53:21.313596 shaarpec-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0       77 2022-07-08 12:22:12.414817 shaarpec-2.3.3/shaarpec/__init__.py
+-rw-r--r--   0        0        0    16262 2023-03-27 11:44:05.074127 shaarpec-2.3.3/shaarpec/client.py
+-rw-r--r--   0        0        0     1681 2023-05-02 08:39:32.060980 shaarpec-2.3.3/shaarpec/tasks.py
+-rw-r--r--   0        0        0      178 2023-01-12 08:38:33.681606 shaarpec-2.3.3/shaarpec/utils.py
+-rw-r--r--   0        0        0    12919 1970-01-01 00:00:00.000000 shaarpec-2.3.3/PKG-INFO
```

### Comparing `shaarpec-2.3.2/LICENSE` & `shaarpec-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shaarpec-2.3.2/README.md` & `shaarpec-2.3.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-
 <!-- PROJECT SHIELDS -->
 <!--
 *** I'm using markdown "reference style" links for readability.
 *** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
 *** See the bottom of this document for the declaration of the reference variables
 *** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
 *** https://www.markdownguide.org/basic-syntax/#reference-style-links
 -->
+
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 
-
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/SHAARPEC/shaarpec-python-client">
     <img src="images/logo.png" alt="Logo" width="248" height="95">
   </a>
 
@@ -31,16 +30,14 @@
     ·
     <a href="https://github.com/SHAARPEC/shaarpec-python-client/issues">Report Bug</a>
     ·
     <a href="https://github.com/SHAARPEC/shaarpec-python-client/issues">Request Feature</a>
   </p>
 </div>
 
-
-
 <!-- TABLE OF CONTENTS -->
 <details>
   <summary>Table of Contents</summary>
   <ol>
     <li>
       <a href="#about-the-project">About The Project</a>
       <ul>
@@ -51,80 +48,84 @@
       <a href="#getting-started">Getting Started</a>
       <ul>
         <li><a href="#prerequisites">Prerequisites</a></li>
         <li><a href="#installation">Installation</a></li>
       </ul>
     </li>
     <li><a href="#usage">Usage</a></li>
+    <li><a href="#troubleshooting">Troubleshooting</a></li>
     <li><a href="#roadmap">Roadmap</a></li>
     <li><a href="#license">License</a></li>
     <li><a href="#contact">Contact</a></li>
   </ol>
 </details>
 
-
-
 <!-- ABOUT THE PROJECT -->
+
 ## About The Project
 
 [![SHAARPEC API screenshot][product-screenshot]](https://www.shaarpec.com)
 
 This is a Python client for simple access to the SHAARPEC Analytics API. Authentication is handled automatically via device flow, authorization code flow, or client credentials flow. Authentication can also be disabled if accessing a public Analytics API.
 
 The SHAARPEC Analytics API provides calculations on the healthcare organization's resources, capacities, clinical outcomes, and much more. These results can be accessed via a standard REST API, which is usually protected by the SHAARPEC Identity Server.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ### Built With
 
-* [![Httpx][Httpx]][Httpx]
-* [![Python][Python]][Python-url]
+-   [![Httpx][Httpx]][Httpx]
+-   [![Python][Python]][Python-url]
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- GETTING STARTED -->
+
 ## Getting Started
 
 ### Prerequisites
 
 The shaarpec client is used as a standard Python library. It is always a good idea to install the library in a virtual environment.
 
 ### Installation
 
 1. Install the library into your virtual environment.
-   ```bash
-   pip install shaarpec
-   ```
+    ```bash
+    pip install shaarpec
+    ```
 2. Store your credentials to the SHAARPEC IdentityServer in an .env file.
-   ```bash
-   $ cat .env
-   OIDCISH_HOST="https://idp.example.com"
-   OIDCISH_CLIENT_ID="my client id"
-   OIDCISH_CLIENT_SECRET="my client secret"
-   OIDCISH_AUDIENCE="shaarpec_api.full_access_scope"
-   OIDCISH_SCOPE="openid shaarpec_api.full_access_scope offline_access"
-   ```
+    ```bash
+    $ cat .env
+    OIDCISH_HOST="https://idp.example.com"
+    OIDCISH_CLIENT_ID="my client id"
+    OIDCISH_CLIENT_SECRET="my client secret"
+    OIDCISH_AUDIENCE="shaarpec_api.full_access_scope"
+    OIDCISH_SCOPE="openid shaarpec_api.full_access_scope offline_access"
+    ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- USAGE EXAMPLES -->
+
 ## Usage
 
-This library provides a Client class to easily interact with the SHAARPEC Analytics API. The class methods `Client.with_device(...)`,  `Client.with_code(...)`, and `Client.with_credentials(...)` create clients that authenticate with the SHAARPEC IdentityServer with either device flow (not tied to an individual user, recommended), code flow (tied to an individual user, for debugging and development), or credentials flow (non-interactive). There is also a class method `Client.without_auth(...)` that does not invoke the IDP server (but will only work if the Analytics API is public, otherwise give 401 Authentication invalid errors).
+This library provides a Client class to easily interact with the SHAARPEC Analytics API. The class methods `Client.with_device(...)`, `Client.with_code(...)`, and `Client.with_credentials(...)` create clients that authenticate with the SHAARPEC IdentityServer with either device flow (not tied to an individual user, recommended), code flow (tied to an individual user, for debugging and development), or credentials flow (non-interactive). There is also a class method `Client.without_auth(...)` that does not invoke the IDP server (but will only work if the Analytics API is public, otherwise give 401 Authentication invalid errors).
 
 All API data is returned as `httpx.Response` objects.
 
 Let's look at some code examples on how to get data from the Analytics API. First, import the client.
+
 ```python
 from shaarpec import Client
 ```
 
 Next, use [device flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/device-authorization-flow) or [code flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/authorization-code-flow) to connect the client to the API with the `Client.with_device(...)`, `Client.with_code(...)`, and/or `Client.with_credentials(...)` class methods.
 
 The credentials can either be stored in a .env file in the working directory (as explained in the Prerequisites section), provided as a path, or given directly as arguments to the `auth` dict.
+
 ```python
 # Create a client with device flow, give authentication details directly.
 client = Client.with_device(
         host="https://api.shaarpec.com/",
         auth={
             "host": "https://idp.shaarpec.com",
             "client_id": ...,
@@ -132,31 +133,35 @@
             "scope": ...,
             "audience": ...
         }
     )
 # Create a client with device flow, read authentication details from .env file.
 client = Client.with_device(host="https://api.shaarpec.com/", auth="path/to/.env")
 ```
+
 Here `host` is the base URL to the Analytics API and `auth` is a dictionary with the login credentials. With device flow, the user needs to finish the sign-in by visiting a url provided by the IdentityServer. A message will be shown:
 
 > Visit https://idp.shaarpec.com/device?userCode=XXXXXXXXX to complete sign-in.
 
 The user visits the website, verifies that the user code is correct and confirms the sign-in. After a few seconds, the client will confirm the sign-in:
 
 > SUCCESS: Authentication was successful. Took XX.Y seconds.
 
-The client is now connected to the API. Visit the Analytics API Base URL to interactively test the endpoints and read their documentation and about their path and query parameters. These parameters are used in the regular (`requests` and `httpx`) way with `client.verb` calls, where `verb` is either `get` or `post`. 
+The client is now connected to the API. Visit the Analytics API Base URL to interactively test the endpoints and read their documentation and about their path and query parameters. These parameters are used in the regular (`requests` and `httpx`) way with `client.verb` calls, where `verb` is either `get` or `post`.
 
 ### GET and POST
 
 The `get` and `post` verbs are supported in the standard way. For example (API responses are returned as `httpx.Response` objects):
+
 ```python
 client.get("terminology/allergy_type").json()
 ```
+
 might return
+
 ```
 {'419263009': 'Allergy to tree pollen',
  '420174000': 'Allergy to wheat',
  '425525006': 'Allergy to dairy product',
  '714035009': 'Allergy to soya',
  '419474003': 'Allergy to mould',
  '232347008': 'Dander (animal) allergy',
@@ -166,19 +171,23 @@
  '232350006': 'House dust mite allergy',
  '418689008': 'Allergy to grass pollen',
  '91935009': 'Allergy to peanuts',
  '91930004': 'Allergy to eggs',
  '300916003': 'Latex allergy',
  '424213003': 'Allergy to bee venom'}
 ```
+
 or
+
 ```python
 client.get("population", conditions=["T78.2", "K81.0"])
 ```
+
 might return
+
 ```
 [{'patient_origin_id': '4c92f494-3c98-f8dd-1473-da9eb0196f6f',
     'age': '10-16',
     'is_alive': True,
     'gender': 'F',
     'deceased_year': 0},
  ...
@@ -206,53 +215,74 @@
     status: str
     success: Optional[bool]
     progress: Optional[float]
     result: Optional[Any]
     error: Optional[Any]
     debugger: Optional[Any]
 ```
+
 As you can see, the success, progress, result and error are optional and updated automatically when available. The method comes with a progress bar which can be disabled via `client.run("path/to/task", progress_bar=False)`. If you want to use the task result in a subsequent command, you can wait (blocking) for the result with the `task.wait_for_result()` method:
 
 ```python
 task = client.run("path/to/task")
 print(f"The result is: {task.wait_for_result()}!")
 ```
 
+<p align="right">(<a href="#top">back to top</a>)</p>
 
+<!-- TROUBLESHOOTING -->
 
-<p align="right">(<a href="#top">back to top</a>)</p>
+## Troubleshooting
+
+### Progress bar fails to render in (Dockerized) Jupyter Lab
+
+Sometimes (especially in a Dockerized environment) the progress bar fails to render when running a task. This seems to be related to an issue in `tqdm` and its dependencies. A workaround seems to be to run:
+
+```bash
+jupyter lab build
+```
+
+in the environment (in a terminal inside the running Docker container) and refresh the browser. This requires a `node.js` installation first, e.g. per:
+
+```
+conda install -c conda-forge nodejs
+```
+
+See discussion for [issue 1310](https://github.com/tqdm/tqdm/issues/1310)
+on the `tqdm` Github repo.
 
 <!-- ROADMAP -->
+
 ## Roadmap
 
 See the [open issues](https://github.com/SHAARPEC/shaarpec-python-client/issues) for a full list of proposed features (and known issues).
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
-
 <!-- LICENSE -->
+
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
-
 <!-- CONTACT -->
+
 ## Contact
 
 SHAARPEC Support - support@shaarpec.com
 
 Project Link: [https://github.com/SHAARPEC/shaarpec-python-client](https://github.com/SHAARPEC/shaarpec-python-client)
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
-
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+
 [contributors-shield]: https://img.shields.io/github/contributors/SHAARPEC/shaarpec-python-client.svg?style=for-the-badge
 [contributors-url]: https://github.com/SHAARPEC/shaarpec-python-client/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/SHAARPEC/shaarpec-python-client.svg?style=for-the-badge
 [forks-url]: https://github.com/SHAARPEC/shaarpec-python-client/network/members
 [stars-shield]: https://img.shields.io/github/stars/SHAARPEC/shaarpec-python-client.svg?style=for-the-badge
 [stars-url]: https://github.com/SHAARPEC/shaarpec-python-client/stargazers
 [issues-shield]: https://img.shields.io/github/issues/SHAARPEC/shaarpec-python-client.svg?style=for-the-badge
```

### Comparing `shaarpec-2.3.2/pyproject.toml` & `shaarpec-2.3.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shaarpec"
-version = "2.3.2"
+version = "2.3.3"
 description = "Client for SHAARPEC Analytics API."
 authors = ["Erik G. Brandt <erik.brandt@shaarpec.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 httpx = "^0.23.3"
@@ -26,20 +26,20 @@
 click = "^8.1.3"
 debugpy = "^1.6.7"
 decorator = "^5.1.1"
 defusedxml = "^0.7.1"
 dill = "^0.3.6"
 ecdsa = "^0.18.0"
 entrypoints = "^0.4"
-ipywidgets = "7.6.5"
 fastjsonschema = "^2.16.3"
 pylint = "^2.17.2"
 tqdm = "^4.65.0"
 executing = "^1.2.0"
 jupyterlab-widgets = "^3.0.7"
+ipywidgets = "^8.0.6"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pylint = "^2.17.2"
 isort = "^5.12.0"
 jupytext = "^1.14.5"
```

### Comparing `shaarpec-2.3.2/shaarpec/client.py` & `shaarpec-2.3.3/shaarpec/client.py`

 * *Files identical despite different names*

### Comparing `shaarpec-2.3.2/shaarpec/tasks.py` & `shaarpec-2.3.3/shaarpec/tasks.py`

 * *Files identical despite different names*

### Comparing `shaarpec-2.3.2/setup.py` & `shaarpec-2.3.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,338 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: shaarpec
+Version: 2.3.3
+Summary: Client for SHAARPEC Analytics API.
+Author: Erik G. Brandt
+Author-email: erik.brandt@shaarpec.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Babel (>=2.12.1,<3.0.0)
+Requires-Dist: anybadge (>=1.14.0,<2.0.0)
+Requires-Dist: anyio (>=3.6.2,<4.0.0)
+Requires-Dist: argon2-cffi (>=21.3.0,<22.0.0)
+Requires-Dist: argon2-cffi-bindings (>=21.2.0,<22.0.0)
+Requires-Dist: asttokens (>=2.2.1,<3.0.0)
+Requires-Dist: attrs (>=22.2.0,<23.0.0)
+Requires-Dist: backcall (>=0.2.0,<0.3.0)
+Requires-Dist: background (>=0.2.1,<0.3.0)
+Requires-Dist: beautifulsoup4 (>=4.12.1,<5.0.0)
+Requires-Dist: bleach (>=6.0.0,<7.0.0)
+Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
+Requires-Dist: cffi (>=1.15.1,<2.0.0)
+Requires-Dist: charset-normalizer (>=3.1.0,<4.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: debugpy (>=1.6.7,<2.0.0)
+Requires-Dist: decorator (>=5.1.1,<6.0.0)
+Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
+Requires-Dist: dill (>=0.3.6,<0.4.0)
+Requires-Dist: ecdsa (>=0.18.0,<0.19.0)
+Requires-Dist: entrypoints (>=0.4,<0.5)
+Requires-Dist: executing (>=1.2.0,<2.0.0)
+Requires-Dist: fastjsonschema (>=2.16.3,<3.0.0)
+Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: ipywidgets (>=8.0.6,<9.0.0)
+Requires-Dist: jupyterlab-widgets (>=3.0.7,<4.0.0)
+Requires-Dist: oidcish (>=0.3.1,<0.4.0)
+Requires-Dist: pylint (>=2.17.2,<3.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['shaarpec']
+<!-- PROJECT SHIELDS -->
+<!--
+*** I'm using markdown "reference style" links for readability.
+*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
+*** See the bottom of this document for the declaration of the reference variables
+*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
+*** https://www.markdownguide.org/basic-syntax/#reference-style-links
+-->
 
-package_data = \
-{'': ['*']}
+[![Contributors][contributors-shield]][contributors-url]
+[![Forks][forks-shield]][forks-url]
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url]
+[![MIT License][license-shield]][license-url]
 
-install_requires = \
-['Babel>=2.12.1,<3.0.0',
- 'anybadge>=1.14.0,<2.0.0',
- 'anyio>=3.6.2,<4.0.0',
- 'argon2-cffi-bindings>=21.2.0,<22.0.0',
- 'argon2-cffi>=21.3.0,<22.0.0',
- 'asttokens>=2.2.1,<3.0.0',
- 'attrs>=22.2.0,<23.0.0',
- 'backcall>=0.2.0,<0.3.0',
- 'background>=0.2.1,<0.3.0',
- 'beautifulsoup4>=4.12.1,<5.0.0',
- 'bleach>=6.0.0,<7.0.0',
- 'certifi>=2022.12.7,<2023.0.0',
- 'cffi>=1.15.1,<2.0.0',
- 'charset-normalizer>=3.1.0,<4.0.0',
- 'click>=8.1.3,<9.0.0',
- 'debugpy>=1.6.7,<2.0.0',
- 'decorator>=5.1.1,<6.0.0',
- 'defusedxml>=0.7.1,<0.8.0',
- 'dill>=0.3.6,<0.4.0',
- 'ecdsa>=0.18.0,<0.19.0',
- 'entrypoints>=0.4,<0.5',
- 'executing>=1.2.0,<2.0.0',
- 'fastjsonschema>=2.16.3,<3.0.0',
- 'httpx>=0.23.3,<0.24.0',
- 'ipywidgets==7.6.5',
- 'jupyterlab-widgets>=3.0.7,<4.0.0',
- 'oidcish>=0.3.1,<0.4.0',
- 'pylint>=2.17.2,<3.0.0',
- 'tqdm>=4.65.0,<5.0.0']
-
-setup_kwargs = {
-    'name': 'shaarpec',
-    'version': '2.3.2',
-    'description': 'Client for SHAARPEC Analytics API.',
-    'long_description': '\n<!-- PROJECT SHIELDS -->\n<!--\n*** I\'m using markdown "reference style" links for readability.\n*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).\n*** See the bottom of this document for the declaration of the reference variables\n*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.\n*** https://www.markdownguide.org/basic-syntax/#reference-style-links\n-->\n[![Contributors][contributors-shield]][contributors-url]\n[![Forks][forks-shield]][forks-url]\n[![Stargazers][stars-shield]][stars-url]\n[![Issues][issues-shield]][issues-url]\n[![MIT License][license-shield]][license-url]\n\n\n<!-- PROJECT LOGO -->\n<br />\n<div align="center">\n  <a href="https://github.com/SHAARPEC/shaarpec-python-client">\n    <img src="images/logo.png" alt="Logo" width="248" height="95">\n  </a>\n\n  <p align="center">\n    Python client for SHAARPEC Analytics API.\n    <br />\n    <a href="https://github.com/SHAARPEC/shaarpec-python-client"><strong>Explore the docs »</strong></a>\n    <br />\n    <br />\n    <a href="https://github.com/SHAARPEC/shaarpec-python-client">View Demo</a>\n    ·\n    <a href="https://github.com/SHAARPEC/shaarpec-python-client/issues">Report Bug</a>\n    ·\n    <a href="https://github.com/SHAARPEC/shaarpec-python-client/issues">Request Feature</a>\n  </p>\n</div>\n\n\n\n<!-- TABLE OF CONTENTS -->\n<details>\n  <summary>Table of Contents</summary>\n  <ol>\n    <li>\n      <a href="#about-the-project">About The Project</a>\n      <ul>\n        <li><a href="#built-with">Built With</a></li>\n      </ul>\n    </li>\n    <li>\n      <a href="#getting-started">Getting Started</a>\n      <ul>\n        <li><a href="#prerequisites">Prerequisites</a></li>\n        <li><a href="#installation">Installation</a></li>\n      </ul>\n    </li>\n    <li><a href="#usage">Usage</a></li>\n    <li><a href="#roadmap">Roadmap</a></li>\n    <li><a href="#license">License</a></li>\n    <li><a href="#contact">Contact</a></li>\n  </ol>\n</details>\n\n\n\n<!-- ABOUT THE PROJECT -->\n## About The Project\n\n[![SHAARPEC API screenshot][product-screenshot]](https://www.shaarpec.com)\n\nThis is a Python client for simple access to the SHAARPEC Analytics API. Authentication is handled automatically via device flow, authorization code flow, or client credentials flow. Authentication can also be disabled if accessing a public Analytics API.\n\nThe SHAARPEC Analytics API provides calculations on the healthcare organization\'s resources, capacities, clinical outcomes, and much more. These results can be accessed via a standard REST API, which is usually protected by the SHAARPEC Identity Server.\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n### Built With\n\n* [![Httpx][Httpx]][Httpx]\n* [![Python][Python]][Python-url]\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n<!-- GETTING STARTED -->\n## Getting Started\n\n### Prerequisites\n\nThe shaarpec client is used as a standard Python library. It is always a good idea to install the library in a virtual environment.\n\n### Installation\n\n1. Install the library into your virtual environment.\n   ```bash\n   pip install shaarpec\n   ```\n2. Store your credentials to the SHAARPEC IdentityServer in an .env file.\n   ```bash\n   $ cat .env\n   OIDCISH_HOST="https://idp.example.com"\n   OIDCISH_CLIENT_ID="my client id"\n   OIDCISH_CLIENT_SECRET="my client secret"\n   OIDCISH_AUDIENCE="shaarpec_api.full_access_scope"\n   OIDCISH_SCOPE="openid shaarpec_api.full_access_scope offline_access"\n   ```\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n<!-- USAGE EXAMPLES -->\n## Usage\n\nThis library provides a Client class to easily interact with the SHAARPEC Analytics API. The class methods `Client.with_device(...)`,  `Client.with_code(...)`, and `Client.with_credentials(...)` create clients that authenticate with the SHAARPEC IdentityServer with either device flow (not tied to an individual user, recommended), code flow (tied to an individual user, for debugging and development), or credentials flow (non-interactive). There is also a class method `Client.without_auth(...)` that does not invoke the IDP server (but will only work if the Analytics API is public, otherwise give 401 Authentication invalid errors).\n\nAll API data is returned as `httpx.Response` objects.\n\nLet\'s look at some code examples on how to get data from the Analytics API. First, import the client.\n```python\nfrom shaarpec import Client\n```\n\nNext, use [device flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/device-authorization-flow) or [code flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/authorization-code-flow) to connect the client to the API with the `Client.with_device(...)`, `Client.with_code(...)`, and/or `Client.with_credentials(...)` class methods.\n\nThe credentials can either be stored in a .env file in the working directory (as explained in the Prerequisites section), provided as a path, or given directly as arguments to the `auth` dict.\n```python\n# Create a client with device flow, give authentication details directly.\nclient = Client.with_device(\n        host="https://api.shaarpec.com/",\n        auth={\n            "host": "https://idp.shaarpec.com",\n            "client_id": ...,\n            "client_secret": ...,\n            "scope": ...,\n            "audience": ...\n        }\n    )\n# Create a client with device flow, read authentication details from .env file.\nclient = Client.with_device(host="https://api.shaarpec.com/", auth="path/to/.env")\n```\nHere `host` is the base URL to the Analytics API and `auth` is a dictionary with the login credentials. With device flow, the user needs to finish the sign-in by visiting a url provided by the IdentityServer. A message will be shown:\n\n> Visit https://idp.shaarpec.com/device?userCode=XXXXXXXXX to complete sign-in.\n\nThe user visits the website, verifies that the user code is correct and confirms the sign-in. After a few seconds, the client will confirm the sign-in:\n\n> SUCCESS: Authentication was successful. Took XX.Y seconds.\n\nThe client is now connected to the API. Visit the Analytics API Base URL to interactively test the endpoints and read their documentation and about their path and query parameters. These parameters are used in the regular (`requests` and `httpx`) way with `client.verb` calls, where `verb` is either `get` or `post`. \n\n### GET and POST\n\nThe `get` and `post` verbs are supported in the standard way. For example (API responses are returned as `httpx.Response` objects):\n```python\nclient.get("terminology/allergy_type").json()\n```\nmight return\n```\n{\'419263009\': \'Allergy to tree pollen\',\n \'420174000\': \'Allergy to wheat\',\n \'425525006\': \'Allergy to dairy product\',\n \'714035009\': \'Allergy to soya\',\n \'419474003\': \'Allergy to mould\',\n \'232347008\': \'Dander (animal) allergy\',\n \'91934008\': \'Allergy to nut\',\n \'417532002\': \'Allergy to fish\',\n \'300913006\': \'Shellfish allergy\',\n \'232350006\': \'House dust mite allergy\',\n \'418689008\': \'Allergy to grass pollen\',\n \'91935009\': \'Allergy to peanuts\',\n \'91930004\': \'Allergy to eggs\',\n \'300916003\': \'Latex allergy\',\n \'424213003\': \'Allergy to bee venom\'}\n```\nor\n```python\nclient.get("population", conditions=["T78.2", "K81.0"])\n```\nmight return\n```\n[{\'patient_origin_id\': \'4c92f494-3c98-f8dd-1473-da9eb0196f6f\',\n    \'age\': \'10-16\',\n    \'is_alive\': True,\n    \'gender\': \'F\',\n    \'deceased_year\': 0},\n ...\n]\n```\n\n### Running tasks\n\nSHAARPEC Analytics API supports long-running tasks by `POST`:ing to `/service/path/to/endpoint`, and then polling with `GET` to `/service/tasks/{task_id}/status` until the result becomes available at `/service/tasks/{task_id}/results`. There is a `run` function in the library that performs this pattern.\n\nFor example\n\n```python\ntask = client.run("population/conditions")\n```\n\nwill return a task with the comorbidities in the entire population. A task is a [Pydantic](https://docs.pydantic.dev/) model with the following properties:\n\n```python\nclass Task(BaseModel):\n    """A running task."""\n    service: str\n    task_id: str\n    submitted_at: str\n    status: str\n    success: Optional[bool]\n    progress: Optional[float]\n    result: Optional[Any]\n    error: Optional[Any]\n    debugger: Optional[Any]\n```\nAs you can see, the success, progress, result and error are optional and updated automatically when available. The method comes with a progress bar which can be disabled via `client.run("path/to/task", progress_bar=False)`. If you want to use the task result in a subsequent command, you can wait (blocking) for the result with the `task.wait_for_result()` method:\n\n```python\ntask = client.run("path/to/task")\nprint(f"The result is: {task.wait_for_result()}!")\n```\n\n\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n<!-- ROADMAP -->\n## Roadmap\n\nSee the [open issues](https://github.com/SHAARPEC/shaarpec-python-client/issues) for a full list of proposed features (and known issues).\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n\n<!-- LICENSE -->\n## License\n\nDistributed under the MIT License. See `LICENSE` for more information.\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n\n<!-- CONTACT -->\n## Contact\n\nSHAARPEC Support - support@shaarpec.com\n\nProject Link: [https://github.com/SHAARPEC/shaarpec-python-client](https://github.com/SHAARPEC/shaarpec-python-client)\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n\n<!-- MARKDOWN LINKS & IMAGES -->\n<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->\n[contributors-shield]: https://img.shields.io/github/contributors/SHAARPEC/shaarpec-python-client.svg?style=for-the-badge\n[contributors-url]: https://github.com/SHAARPEC/shaarpec-python-client/graphs/contributors\n[forks-shield]: https://img.shields.io/github/forks/SHAARPEC/shaarpec-python-client.svg?style=for-the-badge\n[forks-url]: https://github.com/SHAARPEC/shaarpec-python-client/network/members\n[stars-shield]: https://img.shields.io/github/stars/SHAARPEC/shaarpec-python-client.svg?style=for-the-badge\n[stars-url]: https://github.com/SHAARPEC/shaarpec-python-client/stargazers\n[issues-shield]: https://img.shields.io/github/issues/SHAARPEC/shaarpec-python-client.svg?style=for-the-badge\n[issues-url]: https://github.com/SHAARPEC/shaarpec-python-client/issues\n[license-shield]: https://img.shields.io/github/license/SHAARPEC/shaarpec-python-client?style=for-the-badge\n[license-url]: https://github.com/SHAARPEC/shaarpec-python-client/blob/master/LICENSE\n[product-screenshot]: images/screenshot.png\n[Httpx]: images/httpx.svg\n[Httpx-url]: https://www.python-httpx.org/\n[Python]: images/python-3.8.svg\n[Python-url]: https://www.python.org/\n',
-    'author': 'Erik G. Brandt',
-    'author_email': 'erik.brandt@shaarpec.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+<!-- PROJECT LOGO -->
+<br />
+<div align="center">
+  <a href="https://github.com/SHAARPEC/shaarpec-python-client">
+    <img src="images/logo.png" alt="Logo" width="248" height="95">
+  </a>
 
+  <p align="center">
+    Python client for SHAARPEC Analytics API.
+    <br />
+    <a href="https://github.com/SHAARPEC/shaarpec-python-client"><strong>Explore the docs »</strong></a>
+    <br />
+    <br />
+    <a href="https://github.com/SHAARPEC/shaarpec-python-client">View Demo</a>
+    ·
+    <a href="https://github.com/SHAARPEC/shaarpec-python-client/issues">Report Bug</a>
+    ·
+    <a href="https://github.com/SHAARPEC/shaarpec-python-client/issues">Request Feature</a>
+  </p>
+</div>
+
+<!-- TABLE OF CONTENTS -->
+<details>
+  <summary>Table of Contents</summary>
+  <ol>
+    <li>
+      <a href="#about-the-project">About The Project</a>
+      <ul>
+        <li><a href="#built-with">Built With</a></li>
+      </ul>
+    </li>
+    <li>
+      <a href="#getting-started">Getting Started</a>
+      <ul>
+        <li><a href="#prerequisites">Prerequisites</a></li>
+        <li><a href="#installation">Installation</a></li>
+      </ul>
+    </li>
+    <li><a href="#usage">Usage</a></li>
+    <li><a href="#troubleshooting">Troubleshooting</a></li>
+    <li><a href="#roadmap">Roadmap</a></li>
+    <li><a href="#license">License</a></li>
+    <li><a href="#contact">Contact</a></li>
+  </ol>
+</details>
+
+<!-- ABOUT THE PROJECT -->
+
+## About The Project
+
+[![SHAARPEC API screenshot][product-screenshot]](https://www.shaarpec.com)
+
+This is a Python client for simple access to the SHAARPEC Analytics API. Authentication is handled automatically via device flow, authorization code flow, or client credentials flow. Authentication can also be disabled if accessing a public Analytics API.
+
+The SHAARPEC Analytics API provides calculations on the healthcare organization's resources, capacities, clinical outcomes, and much more. These results can be accessed via a standard REST API, which is usually protected by the SHAARPEC Identity Server.
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+### Built With
+
+-   [![Httpx][Httpx]][Httpx]
+-   [![Python][Python]][Python-url]
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- GETTING STARTED -->
+
+## Getting Started
+
+### Prerequisites
+
+The shaarpec client is used as a standard Python library. It is always a good idea to install the library in a virtual environment.
+
+### Installation
+
+1. Install the library into your virtual environment.
+    ```bash
+    pip install shaarpec
+    ```
+2. Store your credentials to the SHAARPEC IdentityServer in an .env file.
+    ```bash
+    $ cat .env
+    OIDCISH_HOST="https://idp.example.com"
+    OIDCISH_CLIENT_ID="my client id"
+    OIDCISH_CLIENT_SECRET="my client secret"
+    OIDCISH_AUDIENCE="shaarpec_api.full_access_scope"
+    OIDCISH_SCOPE="openid shaarpec_api.full_access_scope offline_access"
+    ```
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- USAGE EXAMPLES -->
+
+## Usage
+
+This library provides a Client class to easily interact with the SHAARPEC Analytics API. The class methods `Client.with_device(...)`, `Client.with_code(...)`, and `Client.with_credentials(...)` create clients that authenticate with the SHAARPEC IdentityServer with either device flow (not tied to an individual user, recommended), code flow (tied to an individual user, for debugging and development), or credentials flow (non-interactive). There is also a class method `Client.without_auth(...)` that does not invoke the IDP server (but will only work if the Analytics API is public, otherwise give 401 Authentication invalid errors).
+
+All API data is returned as `httpx.Response` objects.
+
+Let's look at some code examples on how to get data from the Analytics API. First, import the client.
+
+```python
+from shaarpec import Client
+```
+
+Next, use [device flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/device-authorization-flow) or [code flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/authorization-code-flow) to connect the client to the API with the `Client.with_device(...)`, `Client.with_code(...)`, and/or `Client.with_credentials(...)` class methods.
+
+The credentials can either be stored in a .env file in the working directory (as explained in the Prerequisites section), provided as a path, or given directly as arguments to the `auth` dict.
+
+```python
+# Create a client with device flow, give authentication details directly.
+client = Client.with_device(
+        host="https://api.shaarpec.com/",
+        auth={
+            "host": "https://idp.shaarpec.com",
+            "client_id": ...,
+            "client_secret": ...,
+            "scope": ...,
+            "audience": ...
+        }
+    )
+# Create a client with device flow, read authentication details from .env file.
+client = Client.with_device(host="https://api.shaarpec.com/", auth="path/to/.env")
+```
+
+Here `host` is the base URL to the Analytics API and `auth` is a dictionary with the login credentials. With device flow, the user needs to finish the sign-in by visiting a url provided by the IdentityServer. A message will be shown:
+
+> Visit https://idp.shaarpec.com/device?userCode=XXXXXXXXX to complete sign-in.
+
+The user visits the website, verifies that the user code is correct and confirms the sign-in. After a few seconds, the client will confirm the sign-in:
+
+> SUCCESS: Authentication was successful. Took XX.Y seconds.
+
+The client is now connected to the API. Visit the Analytics API Base URL to interactively test the endpoints and read their documentation and about their path and query parameters. These parameters are used in the regular (`requests` and `httpx`) way with `client.verb` calls, where `verb` is either `get` or `post`.
+
+### GET and POST
+
+The `get` and `post` verbs are supported in the standard way. For example (API responses are returned as `httpx.Response` objects):
+
+```python
+client.get("terminology/allergy_type").json()
+```
+
+might return
+
+```
+{'419263009': 'Allergy to tree pollen',
+ '420174000': 'Allergy to wheat',
+ '425525006': 'Allergy to dairy product',
+ '714035009': 'Allergy to soya',
+ '419474003': 'Allergy to mould',
+ '232347008': 'Dander (animal) allergy',
+ '91934008': 'Allergy to nut',
+ '417532002': 'Allergy to fish',
+ '300913006': 'Shellfish allergy',
+ '232350006': 'House dust mite allergy',
+ '418689008': 'Allergy to grass pollen',
+ '91935009': 'Allergy to peanuts',
+ '91930004': 'Allergy to eggs',
+ '300916003': 'Latex allergy',
+ '424213003': 'Allergy to bee venom'}
+```
+
+or
+
+```python
+client.get("population", conditions=["T78.2", "K81.0"])
+```
+
+might return
+
+```
+[{'patient_origin_id': '4c92f494-3c98-f8dd-1473-da9eb0196f6f',
+    'age': '10-16',
+    'is_alive': True,
+    'gender': 'F',
+    'deceased_year': 0},
+ ...
+]
+```
+
+### Running tasks
+
+SHAARPEC Analytics API supports long-running tasks by `POST`:ing to `/service/path/to/endpoint`, and then polling with `GET` to `/service/tasks/{task_id}/status` until the result becomes available at `/service/tasks/{task_id}/results`. There is a `run` function in the library that performs this pattern.
+
+For example
+
+```python
+task = client.run("population/conditions")
+```
+
+will return a task with the comorbidities in the entire population. A task is a [Pydantic](https://docs.pydantic.dev/) model with the following properties:
+
+```python
+class Task(BaseModel):
+    """A running task."""
+    service: str
+    task_id: str
+    submitted_at: str
+    status: str
+    success: Optional[bool]
+    progress: Optional[float]
+    result: Optional[Any]
+    error: Optional[Any]
+    debugger: Optional[Any]
+```
+
+As you can see, the success, progress, result and error are optional and updated automatically when available. The method comes with a progress bar which can be disabled via `client.run("path/to/task", progress_bar=False)`. If you want to use the task result in a subsequent command, you can wait (blocking) for the result with the `task.wait_for_result()` method:
+
+```python
+task = client.run("path/to/task")
+print(f"The result is: {task.wait_for_result()}!")
+```
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- TROUBLESHOOTING -->
+
+## Troubleshooting
+
+### Progress bar fails to render in (Dockerized) Jupyter Lab
+
+Sometimes (especially in a Dockerized environment) the progress bar fails to render when running a task. This seems to be related to an issue in `tqdm` and its dependencies. A workaround seems to be to run:
+
+```bash
+jupyter lab build
+```
+
+in the environment (in a terminal inside the running Docker container) and refresh the browser. This requires a `node.js` installation first, e.g. per:
+
+```
+conda install -c conda-forge nodejs
+```
+
+See discussion for [issue 1310](https://github.com/tqdm/tqdm/issues/1310)
+on the `tqdm` Github repo.
+
+<!-- ROADMAP -->
+
+## Roadmap
+
+See the [open issues](https://github.com/SHAARPEC/shaarpec-python-client/issues) for a full list of proposed features (and known issues).
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- LICENSE -->
+
+## License
+
+Distributed under the MIT License. See `LICENSE` for more information.
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- CONTACT -->
+
+## Contact
+
+SHAARPEC Support - support@shaarpec.com
+
+Project Link: [https://github.com/SHAARPEC/shaarpec-python-client](https://github.com/SHAARPEC/shaarpec-python-client)
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- MARKDOWN LINKS & IMAGES -->
+<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+
+[contributors-shield]: https://img.shields.io/github/contributors/SHAARPEC/shaarpec-python-client.svg?style=for-the-badge
+[contributors-url]: https://github.com/SHAARPEC/shaarpec-python-client/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/SHAARPEC/shaarpec-python-client.svg?style=for-the-badge
+[forks-url]: https://github.com/SHAARPEC/shaarpec-python-client/network/members
+[stars-shield]: https://img.shields.io/github/stars/SHAARPEC/shaarpec-python-client.svg?style=for-the-badge
+[stars-url]: https://github.com/SHAARPEC/shaarpec-python-client/stargazers
+[issues-shield]: https://img.shields.io/github/issues/SHAARPEC/shaarpec-python-client.svg?style=for-the-badge
+[issues-url]: https://github.com/SHAARPEC/shaarpec-python-client/issues
+[license-shield]: https://img.shields.io/github/license/SHAARPEC/shaarpec-python-client?style=for-the-badge
+[license-url]: https://github.com/SHAARPEC/shaarpec-python-client/blob/master/LICENSE
+[product-screenshot]: images/screenshot.png
+[Httpx]: images/httpx.svg
+[Httpx-url]: https://www.python-httpx.org/
+[Python]: images/python-3.8.svg
+[Python-url]: https://www.python.org/
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,174 +1,162 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['shaarpec']
-package_data = \ {'': ['*']} install_requires = \ ['Babel>=2.12.1,<3.0.0',
-'anybadge>=1.14.0,<2.0.0', 'anyio>=3.6.2,<4.0.0', 'argon2-cffi-
-bindings>=21.2.0,<22.0.0', 'argon2-cffi>=21.3.0,<22.0.0',
-'asttokens>=2.2.1,<3.0.0', 'attrs>=22.2.0,<23.0.0', 'backcall>=0.2.0,<0.3.0',
-'background>=0.2.1,<0.3.0', 'beautifulsoup4>=4.12.1,<5.0.0',
-'bleach>=6.0.0,<7.0.0', 'certifi>=2022.12.7,<2023.0.0', 'cffi>=1.15.1,<2.0.0',
-'charset-normalizer>=3.1.0,<4.0.0', 'click>=8.1.3,<9.0.0',
-'debugpy>=1.6.7,<2.0.0', 'decorator>=5.1.1,<6.0.0', 'defusedxml>=0.7.1,<0.8.0',
-'dill>=0.3.6,<0.4.0', 'ecdsa>=0.18.0,<0.19.0', 'entrypoints>=0.4,<0.5',
-'executing>=1.2.0,<2.0.0', 'fastjsonschema>=2.16.3,<3.0.0',
-'httpx>=0.23.3,<0.24.0', 'ipywidgets==7.6.5', 'jupyterlab-
-widgets>=3.0.7,<4.0.0', 'oidcish>=0.3.1,<0.4.0', 'pylint>=2.17.2,<3.0.0',
-'tqdm>=4.65.0,<5.0.0'] setup_kwargs = { 'name': 'shaarpec', 'version': '2.3.2',
-'description': 'Client for SHAARPEC Analytics API.', 'long_description':
-'\n\n\n[![Contributors][contributors-shield]][contributors-url]\n[![Forks]
-[forks-shield]][forks-url]\n[![Stargazers][stars-shield]][stars-url]\n[!
-[Issues][issues-shield]][issues-url]\n[![MIT License][license-shield]][license-
-url]\n\n\n\n
-\n
-                              \n \n_[Logo]\n\n\n
-                \n Python client for SHAARPEC Analytics API.\n
-                           \n Explore_the_docs_Â»\n
-                                      \n
-            \n View_Demo\n Â·\n Report_Bug\n Â·\n Request_Feature\n
-                                      \n
-\n\n\n\n\n\n Table of Contents\n
-   1. \n
-   2. \n About_The_Project\n
-          o \n
+Metadata-Version: 2.1 Name: shaarpec Version: 2.3.3 Summary: Client for
+SHAARPEC Analytics API. Author: Erik G. Brandt Author-email:
+erik.brandt@shaarpec.com Requires-Python: >=3.10,<4.0 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Babel
+(>=2.12.1,<3.0.0) Requires-Dist: anybadge (>=1.14.0,<2.0.0) Requires-Dist:
+anyio (>=3.6.2,<4.0.0) Requires-Dist: argon2-cffi (>=21.3.0,<22.0.0) Requires-
+Dist: argon2-cffi-bindings (>=21.2.0,<22.0.0) Requires-Dist: asttokens
+(>=2.2.1,<3.0.0) Requires-Dist: attrs (>=22.2.0,<23.0.0) Requires-Dist:
+backcall (>=0.2.0,<0.3.0) Requires-Dist: background (>=0.2.1,<0.3.0) Requires-
+Dist: beautifulsoup4 (>=4.12.1,<5.0.0) Requires-Dist: bleach (>=6.0.0,<7.0.0)
+Requires-Dist: certifi (>=2022.12.7,<2023.0.0) Requires-Dist: cffi
+(>=1.15.1,<2.0.0) Requires-Dist: charset-normalizer (>=3.1.0,<4.0.0) Requires-
+Dist: click (>=8.1.3,<9.0.0) Requires-Dist: debugpy (>=1.6.7,<2.0.0) Requires-
+Dist: decorator (>=5.1.1,<6.0.0) Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
+Requires-Dist: dill (>=0.3.6,<0.4.0) Requires-Dist: ecdsa (>=0.18.0,<0.19.0)
+Requires-Dist: entrypoints (>=0.4,<0.5) Requires-Dist: executing
+(>=1.2.0,<2.0.0) Requires-Dist: fastjsonschema (>=2.16.3,<3.0.0) Requires-Dist:
+httpx (>=0.23.3,<0.24.0) Requires-Dist: ipywidgets (>=8.0.6,<9.0.0) Requires-
+Dist: jupyterlab-widgets (>=3.0.7,<4.0.0) Requires-Dist: oidcish
+(>=0.3.1,<0.4.0) Requires-Dist: pylint (>=2.17.2,<3.0.0) Requires-Dist: tqdm
+(>=4.65.0,<5.0.0) Description-Content-Type: text/markdown   [![Contributors]
+[contributors-shield]][contributors-url] [![Forks][forks-shield]][forks-url] [!
+[Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]][issues-url]
+[![MIT License][license-shield]][license-url]
+                                    [Logo]
+                  Python client for SHAARPEC Analytics API.
+                             Explore_the_docs_Â»
+
+                  View_Demo Â· Report_Bug Â· Request_Feature
+  Table of Contents
+   1. About_The_Project
           o Built_With
-          o \n
-      \n
-   3. \n
-   4. \n Getting_Started\n
-          o \n
+   2. Getting_Started
           o Prerequisites
-          o \n
           o Installation
-          o \n
-      \n
-   5. \n
-   6. Usage
-   7. \n
-   8. Roadmap
-   9. \n
-  10. License
-  11. \n
-  12. Contact
-  13. \n
-\n\n\n\n\n\n## About The Project\n\n[![SHAARPEC API screenshot][product-
-screenshot]](https://www.shaarpec.com)\n\nThis is a Python client for simple
-access to the SHAARPEC Analytics API. Authentication is handled automatically
-via device flow, authorization code flow, or client credentials flow.
-Authentication can also be disabled if accessing a public Analytics API.\n\nThe
-SHAARPEC Analytics API provides calculations on the healthcare organization\'s
-resources, capacities, clinical outcomes, and much more. These results can be
-accessed via a standard REST API, which is usually protected by the SHAARPEC
-Identity Server.\n\n
-                                                                  (back_to_top)
-\n\n### Built With\n\n* [![Httpx][Httpx]][Httpx]\n* [![Python][Python]][Python-
-url]\n\n
-                                                                  (back_to_top)
-\n\n\n## Getting Started\n\n### Prerequisites\n\nThe shaarpec client is used as
-a standard Python library. It is always a good idea to install the library in a
-virtual environment.\n\n### Installation\n\n1. Install the library into your
-virtual environment.\n ```bash\n pip install shaarpec\n ```\n2. Store your
-credentials to the SHAARPEC IdentityServer in an .env file.\n ```bash\n $ cat
-.env\n OIDCISH_HOST="https://idp.example.com"\n OIDCISH_CLIENT_ID="my client
-id"\n OIDCISH_CLIENT_SECRET="my client secret"\n
-OIDCISH_AUDIENCE="shaarpec_api.full_access_scope"\n OIDCISH_SCOPE="openid
-shaarpec_api.full_access_scope offline_access"\n ```\n\n
+   3. Usage
+   4. Troubleshooting
+   5. Roadmap
+   6. License
+   7. Contact
+  ## About The Project [![SHAARPEC API screenshot][product-screenshot]](https:/
+/www.shaarpec.com) This is a Python client for simple access to the SHAARPEC
+Analytics API. Authentication is handled automatically via device flow,
+authorization code flow, or client credentials flow. Authentication can also be
+disabled if accessing a public Analytics API. The SHAARPEC Analytics API
+provides calculations on the healthcare organization's resources, capacities,
+clinical outcomes, and much more. These results can be accessed via a standard
+REST API, which is usually protected by the SHAARPEC Identity Server.
+                                                                  (back_to_top)
+### Built With - [![Httpx][Httpx]][Httpx] - [![Python][Python]][Python-url]
+                                                                  (back_to_top)
+ ## Getting Started ### Prerequisites The shaarpec client is used as a standard
+Python library. It is always a good idea to install the library in a virtual
+environment. ### Installation 1. Install the library into your virtual
+environment. ```bash pip install shaarpec ``` 2. Store your credentials to the
+SHAARPEC IdentityServer in an .env file. ```bash $ cat .env
+OIDCISH_HOST="https://idp.example.com" OIDCISH_CLIENT_ID="my client id"
+OIDCISH_CLIENT_SECRET="my client secret"
+OIDCISH_AUDIENCE="shaarpec_api.full_access_scope" OIDCISH_SCOPE="openid
+shaarpec_api.full_access_scope offline_access" ```
                                                                   (back_to_top)
-\n\n\n## Usage\n\nThis library provides a Client class to easily interact with
-the SHAARPEC Analytics API. The class methods `Client.with_device(...)`,
+ ## Usage This library provides a Client class to easily interact with the
+SHAARPEC Analytics API. The class methods `Client.with_device(...)`,
 `Client.with_code(...)`, and `Client.with_credentials(...)` create clients that
 authenticate with the SHAARPEC IdentityServer with either device flow (not tied
 to an individual user, recommended), code flow (tied to an individual user, for
 debugging and development), or credentials flow (non-interactive). There is
 also a class method `Client.without_auth(...)` that does not invoke the IDP
 server (but will only work if the Analytics API is public, otherwise give 401
-Authentication invalid errors).\n\nAll API data is returned as `httpx.Response`
-objects.\n\nLet\'s look at some code examples on how to get data from the
-Analytics API. First, import the client.\n```python\nfrom shaarpec import
-Client\n```\n\nNext, use [device flow](https://auth0.com/docs/get-started/
-authentication-and-authorization-flow/device-authorization-flow) or [code flow]
-(https://auth0.com/docs/get-started/authentication-and-authorization-flow/
-authorization-code-flow) to connect the client to the API with the
-`Client.with_device(...)`, `Client.with_code(...)`, and/or
-`Client.with_credentials(...)` class methods.\n\nThe credentials can either be
-stored in a .env file in the working directory (as explained in the
-Prerequisites section), provided as a path, or given directly as arguments to
-the `auth` dict.\n```python\n# Create a client with device flow, give
-authentication details directly.\nclient = Client.with_device(\n host="https://
-api.shaarpec.com/",\n auth={\n "host": "https://idp.shaarpec.com",\n
-"client_id": ...,\n "client_secret": ...,\n "scope": ...,\n "audience": ...\n
-}\n )\n# Create a client with device flow, read authentication details from
-.env file.\nclient = Client.with_device(host="https://api.shaarpec.com/",
-auth="path/to/.env")\n```\nHere `host` is the base URL to the Analytics API and
-`auth` is a dictionary with the login credentials. With device flow, the user
-needs to finish the sign-in by visiting a url provided by the IdentityServer. A
-message will be shown:\n\n> Visit https://idp.shaarpec.com/
-device?userCode=XXXXXXXXX to complete sign-in.\n\nThe user visits the website,
-verifies that the user code is correct and confirms the sign-in. After a few
-seconds, the client will confirm the sign-in:\n\n> SUCCESS: Authentication was
-successful. Took XX.Y seconds.\n\nThe client is now connected to the API. Visit
-the Analytics API Base URL to interactively test the endpoints and read their
-documentation and about their path and query parameters. These parameters are
-used in the regular (`requests` and `httpx`) way with `client.verb` calls,
-where `verb` is either `get` or `post`. \n\n### GET and POST\n\nThe `get` and
-`post` verbs are supported in the standard way. For example (API responses are
-returned as `httpx.Response` objects):\n```python\nclient.get("terminology/
-allergy_type").json()\n```\nmight return\n```\n{\'419263009\': \'Allergy to
-tree pollen\',\n \'420174000\': \'Allergy to wheat\',\n \'425525006\':
-\'Allergy to dairy product\',\n \'714035009\': \'Allergy to soya\',\n
-\'419474003\': \'Allergy to mould\',\n \'232347008\': \'Dander (animal)
-allergy\',\n \'91934008\': \'Allergy to nut\',\n \'417532002\': \'Allergy to
-fish\',\n \'300913006\': \'Shellfish allergy\',\n \'232350006\': \'House dust
-mite allergy\',\n \'418689008\': \'Allergy to grass pollen\',\n \'91935009\':
-\'Allergy to peanuts\',\n \'91930004\': \'Allergy to eggs\',\n \'300916003\':
-\'Latex allergy\',\n \'424213003\': \'Allergy to bee
-venom\'}\n```\nor\n```python\nclient.get("population", conditions=["T78.2",
-"K81.0"])\n```\nmight return\n```\n[{\'patient_origin_id\': \'4c92f494-3c98-
-f8dd-1473-da9eb0196f6f\',\n \'age\': \'10-16\',\n \'is_alive\': True,\n
-\'gender\': \'F\',\n \'deceased_year\': 0},\n ...\n]\n```\n\n### Running
-tasks\n\nSHAARPEC Analytics API supports long-running tasks by `POST`:ing to `/
-service/path/to/endpoint`, and then polling with `GET` to `/service/tasks/
-{task_id}/status` until the result becomes available at `/service/tasks/
-{task_id}/results`. There is a `run` function in the library that performs this
-pattern.\n\nFor example\n\n```python\ntask = client.run("population/
-conditions")\n```\n\nwill return a task with the comorbidities in the entire
-population. A task is a [Pydantic](https://docs.pydantic.dev/) model with the
-following properties:\n\n```python\nclass Task(BaseModel):\n """A running
-task."""\n service: str\n task_id: str\n submitted_at: str\n status: str\n
-success: Optional[bool]\n progress: Optional[float]\n result: Optional[Any]\n
-error: Optional[Any]\n debugger: Optional[Any]\n```\nAs you can see, the
+Authentication invalid errors). All API data is returned as `httpx.Response`
+objects. Let's look at some code examples on how to get data from the Analytics
+API. First, import the client. ```python from shaarpec import Client ``` Next,
+use [device flow](https://auth0.com/docs/get-started/authentication-and-
+authorization-flow/device-authorization-flow) or [code flow](https://auth0.com/
+docs/get-started/authentication-and-authorization-flow/authorization-code-flow)
+to connect the client to the API with the `Client.with_device(...)`,
+`Client.with_code(...)`, and/or `Client.with_credentials(...)` class methods.
+The credentials can either be stored in a .env file in the working directory
+(as explained in the Prerequisites section), provided as a path, or given
+directly as arguments to the `auth` dict. ```python # Create a client with
+device flow, give authentication details directly. client = Client.with_device
+( host="https://api.shaarpec.com/", auth={ "host": "https://idp.shaarpec.com",
+"client_id": ..., "client_secret": ..., "scope": ..., "audience": ... } ) #
+Create a client with device flow, read authentication details from .env file.
+client = Client.with_device(host="https://api.shaarpec.com/", auth="path/
+to/.env") ``` Here `host` is the base URL to the Analytics API and `auth` is a
+dictionary with the login credentials. With device flow, the user needs to
+finish the sign-in by visiting a url provided by the IdentityServer. A message
+will be shown: > Visit https://idp.shaarpec.com/device?userCode=XXXXXXXXX to
+complete sign-in. The user visits the website, verifies that the user code is
+correct and confirms the sign-in. After a few seconds, the client will confirm
+the sign-in: > SUCCESS: Authentication was successful. Took XX.Y seconds. The
+client is now connected to the API. Visit the Analytics API Base URL to
+interactively test the endpoints and read their documentation and about their
+path and query parameters. These parameters are used in the regular (`requests`
+and `httpx`) way with `client.verb` calls, where `verb` is either `get` or
+`post`. ### GET and POST The `get` and `post` verbs are supported in the
+standard way. For example (API responses are returned as `httpx.Response`
+objects): ```python client.get("terminology/allergy_type").json() ``` might
+return ``` {'419263009': 'Allergy to tree pollen', '420174000': 'Allergy to
+wheat', '425525006': 'Allergy to dairy product', '714035009': 'Allergy to
+soya', '419474003': 'Allergy to mould', '232347008': 'Dander (animal) allergy',
+'91934008': 'Allergy to nut', '417532002': 'Allergy to fish', '300913006':
+'Shellfish allergy', '232350006': 'House dust mite allergy', '418689008':
+'Allergy to grass pollen', '91935009': 'Allergy to peanuts', '91930004':
+'Allergy to eggs', '300916003': 'Latex allergy', '424213003': 'Allergy to bee
+venom'} ``` or ```python client.get("population", conditions=["T78.2",
+"K81.0"]) ``` might return ``` [{'patient_origin_id': '4c92f494-3c98-f8dd-1473-
+da9eb0196f6f', 'age': '10-16', 'is_alive': True, 'gender': 'F',
+'deceased_year': 0}, ... ] ``` ### Running tasks SHAARPEC Analytics API
+supports long-running tasks by `POST`:ing to `/service/path/to/endpoint`, and
+then polling with `GET` to `/service/tasks/{task_id}/status` until the result
+becomes available at `/service/tasks/{task_id}/results`. There is a `run`
+function in the library that performs this pattern. For example ```python task
+= client.run("population/conditions") ``` will return a task with the
+comorbidities in the entire population. A task is a [Pydantic](https://
+docs.pydantic.dev/) model with the following properties: ```python class Task
+(BaseModel): """A running task.""" service: str task_id: str submitted_at: str
+status: str success: Optional[bool] progress: Optional[float] result: Optional
+[Any] error: Optional[Any] debugger: Optional[Any] ``` As you can see, the
 success, progress, result and error are optional and updated automatically when
 available. The method comes with a progress bar which can be disabled via
 `client.run("path/to/task", progress_bar=False)`. If you want to use the task
 result in a subsequent command, you can wait (blocking) for the result with the
-`task.wait_for_result()` method:\n\n```python\ntask = client.run("path/to/
-task")\nprint(f"The result is: {task.wait_for_result()}!")\n```\n\n\n\n
+`task.wait_for_result()` method: ```python task = client.run("path/to/task")
+print(f"The result is: {task.wait_for_result()}!") ```
                                                                   (back_to_top)
-\n\n\n## Roadmap\n\nSee the [open issues](https://github.com/SHAARPEC/shaarpec-
-python-client/issues) for a full list of proposed features (and known
-issues).\n\n
-                                                                  (back_to_top)
-\n\n\n\n## License\n\nDistributed under the MIT License. See `LICENSE` for more
-information.\n\n
-                                                                  (back_to_top)
-\n\n\n\n## Contact\n\nSHAARPEC Support - support@shaarpec.com\n\nProject Link:
-[https://github.com/SHAARPEC/shaarpec-python-client](https://github.com/
-SHAARPEC/shaarpec-python-client)\n\n
-                                                                  (back_to_top)
-\n\n\n\n\n[contributors-shield]: https://img.shields.io/github/contributors/
-SHAARPEC/shaarpec-python-client.svg?style=for-the-badge\n[contributors-url]:
-https://github.com/SHAARPEC/shaarpec-python-client/graphs/contributors\n[forks-
-shield]: https://img.shields.io/github/forks/SHAARPEC/shaarpec-python-
-client.svg?style=for-the-badge\n[forks-url]: https://github.com/SHAARPEC/
-shaarpec-python-client/network/members\n[stars-shield]: https://img.shields.io/
-github/stars/SHAARPEC/shaarpec-python-client.svg?style=for-the-badge\n[stars-
-url]: https://github.com/SHAARPEC/shaarpec-python-client/stargazers\n[issues-
+ ## Troubleshooting ### Progress bar fails to render in (Dockerized) Jupyter
+Lab Sometimes (especially in a Dockerized environment) the progress bar fails
+to render when running a task. This seems to be related to an issue in `tqdm`
+and its dependencies. A workaround seems to be to run: ```bash jupyter lab
+build ``` in the environment (in a terminal inside the running Docker
+container) and refresh the browser. This requires a `node.js` installation
+first, e.g. per: ``` conda install -c conda-forge nodejs ``` See discussion for
+[issue 1310](https://github.com/tqdm/tqdm/issues/1310) on the `tqdm` Github
+repo.  ## Roadmap See the [open issues](https://github.com/SHAARPEC/shaarpec-
+python-client/issues) for a full list of proposed features (and known issues).
+                                                                  (back_to_top)
+ ## License Distributed under the MIT License. See `LICENSE` for more
+information.
+                                                                  (back_to_top)
+ ## Contact SHAARPEC Support - support@shaarpec.com Project Link: [https://
+github.com/SHAARPEC/shaarpec-python-client](https://github.com/SHAARPEC/
+shaarpec-python-client)
+                                                                  (back_to_top)
+  [contributors-shield]: https://img.shields.io/github/contributors/SHAARPEC/
+shaarpec-python-client.svg?style=for-the-badge [contributors-url]: https://
+github.com/SHAARPEC/shaarpec-python-client/graphs/contributors [forks-shield]:
+https://img.shields.io/github/forks/SHAARPEC/shaarpec-python-
+client.svg?style=for-the-badge [forks-url]: https://github.com/SHAARPEC/
+shaarpec-python-client/network/members [stars-shield]: https://img.shields.io/
+github/stars/SHAARPEC/shaarpec-python-client.svg?style=for-the-badge [stars-
+url]: https://github.com/SHAARPEC/shaarpec-python-client/stargazers [issues-
 shield]: https://img.shields.io/github/issues/SHAARPEC/shaarpec-python-
-client.svg?style=for-the-badge\n[issues-url]: https://github.com/SHAARPEC/
-shaarpec-python-client/issues\n[license-shield]: https://img.shields.io/github/
-license/SHAARPEC/shaarpec-python-client?style=for-the-badge\n[license-url]:
-https://github.com/SHAARPEC/shaarpec-python-client/blob/master/LICENSE\n
-[product-screenshot]: images/screenshot.png\n[Httpx]: images/httpx.svg\n[Httpx-
-url]: https://www.python-httpx.org/\n[Python]: images/python-3.8.svg\n[Python-
-url]: https://www.python.org/\n', 'author': 'Erik G. Brandt', 'author_email':
-'erik.brandt@shaarpec.com', 'maintainer': 'None', 'maintainer_email': 'None',
-'url': 'None', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.10,<4.0', } setup
-(**setup_kwargs)
+client.svg?style=for-the-badge [issues-url]: https://github.com/SHAARPEC/
+shaarpec-python-client/issues [license-shield]: https://img.shields.io/github/
+license/SHAARPEC/shaarpec-python-client?style=for-the-badge [license-url]:
+https://github.com/SHAARPEC/shaarpec-python-client/blob/master/LICENSE
+[product-screenshot]: images/screenshot.png [Httpx]: images/httpx.svg [Httpx-
+url]: https://www.python-httpx.org/ [Python]: images/python-3.8.svg [Python-
+url]: https://www.python.org/
```

