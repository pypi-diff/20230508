# Comparing `tmp/m_scheduler_partitioning-0.1.7.tar.gz` & `tmp/m_scheduler_partitioning-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m_scheduler_partitioning-0.1.7.tar", last modified: Thu Mar 30 10:21:05 2023, max compression
+gzip compressed data, was "m_scheduler_partitioning-0.1.8.tar", last modified: Mon May  8 04:59:24 2023, max compression
```

## Comparing `m_scheduler_partitioning-0.1.7.tar` & `m_scheduler_partitioning-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:21:05.925191 m_scheduler_partitioning-0.1.7/
--rw-r--r--   0 root         (0) root         (0)     3153 2023-03-30 10:21:05.924191 m_scheduler_partitioning-0.1.7/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     1882 2023-03-30 10:03:52.000000 m_scheduler_partitioning-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:21:05.919191 m_scheduler_partitioning-0.1.7/m_scheduler_partitioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3153 2023-03-30 10:21:05.000000 m_scheduler_partitioning-0.1.7/m_scheduler_partitioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      728 2023-03-30 10:21:05.000000 m_scheduler_partitioning-0.1.7/m_scheduler_partitioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 10:21:05.000000 m_scheduler_partitioning-0.1.7/m_scheduler_partitioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-30 10:21:05.000000 m_scheduler_partitioning-0.1.7/m_scheduler_partitioning.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-03-30 10:21:05.000000 m_scheduler_partitioning-0.1.7/m_scheduler_partitioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-30 10:21:05.000000 m_scheduler_partitioning-0.1.7/m_scheduler_partitioning.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:21:05.914191 m_scheduler_partitioning-0.1.7/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:21:05.920191 m_scheduler_partitioning-0.1.7/mobio/libs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 10:03:52.000000 m_scheduler_partitioning-0.1.7/mobio/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:21:05.921191 m_scheduler_partitioning-0.1.7/mobio/libs/m_scheduler_partitioning/
--rw-r--r--   0 root         (0) root         (0)      142 2023-03-30 10:03:52.000000 m_scheduler_partitioning-0.1.7/mobio/libs/m_scheduler_partitioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10727 2023-03-30 10:03:52.000000 m_scheduler_partitioning-0.1.7/mobio/libs/m_scheduler_partitioning/m_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:21:05.923191 m_scheduler_partitioning-0.1.7/mobio/libs/m_scheduler_partitioning/scheduler_models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 10:03:52.000000 m_scheduler_partitioning-0.1.7/mobio/libs/m_scheduler_partitioning/scheduler_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-03-30 10:03:52.000000 m_scheduler_partitioning-0.1.7/mobio/libs/m_scheduler_partitioning/scheduler_models/base_model.py
--rw-r--r--   0 root         (0) root         (0)      887 2023-03-30 10:03:52.000000 m_scheduler_partitioning-0.1.7/mobio/libs/m_scheduler_partitioning/scheduler_models/db_manager.py
--rw-r--r--   0 root         (0) root         (0)     3081 2023-03-30 10:03:52.000000 m_scheduler_partitioning-0.1.7/mobio/libs/m_scheduler_partitioning/scheduler_models/scheduler_state_model.py
--rw-r--r--   0 root         (0) root         (0)      103 2023-03-30 10:03:52.000000 m_scheduler_partitioning-0.1.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-30 10:21:05.925191 m_scheduler_partitioning-0.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9269 2023-03-30 10:21:05.000000 m_scheduler_partitioning-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:59:24.074867 m_scheduler_partitioning-0.1.8/
+-rw-r--r--   0 root         (0) root         (0)     3441 2023-05-08 04:59:24.073867 m_scheduler_partitioning-0.1.8/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     2122 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:59:24.066867 m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3441 2023-05-08 04:59:23.000000 m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      728 2023-05-08 04:59:23.000000 m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 04:59:23.000000 m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-08 04:59:23.000000 m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-08 04:59:23.000000 m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-08 04:59:23.000000 m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:59:24.059867 m_scheduler_partitioning-0.1.8/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:59:24.067867 m_scheduler_partitioning-0.1.8/mobio/libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/mobio/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:59:24.069867 m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/
+-rw-r--r--   0 root         (0) root         (0)      142 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10956 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/m_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:59:24.072867 m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/scheduler_models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/scheduler_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/scheduler_models/base_model.py
+-rw-r--r--   0 root         (0) root         (0)      887 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/scheduler_models/db_manager.py
+-rw-r--r--   0 root         (0) root         (0)     3081 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/scheduler_models/scheduler_state_model.py
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 04:59:24.074867 m_scheduler_partitioning-0.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9269 2023-05-08 04:59:23.000000 m_scheduler_partitioning-0.1.8/setup.py
```

### Comparing `m_scheduler_partitioning-0.1.7/PKG-INFO` & `m_scheduler_partitioning-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m_scheduler_partitioning
-Version: 0.1.7
+Version: 0.1.8
 Summary: Mobio scheduler partitioning libs
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: Thư viện scheduler multiple partitions của Profiling
@@ -26,15 +26,15 @@
                     SchedulerStateModel(self.url_connection).set_busy(
                         worker_id=self.node_id
                     )
                 print("Hi there ! :)")
         
         
         if __name__ == "__main__":
