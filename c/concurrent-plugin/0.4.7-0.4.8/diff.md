# Comparing `tmp/concurrent_plugin-0.4.7-py3-none-any.whl.zip` & `tmp/concurrent_plugin-0.4.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 30546 bytes, number of entries: 17
+Zip file size: 30530 bytes, number of entries: 17
 -rw-rw-r--  2.0 unx        2 b- defN 22-Dec-14 21:27 concurrent_plugin/__init__.py
 -rw-rw-r--  2.0 unx    32381 b- defN 23-May-04 12:20 concurrent_plugin/concurrent_backend.py
 -rw-rw-r--  2.0 unx    16820 b- defN 22-Dec-14 21:27 concurrent_plugin/concurrent_core.py
 -rw-rw-r--  2.0 unx    15759 b- defN 23-Apr-27 01:05 concurrent_plugin/login.py
 -rw-rw-r--  2.0 unx     3994 b- defN 23-Apr-27 01:05 concurrent_plugin/periodic_run.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/__init__.py
 -rw-rw-r--  2.0 unx      990 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/infin_download.py
 -rw-rw-r--  2.0 unx     1339 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/infin_prefetch.py
 -rw-rw-r--  2.0 unx    10783 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/infinfs.py
 -rw-rw-r--  2.0 unx     5326 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/infinmount.py
 -rw-rw-r--  2.0 unx     1140 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/mount_main.py
--rw-rw-r--  2.0 unx    15917 b- defN 23-May-08 03:34 concurrent_plugin/infinfs/mount_service.py
--rw-rw-r--  2.0 unx      268 b- defN 23-May-08 03:35 concurrent_plugin-0.4.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-08 03:35 concurrent_plugin-0.4.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx      181 b- defN 23-May-08 03:35 concurrent_plugin-0.4.7.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       18 b- defN 23-May-08 03:35 concurrent_plugin-0.4.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1567 b- defN 23-May-08 03:35 concurrent_plugin-0.4.7.dist-info/RECORD
-17 files, 106577 bytes uncompressed, 27912 bytes compressed:  73.8%
+-rw-rw-r--  2.0 unx    16259 b- defN 23-May-08 06:19 concurrent_plugin/infinfs/mount_service.py
+-rw-rw-r--  2.0 unx      268 b- defN 23-May-08 06:21 concurrent_plugin-0.4.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-08 06:21 concurrent_plugin-0.4.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      181 b- defN 23-May-08 06:21 concurrent_plugin-0.4.8.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       18 b- defN 23-May-08 06:21 concurrent_plugin-0.4.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1567 b- defN 23-May-08 06:21 concurrent_plugin-0.4.8.dist-info/RECORD
+17 files, 106919 bytes uncompressed, 27896 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: concurrent_plugin/infinfs/mount_main.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/mount_service.py
 Comment: 
 
-Filename: concurrent_plugin-0.4.7.dist-info/METADATA
+Filename: concurrent_plugin-0.4.8.dist-info/METADATA
 Comment: 
 
-Filename: concurrent_plugin-0.4.7.dist-info/WHEEL
+Filename: concurrent_plugin-0.4.8.dist-info/WHEEL
 Comment: 
 
-Filename: concurrent_plugin-0.4.7.dist-info/entry_points.txt
+Filename: concurrent_plugin-0.4.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: concurrent_plugin-0.4.7.dist-info/top_level.txt
+Filename: concurrent_plugin-0.4.8.dist-info/top_level.txt
 Comment: 
 
-Filename: concurrent_plugin-0.4.7.dist-info/RECORD
+Filename: concurrent_plugin-0.4.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## concurrent_plugin/infinfs/mount_service.py

