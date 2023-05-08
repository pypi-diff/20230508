# Comparing `tmp/disdrodb-0.0.8.tar.gz` & `tmp/disdrodb-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disdrodb-0.0.8.tar", last modified: Tue Sep 13 09:27:28 2022, max compression
+gzip compressed data, was "disdrodb-0.0.9.tar", last modified: Tue Sep 13 09:34:13 2022, max compression
```

## Comparing `disdrodb-0.0.8.tar` & `disdrodb-0.0.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:28.319907 disdrodb-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-09-13 09:27:28.319907 disdrodb-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2371 2022-09-13 09:27:22.000000 disdrodb-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:28.315907 disdrodb-0.0.8/disdrodb/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:28.315907 disdrodb-0.0.8/disdrodb/L0/
--rw-r--r--   0 runner    (1001) docker     (121)    18103 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L0/L0A_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)    14698 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L0/L0B_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)    16154 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L0/L0_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10190 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L0/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (121)     3695 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L0/check_configs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2633 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L0/check_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    11816 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L0/check_standards.py
--rw-r--r--   0 runner    (1001) docker     (121)    25767 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L0/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L0/issue.py
--rw-r--r--   0 runner    (1001) docker     (121)     4212 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L0/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:28.315907 disdrodb-0.0.8/disdrodb/L0/readers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L0/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8551 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L0/readers/parser_template.py
--rw-r--r--   0 runner    (1001) docker     (121)    10233 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L0/standards.py
--rw-r--r--   0 runner    (1001) docker     (121)    11870 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L0/template_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    10931 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L0/utils_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:28.315907 disdrodb-0.0.8/disdrodb/L1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:28.319907 disdrodb-0.0.8/disdrodb/L2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/L2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:28.319907 disdrodb-0.0.8/disdrodb/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:28.319907 disdrodb-0.0.8/disdrodb/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2354 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/pipeline/run_ARM_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1961 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/pipeline/run_DELFT_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1843 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/pipeline/run_DIVEN_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3163 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/pipeline/run_EPFL_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/pipeline/utils_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:28.319907 disdrodb-0.0.8/disdrodb/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3263 2022-09-13 09:27:22.000000 disdrodb-0.0.8/disdrodb/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:27:28.315907 disdrodb-0.0.8/disdrodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-09-13 09:27:28.000000 disdrodb-0.0.8/disdrodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-09-13 09:27:28.000000 disdrodb-0.0.8/disdrodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 09:27:28.000000 disdrodb-0.0.8/disdrodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-13 09:27:28.000000 disdrodb-0.0.8/disdrodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-13 09:27:28.000000 disdrodb-0.0.8/disdrodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-09-13 09:27:28.319907 disdrodb-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-09-13 09:27:26.000000 disdrodb-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:13.324530 disdrodb-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-09-13 09:34:13.324530 disdrodb-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2371 2022-09-13 09:34:10.000000 disdrodb-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:13.316530 disdrodb-0.0.9/disdrodb/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:13.320530 disdrodb-0.0.9/disdrodb/L0/
+-rw-r--r--   0 runner    (1001) docker     (121)    18103 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L0/L0A_processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14698 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L0/L0B_processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16154 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L0/L0_processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10190 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L0/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3695 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L0/check_configs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2633 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L0/check_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11816 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L0/check_standards.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25767 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L0/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L0/issue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4212 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L0/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:13.320530 disdrodb-0.0.9/disdrodb/L0/readers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L0/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8604 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L0/readers/parser_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10233 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L0/standards.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11870 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L0/template_tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10931 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L0/utils_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:13.320530 disdrodb-0.0.9/disdrodb/L1/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:13.320530 disdrodb-0.0.9/disdrodb/L2/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/L2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:13.320530 disdrodb-0.0.9/disdrodb/api/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:13.320530 disdrodb-0.0.9/disdrodb/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2354 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/pipeline/run_ARM_processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1961 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/pipeline/run_DELFT_processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1843 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/pipeline/run_DIVEN_processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3163 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/pipeline/run_EPFL_processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/pipeline/utils_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:13.320530 disdrodb-0.0.9/disdrodb/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3263 2022-09-13 09:34:10.000000 disdrodb-0.0.9/disdrodb/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 09:34:13.316530 disdrodb-0.0.9/disdrodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-09-13 09:34:13.000000 disdrodb-0.0.9/disdrodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-09-13 09:34:13.000000 disdrodb-0.0.9/disdrodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 09:34:13.000000 disdrodb-0.0.9/disdrodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-13 09:34:13.000000 disdrodb-0.0.9/disdrodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-13 09:34:13.000000 disdrodb-0.0.9/disdrodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-09-13 09:34:13.324530 disdrodb-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-09-13 09:34:12.000000 disdrodb-0.0.9/setup.py
```

### Comparing `disdrodb-0.0.8/PKG-INFO` & `disdrodb-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disdrodb
-Version: 0.0.8
+Version: 0.0.9
 Summary: This package provides tools to homogenize, process, and analyze global disdrometer data.
 Author: Gionata Ghiggi
 Author-email: 
 Keywords: python,disdrometer
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `disdrodb-0.0.8/README.md` & `disdrodb-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/L0/L0A_processing.py` & `disdrodb-0.0.9/disdrodb/L0/L0A_processing.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/L0/L0B_processing.py` & `disdrodb-0.0.9/disdrodb/L0/L0B_processing.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/L0/L0_processing.py` & `disdrodb-0.0.9/disdrodb/L0/L0_processing.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/L0/auxiliary.py` & `disdrodb-0.0.9/disdrodb/L0/auxiliary.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/L0/check_configs.py` & `disdrodb-0.0.9/disdrodb/L0/check_configs.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/L0/check_metadata.py` & `disdrodb-0.0.9/disdrodb/L0/check_metadata.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/L0/check_standards.py` & `disdrodb-0.0.9/disdrodb/L0/check_standards.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/L0/io.py` & `disdrodb-0.0.9/disdrodb/L0/io.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/L0/issue.py` & `disdrodb-0.0.9/disdrodb/L0/issue.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/L0/metadata.py` & `disdrodb-0.0.9/disdrodb/L0/metadata.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/L0/readers/parser_template.py` & `disdrodb-0.0.9/disdrodb/L0/readers/parser_template.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,17 +12,24 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #-----------------------------------------------------------------------------.
+import os
+import sys
 import click
-from disdrodb.L0 import run_L0
- 
+from disdrodb.L0.L0_processing import run_L0
+
+# Add project root folder into sys path
+root_path = os.path.dirname(os.path.dirname(os.path.dirname(os.getcwd())))
+sys.path.insert(0,root_path)
+
+
 
 # -------------------------------------------------------------------------.
 # CLIck Command Line Interface decorator
 @click.command()  # options_metavar='<options>'
 @click.argument('raw_dir', type=click.Path(exists=True), metavar='<raw_dir>')
 @click.argument('processed_dir', metavar='<processed_dir>')
 @click.option('-L0A', '--l0a_processing', type=bool, show_default=True, default=True, help="Perform L0A processing")
@@ -38,154 +45,154 @@
          l0a_processing=True,
          l0b_processing=True,
          keep_l0a=False,
          force=False,
          verbose=False,
          debugging_mode=False,
          lazy=True,
-         single_netcdf = True, 
+         single_netcdf = True,
          ):
-    """Script to process raw data to L0A and L0B format. 
-    
+    """Script to process raw data to L0A and L0B format.
+
     Parameters
     ----------
     raw_dir : str
         Directory path of raw file for a specific campaign.
         The path should end with <campaign_name>.
         Example raw_dir: '<...>/disdrodb/data/raw/<campaign_name>'.
         The directory must have the following structure:
         - /data/<station_id>/<raw_files>
-        - /metadata/<station_id>.json 
+        - /metadata/<station_id>.json
         Important points:
         - For each <station_id> there must be a corresponding JSON file in the metadata subfolder.
         - The <campaign_name> must semantically match between:
            - the raw_dir and processed_dir directory paths;
-           - with the key 'campaign_name' within the metadata YAML files. 
-        - The campaign_name are set to be UPPER CASE. 
+           - with the key 'campaign_name' within the metadata YAML files.
+        - The campaign_name are set to be UPPER CASE.
     processed_dir : str
-        Desired directory path for the processed L0A and L0B products. 
+        Desired directory path for the processed L0A and L0B products.
         The path should end with <campaign_name> and match the end of raw_dir.
         Example: '<...>/disdrodb/data/processed/<campaign_name>'.
     L0A_processing : bool
       Whether to launch processing to generate L0A Apache Parquet file(s) from raw data.
       The default is True.
     L0B_processing : bool
-      Whether to launch processing to generate L0B netCDF4 file(s) from L0A data. 
+      Whether to launch processing to generate L0B netCDF4 file(s) from L0A data.
       The default is True.
-    keep_L0A : bool 
+    keep_L0A : bool
         Whether to keep the L0A files after having generated the L0B netCDF products.
         The default is False.
     force : bool
-        If True, overwrite existing data into destination directories. 
-        If False, raise an error if there are already data into destination directories. 
+        If True, overwrite existing data into destination directories.
+        If False, raise an error if there are already data into destination directories.
         The default is False.
     verbose : bool
-        Whether to print detailed processing information into terminal. 
+        Whether to print detailed processing information into terminal.
         The default is False.
     debugging_mode : bool
         If True, it reduces the amount of data to process.
         - For L0A processing, it processes just 3 raw data files.
         - For L0B processing, it takes a small subset of the L0A Apache Parquet dataframe.
         The default is False.
     lazy : bool
-        Whether to perform processing lazily with dask. 
+        Whether to perform processing lazily with dask.
         If lazy=True, it employed dask.array and dask.dataframe.
         If lazy=False, it employed pandas.DataFrame and numpy.array.
         The default is True.
     single_netcdf : bool
         Whether to concatenate all raw files into a single L0B netCDF file.
         If single_netcdf=True, all raw files will be saved into a single L0B netCDF file.
         If single_netcdf=False, each raw file will be converted into the corresponding L0B netCDF file.
         The default is True.
-    
+
     """
     ####----------------------------------------------------------------------.
     ###########################
     #### CUSTOMIZABLE CODE ####
     ###########################
-    #### - Define raw data headers 
+    #### - Define raw data headers
     column_names = []
-        
+
     ##------------------------------------------------------------------------.
-    #### - Define reader options 
+    #### - Define reader options
     reader_kwargs = {}
     # - Define delimiter
     reader_kwargs['delimiter'] = ','
-    
-    # - Avoid first column to become df index 
-    reader_kwargs["index_col"] = False  
-    
-    # - Define behaviour when encountering bad lines 
+
+    # - Avoid first column to become df index
+    reader_kwargs["index_col"] = False
+
+    # - Define behaviour when encountering bad lines
     reader_kwargs["on_bad_lines"] = 'skip'
-    
-    # - Define parser engine 
+
+    # - Define parser engine
     #   - C engine is faster
     #   - Python engine is more feature-complete
     reader_kwargs["engine"] = 'python'
-    
+
     # - Define on-the-fly decompression of on-disk data
-    #   - Available: gzip, bz2, zip 
-    reader_kwargs['compression'] = 'infer'  
-    
-    # - Strings to recognize as NA/NaN and replace with standard NA flags 
-    #   - Already included: ‘#N/A’, ‘#N/A N/A’, ‘#NA’, ‘-1.#IND’, ‘-1.#QNAN’, 
-    #                       ‘-NaN’, ‘-nan’, ‘1.#IND’, ‘1.#QNAN’, ‘<NA>’, ‘N/A’, 
+    #   - Available: gzip, bz2, zip
+    reader_kwargs['compression'] = 'infer'
+
+    # - Strings to recognize as NA/NaN and replace with standard NA flags
+    #   - Already included: ‘#N/A’, ‘#N/A N/A’, ‘#NA’, ‘-1.#IND’, ‘-1.#QNAN’,
+    #                       ‘-NaN’, ‘-nan’, ‘1.#IND’, ‘1.#QNAN’, ‘<NA>’, ‘N/A’,
     #                       ‘NA’, ‘NULL’, ‘NaN’, ‘n/a’, ‘nan’, ‘null’
     reader_kwargs['na_values'] = ['na', '', 'error']
-    
+
     # - Define max size of dask dataframe chunks (if lazy=True)
     #   - If None: use a single block for each file
     #   - Otherwise: "<max_file_size>MB" by which to cut up larger files
-    reader_kwargs["blocksize"] = None # "50MB" 
-    
+    reader_kwargs["blocksize"] = None # "50MB"
+
     ##------------------------------------------------------------------------.
     #### - Define facultative dataframe sanitizer function for L0 processing
-    # - Enable to deal with bad raw data files 
-    # - Enable to standardize raw data files to L0 standards   
-    df_sanitizer_fun = None 
+    # - Enable to deal with bad raw data files
+    # - Enable to standardize raw data files to L0 standards
+    df_sanitizer_fun = None
     def df_sanitizer_fun(df, lazy=False):
-        # Import dask or pandas 
-        if lazy: 
+        # Import dask or pandas
+        if lazy:
             import dask.dataframe as dd
-        else: 
+        else:
             import pandas as dd
 
-        # - Drop datalogger columns 
+        # - Drop datalogger columns
         columns_to_drop = ['id', 'datalogger_temperature', 'datalogger_voltage', 'datalogger_error']
         df = df.drop(columns=columns_to_drop)
-        
-        # - Drop latitude and longitude 
-        # --> Latitude and longitude is specified in the the metadata.yaml 
+
+        # - Drop latitude and longitude
+        # --> Latitude and longitude is specified in the the metadata.yaml
         df = df.drop(columns=['latitude', 'longitude'])
-        
+
         # - Convert time column to datetime with resolution in seconds
         df['time'] = dd.to_datetime(df['time'], format='%d-%m-%Y %H:%M:%S')
-        
-        return df  
-    
+
+        return df
+
     ##------------------------------------------------------------------------.
     #### - Define glob pattern to search data files within raw_dir/data/<station_id>
-    files_glob_pattern = "*.dat*"   
+    files_glob_pattern = "*.dat*"
 
     ####----------------------------------------------------------------------.
-    #### - Create L0 products  
+    #### - Create L0 products
     run_L0(
-        raw_dir=raw_dir,  
+        raw_dir=raw_dir,
         processed_dir=processed_dir,
         L0A_processing=l0a_processing,
         L0B_processing=l0b_processing,
         keep_L0A=keep_l0a,
         force=force,
         verbose=verbose,
         debugging_mode=debugging_mode,
         lazy=lazy,
         single_netcdf=single_netcdf,
-        # Custom arguments of the parser 
-        files_glob_pattern = files_glob_pattern, 
+        # Custom arguments of the parser
+        files_glob_pattern = files_glob_pattern,
         column_names=column_names,
         reader_kwargs=reader_kwargs,
         df_sanitizer_fun=df_sanitizer_fun,
     )
-    
- 
+
+
 if __name__ == '__main__':
-    main()  
+    main()
```

