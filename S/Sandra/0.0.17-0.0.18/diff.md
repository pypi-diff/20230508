# Comparing `tmp/Sandra-0.0.17.tar.gz` & `tmp/Sandra-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sandra-0.0.17.tar", last modified: Thu May  4 09:54:23 2023, max compression
+gzip compressed data, was "Sandra-0.0.18.tar", last modified: Mon May  8 18:45:40 2023, max compression
```

## Comparing `Sandra-0.0.17.tar` & `Sandra-0.0.18.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 09:54:23.014542 Sandra-0.0.17/
--rw-rw-rw-   0        0        0     1080 2023-04-27 16:41:21.000000 Sandra-0.0.17/LICENSE
--rw-rw-rw-   0        0        0     4427 2023-05-04 09:54:23.014542 Sandra-0.0.17/PKG-INFO
--rw-rw-rw-   0        0        0     3684 2023-05-04 09:53:50.000000 Sandra-0.0.17/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 09:54:22.623147 Sandra-0.0.17/Sandra/
--rw-rw-rw-   0        0        0      133 2023-05-04 09:27:04.000000 Sandra-0.0.17/Sandra/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-05-04 08:39:19.000000 Sandra-0.0.17/Sandra/helpers.py
--rw-rw-rw-   0        0        0     2702 2023-05-04 09:36:56.000000 Sandra-0.0.17/Sandra/performance.py
--rw-rw-rw-   0        0        0     4954 2023-05-04 08:39:49.000000 Sandra-0.0.17/Sandra/sandra.py
--rw-rw-rw-   0        0        0     2095 2023-05-04 09:06:12.000000 Sandra-0.0.17/Sandra/troy.py
-drwxrwxrwx   0        0        0        0 2023-05-04 09:54:23.013549 Sandra-0.0.17/Sandra.egg-info/
--rw-rw-rw-   0        0        0     4427 2023-05-04 09:54:22.000000 Sandra-0.0.17/Sandra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-05-04 09:54:22.000000 Sandra-0.0.17/Sandra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 09:54:22.000000 Sandra-0.0.17/Sandra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-04 09:54:22.000000 Sandra-0.0.17/Sandra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-04 09:54:22.000000 Sandra-0.0.17/Sandra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 09:54:23.015542 Sandra-0.0.17/setup.cfg
--rw-rw-rw-   0        0        0     1284 2023-05-04 09:26:57.000000 Sandra-0.0.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 18:45:40.594226 Sandra-0.0.18/
+-rw-rw-rw-   0        0        0     1080 2023-04-27 16:41:21.000000 Sandra-0.0.18/LICENSE
+-rw-rw-rw-   0        0        0     4788 2023-05-08 18:45:40.593229 Sandra-0.0.18/PKG-INFO
+-rw-rw-rw-   0        0        0     4031 2023-05-08 16:41:47.000000 Sandra-0.0.18/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 18:45:40.567216 Sandra-0.0.18/Sandra/
+-rw-rw-rw-   0        0        0      133 2023-05-08 16:25:25.000000 Sandra-0.0.18/Sandra/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-05-04 08:39:19.000000 Sandra-0.0.18/Sandra/helpers.py
+-rw-rw-rw-   0        0        0     2971 2023-05-08 16:35:55.000000 Sandra-0.0.18/Sandra/performance.py
+-rw-rw-rw-   0        0        0     8543 2023-05-08 17:22:06.000000 Sandra-0.0.18/Sandra/sandra.py
+-rw-rw-rw-   0        0        0     2949 2023-05-08 17:23:49.000000 Sandra-0.0.18/Sandra/troy.py
+drwxrwxrwx   0        0        0        0 2023-05-08 18:45:40.592225 Sandra-0.0.18/Sandra.egg-info/
+-rw-rw-rw-   0        0        0     4788 2023-05-08 18:45:40.000000 Sandra-0.0.18/Sandra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-08 18:45:40.000000 Sandra-0.0.18/Sandra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 18:45:40.000000 Sandra-0.0.18/Sandra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-08 18:45:40.000000 Sandra-0.0.18/Sandra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 18:45:40.000000 Sandra-0.0.18/Sandra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 18:45:40.594226 Sandra-0.0.18/setup.cfg
+-rw-rw-rw-   0        0        0     1284 2023-05-08 16:25:20.000000 Sandra-0.0.18/setup.py
```

### Comparing `Sandra-0.0.17/LICENSE` & `Sandra-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `Sandra-0.0.17/PKG-INFO` & `Sandra-0.0.18/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sandra
-Version: 0.0.17
+Version: 0.0.18
 Summary: AES Stream Cipher with CFB and OpenPGP Modes
 Home-page: https://github.com/lopgogo/Sandra
 Author: George Assaad
 Author-email: <lopgogo@gmail.com>
 License: MIT
 Keywords: python,encryption,decryption,cipher,cryptography
 Classifier: Development Status :: 1 - Planning
@@ -39,22 +39,22 @@
 ```
 
 ## Examples
 ### RSA File Encryption 
 ```python
 import Sandra
 file_names, file_data = Sandra.load_data('./taylor_txt/taylor_swift_1KB.txt') 
-enc_dec_rsa = Sandra.RSA(256)
+enc_dec_rsa = Sandra.RSA(2048, Sandra.RSA_ENGINE_DOME)
 ciphertext = enc_dec_rsa.encrypt(file_data[0])
 print(len(ciphertext))
 plaintext = enc_dec_rsa.decrypt(ciphertext)
 print(plaintext == file_data[0])
 Sandra.write_data(
-    file_names, # name of file to be written
-    [plaintext], # data to be written, must be same length as file_names
+    file_names, # name of the file to be written
+    [plaintext], # data to be written, must be the same length as file_names
     path='./taylor_txt_ed' # path to write data to
 )
 ```
 
 ### AES CFB Mode Sample(NIST) Encryption
 ```python
 import Sandra
@@ -76,15 +76,15 @@
 file_names, file_data = Sandra.load_data('./taylor_txt/taylor_swift_1KB.txt') 
 enc_dec_cfb = Sandra.AES(key, Sandra.MODE_CFB, iv, segment_size=16)
 ciphertext = enc_dec_cfb.encrypt(file_data[0])
 print(len(ciphertext))
 plaintext = enc_dec_cfb.decrypt(ciphertext)
 print(plaintext == file_data[0])
 Sandra.write_data(
-    file_names, # name of file to be written
+    file_names, # name of the file to be written
     [plaintext], # data to be written, must be same length as file_names
     path='./taylor_txt_ed' # path to write data to
 )
 ```
 
 ### AES OpenPGP-CFB Mode File Encryption
 > In This mode, the first 18 bytes of cipher text contain the encrypted IV
