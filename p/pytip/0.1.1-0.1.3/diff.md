# Comparing `tmp/pytip-0.1.1-py2.py3-none-any.whl.zip` & `tmp/pytip-0.1.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,19 @@
-Zip file size: 10643 bytes, number of entries: 14
--rw-rw-r--  2.0 unx      606 b- defN 23-Apr-09 03:58 pytip/__init__.py
+Zip file size: 18007 bytes, number of entries: 17
+-rw-rw-r--  2.0 unx      704 b- defN 23-May-08 03:40 pytip/__init__.py
+-rw-rw-r--  2.0 unx    42686 b- defN 23-Apr-16 06:56 pytip/data/browsers.json
 -rw-rw-r--  2.0 unx      389 b- defN 23-Apr-09 02:24 pytip/tools/__init__.py
 -rw-rw-r--  2.0 unx     3268 b- defN 23-Apr-09 01:31 pytip/tools/item.py
 -rw-rw-r--  2.0 unx      854 b- defN 23-Apr-09 01:59 pytip/tools/plot.py
 -rw-rw-r--  2.0 unx     1597 b- defN 23-Apr-09 10:43 pytip/tools/table.py
--rw-rw-r--  2.0 unx      423 b- defN 23-Apr-09 02:30 pytip/utils/__init__.py
--rw-rw-r--  2.0 unx     3831 b- defN 23-Apr-09 05:24 pytip/utils/celery.py
--rw-rw-r--  2.0 unx     2463 b- defN 23-Apr-02 07:57 pytip/utils/checker.py
--rw-rw-r--  2.0 unx     1292 b- defN 23-Apr-09 01:24 pytip/utils/deco.py
--rw-rw-r--  2.0 unx     2658 b- defN 23-Apr-09 03:49 pytip/utils/file.py
--rw-rw-r--  2.0 unx     1118 b- defN 23-Apr-09 10:45 pytip-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-09 10:45 pytip-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-Apr-09 10:45 pytip-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1058 b- defN 23-Apr-09 10:45 pytip-0.1.1.dist-info/RECORD
-14 files, 19673 bytes uncompressed, 8913 bytes compressed:  54.7%
+-rw-rw-r--  2.0 unx      423 b- defN 23-Apr-16 02:29 pytip/utils/__init__.py
+-rw-rw-r--  2.0 unx     3831 b- defN 23-Apr-16 07:13 pytip/utils/celery.py
+-rw-rw-r--  2.0 unx     2268 b- defN 23-May-08 03:48 pytip/utils/checker.py
+-rw-rw-r--  2.0 unx     1291 b- defN 23-Apr-17 02:26 pytip/utils/deco.py
+-rw-rw-r--  2.0 unx     2983 b- defN 23-Apr-16 07:13 pytip/utils/file.py
+-rw-rw-r--  2.0 unx     1255 b- defN 23-May-08 03:35 pytip/utils/func.py
+-rw-rw-r--  2.0 unx     1823 b- defN 23-Apr-16 08:49 pytip/utils/web.py
+-rw-rw-r--  2.0 unx     1081 b- defN 23-May-08 04:13 pytip-0.1.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-08 04:13 pytip-0.1.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-08 04:13 pytip-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1291 b- defN 23-May-08 04:13 pytip-0.1.3.dist-info/RECORD
+17 files, 65860 bytes uncompressed, 15927 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: pytip/__init__.py
 Comment: 
 
+Filename: pytip/data/browsers.json
+Comment: 
+
 Filename: pytip/tools/__init__.py
 Comment: 
 
 Filename: pytip/tools/item.py
 Comment: 
 
 Filename: pytip/tools/plot.py
@@ -24,20 +27,26 @@
 
 Filename: pytip/utils/deco.py
 Comment: 
 
 Filename: pytip/utils/file.py
 Comment: 
 
-Filename: pytip-0.1.1.dist-info/METADATA
+Filename: pytip/utils/func.py
+Comment: 
+
+Filename: pytip/utils/web.py
+Comment: 
+
+Filename: pytip-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: pytip-0.1.1.dist-info/WHEEL
+Filename: pytip-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: pytip-0.1.1.dist-info/top_level.txt
+Filename: pytip-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pytip-0.1.1.dist-info/RECORD
+Filename: pytip-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytip/__init__.py

