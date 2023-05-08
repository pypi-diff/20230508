# Comparing `tmp/lastversion-2.4.8.tar.gz` & `tmp/lastversion-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lastversion-2.4.8.tar", last modified: Mon Dec  5 18:50:41 2022, max compression
+gzip compressed data, was "lastversion-2.4.9.tar", last modified: Mon Jan 23 05:53:28 2023, max compression
```

## Comparing `lastversion-2.4.8.tar` & `lastversion-2.4.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:50:41.364140 lastversion-2.4.8/
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2022-12-05 18:50:32.000000 lastversion-2.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       57 2022-12-05 18:50:32.000000 lastversion-2.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    25238 2022-12-05 18:50:41.364140 lastversion-2.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    19820 2022-12-05 18:50:32.000000 lastversion-2.4.8/README-ZH-CN.md
--rw-r--r--   0 runner    (1001) docker     (122)    24631 2022-12-05 18:50:32.000000 lastversion-2.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:50:41.364140 lastversion-2.4.8/lastversion/
--rw-r--r--   0 runner    (1001) docker     (122)     1226 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/BitBucketRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     3093 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/FeedRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)    27723 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/GitHubRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     2524 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/GitLabRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)    14030 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/GiteaRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/HelmChartRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     4118 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/HolderFactory.py
--rw-r--r--   0 runner    (1001) docker     (122)      945 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/LocalVersionSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     1980 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/MercurialRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)    11860 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/ProjectHolder.py
--rw-r--r--   0 runner    (1001) docker     (122)     3103 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/PypiRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/SourceForgeRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     3914 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/SystemRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     6082 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/Version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3708 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/WikipediaRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     3121 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/WordPressPluginRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)       58 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       46 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1123 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/argparse_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    27891 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/lastversion.py
--rw-r--r--   0 runner    (1001) docker     (122)      681 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/spdx_id_to_rpmspec.py
--rw-r--r--   0 runner    (1001) docker     (122)     6312 2022-12-05 18:50:32.000000 lastversion-2.4.8/lastversion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:50:41.364140 lastversion-2.4.8/lastversion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    25238 2022-12-05 18:50:41.000000 lastversion-2.4.8/lastversion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2022-12-05 18:50:41.000000 lastversion-2.4.8/lastversion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-05 18:50:41.000000 lastversion-2.4.8/lastversion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2022-12-05 18:50:41.000000 lastversion-2.4.8/lastversion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-05 18:50:41.000000 lastversion-2.4.8/lastversion.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      866 2022-12-05 18:50:41.000000 lastversion-2.4.8/lastversion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-12-05 18:50:41.000000 lastversion-2.4.8/lastversion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      154 2022-12-05 18:50:41.364140 lastversion-2.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2455 2022-12-05 18:50:32.000000 lastversion-2.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-23 05:53:28.001784 lastversion-2.4.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-01-23 05:53:16.000000 lastversion-2.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-01-23 05:53:16.000000 lastversion-2.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    25409 2023-01-23 05:53:28.001784 lastversion-2.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    19820 2023-01-23 05:53:16.000000 lastversion-2.4.9/README-ZH-CN.md
+-rw-r--r--   0 runner    (1001) docker     (122)    24802 2023-01-23 05:53:16.000000 lastversion-2.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-23 05:53:27.997784 lastversion-2.4.9/lastversion/
+-rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/BitBucketRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3093 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/FeedRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27857 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/GitHubRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/GitLabRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13905 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/GiteaRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/HelmChartRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4118 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/HolderFactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)      945 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/LocalVersionSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1981 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/MercurialRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12196 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/ProjectHolder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3107 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/PypiRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/SourceForgeRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3916 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/SystemRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6549 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/Version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3708 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/WikipediaRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3125 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/WordPressPluginRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/argparse_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28269 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/lastversion.py
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/spdx_id_to_rpmspec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6342 2023-01-23 05:53:16.000000 lastversion-2.4.9/lastversion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-23 05:53:28.001784 lastversion-2.4.9/lastversion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    25409 2023-01-23 05:53:27.000000 lastversion-2.4.9/lastversion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-01-23 05:53:27.000000 lastversion-2.4.9/lastversion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-23 05:53:27.000000 lastversion-2.4.9/lastversion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-01-23 05:53:27.000000 lastversion-2.4.9/lastversion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-23 05:53:27.000000 lastversion-2.4.9/lastversion.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-01-23 05:53:27.000000 lastversion-2.4.9/lastversion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-23 05:53:27.000000 lastversion-2.4.9/lastversion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-01-23 05:53:28.001784 lastversion-2.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2455 2023-01-23 05:53:16.000000 lastversion-2.4.9/setup.py
```

### Comparing `lastversion-2.4.8/LICENSE` & `lastversion-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lastversion-2.4.8/PKG-INFO` & `lastversion-2.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastversion
-Version: 2.4.8
+Version: 2.4.9
 Summary: A CLI tool to find the latest stable version of an arbitrary project
 Home-page: https://github.com/dvershinin/lastversion
 Author: Danila Vershinin
 Author-email: info@getpagespeed.com
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -137,31 +137,31 @@
 will use repository search API (slower).
 Helps to answer what is the latest Linux version:
 
 ```bash
 lastversion linux
 ```
 
-Or wondering what is the latest version of WordPress? :
+Or wondering what is the latest version of WordPress? 
 
 ```bash
 lastversion wordpress
 ```
    
-A special value of `self` for the main argument, will lookup the last release of `lastversion` 
+A special value of `self` for the main argument, will look up the last release of `lastversion` 
 itself.
 
 For more options to control output or behavior, see `--help` output:    
 
 ```text
 usage: lastversion [-h] [--pre] [--sem {major,minor,patch,any}] [-v]
                    [-d [FILENAME]] [--format {version,assets,source,json,tag}]
                    [--assets] [--source] [-gt VER] [-b MAJOR] [--only REGEX]
                    [--exclude REGEX] [--filter REGEX] [--having-asset [ASSET]]
-                   [-su]
+                   [-su] [--even]
                    [--at {github,gitlab,bitbucket,pip,hg,sf,website-feed,local,helm_chart,wiki,system,wp,gitea}]
                    [-y] [--version]
                    [{get,download,extract,unzip,test,format,install,update-spec}]
                    <repo URL or string>
 
 Find the latest software release.
 
@@ -191,25 +191,26 @@
   -b MAJOR, --major MAJOR, --branch MAJOR
                         Only consider releases of a specific major version,
                         e.g. 2.1.x
   --only REGEX          Only consider releases containing this text. Useful
                         for repos with multiple projects inside
   --exclude REGEX       Only consider releases NOT containing this text.
                         Useful for repos with multiple projects inside
+  --even                Only even versions like 1.[2].x, or 3.[6].x are
+                        considered as stable                        
   --filter REGEX        Filters --assets result by a regular expression
   --having-asset [ASSET]
                         Only consider releases with this asset
   -su, --shorter-urls   A tiny bit shorter URLs produced
   --at {github,gitlab,bitbucket,pip,hg,sf,website-feed,local,helm_chart,wiki,system,wp,gitea}
                         If the repo argument is one word, specifies where to
                         look up the project. The default is via internal
                         lookup or GitHub Search
   -y, --assumeyes       Automatically answer yes for all questions
   --version             show program's version number and exit
-
 ```
 
 The `--format` will affect what kind of information from the last release and in which format will
  be displayed, e.g.:
 
 *   `version` is the default. Simply outputs well-formatted version number of the latest release
 
