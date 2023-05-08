# Comparing `tmp/oglio-0.7.2.tar.gz` & `tmp/oglio-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oglio-0.7.2.tar", last modified: Tue Apr 18 13:25:02 2023, max compression
+gzip compressed data, was "oglio-0.7.3.tar", last modified: Mon May  8 18:43:51 2023, max compression
```

## Comparing `oglio-0.7.2.tar` & `oglio-0.7.3.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 13:25:02.229397 oglio-0.7.2/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-20 17:57:30.000000 oglio-0.7.2/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2335 2023-04-18 13:25:02.229281 oglio-0.7.2/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2011 2023-04-13 20:29:58.000000 oglio-0.7.2/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 13:25:02.225309 oglio-0.7.2/oglio/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       82 2023-02-13 18:01:45.000000 oglio-0.7.2/oglio/OglVersion.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4580 2023-02-13 18:12:30.000000 oglio-0.7.2/oglio/Reader.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3826 2023-01-01 21:43:45.000000 oglio-0.7.2/oglio/Types.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      123 2022-10-13 12:50:37.000000 oglio-0.7.2/oglio/UnsupportedFileTypeException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2111 2022-10-13 16:59:06.000000 oglio-0.7.2/oglio/Writer.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-09 17:46:52.000000 oglio-0.7.2/oglio/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-07 19:55:58.000000 oglio-0.7.2/oglio/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 13:25:02.229150 oglio-0.7.2/oglio/toXmlV10/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1913 2022-08-26 20:55:45.000000 oglio-0.7.2/oglio/toXmlV10/BaseOglToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      569 2022-08-26 20:55:45.000000 oglio-0.7.2/oglio/toXmlV10/BasePyutToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1103 2023-03-30 23:17:17.000000 oglio-0.7.2/oglio/toXmlV10/BaseToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1646 2022-08-29 20:41:51.000000 oglio-0.7.2/oglio/toXmlV10/OglClassesToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5803 2023-03-22 15:11:37.000000 oglio-0.7.2/oglio/toXmlV10/OglLinksToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1598 2022-08-29 20:41:51.000000 oglio-0.7.2/oglio/toXmlV10/OglNotesToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2622 2023-02-12 20:42:00.000000 oglio-0.7.2/oglio/toXmlV10/OglSequenceToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1569 2022-08-29 20:41:51.000000 oglio-0.7.2/oglio/toXmlV10/OglTextsToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6676 2022-10-13 16:38:44.000000 oglio-0.7.2/oglio/toXmlV10/OglToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2787 2022-08-29 20:41:51.000000 oglio-0.7.2/oglio/toXmlV10/OglUseCasesToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14132 2023-04-16 20:48:23.000000 oglio-0.7.2/oglio/toXmlV10/PyutToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3831 2022-08-19 17:25:32.000000 oglio-0.7.2/oglio/toXmlV10/XmlConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-16 17:46:46.000000 oglio-0.7.2/oglio/toXmlV10/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-07 19:55:58.000000 oglio-0.7.2/oglio/toXmlV10/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 13:25:02.225965 oglio-0.7.2/oglio.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2335 2023-04-18 13:25:02.000000 oglio-0.7.2/oglio.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      736 2023-04-18 13:25:02.000000 oglio-0.7.2/oglio.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-18 13:25:02.000000 oglio-0.7.2/oglio.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      105 2023-04-18 13:25:02.000000 oglio-0.7.2/oglio.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        6 2023-04-18 13:25:02.000000 oglio-0.7.2/oglio.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-18 13:25:02.229428 oglio-0.7.2/setup.cfg
--rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)      964 2023-04-18 13:21:16.000000 oglio-0.7.2/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 18:43:51.959169 oglio-0.7.3/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-20 17:57:30.000000 oglio-0.7.3/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2335 2023-05-08 18:43:51.959044 oglio-0.7.3/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2011 2023-04-13 20:29:58.000000 oglio-0.7.3/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 18:43:51.955482 oglio-0.7.3/oglio/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1009 2023-05-08 00:20:50.000000 oglio-0.7.3/oglio/IDFactory.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       82 2023-02-13 18:01:45.000000 oglio-0.7.3/oglio/OglVersion.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4580 2023-05-06 14:32:39.000000 oglio-0.7.3/oglio/Reader.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3826 2023-05-06 14:32:39.000000 oglio-0.7.3/oglio/Types.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      123 2022-10-13 12:50:37.000000 oglio-0.7.3/oglio/UnsupportedFileTypeException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2111 2023-05-06 14:32:39.000000 oglio-0.7.3/oglio/Writer.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-09 17:46:52.000000 oglio-0.7.3/oglio/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-07 19:55:58.000000 oglio-0.7.3/oglio/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 18:43:51.958899 oglio-0.7.3/oglio/toXmlV10/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1913 2023-05-06 19:50:19.000000 oglio-0.7.3/oglio/toXmlV10/BaseOglToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      569 2022-08-26 20:55:45.000000 oglio-0.7.3/oglio/toXmlV10/BasePyutToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-05-08 00:21:01.000000 oglio-0.7.3/oglio/toXmlV10/BaseToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1646 2023-05-06 19:50:36.000000 oglio-0.7.3/oglio/toXmlV10/OglClassesToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5803 2023-05-06 19:50:47.000000 oglio-0.7.3/oglio/toXmlV10/OglLinksToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1598 2023-05-06 19:51:01.000000 oglio-0.7.3/oglio/toXmlV10/OglNotesToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2622 2023-05-06 19:51:16.000000 oglio-0.7.3/oglio/toXmlV10/OglSequenceToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1569 2023-05-06 14:32:39.000000 oglio-0.7.3/oglio/toXmlV10/OglTextsToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6676 2023-05-06 14:32:39.000000 oglio-0.7.3/oglio/toXmlV10/OglToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2787 2023-05-06 19:51:31.000000 oglio-0.7.3/oglio/toXmlV10/OglUseCasesToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14155 2023-05-08 17:31:58.000000 oglio-0.7.3/oglio/toXmlV10/PyutToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3831 2022-08-19 17:25:32.000000 oglio-0.7.3/oglio/toXmlV10/XmlConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-16 17:46:46.000000 oglio-0.7.3/oglio/toXmlV10/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-07 19:55:58.000000 oglio-0.7.3/oglio/toXmlV10/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 18:43:51.956046 oglio-0.7.3/oglio.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2335 2023-05-08 18:43:51.000000 oglio-0.7.3/oglio.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      755 2023-05-08 18:43:51.000000 oglio-0.7.3/oglio.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-05-08 18:43:51.000000 oglio-0.7.3/oglio.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      105 2023-05-08 18:43:51.000000 oglio-0.7.3/oglio.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        6 2023-05-08 18:43:51.000000 oglio-0.7.3/oglio.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-08 18:43:51.959208 oglio-0.7.3/setup.cfg
+-rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)      964 2023-05-08 18:19:34.000000 oglio-0.7.3/setup.py
```

### Comparing `oglio-0.7.2/LICENSE` & `oglio-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oglio-0.7.2/PKG-INFO` & `oglio-0.7.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oglio
-Version: 0.7.2
+Version: 0.7.3
 Summary: External Pyut Persistence
 Home-page: https://github.com/hasii2011/oglio
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oglio Version: 0.7.2 Summary: External Pyut
+Metadata-Version: 2.1 Name: oglio Version: 0.7.3 Summary: External Pyut
 Persistence Home-page: https://github.com/hasii2011/oglio Author-email:
 Humberto.A.Sanchez.II@gmail.com Maintainer: Humberto A. Sanchez II Maintainer-
 email: humberto.a.sanchez.ii@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./docs/agpl-license-web-badge-version-2-256x48.png] [!
 [Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https:
 //GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![CircleCI](https://
 dl.circleci.com/status-badge/img/gh/hasii2011/oglio/tree/
```

### Comparing `oglio-0.7.2/README.md` & `oglio-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `oglio-0.7.2/oglio/Reader.py` & `oglio-0.7.3/oglio/Reader.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.2/oglio/Types.py` & `oglio-0.7.3/oglio/Types.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.2/oglio/Writer.py` & `oglio-0.7.3/oglio/Writer.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.2/oglio/toXmlV10/BaseOglToDom.py` & `oglio-0.7.3/oglio/toXmlV10/BaseOglToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.2/oglio/toXmlV10/BasePyutToDom.py` & `oglio-0.7.3/oglio/toXmlV10/BasePyutToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.2/oglio/toXmlV10/BaseToDom.py` & `oglio-0.7.3/oglio/IDFactory.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,7 @@
         if cls in self._classCache:
             return self._classCache[cls]
         else:
             clsId = IDFactory.nextID
             self._classCache[cls] = clsId
             IDFactory.nextID += 1
             return clsId
-
-
-class BaseToDom:
-
-    def __init__(self):
-
-        self._idFactory: IDFactory = IDFactory()
```

### Comparing `oglio-0.7.2/oglio/toXmlV10/OglClassesToDom.py` & `oglio-0.7.3/oglio/toXmlV10/OglClassesToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.2/oglio/toXmlV10/OglLinksToDom.py` & `oglio-0.7.3/oglio/toXmlV10/OglLinksToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.2/oglio/toXmlV10/OglNotesToDom.py` & `oglio-0.7.3/oglio/toXmlV10/OglNotesToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.2/oglio/toXmlV10/OglSequenceToDom.py` & `oglio-0.7.3/oglio/toXmlV10/OglSequenceToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.2/oglio/toXmlV10/OglTextsToDom.py` & `oglio-0.7.3/oglio/toXmlV10/OglTextsToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.2/oglio/toXmlV10/OglToDom.py` & `oglio-0.7.3/oglio/toXmlV10/OglToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.2/oglio/toXmlV10/OglUseCasesToDom.py` & `oglio-0.7.3/oglio/toXmlV10/OglUseCasesToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.2/oglio/toXmlV10/PyutToDom.py` & `oglio-0.7.3/oglio/toXmlV10/PyutToDom.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     def pyutTextToDom(self, pyutText: PyutText, xmlDoc: Document) -> Element:
 
         root: Element = xmlDoc.createElement(XmlConstants.ELEMENT_MODEL_TEXT)
         textId: int = self._idFactory.getID(pyutText)
 
         root.setAttribute(XmlConstants.ATTR_ID, str(textId))
         content: str = pyutText.content
-        content = content.replace('\n', "\\\\\\\\")
+        content = content.replace(osLineSep, PyutToDom.END_OF_LINE_MARKER)
 
         root.setAttribute(XmlConstants.ATTR_CONTENT, content)
 
         return root
 
     def pyutUseCaseToDom(self, pyutUseCase: PyutUseCase, xmlDoc: Document) -> Element:
         """
```

### Comparing `oglio-0.7.2/oglio/toXmlV10/XmlConstants.py` & `oglio-0.7.3/oglio/toXmlV10/XmlConstants.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.2/oglio.egg-info/PKG-INFO` & `oglio-0.7.3/oglio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oglio
-Version: 0.7.2
+Version: 0.7.3
 Summary: External Pyut Persistence
 Home-page: https://github.com/hasii2011/oglio
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oglio Version: 0.7.2 Summary: External Pyut
+Metadata-Version: 2.1 Name: oglio Version: 0.7.3 Summary: External Pyut
 Persistence Home-page: https://github.com/hasii2011/oglio Author-email:
 Humberto.A.Sanchez.II@gmail.com Maintainer: Humberto A. Sanchez II Maintainer-
 email: humberto.a.sanchez.ii@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./docs/agpl-license-web-badge-version-2-256x48.png] [!
 [Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https:
 //GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![CircleCI](https://
 dl.circleci.com/status-badge/img/gh/hasii2011/oglio/tree/
```

### Comparing `oglio-0.7.2/oglio.egg-info/SOURCES.txt` & `oglio-0.7.3/oglio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 setup.py
+oglio/IDFactory.py
 oglio/OglVersion.py
 oglio/Reader.py
 oglio/Types.py
 oglio/UnsupportedFileTypeException.py
 oglio/Writer.py
 oglio/__init__.py
 oglio/py.typed
```

### Comparing `oglio-0.7.2/setup.py` & `oglio-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 LICENSE = (HERE / 'LICENSE').read_text()
 
 setup(
     name="oglio",
-    version="0.7.2",
+    version="0.7.3",
     author_email='Humberto.A.Sanchez.II@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='External Pyut Persistence',
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/hasii2011/oglio",
@@ -27,10 +27,10 @@
     },
     install_requires=[
         'wxPython==4.2.0',
         'hasiihelper~=0.2.0',
         'hasiicommon~=0.2.2',
         'pyutmodel~=1.4.3',
         'ogl~=0.70.26',
-        'untanglepyut~=0.6.56',
+        'untanglepyut~=0.6.58',
     ],
 )
```

