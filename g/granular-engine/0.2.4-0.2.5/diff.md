# Comparing `tmp/granular_engine-0.2.4.tar.gz` & `tmp/granular_engine-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "granular_engine-0.2.4.tar", max compression
+gzip compressed data, was "granular_engine-0.2.5.tar", max compression
```

## Comparing `granular_engine-0.2.4.tar` & `granular_engine-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rwxr-xr-x   0        0        0      743 2023-05-01 16:39:46.439016 granular_engine-0.2.4/README.rst
--rwxr-xr-x   0        0        0      238 2023-05-02 13:15:39.797637 granular_engine-0.2.4/engine/__init__.py
--rwxr-xr-x   0        0        0      881 2023-05-02 13:15:25.911286 granular_engine-0.2.4/engine/cli/__init__.py
--rwxr-xr-x   0        0        0     1608 2023-05-01 16:39:24.293915 granular_engine-0.2.4/engine/cli/auth.py
--rwxr-xr-x   0        0        0     4048 2023-05-02 13:15:25.914292 granular_engine-0.2.4/engine/cli/experiment.py
--rwxr-xr-x   0        0        0     7816 2023-05-01 16:41:21.750990 granular_engine-0.2.4/engine/cli/project.py
--rwxr-xr-x   0        0        0      158 2023-05-01 16:39:24.340790 granular_engine-0.2.4/engine/connections/__init__.py
--rwxr-xr-x   0        0        0     5206 2023-05-01 16:39:24.356418 granular_engine-0.2.4/engine/connections/callisto.py
--rwxr-xr-x   0        0        0     4798 2023-05-02 13:15:25.929939 granular_engine-0.2.4/engine/connections/dione.py
--rwxr-xr-x   0        0        0     4969 2023-05-02 12:23:44.392111 granular_engine-0.2.4/engine/connections/europa.py
--rwxr-xr-x   0        0        0     1238 2023-05-01 16:41:21.782633 granular_engine-0.2.4/engine/connections/neso.py
--rwxr-xr-x   0        0        0     3528 2022-12-29 23:25:52.433705 granular_engine-0.2.4/engine/grain.py
--rwxr-xr-x   0        0        0        0 2023-05-01 16:39:24.387667 granular_engine-0.2.4/engine/libs/__init__.py
--rwxr-xr-x   0        0        0     1240 2023-05-01 16:39:24.418916 granular_engine-0.2.4/engine/libs/inquirer.py
--rwxr-xr-x   0        0        0     1208 2023-05-02 13:15:39.782000 granular_engine-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1855 1970-01-01 00:00:00.000000 granular_engine-0.2.4/setup.py
--rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 granular_engine-0.2.4/PKG-INFO
+-rwxr-xr-x   0        0        0      743 2023-05-01 16:39:46.439016 granular_engine-0.2.5/README.rst
+-rwxr-xr-x   0        0        0      210 2023-05-07 22:14:36.978198 granular_engine-0.2.5/engine/__init__.py
+-rwxr-xr-x   0        0        0      881 2023-05-02 13:15:25.911286 granular_engine-0.2.5/engine/cli/__init__.py
+-rwxr-xr-x   0        0        0     1608 2023-05-01 16:39:24.293915 granular_engine-0.2.5/engine/cli/auth.py
+-rwxr-xr-x   0        0        0     4081 2023-05-07 09:47:59.211514 granular_engine-0.2.5/engine/cli/experiment.py
+-rwxr-xr-x   0        0        0     7657 2023-05-07 22:14:20.680298 granular_engine-0.2.5/engine/cli/project.py
+-rwxr-xr-x   0        0        0      158 2023-05-01 16:39:24.340790 granular_engine-0.2.5/engine/connections/__init__.py
+-rwxr-xr-x   0        0        0     5206 2023-05-03 13:48:02.394840 granular_engine-0.2.5/engine/connections/callisto.py
+-rwxr-xr-x   0        0        0     3855 2023-05-07 22:14:20.696334 granular_engine-0.2.5/engine/connections/dione.py
+-rwxr-xr-x   0        0        0     5886 2023-05-07 22:14:20.707358 granular_engine-0.2.5/engine/connections/europa.py
+-rwxr-xr-x   0        0        0     1281 2023-05-07 09:47:59.242275 granular_engine-0.2.5/engine/connections/neso.py
+-rwxr-xr-x   0        0        0     4747 2023-05-07 22:14:20.715879 granular_engine-0.2.5/engine/grain.py
+-rwxr-xr-x   0        0        0        0 2023-05-01 16:39:24.387667 granular_engine-0.2.5/engine/libs/__init__.py
+-rwxr-xr-x   0        0        0     1240 2023-05-01 16:39:24.418916 granular_engine-0.2.5/engine/libs/inquirer.py
+-rwxr-xr-x   0        0        0     1171 2023-05-07 22:14:36.973194 granular_engine-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1855 1970-01-01 00:00:00.000000 granular_engine-0.2.5/setup.py
+-rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 granular_engine-0.2.5/PKG-INFO
```

### Comparing `granular_engine-0.2.4/README.rst` & `granular_engine-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.4/engine/cli/__init__.py` & `granular_engine-0.2.5/engine/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.4/engine/cli/auth.py` & `granular_engine-0.2.5/engine/cli/auth.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.4/engine/cli/experiment.py` & `granular_engine-0.2.5/engine/cli/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
             message=f"Do you want to see {experiment_found['name']} details?",
             qmark="\U0001F4C2",
             amark="\U0001F4C2"
         )
     else:
         experiment_found = dione.get_experiment_by_name(projectId=project_found["id"],
                                                         experiment_name=name)
