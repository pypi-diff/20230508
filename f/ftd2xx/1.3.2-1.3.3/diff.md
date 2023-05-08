# Comparing `tmp/ftd2xx-1.3.2.tar.gz` & `tmp/ftd2xx-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftd2xx-1.3.2.tar", last modified: Thu Apr 13 10:20:53 2023, max compression
+gzip compressed data, was "ftd2xx-1.3.3.tar", last modified: Mon May  8 19:02:40 2023, max compression
```

## Comparing `ftd2xx-1.3.2.tar` & `ftd2xx-1.3.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:20:53.941053 ftd2xx-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-13 10:20:53.941053 ftd2xx-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:20:53.941053 ftd2xx-1.3.2/ftd2xx/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34987 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/_ftd2xx.py
--rw-r--r--   0 runner    (1001) docker     (123)    95427 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/_ftd2xx_darwin.py
--rw-r--r--   0 runner    (1001) docker     (123)    37524 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/_ftd2xx_linux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:20:53.941053 ftd2xx-1.3.2/ftd2xx/aio/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/aio/aio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/defines.py
--rw-r--r--   0 runner    (1001) docker     (123)    19978 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/ftd2xx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:20:53.941053 ftd2xx-1.3.2/ftd2xx/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/tests/t_aio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/tests/t_ftd2xx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:20:53.941053 ftd2xx-1.3.2/ftd2xx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-13 10:20:53.000000 ftd2xx-1.3.2/ftd2xx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-13 10:20:53.000000 ftd2xx-1.3.2/ftd2xx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:20:53.000000 ftd2xx-1.3.2/ftd2xx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:20:53.000000 ftd2xx-1.3.2/ftd2xx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 10:20:53.000000 ftd2xx-1.3.2/ftd2xx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 10:20:53.000000 ftd2xx-1.3.2/ftd2xx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/myversion.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-13 10:20:53.941053 ftd2xx-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:02:40.309650 ftd2xx-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-08 19:02:40.309650 ftd2xx-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:02:40.309650 ftd2xx-1.3.3/ftd2xx/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/ftd2xx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36449 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/ftd2xx/_ftd2xx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95427 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/ftd2xx/_ftd2xx_darwin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37524 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/ftd2xx/_ftd2xx_linux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:02:40.309650 ftd2xx-1.3.3/ftd2xx/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/ftd2xx/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/ftd2xx/aio/aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/ftd2xx/defines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21755 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/ftd2xx/ftd2xx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:02:40.309650 ftd2xx-1.3.3/ftd2xx/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/ftd2xx/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/ftd2xx/tests/t_aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/ftd2xx/tests/t_ftd2xx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:02:40.309650 ftd2xx-1.3.3/ftd2xx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-08 19:02:40.000000 ftd2xx-1.3.3/ftd2xx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-08 19:02:40.000000 ftd2xx-1.3.3/ftd2xx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:02:40.000000 ftd2xx-1.3.3/ftd2xx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:02:40.000000 ftd2xx-1.3.3/ftd2xx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-08 19:02:40.000000 ftd2xx-1.3.3/ftd2xx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 19:02:40.000000 ftd2xx-1.3.3/ftd2xx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/myversion.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-08 19:02:40.313650 ftd2xx-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-08 19:02:28.000000 ftd2xx-1.3.3/setup.py
```

### Comparing `ftd2xx-1.3.2/LICENSE` & `ftd2xx-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.2/PKG-INFO` & `ftd2xx-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftd2xx
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python interface to ftd2xx.dll from FTDI using ctypesbased on d2xx by Pablo Bleyer
 Home-page: https://github.com/snmishra/ftd2xx
 Author: Satya Mishra
 Author-email: satya.devel@gmail.com
 License: MIT
 Keywords: ftd2xx d2xx ftdi
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ftd2xx-1.3.2/README.rst` & `ftd2xx-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.2/ftd2xx/__init__.py` & `ftd2xx-1.3.3/ftd2xx/__init__.py`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.2/ftd2xx/_ftd2xx.py` & `ftd2xx-1.3.3/ftd2xx/_ftd2xx.py`

 * *Files 4% similar despite different names*

