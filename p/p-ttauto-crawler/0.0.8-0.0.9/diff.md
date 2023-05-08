# Comparing `tmp/p-ttauto-crawler-0.0.8.tar.gz` & `tmp/p-ttauto-crawler-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p-ttauto-crawler-0.0.8.tar", last modified: Mon Apr 17 03:39:14 2023, max compression
+gzip compressed data, was "p-ttauto-crawler-0.0.9.tar", last modified: Mon Apr 17 03:50:15 2023, max compression
```

## Comparing `p-ttauto-crawler-0.0.8.tar` & `p-ttauto-crawler-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 03:39:14.230369 p-ttauto-crawler-0.0.8/
--rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      397 2023-04-17 03:39:14.230369 p-ttauto-crawler-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 03:39:14.225368 p-ttauto-crawler-0.0.8/p_ttauto_crawler.egg-info/
--rw-rw-rw-   0        0        0      397 2023-04-17 03:39:14.000000 p-ttauto-crawler-0.0.8/p_ttauto_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-04-17 03:39:14.000000 p-ttauto-crawler-0.0.8/p_ttauto_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 03:39:14.000000 p-ttauto-crawler-0.0.8/p_ttauto_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-17 03:39:14.000000 p-ttauto-crawler-0.0.8/p_ttauto_crawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       63 2023-04-17 03:39:14.000000 p-ttauto-crawler-0.0.8/p_ttauto_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-17 03:39:14.000000 p-ttauto-crawler-0.0.8/p_ttauto_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 03:39:14.231369 p-ttauto-crawler-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      938 2023-04-17 03:38:05.000000 p-ttauto-crawler-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:39:14.228368 p-ttauto-crawler-0.0.8/ttauto_crawler/
--rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.8/ttauto_crawler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:39:14.229371 p-ttauto-crawler-0.0.8/ttauto_crawler/bin/
--rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.8/ttauto_crawler/bin/__init__.py
--rw-rw-rw-   0        0        0    16746 2023-04-17 03:39:11.000000 p-ttauto-crawler-0.0.8/ttauto_crawler/main.py
--rw-rw-rw-   0        0        0    10733 2023-04-17 03:37:59.000000 p-ttauto-crawler-0.0.8/ttauto_crawler/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:50:15.529398 p-ttauto-crawler-0.0.9/
+-rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      397 2023-04-17 03:50:15.528397 p-ttauto-crawler-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 03:50:15.524398 p-ttauto-crawler-0.0.9/p_ttauto_crawler.egg-info/
+-rw-rw-rw-   0        0        0      397 2023-04-17 03:50:15.000000 p-ttauto-crawler-0.0.9/p_ttauto_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-04-17 03:50:15.000000 p-ttauto-crawler-0.0.9/p_ttauto_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 03:50:15.000000 p-ttauto-crawler-0.0.9/p_ttauto_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-17 03:50:15.000000 p-ttauto-crawler-0.0.9/p_ttauto_crawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       63 2023-04-17 03:50:15.000000 p-ttauto-crawler-0.0.9/p_ttauto_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-17 03:50:15.000000 p-ttauto-crawler-0.0.9/p_ttauto_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 03:50:15.529398 p-ttauto-crawler-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      938 2023-04-17 03:49:54.000000 p-ttauto-crawler-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:50:15.526398 p-ttauto-crawler-0.0.9/ttauto_crawler/
+-rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.9/ttauto_crawler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:50:15.527398 p-ttauto-crawler-0.0.9/ttauto_crawler/bin/
+-rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.9/ttauto_crawler/bin/__init__.py
+-rw-rw-rw-   0        0        0    16773 2023-04-17 03:49:47.000000 p-ttauto-crawler-0.0.9/ttauto_crawler/main.py
+-rw-rw-rw-   0        0        0    10733 2023-04-17 03:37:59.000000 p-ttauto-crawler-0.0.9/ttauto_crawler/utils.py
```

### Comparing `p-ttauto-crawler-0.0.8/LICENSE` & `p-ttauto-crawler-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.0.8/setup.py` & `p-ttauto-crawler-0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="p-ttauto-crawler",
-    version="0.0.8",
+    version="0.0.9",
     author="pengjun",
     author_email="mr_lonely@foxmail.com",
     description="template tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `p-ttauto-crawler-0.0.8/ttauto_crawler/main.py` & `p-ttauto-crawler-0.0.9/ttauto_crawler/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,23 +244,23 @@
             zip1.write(filepath, writepath)
     zip1.close()
     shutil.copyfile(dist1, f"d://{curGroupId}_out.zip")
     os.remove(dist1)
 
 def process(url, crawler_template_name):
     global successCount
