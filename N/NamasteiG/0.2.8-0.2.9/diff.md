# Comparing `tmp/NamasteiG-0.2.8.tar.gz` & `tmp/NamasteiG-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NamasteiG-0.2.8.tar", last modified: Fri Apr 21 14:40:05 2023, max compression
+gzip compressed data, was "NamasteiG-0.2.9.tar", last modified: Mon May  8 08:02:45 2023, max compression
```

## Comparing `NamasteiG-0.2.8.tar` & `NamasteiG-0.2.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:40:05.473601 NamasteiG-0.2.8/
--rw-rw-rw-   0        0        0     1077 2022-12-10 14:24:59.000000 NamasteiG-0.2.8/LICENSE
--rw-rw-rw-   0        0        0      838 2023-04-21 14:40:05.473601 NamasteiG-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      326 2022-12-14 19:04:09.000000 NamasteiG-0.2.8/README.md
--rw-rw-rw-   0        0        0      593 2023-04-21 14:39:18.000000 NamasteiG-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 14:40:05.473601 NamasteiG-0.2.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 14:40:05.457568 NamasteiG-0.2.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 14:40:05.464595 NamasteiG-0.2.8/src/NamasteiG/
--rw-rw-rw-   0        0        0     8405 2023-04-16 13:01:55.000000 NamasteiG-0.2.8/src/NamasteiG/VerifyData.py
--rw-rw-rw-   0        0        0    27796 2023-04-21 14:39:18.000000 NamasteiG-0.2.8/src/NamasteiG/__init__.py
--rw-rw-rw-   0        0        0      501 2023-04-21 14:30:38.000000 NamasteiG-0.2.8/src/NamasteiG/example.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:40:05.464595 NamasteiG-0.2.8/src/NamasteiG.egg-info/
--rw-rw-rw-   0        0        0      838 2023-04-21 14:40:05.000000 NamasteiG-0.2.8/src/NamasteiG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-21 14:40:05.000000 NamasteiG-0.2.8/src/NamasteiG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:40:05.000000 NamasteiG-0.2.8/src/NamasteiG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-21 14:40:05.000000 NamasteiG-0.2.8/src/NamasteiG.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 08:02:45.598854 NamasteiG-0.2.9/
+-rw-rw-rw-   0        0        0     1077 2022-12-10 14:24:59.000000 NamasteiG-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0      838 2023-05-08 08:02:45.598854 NamasteiG-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2022-12-14 19:04:09.000000 NamasteiG-0.2.9/README.md
+-rw-rw-rw-   0        0        0      593 2023-05-08 07:59:00.000000 NamasteiG-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 08:02:45.599831 NamasteiG-0.2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 08:02:45.578437 NamasteiG-0.2.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 08:02:45.589321 NamasteiG-0.2.9/src/NamasteiG/
+-rw-rw-rw-   0        0        0     8405 2023-04-16 13:01:55.000000 NamasteiG-0.2.9/src/NamasteiG/VerifyData.py
+-rw-rw-rw-   0        0        0    27949 2023-05-08 07:58:45.000000 NamasteiG-0.2.9/src/NamasteiG/__init__.py
+-rw-rw-rw-   0        0        0      501 2023-04-21 14:30:38.000000 NamasteiG-0.2.9/src/NamasteiG/example.py
+drwxrwxrwx   0        0        0        0 2023-05-08 08:02:45.596832 NamasteiG-0.2.9/src/NamasteiG.egg-info/
+-rw-rw-rw-   0        0        0      838 2023-05-08 08:02:45.000000 NamasteiG-0.2.9/src/NamasteiG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-05-08 08:02:45.000000 NamasteiG-0.2.9/src/NamasteiG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 08:02:45.000000 NamasteiG-0.2.9/src/NamasteiG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-08 08:02:45.000000 NamasteiG-0.2.9/src/NamasteiG.egg-info/top_level.txt
```

### Comparing `NamasteiG-0.2.8/LICENSE` & `NamasteiG-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `NamasteiG-0.2.8/PKG-INFO` & `NamasteiG-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NamasteiG
-Version: 0.2.8
+Version: 0.2.9
 Summary: Most PowerFull Instagram Library
 Author-email: Abhinav Bhardwaj <abhinav.bhardwaj.56614@gmail.com>
 Project-URL: Homepage, https://t.me/namastelibrary
 Project-URL: Bug Tracker, https://t.me/namastehackers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NamasteiG-0.2.8/pyproject.toml` & `NamasteiG-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NamasteiG"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="Abhinav Bhardwaj", email="abhinav.bhardwaj.56614@gmail.com" },
 ]
 description = "Most PowerFull Instagram Library"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `NamasteiG-0.2.8/src/NamasteiG/VerifyData.py` & `NamasteiG-0.2.9/src/NamasteiG/VerifyData.py`

 * *Files identical despite different names*

### Comparing `NamasteiG-0.2.8/src/NamasteiG/__init__.py` & `NamasteiG-0.2.9/src/NamasteiG/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
+
+#Cyber Thodi Mhnt Khud Kr Le Kb TK Chori Krke Kmayega
+
 import uuid
 import string
 import random
 import secrets
 import requests
 import time
 from NamasteiG.VerifyData import IG_Verify
 from urllib.parse   import urlencode
 from Cryptodome.Cipher import AES, PKCS1_v1_5
 from Cryptodome.PublicKey import RSA
 from Cryptodome.Random import get_random_bytes
 import base64
 