@@ -103,21 +103,35 @@
 print(len(ciphertext))
 plaintext = enc_dec_pgp.decrypt(ciphertext)
 print(len(plaintext))
 plaintext = Sandra.unpad(plaintext,Sandra.AES_BLOCK_SIZE)
 print(len(plaintext))
 print(plaintext == file_data[0])
 Sandra.write_data(
-    file_names, # name of file to be written
-    [plaintext], # data to be written, must be same length as file_names
+    file_names, # name of the file to be written
+    [plaintext], # data to be written, must be the same length as file_names
     path='./taylor_txt_ed' # path to write data to
 )
 ```
 
 ## Performance
 To obtain a table like this one, run 
 ```python
 import Sandra
 file_names, file_data = Sandra.load_data('path/to/data')
-Sandra.performance_test(file_names, file_data)
+stats = Sandra.performance_test(
+    file_names, 
+    file_data, 
+    rsa_key_size=256,
+    rsa_engine=Sandra.RSA_ENGINE_RAW,
+    segment_size=64,  
+    verbose=True)
+
+stats = Sandra.performance_test(
+    file_names, 
+    file_data, 
+    rsa_key_size=256,
+    rsa_engine=Sandra.RSA_ENGINE_RAW,
+    segment_size=16,  
+    verbose=True)
 ```
-![image](https://user-images.githubusercontent.com/26662104/236169065-8fb0448c-1d7f-4a7c-89c4-7678ca33c57a.png)
+![image](https://user-images.githubusercontent.com/26662104/236880905-4862877c-1fec-4662-831a-a8cdd5781a2d.png)
```

