# Comparing `tmp/granular_engine-0.2.5.tar.gz` & `tmp/granular_engine-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "granular_engine-0.2.5.tar", max compression
+gzip compressed data, was "granular_engine-0.2.6.tar", max compression
```

## Comparing `granular_engine-0.2.5.tar` & `granular_engine-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rwxr-xr-x   0        0        0      743 2023-05-01 16:39:46.439016 granular_engine-0.2.5/README.rst
--rwxr-xr-x   0        0        0      210 2023-05-07 22:14:36.978198 granular_engine-0.2.5/engine/__init__.py
--rwxr-xr-x   0        0        0      881 2023-05-02 13:15:25.911286 granular_engine-0.2.5/engine/cli/__init__.py
--rwxr-xr-x   0        0        0     1608 2023-05-01 16:39:24.293915 granular_engine-0.2.5/engine/cli/auth.py
--rwxr-xr-x   0        0        0     4081 2023-05-07 09:47:59.211514 granular_engine-0.2.5/engine/cli/experiment.py
--rwxr-xr-x   0        0        0     7657 2023-05-07 22:14:20.680298 granular_engine-0.2.5/engine/cli/project.py
--rwxr-xr-x   0        0        0      158 2023-05-01 16:39:24.340790 granular_engine-0.2.5/engine/connections/__init__.py
--rwxr-xr-x   0        0        0     5206 2023-05-03 13:48:02.394840 granular_engine-0.2.5/engine/connections/callisto.py
--rwxr-xr-x   0        0        0     3855 2023-05-07 22:14:20.696334 granular_engine-0.2.5/engine/connections/dione.py
--rwxr-xr-x   0        0        0     5886 2023-05-07 22:14:20.707358 granular_engine-0.2.5/engine/connections/europa.py
--rwxr-xr-x   0        0        0     1281 2023-05-07 09:47:59.242275 granular_engine-0.2.5/engine/connections/neso.py
--rwxr-xr-x   0        0        0     4747 2023-05-07 22:14:20.715879 granular_engine-0.2.5/engine/grain.py
--rwxr-xr-x   0        0        0        0 2023-05-01 16:39:24.387667 granular_engine-0.2.5/engine/libs/__init__.py
--rwxr-xr-x   0        0        0     1240 2023-05-01 16:39:24.418916 granular_engine-0.2.5/engine/libs/inquirer.py
--rwxr-xr-x   0        0        0     1171 2023-05-07 22:14:36.973194 granular_engine-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1855 1970-01-01 00:00:00.000000 granular_engine-0.2.5/setup.py
--rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 granular_engine-0.2.5/PKG-INFO
+-rwxr-xr-x   0        0        0      743 2023-05-01 16:39:46.439016 granular_engine-0.2.6/README.rst
+-rwxr-xr-x   0        0        0      210 2023-05-08 08:52:47.445743 granular_engine-0.2.6/engine/__init__.py
+-rwxr-xr-x   0        0        0      881 2023-05-02 13:15:25.911286 granular_engine-0.2.6/engine/cli/__init__.py
+-rwxr-xr-x   0        0        0     1608 2023-05-01 16:39:24.293915 granular_engine-0.2.6/engine/cli/auth.py
+-rwxr-xr-x   0        0        0     4081 2023-05-07 09:47:59.211514 granular_engine-0.2.6/engine/cli/experiment.py
+-rwxr-xr-x   0        0        0     7657 2023-05-07 22:14:20.680298 granular_engine-0.2.6/engine/cli/project.py
+-rwxr-xr-x   0        0        0      158 2023-05-01 16:39:24.340790 granular_engine-0.2.6/engine/connections/__init__.py
+-rwxr-xr-x   0        0        0     5206 2023-05-03 13:48:02.394840 granular_engine-0.2.6/engine/connections/callisto.py
+-rwxr-xr-x   0        0        0     4350 2023-05-08 08:52:31.363502 granular_engine-0.2.6/engine/connections/dione.py
+-rwxr-xr-x   0        0        0     5878 2023-05-08 08:52:31.374822 granular_engine-0.2.6/engine/connections/europa.py
+-rwxr-xr-x   0        0        0     1281 2023-05-07 09:47:59.242275 granular_engine-0.2.6/engine/connections/neso.py
+-rwxr-xr-x   0        0        0     4754 2023-05-08 08:52:31.383917 granular_engine-0.2.6/engine/grain.py
+-rwxr-xr-x   0        0        0        0 2023-05-01 16:39:24.387667 granular_engine-0.2.6/engine/libs/__init__.py
+-rwxr-xr-x   0        0        0     1240 2023-05-01 16:39:24.418916 granular_engine-0.2.6/engine/libs/inquirer.py
+-rwxr-xr-x   0        0        0     1171 2023-05-08 08:52:47.440744 granular_engine-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1855 1970-01-01 00:00:00.000000 granular_engine-0.2.6/setup.py
+-rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 granular_engine-0.2.6/PKG-INFO
```

### Comparing `granular_engine-0.2.5/README.rst` & `granular_engine-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.5/engine/cli/__init__.py` & `granular_engine-0.2.6/engine/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.5/engine/cli/auth.py` & `granular_engine-0.2.6/engine/cli/auth.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.5/engine/cli/experiment.py` & `granular_engine-0.2.6/engine/cli/experiment.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.5/engine/cli/project.py` & `granular_engine-0.2.6/engine/cli/project.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.5/engine/connections/callisto.py` & `granular_engine-0.2.6/engine/connections/callisto.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.5/engine/connections/dione.py` & `granular_engine-0.2.6/engine/connections/dione.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         assert experiment["exportId"], "No exportId given"
 
         url = f'{self.callisto.host}/dione/api/v1/experiments?orgId={self.org}'
         response = requests.post(url=url, data=json.dumps(experiment), 
                                  headers=self.callisto.headers)
 
         if response.status_code == 200:
