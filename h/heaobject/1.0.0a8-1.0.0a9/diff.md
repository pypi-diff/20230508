# Comparing `tmp/heaobject-1.0.0a8.tar.gz` & `tmp/heaobject-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/heaobject-1.0.0a8.tar", last modified: Wed Jul 14 02:24:12 2021, max compression
+gzip compressed data, was "dist\heaobject-1.0.0a9.tar", last modified: Thu Jul 15 16:42:08 2021, max compression
```

## Comparing `heaobject-1.0.0a8.tar` & `heaobject-1.0.0a9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2021-07-14 02:24:12.154208 heaobject-1.0.0a8/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     5348 2021-07-14 02:24:12.154208 heaobject-1.0.0a8/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     3682 2021-07-09 23:01:59.000000 heaobject-1.0.0a8/README.md
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2021-07-14 02:24:12.154208 heaobject-1.0.0a8/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2196 2021-07-14 02:22:40.000000 heaobject-1.0.0a8/setup.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2021-07-14 02:24:12.150208 heaobject-1.0.0a8/src/
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2021-07-14 02:24:12.150208 heaobject-1.0.0a8/src/heaobject/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       77 2020-07-26 03:22:22.000000 heaobject-1.0.0a8/src/heaobject/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1249 2021-07-09 23:02:14.000000 heaobject-1.0.0a8/src/heaobject/dataadapter.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      261 2021-07-09 23:02:14.000000 heaobject-1.0.0a8/src/heaobject/dataelement.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1525 2021-07-11 00:32:55.000000 heaobject-1.0.0a8/src/heaobject/datamodel.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      405 2021-07-09 23:02:14.000000 heaobject-1.0.0a8/src/heaobject/datapattern.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      124 2021-07-09 23:02:14.000000 heaobject-1.0.0a8/src/heaobject/dataset.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      232 2020-07-26 03:22:22.000000 heaobject-1.0.0a8/src/heaobject/error.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2279 2021-07-12 03:27:23.000000 heaobject-1.0.0a8/src/heaobject/folder.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1510 2021-07-12 03:27:41.000000 heaobject-1.0.0a8/src/heaobject/keychain.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        0 2020-07-26 20:54:18.000000 heaobject-1.0.0a8/src/heaobject/py.typed
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      123 2021-07-09 23:02:14.000000 heaobject-1.0.0a8/src/heaobject/record.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     4832 2021-07-12 03:45:17.000000 heaobject-1.0.0a8/src/heaobject/registry.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    34773 2021-07-14 02:13:38.000000 heaobject-1.0.0a8/src/heaobject/root.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      128 2021-07-11 00:32:55.000000 heaobject-1.0.0a8/src/heaobject/source.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1117 2021-07-11 00:32:55.000000 heaobject-1.0.0a8/src/heaobject/source2target.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      364 2020-07-26 03:22:22.000000 heaobject-1.0.0a8/src/heaobject/user.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2101 2021-07-12 07:41:48.000000 heaobject-1.0.0a8/src/heaobject/volume.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2021-07-14 02:24:12.154208 heaobject-1.0.0a8/src/heaobject.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     5348 2021-07-14 02:24:12.000000 heaobject-1.0.0a8/src/heaobject.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      636 2021-07-14 02:24:12.000000 heaobject-1.0.0a8/src/heaobject.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2021-07-14 02:24:12.000000 heaobject-1.0.0a8/src/heaobject.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       35 2021-07-14 02:24:12.000000 heaobject-1.0.0a8/src/heaobject.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       10 2021-07-14 02:24:12.000000 heaobject-1.0.0a8/src/heaobject.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-07-15 16:42:08.282851 heaobject-1.0.0a9/
+-rw-rw-rw-   0        0        0     5435 2021-07-15 16:42:08.282851 heaobject-1.0.0a9/PKG-INFO
+-rw-rw-rw-   0        0        0     3742 2021-07-02 22:53:26.000000 heaobject-1.0.0a9/README.md
+-rw-rw-rw-   0        0        0       42 2021-07-15 16:42:08.290963 heaobject-1.0.0a9/setup.cfg
+-rw-rw-rw-   0        0        0     2196 2021-07-15 16:41:20.000000 heaobject-1.0.0a9/setup.py
+drwxrwxrwx   0        0        0        0 2021-07-15 16:42:08.171395 heaobject-1.0.0a9/src/
+drwxrwxrwx   0        0        0        0 2021-07-15 16:42:08.252481 heaobject-1.0.0a9/src/heaobject/
+-rw-rw-rw-   0        0        0       79 2020-02-24 16:30:26.000000 heaobject-1.0.0a9/src/heaobject/__init__.py
+-rw-rw-rw-   0        0        0     2434 2021-07-15 14:52:24.000000 heaobject-1.0.0a9/src/heaobject/data.py
+-rw-rw-rw-   0        0        0     1331 2021-07-14 15:32:49.000000 heaobject-1.0.0a9/src/heaobject/dataadapter.py
+-rw-rw-rw-   0        0        0      272 2021-07-10 19:10:58.000000 heaobject-1.0.0a9/src/heaobject/dataelement.py
+-rw-rw-rw-   0        0        0     1601 2021-07-10 19:14:10.000000 heaobject-1.0.0a9/src/heaobject/datamodel.py
+-rw-rw-rw-   0        0        0      430 2021-07-10 19:10:58.000000 heaobject-1.0.0a9/src/heaobject/datapattern.py
+-rw-rw-rw-   0        0        0      122 2021-07-14 15:37:50.000000 heaobject-1.0.0a9/src/heaobject/datatransform.py
+-rw-rw-rw-   0        0        0      241 2020-02-24 16:30:26.000000 heaobject-1.0.0a9/src/heaobject/error.py
+-rw-rw-rw-   0        0        0     3045 2021-07-15 16:29:24.000000 heaobject-1.0.0a9/src/heaobject/folder.py
+-rw-rw-rw-   0        0        0     1552 2021-07-14 16:13:58.000000 heaobject-1.0.0a9/src/heaobject/keychain.py
+-rw-rw-rw-   0        0        0        0 2020-06-20 07:12:58.000000 heaobject-1.0.0a9/src/heaobject/py.typed
+-rw-rw-rw-   0        0        0      130 2021-07-10 19:10:58.000000 heaobject-1.0.0a9/src/heaobject/record.py
+-rw-rw-rw-   0        0        0     4963 2021-07-14 16:13:58.000000 heaobject-1.0.0a9/src/heaobject/registry.py
+-rw-rw-rw-   0        0        0    37756 2021-07-15 16:36:38.000000 heaobject-1.0.0a9/src/heaobject/root.py
+-rw-rw-rw-   0        0        0      135 2021-07-10 19:14:10.000000 heaobject-1.0.0a9/src/heaobject/source.py
+-rw-rw-rw-   0        0        0     1149 2021-07-10 19:14:10.000000 heaobject-1.0.0a9/src/heaobject/source2target.py
+-rw-rw-rw-   0        0        0      375 2020-02-24 16:30:26.000000 heaobject-1.0.0a9/src/heaobject/user.py
+-rw-rw-rw-   0        0        0     2155 2021-07-14 16:13:35.000000 heaobject-1.0.0a9/src/heaobject/volume.py
+drwxrwxrwx   0        0        0        0 2021-07-15 16:42:08.282851 heaobject-1.0.0a9/src/heaobject.egg-info/
+-rw-rw-rw-   0        0        0     5435 2021-07-15 16:42:07.000000 heaobject-1.0.0a9/src/heaobject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      664 2021-07-15 16:42:08.000000 heaobject-1.0.0a9/src/heaobject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-07-15 16:42:07.000000 heaobject-1.0.0a9/src/heaobject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2021-07-15 16:42:07.000000 heaobject-1.0.0a9/src/heaobject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2021-07-15 16:42:07.000000 heaobject-1.0.0a9/src/heaobject.egg-info/top_level.txt
```

### Comparing `heaobject-1.0.0a8/PKG-INFO` & `heaobject-1.0.0a9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-Metadata-Version: 2.1
-Name: heaobject
-Version: 1.0.0a8
-Summary: Data and other classes that are passed into and out of HEA REST APIs.
-Home-page: https://risr.hci.utah.edu
-Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
-Author-email: Andrew.Post@hci.utah.edu
-License: UNKNOWN
-Description: # HEA Object Library
-        [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
-        
-        The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
-        
-        ## Version 1
-        Initial release.
-        
-        ## Runtime requirements
-        * Python 3.8
-        
-        ## Development environment
-        
-        ### Build requirements
-        * Any development environment is fine.
-        * On Windows, you also will need:
-            * Build Tools for Visual Studio 2019, found at https://visualstudio.microsoft.com/downloads/. Select the C++ tools.
-            * git, found at https://git-scm.com/download/win.
-        * On Mac, Xcode or the command line developer tools is required, found in the Apple Store app.
-        * Python 3.8: Download and install Python 3.8 from https://www.python.org, and select the options to install for all users and add
-        Python to your environment variables. The install for all users option will help keep you from accidentally installing
-        packages into your Python installation's site-packages directory instead of to your virtualenv environment, described
-        below.
-        * Create a virtualenv environment using the `python -m venv <venv_directory>` command, substituting `<venv_directory>`
-        with the directory name of your virtual environment. Run `source <venv_directory>/bin/activate` (or `<venv_directory>/Scripts/activate` on Windows) to activate the virtual
-        environment. You will need to activate the virtualenv every time before starting work, or your IDE may be able to do 
-        this for you automatically. **Note that PyCharm will do this for you, but you have to create a new Terminal panel
-        after you newly configure a project with your virtualenv.**
-        * From the project's root directory, and using the activated virtualenv, run `pip install -r requirements_dev.txt`.
-        **Do NOT run `python setup.py develop`. It will break your environment.**
-        
-        ### Running unit tests
-        Run tests with the `pytest` command from the project root directory.
-        
-        ### Versioning
-        Use semantic versioning as described in 
-        https://packaging.python.org/guides/distributing-packages-using-setuptools/#choosing-a-versioning-scheme. In addition,
-        while development is underway, the version should be the next version number suffixed by -SNAPSHOT.
-        
-        ### Version tags in git
-        Version tags should follow the format `heaobject-<version>`, for example, `heaobject-1.0.0`.
-        
-        ### Uploading to an index server
-        You will need a custom index server such as devpi to upload HEA component releases so that HEA
-        components can depend on each other. You will need to configure pip to use the custom index server
-        instead of the usual Pypi.
-        
-        The following instructions assume separate stable and staging indexes. Numbered releases, including alphas and betas, go 
-        into the stable index. Snapshots of works in progress go into the staging index. Artifacts uploaded to the
-        staging index can be overwritten. Artifacts uploaded to stable cannot. Thus, also use staging to upload numbered
-        releases, verify the uploaded packages, and then upload to stable.
-        
-        From the project's root directory:
-        1. For numbered releases, remove `.dev` from the version number in setup.py, tag it in git to indicate a release, 
-        and commit to version control. Skip this step for SNAPSHOT releases.
-        2. Run `python setup.py clean --all sdist bdist_wheel` to create the artifacts.
-        3. Run `twine upload -r <repository> dist/*` to upload to the repository. The repository name has to be defined in a
-        twine configuration file such as `$HOME/.pypirc`.
-        4. For numbered releases, increment the version number in setup.py, append `.dev` to it, and commit to version 
-        control. Skip this step for SNAPSHOT releases.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: heaobject
+Version: 1.0.0a9
+Summary: Data and other classes that are passed into and out of HEA REST APIs.
+Home-page: https://risr.hci.utah.edu
+Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
+Author-email: Andrew.Post@hci.utah.edu
+License: UNKNOWN
+Description: # HEA Object Library
+        [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
+        
+        The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
+        
+        ## Version 1
+        Initial release.
+        
+        ## Runtime requirements
+        * Python 3.8
+        
+        ## Development environment
+        
+        ### Build requirements
+        * Any development environment is fine.
+        * On Windows, you also will need:
+            * Build Tools for Visual Studio 2019, found at https://visualstudio.microsoft.com/downloads/. Select the C++ tools.
+            * git, found at https://git-scm.com/download/win.
+        * On Mac, Xcode or the command line developer tools is required, found in the Apple Store app.
+        * Python 3.8: Download and install Python 3.8 from https://www.python.org, and select the options to install for all users and add
+        Python to your environment variables. The install for all users option will help keep you from accidentally installing
+        packages into your Python installation's site-packages directory instead of to your virtualenv environment, described
+        below.
+        * Create a virtualenv environment using the `python -m venv <venv_directory>` command, substituting `<venv_directory>`
+        with the directory name of your virtual environment. Run `source <venv_directory>/bin/activate` (or `<venv_directory>/Scripts/activate` on Windows) to activate the virtual
+        environment. You will need to activate the virtualenv every time before starting work, or your IDE may be able to do 
+        this for you automatically. **Note that PyCharm will do this for you, but you have to create a new Terminal panel
+        after you newly configure a project with your virtualenv.**
+        * From the project's root directory, and using the activated virtualenv, run `pip install -r requirements_dev.txt`.
+        **Do NOT run `python setup.py develop`. It will break your environment.**
+        
+        ### Running unit tests
+        Run tests with the `pytest` command from the project root directory.
+        
+        ### Versioning
+        Use semantic versioning as described in 
+        https://packaging.python.org/guides/distributing-packages-using-setuptools/#choosing-a-versioning-scheme. In addition,
+        while development is underway, the version should be the next version number suffixed by -SNAPSHOT.
+        
+        ### Version tags in git
+        Version tags should follow the format `heaobject-<version>`, for example, `heaobject-1.0.0`.
+        
+        ### Uploading to an index server
+        You will need a custom index server such as devpi to upload HEA component releases so that HEA
+        components can depend on each other. You will need to configure pip to use the custom index server
+        instead of the usual Pypi.
+        
+        The following instructions assume separate stable and staging indexes. Numbered releases, including alphas and betas, go 
+        into the stable index. Snapshots of works in progress go into the staging index. Artifacts uploaded to the
+        staging index can be overwritten. Artifacts uploaded to stable cannot. Thus, also use staging to upload numbered
+        releases, verify the uploaded packages, and then upload to stable.
+        
+        From the project's root directory:
+        1. For numbered releases, remove `.dev` from the version number in setup.py, tag it in git to indicate a release, 
+        and commit to version control. Skip this step for SNAPSHOT releases.
+        2. Run `python setup.py clean --all sdist bdist_wheel` to create the artifacts.
+        3. Run `twine upload -r <repository> dist/*` to upload to the repository. The repository name has to be defined in a
+        twine configuration file such as `$HOME/.pypirc`.
+        4. For numbered releases, increment the version number in setup.py, append `.dev` to it, and commit to version 
+        control. Skip this step for SNAPSHOT releases.
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
```

### Comparing `heaobject-1.0.0a8/README.md` & `heaobject-1.0.0a9/README.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# HEA Object Library
-[Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
-
-The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
-
-## Version 1
-Initial release.
-
-## Runtime requirements
-* Python 3.8
-
-## Development environment
-
-### Build requirements
-* Any development environment is fine.
-* On Windows, you also will need:
-    * Build Tools for Visual Studio 2019, found at https://visualstudio.microsoft.com/downloads/. Select the C++ tools.
-    * git, found at https://git-scm.com/download/win.
-* On Mac, Xcode or the command line developer tools is required, found in the Apple Store app.
-* Python 3.8: Download and install Python 3.8 from https://www.python.org, and select the options to install for all users and add
-Python to your environment variables. The install for all users option will help keep you from accidentally installing
-packages into your Python installation's site-packages directory instead of to your virtualenv environment, described
-below.
-* Create a virtualenv environment using the `python -m venv <venv_directory>` command, substituting `<venv_directory>`
-with the directory name of your virtual environment. Run `source <venv_directory>/bin/activate` (or `<venv_directory>/Scripts/activate` on Windows) to activate the virtual
-environment. You will need to activate the virtualenv every time before starting work, or your IDE may be able to do 
-this for you automatically. **Note that PyCharm will do this for you, but you have to create a new Terminal panel
-after you newly configure a project with your virtualenv.**
-* From the project's root directory, and using the activated virtualenv, run `pip install -r requirements_dev.txt`.
-**Do NOT run `python setup.py develop`. It will break your environment.**
-
-### Running unit tests
-Run tests with the `pytest` command from the project root directory.
-
-### Versioning
-Use semantic versioning as described in 
-https://packaging.python.org/guides/distributing-packages-using-setuptools/#choosing-a-versioning-scheme. In addition,
-while development is underway, the version should be the next version number suffixed by -SNAPSHOT.
-
-### Version tags in git
-Version tags should follow the format `heaobject-<version>`, for example, `heaobject-1.0.0`.
-
-### Uploading to an index server
-You will need a custom index server such as devpi to upload HEA component releases so that HEA
-components can depend on each other. You will need to configure pip to use the custom index server
-instead of the usual Pypi.
-
-The following instructions assume separate stable and staging indexes. Numbered releases, including alphas and betas, go 
-into the stable index. Snapshots of works in progress go into the staging index. Artifacts uploaded to the
-staging index can be overwritten. Artifacts uploaded to stable cannot. Thus, also use staging to upload numbered
-releases, verify the uploaded packages, and then upload to stable.
-
-From the project's root directory:
-1. For numbered releases, remove `.dev` from the version number in setup.py, tag it in git to indicate a release, 
-and commit to version control. Skip this step for SNAPSHOT releases.
-2. Run `python setup.py clean --all sdist bdist_wheel` to create the artifacts.
-3. Run `twine upload -r <repository> dist/*` to upload to the repository. The repository name has to be defined in a
-twine configuration file such as `$HOME/.pypirc`.
-4. For numbered releases, increment the version number in setup.py, append `.dev` to it, and commit to version 
-control. Skip this step for SNAPSHOT releases.
+# HEA Object Library
+[Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
+
+The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
+
+## Version 1
+Initial release.
+
+## Runtime requirements
+* Python 3.8
+
+## Development environment
+
+### Build requirements
+* Any development environment is fine.
+* On Windows, you also will need:
+    * Build Tools for Visual Studio 2019, found at https://visualstudio.microsoft.com/downloads/. Select the C++ tools.
+    * git, found at https://git-scm.com/download/win.
+* On Mac, Xcode or the command line developer tools is required, found in the Apple Store app.
+* Python 3.8: Download and install Python 3.8 from https://www.python.org, and select the options to install for all users and add
+Python to your environment variables. The install for all users option will help keep you from accidentally installing
+packages into your Python installation's site-packages directory instead of to your virtualenv environment, described
+below.
+* Create a virtualenv environment using the `python -m venv <venv_directory>` command, substituting `<venv_directory>`
+with the directory name of your virtual environment. Run `source <venv_directory>/bin/activate` (or `<venv_directory>/Scripts/activate` on Windows) to activate the virtual
+environment. You will need to activate the virtualenv every time before starting work, or your IDE may be able to do 
+this for you automatically. **Note that PyCharm will do this for you, but you have to create a new Terminal panel
+after you newly configure a project with your virtualenv.**
+* From the project's root directory, and using the activated virtualenv, run `pip install -r requirements_dev.txt`.
+**Do NOT run `python setup.py develop`. It will break your environment.**
+
+### Running unit tests
+Run tests with the `pytest` command from the project root directory.
+
+### Versioning
+Use semantic versioning as described in 
+https://packaging.python.org/guides/distributing-packages-using-setuptools/#choosing-a-versioning-scheme. In addition,
+while development is underway, the version should be the next version number suffixed by -SNAPSHOT.
+
+### Version tags in git
+Version tags should follow the format `heaobject-<version>`, for example, `heaobject-1.0.0`.
+
+### Uploading to an index server
+You will need a custom index server such as devpi to upload HEA component releases so that HEA
+components can depend on each other. You will need to configure pip to use the custom index server
+instead of the usual Pypi.
+
+The following instructions assume separate stable and staging indexes. Numbered releases, including alphas and betas, go 
+into the stable index. Snapshots of works in progress go into the staging index. Artifacts uploaded to the
+staging index can be overwritten. Artifacts uploaded to stable cannot. Thus, also use staging to upload numbered
+releases, verify the uploaded packages, and then upload to stable.
+
+From the project's root directory:
+1. For numbered releases, remove `.dev` from the version number in setup.py, tag it in git to indicate a release, 
+and commit to version control. Skip this step for SNAPSHOT releases.
+2. Run `python setup.py clean --all sdist bdist_wheel` to create the artifacts.
+3. Run `twine upload -r <repository> dist/*` to upload to the repository. The repository name has to be defined in a
+twine configuration file such as `$HOME/.pypirc`.
+4. For numbered releases, increment the version number in setup.py, append `.dev` to it, and commit to version 
+control. Skip this step for SNAPSHOT releases.
```

### Comparing `heaobject-1.0.0a8/setup.py` & `heaobject-1.0.0a9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaobject',
-                 version='1.0.0a8',
+                 version='1.0.0a9',
                  description='Data and other classes that are passed into and out of HEA REST APIs.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.8',
```

### Comparing `heaobject-1.0.0a8/src/heaobject/datamodel.py` & `heaobject-1.0.0a9/src/heaobject/datamodel.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-from heaobject import root
-
-
-class DataModel(root.AbstractDesktopObject):
-    def __init__(self):
-        super().__init__()
-
-
-class RelationalDataModel(DataModel):
-    def __init__(self):
-        super().__init__()
-        self.entities = []
-
-
-class FlatDataModel(DataModel):
-    def __init__(self):
-        super().__init__()
-        self.row = None
-        self.columns = []
-
-
-class DelimitedDataModel(FlatDataModel):
-    def __init__(self):
-        super().__init__()
-
-
-class FixedWidthDataModel(FlatDataModel):
-    def __init__(self):
-        super().__init__()
-
-
-class Row(root.AbstractMemberObject):
-    def __init__(self):
-        super().__init__()
-
-
-class Column(root.AbstractMemberObject):
-    def __init__(self):
-        super().__init__()
-        self.data_element_uri = None
-
-
-class DynamicWidthColumn(Column):
-    def __init__(self):
-        super().__init__()
-        self.start = 0
-        self.max_width = 0
-
-
-class FixedWidthColumn(Column):
-    def __init__(self):
-        super().__init__()
-        self.start = 0
-        self.width = 0
-
-
-class Entity(root.AbstractMemberObject):
-    def __init__(self):
-        super().__init__()
-        self.attributes = []
-        self.associations = []
-
-
-class Attribute(root.AbstractMemberObject):
-    def __init__(self):
-        super().__init__()
-        self.data_element_uri = None
-
-
-class Association(root.AbstractMemberObject):
-    def __init__(self):
-        super().__init__()
-        self.lhs = None  # An entity
-        self.rhs = None  # Another entity
-
-
+from heaobject import root
+
+
+class DataModel(root.AbstractDesktopObject):
+    def __init__(self):
+        super().__init__()
+
+
+class RelationalDataModel(DataModel):
+    def __init__(self):
+        super().__init__()
+        self.entities = []
+
+
+class FlatDataModel(DataModel):
+    def __init__(self):
+        super().__init__()
+        self.row = None
+        self.columns = []
+
+
+class DelimitedDataModel(FlatDataModel):
+    def __init__(self):
+        super().__init__()
+
+
+class FixedWidthDataModel(FlatDataModel):
+    def __init__(self):
+        super().__init__()
+
+
+class Row(root.AbstractMemberObject):
+    def __init__(self):
+        super().__init__()
+
+
+class Column(root.AbstractMemberObject):
+    def __init__(self):
+        super().__init__()
+        self.data_element_uri = None
+
+
+class DynamicWidthColumn(Column):
+    def __init__(self):
+        super().__init__()
+        self.start = 0
+        self.max_width = 0
+
+
+class FixedWidthColumn(Column):
+    def __init__(self):
+        super().__init__()
+        self.start = 0
+        self.width = 0
+
+
+class Entity(root.AbstractMemberObject):
+    def __init__(self):
+        super().__init__()
+        self.attributes = []
+        self.associations = []
+
+
+class Attribute(root.AbstractMemberObject):
+    def __init__(self):
+        super().__init__()
+        self.data_element_uri = None
+
+
+class Association(root.AbstractMemberObject):
+    def __init__(self):
+        super().__init__()
+        self.lhs = None  # An entity
+        self.rhs = None  # Another entity
+
+
```

### Comparing `heaobject-1.0.0a8/src/heaobject/folder.py` & `heaobject-1.0.0a9/src/heaobject/folder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,98 @@
-from heaobject import root
-from typing import Optional
-import copy
-
-
-class Folder(root.AbstractDesktopObject):
-    def __init__(self):
-        super().__init__()
-
-
-class Item(root.AbstractMemberObject):
-    def __init__(self):
-        super().__init__()
-        self.__actual_object_type_name: Optional[str] = None
-        self.__actual_object_id: Optional[str] = None
-        self.__actual_object: Optional[root.HEAObject] = None
-        self.__folder_id: Optional[str] = None
-        self.__volume_id: Optional[str] = None
-
-    @property
-    def actual_object_type_name(self) -> Optional[str]:
-        """
-        The name of the type of the actual HEAObject.
-        """
-        return self.__actual_object_type_name
-
-    @actual_object_type_name.setter
-    def actual_object_type_name(self, actual_object_type_name: Optional[str]) -> None:
-        self.__actual_object_type_name = str(actual_object_type_name) if actual_object_type_name is not None else None
-
-    @property
-    def actual_object_id(self) -> Optional[str]:
-        """
-        The id of the actual HEAObject.
-        """
-        return self.__actual_object_id
-
-    @actual_object_id.setter
-    def actual_object_id(self, actual_object_id: Optional[str]) -> None:
-        self.__actual_object_id = str(actual_object_id) if actual_object_id is not None else None
-
-    @property
-    def actual_object(self) -> Optional[root.HEAObject]:
-        """
-        The actual HEAObject.
-        """
-        return self.__actual_object
-
-    @actual_object.setter
-    def actual_object(self, actual_object: Optional[root.HEAObject]) -> None:
-        self.__actual_object = copy.deepcopy(actual_object)
-
-    @property
-    def folder_id(self) -> Optional[str]:
-        """
-        The id of this item's folder.
-        """
-        return self.__folder_id
-
-    @folder_id.setter
-    def folder_id(self, folder_id: Optional[str]) -> None:
-        self.__folder_id = str(folder_id) if folder_id is not None else None
-
-    @property
-    def volume_id(self) -> Optional[str]:
-        """
-        The id of this item's volume.
-        """
-        return self.__volume_id
-
-    @volume_id.setter
-    def volume_id(self, volume_id: Optional[str]) -> None:
-        self.__volume_id = str(volume_id) if volume_id is not None else None
-
+from .data import DataObject, MimeTypeTransform
+from .root import AbstractMemberObject, DesktopObject
+from typing import Optional, List
+import copy
+
+
+class Folder(DataObject):
+    """
+    Represents a directory in the HEA desktop.
+    """
+    def __init__(self):
+        super().__init__()
+    
+    @property
+    def mime_type(self) -> str:
+        """
+        Read-only. Always returns 'application/x.folder'.
+        """
+        return 'application/x.folder'
+    
+    @property
+    def mime_type_transforms(self) -> List[MimeTypeTransform]:
+        """
+        Read-only. Always returns ['application/x.folder'].
+        """
+        m = MimeTypeTransform()
+        m.mime_type = 'application/x.folder'
+        return [m]
+
+
+
+class Item(AbstractMemberObject):
+    """
+    Represents an item in a folder. Items contain the actual object being pointed to as a nested 
+    """
+    def __init__(self):
+        super().__init__()
+        self.__actual_object_type_name: Optional[str] = None
+        self.__actual_object_id: Optional[str] = None
+        self.__actual_object: Optional[DesktopObject] = None
+        self.__folder_id: Optional[str] = None
+        self.__volume_id: Optional[str] = None
+
+    @property
+    def actual_object_type_name(self) -> Optional[str]:
+        """
+        The name of the type of the actual HEAObject.
+        """
+        return self.__actual_object_type_name
+
+    @actual_object_type_name.setter
+    def actual_object_type_name(self, actual_object_type_name: Optional[str]) -> None:
+        self.__actual_object_type_name = str(actual_object_type_name) if actual_object_type_name is not None else None
+
+    @property
+    def actual_object_id(self) -> Optional[str]:
+        """
+        The id of the actual HEAObject.
+        """
+        return self.__actual_object_id
+
+    @actual_object_id.setter
+    def actual_object_id(self, actual_object_id: Optional[str]) -> None:
+        self.__actual_object_id = str(actual_object_id) if actual_object_id is not None else None
+
+    @property
+    def actual_object(self) -> Optional[DesktopObject]:
+        """
+        The actual HEAObject.
+        """
+        return self.__actual_object
+
+    @actual_object.setter
+    def actual_object(self, actual_object: Optional[DesktopObject]) -> None:
+        self.__actual_object = copy.deepcopy(actual_object)
+
+    @property
+    def folder_id(self) -> Optional[str]:
+        """
+        The id of this item's folder.
+        """
+        return self.__folder_id
+
+    @folder_id.setter
+    def folder_id(self, folder_id: Optional[str]) -> None:
+        self.__folder_id = str(folder_id) if folder_id is not None else None
+
+    @property
+    def volume_id(self) -> Optional[str]:
+        """
+        The id of this item's volume.
+        """
+        return self.__volume_id
+
+    @volume_id.setter
+    def volume_id(self, volume_id: Optional[str]) -> None:
+        self.__volume_id = str(volume_id) if volume_id is not None else None
+
```

### Comparing `heaobject-1.0.0a8/src/heaobject/root.py` & `heaobject-1.0.0a9/src/heaobject/root.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,936 +1,967 @@
-"""
-A collection of classes and interfaces supporting the construction of data transfer objects for moving data between
-HEA microservices as well as between a HEA microservice and a web browser or other client. The HEAObject is the root
-interface for these data transfer objects, and AbstractHEAObject provides a root abstract implementation for them.
-See the docstring for HEAObject for details.
-"""
-
-import json
-from datetime import datetime, date
-from heaobject.error import DeserializeException
-from heaobject import user
-from enum import Enum, auto
-from typing import Optional, List, Union, Mapping, Any, Type, Iterator, Iterable, Callable, Generic, TypeVar
-import dateutil.parser
-import importlib
-import copy
-import inspect
-import abc
-
-
-class EnumAutoName(Enum):
-    """
-    Subclass of Enum in which auto() returns the name as a string.
-    """
-    def _generate_next_value_(name, start, count, last_values):
-        return name
-
-    def __str__(self) -> str:
-        return self.name
-
-class Permission(EnumAutoName):
-    """
-    The standard permissions that apply to all items in HEA.
-    """
-    VIEWER = auto()
-    EDITOR = auto()
-    COOWNER = auto()
-    EXECUTOR = auto()
-    SHARER = auto()
-
-
-
-
-class HEAObject(abc.ABC):
-    """
-    Interface for all HEA objects. HEA objects are data transfer objects for moving data between HEA microservices as
-    well as between a HEA microservice and a web browser or other client. HEA objects have no behavior except support
-    for storage, retrieval, serialization, and deserialization. The AbstractHEAObject class provides default
-    implementations for setting and getting attributes, as well as default implementations of behaviors.
-
-    There are two sub-types of HEA objects: desktop objects (DesktopObject) and owned
-    objects (MemberObject). The AbstractDesktopObject and AbstractMemberObject classes provide default implementations
-    for setting and getting attributes, and default implementations of behaviors. There may be additional sub-types in
-    the future.
-
-    Desktop objects represent objects that appear on the HEA desktop. Desktop objects have permissions, timestamps for
-    when the object was created and modified, versions, and more. One or more HEA microservices provide CRUD (create,
-    read, update, and delete) operations on each desktop object type. Additional HEA microservices may implement actions
-    that consume or produce specific desktop object types.
-
-    Owned objects cannot appear by themselves on the HEA desktop. Instead, they have a part-of relationship with a
-    desktop object, and their lifecycle is managed by the desktop object. Example owned objects represent permissions
-    and data sharing. While owned objects provide for their own storage, retrieval, serialization, and deserialization,
-    these behaviors are always invoked by the desktop object of which they are a part.
-
-    HEA object implementations must conform to several conventions to ease their use and reuse across the HEA desktop.
-    All subclasses of HEAObject must have a zero-argument constructor. All non-callable instance members must be
-    included in the to_dict() and json_dumps() methods. Copies and deep copies using the copy module will copy all
-    non-callable instance members of any subclass of HEAObject. Override __copy__ and __deepcopy__ to change that
-    behavior. In addition, HEA objects should include type annotations for all properties and callables.
-
-    Desktop objects implement no capability to check the current user when getting and setting owned objects, and
-    different users may only have access to a subset of its owned objects. Similarly, owned objects have no knowledge of
-    permissions at all. It is imperative that users gain access to desktop objects by calling an appropriate HEA
-    microservice as themselves, which will filter the owned objects that are returned according to their permissions.
-    """
-
-    @abc.abstractmethod
-    def to_dict(self) -> Mapping[str, Any]:
-        """
-        Returns a dict containing the attributes of this HEAObject instance. It gets the attributes to include by
-        calling the get_attributes class method.
-
-        :return: a dict of attribute names to attribute values.
-        """
-        pass
-
-    @abc.abstractmethod
-    def json_dumps(self, dumps: Callable[[Mapping[str, Any]], str] = json.dumps) -> str:
-        """
-        Returns a JSON-formatted string from the attributes of this instance. Passes the json_encode function as the
-        default parameter.
-
-        :param dumps: any callable that accepts a HEAObject and returns a string.
-        :return: a string.
-        """
-        pass
-
-    @abc.abstractmethod
-    def json_loads(self, jsn: str, loads: Callable[[Union[str]], Mapping[str, Any]] = json.loads) -> None:
-        """
-        Populates the object's attributes with the property values in the provided JSON. If the provided JSON has a
-        type property, this method requires that it match this object's type.
-
-        :param jsn: a JSON string.
-        :param loads: any callable that accepts str and returns dict with parsed JSON (json.loads() by default).
-        :raises DeserializeException: if any of the JSON object's values are wrong, or the provided JSON
-        document is not a valid JSON document.
-        """
-        pass
-
-    @abc.abstractmethod
-    def from_dict(self, d: Mapping[str, Any]) -> None:
-        """
-        Populates the object's attributes with the property values in the given dict. Supports nested dicts and lists.
-
-        :param d: a dict.
-        :raises DeserializeException: if any of the dict's values are wrong.
-        """
-        pass
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def type(self) -> str:
-        """
-        The string representation of this object's type.
-
-        :return: a string.
-        """
-        pass
-
-    @abc.abstractmethod
-    def get_attributes(self) -> Iterator[str]:
-        """
-        Returns a tuple containing the attributes that to_dict will write to a dictionary.
-
-        :return: an iterator of attribute names.
-        """
-        pass
-
-    @abc.abstractmethod
-    def get_all_attributes(self) -> Iterator[str]:
-        """
-        Returns a tuple containing all of this object's attributes.
-
-        :return: an iterator of attribute names.
-        """
-        pass
-
-    @classmethod
-    @abc.abstractmethod
-    def get_prompt(cls, field_name: Optional[str]) -> Optional[str]:
-        pass
-
-    @classmethod
-    @abc.abstractmethod
-    def is_displayed(cls, field_name: Optional[str]) -> bool:
-        pass
-
-    @classmethod
-    @abc.abstractmethod
-    def get_type_name(cls) -> str:
-        """
-        Returns a string representation of a HEAObject type.
-
-        :return: a type string.
-        """
-        pass
-
-    @classmethod
-    @abc.abstractmethod
-    def get_type_display_name(cls) -> Optional[str]:
-        """
-        Returns a display name for the HEAObject type, or None if there is no display name for this type.
-
-        :return: the display name string
-        """
-        pass
-
-
-class MemberObject(HEAObject, abc.ABC):
-    """
-    Interface for HEA objects that have a part-of relationship with a desktop objects and whose lifecycle is
-    managed by the desktop object. Owned objects have the same permissions as the owning desktop object. As a result,
-    they can be accessed by anyone who can access the desktop object, and they can be modified by anyone who can modify
-    the desktop object.
-    """
-    pass
-
-
-class PermissionAssignment(MemberObject, abc.ABC):
-    """
-    Interface for permission assignments for desktop objects. Desktop objects are owned by the user who created them.
-    After creating an object, the object's owner can share the object with other users with the desired set of
-    permissions. Optionally, users can invite another users to access the object with the desired set of permissions,
-    and the user will receive access upon accepting the invite. Permission assignment objects are owned by a desktop
-    object. As a result, they can be accessed by anyone who can access the desktop object, and they can be
-    modified by anyone who can modify the desktop object.
-    """
-
-    @property # type: ignore
-    @abc.abstractmethod
-    def user(self) -> str:
-        """
-        The user whose permissions will be impacted.
-        """
-        pass
-
-    @user.setter  # type: ignore
-    @abc.abstractmethod
-    def user(self, user_: str) -> None:
-        pass
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def permissions(self) -> List[Permission]:
-        """
-        The list of assigned permissions.
-        """
-        pass
-
-    @permissions.setter  # type: ignore
-    @abc.abstractmethod
-    def permissions(self, perms: List[Permission]):
-        pass
-
-
-class Invite(PermissionAssignment, abc.ABC):
-    """
-    Interface for invites to access a desktop object. Invite objects are owned by a desktop object, and as a result they
-    do not have permissions of their own.
-    """
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def accepted(self) -> bool:
-        """
-        Whether the user has accepted the invite.
-        """
-        pass
-
-    @accepted.setter  # type: ignore
-    @abc.abstractmethod
-    def accepted(self, accepted: bool) -> bool:
-        pass
-
-
-class Share(PermissionAssignment, abc.ABC):
-    """
-    Interface for representing the permissions of users to whom a desktop object has been shared. Share objects are
-    owned by a desktop object, and as a result they do not have permissions of their own.
-    """
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def invite(self) -> Invite:
-        """
-        The invite, if any.
-        """
-        pass
-
-    @invite.setter  # type: ignore
-    @abc.abstractmethod
-    def invite(self, invite: Invite) -> None:
-        pass
-
-
-class DesktopObject(HEAObject, abc.ABC):
-    """
-    Interface for objects that can appear on the HEA desktop. Desktop objects have permissions, with those permissions
-    represented by owned objects implementing the MemberObject interface. Other attributes may also employ owned
-    objects. One or more HEA microservices provide CRUD (create, read, update, and delete) operations on each desktop
-    object type. Additional HEA microservices may implement actions that use specific desktop object types.
-
-    Desktop objects implement no capability to check the current user when getting and setting owned objects, and
-    different users may only have access to a subset of its owned objects. Similarly, owned objects have no knowledge of
-    permissions at all. It is imperative that users gain access to desktop objects by calling an appropriate HEA
-    microservice as themselves, which will filter the owned objects that are returned according to their permissions.
-    """
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def id(self) -> Optional[str]:
-        """
-        The object's resource unique identifier. It must be unique among all objects of the same type.
-        """
-        pass
-
-    @id.setter  # type: ignore
-    @abc.abstractmethod
-    def id(self, id_: Optional[str]) -> None:
-        pass
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def source(self) -> Optional[str]:
-        """
-        The id of a Source object representing this object's source.
-        """
-        pass
-
-    @source.setter  # type: ignore
-    @abc.abstractmethod
-    def source(self, source: Optional[str]) -> Optional[str]:
-        pass
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def version(self) -> Optional[str]:
-        """
-        The version of this object.
-        """
-        pass
-
-    @version.setter  # type: ignore
-    @abc.abstractmethod
-    def version(self, version: Optional[str]) -> Optional[str]:
-        pass
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def name(self) -> Optional[str]:
-        """
-        This object's name. The name must be unique across all objects of the same type.
-        """
-        pass
-
-    @name.setter  # type: ignore
-    @abc.abstractmethod
-    def name(self, name: Optional[str]) -> Optional[str]:
-        pass
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def display_name(self) -> Optional[str]:
-        """
-        The object's display name. The default value is the object's name.
-        """
-        pass
-
-    @display_name.setter  # type: ignore
-    @abc.abstractmethod
-    def display_name(self, display_name: Optional[str]) -> Optional[str]:
-        pass
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def description(self) -> Optional[str]:
-        """
-        The object's description.
-        """
-        pass
-
-    @name.setter  # type: ignore
-    @abc.abstractmethod
-    def description(self, description: Optional[str]) -> Optional[str]:
-        pass
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def owner(self) -> str:
-        """
-        The username of the object's owner. Cannot be None.
-        """
-        pass
-
-    @owner.setter  # type: ignore
-    @abc.abstractmethod
-    def owner(self, owner: str) -> None:
-        pass
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def created(self) -> Optional[Union[date, datetime]]:
-        """
-        This object's created timestamp as a date or datetime object. Setting this property with an ISO 8601
-        string will also work -- the ISO string will be parsed automatically as a datetime object.
-        """
-        pass
-
-    @created.setter  # type: ignore
-    @abc.abstractmethod
-    def created(self, value: Optional[Union[date, datetime]]) -> None:
-        pass
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def modified(self) -> Optional[Union[date, datetime]]:
-        """
-        This object's last modified timestamp as a date or datetime object. Setting this property with an ISO 8601
-        string will also work -- the ISO string will be parsed automatically as a datetime object.
-        """
-        pass
-
-    @modified.setter  # type: ignore
-    @abc.abstractmethod
-    def modified(self, value: Optional[Union[date, datetime]]) -> None:
-        pass
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def derived_by(self) -> Optional[str]:
-        """
-        The id of the mechanism by which this object was derived, if any.
-        """
-        pass
-
-    @derived_by.setter  # type: ignore
-    @abc.abstractmethod
-    def derived_by(self, derived_by: Optional[str]) -> Optional[str]:
-        pass
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def derived_from(self) -> List[str]:
-        """
-        A list of the ids of the HEAObjects from which this object was derived. Cannot be None.
-        """
-        pass
-
-    @derived_from.setter  # type: ignore
-    @abc.abstractmethod
-    def derived_from(self, derived_from: List[str]) -> None:
-        pass
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def invites(self) -> List[Invite]:
-        """
-        A list of Invite objects representing the users who have been invited to access this object. Cannot be None.
-        """
-        pass
-
-    @invites.setter  # type: ignore
-    @abc.abstractmethod
-    def invites(self, invites: List[Invite]) -> None:
-        pass
-
-    @property  # type: ignore
-    @abc.abstractmethod
-    def shares(self) -> List[Share]:
-        """
-        A list of Share objects representing the users with whom this object has been shared.
-        """
-        pass
-
-    @shares.setter  # type: ignore
-    @abc.abstractmethod
-    def shares(self, shares: List[Share]) -> None:
-        pass
-
-
-class AbstractHEAObject(HEAObject, abc.ABC):
-    """
-    Abstract base class for all HEA objects. HEA objects are data transfer objects for moving data between HEA
-    microservices as well as between a HEA microservice and a web browser or other client. HEA objects have no behavior
-    except support for storage, retrieval, serialization, and deserialization. The AbstractHEAObject class provides
-    default implementations for setting and getting attributes, as well as default implementations of behaviors.
-
-    There are two sub-types of HEA objects: desktop objects (DesktopObject) and owned
-    objects (MemberObject). The AbstractDesktopObject and AbstractMemberObject classes provide default implementations
-    for setting and getting attributes, and default implementations of behaviors. There may be additional sub-types in
-    the future.
-
-    Desktop objects represent objects that appear on the HEA desktop. Desktop objects have permissions, timestamps for
-    when the object was created and modified, versions, and more. One or more HEA microservices provide CRUD (create,
-    read, update, and delete) operations on each desktop object type. Additional HEA microservices may implement actions
-    that consume or produce specific desktop object types.
-
-    Owned objects cannot appear by themselves on the HEA desktop. Instead, they have a part-of relationship with a
-    desktop object, and their lifecycle is managed by the desktop object. Example owned objects represent permissions
-    and data sharing. While owned objects provide for their own storage, retrieval, serialization, and deserialization,
-    these behaviors are always invoked by the desktop object of which they are a part.
-
-    HEA object implementations must conform to several conventions to ease their use and reuse across the HEA desktop.
-    All subclasses of HEAObject must have a zero-argument constructor. All non-callable instance members must be
-    included in the to_dict() and json_dumps() methods. Copies and deep copies using the copy module will copy all
-    non-callable instance members of any subclass of HEAObject. Override __copy__ and __deepcopy__ to change that
-    behavior. In addition, HEA objects should include type annotations for all properties and callables.
-
-    Desktop objects implement no capability to check the current user when getting and setting owned objects, and
-    different users may only have access to a subset of its owned objects. Similarly, owned objects have no knowledge of
-    permissions at all. It is imperative that users gain access to desktop objects by calling an appropriate HEA
-    microservice as themselves, which will filter the owned objects that are returned according to their permissions.
-    """
-    def __init__(self):
-        pass
-
-    def to_dict(self) -> Mapping[str, Any]:
-        def nested(obj):
-            if isinstance(obj, HEAObject):
-                return obj.to_dict()
-            elif isinstance(obj, list):
-                return [nested(o) for o in obj]
-            else:
-                return obj
-
-        return {a: nested(getattr(self, a)) for a in self.get_attributes()}
-
-    def json_dumps(self, dumps: Callable[[Mapping[str, Any]], str] = json.dumps) -> str:
-        return dumps(self.to_dict())
-
-    def json_loads(self, jsn: str, loads: Callable[[Union[str]], Mapping[str, Any]] = json.loads) -> None:
-        try:
-            self.from_dict(loads(jsn))
-        except json.JSONDecodeError as e:
-            raise DeserializeException from e
-
-    def from_dict(self, d: Mapping[str, Any]) -> None:
-        try:
-            for k, v in d.items():
-                if k in self.get_attributes():
-                    if isinstance(v, list):
-                        lst = []
-                        for e in v:
-                            if isinstance(e, dict):
-                                if 'type' not in e:
-                                    raise ValueError(
-                                        'type property is required in nested dicts but is missing from {}'.format(e))
-                                obj = type_for_name(e['type'])()
-                                obj.from_dict(e)
-                                lst.append(obj)
-                            else:
-                                lst.append(e)
-                        setattr(self, k, lst)
-                    elif isinstance(v, dict):
-                        if 'type' not in v:
-                            raise ValueError(
-                                'type property is required in nested dicts but is missing from {}'.format(v))
-                        obj = type_for_name(v['type'])()
-                        obj.from_dict(v)
-                        setattr(self, k, obj)
-                    elif k != 'type':
-                        setattr(self, k, v)
-                    else:
-                        if v != self.type:
-                            raise ValueError(
-                                f"type property does not match object type: object type is {self.type} but the dict's type property has value {v}")
-        except (ValueError, TypeError) as e:
-            raise DeserializeException from e
-
-    @property
-    def type(self) -> str:
-        return self.get_type_name()
-
-    def get_attributes(self) -> Iterator[str]:
-        return (m[0] for m in inspect.getmembers(self, self.__is_not_callable)
-                if not m[0].startswith('_') and m not in inspect.getmembers(type(self), self.__is_not_callable))
-
-    def get_all_attributes(self) -> Iterator[str]:
-        return (m[0] for m in inspect.getmembers(self, self.__is_not_callable)
-                if not m[0].startswith('_') and m not in inspect.getmembers(type(self), self.__is_not_callable))
-
-    @classmethod
-    def get_prompt(cls, field_name: Optional[str]) -> Optional[str]:
-        return field_name
-
-    @classmethod
-    def is_displayed(cls, field_name: Optional[str]) -> bool:
-        return True if field_name != 'id' else False
-
-    @classmethod
-    def get_type_name(cls) -> str:
-        return cls.__module__ + '.' + cls.__name__
-
-    @classmethod
-    def get_type_display_name(cls) -> Optional[str]:
-        """
-        Returns a display name for the HEAObject type, or None if there is no display name for this type. The default
-        implementation returns None. A concrete type implementation should override this method to return a display
-        name for the type.
-
-        :return: the display name string
-        """
-        return None
-
-    @staticmethod
-    def __is_not_callable(x) -> bool:
-        return not callable(x)
-
-    def __eq__(self, other) -> bool:
-        if not isinstance(other, type(self)):
-            return NotImplemented
-        attrs = set(self.get_all_attributes()).union(other.get_all_attributes())
-        return all(getattr(self, a, None) == getattr(other, a, None) for a in attrs)
-
-    def __repr__(self) -> str:
-        return 'heaobject.root.from_dict(' + repr(self.to_dict()) + ')'
-
-    def __copy__(self):
-        clz = type(self)
-        result = clz()
-        for a in self.get_attributes():
-            try:
-                setattr(result, a, getattr(self, a))
-            except AttributeError:
-                pass  # Skip read-only attributes
-        return result
-
-    def __deepcopy__(self, memo):
-        result = type(self)()
-        for a in self.get_attributes():
-            try:
-                setattr(result, a, copy.deepcopy(getattr(self, a), memo))
-            except AttributeError:
-                pass  # Skip read-only attributes
-        return result
-
-
-class AbstractMemberObject(AbstractHEAObject, MemberObject, abc.ABC):
-    """
-    Abstract base class for all classes that are owned by a desktop class. Owned classes have a part-of relationship
-    with a desktop class, and their lifecycle is managed by the desktop class. The desktop class and this class have a
-    composition relationship in UML. Owned objects have the same permissions as the owning desktop object. As a result,
-    they can be accessed by anyone who can access the desktop object, and they can be modified by anyone who can modify
-    the desktop object.
-    """
-    pass
-
-
-class AbstractPermissionAssignment(AbstractMemberObject, PermissionAssignment, abc.ABC):
-    """
-    Abstract base class for permissions-related classes. Desktop objects are owned by the user who created them.
-    After creating an object, the object's owner can share the object with other users with the desired set of
-    permissions. Optionally, users can invite another users to access the object with the desired set of permissions,
-    and the user will receive access upon accepting the invite. Permission assignment objects are owned by a desktop
-    object. As a result, they can be accessed by anyone who can access the desktop object, and they can be
-    modified by anyone who can modify the desktop object.
-    """
-    def __init__(self):
-        super().__init__()
-        self.__user = user.NONE_USER
-        self.__permissions: List[Permission] = []
-
-    @property
-    def user(self) -> str:
-        return self.__user
-
-    @user.setter
-    def user(self, user_: str) -> None:
-        self.__user = str(user_)
-
-    @property
-    def permissions(self) -> List[Permission]:
-        """
-        List of granted permissions. Any strings in the list will be parsed into Permission objects. Cannot be None.
-        Attempting to set this property to None will result in setting it to the empty list.
-        """
-        return copy.deepcopy(self.__permissions)
-
-    @permissions.setter
-    def permissions(self, perms: List[Permission]):
-        if perms is None:
-            self.__permissions = []
-        else:
-            perms_ = []
-            for p in perms:
-                if isinstance(p, str):
-                    perms_.append(Permission[p])
-                elif isinstance(p, Permission):
-                    perms_.append(p)
-                else:
-                    raise KeyError("permissions can only be a list of Permission objects or strings that can be converted to Permission objects")
-            self.__permissions = [Permission[p] for p in perms if isinstance(p, str)]
-
-
-class InviteImpl(AbstractPermissionAssignment, Invite):
-    """
-    Implementation of an invite.
-    """
-    def __init__(self):
-        super().__init__()
-        self.__accepted = False
-
-    @property
-    def accepted(self) -> bool:
-        return self.__accepted
-
-    @accepted.setter
-    def accepted(self, accepted: bool) -> None:
-        self.__accepted = bool(accepted)
-
-
-class ShareImpl(AbstractPermissionAssignment, Share):
-    """
-    Implementation of a share.
-    """
-    def __init__(self):
-        super().__init__()
-        self.__invite: Invite = None
-
-    @property
-    def invite(self) -> Invite:
-        return self.__invite
-
-    @invite.setter
-    def invite(self, invite: Invite) -> None:
-        if invite is not None and not isinstance(invite, Invite):
-            raise TypeError('invite not an Invite')
-        self.__invite = copy.deepcopy(invite)
-
-
-class AbstractDesktopObject(AbstractHEAObject, DesktopObject, abc.ABC):
-    """
-    Abstract base class representing HEA desktop objects. Desktop objects have permissions, with those permissions
-    represented by owned objects implementing the MemberObject interface. Other attributes may also employ owned
-    objects.
-
-    Desktop objects implement no capability to check the current user when getting and setting owned objects, and
-    different users may only have access to a subset of its owned objects. Similarly, owned objects have no knowledge of
-    permissions at all. It is imperative that users gain access to desktop objects by calling an appropriate HEA
-    microservice as themselves, which will filter the owned objects that are returned according to their permissions.
-    """
-
-    def __init__(self):
-        super().__init__()
-        self.__id: Optional[str] = None
-        self.__source: Optional[str] = None
-        self.__version: Optional[str] = None
-        self.__name: Optional[str] = None
-        self.__display_name: Optional[str] = None
-        self.__description: Optional[str] = None
-        self.__owner = user.NONE_USER
-        self.__created: Optional[Union[datetime, date]] = None  # The datetime when the object was created
-        self.__modified: Optional[Union[datetime, date]] = None  # The datetime when the object was last modified
-        self.__invites: List[Invite] = []
-        self.__shares: List[Share] = []
-        self.__derived_by = None
-        self.__derived_from = []
-
-    @property
-    def id(self) -> Optional[str]:
-        return self.__id
-
-    @id.setter
-    def id(self, id_: Optional[str]) -> None:
-        self.__id = str(id_) if id_ is not None else None
-
-    @property
-    def source(self) -> Optional[str]:
-        return self.__source
-
-    @source.setter
-    def source(self, source: Optional[str]) -> None:
-        self.__source = str(source) if source is not None else None
-
-    @property
-    def version(self) -> Optional[str]:
-        return self.__version
-
-    @version.setter
-    def version(self, version: Optional[str]) -> None:
-        self.__version = str(version) if version is not None else None
-
-    @property
-    def name(self) -> Optional[str]:
-        return self.__name
-
-    @name.setter
-    def name(self, name: Optional[str]) -> None:
-        self.__name = str(name) if name is not None else None
-
-    @property
-    def display_name(self) -> Optional[str]:
-        return self.__display_name
-
-    @display_name.setter
-    def display_name(self, display_name: Optional[str]) -> None:
-        self.__display_name = str(display_name) if display_name is not None else self.__name
-
-    @property
-    def description(self) -> Optional[str]:
-        return self.__description
-
-    @description.setter
-    def description(self, description: Optional[str]) -> None:
-        self.__description = str(description) if description is not None else None
-
-    @property
-    def owner(self) -> str:
-        return self.__owner
-
-    @owner.setter
-    def owner(self, owner: str) -> None:
-        self.__owner = str(owner)
-
-    @property
-    def created(self) -> Optional[Union[date, datetime]]:
-        return self.__created
-
-    @created.setter
-    def created(self, value: Optional[Union[date, datetime]]) -> None:
-        if value is None or isinstance(value, (datetime, date)):
-            self.__created = value
-        else:
-            self.__created = dateutil.parser.isoparse(value)
-
-    @property
-    def modified(self) -> Optional[Union[date, datetime]]:
-        return self.__modified
-
-    @modified.setter
-    def modified(self, value: Optional[Union[date, datetime]]) -> None:
-        if value is None or isinstance(value, (datetime, date)):
-            self.__modified = value
-        else:
-            self.__modified = dateutil.parser.isoparse(value)
-
-    @property
-    def derived_by(self) -> Optional[str]:
-        return self.__derived_by
-
-    @derived_by.setter
-    def derived_by(self, derived_by: Optional[str]) -> None:
-        self.__derived_by = str(derived_by) if derived_by is not None else None
-
-    @property
-    def derived_from(self) -> List[str]:
-        return list(self.__derived_from)
-
-    @derived_from.setter
-    def derived_from(self, derived_from: List[str]) -> None:
-        if derived_from is None:
-            raise ValueError('derived_from cannot be None')
-        if not all(isinstance(s, str) for s in derived_from):
-            raise TypeError('derived_from can only contain str objects')
-        self.__derived_from = list(derived_from)
-
-    @property
-    def invites(self) -> List[Invite]:
-        """
-        A list of Invite objects representing the users who have been invited to access this object. Cannot be None.
-        """
-        return copy.deepcopy(self.__invites)
-
-    @invites.setter
-    def invites(self, invites: List[Invite]) -> None:
-        if invites is None:
-            raise ValueError('invites cannot be None')
-        if not all(isinstance(s, Invite) for s in invites):
-            raise TypeError('invites can only contain Invite objects')
-        self.__invites = copy.deepcopy(invites)
-
-    @property
-    def shares(self) -> List[Share]:
-        """
-        A list of Share objects representing the users with whom this object has been shared.
-        """
-        return copy.deepcopy(self.__shares)
-
-    @shares.setter
-    def shares(self, shares: List[Share]) -> None:
-        if shares is None:
-            raise ValueError("shares cannot be None")
-        if not all(isinstance(s, Share) for s in shares):
-            raise TypeError("shares can only contain Share objects")
-        self.__shares = copy.deepcopy(shares)
-
-    def __str__(self) -> str:
-        if self.display_name:
-            return self.display_name
-        else:
-            return 'Untitled ' + type(self).__name__
-
-
-def json_dumps(o: HEAObject, dumps=json.dumps):
-    """
-    Serialize an HEAObject to a JSON document. It set the default parameter to the json_encode function.
-
-    :param o: the HEAObject to serialize.
-    :param dumps: the deserializer.
-    :return: a JSON document.
-    """
-    return dumps(o.to_dict(), default=json_encode)
-
-
-def json_encode(o) -> str:
-    """
-    Function to pass into the json.dumps default parameter that customizes encoding for HEAObject objects.
-
-    :param o: the object to encode.
-    :return: the object after encoding.
-    """
-    if isinstance(o, (datetime, date)):
-        return o.isoformat()
-    else:
-        return o
-
-
-def is_heaobject_type(name: str) -> bool:
-    """
-    Returns whether the supplied string is the name of an HEAObject type.
-    :param name: a string.
-    :return: True if the string is the name of an HEAObject type, or False if not.
-    """
-    try:
-        mod_str, cls_str = name.rsplit('.', 1)
-        result = getattr(importlib.import_module(mod_str), cls_str)
-        if not issubclass(result, HEAObject):
-            return False
-        return True
-    except ValueError:
-        return False
-
-
-def type_for_name(name: str) -> Type[HEAObject]:
-    """
-    Returns the HEAObject type for the given string.
-
-    :param name: a type string.
-    :return: a HEAObject type.
-    """
-    try:
-        mod_str, cls_str = name.rsplit('.', 1)
-        result = getattr(importlib.import_module(mod_str), cls_str)
-        if not issubclass(result, HEAObject):
-            raise TypeError(f'Name must be the name of an HEAObject type, but was {name}')
-        return result
-    except ValueError:
-        raise ValueError(f'{name} does not look like a module path')
-
-
-def from_dict(d: Mapping[str, Any]) -> HEAObject:
-    """
-    Creates a HEA object from the given dict.
-
-    :param d: a dict. It must have, at minimum, a type key with the type name of the HEA object to create. It must
-    additionally have key-value pairs for any mandatory attributes of the HEA object.
-    :return: a HEAObject.
-    """
-    type_name = d.get('type', None)
-    if not type_name:
-        raise ValueError('type key is required')
-    obj = type_for_name(type_name)()
-    obj.from_dict(d)
-    return obj
+"""
+A collection of classes and interfaces supporting the construction of data transfer objects for moving data between
+HEA microservices as well as between a HEA microservice and a web browser or other client. The HEAObject is the root
+interface for these data transfer objects, and AbstractHEAObject provides a root abstract implementation for them.
+See the docstring for HEAObject for details.
+"""
+
+import json
+from datetime import datetime, date
+from heaobject.error import DeserializeException
+from heaobject import user
+from enum import Enum, auto
+from typing import Optional, List, Union, Mapping, Any, Type, Iterator, Iterable, Callable, Generic, TypeVar
+import dateutil.parser
+import importlib
+import copy
+import inspect
+import abc
+import logging
+
+
+class EnumAutoName(Enum):
+    """
+    Subclass of Enum in which auto() returns the name as a string.
+    """
+    def _generate_next_value_(name, start, count, last_values):
+        return name
+
+    def __str__(self) -> str:
+        return self.name
+
+class Permission(EnumAutoName):
+    """
+    The standard permissions that apply to all HEA desktop objects.
+    """
+    VIEWER = auto()
+    EDITOR = auto()
+    COOWNER = auto()
+    EXECUTOR = auto()
+    SHARER = auto()
+
+
+
+
+class HEAObject(abc.ABC):
+    """
+    Interface for all HEA objects. HEA objects are data transfer objects for moving data between HEA microservices as
+    well as between a HEA microservice and a web browser or other client. HEA objects have no behavior except support
+    for storage, retrieval, serialization, and deserialization. The AbstractHEAObject class provides default
+    implementations for setting and getting attributes, as well as default implementations of behaviors.
+
+    There are two sub-types of HEA objects: desktop objects (DesktopObject) and owned
+    objects (MemberObject). The AbstractDesktopObject and AbstractMemberObject classes provide default implementations
+    for setting and getting attributes, and default implementations of behaviors. There may be additional sub-types in
+    the future.
+
+    Desktop objects represent objects that appear on the HEA desktop. Desktop objects have permissions, timestamps for
+    when the object was created and modified, versions, and more. One or more HEA microservices provide CRUD (create,
+    read, update, and delete) operations on each desktop object type. Additional HEA microservices may implement actions
+    that consume or produce specific desktop object types.
+
+    Member objects cannot appear by themselves on the HEA desktop. Instead, they have a part-of relationship with a
+    desktop object, and their lifecycle is managed by the desktop object. Example member objects represent permissions
+    and data sharing. While owned objects provide for their own storage, retrieval, serialization, and deserialization,
+    these behaviors are always invoked by the desktop object of which they are a part.
+
+    HEA objects must conform to several conventions to ease their use and reuse across the HEA desktop.
+    All subclasses of HEAObject must have a zero-argument constructor. Attribute values may be strings, numbers, booleans, 
+    enums, or a HEA object; or a list of strings, numbers, booleans, enums, or HEA objects. Attributes of type enum
+    must be implemented as a property with a setter that accepts both strings and the enum values, and will convert the 
+    strings to enum values.
+
+    In general, HEA objects implement composition relationships by making the container a desktop object and the "owned"
+    object a member object. Other association relationships are implemented by storing the id of the associated object
+    rather than nesting it. By convention, the id attributes are named hea_object_class_name_id, where hea_object_class_name
+    is the name of the class converted from camel case to underscores. There is one exception to this convention in the 
+    heaobject library. Item objects contain a nested copy of the desktop object that they refer to.
+    
+    Copies and deep copies using the copy module will copy all non-callable instance members of any subclass of HEAObject.
+    
+    In addition, HEA objects should include type annotations throughout.
+
+    It is imperative that users gain access to desktop objects by calling an appropriate HEA microservice as themselves, which 
+    will filter any nested member objects that are returned according to their permissions.
+    """
+
+    @abc.abstractmethod
+    def to_dict(self) -> Mapping[str, Any]:
+        """
+        Returns a dict containing the attributes of this HEAObject instance. It gets the attributes to include by
+        calling the get_attributes class method.
+
+        :return: a dict of attribute names to attribute values.
+        """
+        pass
+
+    @abc.abstractmethod
+    def json_dumps(self, dumps: Callable[[Mapping[str, Any]], str] = json.dumps) -> str:
+        """
+        Returns a JSON-formatted string from the attributes of this instance. Passes the json_encode function as the
+        default parameter.
+
+        :param dumps: any callable that accepts a HEAObject and returns a string.
+        :return: a string.
+        """
+        pass
+
+    @abc.abstractmethod
+    def json_loads(self, jsn: str, loads: Callable[[Union[str]], Mapping[str, Any]] = json.loads) -> None:
+        """
+        Populates the object's attributes with the property values in the provided JSON. If the provided JSON has a
+        type property, this method requires that it match this object's type.
+
+        :param jsn: a JSON string.
+        :param loads: any callable that accepts str and returns dict with parsed JSON (json.loads() by default).
+        :raises DeserializeException: if any of the JSON object's values are wrong, or the provided JSON
+        document is not a valid JSON document.
+        """
+        pass
+
+    @abc.abstractmethod
+    def from_dict(self, d: Mapping[str, Any]) -> None:
+        """
+        Populates the object's attributes with the property values in the given dict. 
+        
+        The supplied mapping may have nested dicts and lists. Dicts must have a type key whose value is a HEAObject type name, and
+        the other entries should correspond to attributes of that HEAObject type. Lists may contain strings, numbers, booleans, or dicts 
+        corresponding to an HEAObject type. Dict entries that correspond to read-only properties are ignored, as are
+        entries that do not have a corresponding attribute in the HEAObject type.
+
+        :param d: a dict.
+        :raises DeserializeException: if any of the dict's values are wrong.
+        """
+        pass
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def type(self) -> str:
+        """
+        The string representation of this object's type.
+
+        :return: a string.
+        """
+        pass
+
+    @abc.abstractmethod
+    def get_attributes(self) -> Iterator[str]:
+        """
+        Returns a tuple containing the attributes that to_dict will write to a dictionary.
+
+        :return: an iterator of attribute names.
+        """
+        pass
+
+    @abc.abstractmethod
+    def get_all_attributes(self) -> Iterator[str]:
+        """
+        Returns a tuple containing all of this object's attributes.
+
+        :return: an iterator of attribute names.
+        """
+        pass
+
+    @classmethod
+    @abc.abstractmethod
+    def get_prompt(cls, field_name: Optional[str]) -> Optional[str]:
+        pass
+
+    @classmethod
+    @abc.abstractmethod
+    def is_displayed(cls, field_name: Optional[str]) -> bool:
+        pass
+
+    @classmethod
+    @abc.abstractmethod
+    def get_type_name(cls) -> str:
+        """
+        Returns a string representation of a HEAObject type.
+
+        :return: a type string.
+        """
+        pass
+
+    @classmethod
+    @abc.abstractmethod
+    def get_type_display_name(cls) -> Optional[str]:
+        """
+        Returns a display name for the HEAObject type, or None if there is no display name for this type.
+
+        :return: the display name string
+        """
+        pass
+
+
+class MemberObject(HEAObject, abc.ABC):
+    """
+    Interface for HEA objects that have a part-of relationship with a desktop objects and whose lifecycle is
+    managed by the desktop object. Owned objects have the same permissions as the owning desktop object. As a result,
+    they can be accessed by anyone who can access the desktop object, and they can be modified by anyone who can modify
+    the desktop object.
+    """
+    pass
+
+
+class PermissionAssignment(MemberObject, abc.ABC):
+    """
+    Interface for permission assignments for desktop objects. Desktop objects are owned by the user who created them.
+    After creating an object, the object's owner can share the object with other users with the desired set of
+    permissions. Optionally, users can invite another users to access the object with the desired set of permissions,
+    and the user will receive access upon accepting the invite. Permission assignment objects are owned by a desktop
+    object. As a result, they can be accessed by anyone who can access the desktop object, and they can be
+    modified by anyone who can modify the desktop object.
+    """
+
+    @property # type: ignore
+    @abc.abstractmethod
+    def user(self) -> str:
+        """
+        The user whose permissions will be impacted.
+        """
+        pass
+
+    @user.setter  # type: ignore
+    @abc.abstractmethod
+    def user(self, user: str) -> None:
+        pass
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def permissions(self) -> List[Permission]:
+        """
+        The list of assigned permissions.
+        """
+        pass
+
+    @permissions.setter  # type: ignore
+    @abc.abstractmethod
+    def permissions(self, perms: List[Permission]):
+        pass
+
+
+class Invite(PermissionAssignment, abc.ABC):
+    """
+    Interface for invites to access a desktop object. Invite objects are owned by a desktop object, and as a result they
+    do not have permissions of their own.
+    """
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def accepted(self) -> bool:
+        """
+        Whether the user has accepted the invite.
+        """
+        pass
+
+    @accepted.setter  # type: ignore
+    @abc.abstractmethod
+    def accepted(self, accepted: bool) -> bool:
+        pass
+
+
+class Share(PermissionAssignment, abc.ABC):
+    """
+    Interface for representing the permissions of users to whom a desktop object has been shared. Share objects are
+    owned by a desktop object, and as a result they do not have permissions of their own.
+    """
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def invite(self) -> Invite:
+        """
+        The invite, if any.
+        """
+        pass
+
+    @invite.setter  # type: ignore
+    @abc.abstractmethod
+    def invite(self, invite: Invite) -> None:
+        pass
+
+
+class DesktopObject(HEAObject, abc.ABC):
+    """
+    Interface for objects that can appear on the HEA desktop. Desktop objects have permissions, with those permissions
+    represented by owned objects implementing the MemberObject interface. Other attributes may also employ owned
+    objects. One or more HEA microservices provide CRUD (create, read, update, and delete) operations on each desktop
+    object type. Additional HEA microservices may implement actions that use specific desktop object types.
+
+    Desktop objects implement no capability to check the current user when getting and setting owned objects, and
+    different users may only have access to a subset of its owned objects. Similarly, owned objects have no knowledge of
+    permissions at all. It is imperative that users gain access to desktop objects by calling an appropriate HEA
+    microservice as themselves, which will filter the owned objects that are returned according to their permissions.
+    """
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def id(self) -> Optional[str]:
+        """
+        The object's resource unique identifier. It must be unique among all objects of the same type.
+        """
+        pass
+
+    @id.setter  # type: ignore
+    @abc.abstractmethod
+    def id(self, id_: Optional[str]) -> None:
+        pass
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def source(self) -> Optional[str]:
+        """
+        The id of a Source object representing this object's source.
+        """
+        pass
+
+    @source.setter  # type: ignore
+    @abc.abstractmethod
+    def source(self, source: Optional[str]) -> Optional[str]:
+        pass
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def version(self) -> Optional[str]:
+        """
+        The version of this object.
+        """
+        pass
+
+    @version.setter  # type: ignore
+    @abc.abstractmethod
+    def version(self, version: Optional[str]) -> Optional[str]:
+        pass
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def name(self) -> Optional[str]:
+        """
+        This object's name. The name must be unique across all objects of the same type.
+        """
+        pass
+
+    @name.setter  # type: ignore
+    @abc.abstractmethod
+    def name(self, name: Optional[str]) -> Optional[str]:
+        pass
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def display_name(self) -> Optional[str]:
+        """
+        The object's display name. The default value is the object's name.
+        """
+        pass
+
+    @display_name.setter  # type: ignore
+    @abc.abstractmethod
+    def display_name(self, display_name: Optional[str]) -> Optional[str]:
+        pass
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def description(self) -> Optional[str]:
+        """
+        The object's description.
+        """
+        pass
+
+    @name.setter  # type: ignore
+    @abc.abstractmethod
+    def description(self, description: Optional[str]) -> Optional[str]:
+        pass
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def owner(self) -> str:
+        """
+        The username of the object's owner. Cannot be None.
+        """
+        pass
+
+    @owner.setter  # type: ignore
+    @abc.abstractmethod
+    def owner(self, owner: str) -> None:
+        pass
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def created(self) -> Optional[Union[date, datetime]]:
+        """
+        This object's created timestamp as a date or datetime object. Setting this property with an ISO 8601
+        string will also work -- the ISO string will be parsed automatically as a datetime object.
+        """
+        pass
+
+    @created.setter  # type: ignore
+    @abc.abstractmethod
+    def created(self, value: Optional[Union[date, datetime]]) -> None:
+        pass
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def modified(self) -> Optional[Union[date, datetime]]:
+        """
+        This object's last modified timestamp as a date or datetime object. Setting this property with an ISO 8601
+        string will also work -- the ISO string will be parsed automatically as a datetime object.
+        """
+        pass
+
+    @modified.setter  # type: ignore
+    @abc.abstractmethod
+    def modified(self, value: Optional[Union[date, datetime]]) -> None:
+        pass
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def derived_by(self) -> Optional[str]:
+        """
+        The id of the mechanism by which this object was derived, if any.
+        """
+        pass
+
+    @derived_by.setter  # type: ignore
+    @abc.abstractmethod
+    def derived_by(self, derived_by: Optional[str]) -> Optional[str]:
+        pass
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def derived_from(self) -> List[str]:
+        """
+        A list of the ids of the HEAObjects from which this object was derived. Cannot be None.
+        """
+        pass
+
+    @derived_from.setter  # type: ignore
+    @abc.abstractmethod
+    def derived_from(self, derived_from: List[str]) -> None:
+        pass
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def invites(self) -> List[Invite]:
+        """
+        A list of Invite objects representing the users who have been invited to access this object. Cannot be None.
+        """
+        pass
+
+    @invites.setter  # type: ignore
+    @abc.abstractmethod
+    def invites(self, invites: List[Invite]) -> None:
+        pass
+
+    @property  # type: ignore
+    @abc.abstractmethod
+    def shares(self) -> List[Share]:
+        """
+        A list of Share objects representing the users with whom this object has been shared.
+        """
+        pass
+
+    @shares.setter  # type: ignore
+    @abc.abstractmethod
+    def shares(self, shares: List[Share]) -> None:
+        pass
+
+
+class AbstractHEAObject(HEAObject, abc.ABC):
+    """
+    Abstract base class for all HEA objects. HEA objects are data transfer objects for moving data between HEA
+    microservices as well as between a HEA microservice and a web browser or other client. HEA objects have no behavior
+    except support for storage, retrieval, serialization, and deserialization. The AbstractHEAObject class provides
+    default implementations for setting and getting attributes, as well as default implementations of behaviors.
+
+    There are two sub-types of HEA objects: desktop objects (DesktopObject) and owned
+    objects (MemberObject). The AbstractDesktopObject and AbstractMemberObject classes provide default implementations
+    for setting and getting attributes, and default implementations of behaviors. There may be additional sub-types in
+    the future.
+
+    Desktop objects represent objects that appear on the HEA desktop. Desktop objects have permissions, timestamps for
+    when the object was created and modified, versions, and more. One or more HEA microservices provide CRUD (create,
+    read, update, and delete) operations on each desktop object type. Additional HEA microservices may implement actions
+    that consume or produce specific desktop object types.
+
+    Owned objects cannot appear by themselves on the HEA desktop. Instead, they have a part-of relationship with a
+    desktop object, and their lifecycle is managed by the desktop object. Example owned objects represent permissions
+    and data sharing. While owned objects provide for their own storage, retrieval, serialization, and deserialization,
+    these behaviors are always invoked by the desktop object of which they are a part.
+
+    HEA object implementations must conform to several conventions to ease their use and reuse across the HEA desktop.
+    All subclasses of HEAObject must have a zero-argument constructor. All non-callable instance members must be
+    included in the to_dict() and json_dumps() methods. Copies and deep copies using the copy module will copy all
+    non-callable instance members of any subclass of HEAObject. Override __copy__ and __deepcopy__ to change that
+    behavior. In addition, HEA objects should include type annotations for all properties and callables.
+
+    Desktop objects implement no capability to check the current user when getting and setting owned objects, and
+    different users may only have access to a subset of its owned objects. Similarly, owned objects have no knowledge of
+    permissions at all. It is imperative that users gain access to desktop objects by calling an appropriate HEA
+    microservice as themselves, which will filter the owned objects that are returned according to their permissions.
+    """
+    def __init__(self):
+        pass
+
+    def to_dict(self) -> Mapping[str, Any]:
+        def nested(obj):
+            if isinstance(obj, HEAObject):
+                return obj.to_dict()
+            elif isinstance(obj, list):
+                return [nested(o) for o in obj]
+            else:
+                return obj
+
+        return {a: nested(getattr(self, a)) for a in self.get_attributes()}
+
+    def json_dumps(self, dumps: Callable[[Mapping[str, Any]], str] = json.dumps) -> str:
+        return dumps(self.to_dict())
+
+    def json_loads(self, jsn: str, loads: Callable[[Union[str]], Mapping[str, Any]] = json.loads) -> None:
+        try:
+            self.from_dict(loads(jsn))
+        except json.JSONDecodeError as e:
+            raise DeserializeException from e
+
+    def from_dict(self, d: Mapping[str, Any]) -> None:
+        try:
+            for k, v in d.items():
+                if k in self.get_attributes():
+                    if isinstance(v, list):
+                        lst = []
+                        for e in v:
+                            if isinstance(e, dict):
+                                if 'type' not in e:
+                                    raise ValueError(
+                                        'type property is required in nested dicts but is missing from {}'.format(e))
+                                obj = type_for_name(e['type'])()
+                                obj.from_dict(e)
+                                lst.append(obj)
+                            else:
+                                lst.append(e)
+                        self.__setattr_known_and_writeable(k, lst)
+                    elif isinstance(v, dict):
+                        if 'type' not in v:
+                            raise ValueError(
+                                'type property is required in nested dicts but is missing from {}'.format(v))
+                        obj = type_for_name(v['type'])()
+                        obj.from_dict(v)
+                        self.__setattr_known_and_writeable(k, obj)
+                    elif k != 'type':
+                        self.__setattr_known_and_writeable(k, v)
+                    else:
+                        if v != self.type:
+                            raise ValueError(
+                                f"type property does not match object type: object type is {self.type} but the dict's type property has value {v}")
+        except (ValueError, TypeError) as e:
+            raise DeserializeException from e
+
+    @property
+    def type(self) -> str:
+        return self.get_type_name()
+
+    def get_attributes(self) -> Iterator[str]:
+        return (m[0] for m in inspect.getmembers(self, self.__is_not_callable)
+                if not m[0].startswith('_') and m not in inspect.getmembers(type(self), self.__is_not_callable))
+
+    def get_all_attributes(self) -> Iterator[str]:
+        return (m[0] for m in inspect.getmembers(self, self.__is_not_callable)
+                if not m[0].startswith('_') and m not in inspect.getmembers(type(self), self.__is_not_callable))
+
+    @classmethod
+    def get_prompt(cls, field_name: Optional[str]) -> Optional[str]:
+        return field_name
+
+    @classmethod
+    def is_displayed(cls, field_name: Optional[str]) -> bool:
+        return True if field_name != 'id' else False
+
+    @classmethod
+    def get_type_name(cls) -> str:
+        return cls.__module__ + '.' + cls.__name__
+
+    @classmethod
+    def get_type_display_name(cls) -> Optional[str]:
+        """
+        Returns a display name for the HEAObject type, or None if there is no display name for this type. The default
+        implementation returns None. A concrete type implementation should override this method to return a display
+        name for the type.
+
+        :return: the display name string
+        """
+        return None
+
+    @staticmethod
+    def __is_not_callable(x) -> bool:
+        return not callable(x)
+    
+    def __setattr_known_and_writeable(self, name: str, value: Any) -> None:
+        """
+        Sets any of this object's attributes, ignoring attempts to set read-only attributes or to monkey patch the object with additional attributes.
+
+        :param name: the name of the attribute.
+        :param value: the attribute's value.
+        """
+        logger = logging.getLogger()
+        if hasattr(self, name):
+            try:
+                setattr(self, name, value)
+            except AttributeError:
+                logger.debug('Tried setting attribute %s.%s=%s and got an error, most likely because the attribute is read-only. HEA will ignore this attribute.', self, name, value, exc_info=True)
+        else:
+            logger.debug('Attempted to set an unexpected attribute %s.%s=%s. HEA will ignore this attribute.', self, name, value)
+
+
+    def __eq__(self, other) -> bool:
+        if not isinstance(other, type(self)):
+            return NotImplemented
+        attrs = set(self.get_all_attributes()).union(other.get_all_attributes())
+        return all(getattr(self, a, None) == getattr(other, a, None) for a in attrs)
+
+    def __repr__(self) -> str:
+        return 'heaobject.root.from_dict(' + repr(self.to_dict()) + ')'
+
+    def __copy__(self):
+        clz = type(self)
+        result = clz()
+        for a in self.get_attributes():
+            try:
+                setattr(result, a, getattr(self, a))
+            except AttributeError:
+                pass  # Skip read-only attributes
+        return result
+
+    def __deepcopy__(self, memo):
+        result = type(self)()
+        for a in self.get_attributes():
+            try:
+                setattr(result, a, copy.deepcopy(getattr(self, a), memo))
+            except AttributeError:
+                pass  # Skip read-only attributes
+        return result
+
+
+class AbstractMemberObject(AbstractHEAObject, MemberObject, abc.ABC):
+    """
+    Abstract base class for all classes that are owned by a desktop class. Owned classes have a part-of relationship
+    with a desktop class, and their lifecycle is managed by the desktop class. The desktop class and this class have a
+    composition relationship in UML. Owned objects have the same permissions as the owning desktop object. As a result,
+    they can be accessed by anyone who can access the desktop object, and they can be modified by anyone who can modify
+    the desktop object.
+    """
+    pass
+
+
+class AbstractPermissionAssignment(AbstractMemberObject, PermissionAssignment, abc.ABC):
+    """
+    Abstract base class for permissions-related classes. Desktop objects are owned by the user who created them.
+    After creating an object, the object's owner can share the object with other users with the desired set of
+    permissions. Optionally, users can invite another users to access the object with the desired set of permissions,
+    and the user will receive access upon accepting the invite. Permission assignment objects are owned by a desktop
+    object. As a result, they can be accessed by anyone who can access the desktop object, and they can be
+    modified by anyone who can modify the desktop object.
+    """
+    def __init__(self):
+        super().__init__()
+        self.__user = user.NONE_USER
+        self.__permissions: List[Permission] = []
+
+    @property
+    def user(self) -> str:
+        return self.__user
+
+    @user.setter
+    def user(self, user: str) -> None:
+        self.__user = str(user)
+
+    @property
+    def permissions(self) -> List[Permission]:
+        """
+        List of granted permissions. Any strings in the list will be parsed into Permission objects. Cannot be None.
+        Attempting to set this property to None will result in setting it to the empty list.
+        """
+        return copy.deepcopy(self.__permissions)
+
+    @permissions.setter
+    def permissions(self, perms: List[Permission]):
+        if perms is None:
+            self.__permissions = []
+        else:
+            perms_ = []
+            for p in perms:
+                if isinstance(p, str):
+                    perms_.append(Permission[p])
+                elif isinstance(p, Permission):
+                    perms_.append(p)
+                else:
+                    raise KeyError("permissions can only be a list of Permission objects or strings that can be converted to Permission objects")
+            self.__permissions = [Permission[p] for p in perms if isinstance(p, str)]
+
+
+class InviteImpl(AbstractPermissionAssignment, Invite):
+    """
+    Implementation of an invite.
+    """
+    def __init__(self):
+        super().__init__()
+        self.__accepted = False
+
+    @property
+    def accepted(self) -> bool:
+        return self.__accepted
+
+    @accepted.setter
+    def accepted(self, accepted: bool) -> None:
+        self.__accepted = bool(accepted)
+
+
+class ShareImpl(AbstractPermissionAssignment, Share):
+    """
+    Implementation of a share.
+    """
+    def __init__(self):
+        super().__init__()
+        self.__invite: Invite = None
+
+    @property
+    def invite(self) -> Invite:
+        return self.__invite
+
+    @invite.setter
+    def invite(self, invite: Invite) -> None:
+        if invite is not None and not isinstance(invite, Invite):
+            raise TypeError('invite not an Invite')
+        self.__invite = copy.deepcopy(invite)
+
+
+class AbstractDesktopObject(AbstractHEAObject, DesktopObject, abc.ABC):
+    """
+    Abstract base class representing HEA desktop objects. Desktop objects have permissions, with those permissions
+    represented by owned objects implementing the MemberObject interface. Other attributes may also employ owned
+    objects.
+
+    Desktop objects implement no capability to check the current user when getting and setting owned objects, and
+    different users may only have access to a subset of its owned objects. Similarly, owned objects have no knowledge of
+    permissions at all. It is imperative that users gain access to desktop objects by calling an appropriate HEA
+    microservice as themselves, which will filter the owned objects that are returned according to their permissions.
+    """
+
+    def __init__(self):
+        super().__init__()
+        self.__id: Optional[str] = None
+        self.__source: Optional[str] = None
+        self.__version: Optional[str] = None
+        self.__name: Optional[str] = None
+        self.__display_name: Optional[str] = None
+        self.__description: Optional[str] = None
+        self.__owner = user.NONE_USER
+        self.__created: Optional[Union[datetime, date]] = None  # The datetime when the object was created
+        self.__modified: Optional[Union[datetime, date]] = None  # The datetime when the object was last modified
+        self.__invites: List[Invite] = []
+        self.__shares: List[Share] = []
+        self.__derived_by = None
+        self.__derived_from = []
+
+    @property
+    def id(self) -> Optional[str]:
+        return self.__id
+
+    @id.setter
+    def id(self, id_: Optional[str]) -> None:
+        self.__id = str(id_) if id_ is not None else None
+
+    @property
+    def source(self) -> Optional[str]:
+        return self.__source
+
+    @source.setter
+    def source(self, source: Optional[str]) -> None:
+        self.__source = str(source) if source is not None else None
+
+    @property
+    def version(self) -> Optional[str]:
+        return self.__version
+
+    @version.setter
+    def version(self, version: Optional[str]) -> None:
+        self.__version = str(version) if version is not None else None
+
+    @property
+    def name(self) -> Optional[str]:
+        return self.__name
+
+    @name.setter
+    def name(self, name: Optional[str]) -> None:
+        self.__name = str(name) if name is not None else None
+
+    @property
+    def display_name(self) -> Optional[str]:
+        return self.__display_name
+
+    @display_name.setter
+    def display_name(self, display_name: Optional[str]) -> None:
+        self.__display_name = str(display_name) if display_name is not None else self.__name
+
+    @property
+    def description(self) -> Optional[str]:
+        return self.__description
+
+    @description.setter
+    def description(self, description: Optional[str]) -> None:
+        self.__description = str(description) if description is not None else None
+
+    @property
+    def owner(self) -> str:
+        return self.__owner
+
+    @owner.setter
+    def owner(self, owner: str) -> None:
+        self.__owner = str(owner)
+
+    @property
+    def created(self) -> Optional[Union[date, datetime]]:
+        return self.__created
+
+    @created.setter
+    def created(self, value: Optional[Union[date, datetime]]) -> None:
+        if value is None or isinstance(value, (datetime, date)):
+            self.__created = value
+        else:
+            self.__created = dateutil.parser.isoparse(value)
+
+    @property
+    def modified(self) -> Optional[Union[date, datetime]]:
+        return self.__modified
+
+    @modified.setter
+    def modified(self, value: Optional[Union[date, datetime]]) -> None:
+        if value is None or isinstance(value, (datetime, date)):
+            self.__modified = value
+        else:
+            self.__modified = dateutil.parser.isoparse(value)
+
+    @property
+    def derived_by(self) -> Optional[str]:
+        return self.__derived_by
+
+    @derived_by.setter
+    def derived_by(self, derived_by: Optional[str]) -> None:
+        self.__derived_by = str(derived_by) if derived_by is not None else None
+
+    @property
+    def derived_from(self) -> List[str]:
+        return list(self.__derived_from)
+
+    @derived_from.setter
+    def derived_from(self, derived_from: List[str]) -> None:
+        if derived_from is None:
+            raise ValueError('derived_from cannot be None')
+        if not all(isinstance(s, str) for s in derived_from):
+            raise KeyError('derived_from can only contain str objects')
+        self.__derived_from = copy.deepcopy(list(derived_from) if isinstance(derived_from, list) else derived_from)
+
+    @property
+    def invites(self) -> List[Invite]:
+        """
+        A list of Invite objects representing the users who have been invited to access this object. Cannot be None.
+        """
+        return copy.deepcopy(self.__invites)
+
+    @invites.setter
+    def invites(self, invites: List[Invite]) -> None:
+        if invites is None:
+            raise ValueError('invites cannot be None')
+        if not all(isinstance(s, Invite) for s in invites):
+            raise KeyError('invites can only contain Invite objects')
+        self.__invites = copy.deepcopy(list(invites) if isinstance(invites, list) else invites)
+
+    @property
+    def shares(self) -> List[Share]:
+        """
+        A list of Share objects representing the users with whom this object has been shared.
+        """
+        return copy.deepcopy(self.__shares)
+
+    @shares.setter
+    def shares(self, shares: List[Share]) -> None:
+        if shares is None:
+            raise ValueError("shares cannot be None")
+        if not all(isinstance(s, Share) for s in shares):
+            raise KeyError("shares can only contain Share objects")
+        self.__shares = copy.deepcopy(list(shares) if isinstance(shares, list) else shares)
+
+    def __str__(self) -> str:
+        if self.display_name:
+            return self.display_name
+        else:
+            return 'Untitled ' + type(self).__name__
+
+
+def json_dumps(o: HEAObject, dumps=json.dumps):
+    """
+    Serialize an HEAObject to a JSON document. It set the default parameter to the json_encode function.
+
+    :param o: the HEAObject to serialize.
+    :param dumps: the deserializer.
+    :return: a JSON document.
+    """
+    return dumps(o.to_dict(), default=json_encode)
+
+
+def json_encode(o) -> str:
+    """
+    Function to pass into the json.dumps default parameter that customizes encoding for HEAObject objects.
+
+    :param o: the object to encode.
+    :return: the object after encoding.
+    """
+    if isinstance(o, (datetime, date)):
+        return o.isoformat()
+    else:
+        return o
+
+
+def is_heaobject_type(name: str) -> bool:
+    """
+    Returns whether the supplied string is the name of an HEAObject type.
+    :param name: a string.
+    :return: True if the string is the name of an HEAObject type, or False if not.
+    """
+    try:
+        mod_str, cls_str = name.rsplit('.', 1)
+        result = getattr(importlib.import_module(mod_str), cls_str)
+        if not issubclass(result, HEAObject):
+            return False
+        return True
+    except ValueError:
+        return False
+
+
+def type_for_name(name: str) -> Type[HEAObject]:
+    """
+    Returns the HEAObject type for the given string.
+
+    :param name: a type string.
+    :return: a HEAObject type.
+    """
+    try:
+        mod_str, cls_str = name.rsplit('.', 1)
+        result = getattr(importlib.import_module(mod_str), cls_str)
+        if not issubclass(result, HEAObject):
+            raise TypeError(f'Name must be the name of an HEAObject type, but was {name}')
+        return result
+    except ValueError:
+        raise ValueError(f'{name} does not look like a module path')
+
+
+def from_dict(d: Mapping[str, Any]) -> HEAObject:
+    """
+    Creates a HEA object from the given dict.
+
+    :param d: a dict. It must have, at minimum, a type key with the type name of the HEA object to create. It must
+    additionally have key-value pairs for any mandatory attributes of the HEA object.
+    :return: a HEAObject.
+    """
+    type_name = d.get('type', None)
+    if not type_name:
+        raise ValueError('type key is required')
+    obj = type_for_name(type_name)()
+    obj.from_dict(d)
+    return obj
```

### Comparing `heaobject-1.0.0a8/src/heaobject/source2target.py` & `heaobject-1.0.0a9/src/heaobject/source2target.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from heaobject import root
-from typing import List
-import copy
-
-
-class Mapping(root.AbstractMemberObject):
-    """Example:
-    """
-    def __init__(self):
-        super().__init__()
-        self.source = []     # An iterable of 2-tuples, each containing a record type and an attribute of the record.
-        self.target = tuple()    # A tuple containing a record type and attribute.
-        self.transform = None  # A function that transforms the source attribute(s) into a target attribute.
-        self.comment = None
-
-
-class Source2Target(root.AbstractDesktopObject):
-    def __init__(self):
-        super().__init__()
-        self.__mappings: List[Mapping] = []
-
-    @property
-    def mappings(self) -> List[Mapping]:
-        return copy.deepcopy(self.__mappings)
-
-    @mappings.setter
-    def mappings(self, mappings: List[Mapping]) -> None:
-        if mappings is None:
-            raise ValueError('mappings cannot be None')
-        if not all(isinstance(s, Mapping) for s in mappings):
-            raise TypeError('mappings can only contain Mapping objects')
-        self.__mappings = copy.deepcopy(mappings)
+from heaobject import root
+from typing import List
+import copy
+
+
+class Mapping(root.AbstractMemberObject):
+    """Example:
+    """
+    def __init__(self):
+        super().__init__()
+        self.source = []     # An iterable of 2-tuples, each containing a record type and an attribute of the record.
+        self.target = tuple()    # A tuple containing a record type and attribute.
+        self.transform = None  # A function that transforms the source attribute(s) into a target attribute.
+        self.comment = None
+
+
+class Source2Target(root.AbstractDesktopObject):
+    def __init__(self):
+        super().__init__()
+        self.__mappings: List[Mapping] = []
+
+    @property
+    def mappings(self) -> List[Mapping]:
+        return copy.deepcopy(self.__mappings)
+
+    @mappings.setter
+    def mappings(self, mappings: List[Mapping]) -> None:
+        if mappings is None:
+            raise ValueError('mappings cannot be None')
+        if not all(isinstance(s, Mapping) for s in mappings):
+            raise TypeError('mappings can only contain Mapping objects')
+        self.__mappings = copy.deepcopy(mappings)
```

### Comparing `heaobject-1.0.0a8/src/heaobject/volume.py` & `heaobject-1.0.0a9/src/heaobject/volume.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from abc import ABC
-from typing import Optional
-from heaobject import root
-
-
-class FileSystem(root.AbstractDesktopObject, ABC):
-    """
-    Represents a filesystem, which controls how data is stored and retrieved. In HEA, all filesystems are either
-    databases or network file storage.
-    """
-    pass
-
-
-class MongoDBFileSystem(FileSystem):
-    """
-    MongoDB-based filesystem.
-    """
-
-    def __init__(self):
-        super().__init__()
-        self.__connection_string: Optional[str] = None
-
-    @property  # type: ignore
-    def connection_string(self) -> Optional[str]:
-        """The MongoDB connection string."""
-        return self.__connection_string
-
-    @connection_string.setter
-    def connection_string(self, connection_string_: Optional[str]):
-        self.__connection_string = str(connection_string_) if connection_string_ is not None else None
-
-
-class Volume(root.AbstractDesktopObject):
-    """
-    A single accessible storage area that stores a single filesystem. Some volumes may require providing credentials in
-    order to access them.
-    """
-    def __init__(self):
-        super().__init__()
-        self.__file_system_name: Optional[str] = None
-        self.__credentials_id: Optional[str] = None
-
-    @property  # type: ignore
-    def file_system_name(self) -> Optional[str]:
-        """
-        The unique name of this volume's filesystem (a FileSystem object).
-        """
-        return self.__file_system_name
-
-    @file_system_name.setter  # type: ignore
-    def file_system_name(self, file_system_name_: Optional[str]) -> None:
-        self.__file_system_name = str(file_system_name_) if file_system_name_ is not None else None
-
-    @property  # type: ignore
-    def credentials_id(self) -> Optional[str]:
-        """
-        The id of this volume's credentials required for access (a Credentials object).
-        """
-        return self.__credentials_id
-
-    @credentials_id.setter  # type: ignore
-    def credentials_id(self, credentials_id_: Optional[str]) -> None:
-        self.__credentials_id = str(credentials_id_) if credentials_id_ is not None else None
+from abc import ABC
+from typing import Optional
+from heaobject import root
+
+
+class FileSystem(root.AbstractDesktopObject, ABC):
+    """
+    Represents a filesystem, which controls how data is stored and retrieved. In HEA, all filesystems are either
+    databases or network file storage.
+    """
+    pass
+
+
+class MongoDBFileSystem(FileSystem):
+    """
+    MongoDB-based filesystem.
+    """
+
+    def __init__(self):
+        super().__init__()
+        self.__connection_string: Optional[str] = None
+
+    @property  # type: ignore
+    def connection_string(self) -> Optional[str]:
+        """The MongoDB connection string."""
+        return self.__connection_string
+
+    @connection_string.setter
+    def connection_string(self, connection_string: Optional[str]):
+        self.__connection_string = str(connection_string) if connection_string is not None else None
+
+
+class Volume(root.AbstractDesktopObject):
+    """
+    A single accessible storage area that stores a single filesystem. Some volumes may require providing credentials in
+    order to access them.
+    """
+    def __init__(self):
+        super().__init__()
+        self.__file_system_name: Optional[str] = None
+        self.__credentials_id: Optional[str] = None
+
+    @property  # type: ignore
+    def file_system_name(self) -> Optional[str]:
+        """
+        The unique name of this volume's filesystem (a FileSystem object).
+        """
+        return self.__file_system_name
+
+    @file_system_name.setter  # type: ignore
+    def file_system_name(self, file_system_name: Optional[str]) -> None:
+        self.__file_system_name = str(file_system_name) if file_system_name is not None else None
+
+    @property  # type: ignore
+    def credentials_id(self) -> Optional[str]:
+        """
+        The id of this volume's credentials required for access (a Credentials object).
+        """
+        return self.__credentials_id
+
+    @credentials_id.setter  # type: ignore
+    def credentials_id(self, credentials_id: Optional[str]) -> None:
+        self.__credentials_id = str(credentials_id) if credentials_id is not None else None
```

### Comparing `heaobject-1.0.0a8/src/heaobject.egg-info/PKG-INFO` & `heaobject-1.0.0a9/src/heaobject.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-Metadata-Version: 2.1
-Name: heaobject
-Version: 1.0.0a8
-Summary: Data and other classes that are passed into and out of HEA REST APIs.
-Home-page: https://risr.hci.utah.edu
-Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
-Author-email: Andrew.Post@hci.utah.edu
-License: UNKNOWN
-Description: # HEA Object Library
-        [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
-        
-        The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
-        
-        ## Version 1
-        Initial release.
-        
-        ## Runtime requirements
-        * Python 3.8
-        
-        ## Development environment
-        
-        ### Build requirements
-        * Any development environment is fine.
-        * On Windows, you also will need:
-            * Build Tools for Visual Studio 2019, found at https://visualstudio.microsoft.com/downloads/. Select the C++ tools.
-            * git, found at https://git-scm.com/download/win.
-        * On Mac, Xcode or the command line developer tools is required, found in the Apple Store app.
-        * Python 3.8: Download and install Python 3.8 from https://www.python.org, and select the options to install for all users and add
-        Python to your environment variables. The install for all users option will help keep you from accidentally installing
-        packages into your Python installation's site-packages directory instead of to your virtualenv environment, described
-        below.
-        * Create a virtualenv environment using the `python -m venv <venv_directory>` command, substituting `<venv_directory>`
-        with the directory name of your virtual environment. Run `source <venv_directory>/bin/activate` (or `<venv_directory>/Scripts/activate` on Windows) to activate the virtual
-        environment. You will need to activate the virtualenv every time before starting work, or your IDE may be able to do 
-        this for you automatically. **Note that PyCharm will do this for you, but you have to create a new Terminal panel
-        after you newly configure a project with your virtualenv.**
-        * From the project's root directory, and using the activated virtualenv, run `pip install -r requirements_dev.txt`.
-        **Do NOT run `python setup.py develop`. It will break your environment.**
-        
-        ### Running unit tests
-        Run tests with the `pytest` command from the project root directory.
-        
-        ### Versioning
-        Use semantic versioning as described in 
-        https://packaging.python.org/guides/distributing-packages-using-setuptools/#choosing-a-versioning-scheme. In addition,
-        while development is underway, the version should be the next version number suffixed by -SNAPSHOT.
-        
-        ### Version tags in git
-        Version tags should follow the format `heaobject-<version>`, for example, `heaobject-1.0.0`.
-        
-        ### Uploading to an index server
-        You will need a custom index server such as devpi to upload HEA component releases so that HEA
-        components can depend on each other. You will need to configure pip to use the custom index server
-        instead of the usual Pypi.
-        
-        The following instructions assume separate stable and staging indexes. Numbered releases, including alphas and betas, go 
-        into the stable index. Snapshots of works in progress go into the staging index. Artifacts uploaded to the
-        staging index can be overwritten. Artifacts uploaded to stable cannot. Thus, also use staging to upload numbered
-        releases, verify the uploaded packages, and then upload to stable.
-        
-        From the project's root directory:
-        1. For numbered releases, remove `.dev` from the version number in setup.py, tag it in git to indicate a release, 
-        and commit to version control. Skip this step for SNAPSHOT releases.
-        2. Run `python setup.py clean --all sdist bdist_wheel` to create the artifacts.
-        3. Run `twine upload -r <repository> dist/*` to upload to the repository. The repository name has to be defined in a
-        twine configuration file such as `$HOME/.pypirc`.
-        4. For numbered releases, increment the version number in setup.py, append `.dev` to it, and commit to version 
-        control. Skip this step for SNAPSHOT releases.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: heaobject
+Version: 1.0.0a9
+Summary: Data and other classes that are passed into and out of HEA REST APIs.
+Home-page: https://risr.hci.utah.edu
+Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
+Author-email: Andrew.Post@hci.utah.edu
+License: UNKNOWN
+Description: # HEA Object Library
+        [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
+        
+        The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
+        
+        ## Version 1
+        Initial release.
+        
+        ## Runtime requirements
+        * Python 3.8
+        
+        ## Development environment
+        
+        ### Build requirements
+        * Any development environment is fine.
+        * On Windows, you also will need:
+            * Build Tools for Visual Studio 2019, found at https://visualstudio.microsoft.com/downloads/. Select the C++ tools.
+            * git, found at https://git-scm.com/download/win.
+        * On Mac, Xcode or the command line developer tools is required, found in the Apple Store app.
+        * Python 3.8: Download and install Python 3.8 from https://www.python.org, and select the options to install for all users and add
+        Python to your environment variables. The install for all users option will help keep you from accidentally installing
+        packages into your Python installation's site-packages directory instead of to your virtualenv environment, described
+        below.
+        * Create a virtualenv environment using the `python -m venv <venv_directory>` command, substituting `<venv_directory>`
+        with the directory name of your virtual environment. Run `source <venv_directory>/bin/activate` (or `<venv_directory>/Scripts/activate` on Windows) to activate the virtual
+        environment. You will need to activate the virtualenv every time before starting work, or your IDE may be able to do 
+        this for you automatically. **Note that PyCharm will do this for you, but you have to create a new Terminal panel
+        after you newly configure a project with your virtualenv.**
+        * From the project's root directory, and using the activated virtualenv, run `pip install -r requirements_dev.txt`.
+        **Do NOT run `python setup.py develop`. It will break your environment.**
+        
+        ### Running unit tests
+        Run tests with the `pytest` command from the project root directory.
+        
+        ### Versioning
+        Use semantic versioning as described in 
+        https://packaging.python.org/guides/distributing-packages-using-setuptools/#choosing-a-versioning-scheme. In addition,
+        while development is underway, the version should be the next version number suffixed by -SNAPSHOT.
+        
+        ### Version tags in git
+        Version tags should follow the format `heaobject-<version>`, for example, `heaobject-1.0.0`.
+        
+        ### Uploading to an index server
+        You will need a custom index server such as devpi to upload HEA component releases so that HEA
+        components can depend on each other. You will need to configure pip to use the custom index server
+        instead of the usual Pypi.
+        
+        The following instructions assume separate stable and staging indexes. Numbered releases, including alphas and betas, go 
+        into the stable index. Snapshots of works in progress go into the staging index. Artifacts uploaded to the
+        staging index can be overwritten. Artifacts uploaded to stable cannot. Thus, also use staging to upload numbered
+        releases, verify the uploaded packages, and then upload to stable.
+        
+        From the project's root directory:
+        1. For numbered releases, remove `.dev` from the version number in setup.py, tag it in git to indicate a release, 
+        and commit to version control. Skip this step for SNAPSHOT releases.
+        2. Run `python setup.py clean --all sdist bdist_wheel` to create the artifacts.
+        3. Run `twine upload -r <repository> dist/*` to upload to the repository. The repository name has to be defined in a
+        twine configuration file such as `$HOME/.pypirc`.
+        4. For numbered releases, increment the version number in setup.py, append `.dev` to it, and commit to version 
+        control. Skip this step for SNAPSHOT releases.
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
```

### Comparing `heaobject-1.0.0a8/src/heaobject.egg-info/SOURCES.txt` & `heaobject-1.0.0a9/src/heaobject.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 README.md
 setup.py
 src/heaobject/__init__.py
+src/heaobject/data.py
 src/heaobject/dataadapter.py
 src/heaobject/dataelement.py
 src/heaobject/datamodel.py
 src/heaobject/datapattern.py
-src/heaobject/dataset.py
+src/heaobject/datatransform.py
 src/heaobject/error.py
 src/heaobject/folder.py
 src/heaobject/keychain.py
 src/heaobject/py.typed
 src/heaobject/record.py
 src/heaobject/registry.py
 src/heaobject/root.py
```