### Comparing `Sandra-0.0.17/README.md` & `Sandra-0.0.18/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 ```
 
 ## Examples
 ### RSA File Encryption 
 ```python
 import Sandra
 file_names, file_data = Sandra.load_data('./taylor_txt/taylor_swift_1KB.txt') 
-enc_dec_rsa = Sandra.RSA(256)
+enc_dec_rsa = Sandra.RSA(2048, Sandra.RSA_ENGINE_DOME)
 ciphertext = enc_dec_rsa.encrypt(file_data[0])
 print(len(ciphertext))
 plaintext = enc_dec_rsa.decrypt(ciphertext)
 print(plaintext == file_data[0])
 Sandra.write_data(
-    file_names, # name of file to be written
-    [plaintext], # data to be written, must be same length as file_names
+    file_names, # name of the file to be written
+    [plaintext], # data to be written, must be the same length as file_names
     path='./taylor_txt_ed' # path to write data to
 )
 ```
 
 ### AES CFB Mode Sample(NIST) Encryption
 ```python
 import Sandra
@@ -57,15 +57,15 @@
 file_names, file_data = Sandra.load_data('./taylor_txt/taylor_swift_1KB.txt') 
 enc_dec_cfb = Sandra.AES(key, Sandra.MODE_CFB, iv, segment_size=16)
 ciphertext = enc_dec_cfb.encrypt(file_data[0])
 print(len(ciphertext))
 plaintext = enc_dec_cfb.decrypt(ciphertext)
 print(plaintext == file_data[0])
 Sandra.write_data(
-    file_names, # name of file to be written
+    file_names, # name of the file to be written
     [plaintext], # data to be written, must be same length as file_names
     path='./taylor_txt_ed' # path to write data to
 )
 ```
 
 ### AES OpenPGP-CFB Mode File Encryption
 > In This mode, the first 18 bytes of cipher text contain the encrypted IV
@@ -84,21 +84,35 @@
 print(len(ciphertext))
 plaintext = enc_dec_pgp.decrypt(ciphertext)
 print(len(plaintext))
 plaintext = Sandra.unpad(plaintext,Sandra.AES_BLOCK_SIZE)
 print(len(plaintext))
 print(plaintext == file_data[0])
 Sandra.write_data(
-    file_names, # name of file to be written
-    [plaintext], # data to be written, must be same length as file_names
+    file_names, # name of the file to be written
+    [plaintext], # data to be written, must be the same length as file_names
     path='./taylor_txt_ed' # path to write data to
 )
 ```
 
 ## Performance
 To obtain a table like this one, run 
 ```python
 import Sandra
 file_names, file_data = Sandra.load_data('path/to/data')
-Sandra.performance_test(file_names, file_data)
+stats = Sandra.performance_test(
+    file_names, 
+    file_data, 
+    rsa_key_size=256,
+    rsa_engine=Sandra.RSA_ENGINE_RAW,
+    segment_size=64,  
+    verbose=True)
+
+stats = Sandra.performance_test(
+    file_names, 
+    file_data, 
+    rsa_key_size=256,
+    rsa_engine=Sandra.RSA_ENGINE_RAW,
+    segment_size=16,  
+    verbose=True)
 ```
-![image](https://user-images.githubusercontent.com/26662104/236169065-8fb0448c-1d7f-4a7c-89c4-7678ca33c57a.png)
+![image](https://user-images.githubusercontent.com/26662104/236880905-4862877c-1fec-4662-831a-a8cdd5781a2d.png)
```

### Comparing `Sandra-0.0.17/Sandra/helpers.py` & `Sandra-0.0.18/Sandra/helpers.py`

 * *Files identical despite different names*

