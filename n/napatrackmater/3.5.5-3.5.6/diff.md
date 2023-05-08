# Comparing `tmp/napatrackmater-3.5.5.tar.gz` & `tmp/napatrackmater-3.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-ad0urwp9/napatrackmater-3.5.5.tar", last modified: Mon May  8 11:27:37 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-jtrxwopp/napatrackmater-3.5.6.tar", last modified: Mon May  8 15:28:59 2023, max compression
```

## Comparing `napatrackmater-3.5.5.tar` & `napatrackmater-3.5.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-08 11:27:37.591304 napatrackmater-3.5.5/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.5.5/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-08 11:27:37.586853 napatrackmater-3.5.5/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.5.5/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-08 11:27:37.415099 napatrackmater-3.5.5/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-02-11 18:25:27.000000 napatrackmater-3.5.5/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      869 2023-02-26 10:31:22.000000 napatrackmater-3.5.5/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   109623 2023-05-08 11:23:53.000000 napatrackmater-3.5.5/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.5.5/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.5.5/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13523 2023-05-04 16:47:51.000000 napatrackmater-3.5.5/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.5.5/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.5.5/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6013 2023-02-25 15:35:08.000000 napatrackmater-3.5.5/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-05-08 11:24:00.000000 napatrackmater-3.5.5/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-08 11:27:37.560412 napatrackmater-3.5.5/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-08 11:27:36.000000 napatrackmater-3.5.5/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-05-08 11:27:37.000000 napatrackmater-3.5.5/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-05-08 11:27:36.000000 napatrackmater-3.5.5/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-05-08 11:27:36.000000 napatrackmater-3.5.5/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-05-08 11:27:36.000000 napatrackmater-3.5.5/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-05-08 11:27:36.000000 napatrackmater-3.5.5/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-05-08 11:27:37.592305 napatrackmater-3.5.5/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-03-14 22:29:07.000000 napatrackmater-3.5.5/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-08 15:28:59.079046 napatrackmater-3.5.6/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.5.6/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-08 15:28:59.073537 napatrackmater-3.5.6/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.5.6/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-08 15:28:58.831048 napatrackmater-3.5.6/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-02-11 18:25:27.000000 napatrackmater-3.5.6/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      869 2023-02-26 10:31:22.000000 napatrackmater-3.5.6/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   109648 2023-05-08 15:27:57.000000 napatrackmater-3.5.6/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.5.6/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.5.6/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13523 2023-05-04 16:47:51.000000 napatrackmater-3.5.6/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.5.6/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.5.6/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6013 2023-02-25 15:35:08.000000 napatrackmater-3.5.6/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-05-08 15:28:07.000000 napatrackmater-3.5.6/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-08 15:28:59.033544 napatrackmater-3.5.6/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-08 15:28:58.000000 napatrackmater-3.5.6/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-05-08 15:28:58.000000 napatrackmater-3.5.6/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-05-08 15:28:58.000000 napatrackmater-3.5.6/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-05-08 15:28:58.000000 napatrackmater-3.5.6/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-05-08 15:28:58.000000 napatrackmater-3.5.6/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-05-08 15:28:58.000000 napatrackmater-3.5.6/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-05-08 15:28:59.081046 napatrackmater-3.5.6/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-03-14 22:29:07.000000 napatrackmater-3.5.6/setup.py
```

### Comparing `napatrackmater-3.5.5/LICENSE` & `napatrackmater-3.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.5/PKG-INFO` & `napatrackmater-3.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.5.5
+Version: 3.5.6
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.5.5/README.md` & `napatrackmater-3.5.6/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.5/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.5.6/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.5/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.5.6/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.5/napatrackmater/Trackmate.py` & `napatrackmater-3.5.6/napatrackmater/Trackmate.py`

 * *Files 0% similar despite different names*

```diff
@@ -5031,1822 +5031,1823 @@
 00013a60: 5d5b 305d 202a 2073 656c 662e 7a63 616c  ][0] * self.zcal
 00013a70: 6962 7261 7469 6f6e 2c20 6365 6e74 726f  ibration, centro
 00013a80: 6964 735b 696e 6465 785d 5b31 5d2a 7365  ids[index][1]*se
 00013a90: 6c66 2e79 6361 6c69 6272 6174 696f 6e2c  lf.ycalibration,
 00013aa0: 2063 656e 7472 6f69 6473 5b69 6e64 6578   centroids[index
 00013ab0: 5d5b 325d 2a73 656c 662e 7863 616c 6962  ][2]*self.xcalib
 00013ac0: 7261 7469 6f6e 290d 0a20 2020 2020 2020  ration)..       
