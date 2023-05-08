# Comparing `tmp/google-flight-analysis-1.0.0.tar.gz` & `tmp/google-flight-analysis-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-flight-analysis-1.0.0.tar", last modified: Tue Apr 11 05:25:37 2023, max compression
+gzip compressed data, was "google-flight-analysis-1.1.0.tar", last modified: Mon May  8 01:03:54 2023, max compression
```

## Comparing `google-flight-analysis-1.0.0.tar` & `google-flight-analysis-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.852778 google-flight-analysis-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.848778 google-flight-analysis-1.0.0/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.844778 google-flight-analysis-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.848778 google-flight-analysis-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/.github/workflows/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.848778 google-flight-analysis-1.0.0/.github/workflows/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1466 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/.github/workflows/scripts/release.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-04-11 05:25:37.852778 google-flight-analysis-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-11 05:25:37.852778 google-flight-analysis-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.844778 google-flight-analysis-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.848778 google-flight-analysis-1.0.0/src/google_flight_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/src/google_flight_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/src/google_flight_analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/src/google_flight_analysis/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/src/google_flight_analysis/scrape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.848778 google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-04-11 05:25:37.000000 google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-11 05:25:37.000000 google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 05:25:37.000000 google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 05:25:37.000000 google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 05:25:37.000000 google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 05:25:37.000000 google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.848778 google-flight-analysis-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/tests/test_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.848778 google-flight-analysis-1.0.0/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.848778 google-flight-analysis-1.0.0/tests/test_data/.access/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/tests/test_data/.access/CDG-IST.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/tests/test_data/.access/LGA-RDU.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/tests/test_data/CDG-IST.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/tests/test_data/LGA-RDU.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/tests/test_data/test1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/tests/test_data/test2.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.897623 google-flight-analysis-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.893623 google-flight-analysis-1.1.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.893623 google-flight-analysis-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.893623 google-flight-analysis-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/.github/workflows/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.893623 google-flight-analysis-1.1.0/.github/workflows/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1466 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/.github/workflows/scripts/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-08 01:03:54.897623 google-flight-analysis-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-08 01:03:54.897623 google-flight-analysis-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.893623 google-flight-analysis-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.893623 google-flight-analysis-1.1.0/src/google_flight_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/src/google_flight_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/src/google_flight_analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/src/google_flight_analysis/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/src/google_flight_analysis/flight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/src/google_flight_analysis/scrape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.893623 google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-08 01:03:54.000000 google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-08 01:03:54.000000 google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 01:03:54.000000 google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-08 01:03:54.000000 google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 01:03:54.000000 google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 01:03:54.000000 google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.897623 google-flight-analysis-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/tests/test_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.897623 google-flight-analysis-1.1.0/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.897623 google-flight-analysis-1.1.0/tests/test_data/.access/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/tests/test_data/.access/CDG-IST.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/tests/test_data/.access/LGA-RDU.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/tests/test_data/CDG-IST.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/tests/test_data/LGA-RDU.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/tests/test_data/test1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/tests/test_data/test2.csv
```

### Comparing `google-flight-analysis-1.0.0/.circleci/config.yml` & `google-flight-analysis-1.1.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-1.0.0/.github/workflows/scripts/release.py` & `google-flight-analysis-1.1.0/.github/workflows/scripts/release.py`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-1.0.0/LICENSE` & `google-flight-analysis-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-1.0.0/PKG-INFO` & `google-flight-analysis-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: google-flight-analysis
-Version: 1.0.0
+Version: 1.1.0
 Summary: Scraping flight data from Google Flights and analyzing.
 Home-page: https://github.com/kcelebi/flight_analysis
 Author: Kaya Celebi
 Author-email: kayacelebi17@gmail.com
 Project-URL: Bug Tracker, https://github.com/kcelebi/flight_analysis/issues
 Project-URL: Changelog, https://github.com/kcelebi/flight_analysis/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![kcelebi](https://circleci.com/gh/kcelebi/flight-analysis.svg?style=svg)](https://circleci.com/gh/kcelebi/flight-analysis)
+[![kcelebi](https://circleci.com/gh/celebi-pkg/flight-analysis.svg?style=svg)](https://circleci.com/gh/celebi-pkg/flight-analysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Live on PyPI](https://img.shields.io/badge/PyPI-0.0.7-brightgreen)](https://img.shields.io/endpoint?url=img.shields.io/badge/PyPI-0.0.7-brightgreen)
+[![Live on PyPI](https://img.shields.io/badge/PyPI-1.0.0-brightgreen)](https://pypi.org/project/google-flight-analysis/)
 
 # Flight Analysis
 
 This project provides tools and models for users to analyze, forecast, and collect data regarding flights and prices. There are currently many features in initial stages and in development. The current features (as of 4/5/2023) are:
 
 - Scraping tools for Google Flights
 - Base analytical tools/methods for price forecasting/summary
@@ -63,25 +63,34 @@
 The main scraping function that makes up the backbone of most other functionalities is `Scrape()`. It serves also as a data object, preserving the flight information as well as meta-data from your query. For Python package users, import as follows:
 
 	from google_flight_analysis.scrape import *
 
 For GitHub repository cloners, import as follows from the root of the repository:
 
 	from src.google_flight_analysis.scrape import *
+	#---OR---#
+	import sys
+	sys.path.append('src/google_flight_analysis')
+	from scrape import *
+
 
 Here is some quick starter code to accomplish the basic tasks. Find more in the [documentation](https://kcelebi.github.io/flight-analysis/).
 
 	# Try to keep the dates in format YYYY-mm-dd
-	result = Scrape('JFK', 'IST', '2022-05-20', '2022-06-10') # obtain our scrape object
-
+	result = Scrape('JFK', 'IST', '2023-07-20', '2023-08-10') # obtain our scrape object
 	dataframe = result.data # outputs a Pandas DF with flight prices/info
 	origin = result.origin # 'JFK'
 	dest = result.dest # 'IST'
-	date_leave = result.date_leave # '2022-05-20'
-	date_return = result.date_return # '2022-06-10'
+	date_leave = result.date_leave # '2023-05-20'
+	date_return = result.date_return # '2023-06-10'
+
+You can also scrape for one-way trips now:
+
+	results = Scrape('JFK', 'IST', '2023-08-20')
+	result.data.head() #see data
 
 
 ## Updates & New Features
 
 Performing a complete revamp of this package, including new addition to PyPI. Documentation is being updated frequently, contact for any questions.
```

