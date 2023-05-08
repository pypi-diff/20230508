# Comparing `tmp/py_localtunnel-1.0.1-py3-none-any.whl.zip` & `tmp/py_localtunnel-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 5779 bytes, number of entries: 10
+Zip file size: 6204 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-21 17:07 py_localtunnel/__init__.py
--rw-r--r--  2.0 unx     1282 b- defN 23-Apr-21 17:34 py_localtunnel/cli.py
+-rw-r--r--  2.0 unx     1125 b- defN 23-May-08 02:23 py_localtunnel/cli.py
 -rw-r--r--  2.0 unx      752 b- defN 23-Apr-21 11:17 py_localtunnel/get_assigned_url.py
--rw-r--r--  2.0 unx     4875 b- defN 23-Apr-21 17:34 py_localtunnel/tunnel.py
--rw-r--r--  2.0 unx     1063 b- defN 23-Apr-21 17:35 py_localtunnel-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1620 b- defN 23-Apr-21 17:35 py_localtunnel-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 17:35 py_localtunnel-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 23-Apr-21 17:35 py_localtunnel-1.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-21 17:35 py_localtunnel-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      852 b- defN 23-Apr-21 17:35 py_localtunnel-1.0.1.dist-info/RECORD
-10 files, 10600 bytes uncompressed, 4305 bytes compressed:  59.4%
+-rw-r--r--  2.0 unx      342 b- defN 23-May-08 02:23 py_localtunnel/lt.py
+-rw-r--r--  2.0 unx     4902 b- defN 23-May-08 02:23 py_localtunnel/tunnel.py
+-rw-r--r--  2.0 unx     1063 b- defN 23-May-08 02:38 py_localtunnel-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1841 b- defN 23-May-08 02:38 py_localtunnel-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-08 02:38 py_localtunnel-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       78 b- defN 23-May-08 02:38 py_localtunnel-1.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-May-08 02:38 py_localtunnel-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      928 b- defN 23-May-08 02:38 py_localtunnel-1.0.2.dist-info/RECORD
+11 files, 11138 bytes uncompressed, 4614 bytes compressed:  58.6%
```

## zipnote {}

```diff
@@ -3,29 +3,32 @@
 
 Filename: py_localtunnel/cli.py
 Comment: 
 
 Filename: py_localtunnel/get_assigned_url.py
 Comment: 
 
+Filename: py_localtunnel/lt.py
+Comment: 
+
 Filename: py_localtunnel/tunnel.py
 Comment: 
 
-Filename: py_localtunnel-1.0.1.dist-info/LICENSE
+Filename: py_localtunnel-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: py_localtunnel-1.0.1.dist-info/METADATA
+Filename: py_localtunnel-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: py_localtunnel-1.0.1.dist-info/WHEEL
+Filename: py_localtunnel-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: py_localtunnel-1.0.1.dist-info/entry_points.txt
+Filename: py_localtunnel-1.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: py_localtunnel-1.0.1.dist-info/top_level.txt
+Filename: py_localtunnel-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: py_localtunnel-1.0.1.dist-info/RECORD
+Filename: py_localtunnel-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## py_localtunnel/cli.py

```diff
@@ -1,39 +1,31 @@
 import argparse
-from py_localtunnel.tunnel import Tunnel
+from py_localtunnel.lt import run_localtunnel
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 package_name = "pylt"
 
 example_uses = '''example:
-   pylt port {port_number}'''
+   pylt port {port_number}
+   pylt port {port_number} -s {your_custom_subdomain}'''
 
 def main(argv = None):
     parser = argparse.ArgumentParser(prog=package_name, description="localtunnel alternative in python", epilog=example_uses, formatter_class=argparse.RawDescriptionHelpFormatter)
     subparsers = parser.add_subparsers(dest="command")
 
     port_parser = subparsers.add_parser('port', help="Internal HTTP server port")
     port_parser.add_argument('port', type=int, help="Internal HTTP server port")
     port_parser.add_argument('-s', '--subdomain', type=str, default="", help="Request this subdomain")
 
     parser.add_argument('-v',"--version", action="store_true", dest="version", help="check version of deb")
 
     args = parser.parse_args(argv)
 
     if args.command == "port":
-        t = Tunnel()
-        url = t.get_url(args.subdomain)
-        print(f" your url is: {url}")
-        try:
-            t.create_tunnel(args.port)
-        except KeyboardInterrupt:
-            print("KeyboardInterrupt: stopping tunnel")
-
-        t.stop_tunnel()
-
+        run_localtunnel(args.port, args.subdomain)
     elif args.version:
         return print(__version__)
     else:
         parser.print_help()
 
 if __name__ == '__main__':
     raise SystemExit(main())
```

## py_localtunnel/tunnel.py

```diff
@@ -102,15 +102,15 @@
         while reply_ch.qsize() < self.assigned_url_info.max_conn_count:
             cmd = self.cmd_chan.get()
             if cmd == 'STOP':
                 break
 
     def stop_tunnel(self) -> None:
         if Debug:
-            print(f"Stop tunnel for localPort[{self.local_port}]!")
+            print(f" Info: Stop tunnel for localPort[{self.local_port}]!")
         self.cmd_chan.put('STOP')
         for tunnel_conn in self.tunnel_conns:
             tunnel_conn.stop_tunnel()
 
     def get_url(self, assigned_domain: str) -> str:
         if not assigned_domain:
             assigned_domain = "?new"
@@ -124,8 +124,9 @@
         self.start_tunnel()
     
     def check_local_port(self):
         try:
             with socket.create_connection(('localhost', self.local_port)) as sock:
                 pass
         except ConnectionRefusedError:
-            raise Exception('Cannot connect to local port')        
+            print(' Error: Cannot connect to local port')   
+            os._exit(0)
```

