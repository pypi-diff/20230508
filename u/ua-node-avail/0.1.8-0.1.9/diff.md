# Comparing `tmp/ua-node-avail-0.1.8.tar.gz` & `tmp/ua-node-avail-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ua-node-avail-0.1.8.tar", last modified: Mon Jan  9 20:48:33 2023, max compression
+gzip compressed data, was "ua-node-avail-0.1.9.tar", last modified: Wed Jan 11 18:09:10 2023, max compression
```

## Comparing `ua-node-avail-0.1.8.tar` & `ua-node-avail-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tgmaxson (182810) chem_dixon   (405)        0 2023-01-09 20:48:32.993253 ua-node-avail-0.1.8/
--rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)     3249 2023-01-09 20:48:32.988511 ua-node-avail-0.1.8/PKG-INFO
--rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)     2815 2023-01-09 20:42:52.000000 ua-node-avail-0.1.8/README.md
-drwxr-xr-x   0 tgmaxson (182810) chem_dixon   (405)        0 2023-01-09 20:48:32.837454 ua-node-avail-0.1.8/bin/
--rwxr-xr-x   0 tgmaxson (182810) chem_dixon   (405)     2124 2023-01-09 20:44:17.000000 ua-node-avail-0.1.8/bin/job_memcheck
--rwxr-xr-x   0 tgmaxson (182810) chem_dixon   (405)     4584 2023-01-09 20:42:52.000000 ua-node-avail-0.1.8/bin/node_avail
--rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)       38 2023-01-09 20:48:32.993163 ua-node-avail-0.1.8/setup.cfg
--rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)      894 2023-01-09 20:48:17.000000 ua-node-avail-0.1.8/setup.py
-drwxr-xr-x   0 tgmaxson (182810) chem_dixon   (405)        0 2023-01-09 20:48:32.981665 ua-node-avail-0.1.8/ua_node_avail.egg-info/
--rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)     3249 2023-01-09 20:48:32.000000 ua-node-avail-0.1.8/ua_node_avail.egg-info/PKG-INFO
--rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)      234 2023-01-09 20:48:32.000000 ua-node-avail-0.1.8/ua_node_avail.egg-info/SOURCES.txt
--rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)        1 2023-01-09 20:48:32.000000 ua-node-avail-0.1.8/ua_node_avail.egg-info/dependency_links.txt
--rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)        9 2023-01-09 20:48:32.000000 ua-node-avail-0.1.8/ua_node_avail.egg-info/requires.txt
--rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)        1 2023-01-09 20:48:32.000000 ua-node-avail-0.1.8/ua_node_avail.egg-info/top_level.txt
+drwxr-xr-x   0 tgmaxson (182810) chem_dixon   (405)        0 2023-01-11 18:09:10.412081 ua-node-avail-0.1.9/
+-rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)     3249 2023-01-11 18:09:10.408611 ua-node-avail-0.1.9/PKG-INFO
+-rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)     2815 2023-01-09 20:42:52.000000 ua-node-avail-0.1.9/README.md
+drwxr-xr-x   0 tgmaxson (182810) chem_dixon   (405)        0 2023-01-11 18:09:10.368092 ua-node-avail-0.1.9/bin/
+-rwxr-xr-x   0 tgmaxson (182810) chem_dixon   (405)     2163 2023-01-11 18:08:36.000000 ua-node-avail-0.1.9/bin/job_memcheck
+-rwxr-xr-x   0 tgmaxson (182810) chem_dixon   (405)     4584 2023-01-09 20:42:52.000000 ua-node-avail-0.1.9/bin/node_avail
+-rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)       38 2023-01-11 18:09:10.412801 ua-node-avail-0.1.9/setup.cfg
+-rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)      894 2023-01-11 18:08:54.000000 ua-node-avail-0.1.9/setup.py
+drwxr-xr-x   0 tgmaxson (182810) chem_dixon   (405)        0 2023-01-11 18:09:10.401079 ua-node-avail-0.1.9/ua_node_avail.egg-info/
+-rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)     3249 2023-01-11 18:09:09.000000 ua-node-avail-0.1.9/ua_node_avail.egg-info/PKG-INFO
+-rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)      234 2023-01-11 18:09:10.000000 ua-node-avail-0.1.9/ua_node_avail.egg-info/SOURCES.txt
+-rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)        1 2023-01-11 18:09:09.000000 ua-node-avail-0.1.9/ua_node_avail.egg-info/dependency_links.txt
+-rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)        9 2023-01-11 18:09:09.000000 ua-node-avail-0.1.9/ua_node_avail.egg-info/requires.txt
+-rw-r--r--   0 tgmaxson (182810) chem_dixon   (405)        1 2023-01-11 18:09:09.000000 ua-node-avail-0.1.9/ua_node_avail.egg-info/top_level.txt
```

### Comparing `ua-node-avail-0.1.8/PKG-INFO` & `ua-node-avail-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ua-node-avail
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tool to monitor node availablility at UA
 Author: Tristan Maxson
 Author-email: tgmaxson@gmail.com
 Project-URL: Gitlab, https://gitlab.com/szilvasi-lab/ua-node-avail
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `ua-node-avail-0.1.8/README.md` & `ua-node-avail-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ua-node-avail-0.1.8/bin/job_memcheck` & `ua-node-avail-0.1.9/bin/job_memcheck`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
                 sub_parts = part.split("=")
                 if sub_parts[0] == key and len(sub_parts) > 1:
                     return "=".join(sub_parts[1:]).strip()
             return None
 
 chpc_mem_limits = {"main": 4,
                    "osg_main": 4,
+                   "long": 4,
                    "highmem": 2048,
                    "gpu": 4}
 
 def read_sinfo_jobs():
     job_info = []
 
     sinfo = Popen("scontrol show job", shell=True, stdout=PIPE)
@@ -45,15 +46,15 @@
             mem /= 1000
         
         cpu = float(key_equal_val("cpu", TRES))
         mem_per_cpu = mem/cpu
 
         mem_violation = False
         if is_chpc:
-            mem_limit = chpc_mem_limits[qos]
+            mem_limit = chpc_mem_limits.get("qos", 4)
             if mem_per_cpu > mem_limit:
                 mem_violation = True
         else:
             mem_violation = "???"
 
         if mem_violation == True:
             bad_jobs.append(jobid)
```

### Comparing `ua-node-avail-0.1.8/bin/node_avail` & `ua-node-avail-0.1.9/bin/node_avail`

 * *Files identical despite different names*

### Comparing `ua-node-avail-0.1.8/setup.py` & `ua-node-avail-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 
 setuptools.setup(
         name="ua-node-avail",
-        version="0.1.8",
+        version="0.1.9",
         scripts=['bin/node_avail', "bin/job_memcheck"],
         author="Tristan Maxson",
         author_email="tgmaxson@gmail.com",
         description="Tool to monitor node availablility at UA",
         long_description=long_description,
         long_description_content_type="text/markdown",
         project_urls={
```

### Comparing `ua-node-avail-0.1.8/ua_node_avail.egg-info/PKG-INFO` & `ua-node-avail-0.1.9/ua_node_avail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ua-node-avail
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tool to monitor node availablility at UA
 Author: Tristan Maxson
 Author-email: tgmaxson@gmail.com
 Project-URL: Gitlab, https://gitlab.com/szilvasi-lab/ua-node-avail
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
```

