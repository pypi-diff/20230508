# Comparing `tmp/service-configuration-lib-2.8.0.tar.gz` & `tmp/service-configuration-lib-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/service-configuration-lib-2.8.0.tar", last modified: Thu Jan  6 23:19:17 2022, max compression
+gzip compressed data, was "dist/service-configuration-lib-2.9.0.tar", last modified: Mon Jan 31 23:39:35 2022, max compression
```

## Comparing `service-configuration-lib-2.8.0.tar` & `service-configuration-lib-2.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 23:19:17.000000 service-configuration-lib-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-01-06 23:19:17.000000 service-configuration-lib-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-01-06 23:19:17.000000 service-configuration-lib-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-01-06 23:19:10.000000 service-configuration-lib-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 23:19:17.000000 service-configuration-lib-2.8.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)      783 2022-01-06 23:19:10.000000 service-configuration-lib-2.8.0/scripts/services_needing_puppet_help
--rwxr-xr-x   0 runner    (1001) docker     (121)      780 2022-01-06 23:19:10.000000 service-configuration-lib-2.8.0/scripts/services_deployed_here
--rwxr-xr-x   0 runner    (1001) docker     (121)      783 2022-01-06 23:19:10.000000 service-configuration-lib-2.8.0/scripts/all_nodes_that_receive
--rwxr-xr-x   0 runner    (1001) docker     (121)      780 2022-01-06 23:19:10.000000 service-configuration-lib-2.8.0/scripts/services_that_run_here
--rwxr-xr-x   0 runner    (1001) docker     (121)      779 2022-01-06 23:19:10.000000 service-configuration-lib-2.8.0/scripts/all_nodes_that_run
--rwxr-xr-x   0 runner    (1001) docker     (121)      799 2022-01-06 23:19:10.000000 service-configuration-lib-2.8.0/scripts/dump_service_configuration_yaml
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-01-06 23:19:10.000000 service-configuration-lib-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 23:19:17.000000 service-configuration-lib-2.8.0/service_configuration_lib/
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-01-06 23:19:10.000000 service-configuration-lib-2.8.0/service_configuration_lib/yaml_cached_view.py
--rw-r--r--   0 runner    (1001) docker     (121)    34594 2022-01-06 23:19:10.000000 service-configuration-lib-2.8.0/service_configuration_lib/spark_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    10483 2022-01-06 23:19:10.000000 service-configuration-lib-2.8.0/service_configuration_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10272 2022-01-06 23:19:10.000000 service-configuration-lib-2.8.0/service_configuration_lib/cached_view.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 23:19:17.000000 service-configuration-lib-2.8.0/service_configuration_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-06 23:19:17.000000 service-configuration-lib-2.8.0/service_configuration_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-06 23:19:17.000000 service-configuration-lib-2.8.0/service_configuration_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-01-06 23:19:17.000000 service-configuration-lib-2.8.0/service_configuration_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-01-06 23:19:17.000000 service-configuration-lib-2.8.0/service_configuration_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-01-06 23:19:17.000000 service-configuration-lib-2.8.0/service_configuration_lib.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 23:39:35.000000 service-configuration-lib-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-01-31 23:39:35.000000 service-configuration-lib-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-01-31 23:39:35.000000 service-configuration-lib-2.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 23:39:35.000000 service-configuration-lib-2.9.0/service_configuration_lib/
+-rw-r--r--   0 runner    (1001) docker     (121)    34594 2022-01-31 23:39:29.000000 service-configuration-lib-2.9.0/service_configuration_lib/spark_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10272 2022-01-31 23:39:29.000000 service-configuration-lib-2.9.0/service_configuration_lib/cached_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-01-31 23:39:29.000000 service-configuration-lib-2.9.0/service_configuration_lib/yaml_cached_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10672 2022-01-31 23:39:29.000000 service-configuration-lib-2.9.0/service_configuration_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-01-31 23:39:29.000000 service-configuration-lib-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 23:39:35.000000 service-configuration-lib-2.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      780 2022-01-31 23:39:29.000000 service-configuration-lib-2.9.0/scripts/services_that_run_here
+-rwxr-xr-x   0 runner    (1001) docker     (121)      783 2022-01-31 23:39:29.000000 service-configuration-lib-2.9.0/scripts/all_nodes_that_receive
+-rwxr-xr-x   0 runner    (1001) docker     (121)      779 2022-01-31 23:39:29.000000 service-configuration-lib-2.9.0/scripts/all_nodes_that_run
+-rwxr-xr-x   0 runner    (1001) docker     (121)      799 2022-01-31 23:39:29.000000 service-configuration-lib-2.9.0/scripts/dump_service_configuration_yaml
+-rwxr-xr-x   0 runner    (1001) docker     (121)      780 2022-01-31 23:39:29.000000 service-configuration-lib-2.9.0/scripts/services_deployed_here
+-rwxr-xr-x   0 runner    (1001) docker     (121)      783 2022-01-31 23:39:29.000000 service-configuration-lib-2.9.0/scripts/services_needing_puppet_help
+-rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-01-31 23:39:29.000000 service-configuration-lib-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 23:39:35.000000 service-configuration-lib-2.9.0/service_configuration_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2022-01-31 23:39:35.000000 service-configuration-lib-2.9.0/service_configuration_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-01-31 23:39:35.000000 service-configuration-lib-2.9.0/service_configuration_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-31 23:39:35.000000 service-configuration-lib-2.9.0/service_configuration_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-01-31 23:39:35.000000 service-configuration-lib-2.9.0/service_configuration_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 23:39:35.000000 service-configuration-lib-2.9.0/service_configuration_lib.egg-info/dependency_links.txt
```

### Comparing `service-configuration-lib-2.8.0/setup.py` & `service-configuration-lib-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='service-configuration-lib',
-    version='2.8.0',
+    version='2.9.0',
     provides=['service_configuration_lib'],
     description='Start, stop, and inspect Yelp SOA services',
     url='https://github.com/Yelp/service_configuration_lib',
     author='Yelp Compute Infrastructure Team',
     author_email='opensource+scl@yelp.com',
     packages=find_packages(exclude=['tests', 'scripts']),
     install_requires=[
```

### Comparing `service-configuration-lib-2.8.0/scripts/services_needing_puppet_help` & `service-configuration-lib-2.9.0/scripts/services_needing_puppet_help`

 * *Files identical despite different names*

### Comparing `service-configuration-lib-2.8.0/scripts/services_deployed_here` & `service-configuration-lib-2.9.0/scripts/services_deployed_here`

 * *Files identical despite different names*

### Comparing `service-configuration-lib-2.8.0/scripts/all_nodes_that_receive` & `service-configuration-lib-2.9.0/scripts/all_nodes_that_receive`

 * *Files identical despite different names*

### Comparing `service-configuration-lib-2.8.0/scripts/services_that_run_here` & `service-configuration-lib-2.9.0/scripts/services_that_run_here`

 * *Files identical despite different names*

### Comparing `service-configuration-lib-2.8.0/scripts/all_nodes_that_run` & `service-configuration-lib-2.9.0/scripts/all_nodes_that_run`

 * *Files identical despite different names*

### Comparing `service-configuration-lib-2.8.0/scripts/dump_service_configuration_yaml` & `service-configuration-lib-2.9.0/scripts/dump_service_configuration_yaml`

 * *Files identical despite different names*

### Comparing `service-configuration-lib-2.8.0/README.md` & `service-configuration-lib-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `service-configuration-lib-2.8.0/service_configuration_lib/yaml_cached_view.py` & `service-configuration-lib-2.9.0/service_configuration_lib/yaml_cached_view.py`

 * *Files identical despite different names*

### Comparing `service-configuration-lib-2.8.0/service_configuration_lib/spark_config.py` & `service-configuration-lib-2.9.0/service_configuration_lib/spark_config.py`

 * *Files identical despite different names*

### Comparing `service-configuration-lib-2.8.0/service_configuration_lib/__init__.py` & `service-configuration-lib-2.9.0/service_configuration_lib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,19 @@
 
 
 def list_services(soa_dir=DEFAULT_SOA_DIR):
     rootdir = os.path.abspath(soa_dir)
     return os.listdir(rootdir)
 
 
+def read_soa_metadata(soa_dir=DEFAULT_SOA_DIR):
+    """Reads the metadata file in the SOA directory"""
+    return read_yaml_file(os.path.join(os.path.abspath(soa_dir), '.metadata.json'))
+
+
 def get_service_from_port(port, all_services=None):
     """Gets the name of the service from the port
     all_services allows you to feed in the services to look through, pass
     in a dict of service names to service information eg.
     {
         'service_name': {
             'port': port_number
```

### Comparing `service-configuration-lib-2.8.0/service_configuration_lib/cached_view.py` & `service-configuration-lib-2.9.0/service_configuration_lib/cached_view.py`

 * *Files identical despite different names*

### Comparing `service-configuration-lib-2.8.0/service_configuration_lib.egg-info/SOURCES.txt` & `service-configuration-lib-2.9.0/service_configuration_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

