# Comparing `tmp/system-calls-5.19.0.tar.gz` & `tmp/system-calls-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "system-calls-5.19.0.tar", last modified: Thu Jun  9 12:43:57 2022, max compression
+gzip compressed data, was "system-calls-6.4.0.tar", last modified: Mon May  8 09:16:42 2023, max compression
```

## Comparing `system-calls-5.19.0.tar` & `system-calls-6.4.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 marcin    (1003) marcin    (1006)        0 2022-06-09 12:43:57.329366 system-calls-5.19.0/
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     1085 2021-05-13 13:07:58.000000 system-calls-5.19.0/LICENSE
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     1362 2022-06-09 12:43:57.328366 system-calls-5.19.0/PKG-INFO
--rw-rw-r--   0 marcin    (1003) marcin    (1006)      801 2022-01-10 10:42:44.000000 system-calls-5.19.0/README.md
-drwxrwxr-x   0 marcin    (1003) marcin    (1006)        0 2022-06-09 12:43:57.324366 system-calls-5.19.0/bin/
--rwxrwxr-x   0 marcin    (1003) marcin    (1006)     2644 2022-03-10 15:12:20.000000 system-calls-5.19.0/bin/syscall
-drwxrwxr-x   0 marcin    (1003) marcin    (1006)        0 2022-06-09 12:43:57.324366 system-calls-5.19.0/man/
--rw-r--r--   0 marcin    (1003) marcin    (1006)      537 2021-09-15 14:13:40.000000 system-calls-5.19.0/man/syscall.1
--rw-rw-r--   0 marcin    (1003) marcin    (1006)       38 2022-06-09 12:43:57.329366 system-calls-5.19.0/setup.cfg
--rw-r--r--   0 marcin    (1003) marcin    (1006)      978 2022-06-09 12:43:30.000000 system-calls-5.19.0/setup.py
-drwxrwxr-x   0 marcin    (1003) marcin    (1006)        0 2022-06-09 12:43:57.324366 system-calls-5.19.0/system_calls/
--rw-r--r--   0 marcin    (1003) marcin    (1006)     5914 2022-02-06 11:13:32.000000 system-calls-5.19.0/system_calls/__init__.py
-drwxrwxr-x   0 marcin    (1003) marcin    (1006)        0 2022-06-09 12:43:57.328366 system-calls-5.19.0/system_calls/tables/
--rw-rw-r--   0 marcin    (1003) marcin    (1006)    10909 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/alpha.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     7484 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/arc.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     9004 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/arm.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     6788 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/arm64.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)    10974 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/armoabi.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     7007 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/avr32.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     7051 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/blackfin.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     7133 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/c6x.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     7634 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/cris.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     7401 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/csky.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     6986 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/frv.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     7004 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/h8300.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     7354 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/hexagon.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     9509 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/i386.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     8087 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/ia64.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     6666 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/loongarch64.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     5700 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/m32r.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     9382 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/m68k.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     6028 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/metag.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     9561 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/microblaze.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     8097 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/mips64.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     8818 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/mips64n32.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     9460 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/mipso32.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     7202 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/mn10300.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)    10976 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/names.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     7383 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/nds32.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     7375 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/nios2.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     7398 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/openrisc.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     8543 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/parisc.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     9320 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/powerpc.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     8546 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/powerpc64.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     6694 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/riscv32.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     6801 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/riscv64.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     9347 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/s390.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     8060 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/s390x.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     7159 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/score.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     9181 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/sh.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     7749 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/sh64.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     9299 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/sparc.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     8345 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/sparc64.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     6051 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/tile.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     6052 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/tile64.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     7039 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/unicore32.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)    10106 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/x32.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     7820 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/x86_64.py
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     8277 2022-06-09 12:43:00.000000 system-calls-5.19.0/system_calls/tables/xtensa.py
-drwxrwxr-x   0 marcin    (1003) marcin    (1006)        0 2022-06-09 12:43:57.324366 system-calls-5.19.0/system_calls.egg-info/
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     1362 2022-06-09 12:43:56.000000 system-calls-5.19.0/system_calls.egg-info/PKG-INFO
--rw-rw-r--   0 marcin    (1003) marcin    (1006)     1583 2022-06-09 12:43:57.000000 system-calls-5.19.0/system_calls.egg-info/SOURCES.txt
--rw-rw-r--   0 marcin    (1003) marcin    (1006)        1 2022-06-09 12:43:57.000000 system-calls-5.19.0/system_calls.egg-info/dependency_links.txt
--rw-rw-r--   0 marcin    (1003) marcin    (1006)       34 2022-06-09 12:43:57.000000 system-calls-5.19.0/system_calls.egg-info/top_level.txt
+drwxr-xr-x   0 marcin    (1003) marcin    (1006)        0 2023-05-08 09:16:42.344221 system-calls-6.4.0/
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     1085 2021-05-13 13:07:58.000000 system-calls-6.4.0/LICENSE
+-rw-r--r--   0 marcin    (1003) marcin    (1006)     1361 2023-05-08 09:16:42.344221 system-calls-6.4.0/PKG-INFO
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)      801 2023-05-08 09:15:05.000000 system-calls-6.4.0/README.md
+drwxr-xr-x   0 marcin    (1003) marcin    (1006)        0 2023-05-08 09:16:42.339221 system-calls-6.4.0/bin/
+-rwxrwxr-x   0 marcin    (1003) marcin    (1006)     2644 2022-03-10 15:12:20.000000 system-calls-6.4.0/bin/syscall
+drwxr-xr-x   0 marcin    (1003) marcin    (1006)        0 2023-05-08 09:16:42.339221 system-calls-6.4.0/man/
+-rw-r--r--   0 marcin    (1003) marcin    (1006)      537 2021-09-15 14:13:40.000000 system-calls-6.4.0/man/syscall.1
+-rw-r--r--   0 marcin    (1003) marcin    (1006)       38 2023-05-08 09:16:42.344221 system-calls-6.4.0/setup.cfg
+-rw-r--r--   0 marcin    (1003) marcin    (1006)      977 2023-05-08 09:13:46.000000 system-calls-6.4.0/setup.py
+drwxr-xr-x   0 marcin    (1003) marcin    (1006)        0 2023-05-08 09:16:42.340222 system-calls-6.4.0/system_calls/
+-rw-r--r--   0 marcin    (1003) marcin    (1006)     5914 2022-02-06 11:13:32.000000 system-calls-6.4.0/system_calls/__init__.py
+drwxr-xr-x   0 marcin    (1003) marcin    (1006)        0 2023-05-08 09:16:42.344221 system-calls-6.4.0/system_calls/tables/
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)    10909 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/alpha.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     7484 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/arc.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     9004 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/arm.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     6788 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/arm64.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)    10974 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/armoabi.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     7007 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/avr32.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     7051 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/blackfin.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     7133 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/c6x.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     7634 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/cris.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     7401 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/csky.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     6986 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/frv.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     7004 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/h8300.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     7354 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/hexagon.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     9509 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/i386.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     8087 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/ia64.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     6666 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/loongarch64.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     5700 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/m32r.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     9382 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/m68k.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     6028 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/metag.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     9561 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/microblaze.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     8097 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/mips64.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     8818 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/mips64n32.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     9460 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/mipso32.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     7202 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/mn10300.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)    10997 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/names.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     7383 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/nds32.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     7375 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/nios2.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     7398 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/openrisc.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     8543 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/parisc.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     9320 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/powerpc.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     8546 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/powerpc64.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     6720 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/riscv32.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     6827 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/riscv64.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     9372 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/s390.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     8085 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/s390x.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     7159 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/score.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     9181 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/sh.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     7749 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/sh64.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     9299 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/sparc.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     8345 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/sparc64.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     6051 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/tile.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     6052 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/tile64.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     7039 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/unicore32.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)    10106 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/x32.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     7820 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/x86_64.py
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     8277 2023-05-08 09:12:25.000000 system-calls-6.4.0/system_calls/tables/xtensa.py
+drwxr-xr-x   0 marcin    (1003) marcin    (1006)        0 2023-05-08 09:16:42.340222 system-calls-6.4.0/system_calls.egg-info/
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     1361 2023-05-08 09:16:42.000000 system-calls-6.4.0/system_calls.egg-info/PKG-INFO
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)     1583 2023-05-08 09:16:42.000000 system-calls-6.4.0/system_calls.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)        1 2023-05-08 09:16:42.000000 system-calls-6.4.0/system_calls.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcin    (1003) marcin    (1006)       34 2023-05-08 09:16:42.000000 system-calls-6.4.0/system_calls.egg-info/top_level.txt
```

### Comparing `system-calls-5.19.0/LICENSE` & `system-calls-6.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/PKG-INFO` & `system-calls-6.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: system-calls
-Version: 5.19.0
+Version: 6.4.0
 Summary: Python module to check for system call number/name andavailability
 Home-page: https://github.com/hrw/python-syscalls
 Author: Marcin Juszkiewicz
 Author-email: marcin-python@juszkiewicz.com.pl
 Project-URL: Bug Tracker, https://github.com/hrw/python-syscalls/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `system-calls-5.19.0/README.md` & `system-calls-6.4.0/README.md`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/bin/syscall` & `system-calls-6.4.0/bin/syscall`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/man/syscall.1` & `system-calls-6.4.0/man/syscall.1`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/setup.py` & `system-calls-6.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="system-calls",
