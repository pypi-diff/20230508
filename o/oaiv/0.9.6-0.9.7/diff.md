# Comparing `tmp/oaiv-0.9.6.tar.gz` & `tmp/oaiv-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaiv-0.9.6.tar", last modified: Fri Nov 11 15:22:36 2022, max compression
+gzip compressed data, was "oaiv-0.9.7.tar", last modified: Sat Nov 12 14:12:17 2022, max compression
```

## Comparing `oaiv-0.9.6.tar` & `oaiv-0.9.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-11-11 15:22:36.110023 oaiv-0.9.6/
--rw-rw-rw-   0        0        0      324 2022-11-11 15:22:36.110023 oaiv-0.9.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-11-11 15:22:36.080305 oaiv-0.9.6/oaiv/
--rw-rw-rw-   0        0        0        0 2022-09-28 17:56:34.000000 oaiv-0.9.6/oaiv/__init__.py
--rw-rw-rw-   0        0        0      867 2022-11-11 10:05:43.000000 oaiv-0.9.6/oaiv/constants.py
-drwxrwxrwx   0        0        0        0 2022-11-11 15:22:36.101156 oaiv-0.9.6/oaiv/core/
--rw-rw-rw-   0        0        0        0 2022-09-28 17:56:34.000000 oaiv-0.9.6/oaiv/core/__init__.py
--rw-rw-rw-   0        0        0    20475 2022-11-11 14:43:31.000000 oaiv-0.9.6/oaiv/core/account.py
-drwxrwxrwx   0        0        0        0 2022-11-11 15:22:36.101156 oaiv-0.9.6/oaiv/modules/
--rw-rw-rw-   0        0        0        0 2022-09-28 17:56:34.000000 oaiv-0.9.6/oaiv/modules/__init__.py
--rw-rw-rw-   0        0        0     2611 2022-09-28 17:59:49.000000 oaiv-0.9.6/oaiv/modules/swap.py
-drwxrwxrwx   0        0        0        0 2022-11-11 15:22:36.110023 oaiv-0.9.6/oaiv/tools/
--rw-rw-rw-   0        0        0        0 2022-09-28 17:56:34.000000 oaiv-0.9.6/oaiv/tools/__init__.py
--rw-rw-rw-   0        0        0     9859 2022-09-28 17:59:49.000000 oaiv-0.9.6/oaiv/tools/address.py
--rw-rw-rw-   0        0        0     1042 2022-09-28 17:59:49.000000 oaiv-0.9.6/oaiv/tools/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-11 15:22:36.099132 oaiv-0.9.6/oaiv.egg-info/
--rw-rw-rw-   0        0        0      324 2022-11-11 15:22:36.000000 oaiv-0.9.6/oaiv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2022-11-11 15:22:36.000000 oaiv-0.9.6/oaiv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-11 15:22:36.000000 oaiv-0.9.6/oaiv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2022-11-11 15:22:36.000000 oaiv-0.9.6/oaiv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-11 15:22:36.110023 oaiv-0.9.6/setup.cfg
--rw-rw-rw-   0        0        0      667 2022-11-11 14:14:56.000000 oaiv-0.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-12 14:12:17.384928 oaiv-0.9.7/
+-rw-rw-rw-   0        0        0      324 2022-11-12 14:12:17.384928 oaiv-0.9.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-11-12 14:12:17.335894 oaiv-0.9.7/oaiv/
+-rw-rw-rw-   0        0        0        0 2022-09-28 17:56:34.000000 oaiv-0.9.7/oaiv/__init__.py
+-rw-rw-rw-   0        0        0     1569 2022-11-12 13:41:53.000000 oaiv-0.9.7/oaiv/constants.py
+drwxrwxrwx   0        0        0        0 2022-11-12 14:12:17.366079 oaiv-0.9.7/oaiv/core/
+-rw-rw-rw-   0        0        0        0 2022-09-28 17:56:34.000000 oaiv-0.9.7/oaiv/core/__init__.py
+-rw-rw-rw-   0        0        0    20475 2022-11-11 14:43:31.000000 oaiv-0.9.7/oaiv/core/account.py
+drwxrwxrwx   0        0        0        0 2022-11-12 14:12:17.375886 oaiv-0.9.7/oaiv/modules/
+-rw-rw-rw-   0        0        0        0 2022-09-28 17:56:34.000000 oaiv-0.9.7/oaiv/modules/__init__.py
+-rw-rw-rw-   0        0        0     2611 2022-09-28 17:59:49.000000 oaiv-0.9.7/oaiv/modules/swap.py
+drwxrwxrwx   0        0        0        0 2022-11-12 14:12:17.384928 oaiv-0.9.7/oaiv/tools/
+-rw-rw-rw-   0        0        0        0 2022-09-28 17:56:34.000000 oaiv-0.9.7/oaiv/tools/__init__.py
+-rw-rw-rw-   0        0        0     9859 2022-09-28 17:59:49.000000 oaiv-0.9.7/oaiv/tools/address.py
+-rw-rw-rw-   0        0        0     1042 2022-09-28 17:59:49.000000 oaiv-0.9.7/oaiv/tools/utils.py
+drwxrwxrwx   0        0        0        0 2022-11-12 14:12:17.354976 oaiv-0.9.7/oaiv.egg-info/
+-rw-rw-rw-   0        0        0      324 2022-11-12 14:12:17.000000 oaiv-0.9.7/oaiv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2022-11-12 14:12:17.000000 oaiv-0.9.7/oaiv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-12 14:12:17.000000 oaiv-0.9.7/oaiv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2022-11-12 14:12:17.000000 oaiv-0.9.7/oaiv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-11-12 14:12:17.384928 oaiv-0.9.7/setup.cfg
+-rw-rw-rw-   0        0        0      667 2022-11-12 14:09:49.000000 oaiv-0.9.7/setup.py
```

### Comparing `oaiv-0.9.6/oaiv/constants.py` & `oaiv-0.9.7/oaiv/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,50 @@
 #
 
 
 #
 
 
 #
