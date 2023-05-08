# Comparing `tmp/me_setups-1.6.8.tar.gz` & `tmp/me_setups-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "me_setups-1.6.8.tar", last modified: Mon Apr 17 15:08:22 2023, max compression
+gzip compressed data, was "me_setups-1.6.9.tar", last modified: Thu Apr 20 07:05:09 2023, max compression
```

## Comparing `me_setups-1.6.8.tar` & `me_setups-1.6.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-17 15:08:22.125926 me_setups-1.6.8/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-04-17 15:08:22.126908 me_setups-1.6.8/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.6.8/README.md
--rw-r--r--   0 idof     (12090585) develop   (1000)     1192 2023-04-17 15:08:22.128933 me_setups-1.6.8/setup.cfg
--rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.6.8/setup.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-17 15:08:22.083221 me_setups-1.6.8/src/
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-17 15:08:22.095888 me_setups-1.6.8/src/me_setups/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.6.8/src/me_setups/__init__.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-17 15:08:22.114887 me_setups-1.6.8/src/me_setups/boards/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.6.8/src/me_setups/boards/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.6.8/src/me_setups/boards/default_boards.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    10582 2023-04-17 15:06:51.000000 me_setups-1.6.8/src/me_setups/boards/gas52.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.6.8/src/me_setups/boards/types.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-17 15:08:22.124907 me_setups-1.6.8/src/me_setups/components/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.6.8/src/me_setups/components/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     8506 2023-04-17 14:42:22.000000 me_setups-1.6.8/src/me_setups/components/comp.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    11841 2023-04-16 12:25:40.000000 me_setups-1.6.8/src/me_setups/components/eqs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      178 2023-02-20 11:40:34.000000 me_setups-1.6.8/src/me_setups/components/mcs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     4047 2023-02-27 18:33:55.000000 me_setups-1.6.8/src/me_setups/components/mcu.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-03-15 13:23:19.000000 me_setups-1.6.8/src/me_setups/utils.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-17 15:08:22.108563 me_setups-1.6.8/src/me_setups.egg-info/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-04-17 15:08:21.000000 me_setups-1.6.8/src/me_setups.egg-info/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-04-17 15:08:22.000000 me_setups-1.6.8/src/me_setups.egg-info/SOURCES.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-04-17 15:08:21.000000 me_setups-1.6.8/src/me_setups.egg-info/dependency_links.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-04-17 15:08:21.000000 me_setups-1.6.8/src/me_setups.egg-info/requires.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-04-17 15:08:21.000000 me_setups-1.6.8/src/me_setups.egg-info/top_level.txt
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-20 07:05:09.090435 me_setups-1.6.9/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-04-20 07:05:09.091765 me_setups-1.6.9/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.6.9/README.md
+-rw-r--r--   0 idof     (12090585) develop   (1000)     1192 2023-04-20 07:05:09.121060 me_setups-1.6.9/setup.cfg
+-rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.6.9/setup.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-20 07:05:09.024309 me_setups-1.6.9/src/
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-20 07:05:09.041357 me_setups-1.6.9/src/me_setups/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.6.9/src/me_setups/__init__.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-20 07:05:09.070338 me_setups-1.6.9/src/me_setups/boards/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.6.9/src/me_setups/boards/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.6.9/src/me_setups/boards/default_boards.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    10927 2023-04-20 07:02:32.000000 me_setups-1.6.9/src/me_setups/boards/gas52.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.6.9/src/me_setups/boards/types.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-20 07:05:09.087410 me_setups-1.6.9/src/me_setups/components/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.6.9/src/me_setups/components/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     8506 2023-04-17 14:42:22.000000 me_setups-1.6.9/src/me_setups/components/comp.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    11985 2023-04-20 07:02:32.000000 me_setups-1.6.9/src/me_setups/components/eqs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      178 2023-02-20 11:40:34.000000 me_setups-1.6.9/src/me_setups/components/mcs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     4047 2023-02-27 18:33:55.000000 me_setups-1.6.9/src/me_setups/components/mcu.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-03-15 13:23:19.000000 me_setups-1.6.9/src/me_setups/utils.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-20 07:05:09.057312 me_setups-1.6.9/src/me_setups.egg-info/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-04-20 07:05:08.000000 me_setups-1.6.9/src/me_setups.egg-info/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-04-20 07:05:08.000000 me_setups-1.6.9/src/me_setups.egg-info/SOURCES.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-04-20 07:05:08.000000 me_setups-1.6.9/src/me_setups.egg-info/dependency_links.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-04-20 07:05:08.000000 me_setups-1.6.9/src/me_setups.egg-info/requires.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-04-20 07:05:08.000000 me_setups-1.6.9/src/me_setups.egg-info/top_level.txt
```

### Comparing `me_setups-1.6.8/PKG-INFO` & `me_setups-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me_setups
-Version: 1.6.8
+Version: 1.6.9
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.6.8/setup.cfg` & `me_setups-1.6.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = me_setups
-version = 1.6.8
+version = 1.6.9
 description = Abstraction for Mobileye setups.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://gitlab.mobileye.com/idof/me-setups
 author = Ido Frenkel
 author_email = ido.frenkel@mobileye.com
 classifiers =
