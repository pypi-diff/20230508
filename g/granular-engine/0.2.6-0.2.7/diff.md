# Comparing `tmp/granular_engine-0.2.6.tar.gz` & `tmp/granular_engine-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "granular_engine-0.2.6.tar", max compression
+gzip compressed data, was "granular_engine-0.2.7.tar", max compression
```

## Comparing `granular_engine-0.2.6.tar` & `granular_engine-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rwxr-xr-x   0        0        0      743 2023-05-01 16:39:46.439016 granular_engine-0.2.6/README.rst
--rwxr-xr-x   0        0        0      210 2023-05-08 08:52:47.445743 granular_engine-0.2.6/engine/__init__.py
--rwxr-xr-x   0        0        0      881 2023-05-02 13:15:25.911286 granular_engine-0.2.6/engine/cli/__init__.py
--rwxr-xr-x   0        0        0     1608 2023-05-01 16:39:24.293915 granular_engine-0.2.6/engine/cli/auth.py
--rwxr-xr-x   0        0        0     4081 2023-05-07 09:47:59.211514 granular_engine-0.2.6/engine/cli/experiment.py
--rwxr-xr-x   0        0        0     7657 2023-05-07 22:14:20.680298 granular_engine-0.2.6/engine/cli/project.py
--rwxr-xr-x   0        0        0      158 2023-05-01 16:39:24.340790 granular_engine-0.2.6/engine/connections/__init__.py
--rwxr-xr-x   0        0        0     5206 2023-05-03 13:48:02.394840 granular_engine-0.2.6/engine/connections/callisto.py
--rwxr-xr-x   0        0        0     4350 2023-05-08 08:52:31.363502 granular_engine-0.2.6/engine/connections/dione.py
--rwxr-xr-x   0        0        0     5878 2023-05-08 08:52:31.374822 granular_engine-0.2.6/engine/connections/europa.py
--rwxr-xr-x   0        0        0     1281 2023-05-07 09:47:59.242275 granular_engine-0.2.6/engine/connections/neso.py
--rwxr-xr-x   0        0        0     4754 2023-05-08 08:52:31.383917 granular_engine-0.2.6/engine/grain.py
--rwxr-xr-x   0        0        0        0 2023-05-01 16:39:24.387667 granular_engine-0.2.6/engine/libs/__init__.py
--rwxr-xr-x   0        0        0     1240 2023-05-01 16:39:24.418916 granular_engine-0.2.6/engine/libs/inquirer.py
--rwxr-xr-x   0        0        0     1171 2023-05-08 08:52:47.440744 granular_engine-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1855 1970-01-01 00:00:00.000000 granular_engine-0.2.6/setup.py
--rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 granular_engine-0.2.6/PKG-INFO
+-rwxr-xr-x   0        0        0      743 2023-05-01 16:39:46.439016 granular_engine-0.2.7/README.rst
+-rwxr-xr-x   0        0        0      210 2023-05-08 21:01:26.577847 granular_engine-0.2.7/engine/__init__.py
+-rwxr-xr-x   0        0        0      881 2023-05-02 13:15:25.911286 granular_engine-0.2.7/engine/cli/__init__.py
+-rwxr-xr-x   0        0        0     1608 2023-05-01 16:39:24.293915 granular_engine-0.2.7/engine/cli/auth.py
+-rwxr-xr-x   0        0        0     4081 2023-05-07 09:47:59.211514 granular_engine-0.2.7/engine/cli/experiment.py
+-rwxr-xr-x   0        0        0    12512 2023-05-08 21:01:13.081169 granular_engine-0.2.7/engine/cli/project.py
+-rwxr-xr-x   0        0        0      158 2023-05-01 16:39:24.340790 granular_engine-0.2.7/engine/connections/__init__.py
+-rwxr-xr-x   0        0        0     5202 2023-05-08 21:01:13.100756 granular_engine-0.2.7/engine/connections/callisto.py
+-rwxr-xr-x   0        0        0     4350 2023-05-08 08:52:31.363502 granular_engine-0.2.7/engine/connections/dione.py
+-rwxr-xr-x   0        0        0     6310 2023-05-08 21:01:13.116774 granular_engine-0.2.7/engine/connections/europa.py
+-rwxr-xr-x   0        0        0     1281 2023-05-07 09:47:59.242275 granular_engine-0.2.7/engine/connections/neso.py
+-rwxr-xr-x   0        0        0     4754 2023-05-08 08:52:31.383917 granular_engine-0.2.7/engine/grain.py
+-rwxr-xr-x   0        0        0        0 2023-05-01 16:39:24.387667 granular_engine-0.2.7/engine/libs/__init__.py
+-rwxr-xr-x   0        0        0    46675 2023-05-08 21:01:13.134631 granular_engine-0.2.7/engine/libs/config.py
+-rwxr-xr-x   0        0        0     1453 2023-05-08 21:01:13.150663 granular_engine-0.2.7/engine/libs/inquirer.py
+-rwxr-xr-x   0        0        0     4607 2023-05-08 21:01:13.162994 granular_engine-0.2.7/engine/libs/utils.py
+-rwxr-xr-x   0        0        0     1252 2023-05-08 21:01:26.571328 granular_engine-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 granular_engine-0.2.7/PKG-INFO
```

### Comparing `granular_engine-0.2.6/README.rst` & `granular_engine-0.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.6/engine/cli/__init__.py` & `granular_engine-0.2.7/engine/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.6/engine/cli/auth.py` & `granular_engine-0.2.7/engine/cli/auth.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.6/engine/cli/experiment.py` & `granular_engine-0.2.7/engine/cli/experiment.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.6/engine/connections/callisto.py` & `granular_engine-0.2.7/engine/connections/callisto.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,35 +32,35 @@
 
             if not self.host:
                 self.host = config_data['host']
             if not self.email:
                 self.email = config_data['email']
             if not self.password:
                 try:
-                    self.password = keyring.get_password("engine", self.email)
-                except:
                     self.password = config_data['password']
+                except:
+                    self.password = keyring.get_password("engine", self.email)
             try:
-                self.headers['Cookie'] = keyring.get_password("engine-cookie", self.email)
-            except:
                 self.headers['Cookie'] = config_data['Cookie']
+            except:
+                self.headers['Cookie'] = keyring.get_password("engine-cookie", self.email)
         except:
             pass
 
     def update_config(self):
         config_path = os.path.join(user_config_dir('engine'), "config.json")
         fout = open(config_path, 'w')
         try:
             keyring.set_password("engine", self.email, self.password)
             keyring.set_password("engine-cookie", self.email, self.headers['Cookie'])
 
             json.dump({'host': self.host,
                         'email': self.email, 
-                        # 'password': self.password, 
-                        # 'cookie': self.headers['Cookie']
+                        'password': self.password, 
+                        'cookie': self.headers['Cookie']
                         }, fout)
         except:
             json.dump({'host': self.host,
                         'email': self.email, 
                         'password': self.password, 
                         'Cookie': self.headers['Cookie']
                         }, fout)
```

### Comparing `granular_engine-0.2.6/engine/connections/dione.py` & `granular_engine-0.2.7/engine/connections/dione.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.6/engine/connections/europa.py` & `granular_engine-0.2.7/engine/connections/europa.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,14 @@
     def get_project_exports(self, id):
         if self.org:
             project_exports_url = f'{self.callisto.host}/europa/api/v2/projects/{id}/datasets?orgId={self.org}'
         else:
             project_exports_url = f"{self.callisto.host}/europa/api/v2/projects/{id}/datasets?search=&status=all&isPublic=true"
 
         response = requests.get(project_exports_url, headers=self.callisto.headers)
-        
-        response = requests.get(project_exports_url, headers=self.callisto.headers)
 
         if response.status_code == 200:
             exports = response.json()['results']
             exports = {export["name"]: export for export in exports}
             
             return exports
         else:
@@ -125,17 +123,28 @@
     def get_project_export_by_id(self, project_id, export_id):
         if self.org:
             project_export_url = f'{self.callisto.host}/europa/api/v2/projects/{project_id}/datasets/{export_id}?orgId={self.org}'
         else:
             project_export_url = f"{self.callisto.host}/europa/api/v2/projects/{project_id}/datasets/{export_id}?search=&status=all&isPublic=true"
 
         response = requests.get(project_export_url, headers=self.callisto.headers)
