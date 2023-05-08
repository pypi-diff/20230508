# Comparing `tmp/MCTThermalFace-0.1.1.tar.gz` & `tmp/MCTThermalFace-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MCTThermalFace-0.1.1.tar", last modified: Mon May  8 08:53:49 2023, max compression
+gzip compressed data, was "MCTThermalFace-0.1.2.tar", last modified: Mon May  8 09:03:31 2023, max compression
```

## Comparing `MCTThermalFace-0.1.1.tar` & `MCTThermalFace-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-08 08:53:49.288639 MCTThermalFace-0.1.1/
-drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-08 08:53:49.288639 MCTThermalFace-0.1.1/MCTThermalFace.egg-info/
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      401 2023-05-08 08:53:49.000000 MCTThermalFace-0.1.1/MCTThermalFace.egg-info/PKG-INFO
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      197 2023-05-08 08:53:49.000000 MCTThermalFace-0.1.1/MCTThermalFace.egg-info/SOURCES.txt
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)        1 2023-05-08 08:53:49.000000 MCTThermalFace-0.1.1/MCTThermalFace.egg-info/dependency_links.txt
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       38 2023-05-08 08:53:49.000000 MCTThermalFace-0.1.1/MCTThermalFace.egg-info/requires.txt
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)        1 2023-05-08 08:53:49.000000 MCTThermalFace-0.1.1/MCTThermalFace.egg-info/top_level.txt
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      401 2023-05-08 08:53:49.288639 MCTThermalFace-0.1.1/PKG-INFO
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       38 2023-05-08 08:53:49.288639 MCTThermalFace-0.1.1/setup.cfg
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      605 2023-05-08 08:53:00.000000 MCTThermalFace-0.1.1/setup.py
+drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-08 09:03:31.171722 MCTThermalFace-0.1.2/
+drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-08 09:03:31.171722 MCTThermalFace-0.1.2/MCTThermalFace.egg-info/
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1940 2023-05-08 09:03:31.000000 MCTThermalFace-0.1.2/MCTThermalFace.egg-info/PKG-INFO
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      197 2023-05-08 09:03:31.000000 MCTThermalFace-0.1.2/MCTThermalFace.egg-info/SOURCES.txt
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)        1 2023-05-08 09:03:31.000000 MCTThermalFace-0.1.2/MCTThermalFace.egg-info/dependency_links.txt
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       38 2023-05-08 09:03:31.000000 MCTThermalFace-0.1.2/MCTThermalFace.egg-info/requires.txt
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)        1 2023-05-08 09:03:31.000000 MCTThermalFace-0.1.2/MCTThermalFace.egg-info/top_level.txt
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1940 2023-05-08 09:03:31.171722 MCTThermalFace-0.1.2/PKG-INFO
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       38 2023-05-08 09:03:31.171722 MCTThermalFace-0.1.2/setup.cfg
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      782 2023-05-08 09:03:24.000000 MCTThermalFace-0.1.2/setup.py
```