```diff
@@ -395,14 +395,59 @@
         ("InvertRI", UCHAR),
         ("Cbus0", UCHAR),
         ("Cbus1", UCHAR),
         ("Cbus2", UCHAR),
         ("Cbus3", UCHAR),
         ("Cbus4", UCHAR),
         ("RIsVCP", UCHAR),
+        ("PullDownEnable7", UCHAR),
+        ("SerNumEnable7", UCHAR),
+        ("ALSlowSlew", UCHAR),
+        ("ALSchmittInput", UCHAR),
+        ("ALDriveCurrent", UCHAR),
+        ("AHSlowSlew", UCHAR),
+        ("AHSchmittInput", UCHAR),
+        ("AHDriveCurrent", UCHAR),
+        ("BLSlowSlew", UCHAR),
+        ("BLSchmittInput", UCHAR),
+        ("BLDriveCurrent", UCHAR),
+        ("BHSlowSlew", UCHAR),
+        ("BHSchmittInput", UCHAR),
+        ("BHDriveCurrent", UCHAR),
+        ("IFAIsFifo7", UCHAR),
+        ("IFAIsFifoTar7", UCHAR),
+        ("IFAIsFastSer7", UCHAR),
+        ("AIsVCP7", UCHAR),
+        ("IFBIsFifo7", UCHAR),
+        ("IFBIsFifoTar7", UCHAR),
+        ("IFBIsFastSer7", UCHAR),
+        ("BIsVCP7", UCHAR),
+        ("PowerSaveEnable", UCHAR),
+        ("PullDownEnable8", UCHAR),
+        ("SerNumEnable8", UCHAR),
+        ("ASlowSlew", UCHAR),
+        ("ASchmittInput", UCHAR),
+        ("ADriveCurrent", UCHAR),
+        ("BSlowSlew", UCHAR),
+        ("BSchmittInput", UCHAR),
+        ("BDriveCurrent", UCHAR),
+        ("CSlowSlew", UCHAR),
+        ("CSchmittInput", UCHAR),
+        ("CDriveCurrent", UCHAR),
+        ("DSlowSlew", UCHAR),
+        ("DSchmittInput", UCHAR),
+        ("DDriveCurrent", UCHAR),
+        ("ARIIsTXDEN", UCHAR),
+        ("BRIIsTXDEN", UCHAR),
+        ("CRIIsTXDEN", UCHAR),
+        ("DRIIsTXDEN", UCHAR),
+        ("AIsVCP8", UCHAR),
+        ("BIsVCP8", UCHAR),
+        ("CIsVCP8", UCHAR),
+        ("DIsVCP8", UCHAR),
     ]
 
 
 PFT_PROGRAM_DATA = POINTER(ft_program_data)
 FT_PROGRAM_DATA = ft_program_data
 # ftd2xx.h 501
 FT_EE_Program = _libraries["ftd2xx.dll"].FT_EE_Program
```

### Comparing `ftd2xx-1.3.2/ftd2xx/_ftd2xx_darwin.py` & `ftd2xx-1.3.3/ftd2xx/_ftd2xx_darwin.py`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.2/ftd2xx/_ftd2xx_linux.py` & `ftd2xx-1.3.3/ftd2xx/_ftd2xx_linux.py`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.2/ftd2xx/aio/aio.py` & `ftd2xx-1.3.3/ftd2xx/aio/aio.py`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.2/ftd2xx/defines.py` & `ftd2xx-1.3.3/ftd2xx/defines.py`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.2/ftd2xx/ftd2xx.py` & `ftd2xx-1.3.3/ftd2xx/ftd2xx.py`

 * *Files 11% similar despite different names*

