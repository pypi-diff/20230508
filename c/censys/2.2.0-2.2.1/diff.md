# Comparing `tmp/censys-2.2.0.tar.gz` & `tmp/censys-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censys-2.2.0.tar", max compression
+gzip compressed data, was "censys-2.2.1.tar", max compression
```

## Comparing `censys-2.2.0.tar` & `censys-2.2.1.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0    10174 2023-04-27 15:38:12.948205 censys-2.2.0/LICENSE
--rw-r--r--   0        0        0     3893 2023-04-27 15:38:12.948205 censys-2.2.0/README.md
--rw-r--r--   0        0        0       91 2023-04-27 15:38:12.948205 censys-2.2.0/censys/__main__.py
--rw-r--r--   0        0        0      633 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/__init__.py
--rw-r--r--   0        0        0     3474 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/api.py
--rw-r--r--   0        0        0      410 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/assets/__init__.py
--rw-r--r--   0        0        0     5900 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/assets/assets.py
--rw-r--r--   0        0        0      424 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/assets/certificates.py
--rw-r--r--   0        0        0     1118 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/assets/domains.py
--rw-r--r--   0        0        0      389 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/assets/hosts.py
--rw-r--r--   0        0        0     2075 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/assets/subdomains.py
--rw-r--r--   0        0        0     1775 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/assets/web_entities.py
--rw-r--r--   0        0        0     1598 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/client.py
--rw-r--r--   0        0        0     2380 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/clouds.py
--rw-r--r--   0        0        0     2519 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/events.py
--rw-r--r--   0        0        0     2482 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/inventory.py
--rw-r--r--   0        0        0     3981 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/risks.py
--rw-r--r--   0        0        0     2784 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/seeds.py
--rw-r--r--   0        0        0      569 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/__init__.py
--rw-r--r--   0        0        0     1901 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/args.py
--rw-r--r--   0        0        0      174 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/commands/__init__.py
--rw-r--r--   0        0        0     2045 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/commands/account.py
--rw-r--r--   0        0        0     6793 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/commands/asm.py
--rw-r--r--   0        0        0     3171 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/commands/config.py
--rw-r--r--   0        0        0     5526 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/commands/hnri.py
--rw-r--r--   0        0        0     5356 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/commands/search.py
--rw-r--r--   0        0        0     3439 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/commands/subdomains.py
--rw-r--r--   0        0        0     3760 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/commands/view.py
--rw-r--r--   0        0        0     3279 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/utils.py
--rw-r--r--   0        0        0      105 2023-04-27 15:38:12.948205 censys-2.2.0/censys/common/__init__.py
--rw-r--r--   0        0        0     7435 2023-04-27 15:38:12.948205 censys-2.2.0/censys/common/base.py
--rw-r--r--   0        0        0     1690 2023-04-27 15:38:12.948205 censys-2.2.0/censys/common/config.py
--rw-r--r--   0        0        0     1106 2023-04-27 15:38:12.948205 censys-2.2.0/censys/common/deprecation.py
--rw-r--r--   0        0        0    12264 2023-04-27 15:38:12.948205 censys-2.2.0/censys/common/exceptions.py
--rw-r--r--   0        0        0      144 2023-04-27 15:38:12.948205 censys-2.2.0/censys/common/types.py
--rw-r--r--   0        0        0      453 2023-04-27 15:38:12.948205 censys-2.2.0/censys/common/utils.py
--rw-r--r--   0        0        0      242 2023-04-27 15:38:12.948205 censys-2.2.0/censys/common/version.py
--rw-r--r--   0        0        0        0 2023-04-27 15:38:12.948205 censys-2.2.0/censys/py.typed
--rw-r--r--   0        0        0      375 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/__init__.py
--rw-r--r--   0        0        0     2133 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/client.py
--rw-r--r--   0        0        0      169 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/v1/__init__.py
--rw-r--r--   0        0        0     5805 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/v1/api.py
--rw-r--r--   0        0        0     1830 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/v1/certificates.py
--rw-r--r--   0        0        0     1224 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/v1/data.py
--rw-r--r--   0        0        0      151 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/v2/__init__.py
--rw-r--r--   0        0        0    17201 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/v2/api.py
--rw-r--r--   0        0        0    12750 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/v2/certs.py
--rw-r--r--   0        0        0    10570 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/v2/hosts.py
--rw-r--r--   0        0        0     3298 2023-04-27 15:38:12.952205 censys-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     6412 1970-01-01 00:00:00.000000 censys-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-05-08 20:59:03.417712 censys-2.2.1/LICENSE
+-rw-r--r--   0        0        0     4466 2023-05-08 20:59:03.417712 censys-2.2.1/README.md
+-rw-r--r--   0        0        0       91 2023-05-08 20:59:03.417712 censys-2.2.1/censys/__main__.py
+-rw-r--r--   0        0        0      633 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/__init__.py
+-rw-r--r--   0        0        0     3474 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/api.py
+-rw-r--r--   0        0        0      410 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/assets/__init__.py
+-rw-r--r--   0        0        0     5900 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/assets/assets.py
+-rw-r--r--   0        0        0      424 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/assets/certificates.py
+-rw-r--r--   0        0        0     1118 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/assets/domains.py
+-rw-r--r--   0        0        0      389 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/assets/hosts.py
+-rw-r--r--   0        0        0     2075 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/assets/subdomains.py
+-rw-r--r--   0        0        0     1775 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/assets/web_entities.py
+-rw-r--r--   0        0        0     1598 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/client.py
+-rw-r--r--   0        0        0     2380 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/clouds.py
+-rw-r--r--   0        0        0     2519 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/events.py
+-rw-r--r--   0        0        0     2482 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/inventory.py
+-rw-r--r--   0        0        0     3981 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/risks.py
+-rw-r--r--   0        0        0     2784 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/seeds.py
+-rw-r--r--   0        0        0      675 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/__init__.py
+-rw-r--r--   0        0        0     1901 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/args.py
+-rw-r--r--   0        0        0      174 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2045 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/commands/account.py
+-rw-r--r--   0        0        0     6793 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/commands/asm.py
+-rw-r--r--   0        0        0     3171 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/commands/config.py
+-rw-r--r--   0        0        0     5526 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/commands/hnri.py
+-rw-r--r--   0        0        0     6603 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/commands/search.py
+-rw-r--r--   0        0        0     3492 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/commands/subdomains.py
+-rw-r--r--   0        0        0     3760 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/commands/view.py
+-rw-r--r--   0        0        0   233252 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/data/certificates_autocomplete.json
+-rw-r--r--   0        0        0   324545 2023-05-08 20:59:03.421712 censys-2.2.1/censys/cli/data/hosts_autocomplete.json
+-rw-r--r--   0        0        0     3279 2023-05-08 20:59:03.421712 censys-2.2.1/censys/cli/utils.py
+-rw-r--r--   0        0        0      105 2023-05-08 20:59:03.421712 censys-2.2.1/censys/common/__init__.py
+-rw-r--r--   0        0        0     8552 2023-05-08 20:59:03.421712 censys-2.2.1/censys/common/base.py
+-rw-r--r--   0        0        0     1690 2023-05-08 20:59:03.421712 censys-2.2.1/censys/common/config.py
+-rw-r--r--   0        0        0     1106 2023-05-08 20:59:03.421712 censys-2.2.1/censys/common/deprecation.py
+-rw-r--r--   0        0        0    12446 2023-05-08 20:59:03.421712 censys-2.2.1/censys/common/exceptions.py
+-rw-r--r--   0        0        0      144 2023-05-08 20:59:03.421712 censys-2.2.1/censys/common/types.py
+-rw-r--r--   0        0        0      453 2023-05-08 20:59:03.421712 censys-2.2.1/censys/common/utils.py
+-rw-r--r--   0        0        0      242 2023-05-08 20:59:03.421712 censys-2.2.1/censys/common/version.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:59:03.421712 censys-2.2.1/censys/py.typed
+-rw-r--r--   0        0        0      375 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/__init__.py
+-rw-r--r--   0        0        0     2133 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/client.py
+-rw-r--r--   0        0        0      169 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/v1/__init__.py
+-rw-r--r--   0        0        0     5805 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/v1/api.py
+-rw-r--r--   0        0        0     1830 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/v1/certificates.py
+-rw-r--r--   0        0        0     1224 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/v1/data.py
+-rw-r--r--   0        0        0      151 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/v2/__init__.py
+-rw-r--r--   0        0        0    17200 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/v2/api.py
+-rw-r--r--   0        0        0    12823 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/v2/certs.py
+-rw-r--r--   0        0        0    10570 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/v2/hosts.py
+-rw-r--r--   0        0        0     3365 2023-05-08 20:59:03.425712 censys-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7080 1970-01-01 00:00:00.000000 censys-2.2.1/PKG-INFO
```

### Comparing `censys-2.2.0/LICENSE` & `censys-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/README.md` & `censys-2.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 [![PyPI](https://img.shields.io/pypi/v/censys?color=orange&logo=pypi&logoColor=orange)](https://pypi.org/project/censys/)
 [![Python Version](https://img.shields.io/badge/python-3.7.2%2B-blue?logo=python)](https://www.python.org/downloads/)
 [![Read the Docs (version)](https://img.shields.io/readthedocs/censys-python/latest?logo=read%20the%20docs)](https://censys-python.readthedocs.io/en/stable/?badge=stable)
 [![GitHub Discussions](https://img.shields.io/badge/GitHub-Discussions-brightgreen?logo=github)](https://github.com/censys/censys-python/discussions)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-organge.svg?logo=git&logoColor=organge)](http://makeapullrequest.com)
 [![License](https://img.shields.io/github/license/censys/censys-python?logo=apache)](https://github.com/censys/censys-python/blob/main/LICENSE)
 
-An easy-to-use and lightweight API wrapper for Censys APIs ([censys.io](https://censys.io/)). Python 3.7.2+ is currently supported.
+An easy-to-use and lightweight API wrapper for Censys APIs ([censys.io](https://censys.io/)). Python 3.7.2+ is currently supported. This library has been tested on Python 3.7 and 3.x (Currently version 3.11).
 
 > **Notice:** The Censys Search v1 endpoints are deprecated as of Nov. 30, 2021. Please begin using v2 endpoints to query hosts and certificates and check out our [support center](https://support.censys.io/hc/en-us/sections/360013076551-Censys-Search-2-0) for resources.
 
 ## Features
 
 - [Search Censys data](https://censys-python.readthedocs.io/en/stable/usage-v2.html)
 - [Bulk Certificate lookups](https://censys-python.readthedocs.io/en/stable/usage-v1.html#bulk)
 - [Download Bulk Data](https://censys-python.readthedocs.io/en/stable/usage-v1.html#data)
 - [Manage assets, events, and seeds in Censys ASM](https://censys-python.readthedocs.io/en/stable/usage-asm.html)
 - [Command-line interface](https://censys-python.readthedocs.io/en/stable/cli.html)
 
+<!-- markdownlint-disable MD033 -->
 <a href="https://asciinema.org/a/500416" target="_blank"><img src="https://asciinema.org/a/500416.svg" width="600"/></a>
+<!-- markdownlint-enable MD033 -->
 
 ## Getting Started
 
 The library can be installed using `pip`.
 
 ```sh
 pip install censys
@@ -31,14 +33,30 @@
 
 To upgraded using `pip`.
 
 ```sh
 pip install --upgrade censys
 ```
 
+Or, you can install the library from source using `poetry`.
+
+```sh
+git clone https://github.com/censys/censys-python.git
+cd censys-python/
+poetry install
+```
+
+Optionally, you can enable tab completion for the CLI by adding this line to your `~/.bashrc`, `~/.zshrc`, or equivalent.
+
+> Please note that autocomplete is supported for field names in the `search` command.
+
+```sh
+eval "$(register-python-argcomplete censys)"
+```
+
 To configure your search credentials run `censys config` or set both `CENSYS_API_ID` and `CENSYS_API_SECRET` environment variables.
 
 ```sh
 $ censys config
 
 Censys API ID: XXX
 Censys API Secret: XXX
```

#### html2text {}

```diff
@@ -7,37 +7,43 @@
 ?badge=stable) [![GitHub Discussions](https://img.shields.io/badge/GitHub-
 Discussions-brightgreen?logo=github)](https://github.com/censys/censys-python/
 discussions) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-
 organge.svg?logo=git&logoColor=organge)](http://makeapullrequest.com) [!
 [License](https://img.shields.io/github/license/censys/censys-
 python?logo=apache)](https://github.com/censys/censys-python/blob/main/LICENSE)
 An easy-to-use and lightweight API wrapper for Censys APIs ([censys.io](https:/
-/censys.io/)). Python 3.7.2+ is currently supported. > **Notice:** The Censys
+/censys.io/)). Python 3.7.2+ is currently supported. This library has been
+tested on Python 3.7 and 3.x (Currently version 3.11). > **Notice:** The Censys
 Search v1 endpoints are deprecated as of Nov. 30, 2021. Please begin using v2
 endpoints to query hosts and certificates and check out our [support center]
 (https://support.censys.io/hc/en-us/sections/360013076551-Censys-Search-2-0)
 for resources. ## Features - [Search Censys data](https://censys-
 python.readthedocs.io/en/stable/usage-v2.html) - [Bulk Certificate lookups]
 (https://censys-python.readthedocs.io/en/stable/usage-v1.html#bulk) - [Download
 Bulk Data](https://censys-python.readthedocs.io/en/stable/usage-v1.html#data) -
 [Manage assets, events, and seeds in Censys ASM](https://censys-
 python.readthedocs.io/en/stable/usage-asm.html) - [Command-line interface]
-(https://censys-python.readthedocs.io/en/stable/cli.html) [https://
-asciinema.org/a/500416.svg] ## Getting Started The library can be installed
+(https://censys-python.readthedocs.io/en/stable/cli.html)  [https://
+asciinema.org/a/500416.svg]  ## Getting Started The library can be installed
 using `pip`. ```sh pip install censys ``` To upgraded using `pip`. ```sh pip
-install --upgrade censys ``` To configure your search credentials run `censys
-config` or set both `CENSYS_API_ID` and `CENSYS_API_SECRET` environment
-variables. ```sh $ censys config Censys API ID: XXX Censys API Secret: XXX Do
-you want color output? [y/n]: y Successfully authenticated for your@email.com
-``` To configure your ASM credentials run `censys asm config` or set the
-`CENSYS_ASM_API_KEY` environment variables. ```sh $ censys asm config Censys
-ASM API Key: XXX Do you want color output? [y/n]: y Successfully authenticated
-``` ## API Reference and User Guide available on [Read the Docs](https://
-censys-python.readthedocs.io/) [![Read the Docs](https://
-raw.githubusercontent.com/censys/censys-python/main/docs/_static/
+install --upgrade censys ``` Or, you can install the library from source using
+`poetry`. ```sh git clone https://github.com/censys/censys-python.git cd
+censys-python/ poetry install ``` Optionally, you can enable tab completion for
+the CLI by adding this line to your `~/.bashrc`, `~/.zshrc`, or equivalent. >
+Please note that autocomplete is supported for field names in the `search`
+command. ```sh eval "$(register-python-argcomplete censys)" ``` To configure
+your search credentials run `censys config` or set both `CENSYS_API_ID` and
+`CENSYS_API_SECRET` environment variables. ```sh $ censys config Censys API ID:
+XXX Censys API Secret: XXX Do you want color output? [y/n]: y Successfully
+authenticated for your@email.com ``` To configure your ASM credentials run
+`censys asm config` or set the `CENSYS_ASM_API_KEY` environment variables.
+```sh $ censys asm config Censys ASM API Key: XXX Do you want color output? [y/
+n]: y Successfully authenticated ``` ## API Reference and User Guide available
+on [Read the Docs](https://censys-python.readthedocs.io/) [![Read the Docs]
+(https://raw.githubusercontent.com/censys/censys-python/main/docs/_static/
 readthedocs.png)](https://censys-python.readthedocs.io/) ## Resources -
 [Source](https://github.com/censys/censys-python) - [Issue Tracker](https://
 github.com/censys/censys-python/issues) - [Changelog](https://github.com/
 censys/censys-python/releases) - [Documentation](https://censys-python.rtfd.io)
 - [Discussions](https://github.com/censys/censys-python/discussions) - [Censys
 Homepage](https://censys.io/) - [Censys Search](https://search.censys.io/) ##
 Contributing All contributions (no matter how small) are always welcome. See
```

### Comparing `censys-2.2.0/censys/asm/__init__.py` & `censys-2.2.1/censys/asm/__init__.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/asm/api.py` & `censys-2.2.1/censys/asm/api.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/asm/assets/assets.py` & `censys-2.2.1/censys/asm/assets/assets.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/asm/assets/domains.py` & `censys-2.2.1/censys/asm/assets/domains.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/asm/assets/subdomains.py` & `censys-2.2.1/censys/asm/assets/subdomains.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/asm/assets/web_entities.py` & `censys-2.2.1/censys/asm/assets/web_entities.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/asm/client.py` & `censys-2.2.1/censys/asm/client.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/asm/clouds.py` & `censys-2.2.1/censys/asm/clouds.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/asm/events.py` & `censys-2.2.1/censys/asm/events.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/asm/inventory.py` & `censys-2.2.1/censys/asm/inventory.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/asm/risks.py` & `censys-2.2.1/censys/asm/risks.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/asm/seeds.py` & `censys-2.2.1/censys/asm/seeds.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/cli/__init__.py` & `censys-2.2.1/censys/cli/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 #!/usr/bin/env python3
+# PYTHON_ARGCOMPLETE_OK
 """Interact with the Censys Search API through the command line."""
 import sys
 
+import argcomplete
+
 from .args import get_parser
 from censys.common.version import __version__
 
 
 def main():
     """Main cli function."""
     parser = get_parser()
 
+    # Adds autocomplete
+    argcomplete.autocomplete(parser)
+
     # Executes by subcommand
     args = parser.parse_args()
 
     if args.version:
         print(f"Censys Python Version: {__version__}")
         sys.exit(0)
```

### Comparing `censys-2.2.0/censys/cli/args.py` & `censys-2.2.1/censys/cli/args.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/cli/commands/account.py` & `censys-2.2.1/censys/cli/commands/account.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/cli/commands/asm.py` & `censys-2.2.1/censys/cli/commands/asm.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/cli/commands/config.py` & `censys-2.2.1/censys/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/cli/commands/hnri.py` & `censys-2.2.1/censys/cli/commands/hnri.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/cli/commands/subdomains.py` & `censys-2.2.1/censys/cli/commands/subdomains.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,17 @@
     """
     subdomains = set()
     try:
         client = CensysCerts(api_id=args.api_id, api_secret=args.api_secret)
         certificate_query = f"names: {args.domain}"
 
         with err_console.status(f"Querying {args.domain} subdomains"):
-            query = client.search(certificate_query, fields=["names"], pages=args.pages)
+            query = client.search(
+                certificate_query, per_page=100, pages=args.pages
+            )  # 100 is the max per page
 
             # Flatten the result, and remove duplicates
             for hits in query:
                 for cert in hits:
                     new_subdomains: List[str] = cert.get("names", [])
                     subdomains.update(
                         [
```

### Comparing `censys-2.2.0/censys/cli/commands/view.py` & `censys-2.2.1/censys/cli/commands/view.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/cli/utils.py` & `censys-2.2.1/censys/cli/utils.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/common/base.py` & `censys-2.2.1/censys/common/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,29 +8,36 @@
 import backoff
 import requests
 from requests.models import Response
 
 from .exceptions import (
     CensysAPIException,
     CensysException,
+    CensysInternalServerErrorException,
+    CensysInternalServerException,
     CensysJSONDecodeException,
+    CensysRateLimitExceededException,
     CensysTooManyRequestsException,
 )
 from .version import __version__
 
 
 # Wrapper to make max_retries configurable at runtime
 def _backoff_wrapper(method: Callable):
     @wraps(method)
     def _wrapper(self, *args, **kwargs):
         @backoff.on_exception(
             backoff.expo,
             (
+                CensysInternalServerException,
+                CensysInternalServerErrorException,
                 CensysTooManyRequestsException,
+                CensysRateLimitExceededException,
                 requests.exceptions.Timeout,
+                requests.exceptions.ConnectionError,
             ),
             max_tries=self.max_retries,
             max_time=self.timeout,
         )
         def _impl():
             return method(self, *args, **kwargs)
 
@@ -115,14 +122,37 @@
             _ (Response): HTTP requests response object.
 
         Returns:
             Type[CensysAPIException]: Exception to raise.
         """
         return CensysAPIException
 
+    @backoff.on_predicate(
+        backoff.runtime,
+        predicate=lambda r: r.status_code == 429 and r.headers.get("Retry-After"),
+        value=lambda r: int(r.headers.get("Retry-After", 0)),
+    )
+    def _call_method(
+        self, method: Callable[..., Response], url: str, request_kwargs: dict
+    ) -> Response:
+        """Make API call.
+
+        Wrapper functions for all our REST API calls checking for errors
+        and decoding the responses.
+
+        Args:
+            method (Callable): Method to send HTTP request.
+            url (str): The URL to make API requests.
+            request_kwargs (dict): Keyword arguments to pass to method.
+
+        Returns:
+            Response: Results from an API request.
+        """
+        return method(url, **request_kwargs)
+
     @_backoff_wrapper
     def _make_call(
         self,
         method: Callable[..., Response],
         endpoint: str,
         args: Optional[dict] = None,
         data: Optional[Any] = None,
@@ -157,15 +187,15 @@
             "timeout": self.timeout,
             **kwargs,
         }
 
         if data:
             request_kwargs["json"] = data
 
-        res = method(url, **request_kwargs)
+        res = self._call_method(method, url, request_kwargs)
 
         if res.ok:
             # Check for a returned json body
             try:
                 json_data = res.json()
                 if "error" not in json_data:
                     return json_data
```

### Comparing `censys-2.2.0/censys/common/config.py` & `censys-2.2.1/censys/common/config.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/common/deprecation.py` & `censys-2.2.1/censys/common/deprecation.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/common/exceptions.py` & `censys-2.2.1/censys/common/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,18 @@
     """Exception raised when you doesn't have access to the requested resource."""
 
 
 class CensysJSONDecodeException(CensysSearchException):
     """Exception raised when the resource requested is not valid JSON."""
 
 
+class CensysInternalServerException(CensysSearchException):
+    """Exception raised when the server encountered an internal error."""
+
+
 class CensysInvalidRequestException(CensysAsmException):
     """Exception raised when the HTTP request is invalid."""
 
 
 class CensysInvalidAuthTokenException(CensysAsmException):
     """Exception raised when the auth token is invalid."""
 
@@ -172,15 +176,15 @@
     """Exception raised when the requested host is not found."""
 
 
 class CensysInvalidIPv4AddressException(CensysAsmException):
     """Exception raised when the IPv4 address is invalid."""
 
 
-class CensysAssetExludedException(CensysAsmException):
+class CensysAssetExcludedException(CensysAsmException):
     """Exception raised when the asset is excluded."""
 
 
 class CensysInvalidCommentException(CensysAsmException):
     """Exception raised when the comment is invalid."""
 
 
@@ -309,15 +313,15 @@
         10015: CensysNotASeedException,
         10016: CensysTooManyInputNodesException,
         10017: CensysAssociatedAssetsThresholdWarningException,
         10018: CensysHostNotFoundException,
         10019: CensysDomainNotFoundException,
         10020: CensysCertificateNotFoundException,
         10021: CensysInvalidIPv4AddressException,
-        10022: CensysAssetExludedException,
+        10022: CensysAssetExcludedException,
         10025: CensysTagHasTrailingOrLeadingWhitespaceException,
         10026: CensysTagIsEmptyStringException,
         10027: CensysTagLabelsDifferOnlyInCasingException,
         10028: CensysTagLabelTooLongException,
         10029: CensysAppDownForMaintenanceException,
         10034: CensysTagColorTooLongException,
         10035: CensysCannotCreateTagWithNewColorException,
@@ -351,9 +355,10 @@
     """Map of status code to ASM Exception."""
 
     SEARCH_EXCEPTIONS: Dict[int, Type[CensysSearchException]] = {
         401: CensysUnauthorizedException,
         403: CensysUnauthorizedException,
         404: CensysNotFoundException,
         429: CensysRateLimitExceededException,
+        500: CensysInternalServerException,
     }
     """Map of status code to Search Exception."""
```

### Comparing `censys-2.2.0/censys/search/client.py` & `censys-2.2.1/censys/search/client.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/search/v1/api.py` & `censys-2.2.1/censys/search/v1/api.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/search/v1/certificates.py` & `censys-2.2.1/censys/search/v1/certificates.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/search/v1/data.py` & `censys-2.2.1/censys/search/v1/data.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/censys/search/v2/api.py` & `censys-2.2.1/censys/search/v2/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             """
             self.api = api
             self.query = query
             self.per_page = per_page
             self.cursor = cursor
             self.nextCursor: Optional[str] = None
             self.page = 1
-            if pages == -1:
+            if pages <= 0:
                 self.pages = float("inf")
             else:
                 self.pages = pages
             self.extra_args = kwargs
 
         def __call__(self, per_page: Optional[int] = None) -> List[dict]:
             """Search current index.
```

### Comparing `censys-2.2.0/censys/search/v2/certs.py` & `censys-2.2.1/censys/search/v2/certs.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,18 +140,21 @@
 
         Returns:
             dict: Search results.
         """
         data = {
             "q": query,
             "per_page": per_page,
-            "cursor": cursor,
-            "fields": fields,
-            "sort": sort,
         }
+        if cursor:
+            data["cursor"] = cursor
+        if fields:
+            data["fields"] = fields
+        if sort:
+            data["sort"] = sort
         data.update(kwargs)
         return self._post(self.search_path, data=data)
 
     def search_post(
         self,
         query: str,
         per_page: int = 50,
```

### Comparing `censys-2.2.0/censys/search/v2/hosts.py` & `censys-2.2.1/censys/search/v2/hosts.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.0/pyproject.toml` & `censys-2.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "censys"
-version = "2.2.0"
+version = "2.2.1"
 description = "An easy-to-use and lightweight API wrapper for Censys APIs (censys.io)."
 authors = ["Censys, Inc. <support@censys.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 include = ["censys/py.typed"]
 keywords = ["censys", "api", "search", "attack surface management"]
 classifiers = [
@@ -30,14 +30,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 [tool.poetry.urls]
 "Censys Homepage" = "https://censys.io/"
 "Censys Search" = "https://search.censys.io/"
 "Discussions" = "https://github.com/censys/censys-python/discussions"
@@ -51,39 +52,40 @@
 
 [tool.poetry.dependencies]
 python = ">=3.7.2,<4.0.0"
 requests = ">=2.29.0"
 backoff = "^2.0.1"
 rich = ">=10.16.2"
 importlib-metadata = { version = "*", python = "<3.8" }
+argcomplete = "^3.0.8"
 
 [tool.poetry.group.dev.dependencies]
 # Lint
+black = "^23.3.0"
+blacken-docs = "^1.13.0"
+darglint = "^1.8.1"
 flake8 = "^5.0.4"
+flake8-black = "^0.3.6"
+flake8-comprehensions = "^3.12.0"
 flake8-docstrings = "^1.7.0"
+flake8-isort = "^6.0.0"
 flake8-pytest-style = "^1.7.2"
 flake8-simplify = "^0.20.0"
-flake8-comprehensions = "^3.12.0"
-flake8-isort = "^6.0.0"
 isort = "^5.11.5"
 pep8-naming = "^0.13.3"
-flake8-black = "^0.3.6"
-black = "^23.3.0"
-blacken-docs = "^1.13.0"
-darglint = "^1.8.1"
 pyupgrade = "^3.3.1"
 # Tests
 pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 responses = "^0.23.1"
 parameterized = "^0.9.0"
 # Types
 mypy = "^1.2.0"
-types-requests = "^2.28.11.17"
+types-requests = "^2.29.0.0"
 
 [tool.black]
 target-version = ["py37"]
 
 [tool.isort]
 profile = "black"
 line_length = 88
```

### Comparing `censys-2.2.0/PKG-INFO` & `censys-2.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censys
-Version: 2.2.0
+Version: 2.2.1
 Summary: An easy-to-use and lightweight API wrapper for Censys APIs (censys.io).
 License: Apache-2.0
 Keywords: censys,api,search,attack surface management
 Author: Censys, Inc.
 Author-email: support@censys.io
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,28 +21,30 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
+Requires-Dist: argcomplete (>=3.0.8,<4.0.0)
 Requires-Dist: backoff (>=2.0.1,<3.0.0)
 Requires-Dist: importlib-metadata ; python_version < "3.8"
 Requires-Dist: requests (>=2.29.0)
 Requires-Dist: rich (>=10.16.2)
 Project-URL: Censys Homepage, https://censys.io/
 Project-URL: Censys Search, https://search.censys.io/
 Project-URL: Changelog, https://github.com/censys/censys-python/releases
@@ -57,27 +59,29 @@
 [![PyPI](https://img.shields.io/pypi/v/censys?color=orange&logo=pypi&logoColor=orange)](https://pypi.org/project/censys/)
 [![Python Version](https://img.shields.io/badge/python-3.7.2%2B-blue?logo=python)](https://www.python.org/downloads/)
 [![Read the Docs (version)](https://img.shields.io/readthedocs/censys-python/latest?logo=read%20the%20docs)](https://censys-python.readthedocs.io/en/stable/?badge=stable)
 [![GitHub Discussions](https://img.shields.io/badge/GitHub-Discussions-brightgreen?logo=github)](https://github.com/censys/censys-python/discussions)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-organge.svg?logo=git&logoColor=organge)](http://makeapullrequest.com)
 [![License](https://img.shields.io/github/license/censys/censys-python?logo=apache)](https://github.com/censys/censys-python/blob/main/LICENSE)
 
-An easy-to-use and lightweight API wrapper for Censys APIs ([censys.io](https://censys.io/)). Python 3.7.2+ is currently supported.
+An easy-to-use and lightweight API wrapper for Censys APIs ([censys.io](https://censys.io/)). Python 3.7.2+ is currently supported. This library has been tested on Python 3.7 and 3.x (Currently version 3.11).
 
 > **Notice:** The Censys Search v1 endpoints are deprecated as of Nov. 30, 2021. Please begin using v2 endpoints to query hosts and certificates and check out our [support center](https://support.censys.io/hc/en-us/sections/360013076551-Censys-Search-2-0) for resources.
 
 ## Features
 
 - [Search Censys data](https://censys-python.readthedocs.io/en/stable/usage-v2.html)
 - [Bulk Certificate lookups](https://censys-python.readthedocs.io/en/stable/usage-v1.html#bulk)
 - [Download Bulk Data](https://censys-python.readthedocs.io/en/stable/usage-v1.html#data)
 - [Manage assets, events, and seeds in Censys ASM](https://censys-python.readthedocs.io/en/stable/usage-asm.html)
 - [Command-line interface](https://censys-python.readthedocs.io/en/stable/cli.html)
 
+<!-- markdownlint-disable MD033 -->
 <a href="https://asciinema.org/a/500416" target="_blank"><img src="https://asciinema.org/a/500416.svg" width="600"/></a>
+<!-- markdownlint-enable MD033 -->
 
 ## Getting Started
 
 The library can be installed using `pip`.
 
 ```sh
 pip install censys
@@ -85,14 +89,30 @@
 
 To upgraded using `pip`.
 
 ```sh
 pip install --upgrade censys
 ```
 
+Or, you can install the library from source using `poetry`.
+
+```sh
+git clone https://github.com/censys/censys-python.git
+cd censys-python/
+poetry install
+```
+
+Optionally, you can enable tab completion for the CLI by adding this line to your `~/.bashrc`, `~/.zshrc`, or equivalent.
+
+> Please note that autocomplete is supported for field names in the `search` command.
+
+```sh
+eval "$(register-python-argcomplete censys)"
+```
+
 To configure your search credentials run `censys config` or set both `CENSYS_API_ID` and `CENSYS_API_SECRET` environment variables.
 
 ```sh
 $ censys config
 
 Censys API ID: XXX
 Censys API Secret: XXX
```

