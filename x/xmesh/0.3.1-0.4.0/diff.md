# Comparing `tmp/xmesh-0.3.1.tar.gz` & `tmp/xmesh-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmesh-0.3.1.tar", last modified: Fri Sep 23 07:57:32 2022, max compression
+gzip compressed data, was "xmesh-0.4.0.tar", last modified: Mon May  8 13:41:22 2023, max compression
```

## Comparing `xmesh-0.3.1.tar` & `xmesh-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 snowyang   (501) staff       (20)        0 2022-09-23 07:57:32.324272 xmesh-0.3.1/
--rw-r--r--   0 snowyang   (501) staff       (20)    11357 2022-09-16 03:55:08.000000 xmesh-0.3.1/LICENSE
--rw-r--r--   0 snowyang   (501) staff       (20)      984 2022-09-23 07:57:32.324359 xmesh-0.3.1/PKG-INFO
--rw-r--r--   0 snowyang   (501) staff       (20)      508 2022-09-16 03:55:08.000000 xmesh-0.3.1/README.md
--rw-r--r--   0 snowyang   (501) staff       (20)      104 2022-09-16 03:55:08.000000 xmesh-0.3.1/pyproject.toml
--rw-r--r--   0 snowyang   (501) staff       (20)      768 2022-09-23 07:57:32.324664 xmesh-0.3.1/setup.cfg
-drwxr-xr-x   0 snowyang   (501) staff       (20)        0 2022-09-23 07:57:32.321494 xmesh-0.3.1/src/
-drwxr-xr-x   0 snowyang   (501) staff       (20)        0 2022-09-23 07:57:32.322695 xmesh-0.3.1/src/xmesh/
--rw-r--r--   0 snowyang   (501) staff       (20)        0 2022-09-16 03:55:08.000000 xmesh-0.3.1/src/xmesh/__init__.py
--rw-r--r--   0 snowyang   (501) staff       (20)    35801 2022-09-23 07:57:16.000000 xmesh-0.3.1/src/xmesh/main.py
-drwxr-xr-x   0 snowyang   (501) staff       (20)        0 2022-09-23 07:57:32.324168 xmesh-0.3.1/src/xmesh.egg-info/
--rw-r--r--   0 snowyang   (501) staff       (20)      984 2022-09-23 07:57:32.000000 xmesh-0.3.1/src/xmesh.egg-info/PKG-INFO
--rw-r--r--   0 snowyang   (501) staff       (20)      282 2022-09-23 07:57:32.000000 xmesh-0.3.1/src/xmesh.egg-info/SOURCES.txt
--rw-r--r--   0 snowyang   (501) staff       (20)        1 2022-09-23 07:57:32.000000 xmesh-0.3.1/src/xmesh.egg-info/dependency_links.txt
--rw-r--r--   0 snowyang   (501) staff       (20)       42 2022-09-23 07:57:32.000000 xmesh-0.3.1/src/xmesh.egg-info/entry_points.txt
--rw-r--r--   0 snowyang   (501) staff       (20)       14 2022-09-23 07:57:32.000000 xmesh-0.3.1/src/xmesh.egg-info/requires.txt
--rw-r--r--   0 snowyang   (501) staff       (20)        6 2022-09-23 07:57:32.000000 xmesh-0.3.1/src/xmesh.egg-info/top_level.txt
+drwxr-xr-x   0 snowyang   (501) staff       (20)        0 2023-05-08 13:41:22.214871 xmesh-0.4.0/
+-rw-r--r--   0 snowyang   (501) staff       (20)    11357 2022-09-16 03:55:08.000000 xmesh-0.4.0/LICENSE
+-rw-r--r--   0 snowyang   (501) staff       (20)      984 2023-05-08 13:41:22.214933 xmesh-0.4.0/PKG-INFO
+-rw-r--r--   0 snowyang   (501) staff       (20)      508 2022-09-16 03:55:08.000000 xmesh-0.4.0/README.md
+-rw-r--r--   0 snowyang   (501) staff       (20)      104 2022-09-16 03:55:08.000000 xmesh-0.4.0/pyproject.toml
+-rw-r--r--   0 snowyang   (501) staff       (20)      768 2023-05-08 13:41:22.215208 xmesh-0.4.0/setup.cfg
+drwxr-xr-x   0 snowyang   (501) staff       (20)        0 2023-05-08 13:41:22.213019 xmesh-0.4.0/src/
+drwxr-xr-x   0 snowyang   (501) staff       (20)        0 2023-05-08 13:41:22.213747 xmesh-0.4.0/src/xmesh/
+-rw-r--r--   0 snowyang   (501) staff       (20)        0 2022-09-16 03:55:08.000000 xmesh-0.4.0/src/xmesh/__init__.py
+-rw-r--r--   0 snowyang   (501) staff       (20)    35686 2023-05-08 13:40:36.000000 xmesh-0.4.0/src/xmesh/main.py
+drwxr-xr-x   0 snowyang   (501) staff       (20)        0 2023-05-08 13:41:22.214769 xmesh-0.4.0/src/xmesh.egg-info/
+-rw-r--r--   0 snowyang   (501) staff       (20)      984 2023-05-08 13:41:22.000000 xmesh-0.4.0/src/xmesh.egg-info/PKG-INFO
+-rw-r--r--   0 snowyang   (501) staff       (20)      282 2023-05-08 13:41:22.000000 xmesh-0.4.0/src/xmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 snowyang   (501) staff       (20)        1 2023-05-08 13:41:22.000000 xmesh-0.4.0/src/xmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 snowyang   (501) staff       (20)       42 2023-05-08 13:41:22.000000 xmesh-0.4.0/src/xmesh.egg-info/entry_points.txt
+-rw-r--r--   0 snowyang   (501) staff       (20)       14 2023-05-08 13:41:22.000000 xmesh-0.4.0/src/xmesh.egg-info/requires.txt
+-rw-r--r--   0 snowyang   (501) staff       (20)        6 2023-05-08 13:41:22.000000 xmesh-0.4.0/src/xmesh.egg-info/top_level.txt
```

### Comparing `xmesh-0.3.1/LICENSE` & `xmesh-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmesh-0.3.1/PKG-INFO` & `xmesh-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmesh
-Version: 0.3.1
+Version: 0.4.0
 Summary: xMesh sniffer.
 Home-page: https://github.com/smartsnow/xmesh
 Author: Snow Yang
 Author-email: snowyang.iot@outlook.com
 Project-URL: Bug Tracker, https://github.com/smartsnow/xmesh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xmesh-0.3.1/setup.cfg` & `xmesh-0.4.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xmesh