### Comparing `google-flight-analysis-1.0.0/README.md` & `google-flight-analysis-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-[![kcelebi](https://circleci.com/gh/kcelebi/flight-analysis.svg?style=svg)](https://circleci.com/gh/kcelebi/flight-analysis)
+[![kcelebi](https://circleci.com/gh/celebi-pkg/flight-analysis.svg?style=svg)](https://circleci.com/gh/celebi-pkg/flight-analysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Live on PyPI](https://img.shields.io/badge/PyPI-0.0.7-brightgreen)](https://img.shields.io/endpoint?url=img.shields.io/badge/PyPI-0.0.7-brightgreen)
+[![Live on PyPI](https://img.shields.io/badge/PyPI-1.0.0-brightgreen)](https://pypi.org/project/google-flight-analysis/)
 
 # Flight Analysis
 
 This project provides tools and models for users to analyze, forecast, and collect data regarding flights and prices. There are currently many features in initial stages and in development. The current features (as of 4/5/2023) are:
 
 - Scraping tools for Google Flights
 - Base analytical tools/methods for price forecasting/summary
@@ -47,25 +47,34 @@
 The main scraping function that makes up the backbone of most other functionalities is `Scrape()`. It serves also as a data object, preserving the flight information as well as meta-data from your query. For Python package users, import as follows:
 
 	from google_flight_analysis.scrape import *
 
 For GitHub repository cloners, import as follows from the root of the repository:
 
 	from src.google_flight_analysis.scrape import *
+	#---OR---#
+	import sys
+	sys.path.append('src/google_flight_analysis')
+	from scrape import *
+
 
 Here is some quick starter code to accomplish the basic tasks. Find more in the [documentation](https://kcelebi.github.io/flight-analysis/).
 
 	# Try to keep the dates in format YYYY-mm-dd
-	result = Scrape('JFK', 'IST', '2022-05-20', '2022-06-10') # obtain our scrape object
-
+	result = Scrape('JFK', 'IST', '2023-07-20', '2023-08-10') # obtain our scrape object
 	dataframe = result.data # outputs a Pandas DF with flight prices/info
 	origin = result.origin # 'JFK'
 	dest = result.dest # 'IST'
-	date_leave = result.date_leave # '2022-05-20'
-	date_return = result.date_return # '2022-06-10'
+	date_leave = result.date_leave # '2023-05-20'
+	date_return = result.date_return # '2023-06-10'
+
+You can also scrape for one-way trips now:
+
+	results = Scrape('JFK', 'IST', '2023-08-20')
+	result.data.head() #see data
 
 
 ## Updates & New Features
 
 Performing a complete revamp of this package, including new addition to PyPI. Documentation is being updated frequently, contact for any questions.
```

### Comparing `google-flight-analysis-1.0.0/setup.cfg` & `google-flight-analysis-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-1.0.0/src/google_flight_analysis/cache.py` & `google-flight-analysis-1.1.0/src/google_flight_analysis/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 		# If file already exists
 		if os.path.isfile(fname):
 			# Check if most recent access is today
 			with open(access) as file:
 				recent_access = file.readline()
 				if recent_access != current_access:
 					df_old = pd.read_csv(fname, index_col = 'Unnamed: 0')
-					df = pd.concat([df_old, df])
+					df = pd.concat([df_old, df], ignore_index = True)
 				else:
 					return # Data already in csv, redundant
 
 		df.to_csv(fname)
 		with open(access, 'w') as file:
 			file.write(current_access)
 
@@ -61,15 +61,15 @@
 		conn = sqlite3.connect(self.directory + 'flights.db')
 
 		return conn
 
 	def disconnect_db(self, conn):
 		conn.close()
 
-	def create_table()
+	def create_table():
 		...
 
 
 	'''
 		Check that the scraping instance is valid
 	'''
 	@staticmethod
```

### Comparing `google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/PKG-INFO` & `google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: google-flight-analysis
-Version: 1.0.0
+Version: 1.1.0
 Summary: Scraping flight data from Google Flights and analyzing.
 Home-page: https://github.com/kcelebi/flight_analysis
 Author: Kaya Celebi
 Author-email: kayacelebi17@gmail.com
 Project-URL: Bug Tracker, https://github.com/kcelebi/flight_analysis/issues
 Project-URL: Changelog, https://github.com/kcelebi/flight_analysis/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![kcelebi](https://circleci.com/gh/kcelebi/flight-analysis.svg?style=svg)](https://circleci.com/gh/kcelebi/flight-analysis)
+[![kcelebi](https://circleci.com/gh/celebi-pkg/flight-analysis.svg?style=svg)](https://circleci.com/gh/celebi-pkg/flight-analysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Live on PyPI](https://img.shields.io/badge/PyPI-0.0.7-brightgreen)](https://img.shields.io/endpoint?url=img.shields.io/badge/PyPI-0.0.7-brightgreen)
+[![Live on PyPI](https://img.shields.io/badge/PyPI-1.0.0-brightgreen)](https://pypi.org/project/google-flight-analysis/)
 
 # Flight Analysis
 
 This project provides tools and models for users to analyze, forecast, and collect data regarding flights and prices. There are currently many features in initial stages and in development. The current features (as of 4/5/2023) are:
 
 - Scraping tools for Google Flights
 - Base analytical tools/methods for price forecasting/summary
@@ -63,25 +63,34 @@
 The main scraping function that makes up the backbone of most other functionalities is `Scrape()`. It serves also as a data object, preserving the flight information as well as meta-data from your query. For Python package users, import as follows:
 
 	from google_flight_analysis.scrape import *
 
 For GitHub repository cloners, import as follows from the root of the repository:
 
 	from src.google_flight_analysis.scrape import *
+	#---OR---#
+	import sys
+	sys.path.append('src/google_flight_analysis')
+	from scrape import *
+
 
 Here is some quick starter code to accomplish the basic tasks. Find more in the [documentation](https://kcelebi.github.io/flight-analysis/).
 
 	# Try to keep the dates in format YYYY-mm-dd
-	result = Scrape('JFK', 'IST', '2022-05-20', '2022-06-10') # obtain our scrape object
-
+	result = Scrape('JFK', 'IST', '2023-07-20', '2023-08-10') # obtain our scrape object
 	dataframe = result.data # outputs a Pandas DF with flight prices/info
 	origin = result.origin # 'JFK'
 	dest = result.dest # 'IST'
-	date_leave = result.date_leave # '2022-05-20'
-	date_return = result.date_return # '2022-06-10'
+	date_leave = result.date_leave # '2023-05-20'
+	date_return = result.date_return # '2023-06-10'
+
+You can also scrape for one-way trips now:
+
+	results = Scrape('JFK', 'IST', '2023-08-20')
+	result.data.head() #see data
 
 
 ## Updates & New Features
 
 Performing a complete revamp of this package, including new addition to PyPI. Documentation is being updated frequently, contact for any questions.
```

### Comparing `google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/SOURCES.txt` & `google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 .circleci/config.yml
 .github/workflows/publish.yml
 .github/workflows/release.yml
 .github/workflows/scripts/release.py
 src/google_flight_analysis/__init__.py
 src/google_flight_analysis/analysis.py
 src/google_flight_analysis/cache.py
+src/google_flight_analysis/flight.py
 src/google_flight_analysis/scrape.py
 src/google_flight_analysis.egg-info/PKG-INFO
 src/google_flight_analysis.egg-info/SOURCES.txt
 src/google_flight_analysis.egg-info/dependency_links.txt
 src/google_flight_analysis.egg-info/entry_points.txt
 src/google_flight_analysis.egg-info/requires.txt
 src/google_flight_analysis.egg-info/top_level.txt
```

### Comparing `google-flight-analysis-1.0.0/tests/test_class.py` & `google-flight-analysis-1.1.0/tests/test_class.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,29 +2,33 @@
 import pandas as pd
 from pathlib import Path
 import os
 
 from src.google_flight_analysis.scrape import *
 from src.google_flight_analysis.cache import *
 
+'''
+	Create resilience test: run the code 3 times and check DBs the same
+'''
+
 def func_0():
 	return True
 
 res1 = pd.read_csv('tests/test_data/test1.csv')
 res1 = Scrape("LGA", "RDU", "2023-05-15", "2023-06-15", res1)
 
 res2 = pd.read_csv('tests/test_data/test2.csv')
 res2 = Scrape("IST", "CDG", "2023-07-15", "2023-07-20", res2)
 
 os.system('rm tests/test_data/LGA-RDU.csv')
 os.system('rm tests/test_data/CDG-IST.csv')
 os.system('rm -rf tests/test_data/.access')
 
-CacheControl('tests/test_data/', res1)
-CacheControl('tests/test_data/', res2)
+CacheControl('tests/test_data/', res1, False)
+CacheControl('tests/test_data/', res2, False)
 
 def test_0():
 	assert func_0(), "Test 0 Failed"
 
 #-------QUERY 1
 
 def test_1():
```

### Comparing `google-flight-analysis-1.0.0/tests/test_data/CDG-IST.csv` & `google-flight-analysis-1.1.0/tests/test_data/CDG-IST.csv`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-1.0.0/tests/test_data/LGA-RDU.csv` & `google-flight-analysis-1.1.0/tests/test_data/LGA-RDU.csv`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-1.0.0/tests/test_data/test1.csv` & `google-flight-analysis-1.1.0/tests/test_data/test1.csv`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-1.0.0/tests/test_data/test2.csv` & `google-flight-analysis-1.1.0/tests/test_data/test2.csv`

 * *Files identical despite different names*

