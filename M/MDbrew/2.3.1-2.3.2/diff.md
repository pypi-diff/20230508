# Comparing `tmp/MDbrew-2.3.1.tar.gz` & `tmp/MDbrew-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDbrew-2.3.1.tar", last modified: Sun May  7 05:37:54 2023, max compression
+gzip compressed data, was "MDbrew-2.3.2.tar", last modified: Mon May  8 12:17:25 2023, max compression
```

## Comparing `MDbrew-2.3.1.tar` & `MDbrew-2.3.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-07 05:37:54.150186 MDbrew-2.3.1/
--rw-r--r--   0 minu       (501) staff       (20)       25 2023-05-05 06:22:51.000000 MDbrew-2.3.1/MANIFEST.in
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-07 05:37:54.146615 MDbrew-2.3.1/MDbrew/
--rw-r--r--   0 minu       (501) staff       (20)      238 2023-05-07 05:37:43.000000 MDbrew-2.3.1/MDbrew/__init__.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-07 05:37:54.147764 MDbrew-2.3.1/MDbrew/analysis/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/analysis/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     4477 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/analysis/msd.py
--rw-r--r--   0 minu       (501) staff       (20)     5860 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/analysis/rdf.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-07 05:37:54.148005 MDbrew-2.3.1/MDbrew/application/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/application/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     9705 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/application/brewcp2k.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-07 05:37:54.148429 MDbrew-2.3.1/MDbrew/main/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     5302 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/brewery.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-07 05:37:54.149316 MDbrew-2.3.1/MDbrew/main/filetype/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/filetype/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)      896 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/filetype/gro.py
--rw-r--r--   0 minu       (501) staff       (20)      860 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/filetype/lmps.py
--rw-r--r--   0 minu       (501) staff       (20)      777 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/filetype/pdb.py
--rw-r--r--   0 minu       (501) staff       (20)     4172 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/filetype/trr.py
--rw-r--r--   0 minu       (501) staff       (20)     1370 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/filetype/vasp.py
--rw-r--r--   0 minu       (501) staff       (20)      486 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/filetype/xyz.py
--rw-r--r--   0 minu       (501) staff       (20)     1163 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/opener.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-07 05:37:54.150037 MDbrew-2.3.1/MDbrew/tool/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/tool/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     3618 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/tool/colorfont.py
--rw-r--r--   0 minu       (501) staff       (20)     1578 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/tool/decorator.py
--rw-r--r--   0 minu       (501) staff       (20)      756 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/tool/doctor.py
--rw-r--r--   0 minu       (501) staff       (20)      619 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/tool/spacer.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-07 05:37:54.147346 MDbrew-2.3.1/MDbrew.egg-info/
--rw-r--r--   0 minu       (501) staff       (20)      332 2023-05-07 05:37:54.000000 MDbrew-2.3.1/MDbrew.egg-info/PKG-INFO
--rw-r--r--   0 minu       (501) staff       (20)      740 2023-05-07 05:37:54.000000 MDbrew-2.3.1/MDbrew.egg-info/SOURCES.txt
--rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-07 05:37:54.000000 MDbrew-2.3.1/MDbrew.egg-info/dependency_links.txt
--rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-07 05:37:16.000000 MDbrew-2.3.1/MDbrew.egg-info/not-zip-safe
--rw-r--r--   0 minu       (501) staff       (20)        7 2023-05-07 05:37:54.000000 MDbrew-2.3.1/MDbrew.egg-info/top_level.txt
--rw-r--r--   0 minu       (501) staff       (20)      332 2023-05-07 05:37:54.150258 MDbrew-2.3.1/PKG-INFO
--rw-r--r--   0 minu       (501) staff       (20)       62 2023-05-05 06:22:51.000000 MDbrew-2.3.1/requirement.txt
--rw-r--r--   0 minu       (501) staff       (20)       79 2023-05-07 05:37:54.150480 MDbrew-2.3.1/setup.cfg
--rw-r--r--   0 minu       (501) staff       (20)      653 2023-05-07 05:37:07.000000 MDbrew-2.3.1/setup.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-08 12:17:25.644718 MDbrew-2.3.2/
+-rw-r--r--   0 minu       (501) staff       (20)       25 2023-05-07 05:40:59.000000 MDbrew-2.3.2/MANIFEST.in
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-08 12:17:25.640618 MDbrew-2.3.2/MDbrew/
+-rw-r--r--   0 minu       (501) staff       (20)      238 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/__init__.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-08 12:17:25.642027 MDbrew-2.3.2/MDbrew/analysis/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/analysis/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     4477 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/analysis/msd.py
+-rw-r--r--   0 minu       (501) staff       (20)     5860 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/analysis/rdf.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-08 12:17:25.642364 MDbrew-2.3.2/MDbrew/application/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/application/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)    10054 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/application/brewcp2k.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-08 12:17:25.642806 MDbrew-2.3.2/MDbrew/main/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     5374 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/brewery.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-08 12:17:25.643835 MDbrew-2.3.2/MDbrew/main/filetype/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/filetype/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)      940 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/filetype/gro.py
+-rw-r--r--   0 minu       (501) staff       (20)      860 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/filetype/lmps.py
+-rw-r--r--   0 minu       (501) staff       (20)      777 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/filetype/pdb.py
+-rw-r--r--   0 minu       (501) staff       (20)     4294 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/filetype/trr.py
+-rw-r--r--   0 minu       (501) staff       (20)     1370 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/filetype/vasp.py
+-rw-r--r--   0 minu       (501) staff       (20)      486 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/filetype/xyz.py
+-rw-r--r--   0 minu       (501) staff       (20)     1163 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/opener.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-08 12:17:25.644563 MDbrew-2.3.2/MDbrew/tool/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/tool/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     3618 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/tool/colorfont.py
+-rw-r--r--   0 minu       (501) staff       (20)     1578 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/tool/decorator.py
+-rw-r--r--   0 minu       (501) staff       (20)      756 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/tool/doctor.py
+-rw-r--r--   0 minu       (501) staff       (20)      619 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/tool/spacer.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-08 12:17:25.641566 MDbrew-2.3.2/MDbrew.egg-info/
+-rw-r--r--   0 minu       (501) staff       (20)      340 2023-05-08 12:17:25.000000 MDbrew-2.3.2/MDbrew.egg-info/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)      740 2023-05-08 12:17:25.000000 MDbrew-2.3.2/MDbrew.egg-info/SOURCES.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-08 12:17:25.000000 MDbrew-2.3.2/MDbrew.egg-info/dependency_links.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-08 12:17:25.000000 MDbrew-2.3.2/MDbrew.egg-info/not-zip-safe
+-rw-r--r--   0 minu       (501) staff       (20)        7 2023-05-08 12:17:25.000000 MDbrew-2.3.2/MDbrew.egg-info/top_level.txt
+-rw-r--r--   0 minu       (501) staff       (20)      340 2023-05-08 12:17:25.644803 MDbrew-2.3.2/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)       62 2023-05-07 05:40:59.000000 MDbrew-2.3.2/requirement.txt
+-rw-r--r--   0 minu       (501) staff       (20)       79 2023-05-08 12:17:25.645061 MDbrew-2.3.2/setup.cfg
+-rw-r--r--   0 minu       (501) staff       (20)      664 2023-05-08 12:16:46.000000 MDbrew-2.3.2/setup.py
```

### Comparing `MDbrew-2.3.1/MDbrew/analysis/msd.py` & `MDbrew-2.3.2/MDbrew/analysis/msd.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.1/MDbrew/analysis/rdf.py` & `MDbrew-2.3.2/MDbrew/analysis/rdf.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.1/MDbrew/application/brewcp2k.py` & `MDbrew-2.3.2/MDbrew/application/brewcp2k.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,20 +70,24 @@
         print(sep_line)
         return f"\t @CopyRight by  {color.font_blue}minu928@snu.ac.kr{color.reset}\n"
 
     def __error__(self):
         F_energy = len(self._energy_list)
         F_stress = len(self._stress_list) / 3
         F_coords = len(self._coord_list)