### Comparing `Sandra-0.0.17/Sandra/performance.py` & `Sandra-0.0.18/Sandra/performance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from Crypto.Cipher import AES 
 from . import sandra
 from . import troy
 
 import timeit
 import pandas as pd
 
-def performance_test(names, files_data, verbose=True):
+def performance_test(
+        names, 
+        files_data, 
+        rsa_key_size=2048, 
+        rsa_engine=troy.RSA_ENGINE_RAW,
+        segment_size=16,
+        verbose=True):
     files = dict(zip(names, files_data))
 
     iv   = bytes.fromhex('fffffe00000000000000000000000000')
     key  = bytes.fromhex('00000000000000000000000000000000')
 
     stats = dict()
 
@@ -33,43 +39,43 @@
             )
             stats[mode_name + '_dec'][filename] = t.timeit(n) / n
 
 
 
 
     # PyCrypto CFB
-    encryptor = AES.new(key, AES.MODE_CFB, iv, segment_size=16)
-    decryptor = AES.new(key, AES.MODE_CFB, iv, segment_size=16)
-    run_n_times('CFB', encryptor, decryptor, n=1000)
+    encryptor = AES.new(key, AES.MODE_CFB, iv, segment_size=segment_size)
+    decryptor = AES.new(key, AES.MODE_CFB, iv, segment_size=segment_size)
+    run_n_times(f'CFB_{segment_size}', encryptor, decryptor, n=1000)
     if verbose:
-        print(">> Finished running CFB 1000 times")
+        print(f">> Finished running CFB_{segment_size} 1000 times")
 
     # PyCrypto OPENPGP
     encryptor = AES.new(key, AES.MODE_OPENPGP, iv)
     decryptor = None
     run_n_times('OPENPGP',encryptor, decryptor, OPENPGP=1, n=1000)
     if verbose:
         print(">> Finished running OPENPGP 1000 times")
 
     # Sandra CFB
-    enc_dec_sandra = sandra.AES(key, sandra.MODE_CFB, iv)
-    run_n_times('CFB_SANDRA', enc_dec_sandra, enc_dec_sandra, OPENPGP=0, n=100)
+    enc_dec_sandra = sandra.AES(key, sandra.MODE_CFB, iv, segment_size)
+    run_n_times(f'CFB_SANDRA_{segment_size}', enc_dec_sandra, enc_dec_sandra, OPENPGP=0, n=100)
     if verbose:
-        print(">> Finished running CFB_SANDRA 100 times")
+        print(f">> Finished running CFB_SANDRA_{segment_size} 100 times")
 
     # Sandra OPENPGP
     enc_dec_sandra = sandra.AES(key, sandra.MODE_OPENPGP, iv)
     run_n_times('OPENPGP_SANDRA', enc_dec_sandra, enc_dec_sandra, OPENPGP=2, n=100)
     if verbose:
         print(">> Finished running OPENPGP_SANDRA 100 times")
 
     # Troy RSA (a wrapper around PyCrypto)
-    enc_dec_rsa = troy.RSA(256)
-    run_n_times('RSA_TROY_256', enc_dec_rsa, enc_dec_rsa, n=100)
+    enc_dec_rsa = troy.RSA(rsa_key_size, rsa_engine)
+    run_n_times(f'RSA_TROY_{rsa_key_size}', enc_dec_rsa, enc_dec_rsa, n=100)
     if verbose:
-        print(">> Finished running RSA_TROY_256 100 times")
+        print(f">> Finished running RSA_TROY_{rsa_key_size} 100 times")
 
         print("============================================= Results (seconds) ============================================")
         df = pd.DataFrame.from_dict(stats, orient='index')
         print(df.to_string())
         
     return stats
```

### Comparing `Sandra-0.0.17/Sandra.egg-info/PKG-INFO` & `Sandra-0.0.18/Sandra.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sandra
-Version: 0.0.17
+Version: 0.0.18
 Summary: AES Stream Cipher with CFB and OpenPGP Modes
 Home-page: https://github.com/lopgogo/Sandra
 Author: George Assaad
 Author-email: <lopgogo@gmail.com>
 License: MIT
 Keywords: python,encryption,decryption,cipher,cryptography
 Classifier: Development Status :: 1 - Planning
