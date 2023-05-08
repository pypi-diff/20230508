# Comparing `tmp/Fred-Frechet-1.9.8.tar.gz` & `tmp/Fred-Frechet-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fred-Frechet-1.9.8.tar", last modified: Wed Sep 15 09:29:42 2021, max compression
+gzip compressed data, was "Fred-Frechet-1.9.9.tar", last modified: Sun Nov 21 10:49:50 2021, max compression
```

## Comparing `Fred-Frechet-1.9.8.tar` & `Fred-Frechet-1.9.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 glamr     (1000) glamr     (1000)        0 2021-09-15 09:29:42.690752 Fred-Frechet-1.9.8/
--rw-r--r--   0 glamr     (1000) glamr     (1000)       86 2021-08-20 18:12:58.000000 Fred-Frechet-1.9.8/.gitmodules
--rw-r--r--   0 glamr     (1000) glamr     (1000)     1723 2021-09-02 12:39:09.000000 Fred-Frechet-1.9.8/CMakeLists.txt
-drwxr-xr-x   0 glamr     (1000) glamr     (1000)        0 2021-09-15 09:29:42.687419 Fred-Frechet-1.9.8/Fred/
--rw-r--r--   0 glamr     (1000) glamr     (1000)     2391 2021-09-02 13:03:47.000000 Fred-Frechet-1.9.8/Fred/__init__.py
--rw-r--r--   0 glamr     (1000) glamr     (1000)     4899 2021-08-20 17:44:04.000000 Fred-Frechet-1.9.8/Fred/hd_fs.py
--rw-r--r--   0 glamr     (1000) glamr     (1000)     1724 2021-08-20 17:44:04.000000 Fred-Frechet-1.9.8/Fred/median.py
-drwxr-xr-x   0 glamr     (1000) glamr     (1000)        0 2021-09-15 09:29:42.687419 Fred-Frechet-1.9.8/Fred_Frechet.egg-info/
--rw-r--r--   0 glamr     (1000) glamr     (1000)    11073 2021-09-15 09:29:42.000000 Fred-Frechet-1.9.8/Fred_Frechet.egg-info/PKG-INFO
--rw-r--r--   0 glamr     (1000) glamr     (1000)      871 2021-09-15 09:29:42.000000 Fred-Frechet-1.9.8/Fred_Frechet.egg-info/SOURCES.txt
--rw-r--r--   0 glamr     (1000) glamr     (1000)        1 2021-09-15 09:29:42.000000 Fred-Frechet-1.9.8/Fred_Frechet.egg-info/dependency_links.txt
--rw-r--r--   0 glamr     (1000) glamr     (1000)        1 2021-09-15 09:29:42.000000 Fred-Frechet-1.9.8/Fred_Frechet.egg-info/not-zip-safe
--rw-r--r--   0 glamr     (1000) glamr     (1000)       18 2021-09-15 09:29:42.000000 Fred-Frechet-1.9.8/Fred_Frechet.egg-info/requires.txt
--rw-r--r--   0 glamr     (1000) glamr     (1000)       13 2021-09-15 09:29:42.000000 Fred-Frechet-1.9.8/Fred_Frechet.egg-info/top_level.txt
--rw-r--r--   0 glamr     (1000) glamr     (1000)     1074 2021-08-27 12:08:51.000000 Fred-Frechet-1.9.8/LICENSE
--rw-r--r--   0 glamr     (1000) glamr     (1000)      124 2021-08-20 17:44:04.000000 Fred-Frechet-1.9.8/Makefile
--rw-r--r--   0 glamr     (1000) glamr     (1000)    11073 2021-09-15 09:29:42.690752 Fred-Frechet-1.9.8/PKG-INFO
--rw-r--r--   0 glamr     (1000) glamr     (1000)    10669 2021-09-07 08:01:08.000000 Fred-Frechet-1.9.8/README.md
-drwxr-xr-x   0 glamr     (1000) glamr     (1000)        0 2021-09-15 09:29:42.687419 Fred-Frechet-1.9.8/include/
--rw-r--r--   0 glamr     (1000) glamr     (1000)        8 2021-08-20 17:44:04.000000 Fred-Frechet-1.9.8/include/.gitignore
--rw-r--r--   0 glamr     (1000) glamr     (1000)     5779 2021-09-10 11:32:11.000000 Fred-Frechet-1.9.8/include/clustering.hpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     1223 2021-09-03 10:22:20.000000 Fred-Frechet-1.9.8/include/config.hpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     4224 2021-09-14 13:46:03.000000 Fred-Frechet-1.9.8/include/coreset.hpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     5895 2021-08-27 09:39:48.000000 Fred-Frechet-1.9.8/include/curve.hpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     1405 2021-08-20 17:44:04.000000 Fred-Frechet-1.9.8/include/dynamic_time_warping.hpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     2386 2021-09-03 06:41:30.000000 Fred-Frechet-1.9.8/include/frechet.hpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     2816 2021-08-27 09:10:46.000000 Fred-Frechet-1.9.8/include/grid.hpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     2257 2021-09-03 09:45:16.000000 Fred-Frechet-1.9.8/include/interval.hpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     1267 2021-08-27 09:11:17.000000 Fred-Frechet-1.9.8/include/jl_transform.hpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     8398 2021-09-03 09:22:31.000000 Fred-Frechet-1.9.8/include/point.hpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     3704 2021-08-30 11:35:18.000000 Fred-Frechet-1.9.8/include/random.hpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     5366 2021-09-03 10:20:46.000000 Fred-Frechet-1.9.8/include/simplification.hpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     1645 2021-09-03 09:43:12.000000 Fred-Frechet-1.9.8/include/types.hpp
-drwxr-xr-x   0 glamr     (1000) glamr     (1000)        0 2021-09-15 09:29:42.687419 Fred-Frechet-1.9.8/logo/
--rw-r--r--   0 glamr     (1000) glamr     (1000)    23054 2021-08-20 17:44:04.000000 Fred-Frechet-1.9.8/logo/logo.png
--rw-r--r--   0 glamr     (1000) glamr     (1000)   122225 2021-08-20 17:44:04.000000 Fred-Frechet-1.9.8/logo/logo.svg
--rw-r--r--   0 glamr     (1000) glamr     (1000)       38 2021-09-15 09:29:42.690752 Fred-Frechet-1.9.8/setup.cfg
--rw-r--r--   0 glamr     (1000) glamr     (1000)     3462 2021-09-15 09:11:29.000000 Fred-Frechet-1.9.8/setup.py
-drwxr-xr-x   0 glamr     (1000) glamr     (1000)        0 2021-09-15 09:29:42.690752 Fred-Frechet-1.9.8/src/
--rw-r--r--   0 glamr     (1000) glamr     (1000)        8 2021-08-20 17:44:04.000000 Fred-Frechet-1.9.8/src/.gitignore
--rw-r--r--   0 glamr     (1000) glamr     (1000)     9185 2021-09-15 08:27:30.000000 Fred-Frechet-1.9.8/src/clustering.cpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     1183 2021-09-03 10:22:02.000000 Fred-Frechet-1.9.8/src/config.cpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     5096 2021-08-30 10:47:00.000000 Fred-Frechet-1.9.8/src/curve.cpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     2516 2021-09-10 11:33:14.000000 Fred-Frechet-1.9.8/src/dynamic_time_warping.cpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)    12203 2021-09-10 11:28:41.000000 Fred-Frechet-1.9.8/src/frechet.cpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     8832 2021-09-15 07:00:30.000000 Fred-Frechet-1.9.8/src/fred_python_wrapper.cpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     1261 2021-08-27 09:30:48.000000 Fred-Frechet-1.9.8/src/interval.cpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     3299 2021-08-30 11:46:54.000000 Fred-Frechet-1.9.8/src/jl_transform.cpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     2124 2021-08-27 09:32:21.000000 Fred-Frechet-1.9.8/src/point.cpp
--rw-r--r--   0 glamr     (1000) glamr     (1000)     5332 2021-09-03 10:20:03.000000 Fred-Frechet-1.9.8/src/simplification.cpp
-drwxr-xr-x   0 glamr     (1000) glamr     (1000)        0 2021-09-15 09:29:42.690752 Fred-Frechet-1.9.8/test/
--rw-r--r--   0 glamr     (1000) glamr     (1000)     1793 2021-09-07 07:59:19.000000 Fred-Frechet-1.9.8/test/test.py
+drwxr-xr-x   0 glamr     (1000) glamr     (1000)        0 2021-11-21 10:49:50.288560 Fred-Frechet-1.9.9/
+-rw-r--r--   0 glamr     (1000) glamr     (1000)       86 2021-08-20 18:12:58.000000 Fred-Frechet-1.9.9/.gitmodules
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     1723 2021-09-02 12:39:09.000000 Fred-Frechet-1.9.9/CMakeLists.txt
+drwxr-xr-x   0 glamr     (1000) glamr     (1000)        0 2021-11-21 10:49:50.285226 Fred-Frechet-1.9.9/Fred/
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     2391 2021-09-02 13:03:47.000000 Fred-Frechet-1.9.9/Fred/__init__.py
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     4899 2021-08-20 17:44:04.000000 Fred-Frechet-1.9.9/Fred/hd_fs.py
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     1724 2021-08-20 17:44:04.000000 Fred-Frechet-1.9.9/Fred/median.py
+drwxr-xr-x   0 glamr     (1000) glamr     (1000)        0 2021-11-21 10:49:50.285226 Fred-Frechet-1.9.9/Fred_Frechet.egg-info/
+-rw-r--r--   0 glamr     (1000) glamr     (1000)    11073 2021-11-21 10:49:50.000000 Fred-Frechet-1.9.9/Fred_Frechet.egg-info/PKG-INFO
+-rw-r--r--   0 glamr     (1000) glamr     (1000)      871 2021-11-21 10:49:50.000000 Fred-Frechet-1.9.9/Fred_Frechet.egg-info/SOURCES.txt
+-rw-r--r--   0 glamr     (1000) glamr     (1000)        1 2021-11-21 10:49:50.000000 Fred-Frechet-1.9.9/Fred_Frechet.egg-info/dependency_links.txt
+-rw-r--r--   0 glamr     (1000) glamr     (1000)        1 2021-11-21 10:48:12.000000 Fred-Frechet-1.9.9/Fred_Frechet.egg-info/not-zip-safe
+-rw-r--r--   0 glamr     (1000) glamr     (1000)       18 2021-11-21 10:49:50.000000 Fred-Frechet-1.9.9/Fred_Frechet.egg-info/requires.txt
+-rw-r--r--   0 glamr     (1000) glamr     (1000)       13 2021-11-21 10:49:50.000000 Fred-Frechet-1.9.9/Fred_Frechet.egg-info/top_level.txt
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     1074 2021-08-27 12:08:51.000000 Fred-Frechet-1.9.9/LICENSE
+-rw-r--r--   0 glamr     (1000) glamr     (1000)      124 2021-08-20 17:44:04.000000 Fred-Frechet-1.9.9/Makefile
+-rw-r--r--   0 glamr     (1000) glamr     (1000)    11073 2021-11-21 10:49:50.285226 Fred-Frechet-1.9.9/PKG-INFO
+-rw-r--r--   0 glamr     (1000) glamr     (1000)    10669 2021-09-07 08:01:08.000000 Fred-Frechet-1.9.9/README.md
+drwxr-xr-x   0 glamr     (1000) glamr     (1000)        0 2021-11-21 10:49:50.285226 Fred-Frechet-1.9.9/include/
+-rw-r--r--   0 glamr     (1000) glamr     (1000)        8 2021-08-20 17:44:04.000000 Fred-Frechet-1.9.9/include/.gitignore
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     4550 2021-09-16 10:44:29.000000 Fred-Frechet-1.9.9/include/clustering.hpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     1223 2021-09-03 10:22:20.000000 Fred-Frechet-1.9.9/include/config.hpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     4154 2021-09-16 10:52:26.000000 Fred-Frechet-1.9.9/include/coreset.hpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     5895 2021-08-27 09:39:48.000000 Fred-Frechet-1.9.9/include/curve.hpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     1505 2021-11-17 13:47:10.000000 Fred-Frechet-1.9.9/include/dynamic_time_warping.hpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     2320 2021-09-16 10:50:42.000000 Fred-Frechet-1.9.9/include/frechet.hpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     2816 2021-08-27 09:10:46.000000 Fred-Frechet-1.9.9/include/grid.hpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     2257 2021-09-03 09:45:16.000000 Fred-Frechet-1.9.9/include/interval.hpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     1267 2021-08-27 09:11:17.000000 Fred-Frechet-1.9.9/include/jl_transform.hpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     8398 2021-09-03 09:22:31.000000 Fred-Frechet-1.9.9/include/point.hpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     3704 2021-08-30 11:35:18.000000 Fred-Frechet-1.9.9/include/random.hpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     5282 2021-09-16 10:29:55.000000 Fred-Frechet-1.9.9/include/simplification.hpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     1965 2021-09-16 10:55:32.000000 Fred-Frechet-1.9.9/include/types.hpp
+drwxr-xr-x   0 glamr     (1000) glamr     (1000)        0 2021-11-21 10:49:50.285226 Fred-Frechet-1.9.9/logo/
+-rw-r--r--   0 glamr     (1000) glamr     (1000)    23054 2021-08-20 17:44:04.000000 Fred-Frechet-1.9.9/logo/logo.png
+-rw-r--r--   0 glamr     (1000) glamr     (1000)   122225 2021-08-20 17:44:04.000000 Fred-Frechet-1.9.9/logo/logo.svg
+-rw-r--r--   0 glamr     (1000) glamr     (1000)       38 2021-11-21 10:49:50.288560 Fred-Frechet-1.9.9/setup.cfg
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     3462 2021-11-21 10:48:38.000000 Fred-Frechet-1.9.9/setup.py
+drwxr-xr-x   0 glamr     (1000) glamr     (1000)        0 2021-11-21 10:49:50.285226 Fred-Frechet-1.9.9/src/
+-rw-r--r--   0 glamr     (1000) glamr     (1000)        8 2021-08-20 17:44:04.000000 Fred-Frechet-1.9.9/src/.gitignore
+-rw-r--r--   0 glamr     (1000) glamr     (1000)    10599 2021-09-16 10:45:29.000000 Fred-Frechet-1.9.9/src/clustering.cpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     1183 2021-09-03 10:22:02.000000 Fred-Frechet-1.9.9/src/config.cpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     5096 2021-08-30 10:47:00.000000 Fred-Frechet-1.9.9/src/curve.cpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     5307 2021-11-18 12:59:07.000000 Fred-Frechet-1.9.9/src/dynamic_time_warping.cpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)    12023 2021-11-21 10:45:12.000000 Fred-Frechet-1.9.9/src/frechet.cpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     8915 2021-11-17 13:55:12.000000 Fred-Frechet-1.9.9/src/fred_python_wrapper.cpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     1261 2021-08-27 09:30:48.000000 Fred-Frechet-1.9.9/src/interval.cpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     3299 2021-08-30 11:46:54.000000 Fred-Frechet-1.9.9/src/jl_transform.cpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     2124 2021-08-27 09:32:21.000000 Fred-Frechet-1.9.9/src/point.cpp
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     5332 2021-09-03 10:20:03.000000 Fred-Frechet-1.9.9/src/simplification.cpp
+drwxr-xr-x   0 glamr     (1000) glamr     (1000)        0 2021-11-21 10:49:50.285226 Fred-Frechet-1.9.9/test/
+-rw-r--r--   0 glamr     (1000) glamr     (1000)     1793 2021-09-07 07:59:19.000000 Fred-Frechet-1.9.9/test/test.py
```

### Comparing `Fred-Frechet-1.9.8/CMakeLists.txt` & `Fred-Frechet-1.9.9/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/Fred/__init__.py` & `Fred-Frechet-1.9.9/Fred/__init__.py`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/Fred/hd_fs.py` & `Fred-Frechet-1.9.9/Fred/hd_fs.py`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/Fred/median.py` & `Fred-Frechet-1.9.9/Fred/median.py`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/Fred_Frechet.egg-info/PKG-INFO` & `Fred-Frechet-1.9.9/Fred_Frechet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fred-Frechet
-Version: 1.9.8
+Version: 1.9.9
 Summary: A fast, scalable and light-weight C++ Fréchet distance library, exposed to python and focused on (k,l)-clustering of polygonal curves.
 Home-page: http://fred.dennisrohde.work
 Author: Dennis Rohde
 Author-email: dennis.rohde@tu-dortmund.de
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `Fred-Frechet-1.9.8/Fred_Frechet.egg-info/SOURCES.txt` & `Fred-Frechet-1.9.9/Fred_Frechet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/LICENSE` & `Fred-Frechet-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/PKG-INFO` & `Fred-Frechet-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fred-Frechet
-Version: 1.9.8
+Version: 1.9.9
 Summary: A fast, scalable and light-weight C++ Fréchet distance library, exposed to python and focused on (k,l)-clustering of polygonal curves.
 Home-page: http://fred.dennisrohde.work
 Author: Dennis Rohde
 Author-email: dennis.rohde@tu-dortmund.de
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `Fred-Frechet-1.9.8/README.md` & `Fred-Frechet-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/include/clustering.hpp` & `Fred-Frechet-1.9.9/include/clustering.hpp`

 * *Files 21% similar despite different names*