-    # ### downlaod
-    # print(f"=== downloading ")
-    # aaaapp(True, url, "", 0)
-    # ### process
-    # print(f"=== processing ")
-    # processAllVideo(crawler_template_name)
-    # cacheDir() #cache file to d://
-    # ### upload
-    # print(f"=== uploading ")
+    ### downlaod
+    print(f"=== downloading ")
+    aaaapp(True, url, "", 0)
+    ### process
+    print(f"=== processing ")
+    processAllVideo(crawler_template_name)
+    cacheDir() #cache file to d://
+    ### upload
+    print(f"=== uploading ")
     dist = os.path.join(os.path.dirname(curOutputDir()), f"{curGroupId}.zip")
     zip = zipfile.ZipFile(dist, "w", zipfile.ZIP_DEFLATED) 
     for rt,dirs,files in os.walk(curOutputDir()):
         for file in files:
             if str(file).startswith("~$"):
                 continue
             filepath = os.path.join(rt, file)
@@ -322,36 +322,35 @@
                         encoding="utf-8",
                         level=logging.DEBUG)
 
     rootDir = thisFileDir
     while(os.path.exists(os.path.join(thisFileDir, "stop.now")) == False):
         try:
             data = getTask()
-            if len(data) == 0:
-                continue
-            curGroupId = data["id"]
-            allCount = 0
-            successCount = 0
-            start_pts = calendar.timegm(time.gmtime())
-            logging.info(f"================ begin {curGroupId} ===================")
-            logging.info(f"========== GetTask: {data}")
-            print(f"=== begin {curGroupId}")
-            url = data["url"].replace("\n", "").replace(";", "").replace(",", "").strip()
-            crawler_template_name = data["crawler_template_name"].replace("\n", "").replace(";", "").replace(",", "").strip()
-            if len(crawler_template_name) <= 0:
-                crawler_template_name = "template2"
-
-            clearDir()
-            process(url, crawler_template_name)
-            removeLastTask()
-
-            current_pts = calendar.timegm(time.gmtime())
-            print(f"complate => {curGroupId} rst={successCount}/{allCount} duration={(current_pts - start_pts)}")
-            logging.info(f"================ end {curGroupId} rst={successCount}/{allCount} duration={(current_pts - start_pts)}===================")
-            exit(-1)
+            if len(data) > 0:
+                curGroupId = data["id"]
+                allCount = 0
+                successCount = 0
+                start_pts = calendar.timegm(time.gmtime())
+                logging.info(f"================ begin {curGroupId} ===================")
+                logging.info(f"========== GetTask: {data}")
+                print(f"=== begin {curGroupId}")
+                url = data["url"].replace("\n", "").replace(";", "").replace(",", "").strip()
+                crawler_template_name = data["crawler_template_name"].replace("\n", "").replace(";", "").replace(",", "").strip()
+                if len(crawler_template_name) <= 0:
+                    crawler_template_name = "template2"
+
+                clearDir()
+                process(url, crawler_template_name)
+                removeLastTask()
+
+                current_pts = calendar.timegm(time.gmtime())
+                print(f"complate => {curGroupId} rst={successCount}/{allCount} duration={(current_pts - start_pts)}")
+                logging.info(f"================ end {curGroupId} rst={successCount}/{allCount} duration={(current_pts - start_pts)}===================")
+                exit(-1)
         except Exception as e:
             notifyMessage(False, str(e))
             logging.error("====================== uncatch Exception ======================")
             logging.error(e)
             logging.error("======================      end      ======================")
         time.sleep(2)
     os.remove(os.path.join(thisFileDir, "stop.now"))
```

### Comparing `p-ttauto-crawler-0.0.8/ttauto_crawler/utils.py` & `p-ttauto-crawler-0.0.9/ttauto_crawler/utils.py`

 * *Files identical despite different names*