## Comparing `py_localtunnel-1.0.1.dist-info/LICENSE` & `py_localtunnel-1.0.2.dist-info/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Jak Bin
+Copyright (c) 2023 Jak Bin
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

## Comparing `py_localtunnel-1.0.1.dist-info/METADATA` & `py_localtunnel-1.0.2.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-localtunnel
-Version: 1.0.1
+Version: 1.0.2
 Summary: localtunnel alternative in python
 Home-page: https://github.com/jakbin/py-localtunnel
 Author: Jak Bin
 Author-email: jakbin4747@gmail.com
 Project-URL: Bug Tracker, https://github.com/jakbin/py-localtunnel/issues
 Keywords: localtunnel,port-forwarding,expose-locahost,localtunnel
 Classifier: Programming Language :: Python :: 3.6
@@ -14,15 +14,15 @@
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3
 
 # py-localtunnel
 
-localtunnel alternative in python.
+localtunnel client in python.
 
  [![PyPI version](https://badge.fury.io/py/py-localtunnel.svg)](https://pypi.org/project/py-localtunnel/)
  [![Downloads](https://pepy.tech/badge/py-localtunnel/month)](https://pepy.tech/project/py-localtunnel)
  [![Downloads](https://static.pepy.tech/personalized-badge/py-localtunnel?period=total&units=international_system&left_color=green&right_color=blue&left_text=Total%20Downloads)](https://pepy.tech/project/py-localtunnel)
  ![GitHub Contributors](https://img.shields.io/github/contributors/jakbin/py-localtunnel)
  ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/jakbin/py-localtunnel)
  ![GitHub last commit](https://img.shields.io/github/last-commit/jakbin/py-localtunnel)
@@ -33,8 +33,21 @@
 
 ## Installation
 
 ```sh
 pip3 install py-localtunnel
 ```
 
-Special thanks for chatgpt.
+## Usage
+```sh
+pylt port 8080
+```
+
+```sh
+pylt port 8080 -s your_custom_subdomain
+```
+
+## Contributing
+
+Whether reporting bugs, discussing improvements and new ideas or writing extensions: Contributions to pysonDB are welcome!
+
+Special thanks to chatgpt.
```

## Comparing `py_localtunnel-1.0.1.dist-info/RECORD` & `py_localtunnel-1.0.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 py_localtunnel/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-py_localtunnel/cli.py,sha256=C-ACrnV4GEM3q3YHBHX6Z40iTAxo3nm6-86HzSORLxs,1282
+py_localtunnel/cli.py,sha256=7kvu1LCrFXwKs_2tY5dLYYFYxfY72eX0n_ILWtFaBhU,1125
 py_localtunnel/get_assigned_url.py,sha256=MwO3j--DY7XQe50R4UM5q76ksMVTV2eKfe-rEBT_NV0,752
-py_localtunnel/tunnel.py,sha256=Xto7QTXmi6MrgQL55Eohlv9F6fqjd7IjC30Nxs4L50A,4875
-py_localtunnel-1.0.1.dist-info/LICENSE,sha256=lTtOcmt5ceTGoxI999vYv8K2yOk7-pipowcPGw7ERa8,1063
-py_localtunnel-1.0.1.dist-info/METADATA,sha256=cMyG5Vm7pok9iqQvYN7sYYK70D9CtTgw84GJwL_G_yc,1620
-py_localtunnel-1.0.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-py_localtunnel-1.0.1.dist-info/entry_points.txt,sha256=Zd47S0HX3mfPWj7rmIlbG2TlF9FCVyyuN_axoiDUf78,49
-py_localtunnel-1.0.1.dist-info/top_level.txt,sha256=WzNG5oJsOgbON-VjH4TlGoECoGXXr8QzJ64S5xbHYn8,15
-py_localtunnel-1.0.1.dist-info/RECORD,,
+py_localtunnel/lt.py,sha256=lY_wn1qwTVMo37tN0UUlJb8CRFJOTE91zHMirR6m8Co,342
+py_localtunnel/tunnel.py,sha256=1jL2OTy4-SO4UQ3B02KH2rLMzbM40pe4tVp6FZ8Um9o,4902
+py_localtunnel-1.0.2.dist-info/LICENSE,sha256=JuFAr1EF_Q8M1Dc0SU8QxtJljPHoA4cR211lBJUxyZc,1063
+py_localtunnel-1.0.2.dist-info/METADATA,sha256=-kMQdngEQKI0-aIiLroxK_l9FUQSWakO2oF0xsWyzu0,1841
+py_localtunnel-1.0.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+py_localtunnel-1.0.2.dist-info/entry_points.txt,sha256=XrU53rSlghtVpwShQ2Zb0YEr_qgy7FFqwaAw0KTbJ7E,78
+py_localtunnel-1.0.2.dist-info/top_level.txt,sha256=WzNG5oJsOgbON-VjH4TlGoECoGXXr8QzJ64S5xbHYn8,15
+py_localtunnel-1.0.2.dist-info/RECORD,,
```