-    version="5.19.0",
+    version="6.4.0",
     author="Marcin Juszkiewicz",
     author_email="marcin-python@juszkiewicz.com.pl",
     description="Python module to check for system call number/name and"
     "availability",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hrw/python-syscalls",
```

### Comparing `system-calls-5.19.0/system_calls/__init__.py` & `system-calls-6.4.0/system_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/alpha.py` & `system-calls-6.4.0/system_calls/tables/alpha.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/arc.py` & `system-calls-6.4.0/system_calls/tables/arc.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/arm.py` & `system-calls-6.4.0/system_calls/tables/arm.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/arm64.py` & `system-calls-6.4.0/system_calls/tables/arm64.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/armoabi.py` & `system-calls-6.4.0/system_calls/tables/armoabi.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/avr32.py` & `system-calls-6.4.0/system_calls/tables/avr32.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/blackfin.py` & `system-calls-6.4.0/system_calls/tables/blackfin.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/c6x.py` & `system-calls-6.4.0/system_calls/tables/c6x.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/cris.py` & `system-calls-6.4.0/system_calls/tables/cris.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/csky.py` & `system-calls-6.4.0/system_calls/tables/csky.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/frv.py` & `system-calls-6.4.0/system_calls/tables/frv.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/h8300.py` & `system-calls-6.4.0/system_calls/tables/h8300.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/hexagon.py` & `system-calls-6.4.0/system_calls/tables/hexagon.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/i386.py` & `system-calls-6.4.0/system_calls/tables/i386.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/ia64.py` & `system-calls-6.4.0/system_calls/tables/ia64.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/loongarch64.py` & `system-calls-6.4.0/system_calls/tables/loongarch64.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/m32r.py` & `system-calls-6.4.0/system_calls/tables/m32r.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/m68k.py` & `system-calls-6.4.0/system_calls/tables/m68k.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/metag.py` & `system-calls-6.4.0/system_calls/tables/metag.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/microblaze.py` & `system-calls-6.4.0/system_calls/tables/microblaze.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/mips64.py` & `system-calls-6.4.0/system_calls/tables/mips64.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/mips64n32.py` & `system-calls-6.4.0/system_calls/tables/mips64n32.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/mipso32.py` & `system-calls-6.4.0/system_calls/tables/mipso32.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/mn10300.py` & `system-calls-6.4.0/system_calls/tables/mn10300.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/names.py` & `system-calls-6.4.0/system_calls/tables/names.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,14 +425,15 @@
     "removexattr",
     "rename",
     "renameat",
     "renameat2",
     "request_key",
     "restart_syscall",
     "riscv_flush_icache",
