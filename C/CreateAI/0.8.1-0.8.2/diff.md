# Comparing `tmp/CreateAI-0.8.1.tar.gz` & `tmp/CreateAI-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CreateAI-0.8.1.tar", last modified: Sat May  6 04:23:14 2023, max compression
+gzip compressed data, was "CreateAI-0.8.2.tar", last modified: Mon May  8 12:25:55 2023, max compression
```

## Comparing `CreateAI-0.8.1.tar` & `CreateAI-0.8.2.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 04:23:14.216918 CreateAI-0.8.1/
-drwxrwxrwx   0        0        0        0 2023-05-06 04:23:14.198917 CreateAI-0.8.1/CreateAI/
--rw-rw-rw-   0        0        0     4394 2023-05-05 15:01:45.000000 CreateAI-0.8.1/CreateAI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 04:23:14.214914 CreateAI-0.8.1/CreateAI.egg-info/
--rw-rw-rw-   0        0        0     1816 2023-05-06 04:23:14.000000 CreateAI-0.8.1/CreateAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-05-06 04:23:14.000000 CreateAI-0.8.1/CreateAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 04:23:14.000000 CreateAI-0.8.1/CreateAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-06 04:23:14.000000 CreateAI-0.8.1/CreateAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1097 2023-05-05 14:50:25.000000 CreateAI-0.8.1/LICENCE
--rw-rw-rw-   0        0        0       18 2023-05-06 04:23:13.000000 CreateAI-0.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1816 2023-05-06 04:23:14.217916 CreateAI-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     1371 2023-05-05 16:57:35.000000 CreateAI-0.8.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 04:23:14.219918 CreateAI-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0      641 2023-05-06 04:23:13.000000 CreateAI-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:25:55.894458 CreateAI-0.8.2/
+drwxrwxrwx   0        0        0        0 2023-05-08 12:25:55.892467 CreateAI-0.8.2/CreateAI.egg-info/
+-rw-rw-rw-   0        0        0     2244 2023-05-08 12:25:55.000000 CreateAI-0.8.2/CreateAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-08 12:25:55.000000 CreateAI-0.8.2/CreateAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 12:25:55.000000 CreateAI-0.8.2/CreateAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-08 12:25:55.000000 CreateAI-0.8.2/CreateAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1097 2023-05-05 14:50:25.000000 CreateAI-0.8.2/LICENCE
+-rw-rw-rw-   0        0        0       48 2023-05-08 12:25:54.000000 CreateAI-0.8.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2244 2023-05-08 12:25:55.894458 CreateAI-0.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1799 2023-05-08 12:23:43.000000 CreateAI-0.8.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 12:25:55.896029 CreateAI-0.8.2/setup.cfg
+-rw-rw-rw-   0        0        0      671 2023-05-08 12:25:54.000000 CreateAI-0.8.2/setup.py
```

### Comparing `CreateAI-0.8.1/CreateAI.egg-info/PKG-INFO` & `CreateAI-0.8.2/CreateAI.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: CreateAI
-Version: 0.8.1
+Version: 0.8.2
 Summary: Easy tool for creating AI in python
 Home-page: https://github.com/R0fael/CreateAI
 Author: R0fael
 Author-email: roslobodchikov@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 
 # CreateAI
 It's easy tool to create ai in python easy and fast.