-        assert (
-            F_energy == F_stress == F_coords
-        ), f"Frame of Energy {F_energy}, Frame of Stress {F_stress} , Frame of Coords {F_coords}"
         self._num_frame = F_energy
         self._num_atom = len(self._force_list) / F_energy
 
+    def delete(self, idx):
+        self._cell_list = np.delete(self._cell_list, idx)
+        self._force_list = np.delete(self._force_list, idx)
+        self._energy_list = np.delete(self._energy_list, idx)
+        self._virial_list = np.delete(self._virial_list, idx)
+        print(f"DELETE : {idx} is deleted")
+
     @color_print(name=printing_option["save"])
     def save_data(self, folder: str = "./", mode: str = "dpdata"):
         folder = folder if folder[-1] == "/" else folder + "/"
         data_path = os.path.join(folder, "set.000")
         if not os.path.exists(data_path):
             os.makedirs(data_path)
         mode_list = ("dpdata", "raw")
@@ -106,25 +110,27 @@
             np.save(virial_path, self.virials)
             np.save(force_path, self.forces)
             np.save(coord_path, self.coords)
         np.savetxt(folder + "type.raw", self.types, fmt="%d")
         np.savetxt(folder + "type_map.raw", self._type_map, fmt="%s")
 
     def _brew_xyzfile(self, xyz_file):