-
-
-
 value=[]
 value1=[]
 
 def password_encrypt(password):
     resp = requests.get('https://i.instagram.com/api/v1/qe/sync/')
     publickeyid = int(resp.headers.get('ig-set-password-encryption-key-id'))
     publickey = resp.headers.get('ig-set-password-encryption-pub-key')
@@ -53,16 +53,16 @@
         self.PigeonSession = f'UFS-{str(uuid.uuid4())}-0'
         self.IgDeviceId = uuid.uuid4()
         self.IgFamilyDeviceId = uuid.uuid4()
         self.AndroidID = f'android-{secrets.token_hex(8)}'
         self.Waterfall= uuid.uuid4()
         self.Qpl=uuid.uuid4()
         rnd=str(random.randint(150, 999))
-        self.UserAgent = "Instagram 278.0.0.21.117 Android (" + ["23/6.0", "24/7.0", "25/7.1.1", "26/8.0", "27/8.1", "28/9.0"][random.randint(0, 5)] + "; " + str(random.randint(100, 1300)) + "dpi; " + str(random.randint(200, 2000)) + "x" + str(random.randint(200, 2000)) + "; " + ["SAMSUNG", "HUAWEI", "LGE/lge", "HTC", "ASUS", "ZTE", "ONEPLUS", "XIAOMI", "OPPO", "VIVO", "SONY", "REALME"][random.randint(0, 11)] + "; SM-T" + rnd + "; SM-T" + rnd + "; qcom; en_US; 464315254)"
-        self.Blockversion = '329007815be126bc02ffebcd41f0e4f8d889d871c12ca57fe5cbc3ece5196505'
+        self.UserAgent = "Instagram 281.0.0.19.105 Android (" + ["23/6.0", "24/7.0", "25/7.1.1", "26/8.0", "27/8.1", "28/9.0"][random.randint(0, 5)] + "; " + str(random.randint(100, 1300)) + "dpi; " + str(random.randint(200, 2000)) + "x" + str(random.randint(200, 2000)) + "; " + ["SAMSUNG", "HUAWEI", "LGE/lge", "HTC", "ASUS", "ZTE", "ONEPLUS", "XIAOMI", "OPPO", "VIVO", "SONY", "REALME"][random.randint(0, 11)] + "; SM-T" + rnd + "; SM-T" + rnd + "; qcom; en_US; 470774561)"
+        self.Blockversion = 'c0a45b461eed836c64d795e59fde36963cf2dd6a6d58c06a50d936bd9f62180d'
         self.proxy = Proxy
 
     def generate_jazoest(self,symbols):
         amount = sum(ord(s) for s in symbols)
         return f'2{amount}'
 
     def GetMid(self):
@@ -287,16 +287,17 @@
 
                     value = {
                         "Response": f"Login Error: An unexpected error occurred. Please try logging in again.",
                     }
                 elif 'Bearer IGT:2:' in  response.text:
 
 
+
                     self.bearer=response.text.split(r'\\\\\\\", \\\\\\\"IG-Set-Password-Encryption-Key-Id\\\\\\\": \\\\\\\"')[0].split('"Bearer IGT:2:')[1]
-                    self.csrf = response.text.split(r'csrftoken=')[1].split('; Domain=.instagram.com; expires=')[0]
+                    # self.csrf = response.text.split(r'csrftoken=')[1].split('; Domain=.instagram.com; expires=')[0]
                     self.rur = response.text.split(r'\\\\\\\", \\\\\\\"Cross-Origin-Embedder-Policy-Report-Only')[0].split(r'"ig-set-ig-u-rur\\\\\\\": \\\\\\\"')[1]
                     self.UserId = response.text.split(r', \\\\\\\"ig-set-ig-u-rur\\\\\\\"')[0].split(r'"ig-set-ig-u-ds-user-id\\\\\\\": ')[1]
 
                     self.xclaim,self.shbid,self.shbts,self.urur=IG_Verify.Dual_tokens2(self)
 
                     # value = {
                     #     "Response": 'Login Success',
@@ -373,16 +374,16 @@
                     "IgDeviceId": self.IgDeviceId,
                     "IgFamilyDeviceId": self.IgFamilyDeviceId,
                     "AndroidID": self.AndroidID,
                     'UserAgent': self.UserAgent,
                     'BlockVersion': self.Blockversion
                 }
                 return value
-            except Exception as E:
-                print(E)
+            except ConnectionError :
+                pass
     def head(self):
 
 
         headers = {
             'Host': 'i.instagram.com',
             'X-Ig-App-Locale': 'en_US',
             'X-Ig-Device-Locale': 'en_US',
@@ -578,11 +579,13 @@
 
 
 
 
 # if __name__ == '__main__':
 #     ig=Instagram('','')
 #     ig.LoginV2(1)
-#     print(ig.Scrape_Followers(''))
+    # print(ig.Scrape_Followers(''))
+
+#Yha Mt Dekh Khud Mhnt krke apna code likh mere shaare kb tk kmaayega mhnt kr na ki copy paste
```

### Comparing `NamasteiG-0.2.8/src/NamasteiG.egg-info/PKG-INFO` & `NamasteiG-0.2.9/src/NamasteiG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NamasteiG
-Version: 0.2.8
+Version: 0.2.9
 Summary: Most PowerFull Instagram Library
 Author-email: Abhinav Bhardwaj <abhinav.bhardwaj.56614@gmail.com>
 Project-URL: Homepage, https://t.me/namastelibrary
 Project-URL: Bug Tracker, https://t.me/namastehackers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