-        
-        response = requests.get(project_export_url, headers=self.callisto.headers)
 
         if response.status_code == 200:
             export = response.json()
             return export
         else:
             print(f'Export {export_id} for GeoEngine project {project_id} cannot be retrieved')
             print(f'Exports endpoint {project_export_url} returned with HTTP status code : {response.status_code}\n')
+            return None
+        
+    def get_questions_of_project(self, project_id):
+        project_questions_url = f'{self.callisto.host}/europa/api/v2/questions?projectId={project_id}&pageSzie=1000'
+
+        response = requests.get(project_questions_url, headers=self.callisto.headers)
+
+        if response.status_code == 200:
+            export = response.json()
+            return export
+        else:
+            print(f'Questions for GeoEngine project {project_id} cannot be retrieved')
+            print(f'Questions endpoint {project_questions_url} returned with HTTP status code : {response.status_code}\n')
             return None
```

### Comparing `granular_engine-0.2.6/engine/connections/neso.py` & `granular_engine-0.2.7/engine/connections/neso.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.6/engine/grain.py` & `granular_engine-0.2.7/engine/grain.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.6/engine/libs/inquirer.py` & `granular_engine-0.2.7/engine/libs/inquirer.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,22 @@
 def filepath(message, **kwargs):
     return inquirer.filepath(
         message=message,
         qmark=kwargs.get("qmark", ""),
         amark=kwargs.get("amark", ""),
     ).execute()
 
+def dirpath(message, **kwargs):
+    return inquirer.filepath(
+        message=message,
+        qmark=kwargs.get("qmark", ""),
+        amark=kwargs.get("amark", ""),
+        only_directories=True,
+    ).execute()
+
 def text(message, **kwargs):
     return inquirer.text(
         message=message,
         qmark=kwargs.get("qmark", ""),
         amark=kwargs.get("amark", ""),
         ).execute()
```

### Comparing `granular_engine-0.2.6/pyproject.toml` & `granular_engine-0.2.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "granular-engine"
-version = "v0.2.6"
+version = "v0.2.7"
 description = "Experiment tracking for GeoSpatial Machine Learning on GeoEngine"
 authors = ["Sagar Verma <sagar@granular.ai>"]
 license = "MIT"
 readme = "README.rst"
 packages = [{include = "engine"}]
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Natural Language :: English',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
 ]
 repository='https://github.com/granularai/engine'
 
 
 [tool.poetry.scripts]
 engine = 'engine.cli:cli'
 
@@ -27,14 +28,16 @@
 tabulate = "^0.9.0"
 click = "^8.1.3"
 keyrings-alt = "^4.2.0"
 keyring = "^23.11.0"
 passlib = "^1.7.4"
 inquirerpy = "^0.3.4"
 colorama = "^0.4.6"
+yapf = "^0.33.0"
+addict = "^2.4.0"
 
 [tool.poetry.dev-dependencies]
 pip = "^21.1.3"
 beautifulsoup4 = "^4.10.0"
 bump2version = "^1.0.1"
 watchdog = "^2.1.3"
 flake8 = "^3.9.2"
```

### Comparing `granular_engine-0.2.6/PKG-INFO` & `granular_engine-0.2.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granular-engine
-Version: 0.2.6
+Version: 0.2.7
 Summary: Experiment tracking for GeoSpatial Machine Learning on GeoEngine
 Home-page: https://github.com/granularai/engine
 License: MIT
 Author: Sagar Verma
 Author-email: sagar@granular.ai
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: Intended Audience :: Developers
@@ -12,26 +12,29 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: addict (>=2.4.0,<3.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: keyring (>=23.11.0,<24.0.0)
 Requires-Dist: keyrings-alt (>=4.2.0,<5.0.0)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: yacs (>=0.1.8,<0.2.0)
+Requires-Dist: yapf (>=0.33.0,<0.34.0)
 Project-URL: Repository, https://github.com/granularai/engine
 Description-Content-Type: text/x-rst
 
 Engine
 ======
 
 A Utility Library that assists in Geospatial Machine Learning Experiment
```

