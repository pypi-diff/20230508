# Comparing `tmp/intezer_sdk-1.9.3-py3-none-any.whl.zip` & `tmp/intezer_sdk-1.9.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 22983 bytes, number of entries: 17
--rw-r--r--  2.0 unx       22 b- defN 22-Jul-21 17:59 intezer_sdk/__init__.py
+Zip file size: 22990 bytes, number of entries: 17
+-rw-r--r--  2.0 unx       22 b- defN 22-Aug-03 08:34 intezer_sdk/__init__.py
 -rw-r--r--  2.0 unx      220 b- defN 22-Apr-19 13:22 intezer_sdk/_util.py
 -rw-r--r--  2.0 unx    10565 b- defN 22-Jul-21 17:55 intezer_sdk/analysis.py
 -rw-r--r--  2.0 unx    22834 b- defN 22-Jul-21 17:55 intezer_sdk/api.py
 -rw-r--r--  2.0 unx     4575 b- defN 22-Jul-21 17:55 intezer_sdk/base_analysis.py
 -rw-r--r--  2.0 unx     1023 b- defN 22-Jul-21 17:55 intezer_sdk/consts.py
 -rw-r--r--  2.0 unx     3190 b- defN 22-Jul-21 17:55 intezer_sdk/errors.py
 -rw-r--r--  2.0 unx     1169 b- defN 22-Mar-08 14:30 intezer_sdk/family.py
 -rw-r--r--  2.0 unx     3241 b- defN 22-Jul-21 17:55 intezer_sdk/index.py
 -rw-r--r--  2.0 unx     2139 b- defN 22-Jul-21 17:55 intezer_sdk/operation.py
 -rw-r--r--  2.0 unx     7387 b- defN 22-Jul-21 17:55 intezer_sdk/sub_analysis.py
--rw-r--r--  2.0 unx     8023 b- defN 22-Jul-21 17:59 intezer_sdk/util.py
--rw-r--r--  2.0 unx    11342 b- defN 22-Jul-21 18:05 intezer_sdk-1.9.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     6041 b- defN 22-Jul-21 18:05 intezer_sdk-1.9.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jul-21 18:05 intezer_sdk-1.9.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 22-Jul-21 18:05 intezer_sdk-1.9.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1355 b- defN 22-Jul-21 18:05 intezer_sdk-1.9.3.dist-info/RECORD
-17 files, 83230 bytes uncompressed, 20781 bytes compressed:  75.0%
+-rw-r--r--  2.0 unx     8083 b- defN 22-Aug-03 08:01 intezer_sdk/util.py
+-rw-r--r--  2.0 unx    11342 b- defN 22-Aug-03 08:38 intezer_sdk-1.9.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6041 b- defN 22-Aug-03 08:38 intezer_sdk-1.9.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Aug-03 08:38 intezer_sdk-1.9.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 22-Aug-03 08:38 intezer_sdk-1.9.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1355 b- defN 22-Aug-03 08:38 intezer_sdk-1.9.4.dist-info/RECORD
+17 files, 83290 bytes uncompressed, 20788 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: intezer_sdk/sub_analysis.py
 Comment: 
 
 Filename: intezer_sdk/util.py
 Comment: 
 
-Filename: intezer_sdk-1.9.3.dist-info/LICENSE
+Filename: intezer_sdk-1.9.4.dist-info/LICENSE
 Comment: 
 
-Filename: intezer_sdk-1.9.3.dist-info/METADATA
+Filename: intezer_sdk-1.9.4.dist-info/METADATA
 Comment: 
 
-Filename: intezer_sdk-1.9.3.dist-info/WHEEL
+Filename: intezer_sdk-1.9.4.dist-info/WHEEL
 Comment: 
 
-Filename: intezer_sdk-1.9.3.dist-info/top_level.txt
+Filename: intezer_sdk-1.9.4.dist-info/top_level.txt
 Comment: 
 
-Filename: intezer_sdk-1.9.3.dist-info/RECORD
+Filename: intezer_sdk-1.9.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## intezer_sdk/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '1.9.3'
+__version__ = '1.9.4'
```

## intezer_sdk/util.py

```diff
@@ -56,15 +56,15 @@
     if should_include_related_samples:
         related_samples = [sub_analysis.get_account_related_samples(wait=True) for sub_analysis in
                            analysis.get_sub_analyses()]
         if related_samples:
             related_samples_unique_count = len({analysis['analysis']['sha256'] for analysis in
                                                 itertools.chain.from_iterable(
                                                     sample.result['related_samples'] for sample in related_samples
-                                                    if sample is not None)})
+                                                    if sample is not None and sample.result is not None)})
 
     return {
         'verdict': verdict,
         'sub_verdict': sub_verdict,
         'analysis_url': analysis_url,
         'main_family': main_family,
         'gene_count': gene_count,
@@ -144,15 +144,15 @@
 
     related_samples = [sub_analysis.get_account_related_samples(wait=True) for sub_analysis in
                        analysis.get_sub_analyses()]
     if related_samples:
         related_samples_unique_count = len({analysis['analysis']['sha256'] for analysis in
                                             itertools.chain.from_iterable(
                                                 sample.result['related_samples'] for sample in related_samples
-                                                if sample is not None)})
+                                                if sample is not None and sample.result is not None)})
         note = f'{note}Similar previous uploads: {related_samples_unique_count} files \n'
 
     note = (f'{note}\nFull report:\n'
             f'{"" if no_emojis else get_emoji("result_url")} {analysis_url}')
 
     return note