-00013ad0: 2020 2020 2051 5541 4c49 5459 203d 2076       QUALITY = v
-00013ae0: 6f6c 756d 655b 696e 6465 785d 0d0a 2020  olume[index]..  
-00013af0: 2020 2020 2020 2020 2020 5241 4449 5553            RADIUS
-00013b00: 203d 206d 6174 682e 706f 7728 5155 414c   = math.pow(QUAL
-00013b10: 4954 5920 2a20 7365 6c66 2e78 6361 6c69  ITY * self.xcali
-00013b20: 6272 6174 696f 6e20 2a20 7365 6c66 2e79  bration * self.y
-00013b30: 6361 6c69 6272 6174 696f 6e20 2a20 7365  calibration * se
-00013b40: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
-00013b50: 2031 2e30 2f33 2e30 2920 0d0a 0d0a 2020   1.0/3.0) ....  
-00013b60: 2020 2020 2020 2020 2020 6469 7374 616e            distan
-00013b70: 6365 5f63 656c 6c5f 6d61 736b 2c20 6d61  ce_cell_mask, ma
-00013b80: 736b 6365 6e74 726f 6964 203d 2073 656c  skcentroid = sel
-00013b90: 662e 5f67 6574 5f62 6f75 6e64 6172 795f  f._get_boundary_
-00013ba0: 6469 7374 2866 7261 6d65 2c20 6c6f 6361  dist(frame, loca
-00013bb0: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
-00013bc0: 2020 2069 6620 6469 7374 203c 3d20 3220     if dist <= 2 
-00013bd0: 2a20 7665 746f 5f72 6164 6975 733a 0d0a  * veto_radius:..
-00013be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bf0: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-00013c00: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00013c10: 6965 735b 6365 6c6c 5f69 645d 203d 207b  ies[cell_id] = {
-00013c20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013c30: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00013c40: 656c 6c69 645f 6b65 793a 2069 6e74 2863  ellid_key: int(c
-00013c50: 656c 6c5f 6964 292c 200d 0a20 2020 2020  ell_id), ..     
-00013c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c70: 2020 2073 656c 662e 6672 616d 6569 645f     self.frameid_
-00013c80: 6b65 7920 3a20 696e 7428 6672 616d 6529  key : int(frame)
-00013c90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00013ca0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013cb0: 7a70 6f73 6964 5f6b 6579 203a 2066 6c6f  zposid_key : flo
-00013cc0: 6174 2863 656e 7472 6f69 6473 5b69 6e64  at(centroids[ind
-00013cd0: 6578 5d5b 305d 2a20 7365 6c66 2e7a 6361  ex][0]* self.zca
-00013ce0: 6c69 6272 6174 696f 6e29 2c0d 0a20 2020  libration),..   
-00013cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d00: 2020 2020 2073 656c 662e 7970 6f73 6964       self.yposid
-00013d10: 5f6b 6579 203a 2066 6c6f 6174 2863 656e  _key : float(cen
-00013d20: 7472 6f69 6473 5b69 6e64 6578 5d5b 315d  troids[index][1]
-00013d30: 2a20 7365 6c66 2e79 6361 6c69 6272 6174  * self.ycalibrat
-00013d40: 696f 6e29 2c0d 0a20 2020 2020 2020 2020  ion),..         
-00013d50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00013d60: 656c 662e 7870 6f73 6964 5f6b 6579 203a  elf.xposid_key :
-00013d70: 2066 6c6f 6174 2863 656e 7472 6f69 6473   float(centroids
-00013d80: 5b69 6e64 6578 5d5b 325d 2a20 7365 6c66  [index][2]* self
-00013d90: 2e78 6361 6c69 6272 6174 696f 6e29 2c0d  .xcalibration),.
-00013da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013db0: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
-00013dc0: 6163 6b69 645f 6b65 793a 2069 6e74 2874  ackid_key: int(t
-00013dd0: 7261 636b 5f69 6429 2c0d 0a20 2020 2020  rack_id),..     
-00013de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013df0: 2020 2073 656c 662e 746f 7461 6c5f 696e     self.total_in
-00013e00: 7465 6e73 6974 795f 6b65 7920 3a20 2866  tensity_key : (f
-00013e10: 6c6f 6174 2869 6e74 656e 7369 7479 5f74  loat(intensity_t
-00013e20: 6f74 616c 5b69 6e64 6578 5d29 292c 0d0a  otal[index])),..
-00013e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e40: 2020 2020 2020 2020 7365 6c66 2e6d 6561          self.mea
-00013e50: 6e5f 696e 7465 6e73 6974 795f 6b65 7920  n_intensity_key 
-00013e60: 3a20 2866 6c6f 6174 2869 6e74 656e 7369  : (float(intensi
-00013e70: 7479 5f6d 6561 6e5b 696e 6465 785d 2929  ty_mean[index]))
-00013e80: 2c0d 0a0d 0a20 2020 2020 2020 2020 2020  ,....           
-00013e90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00013ea0: 662e 7261 6469 7573 5f6b 6579 203a 2028  f.radius_key : (
-00013eb0: 666c 6f61 7428 5241 4449 5553 2929 2c0d  float(RADIUS)),.
-00013ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013ed0: 2020 2020 2020 2020 2073 656c 662e 7175           self.qu
-00013ee0: 616c 6974 795f 6b65 7920 3a20 2866 6c6f  ality_key : (flo
-00013ef0: 6174 2851 5541 4c49 5459 2929 2c0d 0a20  at(QUALITY)),.. 
-00013f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f10: 2020 2020 2020 2073 656c 662e 6469 7374         self.dist
-00013f20: 616e 6365 5f63 656c 6c5f 6d61 736b 5f6b  ance_cell_mask_k
-00013f30: 6579 3a20 666c 6f61 7428 6469 7374 616e  ey: float(distan
-00013f40: 6365 5f63 656c 6c5f 6d61 736b 292c 0d0a  ce_cell_mask),..
-00013f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f60: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
-00013f70: 6b63 656e 7472 6f69 645f 7a5f 6b65 793a  kcentroid_z_key:
-00013f80: 2066 6c6f 6174 286d 6173 6b63 656e 7472   float(maskcentr
-00013f90: 6f69 645b 305d 292c 0d0a 2020 2020 2020  oid[0]),..      
-00013fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fb0: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
-00013fc0: 6f69 645f 795f 6b65 793a 2066 6c6f 6174  oid_y_key: float
-00013fd0: 286d 6173 6b63 656e 7472 6f69 645b 315d  (maskcentroid[1]
-00013fe0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00013ff0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014000: 2e6d 6173 6b63 656e 7472 6f69 645f 785f  .maskcentroid_x_
-00014010: 6b65 793a 2066 6c6f 6174 286d 6173 6b63  key: float(maskc
-00014020: 656e 7472 6f69 645b 325d 2920 0d0a 0d0a  entroid[2]) ....
-00014030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014040: 7d0d 0a20 2020 2020 2020 2020 2020 2065  }..            e
-00014050: 6c69 6620 6365 6c6c 5f69 6420 696e 2073  lif cell_id in s
-00014060: 656c 662e 6564 6765 5f73 6f75 7263 655f  elf.edge_source_
-00014070: 6c6f 6f6b 7570 2e6b 6579 7328 293a 0d0a  lookup.keys():..
-00014080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014090: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000140a0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000140b0: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
-000140c0: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
-000140d0: 6c6c 5f69 645d 203d 2073 656c 662e 756e  ll_id] = self.un
-000140e0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000140f0: 7469 6573 5b63 656c 6c5f 6964 5d0d 0a0d  ties[cell_id]...
-00014100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014110: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
-00014120: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
-00014130: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
-00014140: 5d2e 7570 6461 7465 287b 7365 6c66 2e74  ].update({self.t
-00014150: 6f74 616c 5f69 6e74 656e 7369 7479 5f6b  otal_intensity_k
-00014160: 6579 3a20 2d31 3030 7d29 0d0a 2020 2020  ey: -100})..    
-00014170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014180: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-00014190: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000141a0: 6965 735b 6365 6c6c 5f69 645d 2e75 7064  ies[cell_id].upd
-000141b0: 6174 6528 7b73 656c 662e 6d65 616e 5f69  ate({self.mean_i
-000141c0: 6e74 656e 7369 7479 5f6b 6579 3a20 2d31  ntensity_key: -1
-000141d0: 3030 7d29 0d0a 2020 2020 2020 2020 2020  00})..          
-000141e0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000141f0: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
-00014200: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
-00014210: 6c6c 5f69 645d 2e75 7064 6174 6528 7b73  ll_id].update({s
-00014220: 656c 662e 7261 6469 7573 5f6b 6579 3a20  elf.radius_key: 
-00014230: 2d31 3030 7d29 0d0a 2020 2020 2020 2020  -100})..        
-00014240: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014250: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
-00014260: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00014270: 6365 6c6c 5f69 645d 2e75 7064 6174 6528  cell_id].update(
-00014280: 7b73 656c 662e 7175 616c 6974 795f 6b65  {self.quality_ke
-00014290: 793a 202d 3130 307d 290d 0a0d 0a0d 0a20  y: -100})...... 
-000142a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142c0: 0d0a 2020 2020 6465 6620 5f64 6963 745f  ..    def _dict_
-000142d0: 7570 6461 7465 2873 656c 662c 2075 6e69  update(self, uni
-000142e0: 7175 655f 7472 6163 6b6c 6574 5f69 6473  que_tracklet_ids
-000142f0: 3a20 4c69 7374 2c20 2063 656c 6c5f 6964  : List,  cell_id
-00014300: 3a20 696e 742c 2074 7261 636b 5f69 643a  : int, track_id:
-00014310: 2069 6e74 2c20 736f 7572 6365 5f69 643a   int, source_id:
-00014320: 2069 6e74 2c20 7461 7267 6574 5f69 643a   int, target_id:
-00014330: 2069 6e74 293a 0d0a 0d0a 200d 0a20 2020   int):.... ..   
-00014340: 2020 2020 2067 656e 6572 6174 696f 6e5f       generation_
-00014350: 6964 203d 2073 656c 662e 6765 6e65 7261  id = self.genera
-00014360: 7469 6f6e 5f64 6963 745b 6365 6c6c 5f69  tion_dict[cell_i
-00014370: 645d 0d0a 2020 2020 2020 2020 7472 6163  d]..        trac
-00014380: 6b6c 6574 5f69 6420 3d20 7365 6c66 2e74  klet_id = self.t
-00014390: 7261 636b 6c65 745f 6469 6374 5b63 656c  racklet_dict[cel
-000143a0: 6c5f 6964 5d0d 0a0d 0a20 2020 2020 2020  l_id]....       
-000143b0: 2075 6e69 7175 655f 6964 203d 2073 7472   unique_id = str
-000143c0: 2874 7261 636b 5f69 6429 202b 2073 7472  (track_id) + str
-000143d0: 2873 656c 662e 6d61 785f 7472 6163 6b5f  (self.max_track_
-000143e0: 6964 2920 2b20 7374 7228 6765 6e65 7261  id) + str(genera
-000143f0: 7469 6f6e 5f69 6429 202b 2073 7472 2874  tion_id) + str(t
-00014400: 7261 636b 6c65 745f 6964 290d 0a20 2020  racklet_id)..   
-00014410: 2020 2020 200d 0a20 2020 2020 2020 2076       ..        v
-00014420: 6563 5f6d 6173 6b20 3d20 5b66 6c6f 6174  ec_mask = [float
-00014430: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00014440: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00014450: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-00014460: 6d61 736b 6365 6e74 726f 6964 5f78 5f6b  maskcentroid_x_k
-00014470: 6579 5d29 2c20 666c 6f61 7428 7365 6c66  ey]), float(self
-00014480: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00014490: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-000144a0: 5f69 6429 5d5b 7365 6c66 2e6d 6173 6b63  _id)][self.maskc
-000144b0: 656e 7472 6f69 645f 795f 6b65 795d 292c  entroid_y_key]),
-000144c0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-000144d0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000144e0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-000144f0: 5b73 656c 662e 6d61 736b 6365 6e74 726f  [self.maskcentro
-00014500: 6964 5f7a 5f6b 6579 5d29 205d 0d0a 0d0a  id_z_key]) ]....
-00014510: 2020 2020 2020 2020 7665 635f 6365 6c6c          vec_cell
-00014520: 203d 205b 666c 6f61 7428 7365 6c66 2e75   = [float(self.u
-00014530: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014540: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014550: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
-00014560: 6b65 795d 2920 2c20 0d0a 2020 2020 2020  key]) , ..      
-00014570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014580: 2020 2020 2020 666c 6f61 7428 7365 6c66        float(self
-00014590: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000145a0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-000145b0: 5f69 6429 5d5b 7365 6c66 2e79 706f 7369  _id)][self.yposi
-000145c0: 645f 6b65 795d 292c 200d 0a20 2020 2020  d_key]), ..     
-000145d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145e0: 2020 2020 2020 2066 6c6f 6174 2873 656c         float(sel
-000145f0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014600: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00014610: 6c5f 6964 295d 5b73 656c 662e 7a70 6f73  l_id)][self.zpos
-00014620: 6964 5f6b 6579 5d29 5d0d 0a0d 0a20 2020  id_key])]....   
-00014630: 2020 2020 2061 6e67 6c65 203d 2061 6e67       angle = ang
-00014640: 756c 6172 5f63 6861 6e67 6528 7665 635f  ular_change(vec_
-00014650: 6d61 736b 2c20 7665 635f 6365 6c6c 290d  mask, vec_cell).
-00014660: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-00014670: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00014680: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00014690: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-000146a0: 662e 7261 6469 616c 5f61 6e67 6c65 5f6b  f.radial_angle_k
-000146b0: 6579 203a 2061 6e67 6c65 7d29 2020 2020  ey : angle})    
-000146c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146d0: 0d0a 0d0a 2020 2020 2020 2020 756e 6971  ....        uniq
-000146e0: 7565 5f74 7261 636b 6c65 745f 6964 732e  ue_tracklet_ids.
-000146f0: 6170 7065 6e64 2873 7472 2875 6e69 7175  append(str(uniqu
-00014700: 655f 6964 2929 0d0a 2020 2020 2020 2020  e_id))..        
-00014710: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00014720: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00014730: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00014740: 287b 7365 6c66 2e63 6c75 7374 6572 636c  ({self.clustercl
-00014750: 6173 735f 6b65 7920 3a20 2d31 3030 7d29  ass_key : -100})
-00014760: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-00014770: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014780: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014790: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-000147a0: 2e63 6c75 7374 6572 7363 6f72 655f 6b65  .clusterscore_ke
-000147b0: 7920 3a20 307d 290d 0a20 2020 2020 2020  y : 0})..       
-000147c0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-000147d0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-000147e0: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-000147f0: 6528 7b73 656c 662e 756e 6971 7565 6964  e({self.uniqueid
-00014800: 5f6b 6579 203a 2073 7472 2875 6e69 7175  _key : str(uniqu
-00014810: 655f 6964 297d 290d 0a20 2020 2020 2020  e_id)})..       
-00014820: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00014830: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00014840: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00014850: 6528 7b73 656c 662e 7472 6163 6b6c 6574  e({self.tracklet
-00014860: 6964 5f6b 6579 203a 2073 7472 2874 7261  id_key : str(tra
-00014870: 636b 6c65 745f 6964 297d 2920 0d0a 2020  cklet_id)}) ..  
-00014880: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00014890: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000148a0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-000148b0: 7570 6461 7465 287b 7365 6c66 2e67 656e  update({self.gen
-000148c0: 6572 6174 696f 6e69 645f 6b65 7920 3a20  erationid_key : 
-000148d0: 7374 7228 6765 6e65 7261 7469 6f6e 5f69  str(generation_i
-000148e0: 6429 7d29 200d 0a20 2020 2020 2020 2073  d)}) ..        s
-000148f0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014900: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00014910: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00014920: 7b73 656c 662e 7472 6163 6b69 645f 6b65  {self.trackid_ke
-00014930: 7920 3a20 7374 7228 7472 6163 6b5f 6964  y : str(track_id
-00014940: 297d 290d 0a20 2020 2020 2020 2073 656c  )})..        sel
-00014950: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014960: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00014970: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00014980: 656c 662e 6d6f 7469 6f6e 5f61 6e67 6c65  elf.motion_angle
-00014990: 5f6b 6579 203a 2030 2e30 7d29 0d0a 2020  _key : 0.0})..  
-000149a0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000149b0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000149c0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-000149d0: 7570 6461 7465 287b 7365 6c66 2e73 7065  update({self.spe
-000149e0: 6564 5f6b 6579 203a 2030 2e30 7d29 0d0a  ed_key : 0.0})..
-000149f0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00014a00: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014a10: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00014a20: 5d2e 7570 6461 7465 287b 7365 6c66 2e61  ].update({self.a
-00014a30: 6363 656c 6572 6174 696f 6e5f 6b65 7920  cceleration_key 
-00014a40: 3a20 302e 307d 290d 0a20 2020 2020 2020  : 0.0})..       
-00014a50: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00014a60: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00014a70: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00014a80: 6528 7b73 656c 662e 6563 6365 6e74 7269  e({self.eccentri
-00014a90: 6369 7479 5f63 6f6d 705f 6669 7273 746b  city_comp_firstk
-00014aa0: 6579 203a 202d 3130 307d 290d 0a20 2020  ey : -100})..   
-00014ab0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00014ac0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00014ad0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00014ae0: 7064 6174 6528 7b73 656c 662e 6563 6365  pdate({self.ecce
-00014af0: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
-00014b00: 636f 6e64 6b65 7920 3a20 2d31 3030 7d29  condkey : -100})
-00014b10: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-00014b20: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014b30: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014b40: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00014b50: 2e73 7572 6661 6365 5f61 7265 615f 6b65  .surface_area_ke
-00014b60: 7920 3a20 2d31 3030 7d29 0d0a 2020 2020  y : -100})..    
-00014b70: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00014b80: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00014b90: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-00014ba0: 6461 7465 287b 7365 6c66 2e63 656c 6c61  date({self.cella
-00014bb0: 7869 735f 6d61 736b 5f6b 6579 203a 202d  xis_mask_key : -
-00014bc0: 3130 307d 290d 0a0d 0a20 2020 2020 2020  100})....       
-00014bd0: 2069 6620 736f 7572 6365 5f69 6420 6973   if source_id is
-00014be0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00014bf0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00014c00: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014c10: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00014c20: 5d2e 7570 6461 7465 287b 7365 6c66 2e62  ].update({self.b
-00014c30: 6566 6f72 6569 645f 6b65 7920 3a20 696e  eforeid_key : in
-00014c40: 7428 736f 7572 6365 5f69 6429 7d29 0d0a  t(source_id)})..
-00014c50: 2020 2020 2020 2020 2020 2020 7665 635f              vec_
-00014c60: 3120 3d20 5b66 6c6f 6174 2873 656c 662e  1 = [float(self.
-00014c70: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00014c80: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00014c90: 6964 295d 5b73 656c 662e 7870 6f73 6964  id)][self.xposid
-00014ca0: 5f6b 6579 5d29 202d 2066 6c6f 6174 2873  _key]) - float(s
-00014cb0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014cc0: 7072 6f70 6572 7469 6573 5b69 6e74 2873  properties[int(s
-00014cd0: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
-00014ce0: 7870 6f73 6964 5f6b 6579 5d29 2c20 0d0a  xposid_key]), ..
-00014cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d00: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
-00014d10: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-00014d20: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00014d30: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
-00014d40: 2e79 706f 7369 645f 6b65 795d 2920 2d20  .yposid_key]) - 
-00014d50: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00014d60: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00014d70: 735b 696e 7428 736f 7572 6365 5f69 6429  s[int(source_id)
-00014d80: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
-00014d90: 795d 292c 200d 0a20 2020 2020 2020 2020  y]), ..         
-00014da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014db0: 2020 2066 6c6f 6174 2873 656c 662e 756e     float(self.un
-00014dc0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014dd0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00014de0: 295d 5b73 656c 662e 7a70 6f73 6964 5f6b  )][self.zposid_k
-00014df0: 6579 5d29 202d 2020 666c 6f61 7428 7365  ey]) -  float(se
-00014e00: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014e10: 726f 7065 7274 6965 735b 696e 7428 736f  roperties[int(so
-00014e20: 7572 6365 5f69 6429 5d5b 7365 6c66 2e7a  urce_id)][self.z
-00014e30: 706f 7369 645f 6b65 795d 295d 0d0a 2020  posid_key])]..  
-00014e40: 2020 2020 2020 2020 2020 7370 6565 6420            speed 
-00014e50: 3d20 6e70 2e73 7172 7428 6e70 2e64 6f74  = np.sqrt(np.dot
-00014e60: 2876 6563 5f31 2c20 7665 635f 3129 292f  (vec_1, vec_1))/
-00014e70: 7365 6c66 2e74 6361 6c69 6272 6174 696f  self.tcalibratio
-00014e80: 6e0d 0a20 2020 2020 2020 2020 2020 2073  n..            s
-00014e90: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014ea0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00014eb0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00014ec0: 7b73 656c 662e 7370 6565 645f 6b65 7920  {self.speed_key 
-00014ed0: 3a20 7370 6565 647d 290d 0a0d 0a20 2020  : speed})....   
-00014ee0: 2020 2020 2020 2020 206d 6f74 696f 6e5f           motion_
-00014ef0: 616e 676c 6520 3d20 616e 6775 6c61 725f  angle = angular_
-00014f00: 6368 616e 6765 2876 6563 5f6d 6173 6b2c  change(vec_mask,
-00014f10: 2076 6563 5f31 290d 0a0d 0a20 2020 2020   vec_1)....     
-00014f20: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00014f30: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00014f40: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00014f50: 2e75 7064 6174 6528 7b73 656c 662e 6d6f  .update({self.mo
-00014f60: 7469 6f6e 5f61 6e67 6c65 5f6b 6579 203a  tion_angle_key :
-00014f70: 206d 6f74 696f 6e5f 616e 676c 657d 2920   motion_angle}) 
-00014f80: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00014f90: 6966 2073 6f75 7263 655f 6964 2069 6e20  if source_id in 
-00014fa0: 7365 6c66 2e65 6467 655f 736f 7572 6365  self.edge_source
-00014fb0: 5f6c 6f6f 6b75 703a 0d0a 2020 2020 2020  _lookup:..      
-00014fc0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00014fd0: 655f 736f 7572 6365 5f69 6420 3d20 7365  e_source_id = se
-00014fe0: 6c66 2e65 6467 655f 736f 7572 6365 5f6c  lf.edge_source_l
-00014ff0: 6f6f 6b75 705b 736f 7572 6365 5f69 645d  ookup[source_id]
-00015000: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015010: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00015020: 2020 2020 2020 2020 2020 2020 7665 635f              vec_
-00015030: 3220 3d20 5b66 6c6f 6174 2873 656c 662e  2 = [float(self.
-00015040: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015050: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00015060: 6964 295d 5b73 656c 662e 7870 6f73 6964  id)][self.xposid
-00015070: 5f6b 6579 5d29 202d 2032 202a 2066 6c6f  _key]) - 2 * flo
-00015080: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00015090: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-000150a0: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
-000150b0: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
-000150c0: 202b 2066 6c6f 6174 2873 656c 662e 756e   + float(self.un
-000150d0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000150e0: 7469 6573 5b69 6e74 2870 7265 5f73 6f75  ties[int(pre_sou
-000150f0: 7263 655f 6964 295d 5b73 656c 662e 7870  rce_id)][self.xp
-00015100: 6f73 6964 5f6b 6579 5d29 2c20 0d0a 2020  osid_key]), ..  
-00015110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015120: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
-00015130: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00015140: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00015150: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e79  cell_id)][self.y
-00015160: 706f 7369 645f 6b65 795d 2920 2d20 3220  posid_key]) - 2 
-00015170: 2a20 666c 6f61 7428 7365 6c66 2e75 6e69  * float(self.uni
-00015180: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00015190: 6965 735b 696e 7428 736f 7572 6365 5f69  ies[int(source_i
-000151a0: 6429 5d5b 7365 6c66 2e79 706f 7369 645f  d)][self.yposid_
-000151b0: 6b65 795d 2920 2b20 666c 6f61 7428 7365  key]) + float(se
-000151c0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000151d0: 726f 7065 7274 6965 735b 696e 7428 7072  roperties[int(pr
-000151e0: 655f 736f 7572 6365 5f69 6429 5d5b 7365  e_source_id)][se
-000151f0: 6c66 2e79 706f 7369 645f 6b65 795d 292c  lf.yposid_key]),
-00015200: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00015210: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00015220: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-00015230: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015240: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-00015250: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
-00015260: 202d 2020 3220 2a20 666c 6f61 7428 7365   -  2 * float(se
-00015270: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00015280: 726f 7065 7274 6965 735b 696e 7428 736f  roperties[int(so
-00015290: 7572 6365 5f69 6429 5d5b 7365 6c66 2e7a  urce_id)][self.z
-000152a0: 706f 7369 645f 6b65 795d 2920 2b20 666c  posid_key]) + fl
-000152b0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-000152c0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000152d0: 696e 7428 7072 655f 736f 7572 6365 5f69  int(pre_source_i
-000152e0: 6429 5d5b 7365 6c66 2e7a 706f 7369 645f  d)][self.zposid_
-000152f0: 6b65 795d 295d 0d0a 2020 2020 2020 2020  key])]..        
-00015300: 2020 2020 2020 2020 2020 2020 6163 6320              acc 
-00015310: 3d20 6e70 2e73 7172 7428 6e70 2e64 6f74  = np.sqrt(np.dot
-00015320: 2876 6563 5f32 2c20 7665 635f 3229 292f  (vec_2, vec_2))/
-00015330: 7365 6c66 2e74 6361 6c69 6272 6174 696f  self.tcalibratio
-00015340: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00015350: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00015360: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015370: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00015380: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00015390: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-000153a0: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
-000153b0: 5f6b 6579 203a 2061 6363 7d29 0d0a 2020  _key : acc})..  
-000153c0: 2020 2020 2020 656c 6966 2073 6f75 7263        elif sourc
-000153d0: 655f 6964 2069 7320 4e6f 6e65 3a0d 0a20  e_id is None:.. 
-000153e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000153f0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015400: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00015410: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00015420: 662e 6265 666f 7265 6964 5f6b 6579 203a  f.beforeid_key :
-00015430: 204e 6f6e 657d 2920 0d0a 2020 2020 2020   None}) ..      
-00015440: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-00015450: 2020 6966 2074 6172 6765 745f 6964 2069    if target_id i
-00015460: 7320 6e6f 7420 4e6f 6e65 3a20 2020 2020  s not None:     
-00015470: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00015480: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00015490: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000154a0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-000154b0: 287b 7365 6c66 2e61 6674 6572 6964 5f6b  ({self.afterid_k
-000154c0: 6579 203a 2069 6e74 2874 6172 6765 745f  ey : int(target_
-000154d0: 6964 297d 2920 0d0a 2020 2020 2020 2020  id)}) ..        
-000154e0: 656c 6966 2074 6172 6765 745f 6964 2069  elif target_id i
-000154f0: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00015500: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00015510: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015520: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00015530: 7064 6174 6528 7b73 656c 662e 6166 7465  pdate({self.afte
-00015540: 7269 645f 6b65 7920 3a20 4e6f 6e65 7d29  rid_key : None})
-00015550: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-00015560: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
-00015570: 636f 6e64 5f63 6861 6e6e 656c 5f75 7064  cond_channel_upd
-00015580: 6174 6528 6365 6c6c 5f69 642c 2074 7261  ate(cell_id, tra
-00015590: 636b 5f69 6429 2020 2020 0d0a 0d0a 0d0a  ck_id)    ......
-000155a0: 2020 2020 6465 6620 5f74 656d 706f 7261      def _tempora
-000155b0: 6c5f 706c 6f74 735f 7472 6163 6b6d 6174  l_plots_trackmat
-000155c0: 6528 7365 6c66 293a 0d0a 2020 2020 0d0a  e(self):..    ..
-000155d0: 2020 2020 0d0a 2020 2020 0d0a 2020 2020      ..    ..    
-000155e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000155f0: 2e41 7474 7220 3d20 7b7d 0d0a 2020 2020  .Attr = {}..    
-00015600: 2020 2020 2020 2020 2020 2020 7374 6172              star
-00015610: 7474 696d 6520 3d20 696e 7428 6d69 6e28  ttime = int(min(
-00015620: 7365 6c66 2e41 6c6c 5661 6c75 6573 5b73  self.AllValues[s
-00015630: 656c 662e 6672 616d 6569 645f 6b65 795d  elf.frameid_key]
-00015640: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00015650: 2020 2020 656e 6474 696d 6520 3d20 696e      endtime = in
-00015660: 7428 6d61 7828 7365 6c66 2e41 6c6c 5661  t(max(self.AllVa
-00015670: 6c75 6573 5b73 656c 662e 6672 616d 6569  lues[self.framei
-00015680: 645f 6b65 795d 2929 0d0a 2020 2020 2020  d_key]))..      
-00015690: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000156a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000156b0: 662e 7469 6d65 203d 205b 5d0d 0a20 2020  f.time = []..   
-000156c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000156d0: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
-000156e0: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
-000156f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015700: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
-00015710: 705f 7a20 3d20 5b5d 0d0a 0d0a 2020 2020  p_z = []....    
-00015720: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015730: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
-00015740: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
-00015750: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015760: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
-00015770: 5f79 203d 205b 5d0d 0a0d 0a20 2020 2020  _y = []....     
-00015780: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015790: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-000157a0: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
-000157b0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-000157c0: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
-000157d0: 7820 3d20 5b5d 0d0a 0d0a 2020 2020 2020  x = []....      
-000157e0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-000157f0: 6974 6f74 6963 5f6d 6561 6e5f 7261 6469  itotic_mean_radi
-00015800: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
-00015810: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00015820: 746f 7469 635f 7661 725f 7261 6469 7573  totic_var_radius
-00015830: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00015840: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00015850: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
-00015860: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00015870: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00015880: 7469 635f 7661 725f 7370 6565 6420 3d20  tic_var_speed = 
-00015890: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-000158a0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-000158b0: 6963 5f6d 6561 6e5f 6163 6320 3d20 5b5d  ic_mean_acc = []
-000158c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000158d0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-000158e0: 6172 5f61 6363 203d 205b 5d0d 0a0d 0a20  ar_acc = [].... 
-000158f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015900: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
-00015910: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00015920: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
-00015930: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00015940: 6974 6f74 6963 5f76 6172 5f64 6972 6563  itotic_var_direc
-00015950: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
-00015960: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00015970: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00015980: 6963 5f6d 6561 6e5f 6469 7374 616e 6365  ic_mean_distance
-00015990: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
-000159a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000159b0: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
-000159c0: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
-000159d0: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
-000159e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000159f0: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00015a00: 616e 5f64 6973 705f 7a20 3d20 5b5d 0d0a  an_disp_z = []..
-00015a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a20: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00015a30: 5f76 6172 5f64 6973 705f 7a20 3d20 5b5d  _var_disp_z = []
-00015a40: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00015a50: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00015a60: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f79  otic_mean_disp_y
-00015a70: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00015a80: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00015a90: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
-00015aa0: 5f79 203d 205b 5d0d 0a0d 0a20 2020 2020  _y = []....     
-00015ab0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015ac0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00015ad0: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
-00015ae0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015af0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-00015b00: 6172 5f64 6973 705f 7820 3d20 5b5d 0d0a  ar_disp_x = []..
-00015b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015b20: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00015b30: 6963 5f6d 6561 6e5f 7261 6469 7573 203d  ic_mean_radius =
-00015b40: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00015b50: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00015b60: 746f 7469 635f 7661 725f 7261 6469 7573  totic_var_radius
-00015b70: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00015b80: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00015b90: 6e5f 6d69 746f 7469 635f 6d65 616e 5f73  n_mitotic_mean_s
-00015ba0: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
-00015bb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015bc0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00015bd0: 7370 6565 6420 3d20 5b5d 0d0a 0d0a 2020  speed = []....  
-00015be0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015bf0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00015c00: 6561 6e5f 6163 6320 3d20 5b5d 0d0a 2020  ean_acc = []..  
-00015c10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015c20: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-00015c30: 6172 5f61 6363 203d 205b 5d0d 0a0d 0a20  ar_acc = [].... 
-00015c40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015c50: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00015c60: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
-00015c70: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 2020  _change = []..  
-00015c80: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015c90: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-00015ca0: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
-00015cb0: 6861 6e67 6520 3d20 5b5d 0d0a 0d0a 2020  hange = []....  
-00015cc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015cd0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00015ce0: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
-00015cf0: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
-00015d00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015d10: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
-00015d20: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
-00015d30: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
-00015d40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015d50: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
-00015d60: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
-00015d70: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00015d80: 5f76 6172 5f64 6973 705f 7a20 3d20 5b5d  _var_disp_z = []
-00015d90: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00015da0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-00015db0: 6e5f 6469 7370 5f79 203d 205b 5d0d 0a20  n_disp_y = [].. 
-00015dc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015dd0: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
-00015de0: 5f79 203d 205b 5d0d 0a0d 0a20 2020 2020  _y = []....     
-00015df0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015e00: 616c 6c5f 6d65 616e 5f64 6973 705f 7820  all_mean_disp_x 
-00015e10: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00015e20: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00015e30: 6172 5f64 6973 705f 7820 3d20 5b5d 0d0a  ar_disp_x = []..
-00015e40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015e50: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
-00015e60: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
-00015e70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015e80: 662e 616c 6c5f 7661 725f 7261 6469 7573  f.all_var_radius
-00015e90: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00015ea0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00015eb0: 6c5f 6d65 616e 5f73 7065 6564 203d 205b  l_mean_speed = [
-00015ec0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00015ed0: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00015ee0: 7370 6565 6420 3d20 5b5d 0d0a 0d0a 2020  speed = []....  
-00015ef0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015f00: 6c66 2e61 6c6c 5f6d 6561 6e5f 6163 6320  lf.all_mean_acc 
-00015f10: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00015f20: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00015f30: 6172 5f61 6363 203d 205b 5d0d 0a0d 0a20  ar_acc = [].... 
-00015f40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015f50: 656c 662e 616c 6c5f 6d65 616e 5f64 6972  elf.all_mean_dir
-00015f60: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-00015f70: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00015f80: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00015f90: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
-00015fa0: 6861 6e67 6520 3d20 5b5d 0d0a 0d0a 2020  hange = []....  
-00015fb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015fc0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7374  lf.all_mean_dist
-00015fd0: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-00015fe0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00015ff0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
-00016000: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
-00016010: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
-00016020: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016030: 662e 6d69 746f 7469 635f 636c 7573 7465  f.mitotic_cluste
-00016040: 725f 636c 6173 7320 3d20 5b5d 0d0a 2020  r_class = []..  
-00016050: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016060: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f63  lf.non_mitotic_c
-00016070: 6c75 7374 6572 5f63 6c61 7373 203d 205b  luster_class = [
-00016080: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016090: 2020 2073 656c 662e 616c 6c5f 636c 7573     self.all_clus
-000160a0: 7465 725f 636c 6173 7320 3d20 5b5d 0d0a  ter_class = []..
-000160b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000160c0: 2020 616c 6c5f 7370 6f74 735f 7472 6163    all_spots_trac
-000160d0: 6b73 203d 207b 7d0d 0a20 2020 2020 2020  ks = {}..       
-000160e0: 2020 2020 2020 2020 2066 6f72 2028 6b2c           for (k,
-000160f0: 7629 2069 6e20 7365 6c66 2e75 6e69 7175  v) in self.uniqu
-00016100: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00016110: 732e 6974 656d 7328 293a 0d0a 2020 2020  s.items():..    
-00016120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016130: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00016140: 2020 2020 2020 2020 2020 616c 6c5f 7370            all_sp
-00016150: 6f74 7320 3d20 7365 6c66 2e75 6e69 7175  ots = self.uniqu
-00016160: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00016170: 735b 6b5d 0d0a 2020 2020 2020 2020 2020  s[k]..          
-00016180: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00016190: 656c 662e 7472 6163 6b69 645f 6b65 7920  elf.trackid_key 
-000161a0: 696e 2061 6c6c 5f73 706f 7473 3a0d 0a20  in all_spots:.. 
-000161b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161c0: 2020 2020 2020 2020 2061 6c6c 5f73 706f           all_spo
-000161d0: 7473 5f74 7261 636b 735b 6b5d 203d 2061  ts_tracks[k] = a
-000161e0: 6c6c 5f73 706f 7473 0d0a 2020 2020 2020  ll_spots..      
-000161f0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-00016200: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00016210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016220: 6675 7475 7265 7320 3d20 5b5d 0d0a 2020  futures = []..  
-00016230: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-00016240: 7468 2063 6f6e 6375 7272 656e 742e 6675  th concurrent.fu
-00016250: 7475 7265 732e 5468 7265 6164 506f 6f6c  tures.ThreadPool
-00016260: 4578 6563 7574 6f72 286d 6178 5f77 6f72  Executor(max_wor
-00016270: 6b65 7273 203d 206f 732e 6370 755f 636f  kers = os.cpu_co
-00016280: 756e 7428 2929 2061 7320 6578 6563 7574  unt()) as execut
-00016290: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-000162a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00013ad0: 2020 2020 2051 5541 4c49 5459 203d 206d       QUALITY = m
+00013ae0: 6174 682e 706f 7728 766f 6c75 6d65 5b69  ath.pow(volume[i
+00013af0: 6e64 6578 5d2c 2031 2e30 2f33 2e30 290d  ndex], 1.0/3.0).
+00013b00: 0a20 2020 2020 2020 2020 2020 2052 4144  .            RAD
+00013b10: 4955 5320 3d20 6d61 7468 2e70 6f77 2876  IUS = math.pow(v
+00013b20: 6f6c 756d 655b 696e 6465 785d 202a 2073  olume[index] * s
+00013b30: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
+00013b40: 202a 2073 656c 662e 7963 616c 6962 7261   * self.ycalibra
+00013b50: 7469 6f6e 202a 2073 656c 662e 7a63 616c  tion * self.zcal
+00013b60: 6962 7261 7469 6f6e 2c20 312e 302f 332e  ibration, 1.0/3.
+00013b70: 3029 200d 0a0d 0a20 2020 2020 2020 2020  0) ....         
+00013b80: 2020 2064 6973 7461 6e63 655f 6365 6c6c     distance_cell
+00013b90: 5f6d 6173 6b2c 206d 6173 6b63 656e 7472  _mask, maskcentr
+00013ba0: 6f69 6420 3d20 7365 6c66 2e5f 6765 745f  oid = self._get_
+00013bb0: 626f 756e 6461 7279 5f64 6973 7428 6672  boundary_dist(fr
+00013bc0: 616d 652c 206c 6f63 6174 696f 6e29 0d0a  ame, location)..
+00013bd0: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+00013be0: 6973 7420 3c3d 2032 202a 2076 6574 6f5f  ist <= 2 * veto_
+00013bf0: 7261 6469 7573 3a0d 0a20 2020 2020 2020  radius:..       
+00013c00: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+00013c10: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
+00013c20: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
+00013c30: 6c5f 6964 5d20 3d20 7b0d 0a20 2020 2020  l_id] = {..     
+00013c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c50: 2020 2073 656c 662e 6365 6c6c 6964 5f6b     self.cellid_k
+00013c60: 6579 3a20 696e 7428 6365 6c6c 5f69 6429  ey: int(cell_id)
+00013c70: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00013c80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013c90: 2e66 7261 6d65 6964 5f6b 6579 203a 2069  .frameid_key : i
+00013ca0: 6e74 2866 7261 6d65 292c 0d0a 2020 2020  nt(frame),..    
+00013cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cc0: 2020 2020 7365 6c66 2e7a 706f 7369 645f      self.zposid_
+00013cd0: 6b65 7920 3a20 666c 6f61 7428 6365 6e74  key : float(cent
+00013ce0: 726f 6964 735b 696e 6465 785d 5b30 5d2a  roids[index][0]*
+00013cf0: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
+00013d00: 6f6e 292c 0d0a 2020 2020 2020 2020 2020  on),..          
+00013d10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00013d20: 6c66 2e79 706f 7369 645f 6b65 7920 3a20  lf.yposid_key : 
+00013d30: 666c 6f61 7428 6365 6e74 726f 6964 735b  float(centroids[
+00013d40: 696e 6465 785d 5b31 5d2a 2073 656c 662e  index][1]* self.
+00013d50: 7963 616c 6962 7261 7469 6f6e 292c 0d0a  ycalibration),..
+00013d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d70: 2020 2020 2020 2020 7365 6c66 2e78 706f          self.xpo
+00013d80: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
+00013d90: 6365 6e74 726f 6964 735b 696e 6465 785d  centroids[index]
+00013da0: 5b32 5d2a 2073 656c 662e 7863 616c 6962  [2]* self.xcalib
+00013db0: 7261 7469 6f6e 292c 0d0a 2020 2020 2020  ration),..      
+00013dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013dd0: 2020 7365 6c66 2e74 7261 636b 6964 5f6b    self.trackid_k
+00013de0: 6579 3a20 696e 7428 7472 6163 6b5f 6964  ey: int(track_id
+00013df0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00013e00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013e10: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
+00013e20: 5f6b 6579 203a 2028 666c 6f61 7428 696e  _key : (float(in
+00013e30: 7465 6e73 6974 795f 746f 7461 6c5b 696e  tensity_total[in
+00013e40: 6465 785d 2929 2c0d 0a20 2020 2020 2020  dex])),..       
+00013e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e60: 2073 656c 662e 6d65 616e 5f69 6e74 656e   self.mean_inten
+00013e70: 7369 7479 5f6b 6579 203a 2028 666c 6f61  sity_key : (floa
+00013e80: 7428 696e 7465 6e73 6974 795f 6d65 616e  t(intensity_mean
+00013e90: 5b69 6e64 6578 5d29 292c 0d0a 0d0a 2020  [index])),....  
+00013ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013eb0: 2020 2020 2020 7365 6c66 2e72 6164 6975        self.radiu
+00013ec0: 735f 6b65 7920 3a20 2866 6c6f 6174 2852  s_key : (float(R
+00013ed0: 4144 4955 5329 292c 0d0a 2020 2020 2020  ADIUS)),..      
+00013ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ef0: 2020 7365 6c66 2e71 7561 6c69 7479 5f6b    self.quality_k
+00013f00: 6579 203a 2028 666c 6f61 7428 5155 414c  ey : (float(QUAL
+00013f10: 4954 5929 292c 0d0a 2020 2020 2020 2020  ITY)),..        
+00013f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f30: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
+00013f40: 6c6c 5f6d 6173 6b5f 6b65 793a 2066 6c6f  ll_mask_key: flo
+00013f50: 6174 2864 6973 7461 6e63 655f 6365 6c6c  at(distance_cell
+00013f60: 5f6d 6173 6b29 2c0d 0a20 2020 2020 2020  _mask),..       
+00013f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f80: 2073 656c 662e 6d61 736b 6365 6e74 726f   self.maskcentro
+00013f90: 6964 5f7a 5f6b 6579 3a20 666c 6f61 7428  id_z_key: float(
+00013fa0: 6d61 736b 6365 6e74 726f 6964 5b30 5d29  maskcentroid[0])
+00013fb0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00013fc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013fd0: 6d61 736b 6365 6e74 726f 6964 5f79 5f6b  maskcentroid_y_k
+00013fe0: 6579 3a20 666c 6f61 7428 6d61 736b 6365  ey: float(maskce
+00013ff0: 6e74 726f 6964 5b31 5d29 2c0d 0a20 2020  ntroid[1]),..   
+00014000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014010: 2020 2020 2073 656c 662e 6d61 736b 6365       self.maskce
+00014020: 6e74 726f 6964 5f78 5f6b 6579 3a20 666c  ntroid_x_key: fl
+00014030: 6f61 7428 6d61 736b 6365 6e74 726f 6964  oat(maskcentroid
+00014040: 5b32 5d29 200d 0a0d 0a20 2020 2020 2020  [2]) ....       
+00014050: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
+00014060: 2020 2020 2020 2020 656c 6966 2063 656c          elif cel
+00014070: 6c5f 6964 2069 6e20 7365 6c66 2e65 6467  l_id in self.edg
+00014080: 655f 736f 7572 6365 5f6c 6f6f 6b75 702e  e_source_lookup.
+00014090: 6b65 7973 2829 3a0d 0a20 2020 2020 2020  keys():..       
+000140a0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000140b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140c0: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+000140d0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+000140e0: 6572 7469 6573 5b63 656c 6c5f 6964 5d20  erties[cell_id] 
+000140f0: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
+00014100: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+00014110: 6c6c 5f69 645d 0d0a 0d0a 2020 2020 2020  ll_id]....      
+00014120: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014130: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+00014140: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014150: 735b 6365 6c6c 5f69 645d 2e75 7064 6174  s[cell_id].updat
+00014160: 6528 7b73 656c 662e 746f 7461 6c5f 696e  e({self.total_in
+00014170: 7465 6e73 6974 795f 6b65 793a 202d 3130  tensity_key: -10
+00014180: 307d 290d 0a20 2020 2020 2020 2020 2020  0})..           
+00014190: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+000141a0: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
+000141b0: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
+000141c0: 6c5f 6964 5d2e 7570 6461 7465 287b 7365  l_id].update({se
+000141d0: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
+000141e0: 795f 6b65 793a 202d 3130 307d 290d 0a20  y_key: -100}).. 
+000141f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014200: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+00014210: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014220: 6572 7469 6573 5b63 656c 6c5f 6964 5d2e  erties[cell_id].
+00014230: 7570 6461 7465 287b 7365 6c66 2e72 6164  update({self.rad
+00014240: 6975 735f 6b65 793a 202d 3130 307d 290d  ius_key: -100}).
+00014250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014260: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
+00014270: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
+00014280: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
+00014290: 5d2e 7570 6461 7465 287b 7365 6c66 2e71  ].update({self.q
+000142a0: 7561 6c69 7479 5f6b 6579 3a20 2d31 3030  uality_key: -100
+000142b0: 7d29 0d0a 0d0a 0d0a 2020 2020 2020 2020  })......        
+000142c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142d0: 2020 2020 2020 2020 200d 0a20 2020 2064           ..    d
+000142e0: 6566 205f 6469 6374 5f75 7064 6174 6528  ef _dict_update(
+000142f0: 7365 6c66 2c20 756e 6971 7565 5f74 7261  self, unique_tra
+00014300: 636b 6c65 745f 6964 733a 204c 6973 742c  cklet_ids: List,
+00014310: 2020 6365 6c6c 5f69 643a 2069 6e74 2c20    cell_id: int, 
+00014320: 7472 6163 6b5f 6964 3a20 696e 742c 2073  track_id: int, s
+00014330: 6f75 7263 655f 6964 3a20 696e 742c 2074  ource_id: int, t
+00014340: 6172 6765 745f 6964 3a20 696e 7429 3a0d  arget_id: int):.
+00014350: 0a0d 0a20 0d0a 2020 2020 2020 2020 6765  ... ..        ge
+00014360: 6e65 7261 7469 6f6e 5f69 6420 3d20 7365  neration_id = se
+00014370: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
+00014380: 6374 5b63 656c 6c5f 6964 5d0d 0a20 2020  ct[cell_id]..   
+00014390: 2020 2020 2074 7261 636b 6c65 745f 6964       tracklet_id
+000143a0: 203d 2073 656c 662e 7472 6163 6b6c 6574   = self.tracklet
+000143b0: 5f64 6963 745b 6365 6c6c 5f69 645d 0d0a  _dict[cell_id]..
+000143c0: 0d0a 2020 2020 2020 2020 756e 6971 7565  ..        unique
+000143d0: 5f69 6420 3d20 7374 7228 7472 6163 6b5f  _id = str(track_
+000143e0: 6964 2920 2b20 7374 7228 7365 6c66 2e6d  id) + str(self.m
+000143f0: 6178 5f74 7261 636b 5f69 6429 202b 2073  ax_track_id) + s
+00014400: 7472 2867 656e 6572 6174 696f 6e5f 6964  tr(generation_id
+00014410: 2920 2b20 7374 7228 7472 6163 6b6c 6574  ) + str(tracklet
+00014420: 5f69 6429 0d0a 2020 2020 2020 2020 0d0a  _id)..        ..
+00014430: 2020 2020 2020 2020 7665 635f 6d61 736b          vec_mask
+00014440: 203d 205b 666c 6f61 7428 7365 6c66 2e75   = [float(self.u
+00014450: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00014460: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00014470: 6429 5d5b 7365 6c66 2e6d 6173 6b63 656e  d)][self.maskcen
+00014480: 7472 6f69 645f 785f 6b65 795d 292c 2066  troid_x_key]), f
+00014490: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+000144a0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000144b0: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+000144c0: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
+000144d0: 5f79 5f6b 6579 5d29 2c20 666c 6f61 7428  _y_key]), float(
+000144e0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000144f0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00014500: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
+00014510: 6173 6b63 656e 7472 6f69 645f 7a5f 6b65  askcentroid_z_ke
+00014520: 795d 2920 5d0d 0a0d 0a20 2020 2020 2020  y]) ]....       
+00014530: 2076 6563 5f63 656c 6c20 3d20 5b66 6c6f   vec_cell = [flo
+00014540: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00014550: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014560: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+00014570: 662e 7870 6f73 6964 5f6b 6579 5d29 202c  f.xposid_key]) ,
+00014580: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00014590: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000145a0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+000145b0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000145c0: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+000145d0: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
+000145e0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+000145f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014600: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00014610: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014620: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+00014630: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
+00014640: 295d 0d0a 0d0a 2020 2020 2020 2020 616e  )]....        an
+00014650: 676c 6520 3d20 616e 6775 6c61 725f 6368  gle = angular_ch
+00014660: 616e 6765 2876 6563 5f6d 6173 6b2c 2076  ange(vec_mask, v
+00014670: 6563 5f63 656c 6c29 0d0a 0d0a 2020 2020  ec_cell)....    
+00014680: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00014690: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000146a0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+000146b0: 6461 7465 287b 7365 6c66 2e72 6164 6961  date({self.radia
+000146c0: 6c5f 616e 676c 655f 6b65 7920 3a20 616e  l_angle_key : an
+000146d0: 676c 657d 2920 2020 2020 2020 2020 2020  gle})           
+000146e0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+000146f0: 2020 2020 2075 6e69 7175 655f 7472 6163       unique_trac
+00014700: 6b6c 6574 5f69 6473 2e61 7070 656e 6428  klet_ids.append(
+00014710: 7374 7228 756e 6971 7565 5f69 6429 290d  str(unique_id)).
+00014720: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00014730: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00014740: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00014750: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00014760: 636c 7573 7465 7263 6c61 7373 5f6b 6579  clusterclass_key
+00014770: 203a 202d 3130 307d 290d 0a20 2020 2020   : -100})..     
+00014780: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00014790: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+000147a0: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+000147b0: 6174 6528 7b73 656c 662e 636c 7573 7465  ate({self.cluste
+000147c0: 7273 636f 7265 5f6b 6579 203a 2030 7d29  rscore_key : 0})
+000147d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+000147e0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000147f0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00014800: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00014810: 2e75 6e69 7175 6569 645f 6b65 7920 3a20  .uniqueid_key : 
+00014820: 7374 7228 756e 6971 7565 5f69 6429 7d29  str(unique_id)})
+00014830: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00014840: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00014850: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00014860: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00014870: 2e74 7261 636b 6c65 7469 645f 6b65 7920  .trackletid_key 
+00014880: 3a20 7374 7228 7472 6163 6b6c 6574 5f69  : str(tracklet_i
+00014890: 6429 7d29 200d 0a20 2020 2020 2020 2073  d)}) ..        s
+000148a0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000148b0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+000148c0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+000148d0: 7b73 656c 662e 6765 6e65 7261 7469 6f6e  {self.generation
+000148e0: 6964 5f6b 6579 203a 2073 7472 2867 656e  id_key : str(gen
+000148f0: 6572 6174 696f 6e5f 6964 297d 2920 0d0a  eration_id)}) ..
+00014900: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00014910: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014920: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00014930: 5d2e 7570 6461 7465 287b 7365 6c66 2e74  ].update({self.t
+00014940: 7261 636b 6964 5f6b 6579 203a 2073 7472  rackid_key : str
+00014950: 2874 7261 636b 5f69 6429 7d29 0d0a 2020  (track_id)})..  
+00014960: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00014970: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014980: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+00014990: 7570 6461 7465 287b 7365 6c66 2e6d 6f74  update({self.mot
+000149a0: 696f 6e5f 616e 676c 655f 6b65 7920 3a20  ion_angle_key : 
+000149b0: 302e 307d 290d 0a20 2020 2020 2020 2073  0.0})..        s
+000149c0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000149d0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+000149e0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+000149f0: 7b73 656c 662e 7370 6565 645f 6b65 7920  {self.speed_key 
+00014a00: 3a20 302e 307d 290d 0a20 2020 2020 2020  : 0.0})..       
+00014a10: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00014a20: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014a30: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+00014a40: 6528 7b73 656c 662e 6163 6365 6c65 7261  e({self.accelera
+00014a50: 7469 6f6e 5f6b 6579 203a 2030 2e30 7d29  tion_key : 0.0})
+00014a60: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00014a70: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00014a80: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00014a90: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00014aa0: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+00014ab0: 6d70 5f66 6972 7374 6b65 7920 3a20 2d31  mp_firstkey : -1
+00014ac0: 3030 7d29 0d0a 2020 2020 2020 2020 7365  00})..        se
+00014ad0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00014ae0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00014af0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00014b00: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
+00014b10: 795f 636f 6d70 5f73 6563 6f6e 646b 6579  y_comp_secondkey
+00014b20: 203a 202d 3130 307d 290d 0a20 2020 2020   : -100})..     
+00014b30: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00014b40: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014b50: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00014b60: 6174 6528 7b73 656c 662e 7375 7266 6163  ate({self.surfac
+00014b70: 655f 6172 6561 5f6b 6579 203a 202d 3130  e_area_key : -10
+00014b80: 307d 290d 0a20 2020 2020 2020 2073 656c  0})..        sel
+00014b90: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00014ba0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00014bb0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00014bc0: 656c 662e 6365 6c6c 6178 6973 5f6d 6173  elf.cellaxis_mas
+00014bd0: 6b5f 6b65 7920 3a20 2d31 3030 7d29 0d0a  k_key : -100})..
+00014be0: 0d0a 2020 2020 2020 2020 6966 2073 6f75  ..        if sou
+00014bf0: 7263 655f 6964 2069 7320 6e6f 7420 4e6f  rce_id is not No
+00014c00: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00014c10: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00014c20: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014c30: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+00014c40: 6528 7b73 656c 662e 6265 666f 7265 6964  e({self.beforeid
+00014c50: 5f6b 6579 203a 2069 6e74 2873 6f75 7263  _key : int(sourc
+00014c60: 655f 6964 297d 290d 0a20 2020 2020 2020  e_id)})..       
+00014c70: 2020 2020 2076 6563 5f31 203d 205b 666c       vec_1 = [fl
+00014c80: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00014c90: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014ca0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00014cb0: 6c66 2e78 706f 7369 645f 6b65 795d 2920  lf.xposid_key]) 
+00014cc0: 2d20 666c 6f61 7428 7365 6c66 2e75 6e69  - float(self.uni
+00014cd0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014ce0: 6965 735b 696e 7428 736f 7572 6365 5f69  ies[int(source_i
+00014cf0: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
+00014d00: 6b65 795d 292c 200d 0a20 2020 2020 2020  key]), ..       
+00014d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d20: 2020 2020 2066 6c6f 6174 2873 656c 662e       float(self.
+00014d30: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014d40: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00014d50: 6964 295d 5b73 656c 662e 7970 6f73 6964  id)][self.yposid
+00014d60: 5f6b 6579 5d29 202d 2066 6c6f 6174 2873  _key]) - float(s
+00014d70: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00014d80: 7072 6f70 6572 7469 6573 5b69 6e74 2873  properties[int(s
+00014d90: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
+00014da0: 7970 6f73 6964 5f6b 6579 5d29 2c20 0d0a  yposid_key]), ..
+00014db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014dc0: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
+00014dd0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00014de0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00014df0: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
+00014e00: 2e7a 706f 7369 645f 6b65 795d 2920 2d20  .zposid_key]) - 
+00014e10: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+00014e20: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014e30: 6573 5b69 6e74 2873 6f75 7263 655f 6964  es[int(source_id
+00014e40: 295d 5b73 656c 662e 7a70 6f73 6964 5f6b  )][self.zposid_k
+00014e50: 6579 5d29 5d0d 0a20 2020 2020 2020 2020  ey])]..         
+00014e60: 2020 2073 7065 6564 203d 206e 702e 7371     speed = np.sq
+00014e70: 7274 286e 702e 646f 7428 7665 635f 312c  rt(np.dot(vec_1,
+00014e80: 2076 6563 5f31 2929 2f73 656c 662e 7463   vec_1))/self.tc
+00014e90: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00014ea0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00014eb0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014ec0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00014ed0: 5d2e 7570 6461 7465 287b 7365 6c66 2e73  ].update({self.s
+00014ee0: 7065 6564 5f6b 6579 203a 2073 7065 6564  peed_key : speed
+00014ef0: 7d29 0d0a 0d0a 2020 2020 2020 2020 2020  })....          
+00014f00: 2020 6d6f 7469 6f6e 5f61 6e67 6c65 203d    motion_angle =
+00014f10: 2061 6e67 756c 6172 5f63 6861 6e67 6528   angular_change(
+00014f20: 7665 635f 6d61 736b 2c20 7665 635f 3129  vec_mask, vec_1)
+00014f30: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00014f40: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00014f50: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00014f60: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00014f70: 287b 7365 6c66 2e6d 6f74 696f 6e5f 616e  ({self.motion_an
+00014f80: 676c 655f 6b65 7920 3a20 6d6f 7469 6f6e  gle_key : motion
+00014f90: 5f61 6e67 6c65 7d29 200d 0a0d 0a20 2020  _angle}) ....   
+00014fa0: 2020 2020 2020 2020 2069 6620 736f 7572           if sour
+00014fb0: 6365 5f69 6420 696e 2073 656c 662e 6564  ce_id in self.ed
+00014fc0: 6765 5f73 6f75 7263 655f 6c6f 6f6b 7570  ge_source_lookup
+00014fd0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00014fe0: 2020 2020 2020 2070 7265 5f73 6f75 7263         pre_sourc
+00014ff0: 655f 6964 203d 2073 656c 662e 6564 6765  e_id = self.edge
+00015000: 5f73 6f75 7263 655f 6c6f 6f6b 7570 5b73  _source_lookup[s
+00015010: 6f75 7263 655f 6964 5d0d 0a20 2020 2020  ource_id]..     
+00015020: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00015030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015040: 2020 2020 2076 6563 5f32 203d 205b 666c       vec_2 = [fl
+00015050: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00015060: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015070: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00015080: 6c66 2e78 706f 7369 645f 6b65 795d 2920  lf.xposid_key]) 
+00015090: 2d20 3220 2a20 666c 6f61 7428 7365 6c66  - 2 * float(self
+000150a0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000150b0: 7065 7274 6965 735b 696e 7428 736f 7572  perties[int(sour
+000150c0: 6365 5f69 6429 5d5b 7365 6c66 2e78 706f  ce_id)][self.xpo
+000150d0: 7369 645f 6b65 795d 2920 2b20 666c 6f61  sid_key]) + floa
+000150e0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+000150f0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00015100: 7428 7072 655f 736f 7572 6365 5f69 6429  t(pre_source_id)
+00015110: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
+00015120: 795d 292c 200d 0a20 2020 2020 2020 2020  y]), ..         
+00015130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015140: 2020 2066 6c6f 6174 2873 656c 662e 756e     float(self.un
+00015150: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015160: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015170: 295d 5b73 656c 662e 7970 6f73 6964 5f6b  )][self.yposid_k
+00015180: 6579 5d29 202d 2032 202a 2066 6c6f 6174  ey]) - 2 * float
+00015190: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+000151a0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+000151b0: 2873 6f75 7263 655f 6964 295d 5b73 656c  (source_id)][sel
+000151c0: 662e 7970 6f73 6964 5f6b 6579 5d29 202b  f.yposid_key]) +
+000151d0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+000151e0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000151f0: 6573 5b69 6e74 2870 7265 5f73 6f75 7263  es[int(pre_sourc
+00015200: 655f 6964 295d 5b73 656c 662e 7970 6f73  e_id)][self.ypos
+00015210: 6964 5f6b 6579 5d29 2c20 0d0a 2020 2020  id_key]), ..    
+00015220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015230: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
+00015240: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015250: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00015260: 6c6c 5f69 6429 5d5b 7365 6c66 2e7a 706f  ll_id)][self.zpo
+00015270: 7369 645f 6b65 795d 2920 2d20 2032 202a  sid_key]) -  2 *
+00015280: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+00015290: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000152a0: 6573 5b69 6e74 2873 6f75 7263 655f 6964  es[int(source_id
+000152b0: 295d 5b73 656c 662e 7a70 6f73 6964 5f6b  )][self.zposid_k
+000152c0: 6579 5d29 202b 2066 6c6f 6174 2873 656c  ey]) + float(sel
+000152d0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000152e0: 6f70 6572 7469 6573 5b69 6e74 2870 7265  operties[int(pre
+000152f0: 5f73 6f75 7263 655f 6964 295d 5b73 656c  _source_id)][sel
+00015300: 662e 7a70 6f73 6964 5f6b 6579 5d29 5d0d  f.zposid_key])].
+00015310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015320: 2020 2020 2061 6363 203d 206e 702e 7371       acc = np.sq
+00015330: 7274 286e 702e 646f 7428 7665 635f 322c  rt(np.dot(vec_2,
+00015340: 2076 6563 5f32 2929 2f73 656c 662e 7463   vec_2))/self.tc
+00015350: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00015360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015370: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015380: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00015390: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000153a0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+000153b0: 7570 6461 7465 287b 7365 6c66 2e61 6363  update({self.acc
+000153c0: 656c 6572 6174 696f 6e5f 6b65 7920 3a20  eleration_key : 
+000153d0: 6163 637d 290d 0a20 2020 2020 2020 2065  acc})..        e
+000153e0: 6c69 6620 736f 7572 6365 5f69 6420 6973  lif source_id is
+000153f0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00015400: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00015410: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015420: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00015430: 6461 7465 287b 7365 6c66 2e62 6566 6f72  date({self.befor
+00015440: 6569 645f 6b65 7920 3a20 4e6f 6e65 7d29  eid_key : None})
+00015450: 200d 0a20 2020 2020 2020 2020 2020 200d   ..            .
+00015460: 0a0d 0a20 2020 2020 2020 2069 6620 7461  ...        if ta
+00015470: 7267 6574 5f69 6420 6973 206e 6f74 204e  rget_id is not N
+00015480: 6f6e 653a 2020 2020 2020 200d 0a20 2020  one:       ..   
+00015490: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+000154a0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000154b0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+000154c0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+000154d0: 6166 7465 7269 645f 6b65 7920 3a20 696e  afterid_key : in
+000154e0: 7428 7461 7267 6574 5f69 6429 7d29 200d  t(target_id)}) .
+000154f0: 0a20 2020 2020 2020 2065 6c69 6620 7461  .        elif ta
+00015500: 7267 6574 5f69 6420 6973 204e 6f6e 653a  rget_id is None:
+00015510: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00015520: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015530: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00015540: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00015550: 7365 6c66 2e61 6674 6572 6964 5f6b 6579  self.afterid_key
+00015560: 203a 204e 6f6e 657d 290d 0a20 2020 2020   : None})..     
+00015570: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00015580: 2073 656c 662e 5f73 6563 6f6e 645f 6368   self._second_ch
+00015590: 616e 6e65 6c5f 7570 6461 7465 2863 656c  annel_update(cel
+000155a0: 6c5f 6964 2c20 7472 6163 6b5f 6964 2920  l_id, track_id) 
+000155b0: 2020 200d 0a0d 0a0d 0a20 2020 2064 6566     ......    def
+000155c0: 205f 7465 6d70 6f72 616c 5f70 6c6f 7473   _temporal_plots
+000155d0: 5f74 7261 636b 6d61 7465 2873 656c 6629  _trackmate(self)
+000155e0: 3a0d 0a20 2020 200d 0a20 2020 200d 0a20  :..    ..    .. 
+000155f0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00015600: 2020 2020 2073 656c 662e 4174 7472 203d       self.Attr =
+00015610: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
+00015620: 2020 2020 2073 7461 7274 7469 6d65 203d       starttime =
+00015630: 2069 6e74 286d 696e 2873 656c 662e 416c   int(min(self.Al
+00015640: 6c56 616c 7565 735b 7365 6c66 2e66 7261  lValues[self.fra
+00015650: 6d65 6964 5f6b 6579 5d29 290d 0a20 2020  meid_key]))..   
+00015660: 2020 2020 2020 2020 2020 2020 2065 6e64               end
+00015670: 7469 6d65 203d 2069 6e74 286d 6178 2873  time = int(max(s
+00015680: 656c 662e 416c 6c56 616c 7565 735b 7365  elf.AllValues[se
+00015690: 6c66 2e66 7261 6d65 6964 5f6b 6579 5d29  lf.frameid_key])
+000156a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000156b0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000156c0: 2020 2020 2020 7365 6c66 2e74 696d 6520        self.time 
+000156d0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+000156e0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+000156f0: 6963 5f6d 6561 6e5f 6469 7370 5f7a 203d  ic_mean_disp_z =
+00015700: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00015710: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00015720: 635f 7661 725f 6469 7370 5f7a 203d 205b  c_var_disp_z = [
+00015730: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00015740: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00015750: 635f 6d65 616e 5f64 6973 705f 7920 3d20  c_mean_disp_y = 
+00015760: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00015770: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00015780: 5f76 6172 5f64 6973 705f 7920 3d20 5b5d  _var_disp_y = []
+00015790: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000157a0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+000157b0: 5f6d 6561 6e5f 6469 7370 5f78 203d 205b  _mean_disp_x = [
+000157c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000157d0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+000157e0: 7661 725f 6469 7370 5f78 203d 205b 5d0d  var_disp_x = [].
+000157f0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00015800: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00015810: 6d65 616e 5f72 6164 6975 7320 3d20 5b5d  mean_radius = []
+00015820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015830: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+00015840: 6172 5f72 6164 6975 7320 3d20 5b5d 0d0a  ar_radius = []..
+00015850: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015860: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00015870: 6561 6e5f 7370 6565 6420 3d20 5b5d 0d0a  ean_speed = []..
+00015880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015890: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+000158a0: 5f73 7065 6564 203d 205b 5d0d 0a0d 0a20  _speed = [].... 
+000158b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000158c0: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+000158d0: 5f61 6363 203d 205b 5d0d 0a20 2020 2020  _acc = []..     
+000158e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000158f0: 6d69 746f 7469 635f 7661 725f 6163 6320  mitotic_var_acc 
+00015900: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00015910: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00015920: 6f74 6963 5f6d 6561 6e5f 6469 7265 6374  otic_mean_direct
+00015930: 696f 6e61 6c5f 6368 616e 6765 203d 205b  ional_change = [
+00015940: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00015950: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00015960: 7661 725f 6469 7265 6374 696f 6e61 6c5f  var_directional_
+00015970: 6368 616e 6765 203d 205b 5d0d 0a0d 0a20  change = [].... 
+00015980: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015990: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+000159a0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+000159b0: 6173 6b20 3d20 5b5d 0d0a 2020 2020 2020  ask = []..      
+000159c0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+000159d0: 6974 6f74 6963 5f76 6172 5f64 6973 7461  itotic_var_dista
+000159e0: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+000159f0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00015a00: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00015a10: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00015a20: 5f7a 203d 205b 5d0d 0a20 2020 2020 2020  _z = []..       
+00015a30: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00015a40: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
+00015a50: 7370 5f7a 203d 205b 5d0d 0a0d 0a20 2020  sp_z = []....   
+00015a60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015a70: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00015a80: 616e 5f64 6973 705f 7920 3d20 5b5d 0d0a  an_disp_y = []..
+00015a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015aa0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00015ab0: 5f76 6172 5f64 6973 705f 7920 3d20 5b5d  _var_disp_y = []
+00015ac0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00015ad0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00015ae0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f78  otic_mean_disp_x
+00015af0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00015b00: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00015b10: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
+00015b20: 5f78 203d 205b 5d0d 0a0d 0a20 2020 2020  _x = []....     
+00015b30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015b40: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+00015b50: 5f72 6164 6975 7320 3d20 5b5d 0d0a 2020  _radius = []..  
+00015b60: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015b70: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00015b80: 6172 5f72 6164 6975 7320 3d20 5b5d 0d0a  ar_radius = []..
+00015b90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015ba0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00015bb0: 6963 5f6d 6561 6e5f 7370 6565 6420 3d20  ic_mean_speed = 
+00015bc0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00015bd0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00015be0: 6f74 6963 5f76 6172 5f73 7065 6564 203d  otic_var_speed =
+00015bf0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00015c00: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00015c10: 6d69 746f 7469 635f 6d65 616e 5f61 6363  mitotic_mean_acc
+00015c20: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00015c30: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00015c40: 6d69 746f 7469 635f 7661 725f 6163 6320  mitotic_var_acc 
+00015c50: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00015c60: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00015c70: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
+00015c80: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00015c90: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00015ca0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00015cb0: 6d69 746f 7469 635f 7661 725f 6469 7265  mitotic_var_dire
+00015cc0: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
+00015cd0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00015ce0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00015cf0: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00015d00: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+00015d10: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00015d20: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00015d30: 6974 6f74 6963 5f76 6172 5f64 6973 7461  itotic_var_dista
+00015d40: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+00015d50: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00015d60: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00015d70: 6561 6e5f 6469 7370 5f7a 203d 205b 5d0d  ean_disp_z = [].
+00015d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015d90: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
+00015da0: 7370 5f7a 203d 205b 5d0d 0a0d 0a20 2020  sp_z = []....   
+00015db0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015dc0: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
+00015dd0: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
+00015de0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00015df0: 5f76 6172 5f64 6973 705f 7920 3d20 5b5d  _var_disp_y = []
+00015e00: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00015e10: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
+00015e20: 6e5f 6469 7370 5f78 203d 205b 5d0d 0a20  n_disp_x = [].. 
+00015e30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015e40: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
+00015e50: 5f78 203d 205b 5d0d 0a0d 0a20 2020 2020  _x = []....     
+00015e60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015e70: 616c 6c5f 6d65 616e 5f72 6164 6975 7320  all_mean_radius 
+00015e80: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00015e90: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00015ea0: 6172 5f72 6164 6975 7320 3d20 5b5d 0d0a  ar_radius = []..
+00015eb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015ec0: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00015ed0: 7370 6565 6420 3d20 5b5d 0d0a 2020 2020  speed = []..    
+00015ee0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015ef0: 2e61 6c6c 5f76 6172 5f73 7065 6564 203d  .all_var_speed =
+00015f00: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00015f10: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00015f20: 6d65 616e 5f61 6363 203d 205b 5d0d 0a20  mean_acc = [].. 
+00015f30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015f40: 656c 662e 616c 6c5f 7661 725f 6163 6320  elf.all_var_acc 
+00015f50: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00015f60: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00015f70: 5f6d 6561 6e5f 6469 7265 6374 696f 6e61  _mean_directiona
+00015f80: 6c5f 6368 616e 6765 203d 205b 5d0d 0a20  l_change = [].. 
+00015f90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015fa0: 656c 662e 616c 6c5f 7661 725f 6469 7265  elf.all_var_dire
+00015fb0: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
+00015fc0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00015fd0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00015fe0: 6d65 616e 5f64 6973 7461 6e63 655f 6365  mean_distance_ce
+00015ff0: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 2020  ll_mask = []..  
+00016000: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016010: 6c66 2e61 6c6c 5f76 6172 5f64 6973 7461  lf.all_var_dista
+00016020: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+00016030: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00016040: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00016050: 6963 5f63 6c75 7374 6572 5f63 6c61 7373  ic_cluster_class
+00016060: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016070: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00016080: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
+00016090: 636c 6173 7320 3d20 5b5d 0d0a 2020 2020  class = []..    
+000160a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000160b0: 2e61 6c6c 5f63 6c75 7374 6572 5f63 6c61  .all_cluster_cla
+000160c0: 7373 203d 205b 5d0d 0a0d 0a20 2020 2020  ss = []....     
+000160d0: 2020 2020 2020 2020 2020 2061 6c6c 5f73             all_s
+000160e0: 706f 7473 5f74 7261 636b 7320 3d20 7b7d  pots_tracks = {}
+000160f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016100: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
+00016110: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00016120: 7072 6f70 6572 7469 6573 2e69 7465 6d73  properties.items
+00016130: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+00016140: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00016150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016160: 2020 2061 6c6c 5f73 706f 7473 203d 2073     all_spots = s
+00016170: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00016180: 7072 6f70 6572 7469 6573 5b6b 5d0d 0a20  properties[k].. 
+00016190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161a0: 2020 2020 2069 6620 7365 6c66 2e74 7261       if self.tra
+000161b0: 636b 6964 5f6b 6579 2069 6e20 616c 6c5f  ckid_key in all_
+000161c0: 7370 6f74 733a 0d0a 2020 2020 2020 2020  spots:..        
+000161d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161e0: 2020 616c 6c5f 7370 6f74 735f 7472 6163    all_spots_trac
+000161f0: 6b73 5b6b 5d20 3d20 616c 6c5f 7370 6f74  ks[k] = all_spot
+00016200: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00016210: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+00016220: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00016230: 2020 2020 2020 2020 2066 7574 7572 6573           futures
+00016240: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016250: 2020 2020 2020 2077 6974 6820 636f 6e63         with conc
+00016260: 7572 7265 6e74 2e66 7574 7572 6573 2e54  urrent.futures.T
+00016270: 6872 6561 6450 6f6f 6c45 7865 6375 746f  hreadPoolExecuto
+00016280: 7228 6d61 785f 776f 726b 6572 7320 3d20  r(max_workers = 
+00016290: 6f73 2e63 7075 5f63 6f75 6e74 2829 2920  os.cpu_count()) 
+000162a0: 6173 2065 7865 6375 746f 723a 0d0a 2020  as executor:..  
 000162b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162c0: 2066 6f72 2069 2069 6e20 7471 646d 2872   for i in tqdm(r
-000162d0: 616e 6765 2873 7461 7274 7469 6d65 2c20  ange(starttime, 
-000162e0: 656e 6474 696d 6529 2c20 746f 7461 6c3d  endtime), total=
-000162f0: 656e 6474 696d 6520 2d20 7374 6172 7474  endtime - startt
-00016300: 696d 6529 3a0d 0a20 2020 2020 2020 2020  ime):..         
-00016310: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000162c0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000162d0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+000162e0: 696e 2074 7164 6d28 7261 6e67 6528 7374  in tqdm(range(st
+000162f0: 6172 7474 696d 652c 2065 6e64 7469 6d65  arttime, endtime
+00016300: 292c 2074 6f74 616c 3d65 6e64 7469 6d65  ), total=endtime
+00016310: 202d 2073 7461 7274 7469 6d65 293a 0d0a   - starttime):..
 00016320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016330: 2020 2020 2020 2066 7574 7572 6573 2e61         futures.a
-00016340: 7070 656e 6428 6578 6563 7574 6f72 2e73  ppend(executor.s
-00016350: 7562 6d69 7428 7365 6c66 2e5f 636f 6d70  ubmit(self._comp
-00016360: 7574 655f 7465 6d70 6f72 616c 2c20 692c  ute_temporal, i,
-00016370: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
-00016380: 7329 290d 0a20 0d0a 2020 2020 2020 2020  s)).. ..        
-00016390: 2020 2020 2020 2020 2020 2020 5b72 2e72              [r.r
-000163a0: 6573 756c 7428 2920 666f 7220 7220 696e  esult() for r in
-000163b0: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
-000163c0: 7265 732e 6173 5f63 6f6d 706c 6574 6564  res.as_completed
-000163d0: 2866 7574 7572 6573 295d 0d0a 0d0a 0d0a  (futures)]......
-000163e0: 2020 2020 6465 6620 5f63 6f6d 7075 7465      def _compute
-000163f0: 5f74 656d 706f 7261 6c28 7365 6c66 2c20  _temporal(self, 
-00016400: 692c 2061 6c6c 5f73 706f 7473 5f74 7261  i, all_spots_tra
-00016410: 636b 7329 3a20 2020 2020 2020 2020 2020  cks):           
-00016420: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00016430: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00016440: 6963 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ic_disp_z = []..
-00016450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016460: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
-00016470: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
-00016480: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00016490: 6f74 6963 5f64 6973 705f 7820 3d20 5b5d  otic_disp_x = []
-000164a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000164b0: 2020 2020 2020 6d69 746f 7469 635f 7261        mitotic_ra
-000164c0: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
-000164d0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000164e0: 6974 6f74 6963 5f73 7065 6564 203d 205b  itotic_speed = [
-000164f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016500: 2020 2020 2020 206d 6974 6f74 6963 5f61         mitotic_a
-00016510: 6363 203d 205b 5d0d 0a20 2020 2020 2020  cc = []..       
-00016520: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00016530: 6f74 6963 5f64 6972 6563 7469 6f6e 616c  otic_directional
-00016540: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 2020  _change = []..  
-00016550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016560: 2020 6d69 746f 7469 635f 636c 7573 7465    mitotic_cluste
-00016570: 725f 636c 6173 7320 3d20 5b5d 0d0a 2020  r_class = []..  
-00016580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016590: 2020 6d69 746f 7469 635f 6469 7374 616e    mitotic_distan
-000165a0: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-000165b0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-000165c0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-000165d0: 6f74 6963 5f64 6973 705f 7a20 3d20 5b5d  otic_disp_z = []
-000165e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000165f0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00016600: 635f 6469 7370 5f79 203d 205b 5d0d 0a20  c_disp_y = [].. 
-00016610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016620: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-00016630: 6973 705f 7820 3d20 5b5d 0d0a 2020 2020  isp_x = []..    
-00016640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016650: 6e6f 6e5f 6d69 746f 7469 635f 7261 6469  non_mitotic_radi
-00016660: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
-00016670: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00016680: 5f6d 6974 6f74 6963 5f73 7065 6564 203d  _mitotic_speed =
-00016690: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000166a0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-000166b0: 6f74 6963 5f61 6363 203d 205b 5d0d 0a20  otic_acc = [].. 
-000166c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000166d0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-000166e0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-000166f0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
-00016700: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-00016710: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
-00016720: 636c 6173 7320 3d20 5b5d 0d0a 2020 2020  class = []..    
-00016730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016740: 6e6f 6e5f 6d69 746f 7469 635f 6469 7374  non_mitotic_dist
-00016750: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-00016760: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016770: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00016780: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00016790: 6c6c 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ll_disp_z = []..
-000167a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000167b0: 2020 2020 616c 6c5f 6469 7370 5f79 203d      all_disp_y =
-000167c0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000167d0: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
-000167e0: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
-000167f0: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00016800: 6c5f 7261 6469 7573 203d 205b 5d0d 0a20  l_radius = [].. 
-00016810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016820: 2020 2061 6c6c 5f73 7065 6564 203d 205b     all_speed = [
-00016830: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016840: 2020 2020 2020 2061 6c6c 5f61 6363 203d         all_acc =
-00016850: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016860: 2020 2020 2020 2020 2061 6c6c 5f64 6972           all_dir
-00016870: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-00016880: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016890: 2020 2020 2020 2020 2020 616c 6c5f 636c            all_cl
-000168a0: 7573 7465 725f 636c 6173 7320 3d20 5b5d  uster_class = []
-000168b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000168c0: 2020 2020 2020 616c 6c5f 6469 7374 616e        all_distan
-000168d0: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-000168e0: 5d0d 0a0d 0a0d 0a0d 0a0d 0a20 2020 2020  ]..........     
-000168f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00016900: 6f72 2028 6b2c 7629 2069 6e20 616c 6c5f  or (k,v) in all_
-00016910: 7370 6f74 735f 7472 6163 6b73 2e69 7465  spots_tracks.ite
-00016920: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
-00016930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016940: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00016950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016960: 2063 7572 7265 6e74 5f74 696d 6520 3d20   current_time = 
-00016970: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00016980: 5b6b 5d5b 7365 6c66 2e66 7261 6d65 6964  [k][self.frameid
-00016990: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
-000169a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169b0: 2020 206d 6974 6f74 6963 203d 2061 6c6c     mitotic = all
-000169c0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-000169d0: 5b73 656c 662e 6469 7669 6469 6e67 5f6b  [self.dividing_k
-000169e0: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
-000169f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016a10: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00016a20: 2069 203d 3d20 696e 7428 6375 7272 656e   i == int(curren
-00016a30: 745f 7469 6d65 293a 0d0a 2020 2020 2020  t_time):..      
-00016a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a50: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-00016a60: 6974 6f74 6963 3a0d 0a20 2020 2020 2020  itotic:..       
-00016a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a90: 206d 6974 6f74 6963 5f64 6973 705f 7a2e   mitotic_disp_z.
-00016aa0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00016ab0: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00016ac0: 7a70 6f73 6964 5f6b 6579 5d29 0d0a 2020  zposid_key])..  
-00016ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016af0: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
-00016b00: 7370 5f79 2e61 7070 656e 6428 616c 6c5f  sp_y.append(all_
-00016b10: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00016b20: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
-00016b30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00016b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b50: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00016b60: 6963 5f64 6973 705f 782e 6170 7065 6e64  ic_disp_x.append
-00016b70: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00016b80: 735b 6b5d 5b73 656c 662e 7870 6f73 6964  s[k][self.xposid
-00016b90: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00016ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bc0: 6d69 746f 7469 635f 7261 6469 7573 2e61  mitotic_radius.a
-00016bd0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00016be0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e72  tracks[k][self.r
-00016bf0: 6164 6975 735f 6b65 795d 290d 0a20 2020  adius_key])..   
-00016c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c20: 2020 2020 206d 6974 6f74 6963 5f73 7065       mitotic_spe
-00016c30: 6564 2e61 7070 656e 6428 616c 6c5f 7370  ed.append(all_sp
-00016c40: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00016c50: 6c66 2e73 7065 6564 5f6b 6579 5d29 0d0a  lf.speed_key])..
-00016c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c80: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00016c90: 6163 632e 6170 7065 6e64 2861 6c6c 5f73  acc.append(all_s
-00016ca0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00016cb0: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
-00016cc0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00016cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cf0: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
-00016d00: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
-00016d10: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-00016d20: 6b73 5b6b 5d5b 7365 6c66 2e6d 6f74 696f  ks[k][self.motio
-00016d30: 6e5f 616e 676c 655f 6b65 795d 290d 0a20  n_angle_key]).. 
-00016d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d60: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
-00016d70: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00016d80: 6b2e 6170 7065 6e64 2861 6c6c 5f73 706f  k.append(all_spo
-00016d90: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00016da0: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
-00016db0: 6d61 736b 5f6b 6579 5d29 0d0a 2020 2020  mask_key])..    
-00016dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016de0: 2020 2020 6966 2073 656c 662e 636c 7573      if self.clus
-00016df0: 7465 7263 6c61 7373 5f6b 6579 2069 6e20  terclass_key in 
-00016e00: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00016e10: 5b6b 5d2e 6b65 7973 2829 203a 0d0a 2020  [k].keys() :..  
-00016e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e40: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00016e50: 6f74 6963 5f63 6c75 7374 6572 5f63 6c61  otic_cluster_cla
-00016e60: 7373 2e61 7070 656e 6428 616c 6c5f 7370  ss.append(all_sp
-00016e70: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00016e80: 6c66 2e63 6c75 7374 6572 636c 6173 735f  lf.clusterclass_
-00016e90: 6b65 795d 290d 0a0d 0a0d 0a20 2020 2020  key])......     
-00016ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016eb0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00016ec0: 6e6f 7420 6d69 746f 7469 633a 0d0a 2020  not mitotic:..  
-00016ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ef0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00016f00: 635f 6469 7370 5f7a 2e61 7070 656e 6428  c_disp_z.append(
-00016f10: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00016f20: 5b6b 5d5b 7365 6c66 2e7a 706f 7369 645f  [k][self.zposid_
-00016f30: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00016f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f50: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00016f60: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
-00016f70: 792e 6170 7065 6e64 2861 6c6c 5f73 706f  y.append(all_spo
-00016f80: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00016f90: 662e 7970 6f73 6964 5f6b 6579 5d29 0d0a  f.yposid_key])..
-00016fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fc0: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00016fd0: 7469 635f 6469 7370 5f78 2e61 7070 656e  tic_disp_x.appen
-00016fe0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-00016ff0: 6b73 5b6b 5d5b 7365 6c66 2e78 706f 7369  ks[k][self.xposi
-00017000: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
-00017010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017030: 206e 6f6e 5f6d 6974 6f74 6963 5f72 6164   non_mitotic_rad
-00017040: 6975 732e 6170 7065 6e64 2861 6c6c 5f73  ius.append(all_s
-00017050: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017060: 656c 662e 7261 6469 7573 5f6b 6579 5d29  elf.radius_key])
-00017070: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017090: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-000170a0: 746f 7469 635f 7370 6565 642e 6170 7065  totic_speed.appe
-000170b0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-000170c0: 636b 735b 6b5d 5b73 656c 662e 7370 6565  cks[k][self.spee
-000170d0: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
-000170e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017100: 206e 6f6e 5f6d 6974 6f74 6963 5f61 6363   non_mitotic_acc
-00017110: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00017120: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00017130: 2e61 6363 656c 6572 6174 696f 6e5f 6b65  .acceleration_ke
-00017140: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00017150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017160: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00017170: 5f6d 6974 6f74 6963 5f64 6972 6563 7469  _mitotic_directi
-00017180: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
-00017190: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-000171a0: 636b 735b 6b5d 5b73 656c 662e 6d6f 7469  cks[k][self.moti
-000171b0: 6f6e 5f61 6e67 6c65 5f6b 6579 5d29 0d0a  on_angle_key])..
-000171c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171e0: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-000171f0: 7469 635f 6469 7374 616e 6365 5f63 656c  tic_distance_cel
-00017200: 6c5f 6d61 736b 2e61 7070 656e 6428 616c  l_mask.append(al
-00017210: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00017220: 5d5b 7365 6c66 2e64 6973 7461 6e63 655f  ][self.distance_
-00017230: 6365 6c6c 5f6d 6173 6b5f 6b65 795d 290d  cell_mask_key]).
-00017240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017260: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00017270: 2e63 6c75 7374 6572 636c 6173 735f 6b65  .clusterclass_ke
-00017280: 7920 696e 2061 6c6c 5f73 706f 7473 5f74  y in all_spots_t
-00017290: 7261 636b 735b 6b5d 2e6b 6579 7328 2920  racks[k].keys() 
-000172a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000172b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016330: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00016340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016350: 6675 7475 7265 732e 6170 7065 6e64 2865  futures.append(e
+00016360: 7865 6375 746f 722e 7375 626d 6974 2873  xecutor.submit(s
+00016370: 656c 662e 5f63 6f6d 7075 7465 5f74 656d  elf._compute_tem
+00016380: 706f 7261 6c2c 2069 2c20 616c 6c5f 7370  poral, i, all_sp
+00016390: 6f74 735f 7472 6163 6b73 2929 0d0a 200d  ots_tracks)).. .
+000163a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000163b0: 2020 2020 205b 722e 7265 7375 6c74 2829       [r.result()
+000163c0: 2066 6f72 2072 2069 6e20 636f 6e63 7572   for r in concur
+000163d0: 7265 6e74 2e66 7574 7572 6573 2e61 735f  rent.futures.as_
+000163e0: 636f 6d70 6c65 7465 6428 6675 7475 7265  completed(future
+000163f0: 7329 5d0d 0a0d 0a0d 0a20 2020 2064 6566  s)]......    def
+00016400: 205f 636f 6d70 7574 655f 7465 6d70 6f72   _compute_tempor
+00016410: 616c 2873 656c 662c 2069 2c20 616c 6c5f  al(self, i, all_
+00016420: 7370 6f74 735f 7472 6163 6b73 293a 2020  spots_tracks):  
+00016430: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00016440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016450: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
+00016460: 5f7a 203d 205b 5d0d 0a20 2020 2020 2020  _z = []..       
+00016470: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00016480: 6f74 6963 5f64 6973 705f 7920 3d20 5b5d  otic_disp_y = []
+00016490: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000164a0: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+000164b0: 7370 5f78 203d 205b 5d0d 0a20 2020 2020  sp_x = []..     
+000164c0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000164d0: 6974 6f74 6963 5f72 6164 6975 7320 3d20  itotic_radius = 
+000164e0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+000164f0: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00016500: 7370 6565 6420 3d20 5b5d 0d0a 2020 2020  speed = []..    
+00016510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016520: 6d69 746f 7469 635f 6163 6320 3d20 5b5d  mitotic_acc = []
+00016530: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016540: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+00016550: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00016560: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016570: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00016580: 6963 5f63 6c75 7374 6572 5f63 6c61 7373  ic_cluster_class
+00016590: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000165a0: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+000165b0: 6963 5f64 6973 7461 6e63 655f 6365 6c6c  ic_distance_cell
+000165c0: 5f6d 6173 6b20 3d20 5b5d 0d0a 0d0a 2020  _mask = []....  
+000165d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000165e0: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
+000165f0: 7370 5f7a 203d 205b 5d0d 0a20 2020 2020  sp_z = []..     
+00016600: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00016610: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00016620: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
+00016630: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00016640: 6d69 746f 7469 635f 6469 7370 5f78 203d  mitotic_disp_x =
+00016650: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016660: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00016670: 6f74 6963 5f72 6164 6975 7320 3d20 5b5d  otic_radius = []
+00016680: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016690: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+000166a0: 635f 7370 6565 6420 3d20 5b5d 0d0a 2020  c_speed = []..  
+000166b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166c0: 2020 6e6f 6e5f 6d69 746f 7469 635f 6163    non_mitotic_ac
+000166d0: 6320 3d20 5b5d 0d0a 2020 2020 2020 2020  c = []..        
+000166e0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+000166f0: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
+00016700: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
+00016710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016720: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+00016730: 5f63 6c75 7374 6572 5f63 6c61 7373 203d  _cluster_class =
+00016740: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016750: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00016760: 6f74 6963 5f64 6973 7461 6e63 655f 6365  otic_distance_ce
+00016770: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 2020  ll_mask = []..  
+00016780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016790: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000167a0: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+000167b0: 5f7a 203d 205b 5d0d 0a20 2020 2020 2020  _z = []..       
+000167c0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+000167d0: 5f64 6973 705f 7920 3d20 5b5d 0d0a 2020  _disp_y = []..  
+000167e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000167f0: 2020 616c 6c5f 6469 7370 5f78 203d 205b    all_disp_x = [
+00016800: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016810: 2020 2020 2020 2061 6c6c 5f72 6164 6975         all_radiu
+00016820: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00016830: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00016840: 7370 6565 6420 3d20 5b5d 0d0a 2020 2020  speed = []..    
+00016850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016860: 616c 6c5f 6163 6320 3d20 5b5d 0d0a 2020  all_acc = []..  
+00016870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016880: 2020 616c 6c5f 6469 7265 6374 696f 6e61    all_directiona
+00016890: 6c5f 6368 616e 6765 203d 205b 5d0d 0a20  l_change = [].. 
+000168a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168b0: 2020 2061 6c6c 5f63 6c75 7374 6572 5f63     all_cluster_c
+000168c0: 6c61 7373 203d 205b 5d0d 0a20 2020 2020  lass = []..     
+000168d0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000168e0: 6c6c 5f64 6973 7461 6e63 655f 6365 6c6c  ll_distance_cell
+000168f0: 5f6d 6173 6b20 3d20 5b5d 0d0a 0d0a 0d0a  _mask = []......
+00016900: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00016910: 2020 2020 2020 2020 666f 7220 286b 2c76          for (k,v
+00016920: 2920 696e 2061 6c6c 5f73 706f 7473 5f74  ) in all_spots_t
+00016930: 7261 636b 732e 6974 656d 7328 293a 0d0a  racks.items():..
+00016940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016950: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00016960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016970: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00016980: 745f 7469 6d65 203d 2061 6c6c 5f73 706f  t_time = all_spo
+00016990: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+000169a0: 662e 6672 616d 6569 645f 6b65 795d 0d0a  f.frameid_key]..
+000169b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169c0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+000169d0: 7469 6320 3d20 616c 6c5f 7370 6f74 735f  tic = all_spots_
+000169e0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e64  tracks[k][self.d
+000169f0: 6976 6964 696e 675f 6b65 795d 0d0a 2020  ividing_key]..  
+00016a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a10: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00016a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a30: 2020 2020 2020 2069 6620 6920 3d3d 2069         if i == i
+00016a40: 6e74 2863 7572 7265 6e74 5f74 696d 6529  nt(current_time)
+00016a50: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00016a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a70: 2020 2020 2069 6620 6d69 746f 7469 633a       if mitotic:
+00016a80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016aa0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+00016ab0: 635f 6469 7370 5f7a 2e61 7070 656e 6428  c_disp_z.append(
+00016ac0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00016ad0: 5b6b 5d5b 7365 6c66 2e7a 706f 7369 645f  [k][self.zposid_
+00016ae0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00016af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b00: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00016b10: 6974 6f74 6963 5f64 6973 705f 792e 6170  itotic_disp_y.ap
+00016b20: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00016b30: 7261 636b 735b 6b5d 5b73 656c 662e 7970  racks[k][self.yp
+00016b40: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00016b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b70: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
+00016b80: 5f78 2e61 7070 656e 6428 616c 6c5f 7370  _x.append(all_sp
+00016b90: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00016ba0: 6c66 2e78 706f 7369 645f 6b65 795d 290d  lf.xposid_key]).
+00016bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016bd0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+00016be0: 5f72 6164 6975 732e 6170 7065 6e64 2861  _radius.append(a
+00016bf0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00016c00: 6b5d 5b73 656c 662e 7261 6469 7573 5f6b  k][self.radius_k
+00016c10: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00016c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c30: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00016c40: 746f 7469 635f 7370 6565 642e 6170 7065  totic_speed.appe
+00016c50: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00016c60: 636b 735b 6b5d 5b73 656c 662e 7370 6565  cks[k][self.spee
+00016c70: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
+00016c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ca0: 206d 6974 6f74 6963 5f61 6363 2e61 7070   mitotic_acc.app
+00016cb0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00016cc0: 6163 6b73 5b6b 5d5b 7365 6c66 2e61 6363  acks[k][self.acc
+00016cd0: 656c 6572 6174 696f 6e5f 6b65 795d 290d  eleration_key]).
+00016ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d00: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+00016d10: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00016d20: 6e67 652e 6170 7065 6e64 2861 6c6c 5f73  nge.append(all_s
+00016d30: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00016d40: 656c 662e 6d6f 7469 6f6e 5f61 6e67 6c65  elf.motion_angle
+00016d50: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00016d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d80: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
+00016d90: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
+00016da0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00016db0: 6b73 5b6b 5d5b 7365 6c66 2e64 6973 7461  ks[k][self.dista
+00016dc0: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
+00016dd0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+00016de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016df0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00016e00: 7365 6c66 2e63 6c75 7374 6572 636c 6173  self.clusterclas
+00016e10: 735f 6b65 7920 696e 2061 6c6c 5f73 706f  s_key in all_spo
+00016e20: 7473 5f74 7261 636b 735b 6b5d 2e6b 6579  ts_tracks[k].key
+00016e30: 7328 2920 3a0d 0a20 2020 2020 2020 2020  s() :..         
+00016e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e60: 2020 2020 2020 6d69 746f 7469 635f 636c        mitotic_cl
+00016e70: 7573 7465 725f 636c 6173 732e 6170 7065  uster_class.appe
+00016e80: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00016e90: 636b 735b 6b5d 5b73 656c 662e 636c 7573  cks[k][self.clus
+00016ea0: 7465 7263 6c61 7373 5f6b 6579 5d29 0d0a  terclass_key])..
+00016eb0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00016ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ed0: 2020 2020 2020 6966 206e 6f74 206d 6974        if not mit
+00016ee0: 6f74 6963 3a0d 0a20 2020 2020 2020 2020  otic:..         
+00016ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f00: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00016f10: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00016f20: 7a2e 6170 7065 6e64 2861 6c6c 5f73 706f  z.append(all_spo
+00016f30: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00016f40: 662e 7a70 6f73 6964 5f6b 6579 5d29 0d0a  f.zposid_key])..
+00016f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f70: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
+00016f80: 7469 635f 6469 7370 5f79 2e61 7070 656e  tic_disp_y.appen
+00016f90: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00016fa0: 6b73 5b6b 5d5b 7365 6c66 2e79 706f 7369  ks[k][self.yposi
+00016fb0: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
+00016fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fe0: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
+00016ff0: 705f 782e 6170 7065 6e64 2861 6c6c 5f73  p_x.append(all_s
+00017000: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00017010: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
+00017020: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017040: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00017050: 746f 7469 635f 7261 6469 7573 2e61 7070  totic_radius.app
+00017060: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00017070: 6163 6b73 5b6b 5d5b 7365 6c66 2e72 6164  acks[k][self.rad
+00017080: 6975 735f 6b65 795d 290d 0a20 2020 2020  ius_key])..     
+00017090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170b0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f73     non_mitotic_s
+000170c0: 7065 6564 2e61 7070 656e 6428 616c 6c5f  peed.append(all_
+000170d0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000170e0: 7365 6c66 2e73 7065 6564 5f6b 6579 5d29  self.speed_key])
+000170f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017110: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00017120: 746f 7469 635f 6163 632e 6170 7065 6e64  totic_acc.append
+00017130: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00017140: 735b 6b5d 5b73 656c 662e 6163 6365 6c65  s[k][self.accele
+00017150: 7261 7469 6f6e 5f6b 6579 5d29 0d0a 2020  ration_key])..  
+00017160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017180: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00017190: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
+000171a0: 616e 6765 2e61 7070 656e 6428 616c 6c5f  ange.append(all_
+000171b0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000171c0: 7365 6c66 2e6d 6f74 696f 6e5f 616e 676c  self.motion_angl
+000171d0: 655f 6b65 795d 290d 0a20 2020 2020 2020  e_key])..       
+000171e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017200: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
+00017210: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
+00017220: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017230: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017240: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00017250: 736b 5f6b 6579 5d29 0d0a 2020 2020 2020  sk_key])..      
+00017260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017280: 2020 6966 2073 656c 662e 636c 7573 7465    if self.cluste
+00017290: 7263 6c61 7373 5f6b 6579 2069 6e20 616c  rclass_key in al
+000172a0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+000172b0: 5d2e 6b65 7973 2829 203a 0d0a 2020 2020  ].keys() :..    
 000172c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172d0: 2020 6e6f 6e5f 6d69 746f 7469 635f 636c    non_mitotic_cl
-000172e0: 7573 7465 725f 636c 6173 732e 6170 7065  uster_class.appe
-000172f0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017300: 636b 735b 6b5d 5b73 656c 662e 636c 7573  cks[k][self.clus
-00017310: 7465 7263 6c61 7373 5f6b 6579 5d29 0d0a  terclass_key])..
-00017320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017340: 2020 2020 616c 6c5f 6469 7370 5f7a 2e61      all_disp_z.a
-00017350: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00017360: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e7a  tracks[k][self.z
-00017370: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
-00017380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017390: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000173a0: 6c6c 5f64 6973 705f 792e 6170 7065 6e64  ll_disp_y.append
-000173b0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-000173c0: 735b 6b5d 5b73 656c 662e 7970 6f73 6964  s[k][self.yposid
-000173d0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-000173e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173f0: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
-00017400: 7370 5f78 2e61 7070 656e 6428 616c 6c5f  sp_x.append(all_
-00017410: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00017420: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
-00017430: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017450: 2020 2020 2061 6c6c 5f72 6164 6975 732e       all_radius.
-00017460: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00017470: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00017480: 7261 6469 7573 5f6b 6579 5d29 0d0a 2020  radius_key])..  
-00017490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174b0: 616c 6c5f 7370 6565 642e 6170 7065 6e64  all_speed.append
-000174c0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-000174d0: 735b 6b5d 5b73 656c 662e 7370 6565 645f  s[k][self.speed_
-000174e0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-000174f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017500: 2020 2020 2020 2020 2061 6c6c 5f61 6363           all_acc
-00017510: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00017520: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00017530: 2e61 6363 656c 6572 6174 696f 6e5f 6b65  .acceleration_ke
-00017540: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00017550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017560: 2020 2020 2020 2061 6c6c 5f64 6972 6563         all_direc
-00017570: 7469 6f6e 616c 5f63 6861 6e67 652e 6170  tional_change.ap
-00017580: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00017590: 7261 636b 735b 6b5d 5b73 656c 662e 6d6f  racks[k][self.mo
-000175a0: 7469 6f6e 5f61 6e67 6c65 5f6b 6579 5d29  tion_angle_key])
-000175b0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000175c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175d0: 2020 2020 2020 2061 6c6c 5f64 6973 7461         all_dista
-000175e0: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-000175f0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00017600: 7261 636b 735b 6b5d 5b73 656c 662e 6469  racks[k][self.di
-00017610: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00017620: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00017630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017640: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00017650: 662e 636c 7573 7465 7263 6c61 7373 5f6b  f.clusterclass_k
-00017660: 6579 2069 6e20 616c 6c5f 7370 6f74 735f  ey in all_spots_
-00017670: 7472 6163 6b73 5b6b 5d2e 6b65 7973 2829  tracks[k].keys()
-00017680: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
-00017690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172e0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+000172f0: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
+00017300: 6c61 7373 2e61 7070 656e 6428 616c 6c5f  lass.append(all_
+00017310: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00017320: 7365 6c66 2e63 6c75 7374 6572 636c 6173  self.clusterclas
+00017330: 735f 6b65 795d 290d 0a0d 0a20 2020 2020  s_key])....     
+00017340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017350: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00017360: 5f64 6973 705f 7a2e 6170 7065 6e64 2861  _disp_z.append(a
+00017370: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00017380: 6b5d 5b73 656c 662e 7a70 6f73 6964 5f6b  k][self.zposid_k
+00017390: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+000173a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173b0: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+000173c0: 5f79 2e61 7070 656e 6428 616c 6c5f 7370  _y.append(all_sp
+000173d0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+000173e0: 6c66 2e79 706f 7369 645f 6b65 795d 290d  lf.yposid_key]).
+000173f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017410: 2020 2061 6c6c 5f64 6973 705f 782e 6170     all_disp_x.ap
+00017420: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00017430: 7261 636b 735b 6b5d 5b73 656c 662e 7870  racks[k][self.xp
+00017440: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00017450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017460: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00017470: 6c5f 7261 6469 7573 2e61 7070 656e 6428  l_radius.append(
+00017480: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017490: 5b6b 5d5b 7365 6c66 2e72 6164 6975 735f  [k][self.radius_
+000174a0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+000174b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174c0: 2020 2020 2020 2020 2061 6c6c 5f73 7065           all_spe
+000174d0: 6564 2e61 7070 656e 6428 616c 6c5f 7370  ed.append(all_sp
+000174e0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+000174f0: 6c66 2e73 7065 6564 5f6b 6579 5d29 0d0a  lf.speed_key])..
+00017500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017520: 2020 616c 6c5f 6163 632e 6170 7065 6e64    all_acc.append
+00017530: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00017540: 735b 6b5d 5b73 656c 662e 6163 6365 6c65  s[k][self.accele
+00017550: 7261 7469 6f6e 5f6b 6579 5d29 0d0a 2020  ration_key])..  
+00017560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017580: 616c 6c5f 6469 7265 6374 696f 6e61 6c5f  all_directional_
+00017590: 6368 616e 6765 2e61 7070 656e 6428 616c  change.append(al
+000175a0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+000175b0: 5d5b 7365 6c66 2e6d 6f74 696f 6e5f 616e  ][self.motion_an
+000175c0: 676c 655f 6b65 795d 2920 2020 0d0a 2020  gle_key])   ..  
+000175d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175f0: 616c 6c5f 6469 7374 616e 6365 5f63 656c  all_distance_cel
+00017600: 6c5f 6d61 736b 2e61 7070 656e 6428 616c  l_mask.append(al
+00017610: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00017620: 5d5b 7365 6c66 2e64 6973 7461 6e63 655f  ][self.distance_
+00017630: 6365 6c6c 5f6d 6173 6b5f 6b65 795d 290d  cell_mask_key]).
+00017640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017660: 2020 2069 6620 7365 6c66 2e63 6c75 7374     if self.clust
+00017670: 6572 636c 6173 735f 6b65 7920 696e 2061  erclass_key in a
+00017680: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00017690: 6b5d 2e6b 6579 7328 2920 3a0d 0a20 2020  k].keys() :..   
 000176a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176b0: 2020 2061 6c6c 5f63 6c75 7374 6572 5f63     all_cluster_c