+        print (experiment_found)
         if not experiment_found:
             print (Fore.RED + name + Style.RESET_ALL + 
               " experiment does not exist.")
             return
         else:
             show_detail = True
```

### Comparing `granular_engine-0.2.4/engine/cli/project.py` & `granular_engine-0.2.5/engine/cli/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,14 +76,15 @@
             print (Fore.GREEN + "Sensors : " + Style.RESET_ALL, end="")
             if org:
                 neso = Neso(callisto, org["id"])
             else:
                 neso = Neso(callisto, None)
             sensor_ids = project['sensorIds']
             sensors = neso.get_sensors()
+            print (sensors)
             sensor_names = [sensors[sensor_id]["name"] for sensor_id in sensor_ids]
             print (Fore.GREEN + ', '.join(sensor_names) + Style.RESET_ALL)
 
         if project["problemType"]:
             print (Fore.GREEN + "Problem Type : " + Style.RESET_ALL, end="")
             print (Fore.GREEN + project['problemType'] + Style.RESET_ALL)
 
@@ -136,14 +137,15 @@
         if org:
             text += [("#3AB222", org['name']), ("#F7F7F7", "'s ")]
         text += [("#B4195D", project['name']),
                 ("#B5B7B4", " with "),
                 ("#B29822", export['name']),
                 ("#B5B7B4", " export?")]
         color_print(text)
+        
         if not callisto.user:
             print ()
             print ("You are not logged in. Engine library requires your organization information to generate experiment tracking configuration.")
             print ("Please login using " + Fore.CYAN + "engine login" + Style.RESET_ALL)
             return
 
         want_config = confirm(message="", qmark="\U0001F913", amark="\U0001F913")
@@ -165,27 +167,23 @@
                             "JSON", 
                             "Py config file for geo-libs"],
                     qmark="\U0001F4DD",
                     amark="\U0001F4DD"
                 )
                 print ()
 
-                
-                config = {"name": project["name"],
-                        "description": project["description"],
-                        "tags": project["tags"],
+                config = {
+                        "description": project["description"].replace('\n', ' ')[:200],
                         "org": project_org["slug"],
+                        "exportName": export["name"],
                         "exportId": export["id"],
+                        "projectName": project["name"],
                         "projectId": project["id"],
-                        "framework": "pytorch",
-                        "gitUrl": "",
-                        "metaInfo": "",
-                        "params": None,
-                        "inputs": None,
-                        "outputs": None}
+                        "tags": project["tags"]
+                        }
                 
                 save_path = filepath(
                     message="Please enter a path to save the configuration",
                     qmark="\U0001F4E9",
                     amark="\U0001F4E9"
                     )
                 if which_config == 'YAML':
@@ -203,13 +201,13 @@
                         json.dump(config, fout, indent=4)
                         print ("Saved to " + Fore.GREEN + save_path + Style.RESET_ALL)  
                 else:
                     if '.py' not in save_path:
                         save_path += '.py'
                     
                     with open(save_path, 'w') as fout:
-                        fout.write("_base_ = [\n\t'../_base_/default_runtime.py'\n]\n\n")
-                        pp = pprint.PrettyPrinter(indent=4)
+                        pp = pprint.PrettyPrinter(indent=4, width=200, compact=True)
                         fout.write(f"engine = {pp.pformat(config)}")
                         print ("Saved to " + Fore.GREEN + save_path + Style.RESET_ALL)
-                            
+
+                print ()
     return
```

### Comparing `granular_engine-0.2.4/engine/connections/callisto.py` & `granular_engine-0.2.5/engine/connections/callisto.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.4/engine/connections/dione.py` & `granular_engine-0.2.5/engine/connections/dione.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,45 +19,37 @@
         assert experiment["exportId"], "No exportId given"
 
         url = f'{self.callisto.host}/dione/api/v1/experiments?orgId={self.org}'
         response = requests.post(url=url, data=json.dumps(experiment), 
                                  headers=self.callisto.headers)
 
         if response.status_code == 200:
-            experiment_id = response.json()["experiment"]["id"]
-            return experiment_id
+            experiment = response.json()
+            return experiment
         else:
             print (response.json())
             print ("Failed to create experiment")
             return None
-
-    def add_best_model(self, experimentId, model_path):
+    
+    def update_experiment(self, experiment):
         assert self.org, "No org slug passed"
-        url = f'{self.callisto.host}/dione/api/v1/experiments/{experimentId}?orgId={self.org}'
-        data = json.dumps({ "bestModel": model_path})
-        response = requests.put(
-                                url=url,
-                                data=data,
-                                headers=self.callisto.headers
-                                )  
+        assert isinstance(experiment, dict), "Experiment should be dictionary"
+        assert experiment["id"], "No experiment id given"
+
+        url = f"{self.callisto.host}/dione/api/v1/experiments/{experiment['id']}?orgId={self.org}"
+        response = requests.put(url=url, data=json.dumps(experiment), 
+                                 headers=self.callisto.headers)
+
         if response.status_code == 200:
-            print ("Experiment updated with best model path")
+            experiment = response.json()
+            return experiment
         else:
-            print ("Failed to update experiment with best model path!")
-
-    def experiment_done(self, experimentId):
-        assert self.org, "No org slug passed"
-        url = f'{self.callisto.host}/dione/api/v1/experiments/{experimentId}?orgId={self.org}'
-        response = requests.put(
-                                url=url,
-                                data=json.dumps({ "status": "success"}),
-                                headers=self.callisto.headers
-                                )  
-        if response.status_code != 200:
-            print ("Failed to update experiment status")
+            print (response.json())
+            print (f"Failed to update experiment {experiment['name']}")
+            return None
 
     def get_experiments(self, projectId):
         assert self.org, "No org slug passed"
         assert projectId, "No projectId given"
 
         get_experiment_url = f'{self.callisto.host}/dione/api/v1/experiments?orgId={self.org}&projectId={projectId}&perPage=1000'
         response = requests.get(get_experiment_url, headers=self.callisto.headers)
@@ -98,20 +90,8 @@
                                 headers=self.callisto.headers)
 
         if response.status_code == 200:
             artifact_id = response.json()["artifact"]["id"]
             return artifact_id
         else:
             print ("Failed to create artifact")
-            return None
-
-    def send_heartbeat(self, experimentId):
-        url = f'{self.callisto.host}/dione/api/v1/experiments/{experimentId}?orgId={self.org}'
-
-        response = requests.patch(url=url, data={}, headers=self.callisto.headers)
-
-        if response.status_code == 200:
-            experiment_status = response.json()["experiment"]["status"]
-            return experiment_status
-        else:
-            print ("Failed to send heartbeat")
             return None
```

### Comparing `granular_engine-0.2.4/engine/connections/europa.py` & `granular_engine-0.2.5/engine/connections/europa.py`

 * *Files 10% similar despite different names*

```diff
@@ -116,8 +116,26 @@
             exports = response.json()['results']
             exports = {export["name"]: export for export in exports}
             
             return exports
         else:
             print(f'All exports for GeoEngine project {id} cannot be retrieved')
             print(f'Exports endpoint {project_exports_url} returned with HTTP status code : {response.status_code}\n')