+    "riscv_hwprobe",
     "rmdir",
     "rseq",
     "rt_sigaction",
     "rt_sigpending",
     "rt_sigprocmask",
     "rt_sigqueueinfo",
     "rt_sigreturn",
```

### Comparing `system-calls-5.19.0/system_calls/tables/nds32.py` & `system-calls-6.4.0/system_calls/tables/nds32.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/nios2.py` & `system-calls-6.4.0/system_calls/tables/nios2.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/openrisc.py` & `system-calls-6.4.0/system_calls/tables/openrisc.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/parisc.py` & `system-calls-6.4.0/system_calls/tables/parisc.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/powerpc.py` & `system-calls-6.4.0/system_calls/tables/powerpc.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/powerpc64.py` & `system-calls-6.4.0/system_calls/tables/powerpc64.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/riscv32.py` & `system-calls-6.4.0/system_calls/tables/riscv32.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,14 +195,15 @@
     "recvmsg": 212,
     "remap_file_pages": 234,
     "removexattr": 14,
     "renameat2": 276,
     "request_key": 218,
     "restart_syscall": 128,
     "riscv_flush_icache": 259,
+    "riscv_hwprobe": 258,
     "rseq": 293,
     "rt_sigaction": 134,
     "rt_sigpending": 136,
     "rt_sigprocmask": 135,
     "rt_sigqueueinfo": 138,
     "rt_sigreturn": 139,
     "rt_sigsuspend": 133,
