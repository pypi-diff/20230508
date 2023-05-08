# Comparing `tmp/PyHaier-0.1.4.tar.gz` & `tmp/PyHaier-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHaier-0.1.4.tar", last modified: Wed Apr 19 20:38:47 2023, max compression
+gzip compressed data, was "PyHaier-0.1.5.tar", last modified: Mon May  8 15:33:57 2023, max compression
```

## Comparing `PyHaier-0.1.4.tar` & `PyHaier-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-04-19 20:38:47.121937 PyHaier-0.1.4/
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)    34523 2023-04-18 19:35:25.000000 PyHaier-0.1.4/LICENSE
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)     5711 2023-04-19 20:38:47.121937 PyHaier-0.1.4/PKG-INFO
-drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-04-19 20:38:47.121020 PyHaier-0.1.4/PyHaier/
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      164 2023-04-19 20:38:27.000000 PyHaier-0.1.4/PyHaier/GetCHTemp.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)       24 2023-04-19 20:38:27.000000 PyHaier-0.1.4/PyHaier/GetCompFreq.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      174 2023-04-19 20:38:27.000000 PyHaier-0.1.4/PyHaier/GetDHWCurTemp.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      155 2023-04-19 20:38:27.000000 PyHaier-0.1.4/PyHaier/GetDHWTemp.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      271 2023-04-19 20:38:27.000000 PyHaier-0.1.4/PyHaier/GetMode.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      776 2023-04-19 20:38:27.000000 PyHaier-0.1.4/PyHaier/GetState.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      570 2023-04-19 20:38:27.000000 PyHaier-0.1.4/PyHaier/GetTwiTwo.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      379 2023-04-19 20:38:27.000000 PyHaier-0.1.4/PyHaier/SetCHTemp.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      378 2023-04-19 20:38:27.000000 PyHaier-0.1.4/PyHaier/SetDHWTemp.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      248 2023-04-19 20:38:27.000000 PyHaier-0.1.4/PyHaier/SetMode.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)     1094 2023-04-19 20:38:27.000000 PyHaier-0.1.4/PyHaier/SetState.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      399 2023-04-19 20:38:27.000000 PyHaier-0.1.4/PyHaier/__init__.py
-drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-04-19 20:38:47.121937 PyHaier-0.1.4/PyHaier.egg-info/
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)     5711 2023-04-19 20:38:47.000000 PyHaier-0.1.4/PyHaier.egg-info/PKG-INFO
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      409 2023-04-19 20:38:47.000000 PyHaier-0.1.4/PyHaier.egg-info/SOURCES.txt
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)        1 2023-04-19 20:38:47.000000 PyHaier-0.1.4/PyHaier.egg-info/dependency_links.txt
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)        8 2023-04-19 20:38:47.000000 PyHaier-0.1.4/PyHaier.egg-info/top_level.txt
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)     5083 2023-04-18 20:04:07.000000 PyHaier-0.1.4/README.md
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      609 2023-04-19 20:35:46.000000 PyHaier-0.1.4/pyproject.toml
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)       38 2023-04-19 20:38:47.121937 PyHaier-0.1.4/setup.cfg
+drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-05-08 15:33:57.967453 PyHaier-0.1.5/
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      204 2023-05-08 15:33:57.966537 PyHaier-0.1.5/PKG-INFO
+drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-05-08 15:33:57.966537 PyHaier-0.1.5/PyHaier/
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      164 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/GetCHTemp.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)       24 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/GetCompFreq.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      174 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/GetDHWCurTemp.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      155 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/GetDHWTemp.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      271 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/GetMode.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      776 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/GetState.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      570 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/GetTwiTwo.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      458 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/SetCHTemp.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      463 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/SetDHWTemp.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      248 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/SetMode.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)     1282 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/SetState.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      399 2023-05-08 15:33:40.000000 PyHaier-0.1.5/PyHaier/__init__.py
+drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-05-08 15:33:57.966537 PyHaier-0.1.5/PyHaier.egg-info/
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      204 2023-05-08 15:33:57.000000 PyHaier-0.1.5/PyHaier.egg-info/PKG-INFO
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      395 2023-05-08 15:33:57.000000 PyHaier-0.1.5/PyHaier.egg-info/SOURCES.txt
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)        1 2023-05-08 15:33:57.000000 PyHaier-0.1.5/PyHaier.egg-info/dependency_links.txt
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)        8 2023-05-08 15:33:57.000000 PyHaier-0.1.5/PyHaier.egg-info/top_level.txt
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)     5238 2023-05-08 15:33:40.000000 PyHaier-0.1.5/README.md
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)       38 2023-05-08 15:33:57.967453 PyHaier-0.1.5/setup.cfg
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      323 2023-05-08 15:33:40.000000 PyHaier-0.1.5/setup.py
```

### Comparing `PyHaier-0.1.4/PKG-INFO` & `PyHaier-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: PyHaier
-Version: 0.1.4
-Summary: Very simple library to manipulate the basic parameters of the Haier heat pump.
-Author-email: Jacek Brzozowski <jacekbrzozowski.pld@gmail.com>
-Project-URL: Homepage, https://github.com/ktostam/PyHaier
-Project-URL: Bug Tracker, https://github.com/ktostam/PyHaier/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyHaier
 
 Very simple (for now) library to manipulate the basic parameters of the Haier heat pump.
 
 ## Donation
 If you like My work and want to support me, you can:
 