```diff
@@ -17,48 +17,59 @@
 #include "random.hpp"
 #include "curve.hpp"
 #include "frechet.hpp"
 #include "dynamic_time_warping.hpp"
 #include "simplification.hpp"
 
 namespace Clustering {
-    
-struct Distance_Matrix : public std::vector<std::vector<distance_t>> {
-    Distance_Matrix() {}
-    Distance_Matrix(const curve_number_t n, const curve_number_t m) : std::vector<std::vector<distance_t>>(n, std::vector<distance_t>(m, -1.0)) {}
-    
-    void print() const;
-};
+
+struct Distance_Matrix;
 
 extern Distance_Matrix distances;
 extern Curves simplifications;
 
-class Cluster_Assignment : public std::vector<std::vector<curve_number_t>> {
+struct Distance_Matrix : public std::vector<Distances> {
+    Distance_Matrix() = default;
+    Distance_Matrix(const curve_number_t n, const curve_number_t m) : std::vector<Distances>(n, Distances(m, -1.0)) {}
+    void print() const;
+};
+
+class Cluster_Assignment : public std::vector<Curve_Numbers> {
 public:
-    inline Cluster_Assignment(const curve_number_t k = 0) : std::vector<std::vector<curve_number_t>>(k, std::vector<curve_number_t>()) {}
-    
-    inline curve_number_t count(const curve_number_t i) const {
-        return operator[](i).size();
-    }
-    
-    inline curve_number_t get(const curve_number_t i, const curve_number_t j) const {
-        return operator[](i)[j];
-    }
+    explicit Cluster_Assignment(const curve_number_t k = 0) : std::vector<Curve_Numbers>(k, Curve_Numbers()) {}
+    curve_number_t count(const curve_number_t) const;
+    curve_number_t get(const curve_number_t, const curve_number_t) const;
+};
+
+struct Clustering_Result {
+    Curves centers;
+    distance_t value;
+    double running_time;
+    Cluster_Assignment assignment;
     
+    Curve& get(const curve_number_t);
+    curve_number_t size() const;
+    Curves::const_iterator cbegin() const;
+    Curves::const_iterator cend() const;
+    void compute_assignment(const Curves&, const bool = false);
+    void set_center_indices(const Curve_Numbers&);
+
+private:
+    Curve_Numbers center_indices;
 };
 
 inline distance_t _cheap_dist(const curve_number_t i, const curve_number_t j, const Curves &in, const Curves &simplified_in, Distance_Matrix &distances) {
     if (distances[i][j] < 0) {
         const auto dist = Frechet::Continuous::distance(in[i], simplified_in[j]);
         distances[i][j] = dist.value;
     }
     return distances[i][j];
 }
 
-inline curve_number_t _nearest_center(const curve_number_t i, const Curves &in, const Curves &simplified_in, const std::vector<curve_number_t> &centers, Distance_Matrix &distances) {
+inline curve_number_t _nearest_center(const curve_number_t i, const Curves &in, const Curves &simplified_in, const Curve_Numbers &centers, Distance_Matrix &distances) {
     const auto infty = std::numeric_limits<distance_t>::infinity();
     // cost for curve is infinity
     auto min_cost = infty;
     curve_number_t nearest = 0;
     
     // except there is a center with smaller cost, then choose the one with smallest cost
     for (curve_number_t j = 0; j < centers.size(); ++j) {
@@ -66,70 +77,29 @@
             min_cost = _cheap_dist(i, centers[j], in, simplified_in, distances);
             nearest = j;
         }
     }
     return nearest;
 }
 
-inline distance_t _curve_cost(const curve_number_t i, const Curves &in, const Curves &simplified_in, const std::vector<curve_number_t> &centers, Distance_Matrix &distances) {
+inline distance_t _curve_cost(const curve_number_t i, const Curves &in, const Curves &simplified_in, const Curve_Numbers &centers, Distance_Matrix &distances) {
     return _cheap_dist(i, centers[_nearest_center(i, in, simplified_in, centers, distances)], in, simplified_in, distances);
 }
 
-inline distance_t _center_cost_sum(const Curves &in, const Curves &simplified_in, const std::vector<curve_number_t> &centers, Distance_Matrix &distances) {
+inline distance_t _center_cost_sum(const Curves &in, const Curves &simplified_in, const Curve_Numbers &centers, Distance_Matrix &distances) {
     distance_t cost = 0;
     
     // for all curves
     for (curve_number_t i = 0; i < in.size(); ++i) {
         const auto min_cost_elem = _curve_cost(i, in, simplified_in, centers, distances);
         cost += min_cost_elem;
     }
     return cost;
 }
 
-struct Clustering_Result {
-    Curves centers;
-    distance_t value;
-    double running_time;
-    Cluster_Assignment assignment;
-    
-    inline Curve& get(const curve_number_t i) {
-        return centers[i];
-    }
-    inline curve_number_t size() const {
-        return centers.size();
-    }
-    
-    inline Curves::const_iterator cbegin() const {
-        return centers.cbegin();
-    }
-    
-    inline Curves::const_iterator cend() const {
-        return centers.cend();
-    }
-    
-    inline void compute_assignment(const Curves &in, const bool consecutive_call = false) {
-        assignment = Cluster_Assignment(centers.size());
-        if (consecutive_call and in.size() == distances.size()) {
-            for (curve_number_t i = 0; i < in.size(); ++i) assignment[_nearest_center(i, in, simplifications, center_indices, distances)].push_back(i);
-        } else {
-            auto ndistances = Distance_Matrix(in.size(), centers.size());
-            auto ncenter_indices = std::vector<curve_number_t>(centers.size());
-            std::iota(ncenter_indices.begin(), ncenter_indices.end(), 0);
-            for (curve_number_t i = 0; i < in.size(); ++i) assignment[_nearest_center(i, in, centers, ncenter_indices, ndistances)].push_back(i);
-        }
-    }
-    
-    inline void set_center_indices(const std::vector<curve_number_t> &pcenter_indices) {
-        center_indices = pcenter_indices;
-    }
-
-private:
-    std::vector<curve_number_t> center_indices;
-};
-
 Clustering_Result kl_cluster(const curve_number_t, const curve_size_t, const Curves &, const bool, const bool, const bool, const bool);
 
 Clustering_Result kl_center(const curve_number_t, const curve_size_t, const Curves &, const bool = false, const bool = true, const bool = false);
 
 Clustering_Result kl_median(const curve_number_t, const curve_size_t, const Curves &, const bool = false, const bool = false);
 
 }
```