```diff
@@ -120,14 +120,59 @@
     InvertRI: Union[_ft.UCHAR, int]
     Cbus0: Union[_ft.UCHAR, int]
     Cbus1: Union[_ft.UCHAR, int]
     Cbus2: Union[_ft.UCHAR, int]
     Cbus3: Union[_ft.UCHAR, int]
     Cbus4: Union[_ft.UCHAR, int]
     RIsVCP: Union[_ft.UCHAR, int]
+    PullDownEnable7: Union[_ft.UCHAR, int]
+    SerNumEnable7: Union[_ft.UCHAR, int]
+    ALSlowSlew: Union[_ft.UCHAR, int]
+    ALSchmittInput: Union[_ft.UCHAR, int]
+    ALDriveCurrent: Union[_ft.UCHAR, int]
+    AHSlowSlew: Union[_ft.UCHAR, int]
+    AHSchmittInput: Union[_ft.UCHAR, int]
+    AHDriveCurrent: Union[_ft.UCHAR, int]
+    BLSlowSlew: Union[_ft.UCHAR, int]
+    BLSchmittInput: Union[_ft.UCHAR, int]
+    BLDriveCurrent: Union[_ft.UCHAR, int]
+    BHSlowSlew: Union[_ft.UCHAR, int]
+    BHSchmittInput: Union[_ft.UCHAR, int]
+    BHDriveCurrent: Union[_ft.UCHAR, int]
+    IFAIsFifo7: Union[_ft.UCHAR, int]
+    IFAIsFifoTar7: Union[_ft.UCHAR, int]
+    IFAIsFastSer7: Union[_ft.UCHAR, int]
+    AIsVCP7: Union[_ft.UCHAR, int]
+    IFBIsFifo7: Union[_ft.UCHAR, int]
+    IFBIsFifoTar7: Union[_ft.UCHAR, int]
+    IFBIsFastSer7: Union[_ft.UCHAR, int]
+    BIsVCP7: Union[_ft.UCHAR, int]
+    PowerSaveEnable: Union[_ft.UCHAR, int]
+    PullDownEnable8: Union[_ft.UCHAR, int]
+    SerNumEnable8: Union[_ft.UCHAR, int]
+    ASlowSlew: Union[_ft.UCHAR, int]
+    ASchmittInput: Union[_ft.UCHAR, int]
+    ADriveCurrent: Union[_ft.UCHAR, int]
+    BSlowSlew: Union[_ft.UCHAR, int]
+    BSchmittInput: Union[_ft.UCHAR, int]
+    BDriveCurrent: Union[_ft.UCHAR, int]
+    CSlowSlew: Union[_ft.UCHAR, int]
+    CSchmittInput: Union[_ft.UCHAR, int]
+    CDriveCurrent: Union[_ft.UCHAR, int]
+    DSlowSlew: Union[_ft.UCHAR, int]
+    DSchmittInput: Union[_ft.UCHAR, int]
+    DDriveCurrent: Union[_ft.UCHAR, int]
+    ARIIsTXDEN: Union[_ft.UCHAR, int]
+    BRIIsTXDEN: Union[_ft.UCHAR, int]
+    CRIIsTXDEN: Union[_ft.UCHAR, int]
+    DRIIsTXDEN: Union[_ft.UCHAR, int]
+    AIsVCP8: Union[_ft.UCHAR, int]
+    BIsVCP8: Union[_ft.UCHAR, int]
+    CIsVCP8: Union[_ft.UCHAR, int]
+    DIsVCP8: Union[_ft.UCHAR, int]
 
 
 def call_ft(function: Callable, *args):
     """Call an FTDI function and check the status. Raise exception on error"""
     status = function(*args)
     if status != defines.Status.OK:
         raise DeviceError(status)
@@ -549,15 +594,15 @@
         ManufacturerId = c.create_string_buffer(defines.MAX_DESCRIPTION_SIZE)
         Description = c.create_string_buffer(defines.MAX_DESCRIPTION_SIZE)
         SerialNumber = c.create_string_buffer(defines.MAX_DESCRIPTION_SIZE)
         progdata = ft_program_data(
             **ProgramData(
                 Signature1=0,
                 Signature2=0xFFFFFFFF,
-                Version=2,
+                Version=4,
                 Manufacturer=c.cast(Manufacturer, c.c_char_p),
                 ManufacturerId=c.cast(ManufacturerId, c.c_char_p),
                 Description=c.cast(Description, c.c_char_p),
                 SerialNumber=c.cast(SerialNumber, c.c_char_p),
             )
         )
```

### Comparing `ftd2xx-1.3.2/ftd2xx/tests/t_aio.py` & `ftd2xx-1.3.3/ftd2xx/tests/t_aio.py`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.2/ftd2xx/tests/t_ftd2xx.py` & `ftd2xx-1.3.3/ftd2xx/tests/t_ftd2xx.py`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.2/ftd2xx.egg-info/PKG-INFO` & `ftd2xx-1.3.3/ftd2xx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftd2xx
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python interface to ftd2xx.dll from FTDI using ctypesbased on d2xx by Pablo Bleyer
 Home-page: https://github.com/snmishra/ftd2xx
 Author: Satya Mishra
 Author-email: satya.devel@gmail.com
 License: MIT
 Keywords: ftd2xx d2xx ftdi
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ftd2xx-1.3.2/ftd2xx.egg-info/SOURCES.txt` & `ftd2xx-1.3.3/ftd2xx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.2/setup.cfg` & `ftd2xx-1.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.2/setup.py` & `ftd2xx-1.3.3/setup.py`

 * *Files identical despite different names*