@@ -26,16 +11,23 @@
 
 [<img width="150px" src="https://buycoffee.to/btn/buycoffeeto-btn-primary.svg">](https://buycoffee.to/jacekbrzozz)
 
 ## Support
 For support, join our Discord channel https://discord.gg/7aF38puD
 
 ## Version
+### 0.1.5
+- More error handling
+
+### 0.1.4
+- Update in error handling
+
 ### 0.1.3
-- Fix function SetState
+New function
+- Add function to read Compressor frequency
 
 ### 0.1.2
 New function:
 - Get value of Twi and Two parameters (not 100% sure if this is OK.)
 
 ### 0.1.1
 New function:
@@ -56,14 +48,20 @@
 1. AU082FYCRA(HW)
 2. AU162FYCRA(HW)
 
 However, it should work with all pumps that feature the YR-e27 remote control
 
 ## Instalation
 
+**Install from pip**
+
+```shell
+$ pip install PyHaier
+```
+
 **Install from source**
 ```shell
 $ git clone https://github.com/ktostam/PyHaier.git
 $ cd PyHaier
 $ python setup.py install
 ```
 
@@ -216,8 +214,8 @@
 $ python script.py
 Current stete:	Heat+Tank ON
 New state:	Cool+Tank ON
 
 ```
 ## License
 
- GNU AGPL v3.0 [©Jacek Brzozowski](https://github.com/ktostam)
+ GNU GPL [©Jacek Brzozowski](https://github.com/ktostam)
```

### Comparing `PyHaier-0.1.4/PyHaier/GetState.py` & `PyHaier-0.1.5/PyHaier/GetState.py`

 * *Files identical despite different names*

### Comparing `PyHaier-0.1.4/PyHaier/GetTwiTwo.py` & `PyHaier-0.1.5/PyHaier/GetTwiTwo.py`

 * *Files identical despite different names*

### Comparing `PyHaier-0.1.4/PyHaier/SetState.py` & `PyHaier-0.1.5/PyHaier/SetState.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,46 +2,49 @@
     """
     function to change pump state
 
     :param current:
     :param new:
     :return:
     """
-    newstate=[]
-    if len(str(current[3])) <4 or len(str(current[0])) <4:
-        return "Error"
+    try:
+        newstate=[]
+        if len(str(current[3])) <4 or len(str(current[0])) <4:
+            return "Error"
 
-    if new == "off":
-        if int(hex(current[0])[4:6])%2 == 1:
-            state=int(hex(current[0])[4:6])-1
+        if new == "off":
+            if int(hex(current[0])[4:6])%2 == 1:
+                state=int(hex(current[0])[4:6])-1
+            else:
+                return -1
+        elif new == "on":
+            if int(hex(current[0])[4:6]%2) == 0:
+                state=int(hex(current[0])[4:6])+1
+            else:
+                return -1
+        elif new == "C":
+            state=3
+        elif new == "H":
+            state=5
+        elif new == "T":
+            state=87
+        elif new == "CT":
+            state=83
+        elif new == "HT":
+            state=85
         else:
             return -1
-    elif new == "on":
-        if int(hex(current[0])[4:6]%2) == 0:
-            state=int(hex(current[0])[4:6])+1
-        else:
-            return -1
-    elif new == "C":
-        state=3
-    elif new == "H":
-        state=5
-    elif new == "T":
-        state=87
-    elif new == "CT":
-        state=83
-    elif new == "HT":
-        state=85
-    else:
-        return -1
 
-    if state%2 == 0:
-        num=256
-    else:
-        num=34304
-    newstate.append(num+int(str(int(state)),16))
-    newstate.append(current[1])
-    newstate.append(int(hex(current[2])[2:6], 16))
-    newstate.append(int(hex(current[3])[4:6], 16))
-    newstate.append(int(hex(current[4])[4:6], 16))
-    newstate.append(current[5])
+        if state%2 == 0:
+            num=256
+        else:
+            num=34304
+        newstate.append(num+int(str(int(state)),16))
+        newstate.append(current[1])
+        newstate.append(int(hex(current[2])[2:6], 16))
+        newstate.append(int(hex(current[3])[4:6], 16))
+        newstate.append(int(hex(current[4])[4:6], 16))
+        newstate.append(current[5])
 
-    return newstate
+        return newstate
+    except:
+        return "ERROR"
```

