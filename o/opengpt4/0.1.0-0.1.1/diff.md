# Comparing `tmp/opengpt4-0.1.0.tar.gz` & `tmp/opengpt4-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengpt4-0.1.0.tar", max compression
+gzip compressed data, was "opengpt4-0.1.1.tar", max compression
```

## Comparing `opengpt4-0.1.0.tar` & `opengpt4-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-05-08 03:29:15.649838 opengpt4-0.1.0/LICENSE
--rw-r--r--   0        0        0     4537 2023-05-08 03:29:15.649838 opengpt4-0.1.0/README.md
--rw-r--r--   0        0        0     1097 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/README.md
--rw-r--r--   0        0        0      896 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/chatbase/DOC.md
--rw-r--r--   0        0        0      497 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/chatbase/README.md
--rw-r--r--   0        0        0     5337 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/chatbase/model.py
--rw-r--r--   0        0        0      679 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/chatgptproxy/DOC.md
--rw-r--r--   0        0        0      533 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/chatgptproxy/README.md
--rw-r--r--   0        0        0     2444 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/chatgptproxy/model.py
--rw-r--r--   0        0        0      654 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/chatllama/DOC.md
--rw-r--r--   0        0        0      467 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/chatllama/README.md
--rw-r--r--   0        0        0     1175 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/chatllama/model.py
--rw-r--r--   0        0        0     6905 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/forefront/DOC.md
--rw-r--r--   0        0        0     6558 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/forefront/README.md
--rw-r--r--   0        0        0     3675 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/forefront/attributes/conversation.py
--rw-r--r--   0        0        0     6620 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/forefront/model.py
--rw-r--r--   0        0        0     2836 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/forefront/tools/system/email_creation.py
--rw-r--r--   0        0        0      673 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/forefront/tools/system/signature.py
--rw-r--r--   0        0        0     1744 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/forefront/tools/system/tempmail.py
--rw-r--r--   0        0        0      464 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/forefront/tools/typing/response.py
--rw-r--r--   0        0        0     1020 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/italygpt/DOC.md
--rw-r--r--   0        0        0      624 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/italygpt/README.md
--rw-r--r--   0        0        0     2071 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/italygpt/model.py
--rw-r--r--   0        0        0     1206 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/usesless/DOC.md
--rw-r--r--   0        0        0      768 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/usesless/README.md
--rw-r--r--   0        0        0     1614 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/usesless/model.py
--rw-r--r--   0        0        0      435 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/usesless/tools/typing/response.py
--rw-r--r--   0        0        0     1142 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/you/DOC.md
--rw-r--r--   0        0        0     1991 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/you/README.md
--rw-r--r--   0        0        0     3642 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/you/model.py
--rw-r--r--   0        0        0      538 2023-05-08 03:29:15.649838 opengpt4-0.1.0/models/you/tools/typing/response.py
--rw-r--r--   0        0        0      397 2023-05-08 03:29:15.649838 opengpt4-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5226 1970-01-01 00:00:00.000000 opengpt4-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-08 04:45:12.990846 opengpt4-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4537 2023-05-08 04:45:12.990846 opengpt4-0.1.1/README.md
+-rw-r--r--   0        0        0     1097 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/README.md
+-rw-r--r--   0        0        0      896 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/chatbase/DOC.md
+-rw-r--r--   0        0        0      497 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/chatbase/README.md
+-rw-r--r--   0        0        0     5337 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/chatbase/model.py
+-rw-r--r--   0        0        0      679 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/chatgptproxy/DOC.md
+-rw-r--r--   0        0        0      533 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/chatgptproxy/README.md
+-rw-r--r--   0        0        0     2444 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/chatgptproxy/model.py
+-rw-r--r--   0        0        0      654 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/chatllama/DOC.md
+-rw-r--r--   0        0        0      467 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/chatllama/README.md
+-rw-r--r--   0        0        0     1175 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/chatllama/model.py
+-rw-r--r--   0        0        0     6905 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/forefront/DOC.md
+-rw-r--r--   0        0        0     6558 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/forefront/README.md
+-rw-r--r--   0        0        0     3675 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/forefront/attributes/conversation.py
+-rw-r--r--   0        0        0     6620 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/forefront/model.py
+-rw-r--r--   0        0        0     2836 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/forefront/tools/system/email_creation.py
+-rw-r--r--   0        0        0      673 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/forefront/tools/system/signature.py
+-rw-r--r--   0        0        0     1744 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/forefront/tools/system/tempmail.py
+-rw-r--r--   0        0        0      464 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/forefront/tools/typing/response.py
+-rw-r--r--   0        0        0     1020 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/italygpt/DOC.md
+-rw-r--r--   0        0        0      624 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/italygpt/README.md
+-rw-r--r--   0        0        0     2071 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/italygpt/model.py
+-rw-r--r--   0        0        0     1206 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/usesless/DOC.md
+-rw-r--r--   0        0        0      768 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/usesless/README.md
+-rw-r--r--   0        0        0     1614 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/usesless/model.py
+-rw-r--r--   0        0        0      435 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/usesless/tools/typing/response.py
+-rw-r--r--   0        0        0     1142 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/you/DOC.md
+-rw-r--r--   0        0        0     1991 2023-05-08 04:45:12.990846 opengpt4-0.1.1/opengpt/you/README.md
+-rw-r--r--   0        0        0     3642 2023-05-08 04:45:12.994846 opengpt4-0.1.1/opengpt/you/model.py
+-rw-r--r--   0        0        0      538 2023-05-08 04:45:12.994846 opengpt4-0.1.1/opengpt/you/tools/typing/response.py
+-rw-r--r--   0        0        0      398 2023-05-08 04:45:12.994846 opengpt4-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5226 1970-01-01 00:00:00.000000 opengpt4-0.1.1/PKG-INFO
```

### Comparing `opengpt4-0.1.0/LICENSE` & `opengpt4-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/README.md` & `opengpt4-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/README.md` & `opengpt4-0.1.1/opengpt/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/chatbase/DOC.md` & `opengpt4-0.1.1/opengpt/chatbase/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/chatbase/model.py` & `opengpt4-0.1.1/opengpt/chatbase/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/chatgptproxy/DOC.md` & `opengpt4-0.1.1/opengpt/chatgptproxy/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/chatgptproxy/README.md` & `opengpt4-0.1.1/opengpt/chatgptproxy/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/chatgptproxy/model.py` & `opengpt4-0.1.1/opengpt/chatgptproxy/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/chatllama/DOC.md` & `opengpt4-0.1.1/opengpt/chatllama/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/chatllama/model.py` & `opengpt4-0.1.1/opengpt/chatllama/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/forefront/DOC.md` & `opengpt4-0.1.1/opengpt/forefront/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/forefront/README.md` & `opengpt4-0.1.1/opengpt/forefront/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/forefront/attributes/conversation.py` & `opengpt4-0.1.1/opengpt/forefront/attributes/conversation.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/forefront/model.py` & `opengpt4-0.1.1/opengpt/forefront/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/forefront/tools/system/email_creation.py` & `opengpt4-0.1.1/opengpt/forefront/tools/system/email_creation.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/forefront/tools/system/signature.py` & `opengpt4-0.1.1/opengpt/forefront/tools/system/signature.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/forefront/tools/system/tempmail.py` & `opengpt4-0.1.1/opengpt/forefront/tools/system/tempmail.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/italygpt/DOC.md` & `opengpt4-0.1.1/opengpt/italygpt/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/italygpt/README.md` & `opengpt4-0.1.1/opengpt/italygpt/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/italygpt/model.py` & `opengpt4-0.1.1/opengpt/italygpt/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/usesless/DOC.md` & `opengpt4-0.1.1/opengpt/usesless/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/usesless/README.md` & `opengpt4-0.1.1/opengpt/usesless/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/usesless/model.py` & `opengpt4-0.1.1/opengpt/usesless/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/you/DOC.md` & `opengpt4-0.1.1/opengpt/you/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/you/README.md` & `opengpt4-0.1.1/opengpt/you/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/you/model.py` & `opengpt4-0.1.1/opengpt/you/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/models/you/tools/typing/response.py` & `opengpt4-0.1.1/opengpt/you/tools/typing/response.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.0/PKG-INFO` & `opengpt4-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengpt4
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: GPL-3.0
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

