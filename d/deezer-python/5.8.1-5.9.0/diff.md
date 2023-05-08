# Comparing `tmp/deezer_python-5.8.1.tar.gz` & `tmp/deezer_python-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deezer_python-5.8.1.tar", max compression
+gzip compressed data, was "deezer_python-5.9.0.tar", max compression
```

## Comparing `deezer_python-5.8.1.tar` & `deezer_python-5.9.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1054 2022-12-02 14:40:39.402150 deezer_python-5.8.1/LICENSE.txt
--rw-r--r--   0        0        0    11594 2022-12-02 14:40:39.402150 deezer_python-5.8.1/README.md
--rw-r--r--   0        0        0     2244 2022-12-02 14:40:40.642147 deezer_python-5.8.1/pyproject.toml
--rw-r--r--   0        0        0      556 2022-12-02 14:40:40.586147 deezer_python-5.8.1/src/deezer/__init__.py
--rw-r--r--   0        0        0    20674 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/client.py
--rw-r--r--   0        0        0      530 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/dates.py
--rw-r--r--   0        0        0     1864 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/exceptions.py
--rw-r--r--   0        0        0     3745 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/pagination.py
--rw-r--r--   0        0        0      549 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/resources/__init__.py
--rw-r--r--   0        0        0     1734 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/resources/album.py
--rw-r--r--   0        0        0     2150 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/resources/artist.py
--rw-r--r--   0        0        0     2047 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/resources/chart.py
--rw-r--r--   0        0        0     1413 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/resources/editorial.py
--rw-r--r--   0        0        0     1043 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/resources/episode.py
--rw-r--r--   0        0        0     1355 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/resources/genre.py
--rw-r--r--   0        0        0     1400 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/resources/playlist.py
--rw-r--r--   0        0        0      914 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/resources/podcast.py
--rw-r--r--   0        0        0      805 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/resources/radio.py
--rw-r--r--   0        0        0     4006 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/resources/resource.py
--rw-r--r--   0        0        0     1546 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/resources/track.py
--rw-r--r--   0        0        0     2984 2022-12-02 14:40:39.406150 deezer_python-5.8.1/src/deezer/resources/user.py
--rw-r--r--   0        0        0    12450 1970-01-01 00:00:00.000000 deezer_python-5.8.1/setup.py
--rw-r--r--   0        0        0    12995 1970-01-01 00:00:00.000000 deezer_python-5.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-04-13 09:24:49.202700 deezer_python-5.9.0/LICENSE.txt
+-rw-r--r--   0        0        0    13246 2023-04-13 09:24:49.202700 deezer_python-5.9.0/README.md
+-rw-r--r--   0        0        0     2244 2023-04-13 09:24:50.086698 deezer_python-5.9.0/pyproject.toml
+-rw-r--r--   0        0        0      556 2023-04-13 09:24:50.046698 deezer_python-5.9.0/src/deezer/__init__.py
+-rw-r--r--   0        0        0    23250 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/client.py
+-rw-r--r--   0        0        0      530 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/dates.py
+-rw-r--r--   0        0        0     1864 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/exceptions.py
+-rw-r--r--   0        0        0     3745 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/pagination.py
+-rw-r--r--   0        0        0      549 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/__init__.py
+-rw-r--r--   0        0        0     1734 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/album.py
+-rw-r--r--   0        0        0     2150 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/artist.py
+-rw-r--r--   0        0        0     2047 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/chart.py
+-rw-r--r--   0        0        0     1413 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/editorial.py
+-rw-r--r--   0        0        0     1043 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/episode.py
+-rw-r--r--   0        0        0     1355 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/genre.py
+-rw-r--r--   0        0        0     1400 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/playlist.py
+-rw-r--r--   0        0        0      914 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/podcast.py
+-rw-r--r--   0        0        0      805 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/radio.py
+-rw-r--r--   0        0        0     4006 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/resource.py
+-rw-r--r--   0        0        0     1546 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/track.py
+-rw-r--r--   0        0        0     2984 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/user.py
+-rw-r--r--   0        0        0    14647 1970-01-01 00:00:00.000000 deezer_python-5.9.0/PKG-INFO
```

### Comparing `deezer_python-5.8.1/LICENSE.txt` & `deezer_python-5.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/README.md` & `deezer_python-5.9.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Deezer Python Client
 
 <p align="center">
-  <a href="https://github.com/browniebroke/deezer-python/actions?query=workflow%3ACI">
-    <img alt="CI Status" src="https://img.shields.io/github/workflow/status/browniebroke/deezer-python/CI?label=CI&logo=github&style=flat-square">
+  <a href="https://github.com/browniebroke/deezer-python/actions/workflows/ci.yml?query=branch%3Amain">
+    <img alt="CI Status" src="https://img.shields.io/github/actions/workflow/status/browniebroke/deezer-python/ci.yml?branch=main&logo=github&style=flat-square">
   </a>
-  <a href="https://deezer-python.readthedocs.io">
+  <a href="https://readthedocs.org/projects/deezer-python/builds/">
     <img src="https://img.shields.io/readthedocs/deezer-python.svg?logo=read-the-docs&style=flat-square" alt="Documentation Status">
   </a>
   <a href="https://codecov.io/gh/browniebroke/deezer-python">
     <img src="https://img.shields.io/codecov/c/github/browniebroke/deezer-python.svg?logo=codecov&style=flat-square" alt="Test coverage percentage">
   </a>
 </p>
 <p align="center">
@@ -32,14 +32,22 @@
   <img src="https://img.shields.io/pypi/pyversions/deezer-python.svg?style=flat-square" alt="pyversions">
   <img src="https://img.shields.io/pypi/l/deezer-python.svg?style=flat-square" alt="license">
   <a href="https://github.com/browniebroke/deezer-python">
     <img src="https://tokei.rs/b1/github/browniebroke/deezer-python" alt="LoC">
   </a>
 </p>
 
