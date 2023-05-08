# Comparing `tmp/spacetool-1.0.5.tar.gz` & `tmp/spacetool-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetool-1.0.5.tar", last modified: Sat May  6 04:21:00 2023, max compression
+gzip compressed data, was "spacetool-1.0.6.tar", last modified: Mon May  8 05:46:09 2023, max compression
```

## Comparing `spacetool-1.0.5.tar` & `spacetool-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-06 04:21:00.781945 spacetool-1.0.5/
--rw-r--r--   0 leo        (501) staff       (20)     1068 2022-11-03 01:53:28.000000 spacetool-1.0.5/LICENSE
--rw-r--r--   0 leo        (501) staff       (20)      432 2023-05-06 04:21:00.781827 spacetool-1.0.5/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)      135 2023-04-10 02:45:30.000000 spacetool-1.0.5/README.md
--rw-r--r--   0 leo        (501) staff       (20)       38 2023-05-06 04:21:00.781988 spacetool-1.0.5/setup.cfg
--rw-r--r--   0 leo        (501) staff       (20)     2483 2023-05-06 04:20:50.000000 spacetool-1.0.5/setup.py
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-06 04:21:00.780620 spacetool-1.0.5/spacetool/
--rw-r--r--   0 leo        (501) staff       (20)        0 2022-11-03 01:53:28.000000 spacetool-1.0.5/spacetool/__init__.py
--rw-r--r--   0 leo        (501) staff       (20)        7 2022-11-08 03:02:34.000000 spacetool-1.0.5/spacetool/__version__.py
--rw-r--r--   0 leo        (501) staff       (20)    52360 2023-05-06 04:20:45.000000 spacetool-1.0.5/spacetool/main_tool.py
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-06 04:21:00.781656 spacetool-1.0.5/spacetool.egg-info/
--rw-r--r--   0 leo        (501) staff       (20)      432 2023-05-06 04:21:00.000000 spacetool-1.0.5/spacetool.egg-info/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)      260 2023-05-06 04:21:00.000000 spacetool-1.0.5/spacetool.egg-info/SOURCES.txt
--rw-r--r--   0 leo        (501) staff       (20)        1 2023-05-06 04:21:00.000000 spacetool-1.0.5/spacetool.egg-info/dependency_links.txt
--rw-r--r--   0 leo        (501) staff       (20)       27 2023-05-06 04:21:00.000000 spacetool-1.0.5/spacetool.egg-info/requires.txt
--rw-r--r--   0 leo        (501) staff       (20)       10 2023-05-06 04:21:00.000000 spacetool-1.0.5/spacetool.egg-info/top_level.txt
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-08 05:46:09.324808 spacetool-1.0.6/
+-rw-r--r--   0 leo        (501) staff       (20)     1068 2022-11-03 01:53:28.000000 spacetool-1.0.6/LICENSE
+-rw-r--r--   0 leo        (501) staff       (20)      432 2023-05-08 05:46:09.324664 spacetool-1.0.6/PKG-INFO
+-rw-r--r--   0 leo        (501) staff       (20)      135 2023-04-10 02:45:30.000000 spacetool-1.0.6/README.md
+-rw-r--r--   0 leo        (501) staff       (20)       38 2023-05-08 05:46:09.324855 spacetool-1.0.6/setup.cfg
+-rw-r--r--   0 leo        (501) staff       (20)     2484 2023-05-08 05:45:32.000000 spacetool-1.0.6/setup.py
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-08 05:46:09.323026 spacetool-1.0.6/spacetool/
+-rw-r--r--   0 leo        (501) staff       (20)        0 2022-11-03 01:53:28.000000 spacetool-1.0.6/spacetool/__init__.py
+-rw-r--r--   0 leo        (501) staff       (20)        7 2022-11-08 03:02:34.000000 spacetool-1.0.6/spacetool/__version__.py
+-rw-r--r--   0 leo        (501) staff       (20)    57255 2023-05-08 05:30:55.000000 spacetool-1.0.6/spacetool/main_tool.py
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-08 05:46:09.324450 spacetool-1.0.6/spacetool.egg-info/
+-rw-r--r--   0 leo        (501) staff       (20)      432 2023-05-08 05:46:09.000000 spacetool-1.0.6/spacetool.egg-info/PKG-INFO
+-rw-r--r--   0 leo        (501) staff       (20)      260 2023-05-08 05:46:09.000000 spacetool-1.0.6/spacetool.egg-info/SOURCES.txt
+-rw-r--r--   0 leo        (501) staff       (20)        1 2023-05-08 05:46:09.000000 spacetool-1.0.6/spacetool.egg-info/dependency_links.txt
+-rw-r--r--   0 leo        (501) staff       (20)       27 2023-05-08 05:46:09.000000 spacetool-1.0.6/spacetool.egg-info/requires.txt
+-rw-r--r--   0 leo        (501) staff       (20)       10 2023-05-08 05:46:09.000000 spacetool-1.0.6/spacetool.egg-info/top_level.txt
```

### Comparing `spacetool-1.0.5/LICENSE` & `spacetool-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spacetool-1.0.5/setup.py` & `spacetool-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 
 from setuptools import setup, find_packages
 
 setup(
     name="spacetool",
-    version="1.0.5",
+    version="1.0.6",
     description='space.top的数据管理工具',
     author="Leo Ni",
     author_email="nij6173@gmail.com",
     url='http://space.top/',
     packages=find_packages(),
     install_requires=["requests", "cos-python-sdk-v5"],
     python_requires=">=3.6,<3.11",
@@ -54,7 +54,8 @@
 # requires : 定义依赖哪些模块
 # provides : 定义可以为哪些模块提供依赖
 # data_files :指定其他的一些文件(如配置文件),规定了哪些文件被安装到哪些目录中。如果目录名是相对路径,则是相对于sys.prefix或sys.exec_prefix的路径。如果没有提供模板,会被添加到MANIFEST文件中。
 
 # python3 setup.py sdist
 # twine upload dist/*
 
+
```

### Comparing `spacetool-1.0.5/spacetool/main_tool.py` & `spacetool-1.0.6/spacetool/main_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 import hashlib
 from urllib import parse
 from datetime import datetime
 from qcloud_cos import CosConfig
 from qcloud_cos import CosS3Client
 from qcloud_cos import CosServiceError
+from qcloud_cos.cos_threadpool import SimpleThreadPool
 # from qcloud_cos import CosClientError
 # from sts.sts import Sts
 import sys
 # import json
 
 # 正常情况日志级别使用 INFO，需要定位时可以修改为 DEBUG，此时 SDK 会打印和服务端的通信信息
 logging.basicConfig(level=logging.INFO, stream=sys.stdout)
@@ -215,20 +216,22 @@
         elif car_p_encoding in self.error_car_p_ser_path:
             return False
         else:
             carparking_name = car_p_encoding.split("/")[0]
             unique_time_string = car_p_encoding.split("/")[1]
             try:
                 carparking_serial = self.get_car_parking_info(carparking_name)["data"]["carparking_serial"]  # get_car_parking_info: {'code': 4004, 'data': '', 'msg': '暂无此停车场信息录入'}
+                print(f"#### carparking_serial: {carparking_serial}  unique_time_string: {unique_time_string} #######")
                 collection_record_serial = self.get_carparking_collection_record_info(carparking_serial, unique_time_string)["data"]["collection_record_serial"]
-            except Exception:
-                logging.info("######error#######")
+            except Exception as e:
+                logging.info(f"######error: {e}#######")
                 logging.info(f"get_car_parking_info: {carparking_name} {self.get_car_parking_info(carparking_name)}")
+                logging.info(f"get_carparking_collection_record_info: {carparking_name} {self.get_carparking_collection_record_info(carparking_serial, unique_time_string)}")
                 self.error_car_p_ser_path[car_p_encoding] = {
-                    "carparking_name": carparking_name, 
+                    "carparking_name": carparking_name,
                     "unique_time_string": unique_time_string
                 }
                 return False
             self.car_p_ser_path[car_p_encoding] = {
                 "carparking_name": carparking_name,
                 "carparking_serial": carparking_serial,
                 "unique_time_string": unique_time_string,
@@ -290,16 +293,18 @@
                     full_f_name = os.path.join(root, file_name)
                     f.write(f"#line{num}: {full_f_name}\n")
                     if file_name.endswith("mp4"):
                         # 格式检查
                         if "1、Raw_Video" in full_f_name:
                             # 追势自有格式
                             carparking_name = full_f_name.split(os.path.sep)[-3]
-                            unique_time_string = file_name.split(".")[0]
+                            # unique_time_string = file_name.split(".")[0].replace("_", "-")
+                            unique_time_string = f"{file_name[:8]}-{file_name[9:11]}-{file_name[11:13]}-{file_name[13:15]}"
                             handle_path = os.path.sep.join(full_f_name.split(os.path.sep)[:-2])
+                            print(f"##### {carparking_name}/{unique_time_string}  {handle_path}")
                             self.set_car_p_ser_handle_path(f"{carparking_name}/{unique_time_string}", handle_type=1, handle_path=handle_path)
                         else:
                             # 追势自有格式错误
                             # todo log
                             f.write(f"#line{num}[WARNING]:{full_f_name}\n")
                             logging.warning(f"#line{num} {full_f_name}")  # 创建一条严重级别为WARNING的日志记录
                     elif file_name.endswith("avi"):
@@ -332,15 +337,19 @@
                 unique_time_string = tmp_car_p_ser["unique_time_string"]
                 handle_type = tmp_car_p_ser["handle_type"]
                 handle_path = tmp_car_p_ser["handle_path"]
                 if handle_type == 1:  # zhuishi
                     raw_video_path = os.path.join(handle_path, "1、Raw_Video")
                     for root, dirs, files in os.walk(raw_video_path, topdown=False):
                         for file_name in files:
-                            if file_name == f"{unique_time_string}.mp4":
+                            # _temp = unique_time_string.replace("-", "_")
+                            _temp_list = unique_time_string.split("-")
+                            _temp = f"{_temp_list[0]}_{_temp_list[1]}{_temp_list[2]}{_temp_list[3]}"
+                            # print(f"#### local_file_name {_temp}")
+                            if file_name == f"{_temp}.mp4":
                                 full_f_name = os.path.join(root, file_name)
                                 target_file_path_key = f"origin/{carparking_serial}-{collection_record_serial}/{carparking_serial}-{collection_record_serial}.mp4"
                                 # # smc_file
                                 # smc_file = self.try_get_smc(handle_path)
                                 self.common_handle_file(full_f_name, target_file_path_key, carparking_serial, collection_record_serial)
                                 handle_num += 1
                                 total_num += 1
@@ -948,14 +957,109 @@
                     'x-cos-security-token': self.token
                 },
                 # Headers={'x-cos-traffic-limit': '819200'},  # 预签名 URL 本身是不包含请求头部的，但请求头部会算入签名，那么使用 URL 时就必须携带请求头部，并且请求头部的值必须是这里指定的值
                 Expired=120  # 120秒后过期，过期时间请根据自身场景定义
             )
         return url
 