```

### Comparing `system-calls-5.19.0/system_calls/tables/riscv64.py` & `system-calls-6.4.0/system_calls/tables/riscv64.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,15 @@
     "recvmsg": 212,
     "remap_file_pages": 234,
     "removexattr": 14,
     "renameat2": 276,
     "request_key": 218,
     "restart_syscall": 128,
     "riscv_flush_icache": 259,
+    "riscv_hwprobe": 258,
     "rseq": 293,
     "rt_sigaction": 134,
     "rt_sigpending": 136,
     "rt_sigprocmask": 135,
     "rt_sigqueueinfo": 138,
     "rt_sigreturn": 139,
     "rt_sigsuspend": 133,
```

### Comparing `system-calls-5.19.0/system_calls/tables/s390.py` & `system-calls-6.4.0/system_calls/tables/s390.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,14 +175,15 @@
     "lsetxattr": 225,
     "lstat": 107,
     "lstat64": 196,
     "madvise": 219,
     "mbind": 268,
     "membarrier": 356,
     "memfd_create": 350,
+    "memfd_secret": 447,
     "migrate_pages": 287,
     "mincore": 218,
     "mkdir": 39,
     "mkdirat": 289,
     "mknod": 14,
     "mknodat": 290,
     "mlock": 150,
```

### Comparing `system-calls-5.19.0/system_calls/tables/s390x.py` & `system-calls-6.4.0/system_calls/tables/s390x.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,14 +149,15 @@
     "lseek": 19,
     "lsetxattr": 225,
     "lstat": 107,
     "madvise": 219,
     "mbind": 268,
     "membarrier": 356,
     "memfd_create": 350,
+    "memfd_secret": 447,
     "migrate_pages": 287,
     "mincore": 218,
     "mkdir": 39,
     "mkdirat": 289,
     "mknod": 14,
     "mknodat": 290,
     "mlock": 150,
```

### Comparing `system-calls-5.19.0/system_calls/tables/score.py` & `system-calls-6.4.0/system_calls/tables/score.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/sh.py` & `system-calls-6.4.0/system_calls/tables/sh.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/sh64.py` & `system-calls-6.4.0/system_calls/tables/sh64.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/sparc.py` & `system-calls-6.4.0/system_calls/tables/sparc.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/sparc64.py` & `system-calls-6.4.0/system_calls/tables/sparc64.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/tile.py` & `system-calls-6.4.0/system_calls/tables/tile.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/tile64.py` & `system-calls-6.4.0/system_calls/tables/tile64.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/unicore32.py` & `system-calls-6.4.0/system_calls/tables/unicore32.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/x32.py` & `system-calls-6.4.0/system_calls/tables/x32.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/x86_64.py` & `system-calls-6.4.0/system_calls/tables/x86_64.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls/tables/xtensa.py` & `system-calls-6.4.0/system_calls/tables/xtensa.py`

 * *Files identical despite different names*

### Comparing `system-calls-5.19.0/system_calls.egg-info/PKG-INFO` & `system-calls-6.4.0/system_calls.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: system-calls
-Version: 5.19.0
+Version: 6.4.0
 Summary: Python module to check for system call number/name andavailability
 Home-page: https://github.com/hrw/python-syscalls
 Author: Marcin Juszkiewicz
 Author-email: marcin-python@juszkiewicz.com.pl
 Project-URL: Bug Tracker, https://github.com/hrw/python-syscalls/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `system-calls-5.19.0/system_calls.egg-info/SOURCES.txt` & `system-calls-6.4.0/system_calls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