### Comparing `Fred-Frechet-1.9.8/include/config.hpp` & `Fred-Frechet-1.9.9/include/config.hpp`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/include/coreset.hpp` & `Fred-Frechet-1.9.9/include/coreset.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     const Curves &in;
     const curve_number_t k;
     const curve_size_t ell;
     const distance_t Lambda;
     parameter_t epsilon;
     distance_t constant;
     Clustering::Clustering_Result c_approx;
-    std::vector<distance_t> cluster_costs;
-    std::vector<curve_number_t> cluster_sizes;
-    std::vector<curve_number_t> coreset;
-    std::vector<distance_t> lambda;
-    std::vector<parameter_t> probabilities;
+    Distances cluster_costs;
+    Curve_Numbers cluster_sizes;
+    Curve_Numbers coreset;
+    Distances lambda;
+    Parameters probabilities;
 
 public:
     inline Median_Coreset(const curve_number_t k, curve_size_t ell, const Curves &in, const parameter_t epsilon, const distance_t constant = 1) : in{in}, k{k}, ell{ell}, epsilon{epsilon}, constant{constant}, cluster_costs(k, 0), cluster_sizes(k, 0), lambda(in.size()), Lambda{2*k + 12*std::sqrt(k) + 18}, probabilities(in.size()), c_approx{Clustering::kl_median(k, ell, in)} {
         c_approx.compute_assignment(in);
         for (curve_number_t i = 0; i < k; ++i) {
             for (curve_number_t j = 0; j < c_approx.assignment.count(i); ++j) {
                 cluster_costs[i] += Frechet::Continuous::distance(in[c_approx.assignment.get(i, j)], c_approx.centers[i]).value;
```

### Comparing `Fred-Frechet-1.9.8/include/curve.hpp` & `Fred-Frechet-1.9.9/include/curve.hpp`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/include/dynamic_time_warping.hpp` & `Fred-Frechet-1.9.9/include/dynamic_time_warping.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -6,27 +6,31 @@
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 */
 
 #pragma once
 
+#include <map>
+
 #include "types.hpp"
 #include "point.hpp"
 #include "interval.hpp"
 #include "curve.hpp"
+#include "random.hpp"
 
 namespace Dynamic_Time_Warping {
     
 namespace Discrete {
     
     struct Distance {
         distance_t value;
         double time;
         
         std::string repr() const;
     };
     
     Distance distance(const Curve&, const Curve&);
+    Distance distance_randomized(const Curve&, const Curve&);
 }
 
 }
```

### Comparing `Fred-Frechet-1.9.8/include/frechet.hpp` & `Fred-Frechet-1.9.9/include/frechet.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     };
     
     Distance distance(const Curve&, const Curve&);
     
     Distance _distance(const Curve&, const Curve&, distance_t, distance_t);
             
     bool _less_than_or_equal(const distance_t, const Curve&, const Curve&, 
-            std::vector<std::vector<parameter_t>>&, std::vector<std::vector<parameter_t>>&, 
-            std::vector<std::vector<Interval>>&, std::vector<std::vector<Interval>>&);
+            std::vector<Parameters>&, std::vector<Parameters>&, 
+            std::vector<Intervals>&, std::vector<Intervals>&);
             
     distance_t _greedy_upper_bound(const Curve&, const Curve&);
     distance_t _projective_lower_bound(const Curve&, const Curve&);
 }
 namespace Discrete {
     
     struct Distance {
@@ -48,11 +48,11 @@
         double time;
         
         std::string repr() const;
     };
     
     Distance distance(const Curve&, const Curve&);
     
-    distance_t _dp(std::vector<std::vector<distance_t>> &a, const curve_size_t i, const curve_size_t j, 
+    distance_t _dp(std::vector<Distances> &a, const curve_size_t i, const curve_size_t j, 
             const Curve &curve1, const Curve &curve2);
 }
 }
```

### Comparing `Fred-Frechet-1.9.8/include/grid.hpp` & `Fred-Frechet-1.9.9/include/grid.hpp`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/include/interval.hpp` & `Fred-Frechet-1.9.9/include/interval.hpp`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/include/jl_transform.hpp` & `Fred-Frechet-1.9.9/include/jl_transform.hpp`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/include/point.hpp` & `Fred-Frechet-1.9.9/include/point.hpp`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/include/random.hpp` & `Fred-Frechet-1.9.9/include/random.hpp`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/include/simplification.hpp` & `Fred-Frechet-1.9.9/include/simplification.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 #include "frechet.hpp"
 
 namespace Simplification {
 
 class Subcurve_Shortcut_Graph {
 
     Curve& curve;
-    std::vector<std::vector<distance_t>> edges;
+    std::vector<Distances> edges;
     
 public:
     
-    Subcurve_Shortcut_Graph(Curve &curve) : curve{curve}, edges{std::vector<std::vector<distance_t>>(curve.complexity(), std::vector<distance_t>(curve.complexity(), std::numeric_limits<distance_t>::infinity()))} {
+    Subcurve_Shortcut_Graph(Curve &curve) : curve{curve}, edges{std::vector<Distances>(curve.complexity(), Distances(curve.complexity(), std::numeric_limits<distance_t>::infinity()))} {
         if (Config::verbosity > 1) std::cout << "SIMPL: computing shortcut graph" << std::endl;
         const curve_size_t complexity = curve.complexity();
         Curve segment(2, curve.front().dimensions());
         auto distance = Frechet::Continuous::Distance();
         
         for (curve_size_t i = 0; i < complexity - 1; ++i) {
             for (curve_size_t j = i + 1; j < complexity; ++j) {
@@ -66,18 +66,18 @@
         
         if (ll <= 2) {
             result.push_back(curve.front());
             result.push_back(curve.back());
             return result;
         }
         
-        std::vector<std::vector<distance_t>> distances(curve.complexity(), std::vector<distance_t>(l, std::numeric_limits<distance_t>::infinity()));
+        std::vector<Distances> distances(curve.complexity(), Distances(l, std::numeric_limits<distance_t>::infinity()));
         std::vector<std::vector<curve_size_t>> predecessors(curve.complexity(), std::vector<curve_size_t>(l));
         
-        std::vector<distance_t> others;
+        Distances others;
         curve_size_t best = 0;
         for (curve_size_t i = 0; i < l; ++i) {
             
             if (i == 0) {
                 if (Config::verbosity > 1) std::cout << "SIMPL: initializing arrays" << std::endl;
                 #pragma omp parallel for
                 for (curve_size_t j = 1; j < curve.complexity(); ++j) {
```

### Comparing `Fred-Frechet-1.9.8/include/types.hpp` & `Fred-Frechet-1.9.9/include/types.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -10,30 +10,32 @@
 
 #pragma once
 
 #include <vector>
 #include <cmath>
 #include <limits>
 
-typedef double distance_t;
-typedef double coordinate_t;
-typedef long double parameter_t;
-
-typedef unsigned long dimensions_t;
-typedef unsigned long curve_size_t;
-typedef unsigned long curve_number_t;
+typedef double distance_t; // Distances
+typedef double coordinate_t; // Coordinates
+typedef long double parameter_t; // Parameters, i.e., values in [0,1]
+
+typedef unsigned long dimensions_t; // Dimensions
+typedef unsigned long curve_size_t; // Curve complexities
+typedef unsigned long curve_number_t; // Number of curves
 
 class Point;
 class Curve;
 class Interval;
 
 using Vector = Point;
-
 using Intervals = std::vector<Interval>;
 using Coordinates = std::vector<coordinate_t>;
+using Distances = std::vector<distance_t>;
+using Curve_Numbers = std::vector<curve_number_t>;
+using Parameters = std::vector<parameter_t>;
 
-template<typename T>
+template<typename T, std::enable_if_t<std::is_arithmetic<T>::value, bool> = true>
 inline bool near_eq(T x, T y) {
   return std::abs(x - y) <= std::min(std::abs(x), std::abs(y)) * std::numeric_limits<T>::epsilon();
 }
```

### Comparing `Fred-Frechet-1.9.8/logo/logo.png` & `Fred-Frechet-1.9.9/logo/logo.png`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/logo/logo.svg` & `Fred-Frechet-1.9.9/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/setup.py` & `Fred-Frechet-1.9.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         subprocess.check_call(['cmake', "{}".format(ext.sourcedir)] + cmake_args,
                               cwd=self.build_temp, env=env)
         subprocess.check_call(['cmake', '--build', '.'] + build_args,
                               cwd=self.build_temp)
 
 setup(
     name='Fred-Frechet',
-    version='1.9.8',
+    version='1.9.9',
     author='Dennis Rohde',
     author_email='dennis.rohde@tu-dortmund.de',
     description='A fast, scalable and light-weight C++ Fréchet distance library, exposed to python and focused on (k,l)-clustering of polygonal curves.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="http://fred.dennisrohde.work",
     packages=setuptools.find_packages(),
```

### Comparing `Fred-Frechet-1.9.8/src/clustering.cpp` & `Fred-Frechet-1.9.9/src/clustering.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -4,32 +4,72 @@
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 */
 
-#include "clustering.hpp"
-
 #include<ctime>
 
+#include "clustering.hpp"
+
 namespace Clustering {
 
 Distance_Matrix distances;
 Curves simplifications;
-    
+
 void Distance_Matrix::print() const {
     for (const auto &row : *this) {
         for (const auto elem : row) {
             std::cout << elem << " ";
         }
         std::cout << std::endl;
     }
 }
 
+Curve& Clustering_Result::get(const curve_number_t i) {
+    return centers[i];
+}
+
+curve_number_t Clustering_Result::size() const {
+    return centers.size();
+}
+
+Curves::const_iterator Clustering_Result::cbegin() const {
+    return centers.cbegin();
+}
+
+Curves::const_iterator Clustering_Result::cend() const {
+    return centers.cend();
+}
+
+void Clustering_Result::compute_assignment(const Curves &in, const bool consecutive_call) {
+    assignment = Cluster_Assignment(centers.size());
+    if (consecutive_call and in.size() == distances.size()) {
+        for (curve_number_t i = 0; i < in.size(); ++i) assignment[_nearest_center(i, in, simplifications, center_indices, distances)].push_back(i);
+    } else {
+        auto ndistances = Distance_Matrix(in.size(), centers.size());
+        auto ncenter_indices = Curve_Numbers(centers.size());
+        std::iota(ncenter_indices.begin(), ncenter_indices.end(), 0);
+        for (curve_number_t i = 0; i < in.size(); ++i) assignment[_nearest_center(i, in, centers, ncenter_indices, ndistances)].push_back(i);
+    }
+}
+
+void Clustering_Result::set_center_indices(const Curve_Numbers &pcenter_indices) {
+    center_indices = pcenter_indices;
+}
+
+curve_number_t Cluster_Assignment::count(const curve_number_t i) const {
+    return operator[](i).size();
+}
+
+curve_number_t Cluster_Assignment::get(const curve_number_t i, const curve_number_t j) const {
+    return operator[](i)[j];
+}
+
 Clustering_Result kl_cluster(const curve_number_t num_centers, const curve_size_t ell, const Curves &in, 
                              const bool local_search = false, const bool consecutive_call = false, const bool random_start_center = true, const bool fast_simplification = false) {
     
     const auto start = std::clock();
     Clustering_Result result;
     
     if (in.empty()) return result;
@@ -45,17 +85,17 @@
         if (distances.size() != in.size()) {
             std::cerr << "WARNING: you have tried to use 'consecutive_call = true' with different input; ignoring!" << std::endl;
             distances = Distance_Matrix(in.size(), in.size());
             simplifications = Curves(in.number(), ell, in.dimensions());
         }
     }
 
-    std::vector<curve_number_t> centers;
+    Curve_Numbers centers;
     
-    auto simplify = [&](const curve_number_t i) {
+    const auto simplify = [&](const curve_number_t i) {
         if (fast_simplification) {
             if (Config::verbosity > 0) std::cout << "KL_CLUST: computing approximate vertex restricted minimum error simplification" << std::endl;
             auto simplified_curve = Simplification::approximate_minimum_error_simplification(const_cast<Curve&>(in[i]), ell);
             simplified_curve.set_name("Simplification of " + in[i].get_name());
             return simplified_curve;
         } else {
             if (Config::verbosity > 0) std::cout << "KL_CLUST: computing exact vertex restricted minimum error simplification" << std::endl;
@@ -168,15 +208,15 @@
         }
         curr_maxdist = cost;
     }
 
     Curves simpl_centers;
     for (const auto center: centers) simpl_centers.push_back(simplifications[center]);
     
-    auto end = std::clock();
+    const auto end = std::clock();
     result.centers = simpl_centers;
     result.set_center_indices(centers);
     result.value = curr_maxdist;
     result.running_time = (end - start) / CLOCKS_PER_SEC;
     return result;
 }
```

### Comparing `Fred-Frechet-1.9.8/src/config.cpp` & `Fred-Frechet-1.9.9/src/config.cpp`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/src/curve.cpp` & `Fred-Frechet-1.9.9/src/curve.cpp`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/src/frechet.cpp` & `Fred-Frechet-1.9.9/src/frechet.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -62,19 +62,19 @@
     const distance_t p_error = lb * error / 100 > std::numeric_limits<distance_t>::epsilon() ? lb * error / 100 : std::numeric_limits<distance_t>::epsilon();
     std::size_t number_searches = 0;
     
     if (ub - lb > p_error) {
         if (Config::verbosity > 2) std::cout << "CFD: binary search using FSD" << std::endl;
         
         const auto infty = std::numeric_limits<parameter_t>::infinity();
-        std::vector<std::vector<parameter_t>> reachable1(curve1.complexity() - 1, std::vector<parameter_t>(curve2.complexity(), infty));
-        std::vector<std::vector<parameter_t>> reachable2(curve1.complexity(), std::vector<parameter_t>(curve2.complexity() - 1, infty));
+        std::vector<Parameters> reachable1(curve1.complexity() - 1, Parameters(curve2.complexity(), infty));
+        std::vector<Parameters> reachable2(curve1.complexity(), Parameters(curve2.complexity() - 1, infty));
         
-        std::vector<std::vector<Interval>> free_intervals1(curve2.complexity(), std::vector<Interval>(curve1.complexity(), Interval()));
-        std::vector<std::vector<Interval>> free_intervals2(curve1.complexity(), std::vector<Interval>(curve2.complexity(), Interval()));
+        std::vector<Intervals> free_intervals1(curve2.complexity(), Intervals(curve1.complexity(), Interval()));
+        std::vector<Intervals> free_intervals2(curve1.complexity(), Intervals(curve2.complexity(), Interval()));
 
         if (std::isnan(lb) or std::isnan(ub)) {
             result.value = std::numeric_limits<distance_t>::signaling_NaN();
             return result;
         }
 
         //Binary search over the feasible distances
@@ -97,16 +97,16 @@
     result.value = lb;
     result.time_searches = (end - start) / CLOCKS_PER_SEC;
     result.number_searches = number_searches;
     return result;
 }
 
 bool _less_than_or_equal(const distance_t distance, Curve const& curve1, Curve const& curve2, 
-        std::vector<std::vector<parameter_t>> &reachable1, std::vector<std::vector<parameter_t>> &reachable2,
-        std::vector<std::vector<Interval>> &free_intervals1, std::vector<std::vector<Interval>> &free_intervals2) {
+        std::vector<Parameters> &reachable1, std::vector<Parameters> &reachable2,
+        std::vector<Intervals> &free_intervals1, std::vector<Intervals> &free_intervals2) {
     
     if (Config::verbosity > 2) std::cout << "CFD: constructing FSD" << std::endl;
     const distance_t dist_sqr = distance * distance;
     const auto infty = std::numeric_limits<parameter_t>::infinity();
     const curve_size_t n1 = curve1.complexity();
     const curve_size_t n2 = curve2.complexity();
 
@@ -132,15 +132,15 @@
     for (curve_size_t j = 0; j < n2 - 1; ++j) {
         reachable2[0][j] = 0;
         if (curve1[0].dist_sqr(curve2[j+1]) > dist_sqr) break;
     }
     
     if (Config::verbosity > 2) std::cout << "CFD: computing free space" << std::endl;
     
-    #pragma omp target teams distribute parallel for collapse(2) if (n1 * n2 > 1000)
+    #pragma omp parallel for collapse(2) if (n1 * n2 > 1000)
     for (curve_size_t i = 0; i < n1; ++i) {
         for (curve_size_t j = 0; j < n2; ++j) {
             if ((i < n1 - 1) and (j > 0)) {
                 free_intervals1[j][i] = curve2[j].ball_intersection_interval(dist_sqr, curve1[i], curve1[i+1]);
             }
             if ((j < n2 - 1) and (i > 0)) {
                 free_intervals2[i][j] = curve1[i].ball_intersection_interval(dist_sqr, curve2[j], curve2[j+1]);
```

### Comparing `Fred-Frechet-1.9.8/src/fred_python_wrapper.cpp` & `Fred-Frechet-1.9.9/src/fred_python_wrapper.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,15 @@
         .def(py::init<curve_number_t, curve_size_t, Curves&, parameter_t>())
         .def("cost", &Coreset::Median_Coreset::cost)
     ;
     
     m.def("continuous_frechet", &fc::distance);
     m.def("discrete_frechet", &fd::distance);
     m.def("discrete_dynamic_time_warping", &ddtw::distance);
+    m.def("discrete_dynamic_time_warping_randomized", &ddtw::distance_randomized);
     
     m.def("minimum_error_simplification", &minimum_error_simplification);
     m.def("approximate_minimum_link_simplification", &approximate_minimum_link_simplification);
     m.def("approximate_minimum_error_simplification", &approximate_minimum_error_simplification);
     
     m.def("dimension_reduction", &JLTransform::transform_naive, py::arg("curves"), py::arg("epsilon") = 0.5, py::arg("empirical_constant") = true);
```

### Comparing `Fred-Frechet-1.9.8/src/interval.cpp` & `Fred-Frechet-1.9.9/src/interval.cpp`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/src/jl_transform.cpp` & `Fred-Frechet-1.9.9/src/jl_transform.cpp`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/src/point.cpp` & `Fred-Frechet-1.9.9/src/point.cpp`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/src/simplification.cpp` & `Fred-Frechet-1.9.9/src/simplification.cpp`

 * *Files identical despite different names*

### Comparing `Fred-Frechet-1.9.8/test/test.py` & `Fred-Frechet-1.9.9/test/test.py`

 * *Files identical despite different names*