```

## Comparing `intezer_sdk-1.9.3.dist-info/LICENSE` & `intezer_sdk-1.9.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `intezer_sdk-1.9.3.dist-info/METADATA` & `intezer_sdk-1.9.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intezer-sdk
-Version: 1.9.3
+Version: 1.9.4
 Summary: Intezer Analyze SDK
 Home-page: https://github.com/intezer/analyze-python-sdk
 Author: Intezer Labs ltd.
 Author-email: info@intezer.com
 License: Apache License v2
 Keywords: intezer
 Platform: UNKNOWN
```

## Comparing `intezer_sdk-1.9.3.dist-info/RECORD` & `intezer_sdk-1.9.4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-intezer_sdk/__init__.py,sha256=iI0hxhllIq2OFo5K7Cpr3ztPjrLq5Y_HGE-6ahdDftI,22
+intezer_sdk/__init__.py,sha256=TVQz9Y2Y5ZZsEAeUXaNdkqQorvWqEFZ5UjMCI8zp6qI,22
 intezer_sdk/_util.py,sha256=d4kOg7NuJufF9kIWdC86A5qR-Q05zVMP46R6BfWSl70,220
 intezer_sdk/analysis.py,sha256=aH-VzMD8vuBDozl9WYr9lJPeeeh1Y8bB6MHgKpJl5zo,10565
 intezer_sdk/api.py,sha256=uoED30ace5VHebUOneqKEYNilfqbFzmz2fFKcpqf6GM,22834
 intezer_sdk/base_analysis.py,sha256=zdxzmMEFTC_PaSe_-LwIxnf8j7bhZx03DI3R4-aNd98,4575
 intezer_sdk/consts.py,sha256=-xo1wAbhkKhn2FFcYXiSzS5xX2SRZ3SBfeskfhV6soY,1023
 intezer_sdk/errors.py,sha256=tqbqBwmAFrg3YcZrQvjdcQGAQ17ROM4byBjoGoqjMaw,3190
 intezer_sdk/family.py,sha256=qW38h0AxtI9Vq2V_-15dYqdv-RlTrM_DjZuU0RgXOZg,1169
 intezer_sdk/index.py,sha256=2bydck6RNqmrFHGuZeNRPgBaB1I87us-_06y2j_NoTI,3241
 intezer_sdk/operation.py,sha256=e831k4s-gGPEaTu_Srqh6mQWyQdjDS1x9A6OS7_DF2U,2139
 intezer_sdk/sub_analysis.py,sha256=awxtfJEHRazqki3MFFXsrN_JVQio9O6dohVxGf-VJlg,7387
-intezer_sdk/util.py,sha256=Up-40MEQNWgSWjyM3TvUzUJpiFivzR8omzWXreEQidk,8023
-intezer_sdk-1.9.3.dist-info/LICENSE,sha256=zkoT-O1fNgAmEJsUEadt8XjpzmPK7V3QK-j8WXHQsVg,11342
-intezer_sdk-1.9.3.dist-info/METADATA,sha256=ZURtI9oc7NbD8Zw8qvYz-FtXyrkkkJ_zmr91V2OgQIE,6041
-intezer_sdk-1.9.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-intezer_sdk-1.9.3.dist-info/top_level.txt,sha256=6PcpeAjiMudfr3Yg7WRYL66BfEBoH8ikU6JM6fUr39U,12
-intezer_sdk-1.9.3.dist-info/RECORD,,
+intezer_sdk/util.py,sha256=0fiAyV34O4buvx0jLolr8ZpLz2HYunOzWaIIhVe4-oI,8083
+intezer_sdk-1.9.4.dist-info/LICENSE,sha256=zkoT-O1fNgAmEJsUEadt8XjpzmPK7V3QK-j8WXHQsVg,11342
+intezer_sdk-1.9.4.dist-info/METADATA,sha256=i0u5HUoK2AF7oEZ6tOpMwOEEoaiHAh985dlWfnb_Exo,6041
+intezer_sdk-1.9.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+intezer_sdk-1.9.4.dist-info/top_level.txt,sha256=6PcpeAjiMudfr3Yg7WRYL66BfEBoH8ikU6JM6fUr39U,12
+intezer_sdk-1.9.4.dist-info/RECORD,,
```

