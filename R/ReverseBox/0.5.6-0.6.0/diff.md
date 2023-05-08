# Comparing `tmp/ReverseBox-0.5.6.tar.gz` & `tmp/ReverseBox-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseBox-0.5.6.tar", last modified: Sun Apr 30 16:35:42 2023, max compression
+gzip compressed data, was "ReverseBox-0.6.0.tar", last modified: Mon May  8 21:55:58 2023, max compression
```

## Comparing `ReverseBox-0.5.6.tar` & `ReverseBox-0.6.0.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 16:35:42.972305 ReverseBox-0.5.6/
--rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:47.000000 ReverseBox-0.5.6/LICENSE
--rw-rw-rw-   0        0        0     5602 2023-04-30 16:35:42.972305 ReverseBox-0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     4340 2023-04-22 15:45:22.000000 ReverseBox-0.5.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 16:35:42.920789 ReverseBox-0.5.6/ReverseBox.egg-info/
--rw-rw-rw-   0        0        0     5602 2023-04-30 16:35:42.000000 ReverseBox-0.5.6/ReverseBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1805 2023-04-30 16:35:42.000000 ReverseBox-0.5.6/ReverseBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 16:35:42.000000 ReverseBox-0.5.6/ReverseBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-30 16:35:42.000000 ReverseBox-0.5.6/ReverseBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-30 16:35:42.000000 ReverseBox-0.5.6/ReverseBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-30 16:35:42.921789 ReverseBox-0.5.6/reversebox/
--rw-rw-rw-   0        0        0        0 2022-06-25 12:19:26.000000 ReverseBox-0.5.6/reversebox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:35:42.924790 ReverseBox-0.5.6/reversebox/checksum/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.6/reversebox/checksum/__init__.py
--rw-rw-rw-   0        0        0      404 2023-01-08 20:51:07.000000 ReverseBox-0.5.6/reversebox/checksum/checksum_adler32.py
--rw-rw-rw-   0        0        0      403 2023-01-09 21:19:57.000000 ReverseBox-0.5.6/reversebox/checksum/checksum_fletcher16.py
--rw-rw-rw-   0        0        0      510 2023-01-09 22:41:53.000000 ReverseBox-0.5.6/reversebox/checksum/checksum_fletcher32.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:35:42.927790 ReverseBox-0.5.6/reversebox/common/
--rw-rw-rw-   0        0        0        0 2022-06-25 16:29:13.000000 ReverseBox-0.5.6/reversebox/common/__init__.py
--rw-rw-rw-   0        0        0      394 2023-04-15 13:54:42.000000 ReverseBox-0.5.6/reversebox/common/common.py
--rw-rw-rw-   0        0        0      730 2022-09-07 19:55:27.000000 ReverseBox-0.5.6/reversebox/common/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:35:42.931791 ReverseBox-0.5.6/reversebox/compression/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.6/reversebox/compression/__init__.py
--rw-rw-rw-   0        0        0      482 2023-04-23 00:00:01.000000 ReverseBox-0.5.6/reversebox/compression/compression_jcalg1.py
--rw-rw-rw-   0        0        0      335 2022-12-27 14:56:59.000000 ReverseBox-0.5.6/reversebox/compression/compression_lzo.py
--rw-rw-rw-   0        0        0      330 2022-10-15 10:41:38.000000 ReverseBox-0.5.6/reversebox/compression/compression_zlib.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:35:42.940868 ReverseBox-0.5.6/reversebox/crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:26:29.000000 ReverseBox-0.5.6/reversebox/crc/__init__.py
--rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:19.000000 ReverseBox-0.5.6/reversebox/crc/crc16_arc.py
--rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:31.000000 ReverseBox-0.5.6/reversebox/crc/crc16_ccitt.py
--rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:06.000000 ReverseBox-0.5.6/reversebox/crc/crc16_dnp.py
--rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:19.000000 ReverseBox-0.5.6/reversebox/crc/crc16_kermit.py
--rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:37.000000 ReverseBox-0.5.6/reversebox/crc/crc16_modbus.py
--rw-rw-rw-   0        0        0      735 2022-07-21 21:35:31.000000 ReverseBox-0.5.6/reversebox/crc/crc16_sick.py
--rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:19.000000 ReverseBox-0.5.6/reversebox/crc/crc32_iso_hdlc.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:35:42.945733 ReverseBox-0.5.6/reversebox/encryption/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.6/reversebox/encryption/__init__.py
--rw-rw-rw-   0        0        0      579 2022-07-17 23:25:19.000000 ReverseBox-0.5.6/reversebox/encryption/encryption_xor_basic.py
--rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:01.000000 ReverseBox-0.5.6/reversebox/encryption/encryption_xor_gianas_return_zda.py
--rw-rw-rw-   0        0        0      574 2022-07-17 23:25:19.000000 ReverseBox-0.5.6/reversebox/encryption/encryption_xor_retro64_eco.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:35:42.949725 ReverseBox-0.5.6/reversebox/hash/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.6/reversebox/hash/__init__.py
--rw-rw-rw-   0        0        0      280 2022-09-11 18:48:36.000000 ReverseBox-0.5.6/reversebox/hash/hash_md5.py
--rw-rw-rw-   0        0        0      283 2023-01-08 14:05:01.000000 ReverseBox-0.5.6/reversebox/hash/hash_sha1.py
--rw-rw-rw-   0        0        0      289 2023-01-08 14:07:31.000000 ReverseBox-0.5.6/reversebox/hash/hash_sha2.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:35:42.953725 ReverseBox-0.5.6/reversebox/image/
--rw-rw-rw-   0        0        0        0 2022-12-27 21:18:24.000000 ReverseBox-0.5.6/reversebox/image/__init__.py
--rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:19.000000 ReverseBox-0.5.6/reversebox/image/image_finder_gui.py
--rw-rw-rw-   0        0        0      713 2023-04-23 00:00:01.000000 ReverseBox-0.5.6/reversebox/image/image_finder_main.py
--rw-rw-rw-   0        0        0     1507 2023-04-15 13:20:43.000000 ReverseBox-0.5.6/reversebox/image/psp_swizzle.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:35:42.959973 ReverseBox-0.5.6/reversebox/io_files/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.6/reversebox/io_files/__init__.py
--rw-rw-rw-   0        0        0      931 2023-04-23 15:32:28.000000 ReverseBox-0.5.6/reversebox/io_files/bytes_handler.py
--rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:49.000000 ReverseBox-0.5.6/reversebox/io_files/check_file.py
--rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:41.000000 ReverseBox-0.5.6/reversebox/io_files/file_handler.py
--rw-rw-rw-   0        0        0     8683 2023-04-30 16:08:06.000000 ReverseBox-0.5.6/reversebox/io_files/translation_text_handler.py
--rw-rw-rw-   0        0        0       42 2023-04-30 16:35:42.972305 ReverseBox-0.5.6/setup.cfg
--rw-rw-rw-   0        0        0     1825 2023-04-30 16:35:42.000000 ReverseBox-0.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:35:42.961557 ReverseBox-0.5.6/tests/
--rw-rw-rw-   0        0        0        0 2022-07-19 22:27:10.000000 ReverseBox-0.5.6/tests/__init__.py
--rw-rw-rw-   0        0        0      626 2023-04-12 20:56:38.000000 ReverseBox-0.5.6/tests/common.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:35:42.971305 ReverseBox-0.5.6/tests/tests_crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:28:33.000000 ReverseBox-0.5.6/tests/tests_crc/__init__.py
--rw-rw-rw-   0        0        0     2301 2023-01-09 18:34:08.000000 ReverseBox-0.5.6/tests/tests_crc/test_crc16_arc.py
--rw-rw-rw-   0        0        0     4539 2023-01-09 18:34:08.000000 ReverseBox-0.5.6/tests/tests_crc/test_crc16_ccitt.py
--rw-rw-rw-   0        0        0     1633 2023-01-09 18:34:08.000000 ReverseBox-0.5.6/tests/tests_crc/test_crc16_dnp.py
--rw-rw-rw-   0        0        0     1651 2023-01-09 18:34:08.000000 ReverseBox-0.5.6/tests/tests_crc/test_crc16_kermit.py
--rw-rw-rw-   0        0        0     1660 2023-01-09 18:34:08.000000 ReverseBox-0.5.6/tests/tests_crc/test_crc16_modbus.py
--rw-rw-rw-   0        0        0     1632 2023-01-09 18:34:08.000000 ReverseBox-0.5.6/tests/tests_crc/test_crc16_sick.py
--rw-rw-rw-   0        0        0     2655 2023-04-23 00:00:01.000000 ReverseBox-0.5.6/tests/tests_crc/test_crc32_iso_hdlc.py
+drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.180420 ReverseBox-0.6.0/
+-rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:47.000000 ReverseBox-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     5768 2023-05-08 21:55:58.180420 ReverseBox-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4506 2023-05-08 21:41:35.000000 ReverseBox-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.114849 ReverseBox-0.6.0/ReverseBox.egg-info/
+-rw-rw-rw-   0        0        0     5768 2023-05-08 21:55:57.000000 ReverseBox-0.6.0/ReverseBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1840 2023-05-08 21:55:58.000000 ReverseBox-0.6.0/ReverseBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 21:55:57.000000 ReverseBox-0.6.0/ReverseBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-08 21:55:58.000000 ReverseBox-0.6.0/ReverseBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-08 21:55:58.000000 ReverseBox-0.6.0/ReverseBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.115849 ReverseBox-0.6.0/reversebox/
+-rw-rw-rw-   0        0        0        0 2022-06-25 12:19:26.000000 ReverseBox-0.6.0/reversebox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.119850 ReverseBox-0.6.0/reversebox/checksum/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.6.0/reversebox/checksum/__init__.py
+-rw-rw-rw-   0        0        0      404 2023-01-08 20:51:07.000000 ReverseBox-0.6.0/reversebox/checksum/checksum_adler32.py
+-rw-rw-rw-   0        0        0      403 2023-01-09 21:19:57.000000 ReverseBox-0.6.0/reversebox/checksum/checksum_fletcher16.py
+-rw-rw-rw-   0        0        0      510 2023-01-09 22:41:53.000000 ReverseBox-0.6.0/reversebox/checksum/checksum_fletcher32.py
+drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.122851 ReverseBox-0.6.0/reversebox/common/
+-rw-rw-rw-   0        0        0        0 2022-06-25 16:29:13.000000 ReverseBox-0.6.0/reversebox/common/__init__.py
+-rw-rw-rw-   0        0        0      394 2023-04-15 13:54:42.000000 ReverseBox-0.6.0/reversebox/common/common.py
+-rw-rw-rw-   0        0        0      730 2022-09-07 19:55:27.000000 ReverseBox-0.6.0/reversebox/common/logger.py
+drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.127014 ReverseBox-0.6.0/reversebox/compression/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.6.0/reversebox/compression/__init__.py
+-rw-rw-rw-   0        0        0      482 2023-04-23 00:00:01.000000 ReverseBox-0.6.0/reversebox/compression/compression_jcalg1.py
+-rw-rw-rw-   0        0        0      335 2022-12-27 14:56:59.000000 ReverseBox-0.6.0/reversebox/compression/compression_lzo.py
+-rw-rw-rw-   0        0        0      330 2022-10-15 10:41:38.000000 ReverseBox-0.6.0/reversebox/compression/compression_zlib.py
+drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.135205 ReverseBox-0.6.0/reversebox/crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:26:29.000000 ReverseBox-0.6.0/reversebox/crc/__init__.py
+-rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:19.000000 ReverseBox-0.6.0/reversebox/crc/crc16_arc.py
+-rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:31.000000 ReverseBox-0.6.0/reversebox/crc/crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:06.000000 ReverseBox-0.6.0/reversebox/crc/crc16_dnp.py
+-rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:19.000000 ReverseBox-0.6.0/reversebox/crc/crc16_kermit.py
+-rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:37.000000 ReverseBox-0.6.0/reversebox/crc/crc16_modbus.py
+-rw-rw-rw-   0        0        0      735 2022-07-21 21:35:31.000000 ReverseBox-0.6.0/reversebox/crc/crc16_sick.py
+-rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:19.000000 ReverseBox-0.6.0/reversebox/crc/crc32_iso_hdlc.py
+drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.140806 ReverseBox-0.6.0/reversebox/encryption/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.6.0/reversebox/encryption/__init__.py
+-rw-rw-rw-   0        0        0      579 2022-07-17 23:25:19.000000 ReverseBox-0.6.0/reversebox/encryption/encryption_xor_basic.py
+-rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:01.000000 ReverseBox-0.6.0/reversebox/encryption/encryption_xor_gianas_return_zda.py
+-rw-rw-rw-   0        0        0      574 2022-07-17 23:25:19.000000 ReverseBox-0.6.0/reversebox/encryption/encryption_xor_retro64_eco.py
+drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.144807 ReverseBox-0.6.0/reversebox/hash/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.6.0/reversebox/hash/__init__.py
+-rw-rw-rw-   0        0        0      280 2022-09-11 18:48:36.000000 ReverseBox-0.6.0/reversebox/hash/hash_md5.py
+-rw-rw-rw-   0        0        0      283 2023-01-08 14:05:01.000000 ReverseBox-0.6.0/reversebox/hash/hash_sha1.py
+-rw-rw-rw-   0        0        0      289 2023-01-08 14:07:31.000000 ReverseBox-0.6.0/reversebox/hash/hash_sha2.py
+drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.148808 ReverseBox-0.6.0/reversebox/image/
+-rw-rw-rw-   0        0        0        0 2022-12-27 21:18:24.000000 ReverseBox-0.6.0/reversebox/image/__init__.py
+-rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:19.000000 ReverseBox-0.6.0/reversebox/image/image_finder_gui.py
+-rw-rw-rw-   0        0        0      713 2023-04-23 00:00:01.000000 ReverseBox-0.6.0/reversebox/image/image_finder_main.py
+-rw-rw-rw-   0        0        0     1507 2023-04-15 13:20:43.000000 ReverseBox-0.6.0/reversebox/image/psp_swizzle.py
+drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.162812 ReverseBox-0.6.0/reversebox/io_files/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.6.0/reversebox/io_files/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-04-23 15:32:28.000000 ReverseBox-0.6.0/reversebox/io_files/bytes_handler.py
+-rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:49.000000 ReverseBox-0.6.0/reversebox/io_files/check_file.py
+-rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:41.000000 ReverseBox-0.6.0/reversebox/io_files/file_handler.py
+-rw-rw-rw-   0        0        0     5195 2023-05-08 21:42:14.000000 ReverseBox-0.6.0/reversebox/io_files/mod_handler.py
+-rw-rw-rw-   0        0        0    11372 2023-05-08 21:44:23.000000 ReverseBox-0.6.0/reversebox/io_files/translation_text_handler.py
+-rw-rw-rw-   0        0        0       42 2023-05-08 21:55:58.180420 ReverseBox-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2023-05-08 21:39:10.000000 ReverseBox-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.164811 ReverseBox-0.6.0/tests/
+-rw-rw-rw-   0        0        0        0 2022-07-19 22:27:10.000000 ReverseBox-0.6.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-04-12 20:56:38.000000 ReverseBox-0.6.0/tests/common.py
+drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.180420 ReverseBox-0.6.0/tests/tests_crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:28:33.000000 ReverseBox-0.6.0/tests/tests_crc/__init__.py
+-rw-rw-rw-   0        0        0     2301 2023-01-09 18:34:08.000000 ReverseBox-0.6.0/tests/tests_crc/test_crc16_arc.py
+-rw-rw-rw-   0        0        0     4539 2023-01-09 18:34:08.000000 ReverseBox-0.6.0/tests/tests_crc/test_crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1633 2023-01-09 18:34:08.000000 ReverseBox-0.6.0/tests/tests_crc/test_crc16_dnp.py
+-rw-rw-rw-   0        0        0     1651 2023-01-09 18:34:08.000000 ReverseBox-0.6.0/tests/tests_crc/test_crc16_kermit.py
+-rw-rw-rw-   0        0        0     1660 2023-01-09 18:34:08.000000 ReverseBox-0.6.0/tests/tests_crc/test_crc16_modbus.py
+-rw-rw-rw-   0        0        0     1632 2023-01-09 18:34:08.000000 ReverseBox-0.6.0/tests/tests_crc/test_crc16_sick.py
+-rw-rw-rw-   0        0        0     2655 2023-04-23 00:00:01.000000 ReverseBox-0.6.0/tests/tests_crc/test_crc32_iso_hdlc.py
```

### Comparing `ReverseBox-0.5.6/LICENSE` & `ReverseBox-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/PKG-INFO` & `ReverseBox-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.5.6
+Version: 0.6.0
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -105,14 +105,15 @@
   - [SourceSDK Swizzling](https://forum.xentax.com/viewtopic.php?p=139510#p139510) (TODO) ❌
 
 * IO
   - File Reader ✔️
   - File Writer ✔️
   - Bytes Handler ✔️
   - Translation Text Handler ✔️
+  - Mod Handler ✔️
   - File extension checking ✔️
   - Padding calculation ✔️
   - File size checking ✔️
 
 # Checksum calculation - example
 
 // CRC32 calculation
@@ -192,8 +193,9 @@
 
 # More Examples
 
 Need more examples? <br>
 Check out list of tools written using ReverseBox:
 - [Giana's Return ZDA Tool](https://github.com/bartlomiejduda/Tools/blob/master/NEW%20Tools/Gianas%20Return/Gianas_Return_ZDA_Tool.py)
 - [ObsCure 2 HVP Extractor](https://github.com/bartlomiejduda/Tools/blob/master/NEW%20Tools/ObsCure%202/ObsCure%202%20HVP%20Tools/Obscure_2_hvp_extractor.py)
+- [Tail Concerto Translation Tools](https://github.com/bartlomiejduda/Tools/tree/master/NEW%20Tools/Tail%20Concerto/Tail%20Concerto%20Tools)
 - and more...
```

### Comparing `ReverseBox-0.5.6/README.md` & `ReverseBox-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -76,14 +76,15 @@
   - [SourceSDK Swizzling](https://forum.xentax.com/viewtopic.php?p=139510#p139510) (TODO) ❌
 
 * IO
   - File Reader ✔️
   - File Writer ✔️
   - Bytes Handler ✔️
   - Translation Text Handler ✔️
+  - Mod Handler ✔️
   - File extension checking ✔️
   - Padding calculation ✔️
   - File size checking ✔️
 
 # Checksum calculation - example
 
 // CRC32 calculation
@@ -163,8 +164,9 @@
 
 # More Examples
 
 Need more examples? <br>
 Check out list of tools written using ReverseBox:
 - [Giana's Return ZDA Tool](https://github.com/bartlomiejduda/Tools/blob/master/NEW%20Tools/Gianas%20Return/Gianas_Return_ZDA_Tool.py)
 - [ObsCure 2 HVP Extractor](https://github.com/bartlomiejduda/Tools/blob/master/NEW%20Tools/ObsCure%202/ObsCure%202%20HVP%20Tools/Obscure_2_hvp_extractor.py)
+- [Tail Concerto Translation Tools](https://github.com/bartlomiejduda/Tools/tree/master/NEW%20Tools/Tail%20Concerto/Tail%20Concerto%20Tools)
 - and more...
```

### Comparing `ReverseBox-0.5.6/ReverseBox.egg-info/PKG-INFO` & `ReverseBox-0.6.0/ReverseBox.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.5.6
+Version: 0.6.0
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -105,14 +105,15 @@
   - [SourceSDK Swizzling](https://forum.xentax.com/viewtopic.php?p=139510#p139510) (TODO) ❌
 
 * IO
   - File Reader ✔️
   - File Writer ✔️
   - Bytes Handler ✔️
   - Translation Text Handler ✔️
+  - Mod Handler ✔️
   - File extension checking ✔️
   - Padding calculation ✔️
   - File size checking ✔️
 
 # Checksum calculation - example
 
 // CRC32 calculation
@@ -192,8 +193,9 @@
 
 # More Examples
 
 Need more examples? <br>
 Check out list of tools written using ReverseBox:
 - [Giana's Return ZDA Tool](https://github.com/bartlomiejduda/Tools/blob/master/NEW%20Tools/Gianas%20Return/Gianas_Return_ZDA_Tool.py)
 - [ObsCure 2 HVP Extractor](https://github.com/bartlomiejduda/Tools/blob/master/NEW%20Tools/ObsCure%202/ObsCure%202%20HVP%20Tools/Obscure_2_hvp_extractor.py)
+- [Tail Concerto Translation Tools](https://github.com/bartlomiejduda/Tools/tree/master/NEW%20Tools/Tail%20Concerto/Tail%20Concerto%20Tools)
 - and more...
```

### Comparing `ReverseBox-0.5.6/ReverseBox.egg-info/SOURCES.txt` & `ReverseBox-0.6.0/ReverseBox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 reversebox/image/image_finder_gui.py
 reversebox/image/image_finder_main.py
 reversebox/image/psp_swizzle.py
 reversebox/io_files/__init__.py
 reversebox/io_files/bytes_handler.py
 reversebox/io_files/check_file.py
 reversebox/io_files/file_handler.py
+reversebox/io_files/mod_handler.py
 reversebox/io_files/translation_text_handler.py
 tests/__init__.py
 tests/common.py
 tests/tests_crc/__init__.py
 tests/tests_crc/test_crc16_arc.py
 tests/tests_crc/test_crc16_ccitt.py
 tests/tests_crc/test_crc16_dnp.py
```

### Comparing `ReverseBox-0.5.6/reversebox/common/logger.py` & `ReverseBox-0.6.0/reversebox/common/logger.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/crc/crc16_arc.py` & `ReverseBox-0.6.0/reversebox/crc/crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/crc/crc16_ccitt.py` & `ReverseBox-0.6.0/reversebox/crc/crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/crc/crc16_dnp.py` & `ReverseBox-0.6.0/reversebox/crc/crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/crc/crc16_kermit.py` & `ReverseBox-0.6.0/reversebox/crc/crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/crc/crc16_modbus.py` & `ReverseBox-0.6.0/reversebox/crc/crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/crc/crc16_sick.py` & `ReverseBox-0.6.0/reversebox/crc/crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/crc/crc32_iso_hdlc.py` & `ReverseBox-0.6.0/reversebox/crc/crc32_iso_hdlc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/encryption/encryption_xor_basic.py` & `ReverseBox-0.6.0/reversebox/encryption/encryption_xor_basic.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/encryption/encryption_xor_gianas_return_zda.py` & `ReverseBox-0.6.0/reversebox/encryption/encryption_xor_gianas_return_zda.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/encryption/encryption_xor_retro64_eco.py` & `ReverseBox-0.6.0/reversebox/encryption/encryption_xor_retro64_eco.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/image/image_finder_gui.py` & `ReverseBox-0.6.0/reversebox/image/image_finder_gui.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/image/image_finder_main.py` & `ReverseBox-0.6.0/reversebox/image/image_finder_main.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/image/psp_swizzle.py` & `ReverseBox-0.6.0/reversebox/image/psp_swizzle.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/io_files/bytes_handler.py` & `ReverseBox-0.6.0/reversebox/io_files/bytes_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/io_files/check_file.py` & `ReverseBox-0.6.0/reversebox/io_files/check_file.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/io_files/file_handler.py` & `ReverseBox-0.6.0/reversebox/io_files/file_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/reversebox/io_files/translation_text_handler.py` & `ReverseBox-0.6.0/reversebox/io_files/translation_text_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             backup_file_path = self.file_path + ".backup"
             logger.info(f"Creating backup file at path: {backup_file_path}")
             try:
                 backup_file = open(backup_file_path, "wb")
                 backup_file.write(import_file_whole_file_content)
                 backup_file.close()
                 logger.info(
-                    "fSuccessfully created backup file at path: {backup_file_path}"
+                    f"Successfully created backup file at path: {backup_file_path}"
                 )
             except Exception as error:
                 logger.error(f"Error occurred while creating backup file: {error}")
 
         self.open_mode = "wb"
         self.open()
         self.write_bytes(import_file_whole_file_content)
@@ -213,7 +213,81 @@
                 import_bytes = bytes_handler.fill_to_length(import_length)
 
             self.seek(memory_entry.text_offset)
             self.write_bytes(import_bytes)
 
         self.close()
         return True
+
+
+def generate_translation_entries(
+    txt_file_path: str, text_key: str = "text_to_translate"
+) -> bool:
+    """
+    This function should be used along with "strings" program from SysInternals https://learn.microsoft.com/en-us/sysinternals/downloads/strings
+    First, you should generate text dump using command "strings64.exe -o <binary_file_path> > <output_path>.
+    Then you should search for text entries in the dump and copy them to some output file e.g. "entries.txt"
+    Then you just need to run this function with your "entries.txt" as an input parameter for this function.
+    """
+    try:
+        txt_file = open(txt_file_path, "rt")
+    except Exception as error:
+        logger.error(f"Error with opening file: {error}")
+        return False
+
+    for line in txt_file:
+        line = line.strip()
+        offset = line.split(":")[0]
+        text = line.split(":")[-1]
+        output_entry = f'\tTranslationEntry(text_offset={offset}, text_export_length={len(text)}, text_key="{text_key}"),'
+        print(output_entry)
+
+    return True
+
+
+def check_translation_entries(
+    translation_memory_to_check: List[TranslationEntry],
+) -> bool:
+    """
+    Default function for checking if entries in Translation Memory are correct.
+    """
+    check_offsets_list: List[int] = []
+
+    for translation_entry in translation_memory_to_check:
+        if translation_entry.text_offset in check_offsets_list:
+            logger.error(f"Duplicated text_offset: {translation_entry.text_offset}")
+            return False
+
+        if (
+            translation_entry.text_import_length
+            and translation_entry.text_import_length
+            < translation_entry.text_export_length
+        ):
+            logger.error(
+                f"Import length is lower than export length for entry with offset {translation_entry.text_offset}"
+            )
+            return False
+
+        check_offsets_list.append(translation_entry.text_offset)
+    return True
+
+
+windows_1250_pl_no_accents_character_mapping: dict = {
+    b"\xAF": b"\x5A",  # Ż -> Z
+    b"\xD3": b"\x4F",  # Ó -> O
+    b"\xA3": b"\x4C",  # Ł -> L
+    b"\xC6": b"\x43",  # Ć -> C
+    b"\xCA": b"\x45",  # Ę -> E
+    b"\x8C": b"\x53",  # Ś -> S
+    b"\xA5": b"\x41",  # Ą -> A
+    b"\x8F": b"\x5A",  # Ź -> Z
+    b"\xD1": b"\x4E",  # Ń -> N
+    b"\xBF": b"\x7A",  # ż -> z
+    b"\xF3": b"\x6F",  # ó -> o
+    b"\xB3": b"\x6C",  # ł -> l
+    b"\xE6": b"\x63",  # ć -> c
+    b"\xEA": b"\x65",  # ę -> e
+    b"\x9C": b"\x73",  # ś -> s
+    b"\xB9": b"\x61",  # ą -> a
+    b"\x9F": b"\x7A",  # ź -> z
+    b"\xF1": b"\x6E",  # ń -> n
+}
```

### Comparing `ReverseBox-0.5.6/setup.py` & `ReverseBox-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 License: GPL-3.0 License
 """
 
 import os
 
 import setuptools
 
-VERSION_NUM = "0.5.6"
+VERSION_NUM = "0.6.0"
 
 
 def get_long_description() -> str:
     with open(
         os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf8"
     ) as readme:
         readme_text = readme.read()
```

### Comparing `ReverseBox-0.5.6/tests/common.py` & `ReverseBox-0.6.0/tests/common.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/tests/tests_crc/test_crc16_arc.py` & `ReverseBox-0.6.0/tests/tests_crc/test_crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/tests/tests_crc/test_crc16_ccitt.py` & `ReverseBox-0.6.0/tests/tests_crc/test_crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/tests/tests_crc/test_crc16_dnp.py` & `ReverseBox-0.6.0/tests/tests_crc/test_crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/tests/tests_crc/test_crc16_kermit.py` & `ReverseBox-0.6.0/tests/tests_crc/test_crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/tests/tests_crc/test_crc16_modbus.py` & `ReverseBox-0.6.0/tests/tests_crc/test_crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/tests/tests_crc/test_crc16_sick.py` & `ReverseBox-0.6.0/tests/tests_crc/test_crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.6/tests/tests_crc/test_crc32_iso_hdlc.py` & `ReverseBox-0.6.0/tests/tests_crc/test_crc32_iso_hdlc.py`

 * *Files identical despite different names*

