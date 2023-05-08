# Comparing `tmp/nexus_extensibility-2.0.0b8-py3-none-any.whl.zip` & `tmp/nexus_extensibility-2.0.0b9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8432 bytes, number of entries: 11
--rw-r--r--  2.0 unx      212 b- defN 23-Apr-24 12:59 nexus_extensibility/__init__.py
--rw-r--r--  2.0 unx    11964 b- defN 23-Apr-24 12:59 nexus_extensibility/_data_model.py
--rw-r--r--  2.0 unx      670 b- defN 23-Apr-24 12:59 nexus_extensibility/_data_model_extensions.py
--rw-r--r--  2.0 unx      377 b- defN 23-Apr-24 12:59 nexus_extensibility/_data_model_utilities.py
--rw-r--r--  2.0 unx     6990 b- defN 23-Apr-24 12:59 nexus_extensibility/_extensibility_data_source.py
--rw-r--r--  2.0 unx      786 b- defN 23-Apr-24 12:59 nexus_extensibility/_extensibility_utilities.py
--rw-r--r--  2.0 unx      107 b- defN 23-Apr-24 12:59 nexus_extensibility/_i_extension.py
--rw-r--r--  2.0 unx      790 b- defN 23-Apr-24 13:03 nexus_extensibility-2.0.0b8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 13:03 nexus_extensibility-2.0.0b8.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Apr-24 13:03 nexus_extensibility-2.0.0b8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1033 b- defN 23-Apr-24 13:03 nexus_extensibility-2.0.0b8.dist-info/RECORD
-11 files, 23041 bytes uncompressed, 6636 bytes compressed:  71.2%
+Zip file size: 8431 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      212 b- defN 23-Apr-25 12:02 nexus_extensibility/__init__.py
+-rw-r--r--  2.0 unx    11964 b- defN 23-Apr-25 12:02 nexus_extensibility/_data_model.py
+-rw-r--r--  2.0 unx      670 b- defN 23-Apr-25 12:02 nexus_extensibility/_data_model_extensions.py
+-rw-r--r--  2.0 unx      377 b- defN 23-Apr-25 12:02 nexus_extensibility/_data_model_utilities.py
+-rw-r--r--  2.0 unx     6990 b- defN 23-Apr-25 12:02 nexus_extensibility/_extensibility_data_source.py
+-rw-r--r--  2.0 unx      786 b- defN 23-Apr-25 12:02 nexus_extensibility/_extensibility_utilities.py
+-rw-r--r--  2.0 unx      107 b- defN 23-Apr-25 12:02 nexus_extensibility/_i_extension.py
+-rw-r--r--  2.0 unx      790 b- defN 23-Apr-25 12:07 nexus_extensibility-2.0.0b9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 12:07 nexus_extensibility-2.0.0b9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Apr-25 12:07 nexus_extensibility-2.0.0b9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1033 b- defN 23-Apr-25 12:07 nexus_extensibility-2.0.0b9.dist-info/RECORD
+11 files, 23041 bytes uncompressed, 6635 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: nexus_extensibility/_extensibility_utilities.py
 Comment: 
 
 Filename: nexus_extensibility/_i_extension.py
 Comment: 
 
-Filename: nexus_extensibility-2.0.0b8.dist-info/METADATA
+Filename: nexus_extensibility-2.0.0b9.dist-info/METADATA
 Comment: 
 
-Filename: nexus_extensibility-2.0.0b8.dist-info/WHEEL
+Filename: nexus_extensibility-2.0.0b9.dist-info/WHEEL
 Comment: 
 
-Filename: nexus_extensibility-2.0.0b8.dist-info/top_level.txt
+Filename: nexus_extensibility-2.0.0b9.dist-info/top_level.txt
 Comment: 
 
-Filename: nexus_extensibility-2.0.0b8.dist-info/RECORD
+Filename: nexus_extensibility-2.0.0b9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `nexus_extensibility-2.0.0b8.dist-info/METADATA` & `nexus_extensibility-2.0.0b9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-extensibility
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: Type definitions to implement data sources for the Nexus system.
 Home-page: https://github.com/malstroem-labs/nexus
 Author: https://github.com/malstroem-labs
 License: MIT
 Project-URL: Project, https://malstroem-labs.github.io/Nexus
 Project-URL: Repository, https://github.com/malstroem-labs/nexus
 Keywords: Nexus extensibility time-series data lake
```

## Comparing `nexus_extensibility-2.0.0b8.dist-info/RECORD` & `nexus_extensibility-2.0.0b9.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 nexus_extensibility/__init__.py,sha256=3NjQgmwGAfhEef3LmQaTBXE9CPORo5ea4xh38hkUQkA,212
 nexus_extensibility/_data_model.py,sha256=HBuH2ftXAq_a5pJWc5UtqbEEcQIVAolz3xLUYgAHyk0,11964
 nexus_extensibility/_data_model_extensions.py,sha256=iLSOVDKvVoorj2h0x_XHGhbKwd_NHtrURgS7aUVe8MI,670
 nexus_extensibility/_data_model_utilities.py,sha256=cb_uJD4CeYz1m7NEttQ7kR3nrcMjovJQCrSUchnglQE,377
 nexus_extensibility/_extensibility_data_source.py,sha256=eKN3tfab0VIYVr3Y58olhCNNRTj4lz3gt2keTaFLGpM,6990
 nexus_extensibility/_extensibility_utilities.py,sha256=hQFcY2joHt1goJSCvMfEW5cprN1I-B1-SihqYme8R1A,786
 nexus_extensibility/_i_extension.py,sha256=JiylZIbVEnKAZ8_4MAIjIVXNcfex76m_FTVOC1CoA2k,107
-nexus_extensibility-2.0.0b8.dist-info/METADATA,sha256=d0sG35QafdMdExRmPA6kRe_5bT6KcwlhTPAo-sZczBc,790
-nexus_extensibility-2.0.0b8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-nexus_extensibility-2.0.0b8.dist-info/top_level.txt,sha256=GTaw9wgS6EKrgO6FhJ3YZuMrkgoK7kP-hW9uybPDbyg,20
-nexus_extensibility-2.0.0b8.dist-info/RECORD,,
+nexus_extensibility-2.0.0b9.dist-info/METADATA,sha256=2GJHSs8-IaxyoeeZeCZ1v644eV0KMG23G52GEp9V8fY,790
+nexus_extensibility-2.0.0b9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+nexus_extensibility-2.0.0b9.dist-info/top_level.txt,sha256=GTaw9wgS6EKrgO6FhJ3YZuMrkgoK7kP-hW9uybPDbyg,20
+nexus_extensibility-2.0.0b9.dist-info/RECORD,,
```

