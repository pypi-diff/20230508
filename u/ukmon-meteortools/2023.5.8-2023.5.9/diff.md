# Comparing `tmp/ukmon_meteortools-2023.5.8.tar.gz` & `tmp/ukmon_meteortools-2023.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukmon_meteortools-2023.5.8.tar", last modified: Sun May  7 14:40:23 2023, max compression
+gzip compressed data, was "ukmon_meteortools-2023.5.9.tar", last modified: Sun May  7 16:50:16 2023, max compression
```

## Comparing `ukmon_meteortools-2023.5.8.tar` & `ukmon_meteortools-2023.5.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 14:40:23.810953 ukmon_meteortools-2023.5.8/
--rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.5.8/LICENSE
--rw-rw-rw-   0        0        0    42725 2023-05-07 14:40:23.806938 ukmon_meteortools-2023.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.5.8/README.md
--rw-rw-rw-   0        0        0     2364 2023-05-07 14:39:47.000000 ukmon_meteortools-2023.5.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 14:40:23.810953 ukmon_meteortools-2023.5.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-07 14:40:23.577939 ukmon_meteortools-2023.5.8/ukmon_meteortools/
--rw-rw-rw-   0        0        0      819 2023-05-07 12:44:14.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 14:40:23.676939 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/
--rw-rw-rw-   0        0        0     2043 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/ECSVhandler.py
--rw-rw-rw-   0        0        0     8691 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/UFOAnalyzerXML.py
--rw-rw-rw-   0        0        0     6742 2023-05-02 20:41:44.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/UFOCapXML.py
--rw-rw-rw-   0        0        0      520 2023-05-04 19:41:10.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/__init__.py
--rw-rw-rw-   0        0        0    18716 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/ftpDetectInfo.py
--rw-rw-rw-   0        0        0     7393 2023-05-02 21:34:25.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/imoWorkingShowerList.py
--rw-rw-rw-   0        0        0     4018 2023-05-05 17:15:20.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/kmlHandlers.py
--rw-rw-rw-   0        0        0     2815 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/platepar.py
-drwxrwxrwx   0        0        0        0 2023-05-07 14:40:23.712940 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/
--rw-rw-rw-   0        0        0      733 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/__init__.py
--rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
--rw-rw-rw-   0        0        0     6077 2023-05-05 15:40:18.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/multiDayRadiant.py
--rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/multiEventGroundMap.py
--rw-rw-rw-   0        0        0     5242 2023-05-05 16:20:15.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/multiTrackStack.py
--rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
--rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/plotRMSOrbits.py
--rw-rw-rw-   0        0        0     3187 2023-05-05 17:16:29.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/trajPickle.py
-drwxrwxrwx   0        0        0        0 2023-05-07 14:40:23.718939 ukmon_meteortools-2023.5.8/ukmon_meteortools/share/
--rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
--rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/share/__init__.py
--rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/share/streamfulldata.npy
-drwxrwxrwx   0        0        0        0 2023-05-07 14:40:23.769945 ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/
--rw-rw-rw-   0        0        0      444 2023-05-04 19:36:38.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/__init__.py
--rw-rw-rw-   0        0        0     3164 2023-05-06 20:43:49.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/apiExampleCode.py
--rw-rw-rw-   0        0        0     1420 2023-03-08 12:49:12.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/findNearDuplicates.py
--rw-rw-rw-   0        0        0     4298 2023-05-06 21:27:34.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/getLiveImages.py
--rw-rw-rw-   0        0        0     3085 2023-05-06 21:17:26.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/getOverlappingFovs.py
--rw-rw-rw-   0        0        0     3429 2023-05-06 20:51:39.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/plotTrack.py
-drwxrwxrwx   0        0        0        0 2023-05-07 14:40:23.804949 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/
--rw-rw-rw-   0        0        0    13798 2023-05-02 20:57:25.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/Math.py
--rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/VectorMaths.py
--rw-rw-rw-   0        0        0     1296 2023-05-04 20:12:42.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/__init__.py
--rw-rw-rw-   0        0        0     2519 2023-05-02 21:35:02.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/annotateImage.py
--rw-rw-rw-   0        0        0     1313 2023-05-02 21:35:22.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/convertSolLon.py
--rw-rw-rw-   0        0        0     2393 2023-05-07 12:29:44.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/drawFTPfile.py
--rw-rw-rw-   0        0        0     2105 2023-05-07 14:36:01.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/getActiveShowers.py
--rw-rw-rw-   0        0        0     3937 2023-05-02 21:41:36.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/getShowerDates.py
--rw-rw-rw-   0        0        0     3699 2023-05-02 20:49:10.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/sendAnEmail.py
-drwxrwxrwx   0        0        0        0 2023-05-07 14:40:23.646941 ukmon_meteortools-2023.5.8/ukmon_meteortools.egg-info/
--rw-rw-rw-   0        0        0    42725 2023-05-07 14:40:23.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1752 2023-05-07 14:40:23.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 14:40:23.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      353 2023-05-07 14:40:23.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-07 14:40:23.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 16:50:16.796562 ukmon_meteortools-2023.5.9/
+-rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.5.9/LICENSE
+-rw-rw-rw-   0        0        0    42725 2023-05-07 16:50:16.794560 ukmon_meteortools-2023.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.5.9/README.md
+-rw-rw-rw-   0        0        0     2364 2023-05-07 16:49:51.000000 ukmon_meteortools-2023.5.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 16:50:16.796562 ukmon_meteortools-2023.5.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 16:50:16.678143 ukmon_meteortools-2023.5.9/ukmon_meteortools/
+-rw-rw-rw-   0        0        0      819 2023-05-07 12:44:14.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 16:50:16.717153 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/
+-rw-rw-rw-   0        0        0     2043 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/ECSVhandler.py
+-rw-rw-rw-   0        0        0     8691 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/UFOAnalyzerXML.py
+-rw-rw-rw-   0        0        0     6742 2023-05-02 20:41:44.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/UFOCapXML.py
+-rw-rw-rw-   0        0        0      520 2023-05-04 19:41:10.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/__init__.py
+-rw-rw-rw-   0        0        0    18716 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/ftpDetectInfo.py
+-rw-rw-rw-   0        0        0     7393 2023-05-02 21:34:25.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/imoWorkingShowerList.py
+-rw-rw-rw-   0        0        0     4018 2023-05-05 17:15:20.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/kmlHandlers.py
+-rw-rw-rw-   0        0        0     2815 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/platepar.py
+drwxrwxrwx   0        0        0        0 2023-05-07 16:50:16.736412 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/
+-rw-rw-rw-   0        0        0      733 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/__init__.py
+-rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
+-rw-rw-rw-   0        0        0     6077 2023-05-05 15:40:18.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/multiDayRadiant.py
+-rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/multiEventGroundMap.py
+-rw-rw-rw-   0        0        0     5242 2023-05-05 16:20:15.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/multiTrackStack.py
+-rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
+-rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/plotRMSOrbits.py
+-rw-rw-rw-   0        0        0     3187 2023-05-05 17:16:29.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/trajPickle.py
+drwxrwxrwx   0        0        0        0 2023-05-07 16:50:16.743045 ukmon_meteortools-2023.5.9/ukmon_meteortools/share/
+-rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
+-rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/share/__init__.py
+-rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/share/streamfulldata.npy
+drwxrwxrwx   0        0        0        0 2023-05-07 16:50:16.766560 ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/
+-rw-rw-rw-   0        0        0      444 2023-05-04 19:36:38.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/__init__.py
+-rw-rw-rw-   0        0        0     3164 2023-05-06 20:43:49.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/apiExampleCode.py
+-rw-rw-rw-   0        0        0     1420 2023-03-08 12:49:12.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/findNearDuplicates.py
+-rw-rw-rw-   0        0        0     4298 2023-05-06 21:27:34.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/getLiveImages.py
+-rw-rw-rw-   0        0        0     3085 2023-05-06 21:17:26.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/getOverlappingFovs.py
+-rw-rw-rw-   0        0        0     3429 2023-05-06 20:51:39.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/plotTrack.py
+drwxrwxrwx   0        0        0        0 2023-05-07 16:50:16.793561 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/
+-rw-rw-rw-   0        0        0    13798 2023-05-02 20:57:25.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/Math.py
+-rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/VectorMaths.py
+-rw-rw-rw-   0        0        0     1296 2023-05-04 20:12:42.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/__init__.py
+-rw-rw-rw-   0        0        0     2519 2023-05-02 21:35:02.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/annotateImage.py
+-rw-rw-rw-   0        0        0     1313 2023-05-02 21:35:22.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/convertSolLon.py
+-rw-rw-rw-   0        0        0     2393 2023-05-07 12:29:44.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/drawFTPfile.py
+-rw-rw-rw-   0        0        0     2042 2023-05-07 16:17:45.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/getActiveShowers.py
+-rw-rw-rw-   0        0        0     4125 2023-05-07 16:11:20.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/getShowerDates.py
+-rw-rw-rw-   0        0        0     3699 2023-05-02 20:49:10.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/sendAnEmail.py
+drwxrwxrwx   0        0        0        0 2023-05-07 16:50:16.704144 ukmon_meteortools-2023.5.9/ukmon_meteortools.egg-info/
+-rw-rw-rw-   0        0        0    42725 2023-05-07 16:50:16.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1752 2023-05-07 16:50:16.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 16:50:16.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      353 2023-05-07 16:50:16.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-07 16:50:16.000000 ukmon_meteortools-2023.5.9/ukmon_meteortools.egg-info/top_level.txt
```

### Comparing `ukmon_meteortools-2023.5.8/LICENSE` & `ukmon_meteortools-2023.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/PKG-INFO` & `ukmon_meteortools-2023.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon_meteortools
-Version: 2023.5.8
+Version: 2023.5.9
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ukmon_meteortools-2023.5.8/README.md` & `ukmon_meteortools-2023.5.9/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/pyproject.toml` & `ukmon_meteortools-2023.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ukmon_meteortools"
-version = "2023.05.8"
+version = "2023.05.9"
 description = "Python Tools for Meteor Data Analysis"
 readme = "ukmon_meteortools/README.md"
 authors = [{ name = "Mark McIntyre", email = "ukmon@markmcintyreastro.co.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -72,15 +72,15 @@
 #[tool.setuptools.packages.find]
 #where = ["ukmon_meteortools"]
 
 [tool.setuptools.package-data]
 "*" = ["*.npy", "*.xml"]
 
 [tool.bumpver]
-current_version = "2023.05.8"
+current_version = "2023.05.9"
 version_pattern = "YYYY.0M.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/README.md` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/ECSVhandler.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/ECSVhandler.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/UFOAnalyzerXML.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/UFOAnalyzerXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/UFOCapXML.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/UFOCapXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/__init__.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/ftpDetectInfo.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/ftpDetectInfo.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/imoWorkingShowerList.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/imoWorkingShowerList.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/kmlHandlers.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/kmlHandlers.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/platepar.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/fileformats/platepar.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/__init__.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/multiDayRadiant.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/multiDayRadiant.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/multiEventGroundMap.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/multiEventGroundMap.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/multiTrackStack.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/multiTrackStack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/plotCAMSOrbits.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/plotCAMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/plotRMSOrbits.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/plotRMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/trajPickle.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/rmsutils/trajPickle.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/share/__init__.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/share/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/share/streamfulldata.npy` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/share/streamfulldata.npy`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/apiExampleCode.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/apiExampleCode.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/findNearDuplicates.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/findNearDuplicates.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/getLiveImages.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/getLiveImages.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/getOverlappingFovs.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/getOverlappingFovs.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/plotTrack.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/usertools/plotTrack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/Math.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/Math.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/VectorMaths.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/VectorMaths.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/__init__.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/annotateImage.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/annotateImage.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/convertSolLon.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/convertSolLon.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/drawFTPfile.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/drawFTPfile.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/getActiveShowers.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/getActiveShowers.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,16 +39,15 @@
     Arguments:  
         targdate:   [str] Date in YYYYMMDD format  
 
     Returns:  
         nothing  
 
     """
-    targdate = datetime.datetime.strptime(targdatestr, '%Y%m%d')
-    shwrs = getActiveShowers(targdate, retlist=True)
+    shwrs = getActiveShowers(targdatestr, retlist=True)
     shwrs.append('spo')
     for s in shwrs:
         print(s)
 
 
 if __name__ == '__main__':
     arg_parser = argparse.ArgumentParser(description='get list of active showers',
```

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/getShowerDates.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/getShowerDates.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,38 +72,42 @@
             pth = 'e:/dev/meteorhunting/WesternMeteorPyLib/wmpl/share'
         else:
             pth = '/home/ec2-user/src/WesternMeteorPyLib/wmpl/share'
     dfil = np.load(os.path.join(pth, fname))
     return dfil
 
 
-def getShowerDets(shwr):
+def getShowerDets(shwr, stringFmt=False):
     """ Get details of a shower 
     
     Arguments:  
         shwr:   [string] three-letter shower code eg PER  
          
     Returns:  
         (id, full name, peak solar longitude, peak date mm-dd)  
     """
     sfd = _loadFullData()
     sfdfltr = sfd[sfd[:,3] == shwr]
     mtch = [sh for sh in sfdfltr if sh[6] != '-2']
-    if len(mtch) == 0:
-        return 0, 'Unknown', 0, 'Unknown'
-
-    id = int(mtch[-1][1])
-    nam = mtch[-1][4].strip()
-    pksollong = float(mtch[-1][7])
-    dt = datetime.datetime.now()
-    yr = dt.year
-    mth = dt.month
-    jd = sollon2jd(yr, mth, pksollong)
-    pkdt = jd2Date(jd, dt_obj=True)
-    return id, nam, pksollong, pkdt.strftime('%m-%d')
+    if len(mtch) > 0:
+        id = int(mtch[-1][1])
+        nam = mtch[-1][4].strip()
+        pksollong = float(mtch[-1][7])
+        dt = datetime.datetime.now()
+        yr = dt.year
+        mth = dt.month
+        jd = sollon2jd(yr, mth, pksollong)
+        pkdt = jd2Date(jd, dt_obj=True)
+        dtstr = pkdt.strftime('%m-%d')
+    else:
+        id, nam, pksollong, dtstr = 0, 'Unknown', 0, 'Unknown'
+    if stringFmt:
+        return f"{pksollong},'{dtstr}','{nam}',{shwr}"
+    else:
+        return id, nam, pksollong, dtstr
 
 
 def getShowerPeak(shwr):
     """ Get date of a shower peak in MM-DD format
     
     Arguments:  
         shwr:   [string] three-letter shower code eg PER  
@@ -111,14 +115,15 @@
     Returns:  
         peak date mm-dd  
     """
     _, _, _, pk = getShowerDets(shwr)
     return pk
 
  
+
 if __name__ == '__main__':
     if sys.argv[1] == 'refresh':
         _refreshShowerData()
         exit(0)
     else:
         id, nam, sl, dt = getShowerDets(sys.argv[1])
         print('{},{},{},{}'.format(sl, dt, nam, sys.argv[1]))
```

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/sendAnEmail.py` & `ukmon_meteortools-2023.5.9/ukmon_meteortools/utils/sendAnEmail.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools.egg-info/PKG-INFO` & `ukmon_meteortools-2023.5.9/ukmon_meteortools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon-meteortools
-Version: 2023.5.8
+Version: 2023.5.9
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ukmon_meteortools-2023.5.8/ukmon_meteortools.egg-info/SOURCES.txt` & `ukmon_meteortools-2023.5.9/ukmon_meteortools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