```diff
@@ -3,14 +3,20 @@
 # `tool` is A mechanical device intended to make a task easier.
 
 # utility : 독립적 프로그램
 # tools   : 부가적
 
 from .utils.celery import Celery
 from .utils.checker import Message, check_folder_file, check_ip
-from .utils.file import multiprocess_items, file_download, file_pickle
 from .utils.deco import web_retries, elapsed_time
+from .utils.web import FakeAgent
+from .utils.func import progressBar
+from .utils.file import (
+    multiprocess_items, file_download, file_pickle, print_error
+)
 
-from .tools.item import date_to_string, string_to_datetime, divide_chunks
 from .tools.plot import plt_ko
 from .tools.table import df_number_column
+from .tools.item import (
+    date_to_string, string_to_datetime, divide_chunks
+)
```

## pytip/utils/checker.py

```diff
@@ -1,31 +1,27 @@
 import os
+import json
 import datetime
 import termcolor
 import http.client as httplib
 from urllib import request
 
 
-def check_ip(url="www.google.com", timeout=3):
+def check_ip(url="http://ip.jsontest.com"):
 
     r"""인터넷 접속확인
     :: return :: True / False"""
-
-    conn = httplib.HTTPConnection(url, timeout=timeout)
+    response = request.urlopen(url).read()
     try:
-        conn.request("HEAD", "/")
-        conn.close()
-        # ip 접속정보 확인
-        fqn = os.uname()[1]
-        ext_ip = request.urlopen('https://api.ipify.org/').read()
-        print ("User: %s " % fqn, "\nIP #: %s " % ext_ip)
-        return True
+        response = json.loads(response)
+        return response['ip']
     except Exception as E:
         print(termcolor.colored(E, 'red'))
-        return False
+        return None
+
 
 # Cache file Check 함수
 def check_folder_file(file:str=None, folder:str=None):
     r"""파일과 폴더 존재여부 확인 (폴더가 없으면 해당 폴더를 생성)
     file (str) : 파일이름
     folder (str) : 폴더명
     :: return :: Boolean, file_path"""
```

## pytip/utils/deco.py

```diff
@@ -18,15 +18,14 @@
             print(f"{function.__name__} : {second} sec")
         else:
             print(f"{function.__name__} : {minute} min {second} sec")
 
         return result
     return wrapper
 
-
 # 웹 크롤링 실패시 반복실행
 def web_retries(number_retries = 3):
 
     def decorator(function):
         @wraps(function)
         def wrapper(*args, **kwargs):
             for _ in range(number_retries):
```

## pytip/utils/file.py

```diff
@@ -1,16 +1,18 @@
 import os
 import json
 import socket
+import subprocess
+from urllib import request
 import pickle
 import requests
-import subprocess
+import termcolor
 from tqdm import tqdm
-from urllib import request
 from multiprocessing import Pool
+from functools import wraps
 
 
 def multiprocess_items(funcion, items:int, worker:list, display=False):
     r"""list() 데이터를  function 에 multiprocessing 반복적용
     function : 반복적용할 함수
     items    : function 에 입력할 데이터"""
 
@@ -78,7 +80,18 @@
         r.raise_for_status()
         with open(file_path, 'wb') as f:
             for chunk in r.iter_content(chunk_size=chunk_size):
                 f.write(chunk)
     print(f'{file_path} downloading is done.')
     return file_path
 
+
+# Error Check
+def print_error(function):
+    @wraps(function)
+    def wrapper(*args, **kwargs):
+        try:
+            result = function(*args, **kwargs)
+            return result
+        except Exception as E:
+            print(termcolor.colored(E, 'red'))
+    return wrapper
```

## Comparing `pytip-0.1.1.dist-info/METADATA` & `pytip-0.1.3.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pytip
-Version: 0.1.1
-Summary: UNKNOWN
+Version: 0.1.3
 Home-page: https://github.com/YongBeomKim/pytip
 Author: momukji lab
 Author-email: ybkim@momukji.com
 License: MIT
 Keywords: pytip
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib
 Requires-Dist: termcolor