### Comparing `disdrodb-0.0.8/disdrodb/L0/standards.py` & `disdrodb-0.0.9/disdrodb/L0/standards.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/L0/template_tools.py` & `disdrodb-0.0.9/disdrodb/L0/template_tools.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/L0/utils_nc.py` & `disdrodb-0.0.9/disdrodb/L0/utils_nc.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/L1/utils.py` & `disdrodb-0.0.9/disdrodb/L1/utils.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/pipeline/run_ARM_processing.py` & `disdrodb-0.0.9/disdrodb/pipeline/run_ARM_processing.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/pipeline/run_DELFT_processing.py` & `disdrodb-0.0.9/disdrodb/pipeline/run_DELFT_processing.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/pipeline/run_DIVEN_processing.py` & `disdrodb-0.0.9/disdrodb/pipeline/run_DIVEN_processing.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/pipeline/run_EPFL_processing.py` & `disdrodb-0.0.9/disdrodb/pipeline/run_EPFL_processing.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/pipeline/utils_cmd.py` & `disdrodb-0.0.9/disdrodb/pipeline/utils_cmd.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb/utils/logger.py` & `disdrodb-0.0.9/disdrodb/utils/logger.py`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/disdrodb.egg-info/PKG-INFO` & `disdrodb-0.0.9/disdrodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disdrodb
-Version: 0.0.8
+Version: 0.0.9
 Summary: This package provides tools to homogenize, process, and analyze global disdrometer data.
 Author: Gionata Ghiggi
 Author-email: 
 Keywords: python,disdrometer
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `disdrodb-0.0.8/disdrodb.egg-info/SOURCES.txt` & `disdrodb-0.0.9/disdrodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `disdrodb-0.0.8/setup.py` & `disdrodb-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = 'v0.0.8'
+VERSION = 'v0.0.9'
 DESCRIPTION = "This package provides tools to homogenize, process, and analyze global disdrometer data."
 
 
 
 # Setting up
 setup(
     name="disdrodb",
```