+    # 列出当前目录子节点，返回所有子节点信息
+    def listCurrentDir(self, prefix):
+        file_infos = []
+        sub_dirs = []
+        marker = ""
+        count = 1
+        delimiter = ""
+        while True:
+            response = self.client.list_objects(self.bucket_name, prefix, delimiter, marker)
+            # 调试输出
+            # json_object = json.dumps(response, indent=4)
+            # print(count, " =======================================")
+            # print(json_object)
+            count += 1
+
+            if "CommonPrefixes" in response:
+                common_prefixes = response.get("CommonPrefixes")
+                sub_dirs.extend(common_prefixes)
+
+            if "Contents" in response:
+                contents = response.get("Contents")
+                file_infos.extend(contents)
+
+            if "NextMarker" in response.keys():
+                marker = response["NextMarker"]
+            else:
+                break
+
+        # print("=======================================================")
+
+        # 如果 delimiter 设置为 "/"，则需要进行递归处理子目录，
+        # sorted(sub_dirs, key=lambda sub_dir: sub_dir["Prefix"])
+        # for sub_dir in sub_dirs:
+        #     print(sub_dir)
+        #     sub_dir_files = listCurrentDir(sub_dir["Prefix"])
+        #     file_infos.extend(sub_dir_files)
+
+        # print("=======================================================")
+
+        sorted(file_infos, key=lambda file_info: file_info["Key"])
+        # for file in file_infos:
+        #     print(file)
+        return file_infos
+
+    # 下载文件到本地目录，如果本地目录已经有同名文件则会被覆盖；
+    # 如果目录结构不存在，则会创建和对象存储一样的目录结构
+    def downLoadFiles(self, file_infos, localDir="./download/"):
+        pool = SimpleThreadPool()
+        for file in file_infos:
+            # 文件下载 获取文件到本地
+            file_cos_key = file["Key"]
+            localName = localDir + file_cos_key
+
+            # 如果本地目录结构不存在，递归创建
+            if not os.path.exists(os.path.dirname(localName)):
+                os.makedirs(os.path.dirname(localName))
+
+            # skip dir, no need to download it
+            if str(localName).endswith("/"):
+                continue
+
+            # 实际下载文件
+            # 使用线程池方式
+            pool.add_task(self.client.download_file, self.bucket_name, file_cos_key, localName)
+
+            # 简单下载方式
+            # response = client.get_object(
+            #     Bucket=test_bucket,
+            #     Key=file_cos_key,
+            # )
+            # response['Body'].get_stream_to_file(localName)
+
+        pool.wait_completion()
+        return None
+
+    # 功能封装，下载对象存储上面的一个目录到本地磁盘
+    def downLoadDirFromCos(self, prefix, localDir="./download/"):
+        global file_infos
+
+        try:
+            file_infos = self.listCurrentDir(prefix)
+        except CosServiceError as e:
+            print(e.get_origin_msg())
+            print(e.get_digest_msg())
+            print(e.get_status_code())
+            print(e.get_error_code())
+            print(e.get_error_msg())
+            print(e.get_resource_location())
+            print(e.get_trace_id())
+            print(e.get_request_id())
+
+        self.downLoadFiles(file_infos, localDir)
+        return None
+    # client.downLoadDirFromCos(start_prefix, localDir)
+
 
 """
 pip install spacetool, requests
 import sys,os,json
 pp2 = os.path.abspath(".")
 sys.path.append(pp2)
 
@@ -987,21 +1091,23 @@
 # 测试
 
 pip install spacetool, requests
 import sys,os,json
 pp2 = os.path.abspath(".")
 sys.path.append(pp2)
 
-import main_tool
+from spacetool import main_tool
 d = main_tool.DataTool(name="", code="", host="http://127.0.0.1:8000/")
 to_handle_dir = "/Users/leo/Documents/data/test数据格式样本/紫横家园东区"
+to_handle_dir = "/Users/leo/Documents/data/文洋大厦地下"
+to_handle_dir = "/Users/leo/Documents/data/wly/文洋大厦地下"
 car_p_ser_path = d.walk_dir(to_handle_dir)
 res = d.handle_local()
 
-import main_tool
+from spacetool import main_tool
 d = main_tool.DataTool(name="", code="", host="")
 f = "/Users/leo/Downloads/追势数据4号盘.txt"
 res = d.walk_log_file(f3)
 res2 = d.walk_log_and_upload_info(f3)
 
 f1 = "/Users/leo/Downloads/用所选项目新建的文件夹2/离线硬盘path地址/追势数据1号盘.txt"
 f2 = "/Users/leo/Downloads/用所选项目新建的文件夹2/离线硬盘path地址/追势数据2号盘.txt"
@@ -1009,14 +1115,27 @@
 
 f1 = "/var/www/data/追势数据1号盘.txt"
 f2 = "/var/www/data/追势数据2号盘.txt"
 f3 = "/var/www/data/追势数据3号盘.txt"
 
 """
 
+"""
+from spacetool import main_tool
+# 长期开发密钥
+secret_id = ""
+secret_key = ""
+region = ""
+bucket_name = ""
+if_ever = True
+token = None
+qcloud_handle_instance = main_tool.QCloudHandle(secret_id, secret_key, region, bucket_name, if_ever, token)
+qcloud_handle_instance.downLoadDirFromCos("data/", "/Users/leo/Downloads/未命名文件夹/")
+
+"""
 
 """
 qcloud 测试
 if __name__ == "__main__":
     # 进入异步任务队列
     # 申请临时密钥, 默认1800秒, 一个case一个密钥
     # 初始化qcloud_tool
@@ -1046,32 +1165,7 @@
     # signed_download_url = qcloud_handle_instance.gen_file_download_url("tmp/screenshot-20230324-151321.png")
     # print(f"#### signed_download_url: {signed_download_url}")
     # response = requests.get(signed_download_url)
     # print(response)
     res = qcloud_handle_instance.list_objects("tmp/")
     # print(f"---res: {res}")
 """
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
```