@@ -30,9 +28,7 @@
 Based on : https://github.com/YongBeomKim/pytip
 ```bash
 	$ pip install pytip
 	$ pip install -i https://pypi.python.org/pytip pytip
 ```
 
 © 2023 GitHub : https://github.com/YongBeomKim
-
-
```

## Comparing `pytip-0.1.1.dist-info/RECORD` & `pytip-0.1.3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-pytip/__init__.py,sha256=YQGvcoSAR1GVhIIfdyk1GkaRZ2ds7SpV9W4OF7sXrxs,606
+pytip/__init__.py,sha256=AUkdQEMPxCJnJ_SXc5bAmj96UBQeiJZ_-Qn3W6_3Ruw,704
+pytip/data/browsers.json,sha256=fgvByElwtpg9QpigM0ss-Rpjnc_Uql4-3y0gJDB7dVI,42686
 pytip/tools/__init__.py,sha256=KKqbkgk5EkEh_2jwQdxUtXATP6peuk43t9zGBN0lQE8,389
 pytip/tools/item.py,sha256=JPF-meLFzP1iwam3jDqeQrPGGfY4fFFYd67jtIfX674,3268
 pytip/tools/plot.py,sha256=2pmcMkz5HZ5fD5A5OgPr1_Cs2nTZP1DMcuqSyiSMCZk,854
 pytip/tools/table.py,sha256=ddAvODKP7SExPgeEBmeW4QCcZXkDi-aaM3saxqw6vDo,1597
 pytip/utils/__init__.py,sha256=ptGGMFwDewyV4fCaRR3BSwZIGAlug5Z_8xs-scpEDYk,423
 pytip/utils/celery.py,sha256=dEPGQtdQjixd6bL1vuCPkZjZA80-1l1yPSWnu4tpab0,3831
-pytip/utils/checker.py,sha256=dKi5FJhpCpxIakfdrnRMcdhjWsN_MfejuUhfk8Wq4jI,2463
-pytip/utils/deco.py,sha256=lGPcGmr0n_8uMi3dCoiHCUkfNzg5BJN3DReP2lTrIxA,1292
-pytip/utils/file.py,sha256=B8CSuXPFj61WBg9w4cm-g6cT-eIWQrmxSo_8Lwbj6VM,2658
-pytip-0.1.1.dist-info/METADATA,sha256=YFx50433ncwr5rOa1NiJ6M9dqPhCTtFtDHFaJfbnLmQ,1118
-pytip-0.1.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-pytip-0.1.1.dist-info/top_level.txt,sha256=jF2tKdrfqmRq7kr--QAKzT5DpQOqrfwdSBO9WrauNHE,6
-pytip-0.1.1.dist-info/RECORD,,
+pytip/utils/checker.py,sha256=VR08MkfhL_rhBll-92c1Xo28yaf4tWRfyBJUQlx2axU,2268
+pytip/utils/deco.py,sha256=BmidVhyoZbLKuziGamyA1TSOBGaU2xZy-ijUn6cAJ3g,1291
+pytip/utils/file.py,sha256=vFbfmPdM7-Fr-8SiJoQWeeu-4LTxCMjgYk4ftauMPBY,2983
+pytip/utils/func.py,sha256=fR_GQcYHMtYb0OC98zQ0i9AMVZqGgS3LJUoJZmjuWI0,1255
+pytip/utils/web.py,sha256=lyR6e7iyDIsSCPovTMmbSm8zu1AHEBEk35adIxYklZo,1823
+pytip-0.1.3.dist-info/METADATA,sha256=jy3M1bZg5H8Te02Q5TOHjtI8KNFSjs7r4rbGqaGJuiU,1081
+pytip-0.1.3.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+pytip-0.1.3.dist-info/top_level.txt,sha256=jF2tKdrfqmRq7kr--QAKzT5DpQOqrfwdSBO9WrauNHE,6
+pytip-0.1.3.dist-info/RECORD,,
```