-version = 0.3.1
+version = 0.4.0
 author = Snow Yang
 author_email = snowyang.iot@outlook.com
 description = xMesh sniffer.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/smartsnow/xmesh
 project_urls =
```

### Comparing `xmesh-0.3.1/src/xmesh/main.py` & `xmesh-0.4.0/src/xmesh/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,15 +384,15 @@
     index.
     """
 
     ports = []
     portslist = comports()
     if sys.platform == 'darwin':
         if type == 'sniffer':
-            ports = [port.device for port in portslist if port.device == '/dev/cu.usbserial-MX0101']
+            ports = [port.device for port in portslist if 'MX0101' in port.device]
         elif type == 'proxy':
             ports = [port.device for port in portslist if port.device == '/dev/cu.usbserial-MX0201']
         elif type == 'cli':
             ports = [port.device for port in portslist if port.device == '/dev/cu.usbserial-MX0301']
     else:
         if type == 'sniffer':
             ports = [port.device for port in portslist if port.serial_number == 'MX0101']
@@ -422,14 +422,15 @@
         self.eol = eol
         self.filters = filters
         self.update_transformations()
         self.exit_character = unichr(0x1d)  # GS/CTRL+]
         self.menu_character = unichr(0x14)  # Menu: CTRL+T
         self.reboot_character = unichr(0x12)  # CTRL+R
         self.start_character = unichr(0x06)  # CTRL+F
+        self.switch_character = unichr(0x0e)  # CTRL+N
         self.alive = None
         self._reader_alive = None
         self.receiver_thread = None
         self.rx_decoder = None
         self.tx_decoder = None
         self.tx_encoder = None
 
@@ -518,25 +519,29 @@
         sys.stderr.write('--- serial input encoding: {}\n'.format(self.input_encoding))
         sys.stderr.write('--- serial output encoding: {}\n'.format(self.output_encoding))
         sys.stderr.write('--- EOL: {}\n'.format(self.eol.upper()))
         sys.stderr.write('--- filters: {}\n'.format(' '.join(self.filters)))
 
     def reader(self):
         """loop and copy serial->console"""
+        self.newline = False
         try:
             while self.alive and self._reader_alive:
                 # read all that is there or wait for one byte
                 data = self.serial.read(1)
                 if data:
                     if self.raw:
+                        if self.newline:
+                            timestamp = '{0:%H:%M:%S:%f} '.format(datetime.datetime.now())[:-4]
+                            self.logfile.write(timestamp)
+                            self.newline = False
                         self.console.write_bytes(data)
                         self.logfile.write(data.decode())
                         if data == b'\n':
-                            timestamp = '{0:%H:%M:%S} '.format(datetime.datetime.now())
-                            self.logfile.write(timestamp)
+                            self.newline = True
                     else:
                         text = self.rx_decoder.decode(data)
                         for transformation in self.rx_transformations:
                             text = transformation.rx(text)
                             self.console.write(text)
         except serial.SerialException:
             self.alive = False
@@ -563,24 +568,17 @@
                     self.handle_menu_key(c)
                     menu_active = False
                 elif c == self.menu_character:
                     menu_active = True      # next char will be for menu
                 elif c == self.exit_character:
                     self.stop()             # exit app
                     break
-                elif c == self.reboot_character:
-                    if self.type == 'cli':
-                        self.serial.write(self.tx_encoder.encode(c))
-                    else:
-                        self.serial.write(self.tx_encoder.encode('kernel reboot cold\r\n\r\n'))
-                elif c == self.start_character:
-                    if self.type == 'cli':
-                        self.serial.write(self.tx_encoder.encode(c))
-                    else:
-                        self.serial.write(self.tx_encoder.encode('sniffer start\r\n'))
+                elif c == self.reboot_character or c == self.start_character or c == self.switch_character:
+                    # sys.stdout.write('%x\n' % ord(c))
+                    self.serial.write(self.tx_encoder.encode(c))
                 else:
                     #~ if self.raw:
                     text = c
                     for transformation in self.tx_transformations:
                         text = transformation.tx(text)
                     self.serial.write(self.tx_encoder.encode(text))
                     if self.echo:
```

### Comparing `xmesh-0.3.1/src/xmesh.egg-info/PKG-INFO` & `xmesh-0.4.0/src/xmesh.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmesh
-Version: 0.3.1
+Version: 0.4.0
 Summary: xMesh sniffer.
 Home-page: https://github.com/smartsnow/xmesh
 Author: Snow Yang
 Author-email: snowyang.iot@outlook.com
 Project-URL: Bug Tracker, https://github.com/smartsnow/xmesh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