```diff
@@ -13,32 +13,24 @@
 import requests
 import subprocess
 # importing it as kubernetes.client since 'client' is used in the code in some places as the Mlflow client.  this mlflow 'client' conflicts with 'from kubernetes import client'.  Need to cleanup.
 import kubernetes.client
 from kubernetes import client, config
 import dpath
 from datetime import datetime
-import atexit
 
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 
 
 FUSE_DEBUG_FILE = '/tmp/fuse_debug.log'
 VERBOSE = False
 
 mlflow_run_status = None
 
-def cleanup_atexit(run_id):
-    if mlflow_run_status:
-      print(f"mount_service: atexit. mlflow_run_status={mlflow_run_status}. Doing nothing", flush=True)
-    else:
-      print(f"mount_service: atexit. WARN mlflow_run_status not set. Calling update_mlflow_run for FAILED", flush=True)
-      update_mlflow_run(run_id, "FAILED")
-
 def parse_mount_request(data):
     req = json.loads(data.decode('utf-8'))
     if req['use_cache'].lower() == 'false':
         use_cache = False
     else:
         use_cache = True
     if req['shadow_path'].lower() == 'none':
@@ -287,64 +279,74 @@
 if __name__ == '__main__':
     print_info("Starting..")
     HOST = "127.0.0.1"
     PORT = 7963
     last_upload_time = time.time()
     start_time = time.time()
     run_id = os.getenv('MLFLOW_RUN_ID')
-    atexit.register(cleanup_atexit, run_id)
-    print("Environment #", os.environ)
-    config.load_incluster_config()
-    print('Setting k8s client configuration item retries to 10', flush=True)
-    kubernetes.client.configuration.retries = 10
-    k8s_client:client.CoreV1Api = client.CoreV1Api()
-    pod_name = os.getenv('MY_POD_NAME')
-    pod_namespace = os.getenv('MY_POD_NAMESPACE')
-    dag_execution_id = os.getenv('DAG_EXECUTION_ID')
-    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-        s.settimeout(15)
-        s.bind((HOST, PORT))
-        print('Mount/Monitor service starting for runid {0}, and podname {1}'.format(run_id, pod_name), flush=True)
-        print('Listening on port {}:{}'.format(HOST, PORT), flush=True)
-        s.listen()
-        mount_service_ready()
-        while True:
-            print_info('Waiting for request..')
-            try:
-                conn, addr = s.accept()
-            except socket.timeout:
-                print_info('accept timed out')
-                pass
-            else:
-                with conn:
-                    print_info(f"Connected by {addr}")
-                    data = conn.recv(1024*16)
-                    if not data:
-                        time.sleep(1)
-                        continue
-                    try:
-                        mount_path, mount_spec, shadow_path, use_cache = parse_mount_request(data)
-                        print_info("mount request {}, {}, {}, {}".format(
-                            mount_path, mount_spec, shadow_path, use_cache))
-                        infinmount.perform_mount(mount_path, mount_spec, shadow_path=shadow_path, use_cache=use_cache)
-                        response = "success".encode('utf-8')
-                        print_info("mount successful")
-                    except Exception as ex:
-                        print_info('Exception in mounting: '+str(ex))
-                        response = str(ex).encode('utf-8')
-                    conn.send(response)
-            if not fetch_upload_pod_status_logs(k8s_client, run_id, pod_name, pod_namespace):
-                print_info("Task process done, exiting mount service")
-                exitCode = get_task_exit_code(k8s_client, pod_name, pod_namespace)
-                if exitCode == 0:
-                    update_mlflow_run(run_id, "FINISHED")
-                    mlflow_run_status = "FINISHED"
-                else:
-                    update_mlflow_run(run_id, "FAILED")
-                    mlflow_run_status = "FAILED"
-                fetch_upload_pod_status_logs(k8s_client, run_id, pod_name, pod_namespace)
-                if dag_execution_id:
-                    launch_dag_controller()
+    try:
+        print("Environment #", os.environ)
+        config.load_incluster_config()
+        print('Setting k8s client configuration item retries to 10', flush=True)
+        kubernetes.client.configuration.retries = 10
+        k8s_client:client.CoreV1Api = client.CoreV1Api()
+        pod_name = os.getenv('MY_POD_NAME')
+        pod_namespace = os.getenv('MY_POD_NAMESPACE')
+        dag_execution_id = os.getenv('DAG_EXECUTION_ID')
+        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+            s.settimeout(15)
+            s.bind((HOST, PORT))
+            print('Mount/Monitor service starting for runid {0}, and podname {1}'.format(run_id, pod_name), flush=True)
+            print('Listening on port {}:{}'.format(HOST, PORT), flush=True)
+            s.listen()
+            mount_service_ready()
+            while True:
+                print_info('Waiting for request..')
+                try:
+                    conn, addr = s.accept()
+                except socket.timeout:
+                    print_info('accept timed out')
+                    pass
                 else:
-                    print_info('Not a dag execution, skip dag controller')
+                    with conn:
+                        print_info(f"Connected by {addr}")
+                        data = conn.recv(1024*16)
+                        if not data:
+                            time.sleep(1)
+                            continue
+                        try:
+                            mount_path, mount_spec, shadow_path, use_cache = parse_mount_request(data)
+                            print_info("mount request {}, {}, {}, {}".format(
+                                mount_path, mount_spec, shadow_path, use_cache))
+                            infinmount.perform_mount(mount_path, mount_spec, shadow_path=shadow_path, use_cache=use_cache)
+                            response = "success".encode('utf-8')
+                            print_info("mount successful")
+                        except Exception as ex:
+                            print_info('Exception in mounting: '+str(ex))
+                            response = str(ex).encode('utf-8')
+                        conn.send(response)
+                if not fetch_upload_pod_status_logs(k8s_client, run_id, pod_name, pod_namespace):
+                    print_info("Task process done, exiting mount service")
+                    exitCode = get_task_exit_code(k8s_client, pod_name, pod_namespace)
+                    if exitCode == 0:
+                        update_mlflow_run(run_id, "FINISHED")
+                        mlflow_run_status = "FINISHED"
+                    else:
+                        update_mlflow_run(run_id, "FAILED")
+                        mlflow_run_status = "FAILED"
+                    fetch_upload_pod_status_logs(k8s_client, run_id, pod_name, pod_namespace)
+                    if dag_execution_id:
+                        launch_dag_controller()
+                    else:
+                        print_info('Not a dag execution, skip dag controller')
+                    exit(0)
+    except Exception as e1:
+        if mlflow_run_status:
+            print(f"mount_service: Caught {e1}. mlflow_run_status={mlflow_run_status}. Doing nothing", flush=True)
+            if mlflow_run_status == "FINISHED":
                 exit(0)
-
+            else:
+                exit(255)
+        else:
+            print(f"mount_service: Caught {e1} WARN mlflow_run_status not set. Calling update_mlflow_run for FAILED", flush=True)
+            update_mlflow_run(run_id, "FAILED")
+            exit(255)
```