-        brewery = Brewery(path=xyz_file, fmt="xyz")
+        brewery = Brewery(trj_file=xyz_file)
         line_range = tqdm(
             brewery.frange(),
             desc=f"[ {color.font_cyan}BREW{color.reset} ]  #{color.font_green}XYZ{color.reset} ",
             **self.tqmd_option,
         )
         self._coord_list = np.array([brewery.coords for _ in line_range])
         self.is_contain_coord = True
 
     def _brew_logfile(self, log_file):
         # BASE for brewing
+        restart_keyword = "RESTART INFORMATION"
+        self._restart_list = []
         ## CELL
         cell_keyword = "CELL| Vector "
         self.is_contain_cell = False
         self._cell_list = []
         ## STRESS
         stress_keyword = "STRESS| Analytical stress"
         self.is_contain_stress = False
@@ -151,14 +157,16 @@
                 tqdm(
                     f,
                     **self.tqmd_option,
                     desc=f"[ {color.font_cyan}BREW{color.reset} ]  #{color.font_green}LOG{color.reset} ",
                 )
             )
             for idx, line in line_range:
+                if restart_keyword in line:
+                    self._restart_list.append(len(self._energy_list))
                 # CELL
                 if len(self._cell_list) < 3:
                     if cell_keyword in line:
                         self.is_contain_cell = True
                         self._cell_list.append(line.split()[4:7])
                         continue
                 # STRESS
```

### Comparing `MDbrew-2.3.1/MDbrew/main/brewery.py` & `MDbrew-2.3.2/MDbrew/main/brewery.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         sep_line = "=" * LINE_WIDTH
         print("")
         print(sep_line)
         print("||" + " " * 23 + " INFO " + " " * 27 + "||")
         print(sep_line)
         print(f"\t[  ATOM  ]:  KIND  ->   {tuple(self.atom_kind)}")
         print(f"\t[  ATOM  ]:  NUMB  ->   {tuple(self.atom_info[-1])}")
-        print(f"\t[   BOX  ]:  SHAPE ->   {np.array(self.box_size).shape}")
+        print(f"\t[  BOX   ]:  SHAPE ->   {np.array(self.box_size).shape}")
         print(f"\t[ COORDS ]:  SHAPE ->   {self.coords.shape}")
         print(f"\t[ FRAMES ]:   NOW  ->   {self.frame:4d}")
         print(sep_line)
         return f"\t    @CopyRight by  {color.font_blue}minu928@snu.ac.kr{color.reset}\n"
 
     @property
     def box_size(self):
