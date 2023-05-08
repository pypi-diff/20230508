# Comparing `tmp/pyldk-1.1.2-py3-none-win_amd64.whl.zip` & `tmp/pyldk-1.1.3-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3903268 bytes, number of entries: 9
--rw-r--r--  2.0 unx      245 b- defN 23-Mar-24 02:35 pyldk/__init__.py
--rw-r--r--  2.0 unx     4168 b- defN 23-Mar-24 02:35 pyldk/hasp_adapter.py
--rw-r--r--  2.0 unx     2480 b- defN 23-Mar-24 02:35 pyldk/pyldk.py
--rw-r--r--  2.0 unx       24 b- defN 23-Mar-24 02:35 pyldk/version.py
--rw-r--r--  2.0 unx  5899264 b- defN 23-Mar-24 02:35 pyldk/lib/Windows/x64/lib_hasp_adapter_x64.dll
--rw-r--r--  2.0 unx      513 b- defN 23-Mar-24 02:35 pyldk-1.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-24 02:35 pyldk-1.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       28 b- defN 23-Mar-24 02:35 pyldk-1.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      688 b- defN 23-Mar-24 02:35 pyldk-1.1.2.dist-info/RECORD
-9 files, 5907502 bytes uncompressed, 3902094 bytes compressed:  33.9%
+Zip file size: 3903314 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      245 b- defN 23-May-08 05:42 pyldk/__init__.py
+-rw-r--r--  2.0 unx     4344 b- defN 23-May-08 05:42 pyldk/hasp_adapter.py
+-rw-r--r--  2.0 unx     2480 b- defN 23-May-08 05:42 pyldk/pyldk.py
+-rw-r--r--  2.0 unx       24 b- defN 23-May-08 05:43 pyldk/version.py
+-rw-r--r--  2.0 unx  5899264 b- defN 23-May-08 05:42 pyldk/lib/Windows/x64/lib_hasp_adapter_x64.dll
+-rw-r--r--  2.0 unx      513 b- defN 23-May-08 05:43 pyldk-1.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-08 05:43 pyldk-1.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       28 b- defN 23-May-08 05:43 pyldk-1.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      688 b- defN 23-May-08 05:43 pyldk-1.1.3.dist-info/RECORD
+9 files, 5907678 bytes uncompressed, 3902140 bytes compressed:  34.0%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: pyldk/version.py
 Comment: 
 
 Filename: pyldk/lib/Windows/x64/lib_hasp_adapter_x64.dll
 Comment: 
 
-Filename: pyldk-1.1.2.dist-info/METADATA
+Filename: pyldk-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: pyldk-1.1.2.dist-info/WHEEL
+Filename: pyldk-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: pyldk-1.1.2.dist-info/top_level.txt
+Filename: pyldk-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pyldk-1.1.2.dist-info/RECORD
+Filename: pyldk-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyldk/hasp_adapter.py

```diff
@@ -50,17 +50,19 @@
                     self.log("获取加密狗ID失败,失败原因为:{}".format(e))
             else:
                 self.log("获取加密狗ID失败,失败代码为:{}".format(haspStruct.status))
         except Exception as e:
             self.log("获取加密狗ID列表失败,失败原因为:{}".format(e))
         return feature_id
 
-    def show_staus(self,operation_str,status):
+    def show_staus(self,operation_str,status,feature_id):
         if status == 7:
             self.log("{},请检查加密狗是否正常插入".format(operation_str))
+        elif status == 31:
+            self.log("{},没有找到该授权,请检查授权ID是否正确,授权ID为:{}".format(operation_str,feature_id))
         elif status == 38:
             self.log("{},请检查登录用户是否超出授权的最大用户数".format(operation_str))
         elif status == 42:
             self.log("{},当前加密狗驱动版本过低,请点击工具中并升级加密狗驱动".format(operation_str))
         elif status == 50:
             self.log("{},加密狗中途断开".format(operation_str))
         elif status == 84:
@@ -84,15 +86,15 @@
                         return True
                     else:
                         self.log("获取加密狗登录最大用户失败,失败原因为:当前用户登录数超过最大用户授权数")
                         return False
                 except Exception as e:
                     self.log("获取加密狗登录最大用户失败,失败原因为:{},info为:{}".format(e,str(haspStruct.info,encoding="utf-8")))
             else:
-                self.show_staus("获取加密狗登录最大用户失败",haspStruct.status)
+                self.show_staus("获取加密狗登录最大用户失败",haspStruct.status,feature_id)
         except Exception as e:
             self.log("获取是否超出加密狗登录最大用户失败,失败原因为:{}".format(e))
 
 
     def login(self,feature_id):
         self.lib.login.restype = HaspStruct
         haspStruct = self.lib.login(feature_id)
```

## pyldk/version.py

```diff
@@ -1 +1 @@
-full_version  = '1.1.2'
+full_version  = '1.1.3'
```

## Comparing `pyldk-1.1.2.dist-info/METADATA` & `pyldk-1.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyldk
-Version: 1.1.2
+Version: 1.1.3
 Summary: pyldk
 Home-page: https://jadehh@live.com
 Author: jade
 Author-email: jadehh@live.com
 License: MIT Licence
 Keywords: pip,pyldk,
 Platform: any
```

## Comparing `pyldk-1.1.2.dist-info/RECORD` & `pyldk-1.1.3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 pyldk/__init__.py,sha256=NV5NModdxHlMQ_yOO2fbeO89UuEmkSPQiRcukwU0Ssk,245
-pyldk/hasp_adapter.py,sha256=Cjhg1i_PSUxtJnX3s9OhM8tP3XJY5ZFtJ4s6cAvx4kI,4168
+pyldk/hasp_adapter.py,sha256=J7c2Gp2WJR9XFu8Et20DUzdFjCMzupJitXUTa7xcM00,4344
 pyldk/pyldk.py,sha256=RqvWKpz7saiawargmYj8pNvB4EA10jRfO8qNWv5V9jg,2480
-pyldk/version.py,sha256=u5O7BXI7YA9iK5nOqhOdECgKJh_yhKM4gj8ieviNjPw,24
+pyldk/version.py,sha256=hz3Ny2IvCMmbQLzTtalIp_fMWWjDEcqsBqTzsHzqzYQ,24
 pyldk/lib/Windows/x64/lib_hasp_adapter_x64.dll,sha256=5F5six-ErdDc9aQqld7LpQ7TlDhLD0C4uwZzLqQcRNA,5899264
-pyldk-1.1.2.dist-info/METADATA,sha256=PHYMLFgIeslOYgOR-C2wt1eHtKtsKfNCa4vj6XiyxdI,513
-pyldk-1.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyldk-1.1.2.dist-info/top_level.txt,sha256=1aCn7AVUNDZFl_MBhuhBcysO6UrkUlIsuKkrsE5eU6o,28
-pyldk-1.1.2.dist-info/RECORD,,
+pyldk-1.1.3.dist-info/METADATA,sha256=J3TYwct9ihpSMcaEseAgi49yAsEy_1nhq8lwYE60318,513
+pyldk-1.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyldk-1.1.3.dist-info/top_level.txt,sha256=1aCn7AVUNDZFl_MBhuhBcysO6UrkUlIsuKkrsE5eU6o,28
+pyldk-1.1.3.dist-info/RECORD,,
```