## Comparing `concurrent_plugin-0.4.7.dist-info/RECORD` & `concurrent_plugin-0.4.8.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -5,13 +5,13 @@
 concurrent_plugin/periodic_run.py,sha256=Ud66-3AtnonAO6oOhcn2EwJQPfbljcrlCQeR23ELH1c,3994
 concurrent_plugin/infinfs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 concurrent_plugin/infinfs/infin_download.py,sha256=6yILg2brDNDNMFGqayFHIshB4cl25byn5dal0QI7JKQ,990
 concurrent_plugin/infinfs/infin_prefetch.py,sha256=ICqCHaiugg0z_gm4cMpQGJHozSXuf54kAw97g4yAhGU,1339
 concurrent_plugin/infinfs/infinfs.py,sha256=3xId2Ocp7UJv7ntBgpr-KCFv5wGJQFw2m8csamIHiYY,10783
 concurrent_plugin/infinfs/infinmount.py,sha256=Y9BPuggy0P9gz-kYH2ZhLy24Z1WTsw7GgU3rgH7JSsY,5326
 concurrent_plugin/infinfs/mount_main.py,sha256=ehL8zXZ1HRviaukp753TjJ6pFCtO9uUfUIjx8yfUHVE,1140
-concurrent_plugin/infinfs/mount_service.py,sha256=4eN3g1r9OTllJp7k7GXd7cnKEUU6gz4Ucy00eK12Vso,15917
-concurrent_plugin-0.4.7.dist-info/METADATA,sha256=rPyWpAWSnie-baw_pwlDmgRdcGD60YSouA9UOZc5I_o,268
-concurrent_plugin-0.4.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-concurrent_plugin-0.4.7.dist-info/entry_points.txt,sha256=1x__D3G335a8YKoEFWsCaUHB-H1IqgvVq07ga4TgtGk,181
-concurrent_plugin-0.4.7.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
-concurrent_plugin-0.4.7.dist-info/RECORD,,
+concurrent_plugin/infinfs/mount_service.py,sha256=mD3Y4oq1LMdNrBtKy2HeWL3JaWmqSbfJzpFTzthtgSI,16259
+concurrent_plugin-0.4.8.dist-info/METADATA,sha256=hLIbHcex7BrkDhsDNVf8qFF8Uw9ufKK5aHw0RogabLY,268
+concurrent_plugin-0.4.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+concurrent_plugin-0.4.8.dist-info/entry_points.txt,sha256=1x__D3G335a8YKoEFWsCaUHB-H1IqgvVq07ga4TgtGk,181
+concurrent_plugin-0.4.8.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
+concurrent_plugin-0.4.8.dist-info/RECORD,,
```