-            SampleScheduler(root_node="test-scheduler", nop=100, delays=1, url_connection="mongodb://test_user:test_password@0.0.0.0:27017/test_db")
+            SampleScheduler(root_node="test-scheduler", nop=100, delays=1, url_connection="mongodb://test_user:test_password@0.0.0.0:27017/test_db", zookeeper_uri="127.0.0.1:2181")
         
         ```
         # Change logs
         * 0.1.2
           * log state of worker
           * get free worker
           * Để không bị mất 50k cho anh Lợi, thêm 2 index này:
@@ -50,16 +50,22 @@
           * cơ chế đảm bảo việc register worker với hệ thống csdl
         * 0.1.5
           * Refix issue register worker
           * Thử nghiệm cơ chế đảm bảo 1 partition chỉ nằm trên 1 worker. 
           * *NOTE*: phần này chưa đảm bảo được việc đủ partitions trên các workers
         
         * 0.1.6
+          * missing version do nâng cấp CICD
+        
+        * 0.1.7
           * Sử dụng threading để quản lý heart_beat và expiry_time
           * Kiểm tra trạng thái subscribe của worker mỗi khi chuẩn bị process data (Đảm bảo rằng việc subscribe phải diễn ra thành công tránh 2 worker cùng xử lý 1 partition)
+        
+        * 0.1.8
+          * Cho phép truyền zookeeper_uri vào param khi khởi tạo Schedule, nếu không truyền thì lấy mặc định từ ENV: ZOOKEEPER_CLUSTER
 Keywords: mobio,scheduler,partitioning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `m_scheduler_partitioning-0.1.7/README.md` & `m_scheduler_partitioning-0.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             SchedulerStateModel(self.url_connection).set_busy(
                 worker_id=self.node_id
             )
         print("Hi there ! :)")
 
 
 if __name__ == "__main__":
-    SampleScheduler(root_node="test-scheduler", nop=100, delays=1, url_connection="mongodb://test_user:test_password@0.0.0.0:27017/test_db")
+    SampleScheduler(root_node="test-scheduler", nop=100, delays=1, url_connection="mongodb://test_user:test_password@0.0.0.0:27017/test_db", zookeeper_uri="127.0.0.1:2181")
 
 ```
 # Change logs
 * 0.1.2
   * log state of worker
   * get free worker
   * Để không bị mất 50k cho anh Lợi, thêm 2 index này:
@@ -41,9 +41,15 @@
   * cơ chế đảm bảo việc register worker với hệ thống csdl
 * 0.1.5
   * Refix issue register worker
   * Thử nghiệm cơ chế đảm bảo 1 partition chỉ nằm trên 1 worker. 
   * *NOTE*: phần này chưa đảm bảo được việc đủ partitions trên các workers
 
 * 0.1.6
+  * missing version do nâng cấp CICD
+
+* 0.1.7
   * Sử dụng threading để quản lý heart_beat và expiry_time
-  * Kiểm tra trạng thái subscribe của worker mỗi khi chuẩn bị process data (Đảm bảo rằng việc subscribe phải diễn ra thành công tránh 2 worker cùng xử lý 1 partition)
+  * Kiểm tra trạng thái subscribe của worker mỗi khi chuẩn bị process data (Đảm bảo rằng việc subscribe phải diễn ra thành công tránh 2 worker cùng xử lý 1 partition)
+
+* 0.1.8
+  * Cho phép truyền zookeeper_uri vào param khi khởi tạo Schedule, nếu không truyền thì lấy mặc định từ ENV: ZOOKEEPER_CLUSTER
```

### Comparing `m_scheduler_partitioning-0.1.7/m_scheduler_partitioning.egg-info/PKG-INFO` & `m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-scheduler-partitioning
-Version: 0.1.7
+Version: 0.1.8
 Summary: Mobio scheduler partitioning libs
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: Thư viện scheduler multiple partitions của Profiling
@@ -26,15 +26,15 @@
                     SchedulerStateModel(self.url_connection).set_busy(
                         worker_id=self.node_id
                     )
                 print("Hi there ! :)")
         
         
         if __name__ == "__main__":