@@ -80,17 +80,18 @@
         return self._opener.frame
 
     @property
     def next_frame(self):
         self._opener.next_frame()
 
     @color_print_verbose(name=__print_option__["b_brewing"])
-    def brew(self, cols: list[str], dtype: str = "float32", verbose: bool = True):
+    def brew(self, cols: list[str] = None, what: str = None, dtype: str = "float32", verbose: bool = True):
         data = pd.DataFrame(data=self.data, columns=self.columns)
         data = data.query(self._what) if self._what is not None else data
+        data = data.query(what) if what is not None else data
         data = data.loc[:, cols] if cols is not None else data
         return data.to_numpy().astype(dtype=dtype)
 
     def reset(self):
         self._opener.reset()
 
     def order(self, what: str = None):
@@ -121,27 +122,27 @@
         return fmt
 
     def _check_path(self, path, **kwrgs):
         path = os.path.join(os.getcwd(), path)
         assert os.path.isfile(path=path), f"Check your path || not {path}"
         return path
 
-    def frange(self, __start: int = 0, __end: int = None, __step: int = 1):
+    def frange(self, start: int = 0, end: int = None, step: int = 1):
         self.reset()
-        assert __start >= 0, ValueError("Frame start idx should be positive")
+        assert start >= 0, ValueError("Frame start idx should be positive")
         i = 0
-        while i < __start:
+        while i < start:
             max_frame = i
             try:
                 self.next_frame
                 i += 1
             except:
                 raise ValueError(f"start idx should be lower than {max_frame}")
         while True:
             try:
-                if self.frame == __end:
+                if self.frame == end:
                     break
-                if not (self.frame - __start) % __step:
+                if not (self.frame - start) % step:
                     yield self.frame
                 self.next_frame
             except:
                 break
```

### Comparing `MDbrew-2.3.1/MDbrew/main/filetype/lmps.py` & `MDbrew-2.3.2/MDbrew/main/filetype/lmps.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.1/MDbrew/main/filetype/pdb.py` & `MDbrew-2.3.2/MDbrew/main/filetype/pdb.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.1/MDbrew/main/filetype/vasp.py` & `MDbrew-2.3.2/MDbrew/main/filetype/vasp.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.1/MDbrew/main/opener.py` & `MDbrew-2.3.2/MDbrew/main/opener.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.1/MDbrew/tool/colorfont.py` & `MDbrew-2.3.2/MDbrew/tool/colorfont.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.1/MDbrew/tool/decorator.py` & `MDbrew-2.3.2/MDbrew/tool/decorator.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.1/MDbrew/tool/doctor.py` & `MDbrew-2.3.2/MDbrew/tool/doctor.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.1/MDbrew/tool/spacer.py` & `MDbrew-2.3.2/MDbrew/tool/spacer.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.1/MDbrew.egg-info/SOURCES.txt` & `MDbrew-2.3.2/MDbrew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.1/setup.py` & `MDbrew-2.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MDbrew",
-    version="2.3.1",
+    version="2.3.2",
     author="Knu",
     author_email="minu928@snu.ac.kr",
     url="https://github.com/MyKnu/MDbrew",
-    download_url="https://github.com/MyKnu/MDbrew/install_file/MDbrew-2.3.1.tar.gz",
+    download_url="https://github.com/MyKnu/MDbrew/install_file/MDbrew-2.3.2.tar.gz",
     install_requies=[
         "numpy>=1.0.0",
         "pandas>=1.0.0",
         "matplotlib>=1.0.0",
         "tqdm>=1.0.0",
     ],
     description="Postprocessing tools for the MD simulation results (ex. lammps)",
     packages=find_packages(),
-    keywords=["MD", "LAMMPS"],
+    keywords=["MD", "LAMMPS", "GROMACS"],
     python_requires=">=3.6",
     package_data={"": ["*"]},
     zip_safe=False,
 )
```