+---
+
+**Documentation**: <a href="https://deezer-python.readthedocs.io" target="_blank">https://deezer-python.readthedocs.io</a>
+
+**Source Code**: <a href="https://github.com/browniebroke/deezer-python" target="_blank">https://github.com/browniebroke/deezer-python </a>
+
+---
+
 A friendly Python wrapper around the [Deezer API](https://developers.deezer.com/api).
 
 ## Installation
 
 The package is published on
 [PyPI](https://pypi.org/project/deezer-python/) and can be installed by running:
 
@@ -62,38 +70,41 @@
 
 ## Contributors
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
-  <tr>
-    <td align="center"><a href="https://www.twitter.com/_BrunoAlla"><img src="https://avatars1.githubusercontent.com/u/861044?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Bruno Alla</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=browniebroke" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=browniebroke" title="Documentation">📖</a> <a href="#ideas-browniebroke" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-browniebroke" title="Maintenance">🚧</a> <a href="#platform-browniebroke" title="Packaging/porting to new platform">📦</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=browniebroke" title="Tests">⚠️</a></td>
-    <td align="center"><a href="https://github.com/misuzu"><img src="https://avatars1.githubusercontent.com/u/248143?v=4?s=100" width="100px;" alt=""/><br /><sub><b>misuzu</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=misuzu" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=misuzu" title="Documentation">📖</a> <a href="#ideas-misuzu" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=misuzu" title="Tests">⚠️</a></td>
-    <td align="center"><a href="https://github.com/pfouque"><img src="https://avatars1.githubusercontent.com/u/8300001?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Pascal</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=pfouque" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=pfouque" title="Tests">⚠️</a></td>
-    <td align="center"><a href="https://github.com/khamaileon"><img src="https://avatars2.githubusercontent.com/u/1322166?v=4?s=100" width="100px;" alt=""/><br /><sub><b>khamaileon</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=khamaileon" title="Documentation">📖</a></td>
-    <td align="center"><a href="https://github.com/sheregeda"><img src="https://avatars3.githubusercontent.com/u/2856444?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nikolay Sheregeda</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=sheregeda" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=sheregeda" title="Tests">⚠️</a></td>
-    <td align="center"><a href="https://github.com/horstmannmat"><img src="https://avatars1.githubusercontent.com/u/11761333?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Matheus Horstmann</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=horstmannmat" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=horstmannmat" title="Documentation">📖</a></td>
-    <td align="center"><a href="https://github.com/MDCEY"><img src="https://avatars2.githubusercontent.com/u/3812864?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Kieran Wynne</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=MDCEY" title="Code">💻</a></td>
-  </tr>
-  <tr>
-    <td align="center"><a href="https://github.com/jnth"><img src="https://avatars0.githubusercontent.com/u/7796167?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jonathan Virga</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=jnth" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=jnth" title="Documentation">📖</a></td>
-    <td align="center"><a href="https://github.com/hugovk"><img src="https://avatars2.githubusercontent.com/u/1324225?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Hugo</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=hugovk" title="Code">💻</a></td>
-    <td align="center"><a href="https://github.com/all-contributors/all-contributors-bot"><img src="https://avatars3.githubusercontent.com/u/46843839?v=4?s=100" width="100px;" alt=""/><br /><sub><b>allcontributors[bot]</b></sub></a><br /><a href="#infra-allcontributors" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
-    <td align="center"><a href="https://github.com/nrebena"><img src="https://avatars3.githubusercontent.com/u/49879400?v=4?s=100" width="100px;" alt=""/><br /><sub><b>nrebena</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/issues?q=author%3Anrebena" title="Bug reports">🐛</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=nrebena" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=nrebena" title="Tests">⚠️</a></td>
-    <td align="center"><a href="https://github.com/spvkgn"><img src="https://avatars0.githubusercontent.com/u/4147135?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Pavel</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/issues?q=author%3Aspvkgn" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="http://www.idiap.ch || www.edeltech.ch"><img src="https://avatars0.githubusercontent.com/u/898010?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Samuel Gaist</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=sgaist" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=sgaist" title="Tests">⚠️</a> <a href="#security-sgaist" title="Security">🛡️</a></td>
-    <td align="center"><a href="https://github.com/hithomasmorelli"><img src="https://avatars0.githubusercontent.com/u/22722644?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Thomas Morelli</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/issues?q=author%3Ahithomasmorelli" title="Bug reports">🐛</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=hithomasmorelli" title="Code">💻</a> <a href="#ideas-hithomasmorelli" title="Ideas, Planning, & Feedback">🤔</a></td>
-  </tr>
-  <tr>
-    <td align="center"><a href="https://naveen.syrusdark.website"><img src="https://avatars1.githubusercontent.com/u/49693820?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Naveen M K</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=naveen521kk" title="Code">💻</a> <a href="#infra-naveen521kk" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
-    <td align="center"><a href="https://github.com/Carababusha"><img src="https://avatars.githubusercontent.com/u/64437819?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Carababusha</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=Carababusha" title="Code">💻</a></td>
-    <td align="center"><a href="https://github.com/bjacquin"><img src="https://avatars.githubusercontent.com/u/5293357?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Bertrand Jacquin</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=bjacquin" title="Code">💻</a></td>
-    <td align="center"><a href="https://github.com/prndrbr"><img src="https://avatars.githubusercontent.com/u/96344856?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Pierre</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=prndrbr" title="Documentation">📖</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=prndrbr" title="Code">💻</a></td>
-  </tr>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.twitter.com/_BrunoAlla"><img src="https://avatars1.githubusercontent.com/u/861044?v=4?s=100" width="100px;" alt="Bruno Alla"/><br /><sub><b>Bruno Alla</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=browniebroke" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=browniebroke" title="Documentation">📖</a> <a href="#ideas-browniebroke" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-browniebroke" title="Maintenance">🚧</a> <a href="#platform-browniebroke" title="Packaging/porting to new platform">📦</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=browniebroke" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/misuzu"><img src="https://avatars1.githubusercontent.com/u/248143?v=4?s=100" width="100px;" alt="misuzu"/><br /><sub><b>misuzu</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=misuzu" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=misuzu" title="Documentation">📖</a> <a href="#ideas-misuzu" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=misuzu" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pfouque"><img src="https://avatars1.githubusercontent.com/u/8300001?v=4?s=100" width="100px;" alt="Pascal"/><br /><sub><b>Pascal</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=pfouque" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=pfouque" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/khamaileon"><img src="https://avatars2.githubusercontent.com/u/1322166?v=4?s=100" width="100px;" alt="khamaileon"/><br /><sub><b>khamaileon</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=khamaileon" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sheregeda"><img src="https://avatars3.githubusercontent.com/u/2856444?v=4?s=100" width="100px;" alt="Nikolay Sheregeda"/><br /><sub><b>Nikolay Sheregeda</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=sheregeda" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=sheregeda" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/horstmannmat"><img src="https://avatars1.githubusercontent.com/u/11761333?v=4?s=100" width="100px;" alt="Matheus Horstmann"/><br /><sub><b>Matheus Horstmann</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=horstmannmat" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=horstmannmat" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/MDCEY"><img src="https://avatars2.githubusercontent.com/u/3812864?v=4?s=100" width="100px;" alt="Kieran Wynne"/><br /><sub><b>Kieran Wynne</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=MDCEY" title="Code">💻</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jnth"><img src="https://avatars0.githubusercontent.com/u/7796167?v=4?s=100" width="100px;" alt="Jonathan Virga"/><br /><sub><b>Jonathan Virga</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=jnth" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=jnth" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/hugovk"><img src="https://avatars2.githubusercontent.com/u/1324225?v=4?s=100" width="100px;" alt="Hugo"/><br /><sub><b>Hugo</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=hugovk" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/all-contributors/all-contributors-bot"><img src="https://avatars3.githubusercontent.com/u/46843839?v=4?s=100" width="100px;" alt="allcontributors[bot]"/><br /><sub><b>allcontributors[bot]</b></sub></a><br /><a href="#infra-allcontributors" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nrebena"><img src="https://avatars3.githubusercontent.com/u/49879400?v=4?s=100" width="100px;" alt="nrebena"/><br /><sub><b>nrebena</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/issues?q=author%3Anrebena" title="Bug reports">🐛</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=nrebena" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=nrebena" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/spvkgn"><img src="https://avatars0.githubusercontent.com/u/4147135?v=4?s=100" width="100px;" alt="Pavel"/><br /><sub><b>Pavel</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/issues?q=author%3Aspvkgn" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://www.idiap.ch || www.edeltech.ch"><img src="https://avatars0.githubusercontent.com/u/898010?v=4?s=100" width="100px;" alt="Samuel Gaist"/><br /><sub><b>Samuel Gaist</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=sgaist" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=sgaist" title="Tests">⚠️</a> <a href="#security-sgaist" title="Security">🛡️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/hithomasmorelli"><img src="https://avatars0.githubusercontent.com/u/22722644?v=4?s=100" width="100px;" alt="Thomas Morelli"/><br /><sub><b>Thomas Morelli</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/issues?q=author%3Ahithomasmorelli" title="Bug reports">🐛</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=hithomasmorelli" title="Code">💻</a> <a href="#ideas-hithomasmorelli" title="Ideas, Planning, & Feedback">🤔</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://naveen.syrusdark.website"><img src="https://avatars1.githubusercontent.com/u/49693820?v=4?s=100" width="100px;" alt="Naveen M K"/><br /><sub><b>Naveen M K</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=naveen521kk" title="Code">💻</a> <a href="#infra-naveen521kk" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Carababusha"><img src="https://avatars.githubusercontent.com/u/64437819?v=4?s=100" width="100px;" alt="Carababusha"/><br /><sub><b>Carababusha</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=Carababusha" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/bjacquin"><img src="https://avatars.githubusercontent.com/u/5293357?v=4?s=100" width="100px;" alt="Bertrand Jacquin"/><br /><sub><b>Bertrand Jacquin</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=bjacquin" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/prndrbr"><img src="https://avatars.githubusercontent.com/u/96344856?v=4?s=100" width="100px;" alt="Pierre"/><br /><sub><b>Pierre</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=prndrbr" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=prndrbr" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://jonathanbangert.com"><img src="https://avatars.githubusercontent.com/u/74015378?v=4?s=100" width="100px;" alt="Jonathan"/><br /><sub><b>Jonathan</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=Un10ck3d" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=Un10ck3d" title="Documentation">📖</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=Un10ck3d" title="Tests">⚠️</a></td>
+    </tr>
+  </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
 # Deezer Python Client
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
       [Launch_demo_on_Binder] [PyPi_Status] [pyversions] [license] [LoC]
-A friendly Python wrapper around the [Deezer API](https://
-developers.deezer.com/api). ## Installation The package is published on [PyPI]
-(https://pypi.org/project/deezer-python/) and can be installed by running: pip
-install deezer-python ## Basic Use Easily query the Deezer API from you Python
-code. The data returned by the Deezer API is mapped to python resources:
-```python >>> client = deezer.Client() >>> client.get_album(680407).title
-'Monkey Business' ``` Ready for more? Look at our whole [documentation](http://
-deezer-python.readthedocs.io/) on Read The Docs or have a play in pre-populated
-Jupyter notebook [on Binder](https://mybinder.org/v2/gh/browniebroke/deezer-
-python/main?filepath=demo.ipynb). ## Contributors
-
-                       Bruno_Alla                                         misuzu                         Pascal                       khamaileon         Nikolay_Sheregeda               Matheus_Horstmann                  Kieran_Wynne
-
-             ð» ð ð¤ ð§ ð¦          ð» ð ð¤ â     ð» â ï¸             ð           ð» â ï¸�             ð» ð                  ð»
-
-                             Jonathan_Virga                                       Hugo            allcontributors[bot]             nrebena                       Pavel                   Samuel_Gaist                   Thomas_Morelli
-
-                                ð» ð                                 ð»                ð             ð ð» â ï        ð            ð» â ï¸ ð�      ð ð» ð¤
-
-                               Naveen_M_K                                      Carababusha           Bertrand_Jacquin                Pierre
-
-                                ð» ð                                 ð»                 ð»                ð ð»
+--- **Documentation**: https://deezer-python.readthedocs.io **Source Code**:
+https://github.com/browniebroke/deezer-python --- A friendly Python wrapper
+around the [Deezer API](https://developers.deezer.com/api). ## Installation The
+package is published on [PyPI](https://pypi.org/project/deezer-python/) and can
+be installed by running: pip install deezer-python ## Basic Use Easily query
+the Deezer API from you Python code. The data returned by the Deezer API is
+mapped to python resources: ```python >>> client = deezer.Client() >>>
+client.get_album(680407).title 'Monkey Business' ``` Ready for more? Look at
+our whole [documentation](http://deezer-python.readthedocs.io/) on Read The
+Docs or have a play in pre-populated Jupyter notebook [on Binder](https://
+mybinder.org/v2/gh/browniebroke/deezer-python/main?filepath=demo.ipynb). ##
+Contributors
+                      [Bruno_Alla]                                       [misuzu]                       [Pascal]                     [khamaileon]           [Nikolay_Sheregeda]                  [Matheus_Horstmann]                [Kieran_Wynne]
+                       Bruno_Alla                                         misuzu                         Pascal                       khamaileon             Nikolay_Sheregeda                    Matheus_Horstmann                  Kieran_Wynne
+             ð» ð ð¤ ð§ ð¦          ð» ð ð¤ â     ð» â ï¸             ð               ð» â ï¸                 ð» ð                  ð»
+                            [Jonathan_Virga]                                     [Hugo]             [allcontributors              [nrebena]                           [Pavel]                    [Samuel_Gaist]                 [Thomas_Morelli]
+                             Jonathan_Virga                                       Hugo                   [bot]]                    nrebena                             Pavel                      Samuel_Gaist                   Thomas_Morelli
+                                ð» ð                                 ð»        allcontributors[bot]         ð ð» â ï¸             ð              ð» â ï¸ ð�      ð ð» ð¤
+                                                                                                          ð
+                              [Naveen_M_K]                                   [Carababusha]          [Bertrand_Jacquin]              [Pierre]                     [Jonathan]
+                               Naveen_M_K                                     Carababusha            Bertrand_Jacquin                Pierre                       Jonathan
+                                ð» ð                                ð»                  ð»                ð» ð          ð» ð â ï¸
    This project follows the [all-contributors](https://allcontributors.org)
 specification. Contributions of any kind are welcome!
```

### Comparing `deezer_python-5.8.1/pyproject.toml` & `deezer_python-5.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deezer-python"
-version = "5.8.1"
+version = "5.9.0"
 description = "A friendly wrapper library for the Deezer API"
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["deezer", "sdk", "client", "requests"]
 repository = "https://github.com/browniebroke/deezer-python"
 documentation = "https://deezer-python.readthedocs.io"
@@ -35,15 +35,15 @@
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
 sphinx = ">=4.0"
 sphinx-autobuild = ">=2021.0"
 sphinx-rtd-theme = ">=1.0"
 
 [tool.poetry.group.dev.dependencies]
-coverage = "^6.0"
+coverage = "^7.0"
 environs = "^9.3"
 pytest = "^7.0"
 pytest-cov = "^4.0"
 pytest-mock = "^3.6"
 pytest-vcr = "^1.0"
 vcrpy = "^4.1"
 deezer-oauth-cli = "^0.4"
```

### Comparing `deezer_python-5.8.1/src/deezer/__init__.py` & `deezer_python-5.9.0/src/deezer/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Podcast,
     Radio,
     Resource,
     Track,
     User,
 )
 
-__version__ = "5.8.1"
+__version__ = "5.9.0"
 __all__ = [
     "Album",
     "Artist",
     "Chart",
     "Client",
     "Editorial",
     "Episode",
```

### Comparing `deezer_python-5.8.1/src/deezer/client.py` & `deezer_python-5.9.0/src/deezer/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -348,14 +348,67 @@
         Get the user with the given ID.
 
         :returns: a :class:`~deezer.User` object
         """
         user_id_str = str(user_id) if user_id else "me"
         return self.request("GET", f"user/{user_id_str}")
 
+    def get_user_recommended_tracks(self, **kwargs) -> PaginatedList[Track]:
+        """
+        Get user's recommended tracks.
+
+        :returns: a :class:`PaginatedList <deezer.PaginatedList>`
+                  of :class:`Track <deezer.Track>` instances
+        """
+        return PaginatedList(
+            client=self, base_path="user/me/recommendations/tracks", **kwargs
+        )
+
+    def get_user_recommended_albums(self, **kwargs) -> PaginatedList[Album]:
+        """
+        Get user's recommended albums.
+
+        :returns: a :class:`PaginatedList <deezer.PaginatedList>`
+                  of :class:`Track <deezer.Album>` instances
+        """
+        return PaginatedList(
+            client=self, base_path="user/me/recommendations/albums", **kwargs
+        )
+
+    def get_user_recommended_artists(self, **kwargs) -> PaginatedList[Artist]:
+        """
+        Get user's recommended artists.
+
+        :returns: a :class:`PaginatedList <deezer.PaginatedList>`
+                  of :class:`Track <deezer.Artist>` instances
+        """
+        return PaginatedList(
+            client=self, base_path="user/me/recommendations/artists", **kwargs
+        )
+
+    def get_user_recommended_playlists(self, **kwargs) -> PaginatedList[Playlist]:
+        """
+        Get user's recommended playlist.
+
+        :returns: a :class:`PaginatedList <deezer.PaginatedList>`
+                  of :class:`Track <deezer.Playlist>` instances
+        """
+        return PaginatedList(
+            client=self, base_path="user/me/recommendations/playlists", **kwargs
+        )
+
+    def get_user_flow(self, **kwargs) -> PaginatedList[Track]:
+        """
+        Get user's flow.
+
+        :returns: a :class:`PaginatedList <deezer.PaginatedList>`
+                  of :class:`Track <deezer.Track>` instances
+        """
+        return PaginatedList(client=self, base_path="user/me/flow", **kwargs)
+
     def get_user_albums(self, user_id: int | None = None) -> PaginatedList[Album]:
         """
         Get the favourites albums for the given user_id if provided or current user if not.
 
         :param user_id: the user ID to get favourites albums.
         :returns: a :class:`~deezer.pagination.PaginatedList`
                   of :class:`~deezer.Album` objects.
@@ -601,7 +654,28 @@
         """
         return self._search(
             path="artist",
             query=query,
             strict=strict,
             ordering=ordering,
         )
+
+    def search_playlists(
+        self,
+        query: str = "",
+        strict: bool | None = None,
+        ordering: str | None = None,
+    ) -> PaginatedList[Playlist]:
+        """
+        Search playlists matching the given query.
+
+        :param query: the query to search for, this is directly passed as q query.
+        :param strict: whether to disable fuzzy search and enable strict mode.
+        :param ordering: see Deezer API docs for possible values.
+        :return: list of :class:`~deezer.Playlist` instances.
+        """
+        return self._search(
+            path="playlist",
+            query=query,
+            strict=strict,
+            ordering=ordering,
+        )
```

### Comparing `deezer_python-5.8.1/src/deezer/dates.py` & `deezer_python-5.9.0/src/deezer/dates.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/src/deezer/exceptions.py` & `deezer_python-5.9.0/src/deezer/exceptions.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/src/deezer/pagination.py` & `deezer_python-5.9.0/src/deezer/pagination.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/src/deezer/resources/__init__.py` & `deezer_python-5.9.0/src/deezer/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/src/deezer/resources/album.py` & `deezer_python-5.9.0/src/deezer/resources/album.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/src/deezer/resources/artist.py` & `deezer_python-5.9.0/src/deezer/resources/artist.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/src/deezer/resources/chart.py` & `deezer_python-5.9.0/src/deezer/resources/chart.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/src/deezer/resources/editorial.py` & `deezer_python-5.9.0/src/deezer/resources/editorial.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/src/deezer/resources/episode.py` & `deezer_python-5.9.0/src/deezer/resources/episode.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/src/deezer/resources/genre.py` & `deezer_python-5.9.0/src/deezer/resources/genre.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/src/deezer/resources/playlist.py` & `deezer_python-5.9.0/src/deezer/resources/playlist.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/src/deezer/resources/podcast.py` & `deezer_python-5.9.0/src/deezer/resources/podcast.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/src/deezer/resources/radio.py` & `deezer_python-5.9.0/src/deezer/resources/radio.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/src/deezer/resources/resource.py` & `deezer_python-5.9.0/src/deezer/resources/resource.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/src/deezer/resources/track.py` & `deezer_python-5.9.0/src/deezer/resources/track.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/src/deezer/resources/user.py` & `deezer_python-5.9.0/src/deezer/resources/user.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.8.1/setup.py` & `deezer_python-5.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,144 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: deezer-python
+Version: 5.9.0
+Summary: A friendly wrapper library for the Deezer API
+Home-page: https://github.com/browniebroke/deezer-python
+License: MIT
+Keywords: deezer,sdk,client,requests
+Author: Bruno Alla
+Author-email: alla.brunoo@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: requests (>=2.18)
+Project-URL: Bug Tracker, https://github.com/browniebroke/deezer-python/issues
+Project-URL: Changelog, https://deezer-python.readthedocs.io/en/latest/changelog.html
+Project-URL: Documentation, https://deezer-python.readthedocs.io
+Project-URL: Mastodon, https://fosstodon.org/@browniebroke
+Project-URL: Repository, https://github.com/browniebroke/deezer-python
+Project-URL: Twitter, https://twitter.com/_BrunoAlla
+Description-Content-Type: text/markdown
+
+# Deezer Python Client
+
+<p align="center">
+  <a href="https://github.com/browniebroke/deezer-python/actions/workflows/ci.yml?query=branch%3Amain">
+    <img alt="CI Status" src="https://img.shields.io/github/actions/workflow/status/browniebroke/deezer-python/ci.yml?branch=main&logo=github&style=flat-square">
+  </a>
+  <a href="https://readthedocs.org/projects/deezer-python/builds/">
+    <img src="https://img.shields.io/readthedocs/deezer-python.svg?logo=read-the-docs&style=flat-square" alt="Documentation Status">
+  </a>
+  <a href="https://codecov.io/gh/browniebroke/deezer-python">
+    <img src="https://img.shields.io/codecov/c/github/browniebroke/deezer-python.svg?logo=codecov&style=flat-square" alt="Test coverage percentage">
+  </a>
+</p>
+<p align="center">
+  <a href="https://python-poetry.org/">
+    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">
+  </a>
+  <a href="https://github.com/ambv/black">
+    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">
+  </a>
+  <a href="https://github.com/pre-commit/pre-commit">
+    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">
+  </a>
+</p>
+<p align="center">
+  <a href="https://mybinder.org/v2/gh/browniebroke/deezer-python/main?filepath=demo.ipynb">
+    <img src="https://mybinder.org/badge_logo.svg" alt="Launch demo on Binder">
+  </a>
+  <a href="https://pypi.org/project/deezer-python/">
+    <img src="https://img.shields.io/pypi/v/deezer-python.svg?logo=python&amp;logoColor=fff&amp;style=flat-square" alt="PyPi Status">
+  </a>
+  <img src="https://img.shields.io/pypi/pyversions/deezer-python.svg?style=flat-square" alt="pyversions">
+  <img src="https://img.shields.io/pypi/l/deezer-python.svg?style=flat-square" alt="license">
+  <a href="https://github.com/browniebroke/deezer-python">
+    <img src="https://tokei.rs/b1/github/browniebroke/deezer-python" alt="LoC">
+  </a>
+</p>
+
+---
+
+**Documentation**: <a href="https://deezer-python.readthedocs.io" target="_blank">https://deezer-python.readthedocs.io</a>
+
+**Source Code**: <a href="https://github.com/browniebroke/deezer-python" target="_blank">https://github.com/browniebroke/deezer-python </a>
+
+---
+
+A friendly Python wrapper around the [Deezer API](https://developers.deezer.com/api).
+
+## Installation
+
+The package is published on
+[PyPI](https://pypi.org/project/deezer-python/) and can be installed by running:
+
+    pip install deezer-python
+
+## Basic Use
+
+Easily query the Deezer API from you Python code. The data returned by the Deezer
+API is mapped to python resources:
+
+```python
+>>> client = deezer.Client()
+>>> client.get_album(680407).title
+'Monkey Business'
+```
+
+Ready for more? Look at our whole [documentation](http://deezer-python.readthedocs.io/)
+on Read The Docs or have a play in pre-populated Jupyter notebook
+[on Binder](https://mybinder.org/v2/gh/browniebroke/deezer-python/main?filepath=demo.ipynb).
+
+## Contributors
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.twitter.com/_BrunoAlla"><img src="https://avatars1.githubusercontent.com/u/861044?v=4?s=100" width="100px;" alt="Bruno Alla"/><br /><sub><b>Bruno Alla</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=browniebroke" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=browniebroke" title="Documentation">📖</a> <a href="#ideas-browniebroke" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-browniebroke" title="Maintenance">🚧</a> <a href="#platform-browniebroke" title="Packaging/porting to new platform">📦</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=browniebroke" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/misuzu"><img src="https://avatars1.githubusercontent.com/u/248143?v=4?s=100" width="100px;" alt="misuzu"/><br /><sub><b>misuzu</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=misuzu" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=misuzu" title="Documentation">📖</a> <a href="#ideas-misuzu" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=misuzu" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pfouque"><img src="https://avatars1.githubusercontent.com/u/8300001?v=4?s=100" width="100px;" alt="Pascal"/><br /><sub><b>Pascal</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=pfouque" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=pfouque" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/khamaileon"><img src="https://avatars2.githubusercontent.com/u/1322166?v=4?s=100" width="100px;" alt="khamaileon"/><br /><sub><b>khamaileon</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=khamaileon" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sheregeda"><img src="https://avatars3.githubusercontent.com/u/2856444?v=4?s=100" width="100px;" alt="Nikolay Sheregeda"/><br /><sub><b>Nikolay Sheregeda</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=sheregeda" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=sheregeda" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/horstmannmat"><img src="https://avatars1.githubusercontent.com/u/11761333?v=4?s=100" width="100px;" alt="Matheus Horstmann"/><br /><sub><b>Matheus Horstmann</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=horstmannmat" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=horstmannmat" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/MDCEY"><img src="https://avatars2.githubusercontent.com/u/3812864?v=4?s=100" width="100px;" alt="Kieran Wynne"/><br /><sub><b>Kieran Wynne</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=MDCEY" title="Code">💻</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jnth"><img src="https://avatars0.githubusercontent.com/u/7796167?v=4?s=100" width="100px;" alt="Jonathan Virga"/><br /><sub><b>Jonathan Virga</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=jnth" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=jnth" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/hugovk"><img src="https://avatars2.githubusercontent.com/u/1324225?v=4?s=100" width="100px;" alt="Hugo"/><br /><sub><b>Hugo</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=hugovk" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/all-contributors/all-contributors-bot"><img src="https://avatars3.githubusercontent.com/u/46843839?v=4?s=100" width="100px;" alt="allcontributors[bot]"/><br /><sub><b>allcontributors[bot]</b></sub></a><br /><a href="#infra-allcontributors" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nrebena"><img src="https://avatars3.githubusercontent.com/u/49879400?v=4?s=100" width="100px;" alt="nrebena"/><br /><sub><b>nrebena</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/issues?q=author%3Anrebena" title="Bug reports">🐛</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=nrebena" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=nrebena" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/spvkgn"><img src="https://avatars0.githubusercontent.com/u/4147135?v=4?s=100" width="100px;" alt="Pavel"/><br /><sub><b>Pavel</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/issues?q=author%3Aspvkgn" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://www.idiap.ch || www.edeltech.ch"><img src="https://avatars0.githubusercontent.com/u/898010?v=4?s=100" width="100px;" alt="Samuel Gaist"/><br /><sub><b>Samuel Gaist</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=sgaist" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=sgaist" title="Tests">⚠️</a> <a href="#security-sgaist" title="Security">🛡️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/hithomasmorelli"><img src="https://avatars0.githubusercontent.com/u/22722644?v=4?s=100" width="100px;" alt="Thomas Morelli"/><br /><sub><b>Thomas Morelli</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/issues?q=author%3Ahithomasmorelli" title="Bug reports">🐛</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=hithomasmorelli" title="Code">💻</a> <a href="#ideas-hithomasmorelli" title="Ideas, Planning, & Feedback">🤔</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://naveen.syrusdark.website"><img src="https://avatars1.githubusercontent.com/u/49693820?v=4?s=100" width="100px;" alt="Naveen M K"/><br /><sub><b>Naveen M K</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=naveen521kk" title="Code">💻</a> <a href="#infra-naveen521kk" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Carababusha"><img src="https://avatars.githubusercontent.com/u/64437819?v=4?s=100" width="100px;" alt="Carababusha"/><br /><sub><b>Carababusha</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=Carababusha" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/bjacquin"><img src="https://avatars.githubusercontent.com/u/5293357?v=4?s=100" width="100px;" alt="Bertrand Jacquin"/><br /><sub><b>Bertrand Jacquin</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=bjacquin" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/prndrbr"><img src="https://avatars.githubusercontent.com/u/96344856?v=4?s=100" width="100px;" alt="Pierre"/><br /><sub><b>Pierre</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=prndrbr" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=prndrbr" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://jonathanbangert.com"><img src="https://avatars.githubusercontent.com/u/74015378?v=4?s=100" width="100px;" alt="Jonathan"/><br /><sub><b>Jonathan</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=Un10ck3d" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=Un10ck3d" title="Documentation">📖</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=Un10ck3d" title="Tests">⚠️</a></td>
+    </tr>
+  </tbody>
+</table>
 
-package_dir = \
-{'': 'src'}
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
 
-packages = \
-['deezer', 'deezer.resources']
+<!-- ALL-CONTRIBUTORS-LIST:END -->
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['requests>=2.18']
-
-setup_kwargs = {
-    'name': 'deezer-python',
-    'version': '5.8.1',
-    'description': 'A friendly wrapper library for the Deezer API',
-    'long_description': '# Deezer Python Client\n\n<p align="center">\n  <a href="https://github.com/browniebroke/deezer-python/actions?query=workflow%3ACI">\n    <img alt="CI Status" src="https://img.shields.io/github/workflow/status/browniebroke/deezer-python/CI?label=CI&logo=github&style=flat-square">\n  </a>\n  <a href="https://deezer-python.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/deezer-python.svg?logo=read-the-docs&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/browniebroke/deezer-python">\n    <img src="https://img.shields.io/codecov/c/github/browniebroke/deezer-python.svg?logo=codecov&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://mybinder.org/v2/gh/browniebroke/deezer-python/main?filepath=demo.ipynb">\n    <img src="https://mybinder.org/badge_logo.svg" alt="Launch demo on Binder">\n  </a>\n  <a href="https://pypi.org/project/deezer-python/">\n    <img src="https://img.shields.io/pypi/v/deezer-python.svg?logo=python&amp;logoColor=fff&amp;style=flat-square" alt="PyPi Status">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/deezer-python.svg?style=flat-square" alt="pyversions">\n  <img src="https://img.shields.io/pypi/l/deezer-python.svg?style=flat-square" alt="license">\n  <a href="https://github.com/browniebroke/deezer-python">\n    <img src="https://tokei.rs/b1/github/browniebroke/deezer-python" alt="LoC">\n  </a>\n</p>\n\nA friendly Python wrapper around the [Deezer API](https://developers.deezer.com/api).\n\n## Installation\n\nThe package is published on\n[PyPI](https://pypi.org/project/deezer-python/) and can be installed by running:\n\n    pip install deezer-python\n\n## Basic Use\n\nEasily query the Deezer API from you Python code. The data returned by the Deezer\nAPI is mapped to python resources:\n\n```python\n>>> client = deezer.Client()\n>>> client.get_album(680407).title\n\'Monkey Business\'\n```\n\nReady for more? Look at our whole [documentation](http://deezer-python.readthedocs.io/)\non Read The Docs or have a play in pre-populated Jupyter notebook\n[on Binder](https://mybinder.org/v2/gh/browniebroke/deezer-python/main?filepath=demo.ipynb).\n\n## Contributors\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tr>\n    <td align="center"><a href="https://www.twitter.com/_BrunoAlla"><img src="https://avatars1.githubusercontent.com/u/861044?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Bruno Alla</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=browniebroke" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=browniebroke" title="Documentation">📖</a> <a href="#ideas-browniebroke" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-browniebroke" title="Maintenance">🚧</a> <a href="#platform-browniebroke" title="Packaging/porting to new platform">📦</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=browniebroke" title="Tests">⚠️</a></td>\n    <td align="center"><a href="https://github.com/misuzu"><img src="https://avatars1.githubusercontent.com/u/248143?v=4?s=100" width="100px;" alt=""/><br /><sub><b>misuzu</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=misuzu" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=misuzu" title="Documentation">📖</a> <a href="#ideas-misuzu" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=misuzu" title="Tests">⚠️</a></td>\n    <td align="center"><a href="https://github.com/pfouque"><img src="https://avatars1.githubusercontent.com/u/8300001?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Pascal</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=pfouque" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=pfouque" title="Tests">⚠️</a></td>\n    <td align="center"><a href="https://github.com/khamaileon"><img src="https://avatars2.githubusercontent.com/u/1322166?v=4?s=100" width="100px;" alt=""/><br /><sub><b>khamaileon</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=khamaileon" title="Documentation">📖</a></td>\n    <td align="center"><a href="https://github.com/sheregeda"><img src="https://avatars3.githubusercontent.com/u/2856444?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nikolay Sheregeda</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=sheregeda" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=sheregeda" title="Tests">⚠️</a></td>\n    <td align="center"><a href="https://github.com/horstmannmat"><img src="https://avatars1.githubusercontent.com/u/11761333?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Matheus Horstmann</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=horstmannmat" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=horstmannmat" title="Documentation">📖</a></td>\n    <td align="center"><a href="https://github.com/MDCEY"><img src="https://avatars2.githubusercontent.com/u/3812864?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Kieran Wynne</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=MDCEY" title="Code">💻</a></td>\n  </tr>\n  <tr>\n    <td align="center"><a href="https://github.com/jnth"><img src="https://avatars0.githubusercontent.com/u/7796167?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jonathan Virga</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=jnth" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=jnth" title="Documentation">📖</a></td>\n    <td align="center"><a href="https://github.com/hugovk"><img src="https://avatars2.githubusercontent.com/u/1324225?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Hugo</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=hugovk" title="Code">💻</a></td>\n    <td align="center"><a href="https://github.com/all-contributors/all-contributors-bot"><img src="https://avatars3.githubusercontent.com/u/46843839?v=4?s=100" width="100px;" alt=""/><br /><sub><b>allcontributors[bot]</b></sub></a><br /><a href="#infra-allcontributors" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>\n    <td align="center"><a href="https://github.com/nrebena"><img src="https://avatars3.githubusercontent.com/u/49879400?v=4?s=100" width="100px;" alt=""/><br /><sub><b>nrebena</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/issues?q=author%3Anrebena" title="Bug reports">🐛</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=nrebena" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=nrebena" title="Tests">⚠️</a></td>\n    <td align="center"><a href="https://github.com/spvkgn"><img src="https://avatars0.githubusercontent.com/u/4147135?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Pavel</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/issues?q=author%3Aspvkgn" title="Bug reports">🐛</a></td>\n    <td align="center"><a href="http://www.idiap.ch || www.edeltech.ch"><img src="https://avatars0.githubusercontent.com/u/898010?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Samuel Gaist</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=sgaist" title="Code">💻</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=sgaist" title="Tests">⚠️</a> <a href="#security-sgaist" title="Security">🛡️</a></td>\n    <td align="center"><a href="https://github.com/hithomasmorelli"><img src="https://avatars0.githubusercontent.com/u/22722644?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Thomas Morelli</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/issues?q=author%3Ahithomasmorelli" title="Bug reports">🐛</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=hithomasmorelli" title="Code">💻</a> <a href="#ideas-hithomasmorelli" title="Ideas, Planning, & Feedback">🤔</a></td>\n  </tr>\n  <tr>\n    <td align="center"><a href="https://naveen.syrusdark.website"><img src="https://avatars1.githubusercontent.com/u/49693820?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Naveen M K</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=naveen521kk" title="Code">💻</a> <a href="#infra-naveen521kk" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>\n    <td align="center"><a href="https://github.com/Carababusha"><img src="https://avatars.githubusercontent.com/u/64437819?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Carababusha</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=Carababusha" title="Code">💻</a></td>\n    <td align="center"><a href="https://github.com/bjacquin"><img src="https://avatars.githubusercontent.com/u/5293357?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Bertrand Jacquin</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=bjacquin" title="Code">💻</a></td>\n    <td align="center"><a href="https://github.com/prndrbr"><img src="https://avatars.githubusercontent.com/u/96344856?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Pierre</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-python/commits?author=prndrbr" title="Documentation">📖</a> <a href="https://github.com/browniebroke/deezer-python/commits?author=prndrbr" title="Code">💻</a></td>\n  </tr>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://allcontributors.org) specification.\nContributions of any kind are welcome!\n',
-    'author': 'Bruno Alla',
-    'author_email': 'alla.brunoo@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/browniebroke/deezer-python',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+This project follows the [all-contributors](https://allcontributors.org) specification.
+Contributions of any kind are welcome!
 
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,42 +1,47 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['deezer', 'deezer.resources'] package_data = \ {'': ['*']}
-install_requires = \ ['requests>=2.18'] setup_kwargs = { 'name': 'deezer-
-python', 'version': '5.8.1', 'description': 'A friendly wrapper library for the
-Deezer API', 'long_description': '# Deezer Python Client\n\n
-     \n \n_[CI_Status]\n\n \n_[Documentation_Status]\n\n \n_[Test_coverage
-                                percentage]\n\n
-\n
-             \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
-\n
-    \n \n_[Launch_demo_on_Binder]\n\n \n_[PyPi_Status]\n\n [pyversions]\n
-                           [license]\n \n_[LoC]\n\n
-\n\nA friendly Python wrapper around the [Deezer API](https://
-developers.deezer.com/api).\n\n## Installation\n\nThe package is published on\n
-[PyPI](https://pypi.org/project/deezer-python/) and can be installed by
-running:\n\n pip install deezer-python\n\n## Basic Use\n\nEasily query the
-Deezer API from you Python code. The data returned by the Deezer\nAPI is mapped
-to python resources:\n\n```python\n>>> client = deezer.Client()\n>>>
-client.get_album(680407).title\n\'Monkey Business\'\n```\n\nReady for more?
-Look at our whole [documentation](http://deezer-python.readthedocs.io/)\non
-Read The Docs or have a play in pre-populated Jupyter notebook\n[on Binder]
-(https://mybinder.org/v2/gh/browniebroke/deezer-python/
-main?filepath=demo.ipynb).\n\n## Contributors\n\n\n\n\n
-
-                       Bruno_Alla                                         misuzu                         Pascal                       khamaileon         Nikolay_Sheregeda               Matheus_Horstmann                  Kieran_Wynne
-
-             ð» ð ð¤ ð§ ð¦          ð» ð ð¤ â     ð» â ï¸             ð           ð» â ï¸�             ð» ð                  ð»
-
-                             Jonathan_Virga                                       Hugo            allcontributors[bot]             nrebena                       Pavel                   Samuel_Gaist                   Thomas_Morelli
-
-                                ð» ð                                 ð»                ð             ð ð» â ï        ð            ð» â ï¸ ð�      ð ð» ð¤
-
-                               Naveen_M_K                                      Carababusha           Bertrand_Jacquin                Pierre
-
-                                ð» ð                                 ð»                 ð»                ð ð»
-\n\n\n\n\n\n\nThis project follows the [all-contributors](https://
-allcontributors.org) specification.\nContributions of any kind are welcome!\n',
-'author': 'Bruno Alla', 'author_email': 'alla.brunoo@gmail.com', 'maintainer':
-'None', 'maintainer_email': 'None', 'url': 'https://github.com/browniebroke/
-deezer-python', 'package_dir': package_dir, 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: deezer-python Version: 5.9.0 Summary: A friendly
+wrapper library for the Deezer API Home-page: https://github.com/browniebroke/
+deezer-python License: MIT Keywords: deezer,sdk,client,requests Author: Bruno
+Alla Author-email: alla.brunoo@gmail.com Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Dist: requests (>=2.18) Project-URL: Bug Tracker, https://
+github.com/browniebroke/deezer-python/issues Project-URL: Changelog, https://
+deezer-python.readthedocs.io/en/latest/changelog.html Project-URL:
+Documentation, https://deezer-python.readthedocs.io Project-URL: Mastodon,
+https://fosstodon.org/@browniebroke Project-URL: Repository, https://
+github.com/browniebroke/deezer-python Project-URL: Twitter, https://
+twitter.com/_BrunoAlla Description-Content-Type: text/markdown # Deezer Python
+Client
+         [CI_Status] [Documentation_Status] [Test_coverage_percentage]
+                         [Poetry] [black] [pre-commit]
+      [Launch_demo_on_Binder] [PyPi_Status] [pyversions] [license] [LoC]
+--- **Documentation**: https://deezer-python.readthedocs.io **Source Code**:
+https://github.com/browniebroke/deezer-python --- A friendly Python wrapper
+around the [Deezer API](https://developers.deezer.com/api). ## Installation The
+package is published on [PyPI](https://pypi.org/project/deezer-python/) and can
+be installed by running: pip install deezer-python ## Basic Use Easily query
+the Deezer API from you Python code. The data returned by the Deezer API is
+mapped to python resources: ```python >>> client = deezer.Client() >>>
+client.get_album(680407).title 'Monkey Business' ``` Ready for more? Look at
+our whole [documentation](http://deezer-python.readthedocs.io/) on Read The
+Docs or have a play in pre-populated Jupyter notebook [on Binder](https://
+mybinder.org/v2/gh/browniebroke/deezer-python/main?filepath=demo.ipynb). ##
+Contributors
+                      [Bruno_Alla]                                       [misuzu]                       [Pascal]                     [khamaileon]           [Nikolay_Sheregeda]                  [Matheus_Horstmann]                [Kieran_Wynne]
+                       Bruno_Alla                                         misuzu                         Pascal                       khamaileon             Nikolay_Sheregeda                    Matheus_Horstmann                  Kieran_Wynne
+             ð» ð ð¤ ð§ ð¦          ð» ð ð¤ â     ð» â ï¸             ð               ð» â ï¸                 ð» ð                  ð»
+                            [Jonathan_Virga]                                     [Hugo]             [allcontributors              [nrebena]                           [Pavel]                    [Samuel_Gaist]                 [Thomas_Morelli]
+                             Jonathan_Virga                                       Hugo                   [bot]]                    nrebena                             Pavel                      Samuel_Gaist                   Thomas_Morelli
+                                ð» ð                                 ð»        allcontributors[bot]         ð ð» â ï¸             ð              ð» â ï¸ ð�      ð ð» ð¤
+                                                                                                          ð
+                              [Naveen_M_K]                                   [Carababusha]          [Bertrand_Jacquin]              [Pierre]                     [Jonathan]
+                               Naveen_M_K                                     Carababusha            Bertrand_Jacquin                Pierre                       Jonathan
+                                ð» ð                                ð»                  ð»                ð» ð          ð» ð â ï¸
+   This project follows the [all-contributors](https://allcontributors.org)
+specification. Contributions of any kind are welcome!
```

