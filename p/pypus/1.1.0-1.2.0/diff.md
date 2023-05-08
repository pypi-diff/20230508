# Comparing `tmp/pypus-1.1.0.tar.gz` & `tmp/pypus-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypus-1.1.0.tar", max compression
+gzip compressed data, was "pypus-1.2.0.tar", max compression
```

## Comparing `pypus-1.1.0.tar` & `pypus-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2021-05-28 19:35:21.744187 pypus-1.1.0/LICENSE
--rw-r--r--   0        0        0      114 2021-05-28 19:36:19.806135 pypus-1.1.0/README.md
--rw-r--r--   0        0        0      511 2021-12-08 23:09:13.600820 pypus-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-05-11 19:37:09.641525 pypus-1.1.0/src/pypus/__init__.py
--rw-r--r--   0        0        0    21615 2021-12-08 23:06:25.046275 pypus-1.1.0/src/pypus/cli.py
--rw-r--r--   0        0        0      947 2021-12-08 23:09:21.807575 pypus-1.1.0/setup.py
--rw-r--r--   0        0        0      716 2021-12-08 23:09:21.807888 pypus-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2021-05-28 19:35:21.744187 pypus-1.2.0/LICENSE
+-rw-r--r--   0        0        0      114 2021-05-28 19:36:19.806135 pypus-1.2.0/README.md
+-rw-r--r--   0        0        0      511 2023-05-08 16:57:22.101016 pypus-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-05-11 19:37:09.641525 pypus-1.2.0/src/pypus/__init__.py
+-rw-r--r--   0        0        0    23328 2023-05-08 16:55:48.132893 pypus-1.2.0/src/pypus/cli.py
+-rw-r--r--   0        0        0      953 1970-01-01 00:00:00.000000 pypus-1.2.0/setup.py
+-rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 pypus-1.2.0/PKG-INFO
```

### Comparing `pypus-1.1.0/LICENSE` & `pypus-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypus-1.1.0/src/pypus/cli.py` & `pypus-1.2.0/src/pypus/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,53 @@
     """ Prints out the current necessary environment variables """
     octopus_api_key = os.getenv('OCTOPUS_API_KEY')
     octopus_server_uri = os.getenv('OCTOPUS_SERVER_URI')
     print(f"Your environment has {octopus_api_key} for the variable OCTOPUS_API_KEY")
     print(f"Your environment has {octopus_server_uri} for the variable OCTOPUS_SERVER_URI")
 
 
+@main.command('get-machines', short_help='Get a list of all machines for a space')
+@click.argument("space")
+def get_projects(space):
+    """ Get a list of all machines for the defined space
+
+    Arguments:
+        space: The name of the Octopus Deploy Space
+
+    """
+    octopus_api_key = os.getenv('OCTOPUS_API_KEY')
+    octopus_server_uri = os.getenv('OCTOPUS_SERVER_URI')
+    headers = {'X-Octopus-ApiKey': octopus_api_key}
+    def get_octopus_resource(uri):
+        """ Gets a resource from the API
+
+        Arguments:
+            uri: The base url of the Octopus Deploy API
+        """
+        response = requests.get(uri, headers=headers, verify=False)
+        response.raise_for_status()
+        return json.loads(response.content.decode('utf-8'))
+
+    def get_by_name(uri, name):
+        """ Gets a resource from the API by name
+
+        Arguments:
+            uri: The base url of the Octopus Deploy API
+            name: The name of the resource
+        """
+        resources = get_octopus_resource(uri)
+        return next((x for x in resources if x['Name'] == name), None)
+    space_name = space
+    space = get_by_name('{0}/spaces/all'.format(octopus_server_uri), space_name)
+    machines = get_octopus_resource('{0}/{1}/machines/all'.format(octopus_server_uri, space['Id']))
+    print(f"The space {space_name} has these machines in it")
+    for i in machines:
+        print(f"Machine {i['Name']} has an ID of {i['Id']} and is assigned to these {i['Roles']} roles.")
+    return machines
+
 @main.command('get-spaces', short_help='Get a list of spaces for server')
 def get_spaces():
     octopus_api_key = os.getenv('OCTOPUS_API_KEY')
     octopus_server_uri = os.getenv('OCTOPUS_SERVER_URI')
     headers = {'X-Octopus-ApiKey': octopus_api_key}
     def get_octopus_resource(uri, headers, skip_count = 0):
         """ Gets a resource from the API
@@ -128,20 +167,24 @@
 @main.command('set-var', short_help='Set a variable for a project in a space')
 @click.argument("space")
 @click.argument("project")
 @click.argument("variable-name")
 @click.argument("variable-value")
 @click.option('--sensitive', is_flag=True)
 def set_var(space, project, variable_name, variable_value, sensitive):
-    """ Get a list of vars for a project within a space
+    """ Set a variable for a project in a space
 
     Arguments:
         space: The space where the project resides
-        project: The project from which to get variables
+        project: The project where the variable is created
+        variable-name: The name of the variable
+        variable-value: The value to set for the variable
+        sensitive: Set this flag for passwords
 
+        note: Only string variable types are currently supported
     """
     def get_octopus_resource(uri, headers, skip_count = 0):
         """ Gets a resource from the API
 
         Arguments:
             uri: The base url of the Octopus Deploy API
         """
```

### Comparing `pypus-1.1.0/setup.py` & `pypus-1.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 ['click>=8.0.0,<9.0.0', 'requests>=2.25.1,<3.0.0', 'termcolor>=1.1.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['pypus = pypus.cli:main']}
 
 setup_kwargs = {
     'name': 'pypus',
-    'version': '1.1.0',
+    'version': '1.2.0',
     'description': 'Octopus cli toolkit',
     'long_description': '# Pypus\n\nPypus is a cli tool for publishing Octopus Deploy Runbooks.\n\n## Install\n\n```bash\n$ pip install pypus\n```\n',
     'author': 'Michael MacKenna',
     'author_email': 'mmackenna@unitedfiregroup.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `pypus-1.1.0/PKG-INFO` & `pypus-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pypus
-Version: 1.1.0
+Version: 1.2.0
 Summary: Octopus cli toolkit
 License: MIT
 Author: Michael MacKenna
 Author-email: mmackenna@unitedfiregroup.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Pypus
```