-You can edit code of CreateAI on my [github](https://github.com/R0fael/CreateAI)
+You can edit source code of CreateAI on [Create AI's github](https://github.com/R0fael/CreateAI)
 
 ## Dependencies
  - numpy
  - knowledge of python
  - our documentation
  - your motivation
  - your brain
 
 ## Authors
 
-- [@R0fael](https://www.github.com/R0fael) - programmer
+ - [@R0fael](https://www.github.com/R0fael) - programmer
 
 ## Features
- - Custom funktion activations
+ - Custom function activations - Errors
  - Neuron creating in one line of code
  - absolutly open sourse
 
 ## Installation
 
-Install my-project with pip
+Installing project with pip
 
 Windows:
 ```bash
 pip install СreateAI
 ```
 
 MacOS:
@@ -48,36 +48,59 @@
 ```
 
 Linux:
 ```bash
 sudo pip install СreateAI
 ```
 
+Or if you don't have pip :
+download sourse code and editing examples files
+
 ## Example
 ```python
 from CreateAI import *
 """
 inputs - create inputs
 outputs - create outputs
 """
-n = Neuron(weights(3, 1), inputs([[0, 0, 1], [1, 1, 1], [1, 0, 1], [0, 1, 1]]), outputs([[0, 1, 1, 0]])) # neuron creating
+# importing CreateAI
+from CreateAI import *
 
-n.learn(20_000) # learning
+n = Neuron(weights(3, 1), inputs([
+    [0, 0, 1],
+    [1, 1, 1],
+    [1, 0, 1],
+    [0, 1, 1]
+]), outputs([[0, 1, 1, 0]]))  # Neuron creating
+
+n.learn(20_000)  # Neuron learning
+
+print(n.process([1, 1, 0]))  # Neuron test
+print(n.process([0, 1, 0]))  # Neuron test
 
-print(n.process([1, 1, 0])) # test
-print(n.process([0, 1, 0])) # test
 ```
 
-## How to create custom funktion activation
+## How to create custom funktion activation - HAS ERRORS
 ```python
 from CreateAI import *
 
 def my_funk(x):
     return x # your code here
 
 n = Neuron(weights(3, 1), inputs([[0, 0, 1], [1, 1, 1], [1, 0, 1], [0, 1, 1]]), outputs([[0, 1, 1, 0]])) # neuron creating
 
 n.learn(20_000,aktivation=my_funk) # learning
 
 print(n.process([1, 1, 0])) # test
 print(n.process([0, 1, 0])) # test
 ```
+
+## Change log
+0.8 - First version
+0.8.1 - Little bug fix
+0.8.2 - Spead up
+
+## Plans
+0.8.3 - convertors
+0.9 - Saving system
+0.9.1 - Fixing custom functions activation
+1.0 / 0.10 - Multi neurons update
```

### Comparing `CreateAI-0.8.1/LICENCE` & `CreateAI-0.8.2/LICENCE`

 * *Files identical despite different names*

### Comparing `CreateAI-0.8.1/PKG-INFO` & `CreateAI-0.8.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: CreateAI
-Version: 0.8.1
+Version: 0.8.2
 Summary: Easy tool for creating AI in python
 Home-page: https://github.com/R0fael/CreateAI
 Author: R0fael
 Author-email: roslobodchikov@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 
 # CreateAI
 It's easy tool to create ai in python easy and fast.
-You can edit code of CreateAI on my [github](https://github.com/R0fael/CreateAI)
+You can edit source code of CreateAI on [Create AI's github](https://github.com/R0fael/CreateAI)
 
 ## Dependencies
  - numpy
  - knowledge of python
  - our documentation
  - your motivation
  - your brain
 
 ## Authors
 
-- [@R0fael](https://www.github.com/R0fael) - programmer
+ - [@R0fael](https://www.github.com/R0fael) - programmer
 
 ## Features
- - Custom funktion activations
+ - Custom function activations - Errors
  - Neuron creating in one line of code
  - absolutly open sourse
 
 ## Installation
 
-Install my-project with pip
+Installing project with pip
 
 Windows:
 ```bash
 pip install СreateAI
 ```
 
 MacOS:
@@ -48,36 +48,59 @@
 ```
 
 Linux:
 ```bash
 sudo pip install СreateAI
 ```
 
+Or if you don't have pip :
+download sourse code and editing examples files
+
 ## Example
 ```python
 from CreateAI import *
 """
 inputs - create inputs
 outputs - create outputs
 """
-n = Neuron(weights(3, 1), inputs([[0, 0, 1], [1, 1, 1], [1, 0, 1], [0, 1, 1]]), outputs([[0, 1, 1, 0]])) # neuron creating
+# importing CreateAI
+from CreateAI import *
 
-n.learn(20_000) # learning
+n = Neuron(weights(3, 1), inputs([
+    [0, 0, 1],
+    [1, 1, 1],
+    [1, 0, 1],
+    [0, 1, 1]
+]), outputs([[0, 1, 1, 0]]))  # Neuron creating
+
+n.learn(20_000)  # Neuron learning
+
+print(n.process([1, 1, 0]))  # Neuron test
+print(n.process([0, 1, 0]))  # Neuron test
 
-print(n.process([1, 1, 0])) # test
-print(n.process([0, 1, 0])) # test
 ```
 
-## How to create custom funktion activation
+## How to create custom funktion activation - HAS ERRORS
 ```python
 from CreateAI import *
 
 def my_funk(x):
     return x # your code here
 
 n = Neuron(weights(3, 1), inputs([[0, 0, 1], [1, 1, 1], [1, 0, 1], [0, 1, 1]]), outputs([[0, 1, 1, 0]])) # neuron creating
 
 n.learn(20_000,aktivation=my_funk) # learning
 
 print(n.process([1, 1, 0])) # test
 print(n.process([0, 1, 0])) # test
 ```
+
+## Change log
+0.8 - First version
+0.8.1 - Little bug fix
+0.8.2 - Spead up
+
+## Plans
+0.8.3 - convertors
+0.9 - Saving system
+0.9.1 - Fixing custom functions activation
+1.0 / 0.10 - Multi neurons update
```

### Comparing `CreateAI-0.8.1/README.md` & `CreateAI-0.8.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 
 # CreateAI
 It's easy tool to create ai in python easy and fast.
-You can edit code of CreateAI on my [github](https://github.com/R0fael/CreateAI)
+You can edit source code of CreateAI on [Create AI's github](https://github.com/R0fael/CreateAI)
 
 ## Dependencies
  - numpy
  - knowledge of python
  - our documentation
  - your motivation
  - your brain
 
 ## Authors
 
-- [@R0fael](https://www.github.com/R0fael) - programmer
+ - [@R0fael](https://www.github.com/R0fael) - programmer
 
 ## Features
- - Custom funktion activations
+ - Custom function activations - Errors
  - Neuron creating in one line of code
  - absolutly open sourse
 
 ## Installation
 
-Install my-project with pip
+Installing project with pip
 
 Windows:
 ```bash
 pip install СreateAI
 ```
 
 MacOS:
@@ -34,36 +34,59 @@
 ```
 
 Linux:
 ```bash
 sudo pip install СreateAI
 ```
 
+Or if you don't have pip :
+download sourse code and editing examples files
+
 ## Example
 ```python
 from CreateAI import *
 """
 inputs - create inputs
 outputs - create outputs
 """
-n = Neuron(weights(3, 1), inputs([[0, 0, 1], [1, 1, 1], [1, 0, 1], [0, 1, 1]]), outputs([[0, 1, 1, 0]])) # neuron creating
+# importing CreateAI
+from CreateAI import *
 
-n.learn(20_000) # learning
+n = Neuron(weights(3, 1), inputs([
+    [0, 0, 1],
+    [1, 1, 1],
+    [1, 0, 1],
+    [0, 1, 1]
+]), outputs([[0, 1, 1, 0]]))  # Neuron creating
+
+n.learn(20_000)  # Neuron learning
+
+print(n.process([1, 1, 0]))  # Neuron test
+print(n.process([0, 1, 0]))  # Neuron test
 
-print(n.process([1, 1, 0])) # test
-print(n.process([0, 1, 0])) # test
 ```
 
-## How to create custom funktion activation
+## How to create custom funktion activation - HAS ERRORS
 ```python
 from CreateAI import *
 
 def my_funk(x):
     return x # your code here
 
 n = Neuron(weights(3, 1), inputs([[0, 0, 1], [1, 1, 1], [1, 0, 1], [0, 1, 1]]), outputs([[0, 1, 1, 0]])) # neuron creating
 
 n.learn(20_000,aktivation=my_funk) # learning
 
 print(n.process([1, 1, 0])) # test
 print(n.process([0, 1, 0])) # test
-```
+```
+
+## Change log
+0.8 - First version
+0.8.1 - Little bug fix
+0.8.2 - Spead up
+
+## Plans
+0.8.3 - convertors
+0.9 - Saving system
+0.9.1 - Fixing custom functions activation
+1.0 / 0.10 - Multi neurons update
```

### Comparing `CreateAI-0.8.1/setup.py` & `CreateAI-0.8.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 with open(r'C:\MyUse\code\python\EasyPack\README.md', 'r', encoding='utf-8') as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='CreateAI',
-	version='0.8.1',
+	version='0.8.2',
 	author='R0fael',
 	author_email='roslobodchikov@gmail.com',
 	description='Easy tool for creating AI in python',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://github.com/R0fael/CreateAI',
-	packages=['CreateAI'],
+	packages=['C:\MyUse\code\python\EasyPack\CreateAI'],
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"License :: OSI Approved :: MIT License",
 		"Operating System :: OS Independent",
 	],
 	python_requires='>=3.6',
 )
```

