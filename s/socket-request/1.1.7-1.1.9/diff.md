# Comparing `tmp/socket_request-1.1.7-py3-none-any.whl.zip` & `tmp/socket_request-1.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 26752 bytes, number of entries: 14
+Zip file size: 26895 bytes, number of entries: 14
 -rw-r--r--  2.0 unx     1231 b- defN 22-Dec-05 03:00 socket_request/__init__.py
 -rw-r--r--  2.0 unx     1486 b- defN 22-Dec-05 03:05 socket_request/__main__.py
--rw-r--r--  2.0 unx      343 b- defN 23-Apr-21 02:59 socket_request/__version__.py
--rw-r--r--  2.0 unx    11299 b- defN 23-Mar-29 08:16 socket_request/control_chain_cli.py
+-rw-r--r--  2.0 unx      343 b- defN 23-Apr-21 08:21 socket_request/__version__.py
+-rw-r--r--  2.0 unx    11845 b- defN 23-Apr-21 08:20 socket_request/control_chain_cli.py
 -rw-r--r--  2.0 unx    14629 b- defN 23-Mar-27 02:49 socket_request/core/connect_sock.py
 -rw-r--r--  2.0 unx    23349 b- defN 23-Mar-29 08:15 socket_request/core/control_chain.py
 -rw-r--r--  2.0 unx     8865 b- defN 23-Apr-21 02:59 socket_request/core/docker_sock.py
 -rw-r--r--  2.0 unx     6948 b- defN 22-Dec-05 02:40 socket_request/utils/data.py
 -rw-r--r--  2.0 unx    14402 b- defN 23-Mar-29 06:57 socket_request/utils/utils.py
--rw-r--r--  2.0 unx     4389 b- defN 23-Apr-21 02:59 socket_request-1.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 02:59 socket_request-1.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Apr-21 02:59 socket_request-1.1.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-21 02:59 socket_request-1.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1222 b- defN 23-Apr-21 02:59 socket_request-1.1.7.dist-info/RECORD
-14 files, 88342 bytes uncompressed, 24704 bytes compressed:  72.0%
+-rw-r--r--  2.0 unx     4389 b- defN 23-Apr-21 08:21 socket_request-1.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 08:21 socket_request-1.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Apr-21 08:21 socket_request-1.1.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-21 08:21 socket_request-1.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1222 b- defN 23-Apr-21 08:21 socket_request-1.1.9.dist-info/RECORD
+14 files, 88888 bytes uncompressed, 24847 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: socket_request/utils/data.py
 Comment: 
 
 Filename: socket_request/utils/utils.py
 Comment: 
 
-Filename: socket_request-1.1.7.dist-info/METADATA
+Filename: socket_request-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: socket_request-1.1.7.dist-info/WHEEL
+Filename: socket_request-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: socket_request-1.1.7.dist-info/entry_points.txt
+Filename: socket_request-1.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: socket_request-1.1.7.dist-info/top_level.txt
+Filename: socket_request-1.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: socket_request-1.1.7.dist-info/RECORD
+Filename: socket_request-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## socket_request/__version__.py

```diff
@@ -1,9 +1,9 @@
 ####
 __title__ = 'socket_request'
 __description__ = 'socket_request is building and parsing HTTP requests with UNIX domain sockets.'
 __url__ = 'https://github.com/jinwoo-j/socket_request'
-__version__ = '1.1.7'
+__version__ = '1.1.9'
 __author__ = 'Jinwoo Jeong'
 __author_email__ = 'jinwoo@parametacorp.com'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2021 JINWOO'
```

## socket_request/control_chain_cli.py