+            return None
+        
+    def get_project_export_by_id(self, project_id, export_id):
+        if self.org:
+            project_export_url = f'{self.callisto.host}/europa/api/v2/projects/{project_id}/datasets/{export_id}?orgId={self.org}'
+        else:
+            project_export_url = f"{self.callisto.host}/europa/api/v2/projects/{project_id}/datasets/{export_id}?search=&status=all&isPublic=true"
+
+        response = requests.get(project_export_url, headers=self.callisto.headers)
+        
+        response = requests.get(project_export_url, headers=self.callisto.headers)
+
+        if response.status_code == 200:
+            export = response.json()
+            return export
+        else:
+            print(f'Export {export_id} for GeoEngine project {project_id} cannot be retrieved')
+            print(f'Exports endpoint {project_export_url} returned with HTTP status code : {response.status_code}\n')
             return None
```

### Comparing `granular_engine-0.2.4/engine/connections/neso.py` & `granular_engine-0.2.5/engine/connections/neso.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 class Neso:
     def __init__(self, callisto=None, org=None):
         self.callisto = callisto 
         self.org = org 
 
     def get_sensors(self):
         if self.org:
-            sensor_url = f'{self.callisto.host}/neso/api/v1/sensors?orgId={self.org}'
+            sensor_url = f'{self.callisto.host}/neso/api/v1/sensors?orgId={self.org}&perPage=1000'
         else:
-            sensor_url = f'{self.callisto.host}/neso/api/v1/sensors'
+            sensor_url = f'{self.callisto.host}/neso/api/v1/sensors?isPublic=true&perPage=1000'
 
         response  = requests.get(sensor_url, headers=self.callisto.headers)
 
         if response.status_code == 200:
-            sensors = response.json()['data']
+            sensors = response.json()['results']
             return {sensor["id"]: sensor for sensor in sensors}
 
         else:
             print(f"Sensor details cannot be retrieved")
             return None
         
     def get_sensor_by_id(self, sensor_id):
```

### Comparing `granular_engine-0.2.4/engine/libs/inquirer.py` & `granular_engine-0.2.5/engine/libs/inquirer.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.4/pyproject.toml` & `granular_engine-0.2.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "granular-engine"
-version = "v0.2.4"
+version = "v0.2.5"
 description = "Experiment tracking for GeoSpatial Machine Learning on GeoEngine"
-authors = ["Sagar Verma <sagar@granular.ai>", "Siddharth Gupta <sid@granular.ai>"]
+authors = ["Sagar Verma <sagar@granular.ai>"]
 license = "MIT"
 readme = "README.rst"
 packages = [{include = "engine"}]
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Natural Language :: English',
```

### Comparing `granular_engine-0.2.4/setup.py` & `granular_engine-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'yacs>=0.1.8,<0.2.0']
 
 entry_points = \
 {'console_scripts': ['engine = engine.cli:cli']}
 
 setup_kwargs = {
     'name': 'granular-engine',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'Experiment tracking for GeoSpatial Machine Learning on GeoEngine',
     'long_description': 'Engine\n======\n\nA Utility Library that assists in Geospatial Machine Learning Experiment\nTracking.\n\nInstallation\n------------\n\n.. code:: shell\n\n   pip install granular-engine\n\nUsage\n-----\n\nCLI\n~~~\n\n.. figure:: https://user-images.githubusercontent.com/2713531/210276844-16d3867d-461c-44ba-870b-00d6d6266dbf.gif\n   :alt: engine_cli\n\n   engine_cli\n\nExperiment Tracking\n~~~~~~~~~~~~~~~~~~~\n\n.. code:: python\n\n   from engine import Engine\n\n   engine = Engine("test_config.yaml")\n\n   for epoch in enumerate(epochs):\n      # train \n      # eval\n      engine.log(step=epoch, train_loss=train_loss, val_loss=val_loss)\n\n   engine.done()\n\nLicense\n-------\n\nGPLv3\n\nDocumentation\n-------------\n\nView documentation ``here <https://engine.granular.ai/>``\\ \\_\n',
     'author': 'Sagar Verma',
     'author_email': 'sagar@granular.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/granularai/engine',
```

### Comparing `granular_engine-0.2.4/PKG-INFO` & `granular_engine-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granular-engine
-Version: 0.2.4
+Version: 0.2.5
 Summary: Experiment tracking for GeoSpatial Machine Learning on GeoEngine
 Home-page: https://github.com/granularai/engine
 License: MIT
 Author: Sagar Verma
 Author-email: sagar@granular.ai
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: Intended Audience :: Developers
```