@@ -294,15 +295,15 @@
     
 Customize downloaded filename (works only for sources, which is the default):
 
 ```bash
 lastversion download mautic/mautic -o mautic.tar.gz
 ```
 
-You can also directly fetch and extract latest release's file into the current working directory 
+You can also directly fetch and extract the latest release's file into the current working directory 
 by using `extract` command:
 
 ```bash
 lastversion extract wordpress
 ```
     
 You can have `lastversion` output sources/assets URLs and have those downloaded by 
@@ -348,15 +349,15 @@
 #> 2.15.2b0
 ```
     
 ### Use case: version of a specific branch
 
 For some projects, there may be several stable releases available simultaneously, in different
 branches. An obvious example is PHP. You can use `--major` flag to specify the major release
-version to match with, to help you find latest stable release of a branch, like so:
+version to match with, to help you find the latest stable release of a branch, like so:
 
 ```bash
 lastversion php/php-src --major 7.2
 ``` 
 
 This will give you current stable version of PHP 7.2.x, e.g. `7.2.28`.
 
@@ -400,15 +401,15 @@
 
 ### Use case: version of an operating system
 
 The operating systems are usually *not* versioned through GitHub releases or such.
 It is a challenge to get the last stable version of an OS other than from its website,
 or other announcement channels.
 
-An easy compromise that `lastversion` does about this, is hardcoding well-known OS names, and using
+An easy compromise that `lastversion` does about this, is hard coding well-known OS names, and using
 Wikipedia behind the scenes:
 
 ```bash 
 lastversion rocky #> 8.4
 lastversion windows #> 10.0.19043.1081
 lastversion ios #> 14.6
 ```
@@ -598,18 +599,18 @@
 Exit status code `2` is returned for `-gt` version comparison negative lookup.
 
 Exit status code `3` is returned when filtering assets of last release yields empty URL set 
 (no match)
 
 ## Tips
 
-Getting latest version is heavy on the API, because GitHub does not allow to fetch tags in 
+Getting the latest version is heavy on the API, because GitHub does not allow to fetch tags in 
 chronological order, and some repositories switch from one version format to another, so *we can't 
-just consider highest version to be latest*.
-We have to fetch every tag's commit date, and see if it's actually more recent. Thus it's slower
+just consider the highest version to be latest*.
+We have to fetch every tag's commit date, and see if it's actually more recent. Thus, it's slower
 with larger repositories, which have potentially a lot of tags.
 
 Thus, `lastversion` makes use of caching API response to be fast and light on GitHub API,
 It does conditional ETag validation, which, as per GitHub API will not count towards rate limit.
 The cache is stored in `~/.cache/lastversion` on Linux systems.
 
 It is *much recommended* to set up your [GitHub API token](https://github.com/settings/tokens).
@@ -684,15 +685,15 @@
     print('It is newer')
 ```
 
 With `output_format='version'` (the default), the function returns a 
 [Version](https://packaging.pypa.io/en/latest/version.html#packaging.version.Version) object, or
  `None`. So you can do things like above, namely version comparison, checking dev status, etc.
  
-With `output_format='dict'`, a dictionary returned with latest release information, or `False`.
+With `output_format='dict'`, a dictionary returned with the latest release information, or `False`.
 The dictionary keys vary between different project locations (GitHub vs BitBucket, for example),
 but are guaranteed to always have these keys:
 
 *   `version`: [Version](https://packaging.pypa.io/en/latest/version.html#packaging.version.Version) 
  object, contains the found release version, e.g. `1.2.3`
 *   `source`: string, the identifier of the project source, e.g. `github`, or `gitlab`
 *   `tag_date`: datetime object, the release date, e.g. `2020-12-15 14:41:39`
```

### Comparing `lastversion-2.4.8/README-ZH-CN.md` & `lastversion-2.4.9/README-ZH-CN.md`

 * *Files identical despite different names*

### Comparing `lastversion-2.4.8/README.md` & `lastversion-2.4.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -118,31 +118,31 @@
 will use repository search API (slower).
 Helps to answer what is the latest Linux version:
 
 ```bash
 lastversion linux
 ```
 
-Or wondering what is the latest version of WordPress? :
+Or wondering what is the latest version of WordPress? 
 
 ```bash
 lastversion wordpress
 ```
    
-A special value of `self` for the main argument, will lookup the last release of `lastversion` 
+A special value of `self` for the main argument, will look up the last release of `lastversion` 
 itself.
 
 For more options to control output or behavior, see `--help` output:    
 
 ```text
 usage: lastversion [-h] [--pre] [--sem {major,minor,patch,any}] [-v]
                    [-d [FILENAME]] [--format {version,assets,source,json,tag}]
                    [--assets] [--source] [-gt VER] [-b MAJOR] [--only REGEX]
                    [--exclude REGEX] [--filter REGEX] [--having-asset [ASSET]]
-                   [-su]
+                   [-su] [--even]
                    [--at {github,gitlab,bitbucket,pip,hg,sf,website-feed,local,helm_chart,wiki,system,wp,gitea}]
                    [-y] [--version]
                    [{get,download,extract,unzip,test,format,install,update-spec}]
                    <repo URL or string>
 
 Find the latest software release.
 
@@ -172,25 +172,26 @@
   -b MAJOR, --major MAJOR, --branch MAJOR
                         Only consider releases of a specific major version,
                         e.g. 2.1.x
   --only REGEX          Only consider releases containing this text. Useful
                         for repos with multiple projects inside
   --exclude REGEX       Only consider releases NOT containing this text.
                         Useful for repos with multiple projects inside
+  --even                Only even versions like 1.[2].x, or 3.[6].x are
+                        considered as stable                        
   --filter REGEX        Filters --assets result by a regular expression
   --having-asset [ASSET]
                         Only consider releases with this asset
   -su, --shorter-urls   A tiny bit shorter URLs produced
   --at {github,gitlab,bitbucket,pip,hg,sf,website-feed,local,helm_chart,wiki,system,wp,gitea}
                         If the repo argument is one word, specifies where to
                         look up the project. The default is via internal
                         lookup or GitHub Search
   -y, --assumeyes       Automatically answer yes for all questions
   --version             show program's version number and exit
-
 ```
 
 The `--format` will affect what kind of information from the last release and in which format will
  be displayed, e.g.:
 
 *   `version` is the default. Simply outputs well-formatted version number of the latest release
 
@@ -275,15 +276,15 @@
     
 Customize downloaded filename (works only for sources, which is the default):
 
 ```bash
 lastversion download mautic/mautic -o mautic.tar.gz
 ```
 
-You can also directly fetch and extract latest release's file into the current working directory 
+You can also directly fetch and extract the latest release's file into the current working directory 
 by using `extract` command:
 
 ```bash
 lastversion extract wordpress
 ```
     
 You can have `lastversion` output sources/assets URLs and have those downloaded by 
@@ -329,15 +330,15 @@
 #> 2.15.2b0
 ```
     
 ### Use case: version of a specific branch
 
 For some projects, there may be several stable releases available simultaneously, in different
 branches. An obvious example is PHP. You can use `--major` flag to specify the major release
-version to match with, to help you find latest stable release of a branch, like so:
+version to match with, to help you find the latest stable release of a branch, like so:
 
 ```bash
 lastversion php/php-src --major 7.2
 ``` 
 
 This will give you current stable version of PHP 7.2.x, e.g. `7.2.28`.
 
@@ -381,15 +382,15 @@
 
 ### Use case: version of an operating system
 
 The operating systems are usually *not* versioned through GitHub releases or such.
 It is a challenge to get the last stable version of an OS other than from its website,
 or other announcement channels.
 
-An easy compromise that `lastversion` does about this, is hardcoding well-known OS names, and using
+An easy compromise that `lastversion` does about this, is hard coding well-known OS names, and using
 Wikipedia behind the scenes:
 
 ```bash 
 lastversion rocky #> 8.4
 lastversion windows #> 10.0.19043.1081
 lastversion ios #> 14.6
 ```
@@ -579,18 +580,18 @@
 Exit status code `2` is returned for `-gt` version comparison negative lookup.
 
 Exit status code `3` is returned when filtering assets of last release yields empty URL set 
 (no match)
 
 ## Tips
 
-Getting latest version is heavy on the API, because GitHub does not allow to fetch tags in 
+Getting the latest version is heavy on the API, because GitHub does not allow to fetch tags in 
 chronological order, and some repositories switch from one version format to another, so *we can't 
-just consider highest version to be latest*.
-We have to fetch every tag's commit date, and see if it's actually more recent. Thus it's slower
+just consider the highest version to be latest*.
+We have to fetch every tag's commit date, and see if it's actually more recent. Thus, it's slower
 with larger repositories, which have potentially a lot of tags.
 
 Thus, `lastversion` makes use of caching API response to be fast and light on GitHub API,
 It does conditional ETag validation, which, as per GitHub API will not count towards rate limit.
 The cache is stored in `~/.cache/lastversion` on Linux systems.
 
 It is *much recommended* to set up your [GitHub API token](https://github.com/settings/tokens).
@@ -665,15 +666,15 @@
     print('It is newer')
 ```
 
 With `output_format='version'` (the default), the function returns a 
 [Version](https://packaging.pypa.io/en/latest/version.html#packaging.version.Version) object, or
  `None`. So you can do things like above, namely version comparison, checking dev status, etc.
  
-With `output_format='dict'`, a dictionary returned with latest release information, or `False`.
+With `output_format='dict'`, a dictionary returned with the latest release information, or `False`.
 The dictionary keys vary between different project locations (GitHub vs BitBucket, for example),
 but are guaranteed to always have these keys:
 
 *   `version`: [Version](https://packaging.pypa.io/en/latest/version.html#packaging.version.Version) 
  object, contains the found release version, e.g. `1.2.3`
 *   `source`: string, the identifier of the project source, e.g. `github`, or `gitlab`
 *   `tag_date`: datetime object, the release date, e.g. `2020-12-15 14:41:39`
```

### Comparing `lastversion-2.4.8/lastversion/BitBucketRepoSession.py` & `lastversion-2.4.9/lastversion/BitBucketRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-2.4.8/lastversion/FeedRepoSession.py` & `lastversion-2.4.9/lastversion/FeedRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-2.4.8/lastversion/GitHubRepoSession.py` & `lastversion-2.4.9/lastversion/GitHubRepoSession.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,16 @@
             }
         )
         if r.status_code == 404:
             # when not found, skip using this holder in the factory by not setting self.repo
             return None
         if r.status_code != 200:
             raise BadProjectError(
-                'Error while identifying full repository on GitHub for search query: {}'.format(
-                    repo
+                'Error while identifying full repository on GitHub for search query: {}. Status: {}'.format(
+                    repo, r.status_code
                 )
             )
         data = r.json()
         full_name = ''
         if data['items']:
             full_name = data['items'][0]['full_name']
         cache[repo] = {
@@ -145,15 +145,17 @@
     def __init__(self, repo, hostname):
         super(GitHubRepoSession, self).__init__()
         # dict holding repo/owner to feed contents of releases atom
         self.feed_contents = {}
         # lazy loaded dict cache of /releases response keyed by tag, only first page
         self.formal_releases_by_tag = None
         self.rate_limited_count = 0
-        self.api_token = os.getenv("GITHUB_API_TOKEN")
+        self.api_token = os.getenv("LASTVERSION_GITHUB_API_TOKEN")
+        if not self.api_token:
+            self.api_token = os.getenv("GITHUB_API_TOKEN")
         if not self.api_token:
             self.api_token = os.getenv("GITHUB_TOKEN")
         self.hostname = hostname
         if not self.hostname:
             self.hostname = self.DEFAULT_HOSTNAME
         # Explicitly specify the API version that we want:
         self.headers.update({
@@ -179,15 +181,15 @@
                     return
         self.set_repo(repo)
 
     def get_rate_limit_url(self):
         return '{}/rate_limit'.format(self.api_base)
 
     def get(self, url, **kwargs):
-        """Send GET reqiest and account for GitHub rate limits and such."""
+        """Send GET request and account for GitHub rate limits and such."""
         r = super(GitHubRepoSession, self).get(url, **kwargs)
         log.info('Got HTTP status code {} from {}'.format(r.status_code, url))
         if r.status_code == 401:
             if self.api_token:
                 raise ApiCredentialsError('API request was denied despite using an API token. '
                                           'Missing scopes?')
             raise ApiCredentialsError('Denied API access. Please set GITHUB_API_TOKEN env var '
@@ -504,15 +506,15 @@
         if not feed.entries:
             log.info('Feed has no elements. Means no tags and no releases')
             return []
         return feed.entries
 
     def get_latest(self, pre_ok=False, major=None):
         """
-        Get the latest release satisfying "prereleases are OK" or major/branch constraints
+        Get the latest release satisfying "pre-releases are OK" or major/branch constraints
         Strives to fetch formal API release if it exists, because it has useful information
         like assets.
         """
         # data of selected tag, always contains ['version', 'tag_name', 'tag_date', 'type'] will
         # be returned
         ret = None
 
@@ -541,15 +543,15 @@
                 if ret and tag_date + timedelta(days=365) < ret['tag_date']:
                     log.info('The version {} is newer, but is too old!'.format(version))
                     break
                 # we always want to return formal release if it exists, because it has useful data
                 # grab formal release via APi to check for pre-release mark
                 formal_release = self.get_formal_release_for_tag(tag_name)
                 if formal_release:
-                    # use full release info
+                    # use the full release info
                     ret = self.set_matching_formal_release(ret, formal_release, version, pre_ok)
                 else:
                     if self.having_asset:
                         continue
                     log.info('No formal release for tag {}'.format(tag_name))
                     tag['tag_name'] = tag_name
                     tag['tag_date'] = tag_date
```

### Comparing `lastversion-2.4.8/lastversion/GitLabRepoSession.py` & `lastversion-2.4.9/lastversion/GitLabRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-2.4.8/lastversion/GiteaRepoSession.py` & `lastversion-2.4.9/lastversion/GiteaRepoSession.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     """ The following format will benefit from:
     1) not using API, so is not subject to its rate limits
     2) likely has been accessed by someone in CDN and thus faster
     3) provides more or less unique filenames once the stuff is downloaded
     See https://fedoraproject.org/wiki/Packaging:SourceURL#Git_Tags
     We use variation of this: it does not need a parsed version (thus works for --pre better)
     and it is not broken on fancy release tags like v1.2.3-stable
-    https://github.com/OWNER/PROJECT/archive/%{gittag}/%{gittag}-%{version}.tar.gz
+    https://github.com/OWNER/PROJECT/archive/%{git_tag}/%{git_tag}-%{version}.tar.gz
     """
     RELEASE_URL_FORMAT = "https://{hostname}/{repo}/archive/{tag}.{ext}"
     SHORT_RELEASE_URL_FORMAT = RELEASE_URL_FORMAT
 
     def find_repo_by_name_only(self, repo):
         if repo.startswith(('https://', 'http://')):
             return None
@@ -147,15 +147,15 @@
                     return
         self.set_repo(repo)
 
     def get_rate_limit_url(self):
         return '{}/rate_limit'.format(self.api_base)
 
     def get(self, url, **kwargs):
-        """Send GET reqiest and account for GitHub rate limits and such."""
+        """Send GET request and account for GitHub rate limits and such."""
         r = super(GiteaRepoSession, self).get(url, **kwargs)
         log.info('Got HTTP status code {} from {}'.format(r.status_code, url))
         if r.status_code == 401:
             if self.api_token:
                 raise ApiCredentialsError('API request was denied despite using an API token. '
                                           'Missing scopes?')
             raise ApiCredentialsError('Denied API access. Please set GITHUB_API_TOKEN env var '
@@ -230,15 +230,16 @@
             # noinspection SpellCheckingInspection
             return r.json()
         return None
 
     # finding in tags requires paging through ALL of them, because the API does not list them
     # in order of recency, thus this is very slow
     # in: current release to be returned, output: newer release to be returned
-    def find_in_tags(self, ret, pre_ok, major):
+    def find_in_tags(self, pre_ok, major):
+        ret = None
         r = self.repo_query('/tags?per_page=100')
         if r.status_code != 200:
             return None
         tags = r.json()
         while 'next' in r.links.keys():
             r = self.get(r.links['next']['url'])
             tags.extend(r.json())
@@ -263,31 +264,28 @@
                     ret['tag_date'] = d
                     ret['version'] = version
                     ret['type'] = 'tag'
         return ret
 
     def get_latest(self, pre_ok=False, major=None):
         """
-        Gets the latest release satisfying "prereleases are OK" or major/branch constraints
+        Gets the latest release satisfying "pre-releases are OK" or major/branch constraints
         Strives to fetch formal API release if it exists, because it has useful information
         like assets.
         """
-        # data of selected tag, always contains ['version', 'tag_name', 'tag_date', 'type'] will
-        # be returned
-        ret = None
 
         if self.having_asset:
             # only formal releases which we enumerated above already, have assets
             # so there is no point looking in the tags/graphql below
             # return whatever we got
-            return ret
+            return None
 
         # formal release may not exist at all, or be "late/old" in case
         # actual release is only a simple tag so let's try /tags
-        ret = self.find_in_tags(ret, pre_ok, major)
+        ret = self.find_in_tags(pre_ok, major)
 
         return ret
 
     def set_matching_formal_release(self, ret, formal_release, version, pre_ok,
                                     data_type='release'):
         """Set current release selection to this formal release if matching conditions."""
         if not pre_ok and formal_release['prerelease']:
```

### Comparing `lastversion-2.4.8/lastversion/HelmChartRepoSession.py` & `lastversion-2.4.9/lastversion/HelmChartRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-2.4.8/lastversion/HolderFactory.py` & `lastversion-2.4.9/lastversion/HolderFactory.py`

 * *Files identical despite different names*

### Comparing `lastversion-2.4.8/lastversion/LocalVersionSession.py` & `lastversion-2.4.9/lastversion/LocalVersionSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-2.4.8/lastversion/MercurialRepoSession.py` & `lastversion-2.4.9/lastversion/MercurialRepoSession.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def __init__(self, repo, hostname):
         super(MercurialRepoSession, self).__init__()
         self.hostname = hostname
         self.set_repo(repo)
 
     def get_latest(self, pre_ok=False, major=None):
         ret = None
-        # to leverage cachecontrol, we fetch the feed using requests as usual
+        # to leverage cachecontrol, we fetch the feed using requests as usual,
         # then feed the feed to feedparser as a raw string
         # e.g. https://hg.nginx.org/nginx/atom-tags
         # https://pythonhosted.org/feedparser/common-atom-elements.html
         r = self.get('https://{}/{}/atom-tags'.format(self.hostname, self.repo))
         feed = feedparser.parse(r.text)
         for tag in feed.entries:
             tag_name = tag['title']
```

### Comparing `lastversion-2.4.8/lastversion/ProjectHolder.py` & `lastversion-2.4.9/lastversion/ProjectHolder.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 class ProjectHolder(requests.Session):
     """Generic project holder class abstracts a web-accessible project storage."""
 
     # List of odd repos where last char is part of version not beta level
     LAST_CHAR_FIX_REQUIRED_ON = []
 
     # web accessible project holders may have single well-known domain usable by everyone
-    # in case of GitHub, that is github.com, for Mercurial web gui - here isn't one, etc.
+    # in case of GitHub, that is GitHub.com, for Mercurial web gui - here isn't one, etc.
     DEFAULT_HOSTNAME = None
     SUBDOMAIN_INDICATOR = None
     KNOWN_REPO_URLS = {}
     KNOWN_REPOS_BY_NAME = {}
     # e.g. owner/project, but mercurial just /project together with hostname
     # adapter array should list how many elements make up "repo", e.g. for hg.nginx.com/repo it
     # is only one instead of 2
     # or a "format" specifier for matching
     REPO_URL_PROJECT_COMPONENTS = 2
-    # if URI starts with project name, 0. Otherwise skip through this many URI dirs
+    # if URI starts with project name, 0. Otherwise, skip through this many URI dirs
     REPO_URL_PROJECT_OFFSET = 0
     RELEASE_URL_FORMAT = None
     SHORT_RELEASE_URL_FORMAT = None
 
     def set_repo(self, repo):
         """Set repo ID property of project holder instance."""
         self.repo = repo
@@ -72,14 +72,15 @@
         self.hostname = None
         # identifies project on a given hostname
         self.repo = None
         # short name for "repo", useful in URLs
         self.name = None
         # in some case we do not specify repo, but feed is discovered, no repo is given then
         self.feed_url = None
+        self.even = False
 
     def is_valid(self):
         """Check if project holder is valid instance."""
         return self.feed_url or self.name
 
     def set_branches(self, branches):
         """Sets project holder's branches."""
@@ -95,14 +96,21 @@
     def set_exclude(self, exclude):
         """Sets "exclude" tag selector for this holder."""
         self.exclude = exclude
         if exclude:
             log.info('Only considering tags without "{}"'.format(exclude))
         return self
 
+    def set_even(self, even):
+        """Set to return only releases with even numbering like 1.2.3."""
+        self.even = even
+        if even:
+            log.info('Only considering releases with even numbering')
+        return self
+
     def set_having_asset(self, having_asset):
         """Sets "having_asset" selector for this holder."""
         self.having_asset = having_asset
         if having_asset:
             log.info('Only considering releases with asset "{}"'.format(having_asset))
         return self
 
@@ -223,14 +231,16 @@
                     except InvalidVersion:
                         log.info('Still not a valid version after applying underscores fix')
         # apply --major filter
         if res and major and not self.matches_major_filter(res, major):
             log.info('{} is not under the desired major {}'.format(
                 version_s, major))
             res = False
+        if res and self.even and not res.even:
+            return False
         return res
 
     def _type(self):
         """Get project holder's class name."""
         return self.__class__.__name__
 
     def release_download_url(self, release, shorter=False):
```

### Comparing `lastversion-2.4.8/lastversion/PypiRepoSession.py` & `lastversion-2.4.9/lastversion/PypiRepoSession.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         """Get release download URL."""
         for f in release['files']:
             if f['packagetype'] == 'sdist':
                 return f['url']
         return None
 
     def get_latest(self, pre_ok=False, major=None):
-        """Get latest project release."""
+        """Get the latest project release."""
         ret = self.project
         # we are in "enriching" project dict with desired version information
         # and return None if there's no matching version
         from .Version import Version
         if self.project is None:
             print("Project is not listed on PyPI")
             return None
```

### Comparing `lastversion-2.4.8/lastversion/SourceForgeRepoSession.py` & `lastversion-2.4.9/lastversion/SourceForgeRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-2.4.8/lastversion/SystemRepoSession.py` & `lastversion-2.4.9/lastversion/SystemRepoSession.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             # A query matches all packages in sack
             q = base.sack.query()
             # https://dnf.readthedocs.io/en/latest/use_cases.html#id3
             # https: // dnf.readthedocs.io / en / latest / api_queries.html  # dnf.query.Query
             # Derived query matches only available packages
             a = q.available()
             a = a.filter(name=self.repo)
-            for pkg in a:  # a only gets evaluated here
+            for pkg in a:  # `a` only gets evaluated here
                 version = self.sanitize_version(pkg.version, pre_ok, major)
                 if not ret or ret['version'] < version:
                     ret = {
                         'version': version,
                         'tag_name': pkg.evr,
                         'tag_date': datetime.datetime.fromtimestamp(pkg.buildtime)
                     }
```

### Comparing `lastversion-2.4.8/lastversion/Version.py` & `lastversion-2.4.9/lastversion/Version.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class Version(PackagingVersion):
     """
     This class abstracts handling of a project's versions. It implements the
     scheme defined in PEP 440. A `Version` instance is comparison
     aware and can be compared and sorted using the standard Python interfaces.
 
-    This class is descendant from Version found in packaging.version,
+    This class is descendant from Version found in `packaging.version`,
     and implements some additional, "AI"-like normalization during instantiation.
 
     Args:
         version (str): The string representation of a version which will be
                       parsed and normalized before use.
     Raises:
         InvalidVersion: If the ``version`` does not conform to PEP 440 in
@@ -21,15 +21,20 @@
     """
 
     def fix_letter_post_release(self, match):
         self.fixed_letter_post_release = True
         return match.group(1) + '.post' + str(ord(match.group(2)))
 
     def __init__(self, version, char_fix_required=False):
-        # type: (str) -> None
+        """Instantiate the `Version` object.
+
+        Args:
+            version (str): The version-like string
+            char_fix_required (bool): Should we treat alphanumerics as part of version
+        """
         self.fixed_letter_post_release = False
 
         # 4.27-chaos-preview-3 -> 4.27-chaos-pre3
         version = re.sub('-preview-(\\d+)', '-pre\\1', version, 1)
         # 5.0.0-early-access-2 -> 5.0.0-alpha2
         version = re.sub('-early-access-(\\d+)', '-alpha\\1', version, 1)
 
@@ -55,25 +60,25 @@
             if not part.isalpha():
                 parts_n.append(part)
 
         if not parts_n:
             raise InvalidVersion("Invalid version: '{0}'".format(version))
         # remove *any* non-digits which appear at the beginning of the version string
         # e.g. Rhino1_7_13_Release does not even bother to put a delimiter...
-        # such string at the beginning typically do not convey stability level
+        # such string at the beginning typically do not convey stability level,
         # so we are fine to remove them (unlike the ones in the tail)
         parts_n[0] = re.sub('^[^0-9]+', '', parts_n[0], 1)
 
         # go back to full string parse out
         version = ".".join(parts_n)
 
         if char_fix_required:
             version = re.sub('(\\d)([a-z])$', self.fix_letter_post_release, version, 1)
         # release-3_0_2 is often seen on Mercurial holders
-        # note that above code removes "release-" already so we are left with "3_0_2"
+        # note that above code removes "release-" already, so we are left with "3_0_2"
         if re.search(r'^(?:\d+_)+(?:\d+)', version):
             version = version.replace('_', '.')
         # finally, split by dot "delimiter", see if there are common words which are definitely
         # removable
         parts = version.split('.')
         version = []
         for p in parts:
@@ -118,14 +123,25 @@
 
     @property
     def local(self):
         if self._version.local:
             return ".".join(str(x) for x in self._version.local)
         return None
 
+    @property
+    def is_prerelease(self):
+        # type: () -> bool
+        if self.micro and self.micro >= 90:
+            return True
+        return self.dev is not None or self.pre is not None
+
+    @property
+    def even(self):
+        return self.minor and not self.minor % 2
+
     def sem_extract_base(self, level=None):
         """
         Return Version with desired semantic version level base
         E.g. for 5.9.3 it will return 5.9 (patch is None)
         """
         if level == 'major':
             # get major
```

### Comparing `lastversion-2.4.8/lastversion/WikipediaRepoSession.py` & `lastversion-2.4.9/lastversion/WikipediaRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-2.4.8/lastversion/WordPressPluginRepoSession.py` & `lastversion-2.4.9/lastversion/WordPressPluginRepoSession.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     def release_download_url(self, release, shorter=False):
         """Get release download URL."""
         return 'https://downloads.wordpress.org/plugin/{}.{}.zip'.format(
             self.repo, release['version'])
 
     def get_latest(self, pre_ok=False, major=None):
-        """Get latest release for this project."""
+        """Get the latest release for this project."""
         ret = {}
         # we are in "enriching" project dict with desired version information
         # and return None if there's no matching version
         from .Version import Version
         if not major:
             latest_ver = self.project['version']
             v = Version(latest_ver)
```

### Comparing `lastversion-2.4.8/lastversion/__init__.py` & `lastversion-2.4.9/lastversion/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 __author__ = "Danila Vershinin"
 
 import logging
 
 from .__about__ import (
     __version__,
 )
-# We intentially import for export here, so it is ok to silence DeepSource test
+# We intentionally import for export here, so it is ok to silence DeepSource test
 # skipcq: PY-W2000
 from .lastversion import __self__
 # skipcq: PY-W2000
 from .lastversion import check_version
 # skipcq: PY-W2000
 from .lastversion import has_update
 # skipcq: PY-W2000
```

### Comparing `lastversion-2.4.8/lastversion/argparse_version.py` & `lastversion-2.4.9/lastversion/argparse_version.py`

 * *Files identical despite different names*

### Comparing `lastversion-2.4.8/lastversion/lastversion.py` & `lastversion-2.4.9/lastversion/lastversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     BadProjectError
 
 log = logging.getLogger(__name__)
 
 
 def latest(repo, output_format='version', pre_ok=False, assets_filter=None,
            short_urls=False, major=None, only=None, at=None,
-           having_asset=None, exclude=None):
+           having_asset=None, exclude=None, even=False):
     """Find the latest release version for a project.
 
     Args:
         major (str): Only consider versions which are "descendants" of this major version string
         short_urls (bool): Whether we should try to return shorter URLs for release data
         assets_filter (str): Regular expression for filtering assets for the latest release
         only (str): Only consider tags with this text. Useful for repos with multiple projects.
@@ -53,14 +53,15 @@
                              `assets`, `source`, `tag`.
         pre_ok (bool): Specifies whether pre-releases can be accepted as newer version.
         at (str): Specifies repo hosting more precisely, only useful if repo argument was
                   specified as one word.
         having_asset (Union[str, bool]): Only consider releases with the given asset.
                                          Pass `True` for any asset
         exclude (str): Only consider releases NOT containing this text/regular expression.
+        even (bool): Consider as stable only releases with even minor component, e.g. 1.2.3
 
     Examples:
         Find the latest version of Mautic, it is OK to consider betas.
 
         >>> latest("mautic/mautic", output_format='version', pre_ok=True)
         <Version('4.4.4')>
 
@@ -90,42 +91,42 @@
                 repo_data['name'] = name
 
     if repo.startswith(('http://', 'https://')) and repo.endswith('Chart.yaml'):
         at = 'helm_chart'
 
     if repo.endswith('.spec'):
         # repo is specified inside the .spec file
-        # github repo is resolved via %{upstream_github} + %{name}/%{upstream_name}
+        # GitHub repo is resolved via %{upstream_github} + %{name}/%{upstream_name}
         # no upstream_github global means that the spec was not prepared for lastversion
         # optional: use of spec_tag macros if the source is from GitHub. in edge cases we check
         # new version via GitHub, but prepared sources are elsewhere
         with open(repo) as f:
             name = None
             upstream_github = None
             upstream_name = None
             current_version = None
             spec_repo = None
             spec_url = None
-            for l in f.readlines():
-                if l.startswith('%global lastversion_repo'):
-                    spec_repo = l.split(' ')[2].strip()
-                elif l.startswith('%global upstream_github'):
-                    upstream_github = l.split(' ')[2].strip()
-                elif l.startswith('%global upstream_name'):
-                    upstream_name = l.split(' ')[2].strip()
-                elif l.startswith('Name:'):
-                    name = l.split('Name:')[1].strip()
-                elif l.startswith('URL:'):
-                    spec_url = l.split('URL:')[1].strip()
-                elif l.startswith('%global upstream_version '):
-                    current_version = l.split(' ')[2].strip()
+            for line in f.readlines():
+                if line.startswith('%global lastversion_repo'):
+                    spec_repo = line.split(' ')[2].strip()
+                elif line.startswith('%global upstream_github'):
+                    upstream_github = line.split(' ')[2].strip()
+                elif line.startswith('%global upstream_name'):
+                    upstream_name = line.split(' ')[2].strip()
+                elif line.startswith('Name:'):
+                    name = line.split('Name:')[1].strip()
+                elif line.startswith('URL:'):
+                    spec_url = line.split('URL:')[1].strip()
+                elif line.startswith('%global upstream_version '):
+                    current_version = line.split(' ')[2].strip()
                     # influences %spec_tag to use %upstream_version instead of %version
                     repo_data['module_of'] = True
-                elif l.startswith('Version:') and not current_version:
-                    current_version = l.split('Version:')[1].strip()
+                elif line.startswith('Version:') and not current_version:
+                    current_version = line.split('Version:')[1].strip()
             if spec_url:
                 spec_host = urlparse(spec_url).hostname
                 if spec_host in ['github.com'] and not upstream_github and not spec_repo:
                     log.warning('Neither %upstream_github nor %lastversion_repo macros were found. '
                                 'Please prepare your spec file using instructions: '
                                 'https://lastversion.getpagespeed.com/spec-preparing.html')
             if not current_version:
@@ -153,14 +154,15 @@
             elif spec_url:
                 repo = spec_url
 
     with HolderFactory.get_instance_for_repo(repo, at=at) as project:
         project.set_only(only)
         project.set_exclude(exclude)
         project.set_having_asset(having_asset)
+        project.set_even(even)
         release = project.get_latest(pre_ok=pre_ok, major=major)
 
         # bail out, found nothing that looks like a release
         if not release:
             return None
 
         from_type = 'Located the latest release tag {} at: {}'.format(
@@ -385,15 +387,15 @@
                              '-vv to increase verbosity level')
     # no --download = False, --download filename.tar, --download = None
     parser.add_argument('-d', '-o', '--download', '--output', dest='download', nargs='?', default=False, const=None,
                         metavar='FILENAME', help='Download with custom filename')
     # how / which data of last release we want to present
     # assets will give download urls for assets if available and sources archive otherwise
     # sources will give download urls for sources always
-    # json always includes "version", "tag_name" etc + whichever json data was
+    # json always includes "version", "tag_name" etc. + whichever json data was
     # used to satisfy lastversion
     parser.add_argument('--format',
                         choices=['version', 'assets', 'source', 'json', 'tag'],
                         help='Output format')
     parser.add_argument('--assets', dest='assets', action='store_true',
                         help='Returns assets download URLs for last release')
     parser.add_argument('--source', dest='source', action='store_true',
@@ -412,25 +414,27 @@
     parser.add_argument('--filter', metavar='REGEX', help="Filters --assets result by a regular "
                                                           "expression")
     parser.add_argument('--having-asset', metavar='ASSET',
                         help="Only consider releases with this asset",
                         nargs='?', const=True)
     parser.add_argument('-su', '--shorter-urls', dest='shorter_urls', action='store_true',
                         help='A tiny bit shorter URLs produced')
+    parser.add_argument('--even', dest='even', action='store_true',
+                        help='Only even versions like 1.[2].x, or 3.[6].x are considered as stable')
     parser.add_argument('--at', dest='at',
                         help='If the repo argument is one word, specifies where to look up the '
                              'project. The default is via internal lookup or GitHub Search',
                         choices=HolderFactory.HOLDERS.keys())
     parser.add_argument('-y', '--assumeyes', dest='assumeyes', action='store_true',
                         help='Automatically answer yes for all questions')
     parser.add_argument('--version', action=VersionAction)
     parser.set_defaults(validate=True, verbose=False, format='version',
                         pre=False, assets=False, newer_than=False, filter=False,
                         shorter_urls=False, major=None, assumeyes=False, at=None,
-                        having_asset=None)
+                        having_asset=None, even=False)
     args = parser.parse_args()
 
     if args.repo == "self":
         args.repo = __self__
 
     # "expand" repo:1.2 as repo --branch 1.2
     if ':' in args.repo and \
@@ -526,15 +530,15 @@
             print(max([args.newer_than, base_compare]))
             sys.exit(2 if base_compare <= args.newer_than else 0)
      
     # other action are either getting release or doing something with release (extend get action)
     try:
         res = latest(args.repo, args.format, args.pre, args.filter,
                      args.shorter_urls, args.major, args.only, args.at,
-                     having_asset=args.having_asset, exclude=args.exclude)
+                     having_asset=args.having_asset, exclude=args.exclude, even=args.even)
     except (ApiCredentialsError, BadProjectError) as error:
         log.critical(str(error))
         if isinstance(error, ApiCredentialsError) and "GITHUB_API_TOKEN" not in os.environ and \
                 "GITHUB_TOKEN" not in os.environ:
             log.critical(TOKEN_PRO_TIP)
         sys.exit(4)
```

### Comparing `lastversion-2.4.8/lastversion/spdx_id_to_rpmspec.py` & `lastversion-2.4.9/lastversion/spdx_id_to_rpmspec.py`

 * *Files identical despite different names*

### Comparing `lastversion-2.4.8/lastversion/utils.py` & `lastversion-2.4.9/lastversion/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,32 +71,33 @@
                     return True
     if sys.platform.startswith('linux'):
         # Weeding out non-matching Linux distros
         for ext, ext_distros in extension_distros.items():
             if asset.endswith("." + ext) and distro.id() not in ext_distros:
                 return True
     # weed out non-64 bit stuff from x86_64 bit OS
-    # caution: may be false positive with 32 bit Python on 64 bit OS
+    # caution: may be false positive with 32 bit Python on 64-bit OS
     if platform.machine() in ['x86_64', 'AMD64']:
         for non_amd64_word in non_amd64_markers:
             r = re.compile(r'\b{}\b'.format(non_amd64_word), flags=re.IGNORECASE)
             if r.search(asset):
                 return True
             r = re.compile(r'\barm\d+\b', flags=re.IGNORECASE)
             if r.search(asset):
                 return True
     return False
 
 
-# monkey patching older requests library's response class so it can use context manager
+# monkey patching older requests library's response class, so it can use context manager
 # https://github.com/psf/requests/issues/4136
 def requests_response_patched_enter(self):
     return self
 
 
+# noinspection PyUnusedLocal
 def requests_response_patched_exit(self, *args):
     self.close()
 
 
 if not hasattr(requests.Response, '__exit__'):
     requests.Response.__enter__ = requests_response_patched_enter
     requests.Response.__exit__ = requests_response_patched_exit
```

### Comparing `lastversion-2.4.8/lastversion.egg-info/PKG-INFO` & `lastversion-2.4.9/lastversion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastversion
-Version: 2.4.8
+Version: 2.4.9
 Summary: A CLI tool to find the latest stable version of an arbitrary project
 Home-page: https://github.com/dvershinin/lastversion
 Author: Danila Vershinin
 Author-email: info@getpagespeed.com
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -137,31 +137,31 @@
 will use repository search API (slower).
 Helps to answer what is the latest Linux version:
 
 ```bash
 lastversion linux
 ```
 
-Or wondering what is the latest version of WordPress? :
+Or wondering what is the latest version of WordPress? 
 
 ```bash
 lastversion wordpress
 ```
    
-A special value of `self` for the main argument, will lookup the last release of `lastversion` 
+A special value of `self` for the main argument, will look up the last release of `lastversion` 
 itself.
 
 For more options to control output or behavior, see `--help` output:    
 
 ```text
 usage: lastversion [-h] [--pre] [--sem {major,minor,patch,any}] [-v]
                    [-d [FILENAME]] [--format {version,assets,source,json,tag}]
                    [--assets] [--source] [-gt VER] [-b MAJOR] [--only REGEX]
                    [--exclude REGEX] [--filter REGEX] [--having-asset [ASSET]]
-                   [-su]
+                   [-su] [--even]
                    [--at {github,gitlab,bitbucket,pip,hg,sf,website-feed,local,helm_chart,wiki,system,wp,gitea}]
                    [-y] [--version]
                    [{get,download,extract,unzip,test,format,install,update-spec}]
                    <repo URL or string>
 
 Find the latest software release.
 
@@ -191,25 +191,26 @@
   -b MAJOR, --major MAJOR, --branch MAJOR
                         Only consider releases of a specific major version,
                         e.g. 2.1.x
   --only REGEX          Only consider releases containing this text. Useful
                         for repos with multiple projects inside
   --exclude REGEX       Only consider releases NOT containing this text.
                         Useful for repos with multiple projects inside
+  --even                Only even versions like 1.[2].x, or 3.[6].x are
+                        considered as stable                        
   --filter REGEX        Filters --assets result by a regular expression
   --having-asset [ASSET]
                         Only consider releases with this asset
   -su, --shorter-urls   A tiny bit shorter URLs produced
   --at {github,gitlab,bitbucket,pip,hg,sf,website-feed,local,helm_chart,wiki,system,wp,gitea}
                         If the repo argument is one word, specifies where to
                         look up the project. The default is via internal
                         lookup or GitHub Search
   -y, --assumeyes       Automatically answer yes for all questions
   --version             show program's version number and exit
-
 ```
 
 The `--format` will affect what kind of information from the last release and in which format will
  be displayed, e.g.:
 
 *   `version` is the default. Simply outputs well-formatted version number of the latest release
 
@@ -294,15 +295,15 @@
     
 Customize downloaded filename (works only for sources, which is the default):
 
 ```bash
 lastversion download mautic/mautic -o mautic.tar.gz
 ```
 
-You can also directly fetch and extract latest release's file into the current working directory 
+You can also directly fetch and extract the latest release's file into the current working directory 
 by using `extract` command:
 
 ```bash
 lastversion extract wordpress
 ```
     
 You can have `lastversion` output sources/assets URLs and have those downloaded by 
@@ -348,15 +349,15 @@
 #> 2.15.2b0
 ```
     
 ### Use case: version of a specific branch
 
 For some projects, there may be several stable releases available simultaneously, in different
 branches. An obvious example is PHP. You can use `--major` flag to specify the major release
-version to match with, to help you find latest stable release of a branch, like so:
+version to match with, to help you find the latest stable release of a branch, like so:
 
 ```bash
 lastversion php/php-src --major 7.2
 ``` 
 
 This will give you current stable version of PHP 7.2.x, e.g. `7.2.28`.
 
@@ -400,15 +401,15 @@
 
 ### Use case: version of an operating system
 
 The operating systems are usually *not* versioned through GitHub releases or such.
 It is a challenge to get the last stable version of an OS other than from its website,
 or other announcement channels.
 
-An easy compromise that `lastversion` does about this, is hardcoding well-known OS names, and using
+An easy compromise that `lastversion` does about this, is hard coding well-known OS names, and using
 Wikipedia behind the scenes:
 
 ```bash 
 lastversion rocky #> 8.4
 lastversion windows #> 10.0.19043.1081
 lastversion ios #> 14.6
 ```
@@ -598,18 +599,18 @@
 Exit status code `2` is returned for `-gt` version comparison negative lookup.
 
 Exit status code `3` is returned when filtering assets of last release yields empty URL set 
 (no match)
 
 ## Tips
 
-Getting latest version is heavy on the API, because GitHub does not allow to fetch tags in 
+Getting the latest version is heavy on the API, because GitHub does not allow to fetch tags in 
 chronological order, and some repositories switch from one version format to another, so *we can't 
-just consider highest version to be latest*.
-We have to fetch every tag's commit date, and see if it's actually more recent. Thus it's slower
+just consider the highest version to be latest*.
+We have to fetch every tag's commit date, and see if it's actually more recent. Thus, it's slower
 with larger repositories, which have potentially a lot of tags.
 
 Thus, `lastversion` makes use of caching API response to be fast and light on GitHub API,
 It does conditional ETag validation, which, as per GitHub API will not count towards rate limit.
 The cache is stored in `~/.cache/lastversion` on Linux systems.
 
 It is *much recommended* to set up your [GitHub API token](https://github.com/settings/tokens).
@@ -684,15 +685,15 @@
     print('It is newer')
 ```
 
 With `output_format='version'` (the default), the function returns a 
 [Version](https://packaging.pypa.io/en/latest/version.html#packaging.version.Version) object, or
  `None`. So you can do things like above, namely version comparison, checking dev status, etc.
  
-With `output_format='dict'`, a dictionary returned with latest release information, or `False`.
+With `output_format='dict'`, a dictionary returned with the latest release information, or `False`.
 The dictionary keys vary between different project locations (GitHub vs BitBucket, for example),
 but are guaranteed to always have these keys:
 
 *   `version`: [Version](https://packaging.pypa.io/en/latest/version.html#packaging.version.Version) 
  object, contains the found release version, e.g. `1.2.3`
 *   `source`: string, the identifier of the project source, e.g. `github`, or `gitlab`
 *   `tag_date`: datetime object, the release date, e.g. `2020-12-15 14:41:39`
```

### Comparing `lastversion-2.4.8/lastversion.egg-info/SOURCES.txt` & `lastversion-2.4.9/lastversion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lastversion-2.4.8/lastversion.egg-info/requires.txt` & `lastversion-2.4.9/lastversion.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lastversion-2.4.8/setup.py` & `lastversion-2.4.9/setup.py`

 * *Files identical despite different names*