```diff
@@ -72,16 +72,18 @@
     parser.add_argument('-pd', '--payload-dict', metavar='payload dict', help=f'payload dict', type=json.loads, default=None)
     parser.add_argument('--interval', type=float,  help=f'retry interval time (seconds)', default=1)
 
     parser.add_argument('--endpoint', metavar='endpoint url', help=f'endpoint url', type=str, default=None)
     parser.add_argument('--cid', metavar='cid', help=f'cid', type=str, default=None)
     parser.add_argument('--gs-file', metavar='gs_file', help=f'genesis file', type=str, default=None)
     parser.add_argument('--platform', metavar='platform', help='platform of goloop', type=str, default=os.environ.get('PLATFORM', 'icon'), choices=AVAIL_PLATFORM)
+    parser.add_argument('--channel', metavar='channel', help='channel name of goloop', type=str, default=os.environ.get('CHANNEL_NAME', 'icon_dex'))
+    parser.add_argument('--role', metavar='role', help='role of goloop', type=int, default=os.environ.get('ROLE', 0), choices=[0, 1, 3])
 
-    parser.add_argument('--compare', metavar='platform', help='compare blockheight endpoint', type=socket_request.str2bool, default=True)
+    parser.add_argument('--compare', metavar='compare', help='compare blockheight endpoint', type=socket_request.str2bool, default=True)
     parser.add_argument('-s', '--unixsocket', metavar='unixsocket', help=f'unix domain socket path (default: {get_base_dir()}/data/cli.socket)',
                         default=f"{get_base_dir()}/data/cli.sock")
 
     return parser.parse_args()
 
 
 def parse_environment():
@@ -113,14 +115,16 @@
 
 
 def check_required(command=None):
     required_params = {
         "payload": ["import_icon", "chain_config", "system_config", "rpc_call"],
         "inspect": ["view_chain", "view_system_config"],
         "seedAddress": ["join"],
+        "role": ["join"],
+        "channel": ["join"],
         "platform": ["join"],
         "compare": ["view_chain"],
         "gs_file": ["join"],
         "blockheight": ["prune", "reset"],
         "restore_name": ["restore"],
 
     }
@@ -141,14 +145,15 @@
 
 def run_function(func, required_keys, args):
     payload = None
     gs_file = None
     seedAddress = None
     result = None
     platform = None
+    role = None
 
     if args.payload:
         if isinstance(args.payload, dict):
             inspect = args.payload
         else:
             json_data = args.payload.read()
             if json_data:
@@ -166,25 +171,31 @@
             gs_file = args.gs_file
         else:
             gs_file = f"{get_base_dir(args)}/config/icon_genesis.zip"
 
     if args.platform:
         platform = args.platform
 
+    if args.role != "":
+        role = args.role
+
+    if args.channel != "":
+        channel = args.channel
+
     if args.command == "view_chain":
         compare = args.compare
 
     must_have_params_command = ["prune", "restore", "reset", "chain_config", "system_config"]
 
     if required_keys:
         arguments = {}
         for required_arg in required_keys:
             if args.debug:
                 debug(locals())
-            if locals().get(required_arg):
+            if locals().get(required_arg, "__NOT_DEFINED__") != "__NOT_DEFINED__":
                 arguments[required_arg] = locals()[required_arg]
             elif args.command in must_have_params_command:
                 try:
                     arguments[required_arg] = getattr(locals().get("args"), required_arg)
                 except Exception as e:
                     print(f"Exception -- {e}")
                     pass
@@ -192,14 +203,16 @@
         if args.debug:
             debug(required_arg)
             debug(arguments)
 
         if payload and func.__name__ in ['join']:
             arguments.update(payload)
 
+        print(f"arguments={arguments}")
+
         if len(arguments) > 0:
             result = func(**arguments)
         else:
             result = func()
     else:
         result = func()
     return result
```

## Comparing `socket_request-1.1.7.dist-info/METADATA` & `socket_request-1.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socket-request
-Version: 1.1.7
+Version: 1.1.9
 Summary: socket_request is building and parsing HTTP requests with UNIX domain sockets.
 Home-page: https://github.com/jinwoo-j/socket_request
 Author: Jinwoo Jeong
 Author-email: jinwoo@parametacorp.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `socket_request-1.1.7.dist-info/RECORD` & `socket_request-1.1.9.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 socket_request/__init__.py,sha256=th1c8L54caSpOK6j80W2PPTQp0pj377uzHx4EjmZGwI,1231
 socket_request/__main__.py,sha256=3vDNAk6O0FjP-OYL-6NGpslwMo6jcB5X3eHmCE8C4l0,1486
-socket_request/__version__.py,sha256=_t4VDafZNhqXl2vMrJsLKXSqPV8AHW_QsjoSTTnrVsY,343
-socket_request/control_chain_cli.py,sha256=88OZE232_gmUD2MtbXcjkEtAGJZJxrjUpkH9Z5mGRuE,11299
+socket_request/__version__.py,sha256=gw7UPfpassfqfAL_SOVSLU9CIOf2bs71UDYwjVY0YQw,343
+socket_request/control_chain_cli.py,sha256=DMosWQd9gX3SXkZuXbBlx2ztegg_f443HgQhtq6d7-0,11845
 socket_request/core/connect_sock.py,sha256=7Q3m1gRdv9KKOFMZyupKMPcZn5gyD9TLLh4cmwrEX5o,14629
 socket_request/core/control_chain.py,sha256=69-j9jhcOt4G8s7heqYwkJosf-Y6dedw60e1BQ5_4-U,23349
 socket_request/core/docker_sock.py,sha256=0B3LZM9R5x6SrDWA2fZqNa5BoNGl85TXtnW6VYIs2-A,8865
 socket_request/utils/data.py,sha256=xG98rz0a6s5DXLWTV66J0vDcZLOiELDf135aJUvzoIk,6948
 socket_request/utils/utils.py,sha256=bBZG_k9zGCP841jxiiVKK386g-cNZ6PjN9gA5XlCFUM,14402
-socket_request-1.1.7.dist-info/METADATA,sha256=bbg8pmAXGJkTO3kFRo9KIzwvcmz3_6zK0tv6cNP7WUg,4389
-socket_request-1.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-socket_request-1.1.7.dist-info/entry_points.txt,sha256=tBwRPrX7Qj5j0QvOCb-th3CzK1dGj3YgTmZgPnHJga0,72
-socket_request-1.1.7.dist-info/top_level.txt,sha256=tZBACHCsKGa1VfS1S4eb38zFd61MH-ydxvksJD5LjyE,15
-socket_request-1.1.7.dist-info/RECORD,,
+socket_request-1.1.9.dist-info/METADATA,sha256=qZO0Fv0CIhBq7neQIsZUvZidQzcqmy1FEWmHbXPBzms,4389
+socket_request-1.1.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+socket_request-1.1.9.dist-info/entry_points.txt,sha256=tBwRPrX7Qj5j0QvOCb-th3CzK1dGj3YgTmZgPnHJga0,72
+socket_request-1.1.9.dist-info/top_level.txt,sha256=tZBACHCsKGa1VfS1S4eb38zFd61MH-ydxvksJD5LjyE,15
+socket_request-1.1.9.dist-info/RECORD,,
```

