# Comparing `tmp/dbus-signature-pyparsing-0.4.tar.gz` & `tmp/dbus-signature-pyparsing-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dbus-signature-pyparsing-0.4.tar", last modified: Thu Dec  3 03:09:08 2020, max compression
+gzip compressed data, was "dbus-signature-pyparsing-0.4.1.tar", last modified: Mon May  8 02:26:18 2023, max compression
```

## Comparing `dbus-signature-pyparsing-0.4.tar` & `dbus-signature-pyparsing-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,21 @@
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2020-12-03 03:09:08.000000 dbus-signature-pyparsing-0.4/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    11358 2019-01-14 15:50:21.000000 dbus-signature-pyparsing-0.4/LICENSE
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      200 2019-01-14 15:50:21.000000 dbus-signature-pyparsing-0.4/MANIFEST.in
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3806 2020-12-03 03:09:08.000000 dbus-signature-pyparsing-0.4/PKG-INFO
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2496 2020-11-30 18:03:15.000000 dbus-signature-pyparsing-0.4/README.rst
--rwxrwxr-x   0 mulhern   (1000) mulhern   (1000)     1454 2020-12-02 17:44:41.000000 dbus-signature-pyparsing-0.4/check.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       41 2020-08-07 16:26:38.000000 dbus-signature-pyparsing-0.4/requirements.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       38 2020-12-03 03:09:08.000000 dbus-signature-pyparsing-0.4/setup.cfg
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1534 2020-12-02 17:44:41.000000 dbus-signature-pyparsing-0.4/setup.py
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2020-12-03 03:09:08.000000 dbus-signature-pyparsing-0.4/src/
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2020-12-03 03:09:08.000000 dbus-signature-pyparsing-0.4/src/dbus_signature_pyparsing/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      666 2020-08-07 16:26:38.000000 dbus-signature-pyparsing-0.4/src/dbus_signature_pyparsing/__init__.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2714 2020-12-02 18:52:24.000000 dbus-signature-pyparsing-0.4/src/dbus_signature_pyparsing/_parsing.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      752 2020-12-03 02:47:02.000000 dbus-signature-pyparsing-0.4/src/dbus_signature_pyparsing/_version.py
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2020-12-03 03:09:08.000000 dbus-signature-pyparsing-0.4/src/dbus_signature_pyparsing.egg-info/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3806 2020-12-03 03:09:08.000000 dbus-signature-pyparsing-0.4/src/dbus_signature_pyparsing.egg-info/PKG-INFO
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      536 2020-12-03 03:09:08.000000 dbus-signature-pyparsing-0.4/src/dbus_signature_pyparsing.egg-info/SOURCES.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        1 2020-12-03 03:09:08.000000 dbus-signature-pyparsing-0.4/src/dbus_signature_pyparsing.egg-info/dependency_links.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       10 2020-12-03 03:09:08.000000 dbus-signature-pyparsing-0.4/src/dbus_signature_pyparsing.egg-info/requires.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       25 2020-12-03 03:09:08.000000 dbus-signature-pyparsing-0.4/src/dbus_signature_pyparsing.egg-info/top_level.txt
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2020-12-03 03:09:08.000000 dbus-signature-pyparsing-0.4/tests/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        0 2019-01-14 15:50:21.000000 dbus-signature-pyparsing-0.4/tests/__init__.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1906 2020-12-02 17:32:30.000000 dbus-signature-pyparsing-0.4/tests/test_deterministic.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1401 2020-12-02 19:51:00.000000 dbus-signature-pyparsing-0.4/tests/test_hypothesis.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      668 2020-12-02 19:51:00.000000 dbus-signature-pyparsing-0.4/tox.ini
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-05-08 02:26:18.445100 dbus-signature-pyparsing-0.4.1/
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)    11358 2021-06-03 22:06:49.000000 dbus-signature-pyparsing-0.4.1/LICENSE
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)     3376 2023-05-08 02:26:18.445100 dbus-signature-pyparsing-0.4.1/PKG-INFO
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     2496 2021-06-03 22:06:49.000000 dbus-signature-pyparsing-0.4.1/README.rst
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)       81 2023-05-08 02:14:35.000000 dbus-signature-pyparsing-0.4.1/pyproject.toml
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)      988 2023-05-08 02:26:18.446100 dbus-signature-pyparsing-0.4.1/setup.cfg
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)      106 2023-05-08 02:14:35.000000 dbus-signature-pyparsing-0.4.1/setup.py
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-05-08 02:26:18.443100 dbus-signature-pyparsing-0.4.1/src/
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-05-08 02:26:18.444100 dbus-signature-pyparsing-0.4.1/src/dbus_signature_pyparsing/
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)      700 2023-05-08 02:14:35.000000 dbus-signature-pyparsing-0.4.1/src/dbus_signature_pyparsing/__init__.py
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     2714 2021-06-03 22:06:49.000000 dbus-signature-pyparsing-0.4.1/src/dbus_signature_pyparsing/_parsing.py
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)      753 2023-05-08 02:22:08.000000 dbus-signature-pyparsing-0.4.1/src/dbus_signature_pyparsing/_version.py
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-05-08 02:26:18.445100 dbus-signature-pyparsing-0.4.1/src/dbus_signature_pyparsing.egg-info/
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)     3376 2023-05-08 02:26:18.000000 dbus-signature-pyparsing-0.4.1/src/dbus_signature_pyparsing.egg-info/PKG-INFO
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)      487 2023-05-08 02:26:18.000000 dbus-signature-pyparsing-0.4.1/src/dbus_signature_pyparsing.egg-info/SOURCES.txt
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)        1 2023-05-08 02:26:18.000000 dbus-signature-pyparsing-0.4.1/src/dbus_signature_pyparsing.egg-info/dependency_links.txt
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)       10 2023-05-08 02:26:18.000000 dbus-signature-pyparsing-0.4.1/src/dbus_signature_pyparsing.egg-info/requires.txt
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)       25 2023-05-08 02:26:18.000000 dbus-signature-pyparsing-0.4.1/src/dbus_signature_pyparsing.egg-info/top_level.txt
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-05-08 02:26:18.445100 dbus-signature-pyparsing-0.4.1/tests/
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     1906 2021-06-03 22:06:49.000000 dbus-signature-pyparsing-0.4.1/tests/test_deterministic.py
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     1401 2021-06-03 22:06:49.000000 dbus-signature-pyparsing-0.4.1/tests/test_hypothesis.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dbus-signature-pyparsing-0.4/LICENSE` & `dbus-signature-pyparsing-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbus-signature-pyparsing-0.4/PKG-INFO` & `dbus-signature-pyparsing-0.4.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,82 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dbus-signature-pyparsing
-Version: 0.4
-Summary: dbus signature parser
+Version: 0.4.1
+Summary: "dbus signature parser"
 Home-page: https://github.com/stratis-storage/dbus-signature-pyparsing
 Author: Anne Mulhern
 Author-email: amulhern@redhat.com