+class BlockchainName:
+    ETHEREUM = 'ETHEREUM'
+    BITCOIN = 'BITCOIN'
+
+
 class BlockchainType(Enum):
     ETHEREUM = auto()
     BITCOIN = auto()
 
 
-def blockchain_name(blockchain_name):
-    available = {'ETHEREUM': BlockchainType.ETHEREUM,
-                 'BITCOIN': BlockchainType.BITCOIN}
+def blockchain_type(blockchain_name):
+    available = {BlockchainName.ETHEREUM: BlockchainType.ETHEREUM,
+                 BlockchainName.BITCOIN: BlockchainType.BITCOIN}
     if blockchain_name in available.keys():
         return available[blockchain_name]
     else:
         raise KeyError("Invalid blockchain type {0} is entered; please, check available ones".format(blockchain_type))
 
 
-def blockchain_type(blockchain_type):
-    available = {BlockchainType.ETHEREUM: 'ETHEREUM',
-                 BlockchainType.BITCOIN: 'BITCOIN'}
+def blockchain_name(blockchain_type):
+    available = {BlockchainType.ETHEREUM: BlockchainName.ETHEREUM,
+                 BlockchainType.BITCOIN: BlockchainName.BITCOIN}
     if blockchain_type in available.keys():
         return available[blockchain_type]
     else:
         raise KeyError("Invalid blockchain name {0} is entered; please, check available ones".format(blockchain_name))
+
+
+def available_blockchain_types():
+    return [BlockchainType.ETHEREUM, BlockchainType.BITCOIN]
+
+
+def available_blockchain_names():
+    return [BlockchainName.ETHEREUM, BlockchainName.BITCOIN]
+
+
+def blockchain_gas_currency(blockchain_type):
+    available = {BlockchainType.ETHEREUM: 'ETH',
+                 BlockchainType.BITCOIN: 'BTC'}
+    if blockchain_type in available.keys():
+        return available[blockchain_type]
+    else:
+        raise KeyError("Invalid blockchain type {0} is entered; please, check available ones".format(blockchain_type))
```

### Comparing `oaiv-0.9.6/oaiv/core/account.py` & `oaiv-0.9.7/oaiv/core/account.py`

 * *Files identical despite different names*

### Comparing `oaiv-0.9.6/oaiv/modules/swap.py` & `oaiv-0.9.7/oaiv/modules/swap.py`

 * *Files identical despite different names*

### Comparing `oaiv-0.9.6/oaiv/tools/address.py` & `oaiv-0.9.7/oaiv/tools/address.py`

 * *Files identical despite different names*

### Comparing `oaiv-0.9.6/oaiv/tools/utils.py` & `oaiv-0.9.7/oaiv/tools/utils.py`

 * *Files identical despite different names*

### Comparing `oaiv-0.9.6/setup.py` & `oaiv-0.9.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,13 +8,13 @@
             'maintainer_email': 'edazizovv@gmail.com',
             'description': 'Blockchain Interaction Library',
             'license': 'MIT',
             'url': 'https://github.com/edazizovv/oaiv',
             'download_url': 'https://github.com/edazizovv/oaiv',
             'packages': setuptools.find_packages(),
             'include_package_data': True,
-            'version': '0.9.6',
+            'version': '0.9.7',
             'long_description': '',
             'python_requires': '>=3.10',
             'install_requires': []}
 
 setup(**metadata)
```