-            SampleScheduler(root_node="test-scheduler", nop=100, delays=1, url_connection="mongodb://test_user:test_password@0.0.0.0:27017/test_db")
+            SampleScheduler(root_node="test-scheduler", nop=100, delays=1, url_connection="mongodb://test_user:test_password@0.0.0.0:27017/test_db", zookeeper_uri="127.0.0.1:2181")
         
         ```
         # Change logs
         * 0.1.2
           * log state of worker
           * get free worker
           * Để không bị mất 50k cho anh Lợi, thêm 2 index này:
@@ -50,16 +50,22 @@
           * cơ chế đảm bảo việc register worker với hệ thống csdl
         * 0.1.5
           * Refix issue register worker
           * Thử nghiệm cơ chế đảm bảo 1 partition chỉ nằm trên 1 worker. 
           * *NOTE*: phần này chưa đảm bảo được việc đủ partitions trên các workers
         
         * 0.1.6
+          * missing version do nâng cấp CICD
+        
+        * 0.1.7
           * Sử dụng threading để quản lý heart_beat và expiry_time
           * Kiểm tra trạng thái subscribe của worker mỗi khi chuẩn bị process data (Đảm bảo rằng việc subscribe phải diễn ra thành công tránh 2 worker cùng xử lý 1 partition)
+        
+        * 0.1.8
+          * Cho phép truyền zookeeper_uri vào param khi khởi tạo Schedule, nếu không truyền thì lấy mặc định từ ENV: ZOOKEEPER_CLUSTER
 Keywords: mobio,scheduler,partitioning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `m_scheduler_partitioning-0.1.7/m_scheduler_partitioning.egg-info/SOURCES.txt` & `m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m_scheduler_partitioning-0.1.7/mobio/libs/m_scheduler_partitioning/m_scheduler.py` & `m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/m_scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,35 +60,43 @@
     def __init__(
         self,
         root_node="test-scheduler",
         node_id=None,
         nop=100,
         delays=1,
         url_connection=None,
+        zookeeper_uri=None
     ):
         if not 10 <= nop <= 1000:
             raise Exception("nop {} not in range 10, 1000".format(nop))
 
         if delays > 3600:
             raise Exception("delays maximum is 3600 seconds")
+
+        if zookeeper_uri:
+            self.zookeeper_uri = zookeeper_uri
+        else:
+            self.zookeeper_uri = os.getenv("ZOOKEEPER_CLUSTER", "localhost:2181")
+
         self.root_path = "/mobio-scheduler/{}".format(root_node)
         self.root_node = root_node
         self.nop = nop
         self.delays = delays
         self.url_connection = url_connection
         if not node_id:
             node_id = generate_nano_id(short=True)
         self.node_id = node_id
         self.my_node_path = "{}/{}".format(self.root_path, node_id)
 
         self.zk_client = KazooClient(
-            hosts=os.getenv("ZOOKEEPER_CLUSTER", "localhost:2181")
+            hosts=self.zookeeper_uri
         )
         self.zk_client.start()
         self.zk_client.ensure_path(self.root_path)
+        print('ensure root path: {}'.format(self.root_path))
         sleep(1)
         self.subscribe_to_node()
         child_watch = ChildrenWatch(
             client=self.zk_client, path=self.root_path, func=self.watch_children
         )
         data_watch_root = DataWatch(
             client=self.zk_client, path=self.root_path, func=self.watch_data_root
```

### Comparing `m_scheduler_partitioning-0.1.7/mobio/libs/m_scheduler_partitioning/scheduler_models/base_model.py` & `m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/scheduler_models/base_model.py`

 * *Files identical despite different names*

### Comparing `m_scheduler_partitioning-0.1.7/mobio/libs/m_scheduler_partitioning/scheduler_models/db_manager.py` & `m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/scheduler_models/db_manager.py`

 * *Files identical despite different names*

### Comparing `m_scheduler_partitioning-0.1.7/mobio/libs/m_scheduler_partitioning/scheduler_models/scheduler_state_model.py` & `m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/scheduler_models/scheduler_state_model.py`

 * *Files identical despite different names*

### Comparing `m_scheduler_partitioning-0.1.7/setup.py` & `m_scheduler_partitioning-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         :return:
         """
         requirements = ["nanoid==2.0.0", "kazoo==2.8.0"]
         return requirements
 
 
 version_dev='0.1.7'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
-version_prod='0.1.6'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
+version_prod='0.1.8'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
 
 run_mode = ''
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -48,15 +48,15 @@
     name="m_scheduler_partitioning" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.7',  # Required, Phần này cũng không được format file.
+    version='0.1.8',  # Required, Phần này cũng không được format file.
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio scheduler partitioning libs",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