```

### Comparing `me_setups-1.6.8/src/me_setups/boards/default_boards.py` & `me_setups-1.6.9/src/me_setups/boards/default_boards.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.6.8/src/me_setups/boards/gas52.py` & `me_setups-1.6.9/src/me_setups/boards/gas52.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,14 +231,15 @@
         core_type: CoreType = CoreType.PCD,
         timeout: float = 180,
     ) -> list[bool]:
         """wait for core to be write to all EQs
 
         Args:
             core_type (CoreType): The type of core to wait for
+            timeout (float): timeout for waiting until core write complete
 
         Returns:
             list[bool]: list of success core write
         """
         with ThreadPoolExecutor(max_workers=len(self.eqs)) as executor:
             fs = [
                 executor.submit(eq.wait_for_core_write, core_type, timeout)
@@ -268,40 +269,49 @@
         self.mcu.run_serial_cmd("reboot")
 
         if sleep_after > 0:
             self.logger.info(f"sleeping for {sleep_after} seconds.")
             time.sleep(sleep_after)
 
     def is_alive(self, timeout: float = 1, frames: int = 10) -> bool:
-        """Return if all EQs is alive - MEST is running and more then 10 frames ran"""
+        """Return if all EQs is alive - MEST and frames is running.
+
+        Args:
+            timeout (float, optional): timeout to wait until frames. Defaults to 1.
+            frames (int, optional): how many frames to wait for. Defaults to 10.
+
+        Returns:
+            bool: if the Board is alive
+        """
         with ThreadPoolExecutor(max_workers=len(self.eqs)) as executor:
             fs = [executor.submit(eq.is_alive, timeout, frames) for eq in self.eqs]
             results = [f.result() for f in as_completed(fs)]
         return all(results)
 
     def delete_crash_folder(self) -> list[CompletedProcess[str]]:
         """Delete PCD and FCD crash folder"""
         with ThreadPoolExecutor(max_workers=len(self.eqs)) as executor:
             fs = [executor.submit(eq.delete_crash_folder) for eq in self.eqs]
             return [f.result() for f in as_completed(fs)]
 
     def copy_cores(
         self,
         dst: pathlib.Path | str,
+        timeout: float = 300,
     ) -> list[CompletedProcess[str] | None]:
         """Extract cores from EQs
 
         Args:
             dst (pathlib.Path | str): Path to folder to extract to
 
         Returns:
             list[CompletedProcess[str] | None]: status of extracting process.
         """
         with ThreadPoolExecutor(max_workers=len(self.eqs)) as executor:
-            fs = [executor.submit(eq.copy_cores, dst) for eq in self.eqs]
+            fs = [executor.submit(eq.copy_cores, dst, timeout) for eq in self.eqs]
         return [f.result() for f in fs]
 
     @staticmethod
     def create_eqs(
         pbcm_ports: dict[str, str] = DEFAULT_PBCM_PORTS,
         os_type: OSType = OSType.LINUX,
     ) -> list[EyeQ5]:
```

### Comparing `me_setups-1.6.8/src/me_setups/components/comp.py` & `me_setups-1.6.9/src/me_setups/components/comp.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.6.8/src/me_setups/components/eqs.py` & `me_setups-1.6.9/src/me_setups/components/eqs.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,32 +183,37 @@
             str(src),
             f"{self._ssh_root}:{dst}",
             timeout,
             recurcive,
             **kwargs,
         )
 
-    def copy_cores(self, dst: pathlib.Path | str) -> CompletedProcess[str] | None:
+    def copy_cores(
+        self,
+        dst: pathlib.Path | str,
+        timeout: float = 180,
+    ) -> CompletedProcess[str] | None:
         """Extract cores from EQ
 
         Args:
-            dst (pathlib.Path | str): Path to folder to extract to
+            dst (pathlib.Path | str): Path to folder to extract to.
+            timeout (float, optional): timeout for the copy process. Defaults to 180.
 
         Returns:
             CompletedProcess[str] | None: status of extracting process None if no cores
         """
         cores = self.ssh_cmd_stdout("find /media/storage/crash/ -type f").splitlines()
         if not cores:
             return None
         if not all(core.endswith(".zip") for core in cores):
             self.wait_for_core_write(core_type=CoreType.PCD)
         return self.copy_from(
             f"{self.crash_folder}/*",
             pathlib.Path(dst) / self.name,
-            timeout=300,
+            timeout=timeout,
             recurcive=True,
             mkdir=True,
         )
 
     def wait_for_linux_boot(self) -> bool:
         """waits to Linux boot msg "Welcome to EyeQ5"
```

### Comparing `me_setups-1.6.8/src/me_setups/components/mcu.py` & `me_setups-1.6.9/src/me_setups/components/mcu.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.6.8/src/me_setups.egg-info/PKG-INFO` & `me_setups-1.6.9/src/me_setups.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me-setups
-Version: 1.6.8
+Version: 1.6.9
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.6.8/src/me_setups.egg-info/SOURCES.txt` & `me_setups-1.6.9/src/me_setups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