-License: Apache 2.0
-Description: A Parser for a D-Bus Signature
-        ==============================
-        
-        A parser for a dbus signature.
-        
-        Introduction
-        ------------
-        
-        This module contains a parser for dbus signatures constructed using the
-        pyparsing library (http://pyparsing.wikispaces.com/).
-        
-        The grammar follows the informal specifications at
-        https://dbus.freedesktop.org/doc/dbus-specification.html.
-        This grammar is a very simple one, parsable by an LL(1) parser.
-        
-        The grammar has undergone significant testing using the Hypothesis testing
-        library (http://hypothesis.works/).
-        
-        Usage and Implementation Hints
-        ------------------------------
-        
-        Usage of the library to verify that a string is a signature is fairly
-        straightforward::
-        
-           >>> from dbus_signature_pyparsing import Parser
-           >>> parser = Parser()
-           >>> parser.PARSER.parseString("a(qy)", parseAll=True)
-        
-        If parseString() does not raise a pyparsing exception, the argument string
-        is a valid signature.
-        
-        Note that the empty string is a valid signature. Thus, it is important to
-        require that the parser parse the entire string by setting the parseAll
-        parameter to True. If parseAll is False, which is the default, the parser
-        can always parse the empty string, and every string will be parsed and verified
-        to be a valid signature.
-        
-        The Parser object exposes all its sub-parsers as instance attributes.
-        The PARSER attribute is the top-level parser, suitable for parsing general
-        signatures. The COMPLETE attribute parses what is defined in the
-        informal specification as a "single complete type". The CODE attribute is
-        equivalent to the specification's "type code".
-        
-        The parser is easily used either by delegation or by inheritance. Each
-        sub-parser attribute is a ParserElement; consequently each sub-parser supports
-        the addParseAction() method. To customize the basic parser to return a
-        particular value as a result of having parsed a signature invoke the
-        addParseAction() method on each appropriate sub-parser with an appropriately
-        chosen method. The modified parser should then return the desired value when
-        the parseString() method is invoked on a valid signature string.
-        For further assistance, consult pyparsing's extensive documentation at
-        http://pyparsing.wikispaces.com/ and https://pythonhosted.org/pyparsing/.
-        
-        Packaging
-        ---------
-        
-        Downstream packagers, if incorporating testing into their packaging, are
-        encouraged to use only the tests in the test_deterministic.py module, to
-        avoid testing failures that may arise due to the non-deterministic behavior
-        of Hypothesis tests.
-        
+License: Apache-2.0
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+A Parser for a D-Bus Signature
+==============================
+
+A parser for a dbus signature.
+
+Introduction
+------------
+
+This module contains a parser for dbus signatures constructed using the
+pyparsing library (http://pyparsing.wikispaces.com/).
+
+The grammar follows the informal specifications at
+https://dbus.freedesktop.org/doc/dbus-specification.html.
+This grammar is a very simple one, parsable by an LL(1) parser.
+
+The grammar has undergone significant testing using the Hypothesis testing
+library (http://hypothesis.works/).
+
+Usage and Implementation Hints
+------------------------------
+
+Usage of the library to verify that a string is a signature is fairly
+straightforward::
+
+   >>> from dbus_signature_pyparsing import Parser
+   >>> parser = Parser()
+   >>> parser.PARSER.parseString("a(qy)", parseAll=True)
+
+If parseString() does not raise a pyparsing exception, the argument string
+is a valid signature.
+
+Note that the empty string is a valid signature. Thus, it is important to
+require that the parser parse the entire string by setting the parseAll
+parameter to True. If parseAll is False, which is the default, the parser
+can always parse the empty string, and every string will be parsed and verified
+to be a valid signature.
+
+The Parser object exposes all its sub-parsers as instance attributes.
+The PARSER attribute is the top-level parser, suitable for parsing general
+signatures. The COMPLETE attribute parses what is defined in the
+informal specification as a "single complete type". The CODE attribute is
+equivalent to the specification's "type code".
+
+The parser is easily used either by delegation or by inheritance. Each
+sub-parser attribute is a ParserElement; consequently each sub-parser supports
+the addParseAction() method. To customize the basic parser to return a
+particular value as a result of having parsed a signature invoke the
+addParseAction() method on each appropriate sub-parser with an appropriately
+chosen method. The modified parser should then return the desired value when
+the parseString() method is invoked on a valid signature string.
+For further assistance, consult pyparsing's extensive documentation at
+http://pyparsing.wikispaces.com/ and https://pythonhosted.org/pyparsing/.
+
+Packaging
+---------
+
+Downstream packagers, if incorporating testing into their packaging, are
+encouraged to use only the tests in the test_deterministic.py module, to
+avoid testing failures that may arise due to the non-deterministic behavior
+of Hypothesis tests.
```

### Comparing `dbus-signature-pyparsing-0.4/README.rst` & `dbus-signature-pyparsing-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `dbus-signature-pyparsing-0.4/src/dbus_signature_pyparsing/__init__.py` & `dbus-signature-pyparsing-0.4.1/src/dbus_signature_pyparsing/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,7 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Module for parsing dbus signature using pyparsing.
 """
 
 from ._parsing import Parser
+from ._version import __version__
```

### Comparing `dbus-signature-pyparsing-0.4/src/dbus_signature_pyparsing/_parsing.py` & `dbus-signature-pyparsing-0.4.1/src/dbus_signature_pyparsing/_parsing.py`

 * *Files identical despite different names*

### Comparing `dbus-signature-pyparsing-0.4/src/dbus_signature_pyparsing/_version.py` & `dbus-signature-pyparsing-0.4.1/src/dbus_signature_pyparsing/_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 # limitations under the License.
 """
     Version information.
 
     .. moduleauthor::  mulhern  <amulhern@redhat.com>
 """
 
-__version__ = "0.04"
+__version__ = "0.4.1"
 __version_info__ = tuple(int(x) for x in __version__.split("."))
```

### Comparing `dbus-signature-pyparsing-0.4/src/dbus_signature_pyparsing.egg-info/PKG-INFO` & `dbus-signature-pyparsing-0.4.1/src/dbus_signature_pyparsing.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,82 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dbus-signature-pyparsing
-Version: 0.4
-Summary: dbus signature parser
+Version: 0.4.1
+Summary: "dbus signature parser"
 Home-page: https://github.com/stratis-storage/dbus-signature-pyparsing
 Author: Anne Mulhern
 Author-email: amulhern@redhat.com
-License: Apache 2.0
-Description: A Parser for a D-Bus Signature
-        ==============================
-        
-        A parser for a dbus signature.
-        
-        Introduction
-        ------------
-        
-        This module contains a parser for dbus signatures constructed using the
-        pyparsing library (http://pyparsing.wikispaces.com/).
-        
-        The grammar follows the informal specifications at
-        https://dbus.freedesktop.org/doc/dbus-specification.html.
-        This grammar is a very simple one, parsable by an LL(1) parser.
-        
-        The grammar has undergone significant testing using the Hypothesis testing
-        library (http://hypothesis.works/).
-        
-        Usage and Implementation Hints
-        ------------------------------
-        
-        Usage of the library to verify that a string is a signature is fairly
-        straightforward::
-        
-           >>> from dbus_signature_pyparsing import Parser
-           >>> parser = Parser()
-           >>> parser.PARSER.parseString("a(qy)", parseAll=True)
-        
-        If parseString() does not raise a pyparsing exception, the argument string
-        is a valid signature.
-        
-        Note that the empty string is a valid signature. Thus, it is important to
-        require that the parser parse the entire string by setting the parseAll
-        parameter to True. If parseAll is False, which is the default, the parser
-        can always parse the empty string, and every string will be parsed and verified
-        to be a valid signature.
-        
-        The Parser object exposes all its sub-parsers as instance attributes.
-        The PARSER attribute is the top-level parser, suitable for parsing general
-        signatures. The COMPLETE attribute parses what is defined in the
-        informal specification as a "single complete type". The CODE attribute is
-        equivalent to the specification's "type code".
-        
-        The parser is easily used either by delegation or by inheritance. Each
-        sub-parser attribute is a ParserElement; consequently each sub-parser supports
-        the addParseAction() method. To customize the basic parser to return a
-        particular value as a result of having parsed a signature invoke the
-        addParseAction() method on each appropriate sub-parser with an appropriately
-        chosen method. The modified parser should then return the desired value when
-        the parseString() method is invoked on a valid signature string.
-        For further assistance, consult pyparsing's extensive documentation at
-        http://pyparsing.wikispaces.com/ and https://pythonhosted.org/pyparsing/.
-        
-        Packaging
-        ---------
-        
-        Downstream packagers, if incorporating testing into their packaging, are
-        encouraged to use only the tests in the test_deterministic.py module, to
-        avoid testing failures that may arise due to the non-deterministic behavior
-        of Hypothesis tests.
-        
+License: Apache-2.0
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+A Parser for a D-Bus Signature
+==============================
+
+A parser for a dbus signature.
+
+Introduction
+------------
+
+This module contains a parser for dbus signatures constructed using the
+pyparsing library (http://pyparsing.wikispaces.com/).
+
+The grammar follows the informal specifications at
+https://dbus.freedesktop.org/doc/dbus-specification.html.
+This grammar is a very simple one, parsable by an LL(1) parser.
+
+The grammar has undergone significant testing using the Hypothesis testing
+library (http://hypothesis.works/).
+
+Usage and Implementation Hints
+------------------------------
+
+Usage of the library to verify that a string is a signature is fairly
+straightforward::
+
+   >>> from dbus_signature_pyparsing import Parser
+   >>> parser = Parser()
+   >>> parser.PARSER.parseString("a(qy)", parseAll=True)
+
+If parseString() does not raise a pyparsing exception, the argument string
+is a valid signature.
+
+Note that the empty string is a valid signature. Thus, it is important to
+require that the parser parse the entire string by setting the parseAll
+parameter to True. If parseAll is False, which is the default, the parser
+can always parse the empty string, and every string will be parsed and verified
+to be a valid signature.
+
+The Parser object exposes all its sub-parsers as instance attributes.
+The PARSER attribute is the top-level parser, suitable for parsing general
+signatures. The COMPLETE attribute parses what is defined in the
+informal specification as a "single complete type". The CODE attribute is
+equivalent to the specification's "type code".
+
+The parser is easily used either by delegation or by inheritance. Each
+sub-parser attribute is a ParserElement; consequently each sub-parser supports
+the addParseAction() method. To customize the basic parser to return a
+particular value as a result of having parsed a signature invoke the
+addParseAction() method on each appropriate sub-parser with an appropriately
+chosen method. The modified parser should then return the desired value when
+the parseString() method is invoked on a valid signature string.
+For further assistance, consult pyparsing's extensive documentation at
+http://pyparsing.wikispaces.com/ and https://pythonhosted.org/pyparsing/.
+
+Packaging
+---------
+
+Downstream packagers, if incorporating testing into their packaging, are
+encouraged to use only the tests in the test_deterministic.py module, to
+avoid testing failures that may arise due to the non-deterministic behavior
+of Hypothesis tests.
```

### Comparing `dbus-signature-pyparsing-0.4/tests/test_deterministic.py` & `dbus-signature-pyparsing-0.4.1/tests/test_deterministic.py`

 * *Files identical despite different names*

### Comparing `dbus-signature-pyparsing-0.4/tests/test_hypothesis.py` & `dbus-signature-pyparsing-0.4.1/tests/test_hypothesis.py`

 * *Files identical despite different names*