-            experiment = response.json()
+            experiment = response.json()['experiment']
             return experiment
         else:
             print (response.json())
             print ("Failed to create experiment")
             return None
     
     def update_experiment(self, experiment):
@@ -36,15 +36,15 @@
         assert experiment["id"], "No experiment id given"
 
         url = f"{self.callisto.host}/dione/api/v1/experiments/{experiment['id']}?orgId={self.org}"
         response = requests.put(url=url, data=json.dumps(experiment), 
                                  headers=self.callisto.headers)
 
         if response.status_code == 200:
-            experiment = response.json()
+            experiment = response.json()['experiment']
             return experiment
         else:
             print (response.json())
             print (f"Failed to update experiment {experiment['name']}")
             return None
 
     def get_experiments(self, projectId):
@@ -90,8 +90,20 @@
                                 headers=self.callisto.headers)
 
         if response.status_code == 200:
             artifact_id = response.json()["artifact"]["id"]
             return artifact_id
         else:
             print ("Failed to create artifact")
+            return None
+        
+    def send_heartbeat(self, experimentId):
+        url = f'{self.callisto.host}/dione/api/v1/experiments/{experimentId}?orgId={self.org}'
+
+        response = requests.patch(url=url, data={}, headers=self.callisto.headers)
+
+        if response.status_code == 200:
+            experiment_status = response.json()["experiment"]["status"]
+            return experiment_status
+        else:
+            print ("Failed to send heartbeat")
             return None
```

### Comparing `granular_engine-0.2.5/engine/connections/europa.py` & `granular_engine-0.2.6/engine/connections/europa.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             project_details_url = f'{self.callisto.host}/europa/api/v2/projects/{id}?orgId={self.org}'
         else:
             project_details_url = f"{self.callisto.host}/europa/api/v2/projects/{id}?search=&status=all&isPublic=true"
 
         response = requests.get(project_details_url, headers=self.callisto.headers)
         
         if response.status_code == 200:
-            project = response.json()['task']
+            project = response.json()
             
             if verbose:
                 ignorelist = ['populateCounter', 'owner', 'createdAt', 'updatedAt', 'deteledAt', 'annotators']
                 print('\Project Details:\n')
             
                 for key in project.keys():
                     if key == 'questions':
```

### Comparing `granular_engine-0.2.5/engine/connections/neso.py` & `granular_engine-0.2.6/engine/connections/neso.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.5/engine/grain.py` & `granular_engine-0.2.6/engine/grain.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,22 +87,22 @@
         self._heartbeat_thread.start()
     
     def _heartbeat(self):
         while True:
             if self._exit_flag:
                 return
   
-            _ = self.dione.update_experiment(self.experiment)
+            _ = self.dione.send_heartbeat(self.experiment["id"])
 
             # TODO: experiment status can be used to stop an experiment from UI side by ckecking the status
 
             time.sleep(5)
 
     def log(self, step, best=False, checkpoint_path=None, **kwargs):
-        artifact = {"experimentId": self.experimentId,
+        artifact = {"experimentId": self.experiment['id'],
                     "metadata": kwargs,
                     "step": step}
         if checkpoint_path:
             dst_state_path = f"{self.meta['experimentUrl']}/weights/"
             os.system(f"gsutil rsync {checkpoint_path} {dst_state_path} 2> /dev/null")
             artifact["metadata"]["checkpoint"] = f"{dst_state_path}{checkpoint_path.split('/')[-1]}"
```

### Comparing `granular_engine-0.2.5/engine/libs/inquirer.py` & `granular_engine-0.2.6/engine/libs/inquirer.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.5/pyproject.toml` & `granular_engine-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "granular-engine"
-version = "v0.2.5"
+version = "v0.2.6"
 description = "Experiment tracking for GeoSpatial Machine Learning on GeoEngine"
 authors = ["Sagar Verma <sagar@granular.ai>"]
 license = "MIT"
 readme = "README.rst"
 packages = [{include = "engine"}]
 classifiers = [
     'Intended Audience :: Developers',
```

### Comparing `granular_engine-0.2.5/setup.py` & `granular_engine-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'yacs>=0.1.8,<0.2.0']
 
 entry_points = \
 {'console_scripts': ['engine = engine.cli:cli']}
 
 setup_kwargs = {
     'name': 'granular-engine',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'Experiment tracking for GeoSpatial Machine Learning on GeoEngine',
     'long_description': 'Engine\n======\n\nA Utility Library that assists in Geospatial Machine Learning Experiment\nTracking.\n\nInstallation\n------------\n\n.. code:: shell\n\n   pip install granular-engine\n\nUsage\n-----\n\nCLI\n~~~\n\n.. figure:: https://user-images.githubusercontent.com/2713531/210276844-16d3867d-461c-44ba-870b-00d6d6266dbf.gif\n   :alt: engine_cli\n\n   engine_cli\n\nExperiment Tracking\n~~~~~~~~~~~~~~~~~~~\n\n.. code:: python\n\n   from engine import Engine\n\n   engine = Engine("test_config.yaml")\n\n   for epoch in enumerate(epochs):\n      # train \n      # eval\n      engine.log(step=epoch, train_loss=train_loss, val_loss=val_loss)\n\n   engine.done()\n\nLicense\n-------\n\nGPLv3\n\nDocumentation\n-------------\n\nView documentation ``here <https://engine.granular.ai/>``\\ \\_\n',
     'author': 'Sagar Verma',
     'author_email': 'sagar@granular.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/granularai/engine',
```

### Comparing `granular_engine-0.2.5/PKG-INFO` & `granular_engine-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granular-engine
-Version: 0.2.5
+Version: 0.2.6
 Summary: Experiment tracking for GeoSpatial Machine Learning on GeoEngine
 Home-page: https://github.com/granularai/engine
 License: MIT
 Author: Sagar Verma
 Author-email: sagar@granular.ai
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: Intended Audience :: Developers
```