@@ -39,22 +39,22 @@
 ```
 
 ## Examples
 ### RSA File Encryption 
 ```python
 import Sandra
 file_names, file_data = Sandra.load_data('./taylor_txt/taylor_swift_1KB.txt') 
-enc_dec_rsa = Sandra.RSA(256)
+enc_dec_rsa = Sandra.RSA(2048, Sandra.RSA_ENGINE_DOME)
 ciphertext = enc_dec_rsa.encrypt(file_data[0])
 print(len(ciphertext))
 plaintext = enc_dec_rsa.decrypt(ciphertext)
 print(plaintext == file_data[0])
 Sandra.write_data(
-    file_names, # name of file to be written
-    [plaintext], # data to be written, must be same length as file_names
+    file_names, # name of the file to be written
+    [plaintext], # data to be written, must be the same length as file_names
     path='./taylor_txt_ed' # path to write data to
 )
 ```
 
 ### AES CFB Mode Sample(NIST) Encryption
 ```python
 import Sandra
@@ -76,15 +76,15 @@
 file_names, file_data = Sandra.load_data('./taylor_txt/taylor_swift_1KB.txt') 
 enc_dec_cfb = Sandra.AES(key, Sandra.MODE_CFB, iv, segment_size=16)
 ciphertext = enc_dec_cfb.encrypt(file_data[0])
 print(len(ciphertext))
 plaintext = enc_dec_cfb.decrypt(ciphertext)
 print(plaintext == file_data[0])
 Sandra.write_data(
-    file_names, # name of file to be written
+    file_names, # name of the file to be written
     [plaintext], # data to be written, must be same length as file_names
     path='./taylor_txt_ed' # path to write data to
 )
 ```
 
 ### AES OpenPGP-CFB Mode File Encryption
 > In This mode, the first 18 bytes of cipher text contain the encrypted IV
@@ -103,21 +103,35 @@
 print(len(ciphertext))
 plaintext = enc_dec_pgp.decrypt(ciphertext)
 print(len(plaintext))
 plaintext = Sandra.unpad(plaintext,Sandra.AES_BLOCK_SIZE)
 print(len(plaintext))
 print(plaintext == file_data[0])
 Sandra.write_data(
-    file_names, # name of file to be written
-    [plaintext], # data to be written, must be same length as file_names
+    file_names, # name of the file to be written
+    [plaintext], # data to be written, must be the same length as file_names
     path='./taylor_txt_ed' # path to write data to
 )
 ```
 
 ## Performance
 To obtain a table like this one, run 
 ```python
 import Sandra
 file_names, file_data = Sandra.load_data('path/to/data')
-Sandra.performance_test(file_names, file_data)
+stats = Sandra.performance_test(
+    file_names, 
+    file_data, 
+    rsa_key_size=256,
+    rsa_engine=Sandra.RSA_ENGINE_RAW,
+    segment_size=64,  
+    verbose=True)
+
+stats = Sandra.performance_test(
+    file_names, 
+    file_data, 
+    rsa_key_size=256,
+    rsa_engine=Sandra.RSA_ENGINE_RAW,
+    segment_size=16,  
+    verbose=True)
 ```
-![image](https://user-images.githubusercontent.com/26662104/236169065-8fb0448c-1d7f-4a7c-89c4-7678ca33c57a.png)
+![image](https://user-images.githubusercontent.com/26662104/236880905-4862877c-1fec-4662-831a-a8cdd5781a2d.png)
```

### Comparing `Sandra-0.0.17/setup.py` & `Sandra-0.0.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.17'
+VERSION = '0.0.18'
 DESCRIPTION = 'AES Stream Cipher with CFB and OpenPGP Modes'
 LONG_DESCRIPTION = 'A package that allows you to build encrypt variable sized files using AES as a stream cipher with CFB and OpenPGP modes'
 
 # Setting up
 setup(
     name="Sandra",
     version=VERSION,
```

