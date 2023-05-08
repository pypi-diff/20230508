# Comparing `tmp/uplc-0.6.5.tar.gz` & `tmp/uplc-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uplc-0.6.5.tar", max compression
+gzip compressed data, was "uplc-0.6.6.tar", max compression
```

## Comparing `uplc-0.6.5.tar` & `uplc-0.6.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1077 2023-01-04 11:32:30.433673 uplc-0.6.5/LICENSE.txt
--rw-r--r--   0        0        0     2218 2023-05-03 14:34:13.048895 uplc-0.6.5/README.md
--rw-r--r--   0        0        0     1347 2023-05-03 14:30:50.424968 uplc-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      506 2023-05-03 14:30:50.424968 uplc-0.6.5/uplc/__init__.py
--rw-r--r--   0        0        0     4935 2023-03-26 20:25:01.867354 uplc-0.6.5/uplc/__main__.py
--rw-r--r--   0        0        0    28464 2023-04-24 17:32:55.398635 uplc-0.6.5/uplc/ast.py
--rw-r--r--   0        0        0     9066 2023-03-26 20:25:01.867354 uplc-0.6.5/uplc/flat_decoder.py
--rw-r--r--   0        0        0    10052 2023-03-26 20:25:01.867354 uplc-0.6.5/uplc/flat_encoder.py
--rw-r--r--   0        0        0     1202 2023-02-14 01:15:57.671994 uplc-0.6.5/uplc/lexer.py
--rw-r--r--   0        0        0     3357 2023-03-16 14:22:54.137366 uplc-0.6.5/uplc/machine.py
--rw-r--r--   0        0        0        0 2023-02-09 01:14:10.658495 uplc-0.6.5/uplc/optimizer/__init__.py
--rw-r--r--   0        0        0      630 2023-04-06 19:16:35.707063 uplc-0.6.5/uplc/optimizer/pre_evaluation.py
--rw-r--r--   0        0        0    10960 2023-03-26 20:25:01.867354 uplc-0.6.5/uplc/parser.py
--rw-r--r--   0        0        0        0 2023-01-09 21:06:56.197975 uplc-0.6.5/uplc/tests/__init__.py
--rw-r--r--   0        0        0     3391 2023-02-09 01:14:54.974376 uplc-0.6.5/uplc/tests/test_acceptance.py
--rw-r--r--   0        0        0    14584 2023-04-24 17:32:55.398635 uplc-0.6.5/uplc/tests/test_hypothesis.py
--rw-r--r--   0        0        0   211128 2023-03-26 20:25:01.871354 uplc-0.6.5/uplc/tests/test_misc.py
--rw-r--r--   0        0        0     1998 2023-04-06 19:16:35.707063 uplc-0.6.5/uplc/tools.py
--rw-r--r--   0        0        0        0 2023-01-22 02:07:47.763052 uplc-0.6.5/uplc/transformer/__init__.py
--rw-r--r--   0        0        0      784 2023-03-26 20:25:01.871354 uplc-0.6.5/uplc/transformer/debrujin_variables.py
--rw-r--r--   0        0        0      938 2023-03-26 20:25:01.871354 uplc-0.6.5/uplc/transformer/undebrujin_variables.py
--rw-r--r--   0        0        0     1947 2023-04-13 20:56:49.628229 uplc-0.6.5/uplc/transformer/unique_variables.py
--rw-r--r--   0        0        0     3009 2023-04-06 19:16:35.707063 uplc-0.6.5/uplc/util.py
--rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 uplc-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-08 19:03:17.159501 uplc-0.6.6/LICENSE.txt
+-rw-r--r--   0        0        0     2218 2023-05-08 19:03:17.159501 uplc-0.6.6/README.md
+-rw-r--r--   0        0        0     1347 2023-05-08 19:03:17.223501 uplc-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0      506 2023-05-08 19:03:17.223501 uplc-0.6.6/uplc/__init__.py
+-rw-r--r--   0        0        0     4935 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/__main__.py
+-rw-r--r--   0        0        0    28865 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/ast.py
+-rw-r--r--   0        0        0     9066 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/flat_decoder.py
+-rw-r--r--   0        0        0    10052 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/flat_encoder.py
+-rw-r--r--   0        0        0     1202 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/lexer.py
+-rw-r--r--   0        0        0     3357 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/machine.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/optimizer/__init__.py
+-rw-r--r--   0        0        0      630 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/optimizer/pre_evaluation.py
+-rw-r--r--   0        0        0    10960 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/parser.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/tests/__init__.py
+-rw-r--r--   0        0        0     3391 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/tests/test_acceptance.py
+-rw-r--r--   0        0        0    14584 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/tests/test_hypothesis.py
+-rw-r--r--   0        0        0   211128 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/tests/test_misc.py
+-rw-r--r--   0        0        0     1998 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/tools.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/transformer/__init__.py
+-rw-r--r--   0        0        0      784 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/transformer/debrujin_variables.py
+-rw-r--r--   0        0        0      938 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/transformer/undebrujin_variables.py
+-rw-r--r--   0        0        0     1947 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/transformer/unique_variables.py
+-rw-r--r--   0        0        0     3009 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/util.py
+-rw-r--r--   0        0        0     3559 1970-01-01 00:00:00.000000 uplc-0.6.6/PKG-INFO
```

### Comparing `uplc-0.6.5/LICENSE.txt` & `uplc-0.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/README.md` & `uplc-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/pyproject.toml` & `uplc-0.6.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uplc"
-version = "0.6.5"
+version = "0.6.6"
 description = "Python implementation of untyped plutus language core"
 authors = ["nielstron <n.muendler@web.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/opshin/uplc"
 keywords = ["python", "language", "programming-language", "compiler", "validator", "smart-contracts", "cardano"]
 classifiers=[
@@ -21,15 +21,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 frozendict = "^2.3.8"
 cbor2 = "^5.4.6"
 frozenlist = "^1.3.3"
 rply = "^0.7.8"
-pycardano = "^0.8.1"
+pycardano = "^0.9.0"
 python-secp256k1-cardano = "^0.2.3"
 
 [tool.poetry.group.dev.dependencies]
 pyaiken = "^0.5.1"
 hypothesis = "^6.75.0"
 parameterized = "^0.9.0"
 poetry-bumpversion = "^0.3.0"
```

### Comparing `uplc-0.6.5/uplc/__main__.py` & `uplc-0.6.6/uplc/__main__.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/uplc/ast.py` & `uplc-0.6.6/uplc/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 import cbor2
 import frozendict
 import frozenlist
 import nacl.exceptions
 from _cbor2 import CBOREncoder
 from pycardano.crypto.bip32 import BIP32ED25519PublicKey
+from pycardano import IndefiniteList
 
 try:
     import pysecp256k1
 except ImportError:
     pysecp256k1 = None
 
 try:
@@ -401,40 +402,46 @@
 
 @dataclass(frozen=True, eq=True)
 class PlutusConstr(PlutusData):
     constructor: int
     fields: Union[List[PlutusData], frozenlist.FrozenList]
 
     def to_cbor(self):
+        fields = (
+            IndefiniteList([f.to_cbor() for f in self.fields]) if self.fields else []
+        )
         if 0 <= self.constructor < 7:
-            return cbor2.CBORTag(
-                self.constructor + 121, [f.to_cbor() for f in self.fields]
-            )
+            return cbor2.CBORTag(self.constructor + 121, fields)
         elif 7 <= self.constructor < 128:
-            return cbor2.CBORTag(
-                (self.constructor - 7) + 1280, [f.to_cbor() for f in self.fields]
-            )
+            return cbor2.CBORTag((self.constructor - 7) + 1280, fields)
         else:
-            return cbor2.CBORTag(
-                102, [self.constructor, [f.to_cbor() for f in self.fields]]
-            )
+            return cbor2.CBORTag(102, [self.constructor, fields])
 
     def to_json(self):
         return {
             "constructor": self.constructor,
             "fields": [v.to_json() for v in self.fields],
         }
 
 
 def _int_to_bytes(x: int):
     return x.to_bytes((x.bit_length() + 7) // 8, byteorder="big")
 
 
-def default_encoder(encoder: CBOREncoder, value: PlutusData):
+def default_encoder(encoder: CBOREncoder, value: Union[PlutusData, IndefiniteList]):
     """A fallback function that encodes PlutusData objects"""
+    if isinstance(value, IndefiniteList):
+        # Currently, cbor2 doesn't support indefinite list, therefore we need special
+        # handling here to explicitly write header (b'\x9f'), each body item, and footer (b'\xff') to
+        # the output bytestring.
+        encoder.write(b"\x9f")
+        for item in value:
+            encoder.encode(item)
+        encoder.write(b"\xff")
+        return
     if not isinstance(value, PlutusData):
         raise NotImplementedError(f"Can not encode type {type(value)}")
     value = value.to_cbor()
     if isinstance(value, PlutusByteString):
         # the encoder can not handle indefinite length arrays, but the plutus standard
         # requires encoding bytes as indefinite byte sequence where each chunk is at most 64 bytes long
         byts = value.value
```

### Comparing `uplc-0.6.5/uplc/flat_decoder.py` & `uplc-0.6.6/uplc/flat_decoder.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/uplc/flat_encoder.py` & `uplc-0.6.6/uplc/flat_encoder.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/uplc/lexer.py` & `uplc-0.6.6/uplc/lexer.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/uplc/machine.py` & `uplc-0.6.6/uplc/machine.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/uplc/optimizer/pre_evaluation.py` & `uplc-0.6.6/uplc/optimizer/pre_evaluation.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/uplc/parser.py` & `uplc-0.6.6/uplc/parser.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/uplc/tests/test_acceptance.py` & `uplc-0.6.6/uplc/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/uplc/tests/test_hypothesis.py` & `uplc-0.6.6/uplc/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/uplc/tests/test_misc.py` & `uplc-0.6.6/uplc/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/uplc/tools.py` & `uplc-0.6.6/uplc/tools.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/uplc/transformer/debrujin_variables.py` & `uplc-0.6.6/uplc/transformer/debrujin_variables.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/uplc/transformer/undebrujin_variables.py` & `uplc-0.6.6/uplc/transformer/undebrujin_variables.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/uplc/transformer/unique_variables.py` & `uplc-0.6.6/uplc/transformer/unique_variables.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/uplc/util.py` & `uplc-0.6.6/uplc/util.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.5/PKG-INFO` & `uplc-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uplc
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python implementation of untyped plutus language core
 Home-page: https://github.com/opshin/uplc
 License: MIT
 Keywords: python,language,programming-language,compiler,validator,smart-contracts,cardano
 Author: nielstron
 Author-email: n.muendler@web.de
 Requires-Python: >=3.8,<3.12
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Assemblers
 Requires-Dist: cbor2 (>=5.4.6,<6.0.0)
 Requires-Dist: frozendict (>=2.3.8,<3.0.0)
 Requires-Dist: frozenlist (>=1.3.3,<2.0.0)
-Requires-Dist: pycardano (>=0.8.1,<0.9.0)
+Requires-Dist: pycardano (>=0.9.0,<0.10.0)
 Requires-Dist: python-secp256k1-cardano (>=0.2.3,<0.3.0)
 Requires-Dist: rply (>=0.7.8,<0.8.0)
 Project-URL: Repository, https://github.com/opshin/uplc
 Description-Content-Type: text/markdown
 
 Untyped Plutus Language Core 
 ==================================================
```