-000176c0: 6c61 7373 2e61 7070 656e 6428 616c 6c5f  lass.append(all_
-000176d0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-000176e0: 7365 6c66 2e63 6c75 7374 6572 636c 6173  self.clusterclas
-000176f0: 735f 6b65 795d 2920 2020 200d 0a20 2020  s_key])    ..   
-00017700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017720: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+000176b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000176c0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+000176d0: 636c 7573 7465 725f 636c 6173 732e 6170  cluster_class.ap
+000176e0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+000176f0: 7261 636b 735b 6b5d 5b73 656c 662e 636c  racks[k][self.cl
+00017700: 7573 7465 7263 6c61 7373 5f6b 6579 5d29  usterclass_key])
+00017710: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00017720: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017740: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
-00017750: 7a20 3d20 6e70 2e61 6273 286e 702e 6469  z = np.abs(np.di
-00017760: 6666 286d 6974 6f74 6963 5f64 6973 705f  ff(mitotic_disp_
-00017770: 7a29 290d 0a20 2020 2020 2020 2020 2020  z))..           
-00017780: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00017790: 5f64 6973 705f 7920 3d20 6e70 2e61 6273  _disp_y = np.abs
-000177a0: 286e 702e 6469 6666 286d 6974 6f74 6963  (np.diff(mitotic
-000177b0: 5f64 6973 705f 7929 290d 0a20 2020 2020  _disp_y))..     
-000177c0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000177d0: 6974 6f74 6963 5f64 6973 705f 7820 3d20  itotic_disp_x = 
-000177e0: 6e70 2e61 6273 286e 702e 6469 6666 286d  np.abs(np.diff(m
-000177f0: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
-00017800: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00017810: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
-00017820: 6963 5f64 6973 705f 7a20 3d20 6e70 2e61  ic_disp_z = np.a
-00017830: 6273 286e 702e 6469 6666 286e 6f6e 5f6d  bs(np.diff(non_m
-00017840: 6974 6f74 6963 5f64 6973 705f 7a29 290d  itotic_disp_z)).
-00017850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017860: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00017870: 5f64 6973 705f 7920 3d20 6e70 2e61 6273  _disp_y = np.abs
-00017880: 286e 702e 6469 6666 286e 6f6e 5f6d 6974  (np.diff(non_mit
-00017890: 6f74 6963 5f64 6973 705f 7929 290d 0a20  otic_disp_y)).. 
-000178a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178b0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-000178c0: 6973 705f 7820 3d20 6e70 2e61 6273 286e  isp_x = np.abs(n
-000178d0: 702e 6469 6666 286e 6f6e 5f6d 6974 6f74  p.diff(non_mitot
-000178e0: 6963 5f64 6973 705f 7829 290d 0a0d 0a20  ic_disp_x)).... 
-000178f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017900: 2020 2061 6c6c 5f64 6973 705f 7a20 3d20     all_disp_z = 
-00017910: 6e70 2e61 6273 286e 702e 6469 6666 2861  np.abs(np.diff(a
-00017920: 6c6c 5f64 6973 705f 7a29 290d 0a20 2020  ll_disp_z))..   
-00017930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017940: 2061 6c6c 5f64 6973 705f 7920 3d20 6e70   all_disp_y = np
-00017950: 2e61 6273 286e 702e 6469 6666 2861 6c6c  .abs(np.diff(all
-00017960: 5f64 6973 705f 7929 290d 0a20 2020 2020  _disp_y))..     
-00017970: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00017980: 6c6c 5f64 6973 705f 7820 3d20 6e70 2e61  ll_disp_x = np.a
-00017990: 6273 286e 702e 6469 6666 2861 6c6c 5f64  bs(np.diff(all_d
-000179a0: 6973 705f 7829 290d 0a0d 0a0d 0a20 2020  isp_x))......   
-000179b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000179e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000179f0: 7469 6d65 2e61 7070 656e 6428 6920 2a20  time.append(i * 
-00017a00: 7365 6c66 2e74 6361 6c69 6272 6174 696f  self.tcalibratio
-00017a10: 6e29 0d0a 0d0a 2020 2020 2020 2020 2020  n)....          
-00017a20: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00017a30: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
-00017a40: 6c61 7373 2e61 7070 656e 6428 6e70 2e61  lass.append(np.a
-00017a50: 7361 7272 6179 286d 6974 6f74 6963 5f63  sarray(mitotic_c
-00017a60: 6c75 7374 6572 5f63 6c61 7373 2c20 6474  luster_class, dt
-00017a70: 7970 653d 6e70 2e66 6c6f 6174 3332 2929  ype=np.float32))
-00017a80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017a90: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00017aa0: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
-00017ab0: 6c61 7373 2e61 7070 656e 6428 6e70 2e61  lass.append(np.a
-00017ac0: 7361 7272 6179 286e 6f6e 5f6d 6974 6f74  sarray(non_mitot
-00017ad0: 6963 5f63 6c75 7374 6572 5f63 6c61 7373  ic_cluster_class
-00017ae0: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-00017af0: 3332 2929 0d0a 2020 2020 2020 2020 2020  32))..          
-00017b00: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00017b10: 6c6c 5f63 6c75 7374 6572 5f63 6c61 7373  ll_cluster_class
-00017b20: 2e61 7070 656e 6428 6e70 2e61 7361 7272  .append(np.asarr
-00017b30: 6179 2861 6c6c 5f63 6c75 7374 6572 5f63  ay(all_cluster_c
-00017b40: 6c61 7373 2c20 6474 7970 653d 6e70 2e66  lass, dtype=np.f
-00017b50: 6c6f 6174 3332 2929 0d0a 0d0a 2020 2020  loat32))....    
-00017b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b70: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
-00017b80: 6e5f 6469 7370 5f7a 2e61 7070 656e 6428  n_disp_z.append(
-00017b90: 6e70 2e6d 6561 6e28 6d69 746f 7469 635f  np.mean(mitotic_
-00017ba0: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
-00017bb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017bc0: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
-00017bd0: 6973 705f 7a2e 6170 7065 6e64 286e 702e  isp_z.append(np.
-00017be0: 7374 6428 6d69 746f 7469 635f 6469 7370  std(mitotic_disp
-00017bf0: 5f7a 2929 0d0a 0d0a 2020 2020 2020 2020  _z))....        
-00017c00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017c10: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
-00017c20: 7370 5f79 2e61 7070 656e 6428 6e70 2e6d  sp_y.append(np.m
-00017c30: 6561 6e28 6d69 746f 7469 635f 6469 7370  ean(mitotic_disp
-00017c40: 5f79 2929 0d0a 2020 2020 2020 2020 2020  _y))..          
-00017c50: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00017c60: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
-00017c70: 792e 6170 7065 6e64 286e 702e 7374 6428  y.append(np.std(
-00017c80: 6d69 746f 7469 635f 6469 7370 5f79 2929  mitotic_disp_y))
-00017c90: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00017ca0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00017cb0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f78  otic_mean_disp_x
-00017cc0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00017cd0: 6d69 746f 7469 635f 6469 7370 5f78 2929  mitotic_disp_x))
-00017ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017cf0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00017d00: 6963 5f76 6172 5f64 6973 705f 782e 6170  ic_var_disp_x.ap
-00017d10: 7065 6e64 286e 702e 7374 6428 6d69 746f  pend(np.std(mito
-00017d20: 7469 635f 6469 7370 5f78 2929 0d0a 0d0a  tic_disp_x))....
-00017d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d40: 2020 2020 6966 206c 656e 286d 6974 6f74      if len(mitot
-00017d50: 6963 5f72 6164 6975 7329 203e 2030 3a0d  ic_radius) > 0:.
-00017d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017d70: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00017d80: 746f 7469 635f 6d65 616e 5f72 6164 6975  totic_mean_radiu
-00017d90: 732e 6170 7065 6e64 286e 702e 6d65 616e  s.append(np.mean
-00017da0: 286d 6974 6f74 6963 5f72 6164 6975 7329  (mitotic_radius)
-00017db0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017dc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017dd0: 6d69 746f 7469 635f 7661 725f 7261 6469  mitotic_var_radi
-00017de0: 7573 2e61 7070 656e 6428 6e70 2e73 7464  us.append(np.std
-00017df0: 286d 6974 6f74 6963 5f72 6164 6975 7329  (mitotic_radius)
-00017e00: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00017e10: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00017e20: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
-00017e30: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00017e40: 6d69 746f 7469 635f 7370 6565 6429 290d  mitotic_speed)).
-00017e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017e60: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00017e70: 635f 7661 725f 7370 6565 642e 6170 7065  c_var_speed.appe
-00017e80: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
-00017e90: 635f 7370 6565 6429 290d 0a0d 0a20 2020  c_speed))....   
-00017ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017eb0: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-00017ec0: 616e 5f61 6363 2e61 7070 656e 6428 6e70  an_acc.append(np
-00017ed0: 2e6d 6561 6e28 6d69 746f 7469 635f 6163  .mean(mitotic_ac
-00017ee0: 6329 290d 0a20 2020 2020 2020 2020 2020  c))..           
-00017ef0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00017f00: 746f 7469 635f 7661 725f 6163 632e 6170  totic_var_acc.ap
-00017f10: 7065 6e64 286e 702e 7374 6428 6d69 746f  pend(np.std(mito
-00017f20: 7469 635f 6163 6329 290d 0a0d 0a20 2020  tic_acc))....   
-00017f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f40: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-00017f50: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
-00017f60: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
-00017f70: 6d65 616e 286d 6974 6f74 6963 5f64 6972  mean(mitotic_dir
-00017f80: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
-00017f90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017fa0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00017fb0: 7469 635f 7661 725f 6469 7265 6374 696f  tic_var_directio
-00017fc0: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
-00017fd0: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
-00017fe0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00017ff0: 6e67 6529 290d 0a0d 0a20 2020 2020 2020  nge))....       
-00018000: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018010: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
-00018020: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00018030: 6b2e 6170 7065 6e64 286e 702e 6d65 616e  k.append(np.mean
-00018040: 286d 6974 6f74 6963 5f64 6973 7461 6e63  (mitotic_distanc
-00018050: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a20  e_cell_mask)).. 
-00018060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018070: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00018080: 7661 725f 6469 7374 616e 6365 5f63 656c  var_distance_cel
-00018090: 6c5f 6d61 736b 2e61 7070 656e 6428 6e70  l_mask.append(np
-000180a0: 2e73 7464 286d 6974 6f74 6963 5f64 6973  .std(mitotic_dis
-000180b0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
-000180c0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-000180d0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-000180e0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
-000180f0: 6973 705f 7a2e 6170 7065 6e64 286e 702e  isp_z.append(np.
-00018100: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
-00018110: 5f64 6973 705f 7a29 290d 0a20 2020 2020  _disp_z))..     
-00018120: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018130: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00018140: 7661 725f 6469 7370 5f7a 2e61 7070 656e  var_disp_z.appen
-00018150: 6428 6e70 2e73 7464 286e 6f6e 5f6d 6974  d(np.std(non_mit
-00018160: 6f74 6963 5f64 6973 705f 7a29 290d 0a0d  otic_disp_z))...
-00018170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018180: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00018190: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-000181a0: 792e 6170 7065 6e64 286e 702e 6d65 616e  y.append(np.mean
-000181b0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
-000181c0: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
-000181d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000181e0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-000181f0: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
-00018200: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
-00018210: 5f64 6973 705f 7929 290d 0a0d 0a20 2020  _disp_y))....   
-00018220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018230: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00018240: 635f 6d65 616e 5f64 6973 705f 782e 6170  c_mean_disp_x.ap
-00018250: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
-00018260: 5f6d 6974 6f74 6963 5f64 6973 705f 7829  _mitotic_disp_x)
-00018270: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018280: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00018290: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
-000182a0: 5f78 2e61 7070 656e 6428 6e70 2e73 7464  _x.append(np.std
-000182b0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
-000182c0: 705f 7829 290d 0a0d 0a20 2020 2020 2020  p_x))....       
-000182d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000182e0: 6c65 6e28 6e6f 6e5f 6d69 746f 7469 635f  len(non_mitotic_
-000182f0: 7261 6469 7573 2920 3e20 303a 0d0a 2020  radius) > 0:..  
-00018300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018310: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00018320: 6974 6f74 6963 5f6d 6561 6e5f 7261 6469  itotic_mean_radi
-00018330: 7573 2e61 7070 656e 6428 6e70 2e6d 6561  us.append(np.mea
-00018340: 6e28 6e6f 6e5f 6d69 746f 7469 635f 7261  n(non_mitotic_ra
-00018350: 6469 7573 2929 0d0a 2020 2020 2020 2020  dius))..        
-00018360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018370: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00018380: 5f76 6172 5f72 6164 6975 732e 6170 7065  _var_radius.appe
-00018390: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
-000183a0: 746f 7469 635f 7261 6469 7573 2929 0d0a  totic_radius))..
-000183b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000183c0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000183d0: 6974 6f74 6963 5f6d 6561 6e5f 7370 6565  itotic_mean_spee
-000183e0: 642e 6170 7065 6e64 286e 702e 6d65 616e  d.append(np.mean
-000183f0: 286e 6f6e 5f6d 6974 6f74 6963 5f73 7065  (non_mitotic_spe
-00018400: 6564 2929 0d0a 2020 2020 2020 2020 2020  ed))..          
-00018410: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00018420: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f73  on_mitotic_var_s
-00018430: 7065 6564 2e61 7070 656e 6428 6e70 2e73  peed.append(np.s
-00018440: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f73  td(non_mitotic_s
-00018450: 7065 6564 2929 0d0a 0d0a 2020 2020 2020  peed))....      
-00018460: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018470: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00018480: 6561 6e5f 6163 632e 6170 7065 6e64 286e  ean_acc.append(n
-00018490: 702e 6d65 616e 286e 6f6e 5f6d 6974 6f74  p.mean(non_mitot
-000184a0: 6963 5f61 6363 2929 0d0a 2020 2020 2020  ic_acc))..      
-000184b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000184c0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-000184d0: 6172 5f61 6363 2e61 7070 656e 6428 6e70  ar_acc.append(np
-000184e0: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
-000184f0: 5f61 6363 2929 0d0a 0d0a 2020 2020 2020  _acc))....      
-00018500: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018510: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00018520: 6561 6e5f 6469 7265 6374 696f 6e61 6c5f  ean_directional_
-00018530: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
-00018540: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
-00018550: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
-00018560: 616e 6765 2929 0d0a 2020 2020 2020 2020  ange))..        
-00018570: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018580: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-00018590: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-000185a0: 6e67 652e 6170 7065 6e64 286e 702e 7374  nge.append(np.st
-000185b0: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
-000185c0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-000185d0: 2929 200d 0a0d 0a20 2020 2020 2020 2020  )) ....         
-000185e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000185f0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00018600: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00018610: 6173 6b2e 6170 7065 6e64 286e 702e 6d65  ask.append(np.me
-00018620: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f64  an(non_mitotic_d
-00018630: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00018640: 6b29 290d 0a20 2020 2020 2020 2020 2020  k))..           
-00018650: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00018660: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
-00018670: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00018680: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
-00018690: 6f6e 5f6d 6974 6f74 6963 5f64 6973 7461  on_mitotic_dista
-000186a0: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
-000186b0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-000186c0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-000186d0: 6c5f 6d65 616e 5f64 6973 705f 7a2e 6170  l_mean_disp_z.ap
-000186e0: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
-000186f0: 5f64 6973 705f 7a29 290d 0a20 2020 2020  _disp_z))..     
-00018700: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018710: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
-00018720: 5f7a 2e61 7070 656e 6428 6e70 2e73 7464  _z.append(np.std
-00018730: 2861 6c6c 5f64 6973 705f 7a29 290d 0a0d  (all_disp_z))...
-00018740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018750: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00018760: 616e 5f64 6973 705f 792e 6170 7065 6e64  an_disp_y.append
-00018770: 286e 702e 6d65 616e 2861 6c6c 5f64 6973  (np.mean(all_dis
-00018780: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
-00018790: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000187a0: 616c 6c5f 7661 725f 6469 7370 5f79 2e61  all_var_disp_y.a
-000187b0: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
-000187c0: 5f64 6973 705f 7929 290d 0a0d 0a20 2020  _disp_y))....   
-000187d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187e0: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
-000187f0: 6973 705f 782e 6170 7065 6e64 286e 702e  isp_x.append(np.
-00018800: 6d65 616e 2861 6c6c 5f64 6973 705f 7829  mean(all_disp_x)
-00018810: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018820: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00018830: 7661 725f 6469 7370 5f78 2e61 7070 656e  var_disp_x.appen
-00018840: 6428 6e70 2e73 7464 2861 6c6c 5f64 6973  d(np.std(all_dis
-00018850: 705f 7829 290d 0a0d 0a20 2020 2020 2020  p_x))....       
-00018860: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00018870: 6c65 6e28 616c 6c5f 7261 6469 7573 2920  len(all_radius) 
-00018880: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
-00018890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188a0: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
-000188b0: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
-000188c0: 2e6d 6561 6e28 616c 6c5f 7261 6469 7573  .mean(all_radius
-000188d0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000188e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188f0: 7365 6c66 2e61 6c6c 5f76 6172 5f72 6164  self.all_var_rad
-00018900: 6975 732e 6170 7065 6e64 286e 702e 7374  ius.append(np.st
-00018910: 6428 616c 6c5f 7261 6469 7573 2929 0d0a  d(all_radius))..
-00018920: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018930: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-00018940: 6561 6e5f 7370 6565 642e 6170 7065 6e64  ean_speed.append
-00018950: 286e 702e 6d65 616e 2861 6c6c 5f73 7065  (np.mean(all_spe
-00018960: 6564 2929 0d0a 2020 2020 2020 2020 2020  ed))..          
-00018970: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00018980: 6c6c 5f76 6172 5f73 7065 6564 2e61 7070  ll_var_speed.app
-00018990: 656e 6428 6e70 2e73 7464 2861 6c6c 5f73  end(np.std(all_s
-000189a0: 7065 6564 2929 0d0a 0d0a 2020 2020 2020  peed))....      
-000189b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000189c0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6163 632e  lf.all_mean_acc.
-000189d0: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
-000189e0: 6c6c 5f61 6363 2929 0d0a 2020 2020 2020  ll_acc))..      
-000189f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018a00: 6c66 2e61 6c6c 5f76 6172 5f61 6363 2e61  lf.all_var_acc.a
-00018a10: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
-00018a20: 5f61 6363 2929 0d0a 0d0a 0d0a 0d0a 2020  _acc))........  
-00018a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a40: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
-00018a50: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00018a60: 6765 2e61 7070 656e 6428 6e70 2e6d 6561  ge.append(np.mea
-00018a70: 6e28 616c 6c5f 6469 7265 6374 696f 6e61  n(all_directiona
-00018a80: 6c5f 6368 616e 6765 2929 0d0a 2020 2020  l_change))..    
-00018a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018aa0: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6972  self.all_var_dir
-00018ab0: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
-00018ac0: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
-00018ad0: 6c5f 6469 7265 6374 696f 6e61 6c5f 6368  l_directional_ch
-00018ae0: 616e 6765 2929 0d0a 0d0a 2020 2020 2020  ange))....      
-00018af0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018b00: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7374  lf.all_mean_dist
-00018b10: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
-00018b20: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
-00018b30: 6c5f 6469 7374 616e 6365 5f63 656c 6c5f  l_distance_cell_
-00018b40: 6d61 736b 2929 0d0a 2020 2020 2020 2020  mask))..        
-00018b50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018b60: 2e61 6c6c 5f76 6172 5f64 6973 7461 6e63  .all_var_distanc
-00018b70: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
-00018b80: 6e64 286e 702e 7374 6428 616c 6c5f 6469  nd(np.std(all_di
-00018b90: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00018ba0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00018bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018bc0: 0d0a 2020 2020 2020 2020 0d0a 6465 6620  ..        ..def 
-00018bd0: 626f 756e 6461 7279 5f70 6f69 6e74 7328  boundary_points(
-00018be0: 6d61 736b 2c20 7863 616c 6962 7261 7469  mask, xcalibrati
-00018bf0: 6f6e 2c20 7963 616c 6962 7261 7469 6f6e  on, ycalibration
-00018c00: 2c20 7a63 616c 6962 7261 7469 6f6e 293a  , zcalibration):
-00018c10: 0d0a 0d0a 2020 2020 6e64 696d 203d 206c  ....    ndim = l
-00018c20: 656e 286d 6173 6b2e 7368 6170 6529 0d0a  en(mask.shape)..
-00018c30: 2020 2020 7469 6d65 645f 6d61 736b 203d      timed_mask =
-00018c40: 207b 7d0d 0a20 2020 206d 6173 6b20 3d20   {}..    mask = 
-00018c50: 6d61 736b 203e 2030 0d0a 2020 2020 6d61  mask > 0..    ma
-00018c60: 736b 203d 206d 6173 6b2e 6173 7479 7065  sk = mask.astype
-00018c70: 2827 7569 6e74 3827 290d 0a20 2020 2023  ('uint8')..    #
-00018c80: 2059 5820 7368 6170 6564 206f 626a 6563   YX shaped objec
-00018c90: 740d 0a20 2020 2069 6620 6e64 696d 203d  t..    if ndim =
-00018ca0: 3d20 323a 0d0a 2020 2020 2020 2020 0d0a  = 2:..        ..
-00018cb0: 2020 2020 2020 2020 626f 756e 6461 7279          boundary
-00018cc0: 203d 2066 696e 645f 626f 756e 6461 7269   = find_boundari
-00018cd0: 6573 286d 6173 6b29 0d0a 2020 2020 2020  es(mask)..      
-00018ce0: 2020 7265 6769 6f6e 6365 6e74 726f 6964    regioncentroid
-00018cf0: 203d 2028 302c 2920 2b20 636f 6d70 7574   = (0,) + comput
-00018d00: 655f 6365 6e74 726f 6964 2862 6f75 6e64  e_centroid(bound
-00018d10: 6172 7929 200d 0a20 2020 2020 2020 2069  ary) ..        i
-00018d20: 6e64 6963 6573 203d 206e 702e 7768 6572  ndices = np.wher
-00018d30: 6528 626f 756e 6461 7279 203e 2030 290d  e(boundary > 0).
-00018d40: 0a20 2020 2020 2020 2072 6561 6c5f 696e  .        real_in
-00018d50: 6469 6365 7320 3d20 6e70 2e74 7261 6e73  dices = np.trans
-00018d60: 706f 7365 286e 702e 6173 6172 7261 7928  pose(np.asarray(
-00018d70: 696e 6469 6365 732c 2064 7479 7065 3d6e  indices, dtype=n
-00018d80: 702e 666c 6f61 7433 3229 292e 636f 7079  p.float32)).copy
-00018d90: 2829 0d0a 0d0a 2020 2020 2020 2020 666f  ()....        fo
-00018da0: 7220 6a20 696e 2072 616e 6765 2830 2c20  r j in range(0, 
-00018db0: 6c65 6e28 7265 616c 5f69 6e64 6963 6573  len(real_indices
-00018dc0: 2929 3a0d 0a0d 0a20 2020 2020 2020 2020  )):....         
-00018dd0: 2020 2072 6561 6c5f 696e 6469 6365 735b     real_indices[
-00018de0: 6a5d 5b30 5d20 3d20 7265 616c 5f69 6e64  j][0] = real_ind
-00018df0: 6963 6573 5b6a 5d5b 305d 202a 2079 6361  ices[j][0] * yca
-00018e00: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-00018e10: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
-00018e20: 6365 735b 6a5d 5b31 5d20 3d20 7265 616c  ces[j][1] = real
-00018e30: 5f69 6e64 6963 6573 5b6a 5d5b 315d 202a  _indices[j][1] *
-00018e40: 2078 6361 6c69 6272 6174 696f 6e0d 0a0d   xcalibration...
-00018e50: 0a20 2020 2020 2020 2074 7265 6520 3d20  .        tree = 
-00018e60: 7370 6174 6961 6c2e 634b 4454 7265 6528  spatial.cKDTree(
-00018e70: 7265 616c 5f69 6e64 6963 6573 290d 0a20  real_indices).. 
-00018e80: 2020 2020 2020 2023 2054 6869 7320 6f62         # This ob
-00018e90: 6a65 6374 2063 6f6e 7461 696e 7320 6c69  ject contains li
-00018ea0: 7374 206f 6620 616c 6c20 7468 6520 706f  st of all the po
-00018eb0: 696e 7473 2066 6f72 2061 6c6c 2074 6865  ints for all the
-00018ec0: 206c 6162 656c 7320 696e 2074 6865 204d   labels in the M
-00018ed0: 6173 6b20 696d 6167 6520 7769 7468 2074  ask image with t
-00018ee0: 6865 206c 6162 656c 2069 6420 616e 6420  he label id and 
-00018ef0: 766f 6c75 6d65 206f 6620 6561 6368 206c  volume of each l
-00018f00: 6162 656c 0d0a 2020 2020 2020 2020 7469  abel..        ti
-00018f10: 6d65 645f 6d61 736b 5b73 7472 2830 295d  med_mask[str(0)]
-00018f20: 203d 205b 7472 6565 2c20 696e 6469 6365   = [tree, indice
-00018f30: 732c 2072 6567 696f 6e63 656e 7472 6f69  s, regioncentroi
-00018f40: 645d 0d0a 0d0a 2020 2020 2320 5459 5820  d]....    # TYX 
-00018f50: 7368 6170 6564 206f 626a 6563 740d 0a20  shaped object.. 
-00018f60: 2020 2069 6620 6e64 696d 203d 3d20 333a     if ndim == 3:
-00018f70: 0d0a 0d0a 0d0a 2020 2020 2020 2020 666f  ......        fo
-00018f80: 7220 6920 696e 2074 7164 6d28 7261 6e67  r i in tqdm(rang
-00018f90: 6528 302c 206d 6173 6b2e 7368 6170 655b  e(0, mask.shape[
-00018fa0: 305d 2929 3a0d 0a20 2020 2020 2020 2020  0])):..         
-00018fb0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00018fc0: 2020 2020 2020 2020 2062 6f75 6e64 6172           boundar
-00018fd0: 7920 3d20 6669 6e64 5f62 6f75 6e64 6172  y = find_boundar
-00018fe0: 6965 7328 6d61 736b 5b69 2c3a 5d29 0d0a  ies(mask[i,:])..
-00018ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019000: 7265 6769 6f6e 6365 6e74 726f 6964 203d  regioncentroid =
-00019010: 2028 302c 2920 2b20 636f 6d70 7574 655f   (0,) + compute_
-00019020: 6365 6e74 726f 6964 2862 6f75 6e64 6172  centroid(boundar
-00019030: 7929 200d 0a20 2020 2020 2020 2020 2020  y) ..           
-00019040: 2020 2020 2069 6e64 6963 6573 203d 206e       indices = n
-00019050: 702e 7768 6572 6528 626f 756e 6461 7279  p.where(boundary
-00019060: 203e 2030 290d 0a20 2020 2020 2020 2020   > 0)..         
-00019070: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
-00019080: 6365 7320 3d20 6e70 2e74 7261 6e73 706f  ces = np.transpo
-00019090: 7365 286e 702e 6173 6172 7261 7928 696e  se(np.asarray(in
-000190a0: 6469 6365 732c 2064 7479 7065 3d6e 702e  dices, dtype=np.
-000190b0: 666c 6f61 7433 3229 292e 636f 7079 2829  float32)).copy()
-000190c0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000190d0: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
-000190e0: 6765 2830 2c20 6c65 6e28 7265 616c 5f69  ge(0, len(real_i
-000190f0: 6e64 6963 6573 2929 3a0d 0a0d 0a20 2020  ndices)):....   
-00019100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019110: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-00019120: 5b30 5d20 3d20 7265 616c 5f69 6e64 6963  [0] = real_indic
-00019130: 6573 5b6a 5d5b 305d 202a 2079 6361 6c69  es[j][0] * ycali
-00019140: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
-00019150: 2020 2020 2020 2020 2020 2020 2072 6561               rea
-00019160: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
-00019170: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
-00019180: 5d5b 315d 202a 2078 6361 6c69 6272 6174  ][1] * xcalibrat
-00019190: 696f 6e0d 0a0d 0a20 2020 2020 2020 2020  ion....         
-000191a0: 2020 2020 2020 2074 7265 6520 3d20 7370         tree = sp
-000191b0: 6174 6961 6c2e 634b 4454 7265 6528 7265  atial.cKDTree(re
-000191c0: 616c 5f69 6e64 6963 6573 290d 0a0d 0a20  al_indices).... 
-000191d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000191e0: 696d 6564 5f6d 6173 6b5b 7374 7228 6929  imed_mask[str(i)
-000191f0: 5d20 3d20 5b74 7265 652c 2069 6e64 6963  ] = [tree, indic
-00019200: 6573 2c20 7265 6769 6f6e 6365 6e74 726f  es, regioncentro
-00019210: 6964 5d0d 0a20 2020 2020 2020 2020 2020  id]..           
-00019220: 200d 0a20 2020 2023 2054 5a59 5820 7368   ..    # TZYX sh
-00019230: 6170 6564 206f 626a 6563 740d 0a20 2020  aped object..   
-00019240: 2069 6620 6e64 696d 203d 3d20 343a 0d0a   if ndim == 4:..
-00019250: 2020 2020 2020 2020 7072 696e 7428 274d          print('M
-00019260: 6173 6b73 206d 6164 6520 696e 746f 2061  asks made into a
-00019270: 2034 4420 6379 6c69 6e64 6572 2c20 7570   4D cylinder, up
-00019280: 2729 0d0a 2020 2020 2020 2020 626f 756e  ')..        boun
-00019290: 6461 7279 203d 206e 702e 7a65 726f 7328  dary = np.zeros(
-000192a0: 0d0a 2020 2020 2020 2020 2020 2020 5b6d  ..            [m
-000192b0: 6173 6b2e 7368 6170 655b 305d 2c20 6d61  ask.shape[0], ma
-000192c0: 736b 2e73 6861 7065 5b31 5d2c 206d 6173  sk.shape[1], mas
-000192d0: 6b2e 7368 6170 655b 325d 2c20 6d61 736b  k.shape[2], mask
-000192e0: 2e73 6861 7065 5b33 5d5d 0d0a 2020 2020  .shape[3]]..    
-000192f0: 2020 2020 290d 0a20 2020 2020 2020 2066      )..        f
-00019300: 6f72 2069 2069 6e20 7261 6e67 6528 302c  or i in range(0,
-00019310: 206d 6173 6b2e 7368 6170 655b 305d 293a   mask.shape[0]):
-00019320: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-00019330: 2020 2020 2020 2020 2020 2020 626f 756e              boun
-00019340: 6461 7279 5b69 2c3a 5d20 3d20 6669 6e64  dary[i,:] = find
-00019350: 5f62 6f75 6e64 6172 6965 7328 6d61 736b  _boundaries(mask
-00019360: 5b69 2c3a 5d29 0d0a 2020 2020 2020 2020  [i,:])..        
-00019370: 2020 2020 7265 6769 6f6e 6365 6e74 726f      regioncentro
-00019380: 6964 203d 2063 6f6d 7075 7465 5f63 656e  id = compute_cen
-00019390: 7472 6f69 6428 626f 756e 6461 7279 5b69  troid(boundary[i
-000193a0: 2c3a 5d29 200d 0a20 2020 2020 2020 2020  ,:]) ..         
-000193b0: 2020 2069 6e64 6963 6573 203d 206e 702e     indices = np.
-000193c0: 7768 6572 6528 626f 756e 6461 7279 5b69  where(boundary[i
-000193d0: 2c3a 5d20 3e20 3029 0d0a 2020 2020 2020  ,:] > 0)..      
-000193e0: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
-000193f0: 6573 203d 206e 702e 7472 616e 7370 6f73  es = np.transpos
-00019400: 6528 6e70 2e61 7361 7272 6179 2869 6e64  e(np.asarray(ind
-00019410: 6963 6573 2c20 6474 7970 653d 6e70 2e66  ices, dtype=np.f
-00019420: 6c6f 6174 3332 2929 2e63 6f70 7928 290d  loat32)).copy().
-00019430: 0a0d 0a20 2020 2020 2020 2020 2020 2066  ...            f
-00019440: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
-00019450: 206c 656e 2872 6561 6c5f 696e 6469 6365   len(real_indice
-00019460: 7329 293a 0d0a 0d0a 2020 2020 2020 2020  s)):....        
-00019470: 2020 2020 2020 2020 2020 2020 7265 616c              real
-00019480: 5f69 6e64 6963 6573 5b6a 5d5b 305d 203d  _indices[j][0] =
-00019490: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-000194a0: 5b30 5d20 2a20 7a63 616c 6962 7261 7469  [0] * zcalibrati
-000194b0: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
-000194c0: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
-000194d0: 6963 6573 5b6a 5d5b 315d 203d 2072 6561  ices[j][1] = rea
-000194e0: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
-000194f0: 2a20 7963 616c 6962 7261 7469 6f6e 0d0a  * ycalibration..
-00019500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019510: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
-00019520: 5b6a 5d5b 325d 203d 2072 6561 6c5f 696e  [j][2] = real_in
-00019530: 6469 6365 735b 6a5d 5b32 5d20 2a20 7863  dices[j][2] * xc
-00019540: 616c 6962 7261 7469 6f6e 0d0a 0d0a 2020  alibration....  
-00019550: 2020 2020 2020 2020 2020 7472 6565 203d            tree =
-00019560: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
-00019570: 2872 6561 6c5f 696e 6469 6365 7329 0d0a  (real_indices)..
-00019580: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-00019590: 645f 6d61 736b 5b73 7472 2869 295d 203d  d_mask[str(i)] =
-000195a0: 205b 7472 6565 2c20 696e 6469 6365 732c   [tree, indices,
-000195b0: 2072 6567 696f 6e63 656e 7472 6f69 645d   regioncentroid]
-000195c0: 0d0a 2020 2020 7072 696e 7428 2743 6f6d  ..    print('Com
-000195d0: 7075 7465 6420 7468 6520 626f 756e 6461  puted the bounda
-000195e0: 7279 2070 6f69 6e74 7327 290d 0a0d 0a20  ry points').... 
-000195f0: 2020 2072 6574 7572 6e20 7469 6d65 645f     return timed_
-00019600: 6d61 736b 2c20 626f 756e 6461 7279 2020  mask, boundary  
-00019610: 2020 2020 2020 0d0a 0d0a 6465 6620 636f        ....def co
-00019620: 6d70 7574 655f 6365 6e74 726f 6964 2862  mpute_centroid(b
-00019630: 696e 6172 795f 696d 6167 6529 3a0d 0a20  inary_image):.. 
-00019640: 2020 2023 2045 6e73 7572 6520 6269 6e61     # Ensure bina
-00019650: 7279 2069 6d61 6765 2069 7320 6120 4e75  ry image is a Nu
-00019660: 6d50 7920 6172 7261 790d 0a20 2020 2062  mPy array..    b
-00019670: 696e 6172 795f 696d 6167 6520 3d20 6e70  inary_image = np
-00019680: 2e61 7272 6179 2862 696e 6172 795f 696d  .array(binary_im
-00019690: 6167 6529 0d0a 0d0a 2020 2020 7768 6974  age)....    whit
-000196a0: 655f 7069 7865 6c73 203d 206e 702e 7768  e_pixels = np.wh
-000196b0: 6572 6528 6269 6e61 7279 5f69 6d61 6765  ere(binary_image
-000196c0: 203d 3d20 3129 0d0a 2020 2020 6e75 6d5f   == 1)..    num_
-000196d0: 7069 7865 6c73 203d 206c 656e 2877 6869  pixels = len(whi
-000196e0: 7465 5f70 6978 656c 735b 305d 290d 0a0d  te_pixels[0])...
-000196f0: 0a20 2020 2023 2043 6f6d 7075 7465 2074  .    # Compute t
-00019700: 6865 2063 656e 7472 6f69 6420 6f66 2074  he centroid of t
-00019710: 6865 2077 6869 7465 2070 6978 656c 7320  he white pixels 
-00019720: 696e 2074 6865 2062 6f75 6e64 6172 7920  in the boundary 
-00019730: 696d 6167 650d 0a20 2020 2063 656e 7472  image..    centr
-00019740: 6f69 6420 3d20 6e70 2e7a 6572 6f73 2862  oid = np.zeros(b
-00019750: 696e 6172 795f 696d 6167 652e 6e64 696d  inary_image.ndim
-00019760: 290d 0a20 2020 2066 6f72 2064 696d 2069  )..    for dim i
-00019770: 6e20 7261 6e67 6528 6269 6e61 7279 5f69  n range(binary_i
-00019780: 6d61 6765 2e6e 6469 6d29 3a0d 0a20 2020  mage.ndim):..   
-00019790: 2020 2020 2063 656e 7472 6f69 645b 6469       centroid[di
-000197a0: 6d5d 203d 2077 6869 7465 5f70 6978 656c  m] = white_pixel
-000197b0: 735b 6469 6d5d 2e73 756d 2829 202f 206e  s[dim].sum() / n
-000197c0: 756d 5f70 6978 656c 730d 0a0d 0a20 2020  um_pixels....   
-000197d0: 2072 6574 7572 6e20 6365 6e74 726f 6964   return centroid
-000197e0: 0d0a 0d0a 0d0a 0d0a 200d 0a0d 0a64 6566  ........ ....def
-000197f0: 2067 6574 5f63 7376 5f64 6174 6128 6373   get_csv_data(cs
-00019800: 7629 3a0d 0a0d 0a20 2020 2020 2020 2064  v):....        d
-00019810: 6174 6173 6574 203d 2070 642e 7265 6164  ataset = pd.read
-00019820: 5f63 7376 280d 0a20 2020 2020 2020 2020  _csv(..         
-00019830: 2020 2063 7376 2c20 6465 6c69 6d69 7465     csv, delimite
-00019840: 723d 222c 222c 2065 6e63 6f64 696e 673d  r=",", encoding=
-00019850: 2275 6e69 636f 6465 5f65 7363 6170 6522  "unicode_escape"
-00019860: 2c20 6c6f 775f 6d65 6d6f 7279 3d46 616c  , low_memory=Fal
-00019870: 7365 0d0a 2020 2020 2020 2020 295b 333a  se..        )[3:
-00019880: 5d0d 0a20 2020 2020 2020 2064 6174 6173  ]..        datas
-00019890: 6574 5f69 6e64 6578 203d 2064 6174 6173  et_index = datas
-000198a0: 6574 2e69 6e64 6578 0d0a 2020 2020 2020  et.index..      
-000198b0: 2020 7265 7475 726e 2064 6174 6173 6574    return dataset
-000198c0: 2c20 6461 7461 7365 745f 696e 6465 780d  , dataset_index.
-000198d0: 0a20 2020 200d 0a64 6566 2067 6574 5f73  .    ..def get_s
-000198e0: 706f 745f 6461 7461 7365 7428 7370 6f74  pot_dataset(spot
-000198f0: 5f64 6174 6173 6574 2c20 7472 6163 6b5f  _dataset, track_
-00019900: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-00019910: 7973 2c20 7863 616c 6962 7261 7469 6f6e  ys, xcalibration
-00019920: 2c20 7963 616c 6962 7261 7469 6f6e 2c20  , ycalibration, 
-00019930: 7a63 616c 6962 7261 7469 6f6e 2c20 4174  zcalibration, At
-00019940: 7472 6962 7574 6542 6f78 6e61 6d65 2c20  tributeBoxname, 
-00019950: 6465 7465 6374 696f 6e63 6861 6e6e 656c  detectionchannel
-00019960: 293a 0d0a 2020 2020 2020 2020 416c 6c56  ):..        AllV
-00019970: 616c 7565 7320 3d20 7b7d 0d0a 2020 2020  alues = {}..    
-00019980: 2020 2020 706f 7369 7820 3d20 7472 6163      posix = trac
-00019990: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-000199a0: 6b65 7973 5b22 706f 7369 7822 5d0d 0a20  keys["posix"].. 
-000199b0: 2020 2020 2020 2070 6f73 6979 203d 2074         posiy = t
-000199c0: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-000199d0: 6f74 5f6b 6579 735b 2270 6f73 6979 225d  ot_keys["posiy"]
-000199e0: 0d0a 2020 2020 2020 2020 706f 7369 7a20  ..        posiz 
-000199f0: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
-00019a00: 5f73 706f 745f 6b65 7973 5b22 706f 7369  _spot_keys["posi
-00019a10: 7a22 5d0d 0a20 2020 2020 2020 2066 7261  z"]..        fra
-00019a20: 6d65 203d 2074 7261 636b 5f61 6e61 6c79  me = track_analy
-00019a30: 7369 735f 7370 6f74 5f6b 6579 735b 2266  sis_spot_keys["f
-00019a40: 7261 6d65 225d 0d0a 2020 2020 2020 2020  rame"]..        
-00019a50: 0d0a 2020 2020 2020 2020 4c6f 6361 7469  ..        Locati
-00019a60: 6f6e 5820 3d20 280d 0a20 2020 2020 2020  onX = (..       
-00019a70: 2020 2020 2073 706f 745f 6461 7461 7365       spot_datase
-00019a80: 745b 706f 7369 785d 2e61 7374 7970 6528  t[posix].astype(
-00019a90: 2266 6c6f 6174 2229 202f 2078 6361 6c69  "float") / xcali
-00019aa0: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
-00019ab0: 2029 2e61 7374 7970 6528 2269 6e74 2229   ).astype("int")
-00019ac0: 0d0a 2020 2020 2020 2020 4c6f 6361 7469  ..        Locati
-00019ad0: 6f6e 5920 3d20 280d 0a20 2020 2020 2020  onY = (..       
-00019ae0: 2020 2020 2073 706f 745f 6461 7461 7365       spot_datase
-00019af0: 745b 706f 7369 795d 2e61 7374 7970 6528  t[posiy].astype(
-00019b00: 2266 6c6f 6174 2229 202f 2079 6361 6c69  "float") / ycali
-00019b10: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
-00019b20: 2029 2e61 7374 7970 6528 2269 6e74 2229   ).astype("int")
-00019b30: 0d0a 2020 2020 2020 2020 4c6f 6361 7469  ..        Locati
-00019b40: 6f6e 5a20 3d20 280d 0a20 2020 2020 2020  onZ = (..       
-00019b50: 2020 2020 2073 706f 745f 6461 7461 7365       spot_datase
-00019b60: 745b 706f 7369 7a5d 2e61 7374 7970 6528  t[posiz].astype(
-00019b70: 2266 6c6f 6174 2229 202f 207a 6361 6c69  "float") / zcali
-00019b80: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
-00019b90: 2029 2e61 7374 7970 6528 2269 6e74 2229   ).astype("int")
-00019ba0: 0d0a 2020 2020 2020 2020 4c6f 6361 7469  ..        Locati
-00019bb0: 6f6e 5420 3d20 2873 706f 745f 6461 7461  onT = (spot_data
-00019bc0: 7365 745b 6672 616d 655d 2e61 7374 7970  set[frame].astyp
-00019bd0: 6528 2266 6c6f 6174 2229 292e 6173 7479  e("float")).asty
-00019be0: 7065 2822 696e 7422 290d 0a20 2020 2020  pe("int")..     
-00019bf0: 2020 200d 0a0d 0a20 2020 2020 2020 2069     ....        i
-00019c00: 676e 6f72 655f 7661 6c75 6573 203d 205b  gnore_values = [
-00019c10: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-00019c20: 706f 745f 6b65 7973 5b22 6d65 616e 5f69  pot_keys["mean_i
-00019c30: 6e74 656e 7369 7479 225d 2c74 7261 636b  ntensity"],track
-00019c40: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-00019c50: 6579 735b 2274 6f74 616c 5f69 6e74 656e  eys["total_inten
-00019c60: 7369 7479 225d 5d20 0d0a 2020 2020 2020  sity"]] ..      
-00019c70: 2020 666f 7220 286b 2c76 2920 696e 2074    for (k,v) in t
-00019c80: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-00019c90: 6f74 5f6b 6579 732e 6974 656d 7328 293a  ot_keys.items():
-00019ca0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00019cb0: 2020 2020 6966 2064 6574 6563 7469 6f6e      if detection
-00019cc0: 6368 616e 6e65 6c20 3d3d 2031 3a0d 0a20  channel == 1:.. 
-00019cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ce0: 2020 2020 6966 206b 203d 3d20 226d 6561      if k == "mea
-00019cf0: 6e5f 696e 7465 6e73 6974 795f 6368 3222  n_intensity_ch2"
-00019d00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00019d10: 2020 2020 2020 2020 2020 2020 2020 7661                va
-00019d20: 6c75 6520 3d20 7472 6163 6b5f 616e 616c  lue = track_anal
-00019d30: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-00019d40: 6d65 616e 5f69 6e74 656e 7369 7479 225d  mean_intensity"]
-00019d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019d60: 2020 2020 2020 2020 2020 2020 2041 6c6c               All
-00019d70: 5661 6c75 6573 5b76 616c 7565 5d20 3d20  Values[value] = 
-00019d80: 7370 6f74 5f64 6174 6173 6574 5b76 5d2e  spot_dataset[v].
-00019d90: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
-00019da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019db0: 2020 2020 2020 6966 206b 203d 3d20 2274        if k == "t
-00019dc0: 6f74 616c 5f69 6e74 656e 7369 7479 5f63  otal_intensity_c
-00019dd0: 6832 223a 0d0a 2020 2020 2020 2020 2020  h2":..          
-00019de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019df0: 2076 616c 7565 203d 2074 7261 636b 5f61   value = track_a
-00019e00: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-00019e10: 735b 2274 6f74 616c 5f69 6e74 656e 7369  s["total_intensi
-00019e20: 7479 225d 0d0a 2020 2020 2020 2020 2020  ty"]..          
-00019e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019e40: 2041 6c6c 5661 6c75 6573 5b76 616c 7565   AllValues[value
-00019e50: 5d20 3d20 7370 6f74 5f64 6174 6173 6574  ] = spot_dataset
-00019e60: 5b76 5d2e 6173 7479 7065 2822 666c 6f61  [v].astype("floa
-00019e70: 7422 2920 2020 2020 2020 0d0a 0d0a 2020  t")       ....  
-00019e80: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00019e90: 2076 206e 6f74 2069 6e20 6967 6e6f 7265   v not in ignore
-00019ea0: 5f76 616c 7565 733a 0d0a 2020 2020 2020  _values:..      
-00019eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ec0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00019ed0: 2020 2020 2020 2020 2020 416c 6c56 616c            AllVal
-00019ee0: 7565 735b 765d 203d 2073 706f 745f 6461  ues[v] = spot_da
-00019ef0: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
-00019f00: 2266 6c6f 6174 2229 0d0a 0d0a 2020 2020  "float")....    
-00019f10: 2020 2020 416c 6c56 616c 7565 735b 706f      AllValues[po
-00019f20: 7369 785d 203d 2072 6f75 6e64 284c 6f63  six] = round(Loc
-00019f30: 6174 696f 6e58 2c33 290d 0a20 2020 2020  ationX,3)..     
-00019f40: 2020 2041 6c6c 5661 6c75 6573 5b70 6f73     AllValues[pos
-00019f50: 6979 5d20 3d20 726f 756e 6428 4c6f 6361  iy] = round(Loca
-00019f60: 7469 6f6e 592c 3329 0d0a 2020 2020 2020  tionY,3)..      
-00019f70: 2020 416c 6c56 616c 7565 735b 706f 7369    AllValues[posi
-00019f80: 7a5d 203d 2072 6f75 6e64 284c 6f63 6174  z] = round(Locat
-00019f90: 696f 6e5a 2c33 290d 0a20 2020 2020 2020  ionZ,3)..       
-00019fa0: 2041 6c6c 5661 6c75 6573 5b66 7261 6d65   AllValues[frame
-00019fb0: 5d20 3d20 726f 756e 6428 4c6f 6361 7469  ] = round(Locati
-00019fc0: 6f6e 542c 3329 0d0a 2020 2020 2020 2020  onT,3)..        
-00019fd0: 4174 7472 6962 7574 6569 6473 203d 205b  Attributeids = [
-00019fe0: 5d0d 0a20 2020 2020 2020 2041 7474 7269  ]..        Attri
-00019ff0: 6275 7465 6964 732e 6170 7065 6e64 2841  buteids.append(A
-0001a000: 7474 7269 6275 7465 426f 786e 616d 6529  ttributeBoxname)
-0001a010: 0d0a 2020 2020 2020 2020 666f 7220 6174  ..        for at
-0001a020: 7472 6962 7574 656e 616d 6520 696e 2041  tributename in A
-0001a030: 6c6c 5661 6c75 6573 2e6b 6579 7328 293a  llValues.keys():
-0001a040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a050: 4174 7472 6962 7574 6569 6473 2e61 7070  Attributeids.app
-0001a060: 656e 6428 6174 7472 6962 7574 656e 616d  end(attributenam
-0001a070: 6529 2020 2020 0d0a 2020 2020 2020 2020  e)    ..        
-0001a080: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
-0001a090: 2020 2020 2020 2020 7265 7475 726e 2041          return A
-0001a0a0: 7474 7269 6275 7465 6964 732c 2041 6c6c  ttributeids, All
-0001a0b0: 5661 6c75 6573 2020 2020 200d 0a20 2020  Values     ..   
-0001a0c0: 200d 0a64 6566 2067 6574 5f74 7261 636b   ..def get_track
-0001a0d0: 5f64 6174 6173 6574 2874 7261 636b 5f64  _dataset(track_d
-0001a0e0: 6174 6173 6574 2c20 7472 6163 6b5f 616e  ataset, track_an
-0001a0f0: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-0001a100: 2c20 7472 6163 6b5f 616e 616c 7973 6973  , track_analysis
-0001a110: 5f74 7261 636b 5f6b 6579 732c 2054 7261  _track_keys, Tra
-0001a120: 636b 4174 7472 6962 7574 6542 6f78 6e61  ckAttributeBoxna
-0001a130: 6d65 293a 0d0a 0d0a 2020 2020 2020 2020  me):....        
-0001a140: 416c 6c54 7261 636b 5661 6c75 6573 203d  AllTrackValues =
-0001a150: 207b 7d0d 0a20 2020 2020 2020 2074 7261   {}..        tra
-0001a160: 636b 5f69 6420 3d20 7472 6163 6b5f 616e  ck_id = track_an
-0001a170: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-0001a180: 5b22 7472 6163 6b5f 6964 225d 0d0a 2020  ["track_id"]..  
-0001a190: 2020 2020 2020 5469 6420 3d20 7472 6163        Tid = trac
-0001a1a0: 6b5f 6461 7461 7365 745b 7472 6163 6b5f  k_dataset[track_
-0001a1b0: 6964 5d2e 6173 7479 7065 2822 666c 6f61  id].astype("floa
-0001a1c0: 7422 290d 0a20 2020 2020 2020 0d0a 2020  t")..       ..  
-0001a1d0: 2020 2020 2020 416c 6c54 7261 636b 5661        AllTrackVa
-0001a1e0: 6c75 6573 5b74 7261 636b 5f69 645d 203d  lues[track_id] =
-0001a1f0: 2054 6964 0d0a 2020 2020 2020 0d0a 2020   Tid..      ..  
-0001a200: 2020 2020 2020 666f 7220 286b 2c20 7629        for (k, v)
-0001a210: 2069 6e20 7472 6163 6b5f 616e 616c 7973   in track_analys
-0001a220: 6973 5f74 7261 636b 5f6b 6579 732e 6974  is_track_keys.it
-0001a230: 656d 7328 293a 0d0a 0d0a 2020 2020 2020  ems():....      
-0001a240: 2020 2020 2020 2020 2020 7820 3d20 7472            x = tr
-0001a250: 6163 6b5f 6461 7461 7365 745b 765d 2e61  ack_dataset[v].a
-0001a260: 7374 7970 6528 2266 6c6f 6174 2229 0d0a  stype("float")..
-0001a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a280: 6d69 6e76 616c 203d 206d 696e 2878 290d  minval = min(x).
-0001a290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a2a0: 206d 6178 7661 6c20 3d20 6d61 7828 7829   maxval = max(x)
-0001a2b0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001a2c0: 2020 2020 6966 206d 696e 7661 6c20 3e20      if minval > 
-0001a2d0: 3020 616e 6420 6d61 7876 616c 203c 3d20  0 and maxval <= 
-0001a2e0: 313a 0d0a 0d0a 2020 2020 2020 2020 2020  1:....          
-0001a2f0: 2020 2020 2020 2020 2020 7820 3d20 7820            x = x 
-0001a300: 2b20 310d 0a0d 0a20 2020 2020 2020 2020  + 1....         
-0001a310: 2020 2020 2020 2041 6c6c 5472 6163 6b56         AllTrackV
-0001a320: 616c 7565 735b 6b5d 203d 2072 6f75 6e64  alues[k] = round
-0001a330: 2878 2c20 3329 0d0a 0d0a 2020 2020 2020  (x, 3)....      
-0001a340: 2020 5472 6163 6b41 7474 7269 6275 7465    TrackAttribute
-0001a350: 6964 7320 3d20 5b5d 0d0a 2020 2020 2020  ids = []..      
-0001a360: 2020 5472 6163 6b41 7474 7269 6275 7465    TrackAttribute
-0001a370: 6964 732e 6170 7065 6e64 2854 7261 636b  ids.append(Track
-0001a380: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
-0001a390: 290d 0a20 2020 2020 2020 2066 6f72 2061  )..        for a
-0001a3a0: 7474 7269 6275 7465 6e61 6d65 2069 6e20  ttributename in 
-0001a3b0: 7472 6163 6b5f 616e 616c 7973 6973 5f74  track_analysis_t
-0001a3c0: 7261 636b 5f6b 6579 732e 6b65 7973 2829  rack_keys.keys()
-0001a3d0: 3a0d 0a20 2020 2020 2020 2020 2020 2054  :..            T
-0001a3e0: 7261 636b 4174 7472 6962 7574 6569 6473  rackAttributeids
-0001a3f0: 2e61 7070 656e 6428 6174 7472 6962 7574  .append(attribut
-0001a400: 656e 616d 6529 2020 2020 0d0a 2020 2020  ename)    ..    
-0001a410: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0001a420: 2054 7261 636b 4174 7472 6962 7574 6569   TrackAttributei
-0001a430: 6473 2c20 416c 6c54 7261 636b 5661 6c75  ds, AllTrackValu
-0001a440: 6573 0d0a 2020 2020 0d0a 6465 6620 6765  es..    ..def ge
-0001a450: 745f 6564 6765 735f 6461 7461 7365 7428  t_edges_dataset(
-0001a460: 6564 6765 735f 6461 7461 7365 742c 2065  edges_dataset, e
-0001a470: 6467 6573 5f64 6174 6173 6574 5f69 6e64  dges_dataset_ind
-0001a480: 6578 2c20 7472 6163 6b5f 616e 616c 7973  ex, track_analys
-0001a490: 6973 5f73 706f 745f 6b65 7973 2c20 7472  is_spot_keys, tr
-0001a4a0: 6163 6b5f 616e 616c 7973 6973 5f65 6467  ack_analysis_edg
-0001a4b0: 6573 5f6b 6579 7329 3a0d 0a0d 0a20 2020  es_keys):....   
-0001a4c0: 2020 2020 2041 6c6c 4564 6765 7356 616c       AllEdgesVal
-0001a4d0: 7565 7320 3d20 7b7d 0d0a 2020 2020 2020  ues = {}..      
-0001a4e0: 2020 7472 6163 6b5f 6964 203d 2074 7261    track_id = tra
-0001a4f0: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-0001a500: 5f6b 6579 735b 2274 7261 636b 5f69 6422  _keys["track_id"
-0001a510: 5d0d 0a20 2020 2020 2020 2054 6964 203d  ]..        Tid =
-0001a520: 2065 6467 6573 5f64 6174 6173 6574 5b74   edges_dataset[t
-0001a530: 7261 636b 5f69 645d 2e61 7374 7970 6528  rack_id].astype(
-0001a540: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
-0001a550: 2020 696e 6469 6365 7320 3d20 6e70 2e77    indices = np.w
-0001a560: 6865 7265 2854 6964 203d 3d20 3029 0d0a  here(Tid == 0)..
-0001a570: 2020 2020 2020 2020 6d61 7874 7261 636b          maxtrack
-0001a580: 5f69 6420 3d20 6d61 7828 5469 6429 0d0a  _id = max(Tid)..
-0001a590: 2020 2020 2020 2020 636f 6e64 6974 696f          conditio
-0001a5a0: 6e5f 696e 6469 6365 7320 3d20 6564 6765  n_indices = edge
-0001a5b0: 735f 6461 7461 7365 745f 696e 6465 785b  s_dataset_index[
-0001a5c0: 696e 6469 6365 735d 0d0a 2020 2020 2020  indices]..      
-0001a5d0: 2020 5469 645b 636f 6e64 6974 696f 6e5f    Tid[condition_
-0001a5e0: 696e 6469 6365 735d 203d 206d 6178 7472  indices] = maxtr
-0001a5f0: 6163 6b5f 6964 202b 2031 0d0a 2020 2020  ack_id + 1..    
-0001a600: 2020 2020 416c 6c45 6467 6573 5661 6c75      AllEdgesValu
-0001a610: 6573 5b74 7261 636b 5f69 645d 203d 2054  es[track_id] = T
-0001a620: 6964 0d0a 0d0a 2020 2020 2020 2020 666f  id....        fo
-0001a630: 7220 6b20 696e 2074 7261 636b 5f61 6e61  r k in track_ana
-0001a640: 6c79 7369 735f 6564 6765 735f 6b65 7973  lysis_edges_keys
-0001a650: 2e76 616c 7565 7328 293a 0d0a 0d0a 2020  .values():....  
-0001a660: 2020 2020 2020 2020 2020 6966 206b 2021            if k !
-0001a670: 3d20 7472 6163 6b5f 6964 3a0d 0a20 2020  = track_id:..   
-0001a680: 2020 2020 2020 2020 2020 2020 2078 203d               x =
-0001a690: 2065 6467 6573 5f64 6174 6173 6574 5b6b   edges_dataset[k
-0001a6a0: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
-0001a6b0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-0001a6c0: 2020 2020 2041 6c6c 4564 6765 7356 616c       AllEdgesVal
-0001a6d0: 7565 735b 6b5d 203d 2078 2020 200d 0a20  ues[k] = x   .. 
-0001a6e0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0001a6f0: 2020 7265 7475 726e 2041 6c6c 4564 6765    return AllEdge
-0001a700: 7356 616c 7565 7320 2020 0d0a 2020 2020  sValues   ..    
-0001a710: 0d0a 2020 2020 2020 200d 0a20 2020 200d  ..       ..    .
-0001a720: 0a64 6566 2073 6361 6c65 5f76 616c 7565  .def scale_value
-0001a730: 2878 2c20 7363 616c 6520 3d20 3235 3520  (x, scale = 255 
-0001a740: 2a20 3235 3529 3a0d 0a0d 0a0d 0a20 2020  * 255):......   
-0001a750: 2020 7265 7475 726e 2078 202a 2073 6361    return x * sca
-0001a760: 6c65 2020 200d 0a20 2020 200d 0a0d 0a0d  le   ..    .....
-0001a770: 0a64 6566 2070 726f 625f 7369 676d 6f69  .def prob_sigmoi
-0001a780: 6428 7829 3a0d 0a20 2020 2072 6574 7572  d(x):..    retur
-0001a790: 6e20 3120 2d20 6d61 7468 2e65 7870 282d  n 1 - math.exp(-
-0001a7a0: 7829 0d0a 0d0a 0d0a 6465 6620 616e 6775  x)......def angu
-0001a7b0: 6c61 725f 6368 616e 6765 2876 6563 5f30  lar_change(vec_0
-0001a7c0: 2c20 7665 635f 3129 3a0d 0a20 2020 2020  , vec_1):..     
-0001a7d0: 2020 200d 0a20 2020 2020 2020 2076 6563     ..        vec
-0001a7e0: 5f30 203d 2076 6563 5f30 202f 206e 702e  _0 = vec_0 / np.
-0001a7f0: 6c69 6e61 6c67 2e6e 6f72 6d28 7665 635f  linalg.norm(vec_
-0001a800: 3029 0d0a 2020 2020 2020 2020 7665 635f  0)..        vec_
-0001a810: 3120 3d20 7665 635f 3120 2f20 6e70 2e6c  1 = vec_1 / np.l
-0001a820: 696e 616c 672e 6e6f 726d 2876 6563 5f31  inalg.norm(vec_1
-0001a830: 290d 0a20 2020 2020 2020 2061 6e67 6c65  )..        angle
-0001a840: 203d 206e 702e 6172 6363 6f73 286e 702e   = np.arccos(np.
-0001a850: 636c 6970 286e 702e 646f 7428 7665 635f  clip(np.dot(vec_
-0001a860: 302c 2076 6563 5f31 292c 202d 312e 302c  0, vec_1), -1.0,
-0001a870: 2031 2e30 2929 0d0a 2020 2020 2020 2020   1.0))..        
-0001a880: 616e 676c 6520 3d20 616e 676c 6520 2a20  angle = angle * 
-0001a890: 3138 3020 2f20 6e70 2e70 690d 0a20 2020  180 / np.pi..   
-0001a8a0: 2020 2020 2072 6574 7572 6e20 616e 676c       return angl
-0001a8b0: 650d 0a20 2020 2020 0d0a 0d0a 6465 6620  e..     ....def 
-0001a8c0: 6576 616c 5f62 6f6f 6c28 7661 6c75 6529  eval_bool(value)
-0001a8d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001a8e0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-0001a8f0: 6620 7661 6c75 6520 203d 3d20 2754 7275  f value  == 'Tru
-0001a900: 6527 3a20 0d0a 2020 2020 2020 2020 2020  e': ..          
-0001a910: 2020 2020 2020 6469 765f 6b65 7920 3d20        div_key = 
-0001a920: 5472 7565 0d0a 2020 2020 2020 2020 656c  True..        el
-0001a930: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0001a940: 2020 2020 2064 6976 5f6b 6579 203d 2046       div_key = F
-0001a950: 616c 7365 200d 0a0d 0a20 2020 2020 2020  alse ....       
-0001a960: 2072 6574 7572 6e20 6469 765f 6b65 7920   return div_key 
-0001a970: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0001a980: 0a0d 0a64 6566 2063 6865 636b 5f61 6e64  ...def check_and
-0001a990: 5f75 7064 6174 655f 6d61 736b 286d 6173  _update_mask(mas
-0001a9a0: 6b2c 696d 6167 6529 3a0d 0a20 2020 2020  k,image):..     
-0001a9b0: 2020 0d0a 2020 2020 2020 2020 6966 206c    ..        if l
-0001a9c0: 656e 286d 6173 6b2e 7368 6170 6529 203c  en(mask.shape) <
-0001a9d0: 206c 656e 2869 6d61 6765 2e73 6861 7065   len(image.shape
-0001a9e0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0001a9f0: 7570 6461 7465 5f6d 6173 6b20 3d20 6e70  update_mask = np
-0001aa00: 2e7a 6572 6f73 280d 0a20 2020 2020 2020  .zeros(..       
-0001aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa20: 2020 2020 205b 0d0a 2020 2020 2020 2020       [..        
-0001aa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa40: 2020 2020 2020 2020 696d 6167 652e 7368          image.sh
-0001aa50: 6170 655b 305d 2c0d 0a20 2020 2020 2020  ape[0],..       
-0001aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa70: 2020 2020 2020 2020 2069 6d61 6765 2e73           image.s
-0001aa80: 6861 7065 5b31 5d2c 0d0a 2020 2020 2020  hape[1],..      
-0001aa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aaa0: 2020 2020 2020 2020 2020 696d 6167 652e            image.
-0001aab0: 7368 6170 655b 325d 2c0d 0a20 2020 2020  shape[2],..     
-0001aac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aad0: 2020 2020 2020 2020 2020 2069 6d61 6765             image
-0001aae0: 2e73 6861 7065 5b33 5d2c 0d0a 2020 2020  .shape[3],..    
-0001aaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab00: 2020 2020 2020 2020 5d0d 0a20 2020 2020          ]..     
+00017740: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+00017750: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+00017760: 7469 635f 6469 7370 5f7a 203d 206e 702e  tic_disp_z = np.
+00017770: 6162 7328 6e70 2e64 6966 6628 6d69 746f  abs(np.diff(mito
+00017780: 7469 635f 6469 7370 5f7a 2929 0d0a 2020  tic_disp_z))..  
+00017790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177a0: 2020 6d69 746f 7469 635f 6469 7370 5f79    mitotic_disp_y
+000177b0: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
+000177c0: 6628 6d69 746f 7469 635f 6469 7370 5f79  f(mitotic_disp_y
+000177d0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000177e0: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+000177f0: 6469 7370 5f78 203d 206e 702e 6162 7328  disp_x = np.abs(
+00017800: 6e70 2e64 6966 6628 6d69 746f 7469 635f  np.diff(mitotic_
+00017810: 6469 7370 5f78 2929 0d0a 0d0a 2020 2020  disp_x))....    
+00017820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017830: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+00017840: 5f7a 203d 206e 702e 6162 7328 6e70 2e64  _z = np.abs(np.d
+00017850: 6966 6628 6e6f 6e5f 6d69 746f 7469 635f  iff(non_mitotic_
+00017860: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
+00017870: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00017880: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
+00017890: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
+000178a0: 6628 6e6f 6e5f 6d69 746f 7469 635f 6469  f(non_mitotic_di
+000178b0: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
+000178c0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+000178d0: 6d69 746f 7469 635f 6469 7370 5f78 203d  mitotic_disp_x =
+000178e0: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
+000178f0: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+00017900: 5f78 2929 0d0a 0d0a 2020 2020 2020 2020  _x))....        
+00017910: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00017920: 6469 7370 5f7a 203d 206e 702e 6162 7328  disp_z = np.abs(
+00017930: 6e70 2e64 6966 6628 616c 6c5f 6469 7370  np.diff(all_disp
+00017940: 5f7a 2929 0d0a 2020 2020 2020 2020 2020  _z))..          
+00017950: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+00017960: 7370 5f79 203d 206e 702e 6162 7328 6e70  sp_y = np.abs(np
+00017970: 2e64 6966 6628 616c 6c5f 6469 7370 5f79  .diff(all_disp_y
+00017980: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00017990: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+000179a0: 5f78 203d 206e 702e 6162 7328 6e70 2e64  _x = np.abs(np.d
+000179b0: 6966 6628 616c 6c5f 6469 7370 5f78 2929  iff(all_disp_x))
+000179c0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+000179d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000179f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a00: 2020 2020 7365 6c66 2e74 696d 652e 6170      self.time.ap
+00017a10: 7065 6e64 2869 202a 2073 656c 662e 7463  pend(i * self.tc
+00017a20: 616c 6962 7261 7469 6f6e 290d 0a0d 0a20  alibration).... 
+00017a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a40: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00017a50: 636c 7573 7465 725f 636c 6173 732e 6170  cluster_class.ap
+00017a60: 7065 6e64 286e 702e 6173 6172 7261 7928  pend(np.asarray(
+00017a70: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
+00017a80: 636c 6173 732c 2064 7479 7065 3d6e 702e  class, dtype=np.
+00017a90: 666c 6f61 7433 3229 290d 0a20 2020 2020  float32))..     
+00017aa0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017ab0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00017ac0: 636c 7573 7465 725f 636c 6173 732e 6170  cluster_class.ap
+00017ad0: 7065 6e64 286e 702e 6173 6172 7261 7928  pend(np.asarray(
+00017ae0: 6e6f 6e5f 6d69 746f 7469 635f 636c 7573  non_mitotic_clus
+00017af0: 7465 725f 636c 6173 732c 2064 7479 7065  ter_class, dtype
+00017b00: 3d6e 702e 666c 6f61 7433 3229 290d 0a20  =np.float32)).. 
+00017b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b20: 2020 2073 656c 662e 616c 6c5f 636c 7573     self.all_clus
+00017b30: 7465 725f 636c 6173 732e 6170 7065 6e64  ter_class.append
+00017b40: 286e 702e 6173 6172 7261 7928 616c 6c5f  (np.asarray(all_
+00017b50: 636c 7573 7465 725f 636c 6173 732c 2064  cluster_class, d
+00017b60: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00017b70: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00017b80: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00017b90: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
+00017ba0: 7a2e 6170 7065 6e64 286e 702e 6d65 616e  z.append(np.mean
+00017bb0: 286d 6974 6f74 6963 5f64 6973 705f 7a29  (mitotic_disp_z)
+00017bc0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00017bd0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00017be0: 7469 635f 7661 725f 6469 7370 5f7a 2e61  tic_var_disp_z.a
+00017bf0: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
+00017c00: 6f74 6963 5f64 6973 705f 7a29 290d 0a0d  otic_disp_z))...
+00017c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017c20: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00017c30: 635f 6d65 616e 5f64 6973 705f 792e 6170  c_mean_disp_y.ap
+00017c40: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
+00017c50: 6f74 6963 5f64 6973 705f 7929 290d 0a20  otic_disp_y)).. 
+00017c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c70: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00017c80: 7661 725f 6469 7370 5f79 2e61 7070 656e  var_disp_y.appen
+00017c90: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
+00017ca0: 5f64 6973 705f 7929 290d 0a0d 0a20 2020  _disp_y))....   
+00017cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017cc0: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
+00017cd0: 616e 5f64 6973 705f 782e 6170 7065 6e64  an_disp_x.append
+00017ce0: 286e 702e 6d65 616e 286d 6974 6f74 6963  (np.mean(mitotic
+00017cf0: 5f64 6973 705f 7829 290d 0a20 2020 2020  _disp_x))..     
+00017d00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017d10: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
+00017d20: 6469 7370 5f78 2e61 7070 656e 6428 6e70  disp_x.append(np
+00017d30: 2e73 7464 286d 6974 6f74 6963 5f64 6973  .std(mitotic_dis
+00017d40: 705f 7829 290d 0a0d 0a20 2020 2020 2020  p_x))....       
+00017d50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00017d60: 6c65 6e28 6d69 746f 7469 635f 7261 6469  len(mitotic_radi
+00017d70: 7573 2920 3e20 303a 0d0a 2020 2020 2020  us) > 0:..      
+00017d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d90: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00017da0: 6561 6e5f 7261 6469 7573 2e61 7070 656e  ean_radius.appen
+00017db0: 6428 6e70 2e6d 6561 6e28 6d69 746f 7469  d(np.mean(mitoti
+00017dc0: 635f 7261 6469 7573 2929 0d0a 2020 2020  c_radius))..    
+00017dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017de0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00017df0: 5f76 6172 5f72 6164 6975 732e 6170 7065  _var_radius.appe
+00017e00: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
+00017e10: 635f 7261 6469 7573 2929 0d0a 0d0a 2020  c_radius))....  
+00017e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e30: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00017e40: 6561 6e5f 7370 6565 642e 6170 7065 6e64  ean_speed.append
+00017e50: 286e 702e 6d65 616e 286d 6974 6f74 6963  (np.mean(mitotic
+00017e60: 5f73 7065 6564 2929 0d0a 2020 2020 2020  _speed))..      
+00017e70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017e80: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f73  lf.mitotic_var_s
+00017e90: 7065 6564 2e61 7070 656e 6428 6e70 2e73  peed.append(np.s
+00017ea0: 7464 286d 6974 6f74 6963 5f73 7065 6564  td(mitotic_speed
+00017eb0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00017ec0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00017ed0: 6974 6f74 6963 5f6d 6561 6e5f 6163 632e  itotic_mean_acc.
+00017ee0: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
+00017ef0: 6974 6f74 6963 5f61 6363 2929 0d0a 2020  itotic_acc))..  
+00017f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f10: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+00017f20: 6172 5f61 6363 2e61 7070 656e 6428 6e70  ar_acc.append(np
+00017f30: 2e73 7464 286d 6974 6f74 6963 5f61 6363  .std(mitotic_acc
+00017f40: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00017f50: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00017f60: 6974 6f74 6963 5f6d 6561 6e5f 6469 7265  itotic_mean_dire
+00017f70: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
+00017f80: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
+00017f90: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
+00017fa0: 6c5f 6368 616e 6765 2929 0d0a 2020 2020  l_change))..    
+00017fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017fc0: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+00017fd0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00017fe0: 6e67 652e 6170 7065 6e64 286e 702e 7374  nge.append(np.st
+00017ff0: 6428 6d69 746f 7469 635f 6469 7265 6374  d(mitotic_direct
+00018000: 696f 6e61 6c5f 6368 616e 6765 2929 0d0a  ional_change))..
+00018010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018020: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00018030: 6963 5f6d 6561 6e5f 6469 7374 616e 6365  ic_mean_distance
+00018040: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
+00018050: 6428 6e70 2e6d 6561 6e28 6d69 746f 7469  d(np.mean(mitoti
+00018060: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
+00018070: 6d61 736b 2929 0d0a 2020 2020 2020 2020  mask))..        
+00018080: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018090: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
+000180a0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
+000180b0: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
+000180c0: 746f 7469 635f 6469 7374 616e 6365 5f63  totic_distance_c
+000180d0: 656c 6c5f 6d61 736b 2929 0d0a 0d0a 2020  ell_mask))....  
+000180e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180f0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00018100: 6963 5f6d 6561 6e5f 6469 7370 5f7a 2e61  ic_mean_disp_z.a
+00018110: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
+00018120: 6e5f 6d69 746f 7469 635f 6469 7370 5f7a  n_mitotic_disp_z
+00018130: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018140: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00018150: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
+00018160: 705f 7a2e 6170 7065 6e64 286e 702e 7374  p_z.append(np.st
+00018170: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
+00018180: 7370 5f7a 2929 0d0a 0d0a 2020 2020 2020  sp_z))....      
+00018190: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000181a0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+000181b0: 6561 6e5f 6469 7370 5f79 2e61 7070 656e  ean_disp_y.appen
+000181c0: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
+000181d0: 746f 7469 635f 6469 7370 5f79 2929 0d0a  totic_disp_y))..
+000181e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181f0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00018200: 6f74 6963 5f76 6172 5f64 6973 705f 792e  otic_var_disp_y.
+00018210: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
+00018220: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
+00018230: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00018240: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00018250: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+00018260: 6469 7370 5f78 2e61 7070 656e 6428 6e70  disp_x.append(np
+00018270: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
+00018280: 635f 6469 7370 5f78 2929 0d0a 2020 2020  c_disp_x))..    
+00018290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000182a0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+000182b0: 5f76 6172 5f64 6973 705f 782e 6170 7065  _var_disp_x.appe
+000182c0: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
+000182d0: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
+000182e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000182f0: 2020 2020 2020 6966 206c 656e 286e 6f6e        if len(non
+00018300: 5f6d 6974 6f74 6963 5f72 6164 6975 7329  _mitotic_radius)
+00018310: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
+00018320: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018330: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00018340: 6d65 616e 5f72 6164 6975 732e 6170 7065  mean_radius.appe
+00018350: 6e64 286e 702e 6d65 616e 286e 6f6e 5f6d  nd(np.mean(non_m
+00018360: 6974 6f74 6963 5f72 6164 6975 7329 290d  itotic_radius)).
+00018370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018380: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00018390: 6e5f 6d69 746f 7469 635f 7661 725f 7261  n_mitotic_var_ra
+000183a0: 6469 7573 2e61 7070 656e 6428 6e70 2e73  dius.append(np.s
+000183b0: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f72  td(non_mitotic_r
+000183c0: 6164 6975 7329 290d 0a0d 0a20 2020 2020  adius))....     
+000183d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000183e0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+000183f0: 6d65 616e 5f73 7065 6564 2e61 7070 656e  mean_speed.appen
+00018400: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
+00018410: 746f 7469 635f 7370 6565 6429 290d 0a20  totic_speed)).. 
+00018420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018430: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00018440: 7469 635f 7661 725f 7370 6565 642e 6170  tic_var_speed.ap
+00018450: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
+00018460: 6d69 746f 7469 635f 7370 6565 6429 290d  mitotic_speed)).
+00018470: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018480: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00018490: 6d69 746f 7469 635f 6d65 616e 5f61 6363  mitotic_mean_acc
+000184a0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+000184b0: 6e6f 6e5f 6d69 746f 7469 635f 6163 6329  non_mitotic_acc)
+000184c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000184d0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+000184e0: 6d69 746f 7469 635f 7661 725f 6163 632e  mitotic_var_acc.
+000184f0: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
+00018500: 6e5f 6d69 746f 7469 635f 6163 6329 290d  n_mitotic_acc)).
+00018510: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018520: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00018530: 6d69 746f 7469 635f 6d65 616e 5f64 6972  mitotic_mean_dir
+00018540: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
+00018550: 6170 7065 6e64 286e 702e 6d65 616e 286e  append(np.mean(n
+00018560: 6f6e 5f6d 6974 6f74 6963 5f64 6972 6563  on_mitotic_direc
+00018570: 7469 6f6e 616c 5f63 6861 6e67 6529 290d  tional_change)).
+00018580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018590: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+000185a0: 746f 7469 635f 7661 725f 6469 7265 6374  totic_var_direct
+000185b0: 696f 6e61 6c5f 6368 616e 6765 2e61 7070  ional_change.app
+000185c0: 656e 6428 6e70 2e73 7464 286e 6f6e 5f6d  end(np.std(non_m
+000185d0: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
+000185e0: 616c 5f63 6861 6e67 6529 2920 0d0a 0d0a  al_change)) ....
+000185f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018600: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00018610: 6f74 6963 5f6d 6561 6e5f 6469 7374 616e  otic_mean_distan
+00018620: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
+00018630: 656e 6428 6e70 2e6d 6561 6e28 6e6f 6e5f  end(np.mean(non_
+00018640: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
+00018650: 5f63 656c 6c5f 6d61 736b 2929 0d0a 2020  _cell_mask))..  
+00018660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018670: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00018680: 6963 5f76 6172 5f64 6973 7461 6e63 655f  ic_var_distance_
+00018690: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
+000186a0: 286e 702e 7374 6428 6e6f 6e5f 6d69 746f  (np.std(non_mito
+000186b0: 7469 635f 6469 7374 616e 6365 5f63 656c  tic_distance_cel
+000186c0: 6c5f 6d61 736b 2929 0d0a 0d0a 0d0a 2020  l_mask))......  
+000186d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186e0: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+000186f0: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
+00018700: 2e6d 6561 6e28 616c 6c5f 6469 7370 5f7a  .mean(all_disp_z
+00018710: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018720: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00018730: 5f76 6172 5f64 6973 705f 7a2e 6170 7065  _var_disp_z.appe
+00018740: 6e64 286e 702e 7374 6428 616c 6c5f 6469  nd(np.std(all_di
+00018750: 7370 5f7a 2929 0d0a 0d0a 2020 2020 2020  sp_z))....      
+00018760: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018770: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7370  lf.all_mean_disp
+00018780: 5f79 2e61 7070 656e 6428 6e70 2e6d 6561  _y.append(np.mea
+00018790: 6e28 616c 6c5f 6469 7370 5f79 2929 0d0a  n(all_disp_y))..
+000187a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187b0: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+000187c0: 5f64 6973 705f 792e 6170 7065 6e64 286e  _disp_y.append(n
+000187d0: 702e 7374 6428 616c 6c5f 6469 7370 5f79  p.std(all_disp_y
+000187e0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+000187f0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00018800: 6c6c 5f6d 6561 6e5f 6469 7370 5f78 2e61  ll_mean_disp_x.a
+00018810: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
+00018820: 6c5f 6469 7370 5f78 2929 0d0a 2020 2020  l_disp_x))..    
+00018830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018840: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6973  self.all_var_dis
+00018850: 705f 782e 6170 7065 6e64 286e 702e 7374  p_x.append(np.st
+00018860: 6428 616c 6c5f 6469 7370 5f78 2929 0d0a  d(all_disp_x))..
+00018870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018880: 2020 2020 2020 6966 206c 656e 2861 6c6c        if len(all
+00018890: 5f72 6164 6975 7329 203e 2030 3a0d 0a20  _radius) > 0:.. 
+000188a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000188c0: 616c 6c5f 6d65 616e 5f72 6164 6975 732e  all_mean_radius.
+000188d0: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
+000188e0: 6c6c 5f72 6164 6975 7329 290d 0a20 2020  ll_radius))..   
+000188f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018900: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018910: 6c5f 7661 725f 7261 6469 7573 2e61 7070  l_var_radius.app
+00018920: 656e 6428 6e70 2e73 7464 2861 6c6c 5f72  end(np.std(all_r
+00018930: 6164 6975 7329 290d 0a0d 0a20 2020 2020  adius))....     
+00018940: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018950: 656c 662e 616c 6c5f 6d65 616e 5f73 7065  elf.all_mean_spe
+00018960: 6564 2e61 7070 656e 6428 6e70 2e6d 6561  ed.append(np.mea
+00018970: 6e28 616c 6c5f 7370 6565 6429 290d 0a20  n(all_speed)).. 
+00018980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018990: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+000189a0: 7370 6565 642e 6170 7065 6e64 286e 702e  speed.append(np.
+000189b0: 7374 6428 616c 6c5f 7370 6565 6429 290d  std(all_speed)).
+000189c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000189d0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+000189e0: 6d65 616e 5f61 6363 2e61 7070 656e 6428  mean_acc.append(
+000189f0: 6e70 2e6d 6561 6e28 616c 6c5f 6163 6329  np.mean(all_acc)
+00018a00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018a10: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00018a20: 7661 725f 6163 632e 6170 7065 6e64 286e  var_acc.append(n
+00018a30: 702e 7374 6428 616c 6c5f 6163 6329 290d  p.std(all_acc)).
+00018a40: 0a0d 0a0d 0a0d 0a20 2020 2020 2020 2020  .......         
+00018a50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018a60: 616c 6c5f 6d65 616e 5f64 6972 6563 7469  all_mean_directi
+00018a70: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
+00018a80: 6e64 286e 702e 6d65 616e 2861 6c6c 5f64  nd(np.mean(all_d
+00018a90: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00018aa0: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
+00018ab0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018ac0: 6c5f 7661 725f 6469 7265 6374 696f 6e61  l_var_directiona
+00018ad0: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
+00018ae0: 6e70 2e73 7464 2861 6c6c 5f64 6972 6563  np.std(all_direc
+00018af0: 7469 6f6e 616c 5f63 6861 6e67 6529 290d  tional_change)).
+00018b00: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018b10: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00018b20: 6d65 616e 5f64 6973 7461 6e63 655f 6365  mean_distance_ce
+00018b30: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 286e  ll_mask.append(n
+00018b40: 702e 6d65 616e 2861 6c6c 5f64 6973 7461  p.mean(all_dista
+00018b50: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
+00018b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018b70: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+00018b80: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
+00018b90: 6d61 736b 2e61 7070 656e 6428 6e70 2e73  mask.append(np.s
+00018ba0: 7464 2861 6c6c 5f64 6973 7461 6e63 655f  td(all_distance_
+00018bb0: 6365 6c6c 5f6d 6173 6b29 290d 0a20 2020  cell_mask))..   
+00018bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018bd0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00018be0: 2020 200d 0a64 6566 2062 6f75 6e64 6172     ..def boundar
+00018bf0: 795f 706f 696e 7473 286d 6173 6b2c 2078  y_points(mask, x
+00018c00: 6361 6c69 6272 6174 696f 6e2c 2079 6361  calibration, yca
+00018c10: 6c69 6272 6174 696f 6e2c 207a 6361 6c69  libration, zcali
+00018c20: 6272 6174 696f 6e29 3a0d 0a0d 0a20 2020  bration):....   
+00018c30: 206e 6469 6d20 3d20 6c65 6e28 6d61 736b   ndim = len(mask
+00018c40: 2e73 6861 7065 290d 0a20 2020 2074 696d  .shape)..    tim
+00018c50: 6564 5f6d 6173 6b20 3d20 7b7d 0d0a 2020  ed_mask = {}..  
+00018c60: 2020 6d61 736b 203d 206d 6173 6b20 3e20    mask = mask > 
+00018c70: 300d 0a20 2020 206d 6173 6b20 3d20 6d61  0..    mask = ma
+00018c80: 736b 2e61 7374 7970 6528 2775 696e 7438  sk.astype('uint8
+00018c90: 2729 0d0a 2020 2020 2320 5958 2073 6861  ')..    # YX sha
+00018ca0: 7065 6420 6f62 6a65 6374 0d0a 2020 2020  ped object..    
+00018cb0: 6966 206e 6469 6d20 3d3d 2032 3a0d 0a20  if ndim == 2:.. 
+00018cc0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00018cd0: 2062 6f75 6e64 6172 7920 3d20 6669 6e64   boundary = find
+00018ce0: 5f62 6f75 6e64 6172 6965 7328 6d61 736b  _boundaries(mask
+00018cf0: 290d 0a20 2020 2020 2020 2072 6567 696f  )..        regio
+00018d00: 6e63 656e 7472 6f69 6420 3d20 2830 2c29  ncentroid = (0,)
+00018d10: 202b 2063 6f6d 7075 7465 5f63 656e 7472   + compute_centr
+00018d20: 6f69 6428 626f 756e 6461 7279 2920 0d0a  oid(boundary) ..
+00018d30: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
+00018d40: 3d20 6e70 2e77 6865 7265 2862 6f75 6e64  = np.where(bound
+00018d50: 6172 7920 3e20 3029 0d0a 2020 2020 2020  ary > 0)..      
+00018d60: 2020 7265 616c 5f69 6e64 6963 6573 203d    real_indices =
+00018d70: 206e 702e 7472 616e 7370 6f73 6528 6e70   np.transpose(np
+00018d80: 2e61 7361 7272 6179 2869 6e64 6963 6573  .asarray(indices
+00018d90: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+00018da0: 3332 2929 2e63 6f70 7928 290d 0a0d 0a20  32)).copy().... 
+00018db0: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+00018dc0: 7261 6e67 6528 302c 206c 656e 2872 6561  range(0, len(rea
+00018dd0: 6c5f 696e 6469 6365 7329 293a 0d0a 0d0a  l_indices)):....
+00018de0: 2020 2020 2020 2020 2020 2020 7265 616c              real
+00018df0: 5f69 6e64 6963 6573 5b6a 5d5b 305d 203d  _indices[j][0] =
+00018e00: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+00018e10: 5b30 5d20 2a20 7963 616c 6962 7261 7469  [0] * ycalibrati
+00018e20: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+00018e30: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
+00018e40: 315d 203d 2072 6561 6c5f 696e 6469 6365  1] = real_indice
+00018e50: 735b 6a5d 5b31 5d20 2a20 7863 616c 6962  s[j][1] * xcalib
+00018e60: 7261 7469 6f6e 0d0a 0d0a 2020 2020 2020  ration....      
+00018e70: 2020 7472 6565 203d 2073 7061 7469 616c    tree = spatial
+00018e80: 2e63 4b44 5472 6565 2872 6561 6c5f 696e  .cKDTree(real_in
+00018e90: 6469 6365 7329 0d0a 2020 2020 2020 2020  dices)..        
+00018ea0: 2320 5468 6973 206f 626a 6563 7420 636f  # This object co
+00018eb0: 6e74 6169 6e73 206c 6973 7420 6f66 2061  ntains list of a
+00018ec0: 6c6c 2074 6865 2070 6f69 6e74 7320 666f  ll the points fo
+00018ed0: 7220 616c 6c20 7468 6520 6c61 6265 6c73  r all the labels
+00018ee0: 2069 6e20 7468 6520 4d61 736b 2069 6d61   in the Mask ima
+00018ef0: 6765 2077 6974 6820 7468 6520 6c61 6265  ge with the labe
+00018f00: 6c20 6964 2061 6e64 2076 6f6c 756d 6520  l id and volume 
+00018f10: 6f66 2065 6163 6820 6c61 6265 6c0d 0a20  of each label.. 
+00018f20: 2020 2020 2020 2074 696d 6564 5f6d 6173         timed_mas
+00018f30: 6b5b 7374 7228 3029 5d20 3d20 5b74 7265  k[str(0)] = [tre
+00018f40: 652c 2069 6e64 6963 6573 2c20 7265 6769  e, indices, regi
+00018f50: 6f6e 6365 6e74 726f 6964 5d0d 0a0d 0a20  oncentroid].... 
+00018f60: 2020 2023 2054 5958 2073 6861 7065 6420     # TYX shaped 
+00018f70: 6f62 6a65 6374 0d0a 2020 2020 6966 206e  object..    if n
+00018f80: 6469 6d20 3d3d 2033 3a0d 0a0d 0a0d 0a20  dim == 3:...... 
+00018f90: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00018fa0: 7471 646d 2872 616e 6765 2830 2c20 6d61  tqdm(range(0, ma
+00018fb0: 736b 2e73 6861 7065 5b30 5d29 293a 0d0a  sk.shape[0])):..
+00018fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018fe0: 2020 626f 756e 6461 7279 203d 2066 696e    boundary = fin
+00018ff0: 645f 626f 756e 6461 7269 6573 286d 6173  d_boundaries(mas
+00019000: 6b5b 692c 3a5d 290d 0a20 2020 2020 2020  k[i,:])..       
+00019010: 2020 2020 2020 2020 2072 6567 696f 6e63           regionc
+00019020: 656e 7472 6f69 6420 3d20 2830 2c29 202b  entroid = (0,) +
+00019030: 2063 6f6d 7075 7465 5f63 656e 7472 6f69   compute_centroi
+00019040: 6428 626f 756e 6461 7279 2920 0d0a 2020  d(boundary) ..  
+00019050: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00019060: 6469 6365 7320 3d20 6e70 2e77 6865 7265  dices = np.where
+00019070: 2862 6f75 6e64 6172 7920 3e20 3029 0d0a  (boundary > 0)..
+00019080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019090: 7265 616c 5f69 6e64 6963 6573 203d 206e  real_indices = n
+000190a0: 702e 7472 616e 7370 6f73 6528 6e70 2e61  p.transpose(np.a
+000190b0: 7361 7272 6179 2869 6e64 6963 6573 2c20  sarray(indices, 
+000190c0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+000190d0: 2929 2e63 6f70 7928 290d 0a0d 0a20 2020  )).copy()....   
+000190e0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000190f0: 206a 2069 6e20 7261 6e67 6528 302c 206c   j in range(0, l
+00019100: 656e 2872 6561 6c5f 696e 6469 6365 7329  en(real_indices)
+00019110: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
+00019120: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
+00019130: 6e64 6963 6573 5b6a 5d5b 305d 203d 2072  ndices[j][0] = r
+00019140: 6561 6c5f 696e 6469 6365 735b 6a5d 5b30  eal_indices[j][0
+00019150: 5d20 2a20 7963 616c 6962 7261 7469 6f6e  ] * ycalibration
+00019160: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019170: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
+00019180: 6573 5b6a 5d5b 315d 203d 2072 6561 6c5f  es[j][1] = real_
+00019190: 696e 6469 6365 735b 6a5d 5b31 5d20 2a20  indices[j][1] * 
+000191a0: 7863 616c 6962 7261 7469 6f6e 0d0a 0d0a  xcalibration....
+000191b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191c0: 7472 6565 203d 2073 7061 7469 616c 2e63  tree = spatial.c
+000191d0: 4b44 5472 6565 2872 6561 6c5f 696e 6469  KDTree(real_indi
+000191e0: 6365 7329 0d0a 0d0a 2020 2020 2020 2020  ces)....        
+000191f0: 2020 2020 2020 2020 7469 6d65 645f 6d61          timed_ma
+00019200: 736b 5b73 7472 2869 295d 203d 205b 7472  sk[str(i)] = [tr
+00019210: 6565 2c20 696e 6469 6365 732c 2072 6567  ee, indices, reg
+00019220: 696f 6e63 656e 7472 6f69 645d 0d0a 2020  ioncentroid]..  
+00019230: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00019240: 2320 545a 5958 2073 6861 7065 6420 6f62  # TZYX shaped ob
+00019250: 6a65 6374 0d0a 2020 2020 6966 206e 6469  ject..    if ndi
+00019260: 6d20 3d3d 2034 3a0d 0a20 2020 2020 2020  m == 4:..       
+00019270: 2070 7269 6e74 2827 4d61 736b 7320 6d61   print('Masks ma
+00019280: 6465 2069 6e74 6f20 6120 3444 2063 796c  de into a 4D cyl
+00019290: 696e 6465 722c 2075 7027 290d 0a20 2020  inder, up')..   
+000192a0: 2020 2020 2062 6f75 6e64 6172 7920 3d20       boundary = 
+000192b0: 6e70 2e7a 6572 6f73 280d 0a20 2020 2020  np.zeros(..     
+000192c0: 2020 2020 2020 205b 6d61 736b 2e73 6861         [mask.sha
+000192d0: 7065 5b30 5d2c 206d 6173 6b2e 7368 6170  pe[0], mask.shap
+000192e0: 655b 315d 2c20 6d61 736b 2e73 6861 7065  e[1], mask.shape
+000192f0: 5b32 5d2c 206d 6173 6b2e 7368 6170 655b  [2], mask.shape[
+00019300: 335d 5d0d 0a20 2020 2020 2020 2029 0d0a  3]]..        )..
+00019310: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00019320: 2072 616e 6765 2830 2c20 6d61 736b 2e73   range(0, mask.s
+00019330: 6861 7065 5b30 5d29 3a0d 0a20 2020 2020  hape[0]):..     
+00019340: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00019350: 2020 2020 2062 6f75 6e64 6172 795b 692c       boundary[i,
+00019360: 3a5d 203d 2066 696e 645f 626f 756e 6461  :] = find_bounda
+00019370: 7269 6573 286d 6173 6b5b 692c 3a5d 290d  ries(mask[i,:]).
+00019380: 0a20 2020 2020 2020 2020 2020 2072 6567  .            reg
+00019390: 696f 6e63 656e 7472 6f69 6420 3d20 636f  ioncentroid = co
+000193a0: 6d70 7574 655f 6365 6e74 726f 6964 2862  mpute_centroid(b
+000193b0: 6f75 6e64 6172 795b 692c 3a5d 2920 0d0a  oundary[i,:]) ..
+000193c0: 2020 2020 2020 2020 2020 2020 696e 6469              indi
+000193d0: 6365 7320 3d20 6e70 2e77 6865 7265 2862  ces = np.where(b
+000193e0: 6f75 6e64 6172 795b 692c 3a5d 203e 2030  oundary[i,:] > 0
+000193f0: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+00019400: 6561 6c5f 696e 6469 6365 7320 3d20 6e70  eal_indices = np
+00019410: 2e74 7261 6e73 706f 7365 286e 702e 6173  .transpose(np.as
+00019420: 6172 7261 7928 696e 6469 6365 732c 2064  array(indices, d
+00019430: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00019440: 292e 636f 7079 2829 0d0a 0d0a 2020 2020  ).copy()....    
+00019450: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
+00019460: 2072 616e 6765 2830 2c20 6c65 6e28 7265   range(0, len(re
+00019470: 616c 5f69 6e64 6963 6573 2929 3a0d 0a0d  al_indices)):...
+00019480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019490: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
+000194a0: 735b 6a5d 5b30 5d20 3d20 7265 616c 5f69  s[j][0] = real_i
+000194b0: 6e64 6963 6573 5b6a 5d5b 305d 202a 207a  ndices[j][0] * z
+000194c0: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
+000194d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194e0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+000194f0: 5b31 5d20 3d20 7265 616c 5f69 6e64 6963  [1] = real_indic
+00019500: 6573 5b6a 5d5b 315d 202a 2079 6361 6c69  es[j][1] * ycali
+00019510: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+00019520: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+00019530: 6c5f 696e 6469 6365 735b 6a5d 5b32 5d20  l_indices[j][2] 
+00019540: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
+00019550: 5d5b 325d 202a 2078 6361 6c69 6272 6174  ][2] * xcalibrat
+00019560: 696f 6e0d 0a0d 0a20 2020 2020 2020 2020  ion....         
+00019570: 2020 2074 7265 6520 3d20 7370 6174 6961     tree = spatia
+00019580: 6c2e 634b 4454 7265 6528 7265 616c 5f69  l.cKDTree(real_i
+00019590: 6e64 6963 6573 290d 0a20 2020 2020 2020  ndices)..       
+000195a0: 2020 2020 2074 696d 6564 5f6d 6173 6b5b       timed_mask[
+000195b0: 7374 7228 6929 5d20 3d20 5b74 7265 652c  str(i)] = [tree,
+000195c0: 2069 6e64 6963 6573 2c20 7265 6769 6f6e   indices, region
+000195d0: 6365 6e74 726f 6964 5d0d 0a20 2020 2070  centroid]..    p
+000195e0: 7269 6e74 2827 436f 6d70 7574 6564 2074  rint('Computed t
+000195f0: 6865 2062 6f75 6e64 6172 7920 706f 696e  he boundary poin
+00019600: 7473 2729 0d0a 0d0a 2020 2020 7265 7475  ts')....    retu
+00019610: 726e 2074 696d 6564 5f6d 6173 6b2c 2062  rn timed_mask, b
+00019620: 6f75 6e64 6172 7920 2020 2020 2020 200d  oundary        .
+00019630: 0a0d 0a64 6566 2063 6f6d 7075 7465 5f63  ...def compute_c
+00019640: 656e 7472 6f69 6428 6269 6e61 7279 5f69  entroid(binary_i
+00019650: 6d61 6765 293a 0d0a 2020 2020 2320 456e  mage):..    # En
+00019660: 7375 7265 2062 696e 6172 7920 696d 6167  sure binary imag
+00019670: 6520 6973 2061 204e 756d 5079 2061 7272  e is a NumPy arr
+00019680: 6179 0d0a 2020 2020 6269 6e61 7279 5f69  ay..    binary_i
+00019690: 6d61 6765 203d 206e 702e 6172 7261 7928  mage = np.array(
+000196a0: 6269 6e61 7279 5f69 6d61 6765 290d 0a0d  binary_image)...
+000196b0: 0a20 2020 2077 6869 7465 5f70 6978 656c  .    white_pixel
+000196c0: 7320 3d20 6e70 2e77 6865 7265 2862 696e  s = np.where(bin
+000196d0: 6172 795f 696d 6167 6520 3d3d 2031 290d  ary_image == 1).
+000196e0: 0a20 2020 206e 756d 5f70 6978 656c 7320  .    num_pixels 
+000196f0: 3d20 6c65 6e28 7768 6974 655f 7069 7865  = len(white_pixe
+00019700: 6c73 5b30 5d29 0d0a 0d0a 2020 2020 2320  ls[0])....    # 
+00019710: 436f 6d70 7574 6520 7468 6520 6365 6e74  Compute the cent
+00019720: 726f 6964 206f 6620 7468 6520 7768 6974  roid of the whit
+00019730: 6520 7069 7865 6c73 2069 6e20 7468 6520  e pixels in the 
+00019740: 626f 756e 6461 7279 2069 6d61 6765 0d0a  boundary image..
+00019750: 2020 2020 6365 6e74 726f 6964 203d 206e      centroid = n
+00019760: 702e 7a65 726f 7328 6269 6e61 7279 5f69  p.zeros(binary_i
+00019770: 6d61 6765 2e6e 6469 6d29 0d0a 2020 2020  mage.ndim)..    
+00019780: 666f 7220 6469 6d20 696e 2072 616e 6765  for dim in range
+00019790: 2862 696e 6172 795f 696d 6167 652e 6e64  (binary_image.nd
+000197a0: 696d 293a 0d0a 2020 2020 2020 2020 6365  im):..        ce
+000197b0: 6e74 726f 6964 5b64 696d 5d20 3d20 7768  ntroid[dim] = wh
+000197c0: 6974 655f 7069 7865 6c73 5b64 696d 5d2e  ite_pixels[dim].
+000197d0: 7375 6d28 2920 2f20 6e75 6d5f 7069 7865  sum() / num_pixe
+000197e0: 6c73 0d0a 0d0a 2020 2020 7265 7475 726e  ls....    return
+000197f0: 2063 656e 7472 6f69 640d 0a0d 0a0d 0a0d   centroid.......
+00019800: 0a20 0d0a 0d0a 6465 6620 6765 745f 6373  . ....def get_cs
+00019810: 765f 6461 7461 2863 7376 293a 0d0a 0d0a  v_data(csv):....
+00019820: 2020 2020 2020 2020 6461 7461 7365 7420          dataset 
+00019830: 3d20 7064 2e72 6561 645f 6373 7628 0d0a  = pd.read_csv(..
+00019840: 2020 2020 2020 2020 2020 2020 6373 762c              csv,
+00019850: 2064 656c 696d 6974 6572 3d22 2c22 2c20   delimiter=",", 
+00019860: 656e 636f 6469 6e67 3d22 756e 6963 6f64  encoding="unicod
+00019870: 655f 6573 6361 7065 222c 206c 6f77 5f6d  e_escape", low_m
+00019880: 656d 6f72 793d 4661 6c73 650d 0a20 2020  emory=False..   
+00019890: 2020 2020 2029 5b33 3a5d 0d0a 2020 2020       )[3:]..    
+000198a0: 2020 2020 6461 7461 7365 745f 696e 6465      dataset_inde
+000198b0: 7820 3d20 6461 7461 7365 742e 696e 6465  x = dataset.inde
+000198c0: 780d 0a20 2020 2020 2020 2072 6574 7572  x..        retur
+000198d0: 6e20 6461 7461 7365 742c 2064 6174 6173  n dataset, datas
+000198e0: 6574 5f69 6e64 6578 0d0a 2020 2020 0d0a  et_index..    ..
+000198f0: 6465 6620 6765 745f 7370 6f74 5f64 6174  def get_spot_dat
+00019900: 6173 6574 2873 706f 745f 6461 7461 7365  aset(spot_datase
+00019910: 742c 2074 7261 636b 5f61 6e61 6c79 7369  t, track_analysi
+00019920: 735f 7370 6f74 5f6b 6579 732c 2078 6361  s_spot_keys, xca
+00019930: 6c69 6272 6174 696f 6e2c 2079 6361 6c69  libration, ycali
+00019940: 6272 6174 696f 6e2c 207a 6361 6c69 6272  bration, zcalibr
+00019950: 6174 696f 6e2c 2041 7474 7269 6275 7465  ation, Attribute
+00019960: 426f 786e 616d 652c 2064 6574 6563 7469  Boxname, detecti
+00019970: 6f6e 6368 616e 6e65 6c29 3a0d 0a20 2020  onchannel):..   
+00019980: 2020 2020 2041 6c6c 5661 6c75 6573 203d       AllValues =
+00019990: 207b 7d0d 0a20 2020 2020 2020 2070 6f73   {}..        pos
+000199a0: 6978 203d 2074 7261 636b 5f61 6e61 6c79  ix = track_analy
+000199b0: 7369 735f 7370 6f74 5f6b 6579 735b 2270  sis_spot_keys["p
+000199c0: 6f73 6978 225d 0d0a 2020 2020 2020 2020  osix"]..        
+000199d0: 706f 7369 7920 3d20 7472 6163 6b5f 616e  posiy = track_an
+000199e0: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+000199f0: 5b22 706f 7369 7922 5d0d 0a20 2020 2020  ["posiy"]..     
+00019a00: 2020 2070 6f73 697a 203d 2074 7261 636b     posiz = track
+00019a10: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+00019a20: 6579 735b 2270 6f73 697a 225d 0d0a 2020  eys["posiz"]..  
+00019a30: 2020 2020 2020 6672 616d 6520 3d20 7472        frame = tr
+00019a40: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+00019a50: 745f 6b65 7973 5b22 6672 616d 6522 5d0d  t_keys["frame"].
+00019a60: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00019a70: 2020 204c 6f63 6174 696f 6e58 203d 2028     LocationX = (
+00019a80: 0d0a 2020 2020 2020 2020 2020 2020 7370  ..            sp
+00019a90: 6f74 5f64 6174 6173 6574 5b70 6f73 6978  ot_dataset[posix
+00019aa0: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
+00019ab0: 2920 2f20 7863 616c 6962 7261 7469 6f6e  ) / xcalibration
+00019ac0: 0d0a 2020 2020 2020 2020 292e 6173 7479  ..        ).asty
+00019ad0: 7065 2822 696e 7422 290d 0a20 2020 2020  pe("int")..     
+00019ae0: 2020 204c 6f63 6174 696f 6e59 203d 2028     LocationY = (
+00019af0: 0d0a 2020 2020 2020 2020 2020 2020 7370  ..            sp
+00019b00: 6f74 5f64 6174 6173 6574 5b70 6f73 6979  ot_dataset[posiy
+00019b10: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
+00019b20: 2920 2f20 7963 616c 6962 7261 7469 6f6e  ) / ycalibration
+00019b30: 0d0a 2020 2020 2020 2020 292e 6173 7479  ..        ).asty
+00019b40: 7065 2822 696e 7422 290d 0a20 2020 2020  pe("int")..     
+00019b50: 2020 204c 6f63 6174 696f 6e5a 203d 2028     LocationZ = (
+00019b60: 0d0a 2020 2020 2020 2020 2020 2020 7370  ..            sp
+00019b70: 6f74 5f64 6174 6173 6574 5b70 6f73 697a  ot_dataset[posiz
+00019b80: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
+00019b90: 2920 2f20 7a63 616c 6962 7261 7469 6f6e  ) / zcalibration
+00019ba0: 0d0a 2020 2020 2020 2020 292e 6173 7479  ..        ).asty
+00019bb0: 7065 2822 696e 7422 290d 0a20 2020 2020  pe("int")..     
+00019bc0: 2020 204c 6f63 6174 696f 6e54 203d 2028     LocationT = (
+00019bd0: 7370 6f74 5f64 6174 6173 6574 5b66 7261  spot_dataset[fra
+00019be0: 6d65 5d2e 6173 7479 7065 2822 666c 6f61  me].astype("floa
+00019bf0: 7422 2929 2e61 7374 7970 6528 2269 6e74  t")).astype("int
+00019c00: 2229 0d0a 2020 2020 2020 2020 0d0a 0d0a  ")..        ....
+00019c10: 2020 2020 2020 2020 6967 6e6f 7265 5f76          ignore_v
+00019c20: 616c 7565 7320 3d20 5b74 7261 636b 5f61  alues = [track_a
+00019c30: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+00019c40: 735b 226d 6561 6e5f 696e 7465 6e73 6974  s["mean_intensit
+00019c50: 7922 5d2c 7472 6163 6b5f 616e 616c 7973  y"],track_analys
+00019c60: 6973 5f73 706f 745f 6b65 7973 5b22 746f  is_spot_keys["to
+00019c70: 7461 6c5f 696e 7465 6e73 6974 7922 5d5d  tal_intensity"]]
+00019c80: 200d 0a20 2020 2020 2020 2066 6f72 2028   ..        for (
+00019c90: 6b2c 7629 2069 6e20 7472 6163 6b5f 616e  k,v) in track_an
+00019ca0: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+00019cb0: 2e69 7465 6d73 2829 3a0d 0a0d 0a20 2020  .items():....   
+00019cc0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00019cd0: 6465 7465 6374 696f 6e63 6861 6e6e 656c  detectionchannel
+00019ce0: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
+00019cf0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00019d00: 6b20 3d3d 2022 6d65 616e 5f69 6e74 656e  k == "mean_inten
+00019d10: 7369 7479 5f63 6832 223a 0d0a 2020 2020  sity_ch2":..    
+00019d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d30: 2020 2020 2020 2076 616c 7565 203d 2074         value = t
+00019d40: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+00019d50: 6f74 5f6b 6579 735b 226d 6561 6e5f 696e  ot_keys["mean_in
+00019d60: 7465 6e73 6974 7922 5d0d 0a20 2020 2020  tensity"]..     
+00019d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d80: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
+00019d90: 7661 6c75 655d 203d 2073 706f 745f 6461  value] = spot_da
+00019da0: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
+00019db0: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
+00019dc0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00019dd0: 6620 6b20 3d3d 2022 746f 7461 6c5f 696e  f k == "total_in
+00019de0: 7465 6e73 6974 795f 6368 3222 3a0d 0a20  tensity_ch2":.. 
+00019df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e00: 2020 2020 2020 2020 2020 7661 6c75 6520            value 
+00019e10: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
+00019e20: 5f73 706f 745f 6b65 7973 5b22 746f 7461  _spot_keys["tota
+00019e30: 6c5f 696e 7465 6e73 6974 7922 5d0d 0a20  l_intensity"].. 
+00019e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e50: 2020 2020 2020 2020 2020 416c 6c56 616c            AllVal
+00019e60: 7565 735b 7661 6c75 655d 203d 2073 706f  ues[value] = spo
+00019e70: 745f 6461 7461 7365 745b 765d 2e61 7374  t_dataset[v].ast
+00019e80: 7970 6528 2266 6c6f 6174 2229 2020 2020  ype("float")    
+00019e90: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+00019ea0: 2020 2020 2020 2069 6620 7620 6e6f 7420         if v not 
+00019eb0: 696e 2069 676e 6f72 655f 7661 6c75 6573  in ignore_values
+00019ec0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00019ed0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00019ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ef0: 2020 2041 6c6c 5661 6c75 6573 5b76 5d20     AllValues[v] 
+00019f00: 3d20 7370 6f74 5f64 6174 6173 6574 5b76  = spot_dataset[v
+00019f10: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
+00019f20: 290d 0a0d 0a20 2020 2020 2020 2041 6c6c  )....        All
+00019f30: 5661 6c75 6573 5b70 6f73 6978 5d20 3d20  Values[posix] = 
+00019f40: 726f 756e 6428 4c6f 6361 7469 6f6e 582c  round(LocationX,
+00019f50: 3329 0d0a 2020 2020 2020 2020 416c 6c56  3)..        AllV
+00019f60: 616c 7565 735b 706f 7369 795d 203d 2072  alues[posiy] = r
+00019f70: 6f75 6e64 284c 6f63 6174 696f 6e59 2c33  ound(LocationY,3
+00019f80: 290d 0a20 2020 2020 2020 2041 6c6c 5661  )..        AllVa
+00019f90: 6c75 6573 5b70 6f73 697a 5d20 3d20 726f  lues[posiz] = ro
+00019fa0: 756e 6428 4c6f 6361 7469 6f6e 5a2c 3329  und(LocationZ,3)
+00019fb0: 0d0a 2020 2020 2020 2020 416c 6c56 616c  ..        AllVal
+00019fc0: 7565 735b 6672 616d 655d 203d 2072 6f75  ues[frame] = rou
+00019fd0: 6e64 284c 6f63 6174 696f 6e54 2c33 290d  nd(LocationT,3).
+00019fe0: 0a20 2020 2020 2020 2041 7474 7269 6275  .        Attribu
+00019ff0: 7465 6964 7320 3d20 5b5d 0d0a 2020 2020  teids = []..    
+0001a000: 2020 2020 4174 7472 6962 7574 6569 6473      Attributeids
+0001a010: 2e61 7070 656e 6428 4174 7472 6962 7574  .append(Attribut
+0001a020: 6542 6f78 6e61 6d65 290d 0a20 2020 2020  eBoxname)..     
+0001a030: 2020 2066 6f72 2061 7474 7269 6275 7465     for attribute
+0001a040: 6e61 6d65 2069 6e20 416c 6c56 616c 7565  name in AllValue
+0001a050: 732e 6b65 7973 2829 3a0d 0a20 2020 2020  s.keys():..     
+0001a060: 2020 2020 2020 2020 2041 7474 7269 6275           Attribu
+0001a070: 7465 6964 732e 6170 7065 6e64 2861 7474  teids.append(att
+0001a080: 7269 6275 7465 6e61 6d65 2920 2020 200d  ributename)    .
+0001a090: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+0001a0a0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001a0b0: 2072 6574 7572 6e20 4174 7472 6962 7574   return Attribut
+0001a0c0: 6569 6473 2c20 416c 6c56 616c 7565 7320  eids, AllValues 
+0001a0d0: 2020 2020 0d0a 2020 2020 0d0a 6465 6620      ..    ..def 
+0001a0e0: 6765 745f 7472 6163 6b5f 6461 7461 7365  get_track_datase
+0001a0f0: 7428 7472 6163 6b5f 6461 7461 7365 742c  t(track_dataset,
+0001a100: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001a110: 7370 6f74 5f6b 6579 732c 2074 7261 636b  spot_keys, track
+0001a120: 5f61 6e61 6c79 7369 735f 7472 6163 6b5f  _analysis_track_
+0001a130: 6b65 7973 2c20 5472 6163 6b41 7474 7269  keys, TrackAttri
+0001a140: 6275 7465 426f 786e 616d 6529 3a0d 0a0d  buteBoxname):...
+0001a150: 0a20 2020 2020 2020 2041 6c6c 5472 6163  .        AllTrac
+0001a160: 6b56 616c 7565 7320 3d20 7b7d 0d0a 2020  kValues = {}..  
+0001a170: 2020 2020 2020 7472 6163 6b5f 6964 203d        track_id =
+0001a180: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001a190: 7370 6f74 5f6b 6579 735b 2274 7261 636b  spot_keys["track
+0001a1a0: 5f69 6422 5d0d 0a20 2020 2020 2020 2054  _id"]..        T
+0001a1b0: 6964 203d 2074 7261 636b 5f64 6174 6173  id = track_datas
+0001a1c0: 6574 5b74 7261 636b 5f69 645d 2e61 7374  et[track_id].ast
+0001a1d0: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
+0001a1e0: 2020 2020 200d 0a20 2020 2020 2020 2041       ..        A
+0001a1f0: 6c6c 5472 6163 6b56 616c 7565 735b 7472  llTrackValues[tr
+0001a200: 6163 6b5f 6964 5d20 3d20 5469 640d 0a20  ack_id] = Tid.. 
+0001a210: 2020 2020 200d 0a20 2020 2020 2020 2066       ..        f
+0001a220: 6f72 2028 6b2c 2076 2920 696e 2074 7261  or (k, v) in tra
+0001a230: 636b 5f61 6e61 6c79 7369 735f 7472 6163  ck_analysis_trac
+0001a240: 6b5f 6b65 7973 2e69 7465 6d73 2829 3a0d  k_keys.items():.
+0001a250: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001a260: 2020 2078 203d 2074 7261 636b 5f64 6174     x = track_dat
+0001a270: 6173 6574 5b76 5d2e 6173 7479 7065 2822  aset[v].astype("
+0001a280: 666c 6f61 7422 290d 0a20 2020 2020 2020  float")..       
+0001a290: 2020 2020 2020 2020 206d 696e 7661 6c20           minval 
+0001a2a0: 3d20 6d69 6e28 7829 0d0a 2020 2020 2020  = min(x)..      
+0001a2b0: 2020 2020 2020 2020 2020 6d61 7876 616c            maxval
+0001a2c0: 203d 206d 6178 2878 290d 0a0d 0a20 2020   = max(x)....   
+0001a2d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001a2e0: 6d69 6e76 616c 203e 2030 2061 6e64 206d  minval > 0 and m
+0001a2f0: 6178 7661 6c20 3c3d 2031 3a0d 0a0d 0a20  axval <= 1:.... 
+0001a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a310: 2020 2078 203d 2078 202b 2031 0d0a 0d0a     x = x + 1....
+0001a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a330: 416c 6c54 7261 636b 5661 6c75 6573 5b6b  AllTrackValues[k
+0001a340: 5d20 3d20 726f 756e 6428 782c 2033 290d  ] = round(x, 3).
+0001a350: 0a0d 0a20 2020 2020 2020 2054 7261 636b  ...        Track
+0001a360: 4174 7472 6962 7574 6569 6473 203d 205b  Attributeids = [
+0001a370: 5d0d 0a20 2020 2020 2020 2054 7261 636b  ]..        Track
+0001a380: 4174 7472 6962 7574 6569 6473 2e61 7070  Attributeids.app
+0001a390: 656e 6428 5472 6163 6b41 7474 7269 6275  end(TrackAttribu
+0001a3a0: 7465 426f 786e 616d 6529 0d0a 2020 2020  teBoxname)..    
+0001a3b0: 2020 2020 666f 7220 6174 7472 6962 7574      for attribut
+0001a3c0: 656e 616d 6520 696e 2074 7261 636b 5f61  ename in track_a
+0001a3d0: 6e61 6c79 7369 735f 7472 6163 6b5f 6b65  nalysis_track_ke
+0001a3e0: 7973 2e6b 6579 7328 293a 0d0a 2020 2020  ys.keys():..    
+0001a3f0: 2020 2020 2020 2020 5472 6163 6b41 7474          TrackAtt
+0001a400: 7269 6275 7465 6964 732e 6170 7065 6e64  ributeids.append
+0001a410: 2861 7474 7269 6275 7465 6e61 6d65 2920  (attributename) 
+0001a420: 2020 200d 0a20 2020 200d 0a20 2020 2020     ..    ..     
+0001a430: 2020 2072 6574 7572 6e20 5472 6163 6b41     return TrackA
+0001a440: 7474 7269 6275 7465 6964 732c 2041 6c6c  ttributeids, All
+0001a450: 5472 6163 6b56 616c 7565 730d 0a20 2020  TrackValues..   
+0001a460: 200d 0a64 6566 2067 6574 5f65 6467 6573   ..def get_edges
+0001a470: 5f64 6174 6173 6574 2865 6467 6573 5f64  _dataset(edges_d
+0001a480: 6174 6173 6574 2c20 6564 6765 735f 6461  ataset, edges_da
+0001a490: 7461 7365 745f 696e 6465 782c 2074 7261  taset_index, tra
+0001a4a0: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+0001a4b0: 5f6b 6579 732c 2074 7261 636b 5f61 6e61  _keys, track_ana
+0001a4c0: 6c79 7369 735f 6564 6765 735f 6b65 7973  lysis_edges_keys
+0001a4d0: 293a 0d0a 0d0a 2020 2020 2020 2020 416c  ):....        Al
+0001a4e0: 6c45 6467 6573 5661 6c75 6573 203d 207b  lEdgesValues = {
+0001a4f0: 7d0d 0a20 2020 2020 2020 2074 7261 636b  }..        track
+0001a500: 5f69 6420 3d20 7472 6163 6b5f 616e 616c  _id = track_anal
+0001a510: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+0001a520: 7472 6163 6b5f 6964 225d 0d0a 2020 2020  track_id"]..    
+0001a530: 2020 2020 5469 6420 3d20 6564 6765 735f      Tid = edges_
+0001a540: 6461 7461 7365 745b 7472 6163 6b5f 6964  dataset[track_id
+0001a550: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
+0001a560: 290d 0a20 2020 2020 2020 2069 6e64 6963  )..        indic
+0001a570: 6573 203d 206e 702e 7768 6572 6528 5469  es = np.where(Ti
+0001a580: 6420 3d3d 2030 290d 0a20 2020 2020 2020  d == 0)..       
+0001a590: 206d 6178 7472 6163 6b5f 6964 203d 206d   maxtrack_id = m
+0001a5a0: 6178 2854 6964 290d 0a20 2020 2020 2020  ax(Tid)..       
+0001a5b0: 2063 6f6e 6469 7469 6f6e 5f69 6e64 6963   condition_indic
+0001a5c0: 6573 203d 2065 6467 6573 5f64 6174 6173  es = edges_datas
+0001a5d0: 6574 5f69 6e64 6578 5b69 6e64 6963 6573  et_index[indices
+0001a5e0: 5d0d 0a20 2020 2020 2020 2054 6964 5b63  ]..        Tid[c
+0001a5f0: 6f6e 6469 7469 6f6e 5f69 6e64 6963 6573  ondition_indices
+0001a600: 5d20 3d20 6d61 7874 7261 636b 5f69 6420  ] = maxtrack_id 
+0001a610: 2b20 310d 0a20 2020 2020 2020 2041 6c6c  + 1..        All
+0001a620: 4564 6765 7356 616c 7565 735b 7472 6163  EdgesValues[trac
+0001a630: 6b5f 6964 5d20 3d20 5469 640d 0a0d 0a20  k_id] = Tid.... 
+0001a640: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+0001a650: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
+0001a660: 6467 6573 5f6b 6579 732e 7661 6c75 6573  dges_keys.values
+0001a670: 2829 3a0d 0a0d 0a20 2020 2020 2020 2020  ():....         
+0001a680: 2020 2069 6620 6b20 213d 2074 7261 636b     if k != track
+0001a690: 5f69 643a 0d0a 2020 2020 2020 2020 2020  _id:..          
+0001a6a0: 2020 2020 2020 7820 3d20 6564 6765 735f        x = edges_
+0001a6b0: 6461 7461 7365 745b 6b5d 2e61 7374 7970  dataset[k].astyp
+0001a6c0: 6528 2266 6c6f 6174 2229 0d0a 0d0a 2020  e("float")....  
+0001a6d0: 2020 2020 2020 2020 2020 2020 2020 416c                Al
+0001a6e0: 6c45 6467 6573 5661 6c75 6573 5b6b 5d20  lEdgesValues[k] 
+0001a6f0: 3d20 7820 2020 0d0a 2020 2020 2020 2020  = x   ..        
+0001a700: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
+0001a710: 6e20 416c 6c45 6467 6573 5661 6c75 6573  n AllEdgesValues
+0001a720: 2020 200d 0a20 2020 200d 0a20 2020 2020     ..    ..     
+0001a730: 2020 0d0a 2020 2020 0d0a 6465 6620 7363    ..    ..def sc
+0001a740: 616c 655f 7661 6c75 6528 782c 2073 6361  ale_value(x, sca
+0001a750: 6c65 203d 2032 3535 202a 2032 3535 293a  le = 255 * 255):
+0001a760: 0d0a 0d0a 0d0a 2020 2020 2072 6574 7572  ......     retur
+0001a770: 6e20 7820 2a20 7363 616c 6520 2020 0d0a  n x * scale   ..
+0001a780: 2020 2020 0d0a 0d0a 0d0a 6465 6620 7072      ......def pr
+0001a790: 6f62 5f73 6967 6d6f 6964 2878 293a 0d0a  ob_sigmoid(x):..
+0001a7a0: 2020 2020 7265 7475 726e 2031 202d 206d      return 1 - m
+0001a7b0: 6174 682e 6578 7028 2d78 290d 0a0d 0a0d  ath.exp(-x).....
+0001a7c0: 0a64 6566 2061 6e67 756c 6172 5f63 6861  .def angular_cha
+0001a7d0: 6e67 6528 7665 635f 302c 2076 6563 5f31  nge(vec_0, vec_1
+0001a7e0: 293a 0d0a 2020 2020 2020 2020 0d0a 2020  ):..        ..  
+0001a7f0: 2020 2020 2020 7665 635f 3020 3d20 7665        vec_0 = ve
+0001a800: 635f 3020 2f20 6e70 2e6c 696e 616c 672e  c_0 / np.linalg.
+0001a810: 6e6f 726d 2876 6563 5f30 290d 0a20 2020  norm(vec_0)..   
+0001a820: 2020 2020 2076 6563 5f31 203d 2076 6563       vec_1 = vec
+0001a830: 5f31 202f 206e 702e 6c69 6e61 6c67 2e6e  _1 / np.linalg.n
+0001a840: 6f72 6d28 7665 635f 3129 0d0a 2020 2020  orm(vec_1)..    
+0001a850: 2020 2020 616e 676c 6520 3d20 6e70 2e61      angle = np.a
+0001a860: 7263 636f 7328 6e70 2e63 6c69 7028 6e70  rccos(np.clip(np
+0001a870: 2e64 6f74 2876 6563 5f30 2c20 7665 635f  .dot(vec_0, vec_
+0001a880: 3129 2c20 2d31 2e30 2c20 312e 3029 290d  1), -1.0, 1.0)).
+0001a890: 0a20 2020 2020 2020 2061 6e67 6c65 203d  .        angle =
+0001a8a0: 2061 6e67 6c65 202a 2031 3830 202f 206e   angle * 180 / n
+0001a8b0: 702e 7069 0d0a 2020 2020 2020 2020 7265  p.pi..        re
+0001a8c0: 7475 726e 2061 6e67 6c65 0d0a 2020 2020  turn angle..    
+0001a8d0: 200d 0a0d 0a64 6566 2065 7661 6c5f 626f   ....def eval_bo
+0001a8e0: 6f6c 2876 616c 7565 293a 0d0a 2020 2020  ol(value):..    
+0001a8f0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0001a900: 2020 2020 2020 2020 6966 2076 616c 7565          if value
+0001a910: 2020 3d3d 2027 5472 7565 273a 200d 0a20    == 'True': .. 
+0001a920: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0001a930: 6976 5f6b 6579 203d 2054 7275 650d 0a20  iv_key = True.. 
+0001a940: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0001a950: 2020 2020 2020 2020 2020 2020 2020 6469                di
+0001a960: 765f 6b65 7920 3d20 4661 6c73 6520 0d0a  v_key = False ..
+0001a970: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001a980: 2064 6976 5f6b 6579 2020 2020 2020 2020   div_key        
+0001a990: 2020 2020 2020 2020 0d0a 0d0a 6465 6620          ....def 
+0001a9a0: 6368 6563 6b5f 616e 645f 7570 6461 7465  check_and_update
+0001a9b0: 5f6d 6173 6b28 6d61 736b 2c69 6d61 6765  _mask(mask,image
+0001a9c0: 293a 0d0a 2020 2020 2020 200d 0a20 2020  ):..       ..   
+0001a9d0: 2020 2020 2069 6620 6c65 6e28 6d61 736b       if len(mask
+0001a9e0: 2e73 6861 7065 2920 3c20 6c65 6e28 696d  .shape) < len(im
+0001a9f0: 6167 652e 7368 6170 6529 3a0d 0a20 2020  age.shape):..   
+0001aa00: 2020 2020 2020 2020 2075 7064 6174 655f           update_
+0001aa10: 6d61 736b 203d 206e 702e 7a65 726f 7328  mask = np.zeros(
+0001aa20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001aa30: 2020 2020 2020 2020 2020 2020 2020 5b0d                [.
+0001aa40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001aa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aa60: 2069 6d61 6765 2e73 6861 7065 5b30 5d2c   image.shape[0],
+0001aa70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001aa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aa90: 2020 696d 6167 652e 7368 6170 655b 315d    image.shape[1]
+0001aaa0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001aab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aac0: 2020 2069 6d61 6765 2e73 6861 7065 5b32     image.shape[2
+0001aad0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+0001aae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aaf0: 2020 2020 696d 6167 652e 7368 6170 655b      image.shape[
+0001ab00: 335d 2c0d 0a20 2020 2020 2020 2020 2020  3],..           
 0001ab10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab20: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-0001ab30: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-0001ab40: 2830 2c20 7570 6461 7465 5f6d 6173 6b2e  (0, update_mask.
-0001ab50: 7368 6170 655b 305d 293a 0d0a 2020 2020  shape[0]):..    
-0001ab60: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001ab70: 6a20 696e 2072 616e 6765 2830 2c20 7570  j in range(0, up
-0001ab80: 6461 7465 5f6d 6173 6b2e 7368 6170 655b  date_mask.shape[
-0001ab90: 315d 293a 0d0a 0d0a 2020 2020 2020 2020  1]):....        
-0001aba0: 2020 2020 2020 2020 2020 2020 7570 6461              upda
-0001abb0: 7465 5f6d 6173 6b5b 692c 206a 2c20 3a2c  te_mask[i, j, :,
-0001abc0: 203a 5d20 3d20 6d61 736b 5b69 2c20 3a2c   :] = mask[i, :,
-0001abd0: 203a 5d0d 0a20 2020 2020 2020 2065 6c73   :]..        els
-0001abe0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0001abf0: 2020 2020 7570 6461 7465 5f6d 6173 6b20      update_mask 
-0001ac00: 3d20 6d61 736b 0d0a 0d0a 2020 2020 2020  = mask....      
-0001ac10: 2020 7265 7475 726e 2075 7064 6174 655f    return update_
-0001ac20: 6d61 736b 2020 2020 2020 2020 0d0a 2020  mask        ..  
-0001ac30: 2020 2020 200d 0a                             ..
+0001ab20: 205d 0d0a 2020 2020 2020 2020 2020 2020   ]..            
+0001ab30: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+0001ab40: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+0001ab50: 2069 6e20 7261 6e67 6528 302c 2075 7064   in range(0, upd
+0001ab60: 6174 655f 6d61 736b 2e73 6861 7065 5b30  ate_mask.shape[0
+0001ab70: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
+0001ab80: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
+0001ab90: 6e67 6528 302c 2075 7064 6174 655f 6d61  nge(0, update_ma
+0001aba0: 736b 2e73 6861 7065 5b31 5d29 3a0d 0a0d  sk.shape[1]):...
+0001abb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001abc0: 2020 2020 2075 7064 6174 655f 6d61 736b       update_mask
+0001abd0: 5b69 2c20 6a2c 203a 2c20 3a5d 203d 206d  [i, j, :, :] = m
+0001abe0: 6173 6b5b 692c 203a 2c20 3a5d 0d0a 2020  ask[i, :, :]..  
+0001abf0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+0001ac00: 2020 2020 2020 2020 2020 2020 2075 7064               upd
+0001ac10: 6174 655f 6d61 736b 203d 206d 6173 6b0d  ate_mask = mask.
+0001ac20: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+0001ac30: 6e20 7570 6461 7465 5f6d 6173 6b20 2020  n update_mask   
+0001ac40: 2020 2020 200d 0a20 2020 2020 2020 0d0a       ..       ..
```

### Comparing `napatrackmater-3.5.5/napatrackmater/Trackvector.py` & `napatrackmater-3.5.6/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.5/napatrackmater/__init__.py` & `napatrackmater-3.5.6/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.5/napatrackmater/clustering.py` & `napatrackmater-3.5.6/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.5/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.5.6/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.5/napatrackmater/fate_mapping.py` & `napatrackmater-3.5.6/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.5/napatrackmater/pretrained.py` & `napatrackmater-3.5.6/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.5/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.5.6/napatrackmater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.5.5
+Version: 3.5.6
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.5.5/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.5.6/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.5/setup.py` & `napatrackmater-3.5.6/setup.py`

 * *Files identical despite different names*

