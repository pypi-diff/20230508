# Comparing `tmp/pcs-get-0.9.8.tar.gz` & `tmp/pcs-get-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcs-get-0.9.8.tar", last modified: Sat Apr 30 15:15:58 2022, max compression
+gzip compressed data, was "pcs-get-0.9.9.tar", last modified: Wed May  4 14:51:04 2022, max compression
```

## Comparing `pcs-get-0.9.8.tar` & `pcs-get-0.9.9.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 garen      (501) staff       (20)        0 2022-04-30 15:15:58.590628 pcs-get-0.9.8/
--rw-r--r--   0 garen      (501) staff       (20)    35083 2022-04-29 16:03:20.000000 pcs-get-0.9.8/LICENSE
--rw-r--r--   0 garen      (501) staff       (20)     3824 2022-04-30 15:15:58.590521 pcs-get-0.9.8/PKG-INFO
--rw-r--r--   0 garen      (501) staff       (20)     3170 2022-04-30 15:15:42.000000 pcs-get-0.9.8/README.md
-drwxr-xr-x   0 garen      (501) staff       (20)        0 2022-04-30 15:15:58.589581 pcs-get-0.9.8/pcs_get.egg-info/
--rw-r--r--   0 garen      (501) staff       (20)     3824 2022-04-30 15:15:58.000000 pcs-get-0.9.8/pcs_get.egg-info/PKG-INFO
--rw-r--r--   0 garen      (501) staff       (20)      372 2022-04-30 15:15:58.000000 pcs-get-0.9.8/pcs_get.egg-info/SOURCES.txt
--rw-r--r--   0 garen      (501) staff       (20)        1 2022-04-30 15:15:58.000000 pcs-get-0.9.8/pcs_get.egg-info/dependency_links.txt
--rw-r--r--   0 garen      (501) staff       (20)       51 2022-04-30 15:15:58.000000 pcs-get-0.9.8/pcs_get.egg-info/entry_points.txt
--rw-r--r--   0 garen      (501) staff       (20)       14 2022-04-30 15:15:58.000000 pcs-get-0.9.8/pcs_get.egg-info/requires.txt
--rw-r--r--   0 garen      (501) staff       (20)        7 2022-04-30 15:15:58.000000 pcs-get-0.9.8/pcs_get.egg-info/top_level.txt
-drwxr-xr-x   0 garen      (501) staff       (20)        0 2022-04-30 15:15:58.589770 pcs-get-0.9.8/pcsget/
--rw-r--r--   0 garen      (501) staff       (20)       60 2022-04-30 15:15:42.000000 pcs-get-0.9.8/pcsget/__init__.py
-drwxr-xr-x   0 garen      (501) staff       (20)        0 2022-04-30 15:15:58.590376 pcs-get-0.9.8/pcsget/biz/
--rw-r--r--   0 garen      (501) staff       (20)        0 2022-04-30 06:54:23.000000 pcs-get-0.9.8/pcsget/biz/__init__.py
--rw-r--r--   0 garen      (501) staff       (20)     2374 2022-04-30 07:14:55.000000 pcs-get-0.9.8/pcsget/biz/config.py
--rw-r--r--   0 garen      (501) staff       (20)      994 2022-04-30 14:38:26.000000 pcs-get-0.9.8/pcsget/biz/log.py
--rw-r--r--   0 garen      (501) staff       (20)     2827 2022-04-30 06:58:11.000000 pcs-get-0.9.8/pcsget/biz/login.py
--rw-r--r--   0 garen      (501) staff       (20)     7991 2022-04-30 14:56:04.000000 pcs-get-0.9.8/pcsget/biz/sync.py
--rw-r--r--   0 garen      (501) staff       (20)     3559 2022-04-30 14:28:49.000000 pcs-get-0.9.8/pcsget/biz/utils.py
--rw-r--r--   0 garen      (501) staff       (20)     2577 2022-04-30 15:11:10.000000 pcs-get-0.9.8/pcsget/cmdline.py
--rw-r--r--   0 garen      (501) staff       (20)       38 2022-04-30 15:15:58.590663 pcs-get-0.9.8/setup.cfg
--rw-r--r--   0 garen      (501) staff       (20)     1116 2022-04-30 14:56:04.000000 pcs-get-0.9.8/setup.py
+drwxr-xr-x   0 garen      (501) staff       (20)        0 2022-05-04 14:51:04.149898 pcs-get-0.9.9/
+-rw-r--r--   0 garen      (501) staff       (20)    35083 2022-04-29 16:03:20.000000 pcs-get-0.9.9/LICENSE
+-rw-r--r--   0 garen      (501) staff       (20)     3824 2022-05-04 14:51:04.149772 pcs-get-0.9.9/PKG-INFO
+-rw-r--r--   0 garen      (501) staff       (20)     3170 2022-04-30 15:29:07.000000 pcs-get-0.9.9/README.md
+drwxr-xr-x   0 garen      (501) staff       (20)        0 2022-05-04 14:51:04.147203 pcs-get-0.9.9/pcs_get.egg-info/
+-rw-r--r--   0 garen      (501) staff       (20)     3824 2022-05-04 14:51:03.000000 pcs-get-0.9.9/pcs_get.egg-info/PKG-INFO
+-rw-r--r--   0 garen      (501) staff       (20)      450 2022-05-04 14:51:04.000000 pcs-get-0.9.9/pcs_get.egg-info/SOURCES.txt
+-rw-r--r--   0 garen      (501) staff       (20)        1 2022-05-04 14:51:03.000000 pcs-get-0.9.9/pcs_get.egg-info/dependency_links.txt
+-rw-r--r--   0 garen      (501) staff       (20)       51 2022-05-04 14:51:04.000000 pcs-get-0.9.9/pcs_get.egg-info/entry_points.txt
+-rw-r--r--   0 garen      (501) staff       (20)       14 2022-05-04 14:51:04.000000 pcs-get-0.9.9/pcs_get.egg-info/requires.txt
+-rw-r--r--   0 garen      (501) staff       (20)        7 2022-05-04 14:51:04.000000 pcs-get-0.9.9/pcs_get.egg-info/top_level.txt
+drwxr-xr-x   0 garen      (501) staff       (20)        0 2022-05-04 14:51:04.148165 pcs-get-0.9.9/pcsget/
+-rw-r--r--   0 garen      (501) staff       (20)       61 2022-05-04 14:49:15.000000 pcs-get-0.9.9/pcsget/__init__.py
+drwxr-xr-x   0 garen      (501) staff       (20)        0 2022-05-04 14:51:04.149582 pcs-get-0.9.9/pcsget/biz/
+-rw-r--r--   0 garen      (501) staff       (20)        0 2022-04-30 15:28:15.000000 pcs-get-0.9.9/pcsget/biz/__init__.py
+-rw-r--r--   0 garen      (501) staff       (20)     2356 2022-05-04 14:49:15.000000 pcs-get-0.9.9/pcsget/biz/config.py
+-rw-r--r--   0 garen      (501) staff       (20)      994 2022-04-30 15:28:15.000000 pcs-get-0.9.9/pcsget/biz/log.py
+-rw-r--r--   0 garen      (501) staff       (20)     2827 2022-04-30 15:28:15.000000 pcs-get-0.9.9/pcsget/biz/login.py
+-rw-r--r--   0 garen      (501) staff       (20)     7991 2022-04-30 15:28:15.000000 pcs-get-0.9.9/pcsget/biz/sync.py
+-rw-r--r--   0 garen      (501) staff       (20)     3559 2022-04-30 15:28:15.000000 pcs-get-0.9.9/pcsget/biz/utils.py
+-rw-r--r--   0 garen      (501) staff       (20)     2577 2022-04-30 15:28:59.000000 pcs-get-0.9.9/pcsget/cmdline.py
+-rw-r--r--   0 garen      (501) staff       (20)     2356 2022-05-04 14:49:15.000000 pcs-get-0.9.9/pcsget/config.py
+-rw-r--r--   0 garen      (501) staff       (20)     1031 2022-04-30 15:28:15.000000 pcs-get-0.9.9/pcsget/log.py
+-rw-r--r--   0 garen      (501) staff       (20)     2877 2022-04-30 15:28:15.000000 pcs-get-0.9.9/pcsget/login.py
+-rw-r--r--   0 garen      (501) staff       (20)     8312 2022-04-30 15:28:15.000000 pcs-get-0.9.9/pcsget/sync.py
+-rw-r--r--   0 garen      (501) staff       (20)     3365 2022-04-30 15:28:15.000000 pcs-get-0.9.9/pcsget/utils.py
+-rw-r--r--   0 garen      (501) staff       (20)       38 2022-05-04 14:51:04.149939 pcs-get-0.9.9/setup.cfg
+-rw-r--r--   0 garen      (501) staff       (20)     1116 2022-04-30 15:29:18.000000 pcs-get-0.9.9/setup.py
```

### Comparing `pcs-get-0.9.8/LICENSE` & `pcs-get-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pcs-get-0.9.8/PKG-INFO` & `pcs-get-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcs-get
-Version: 0.9.8
+Version: 0.9.9
 Summary: the spider for pcs-protocol
 Home-page: https://git.sysop.bigo.sg/zhoujianwei.garen/pcs-get
 Author: zhoujianwei.garen
 Author-email: zhoujianwei.garen@bigo.com
 License: GPLv3+
 Keywords: pcs,bigo,spider
 Platform: all
@@ -33,15 +33,14 @@
          --set-user,         - 可选项，用户名（oa账号），用于cookie过期时的自动登录
          --set-password,     - 可选项，密码，用于cookie过期时的自动登录
          --set-lang,         - 协议文件格式，可选：java(默认), kotlin, kotlin-marshallize(TODO)，swift(TODO), oc(TODO)
          -h, --help,         - 帮助
          -v, --version,      - 查看版本
 ```
 
-
 ## 安装
 
 ```commandline
 pip install pcs-get
 ```
 
 ## 配置
@@ -57,14 +56,15 @@
 
 当然也可配置浏览器中已有的cookie，但是过期之后需要再次手动更新
 
 ```commandline
 pcs-get --set-token your_csrftoken
 pcs-get --set-session your_sessionid
 ```
+
 浏览器获取现有cookie看这里
 ![get-token-session](https://raw.githubusercontent.com/BladesOfTime/pure-img-holder/main/pcs-get/get-token-session.png)
 
 ## 使用
 
 建议建新包存放协议类文件，比如需求包是livepass，新建protocol目录作为协议包，先cd到此路径再执行本脚本
```

### Comparing `pcs-get-0.9.8/README.md` & `pcs-get-0.9.9/README.md`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
          --set-user,         - 可选项，用户名（oa账号），用于cookie过期时的自动登录
          --set-password,     - 可选项，密码，用于cookie过期时的自动登录
          --set-lang,         - 协议文件格式，可选：java(默认), kotlin, kotlin-marshallize(TODO)，swift(TODO), oc(TODO)
          -h, --help,         - 帮助
          -v, --version,      - 查看版本
 ```
 
-
 ## 安装
 
 ```commandline
 pip install pcs-get
 ```
 
 ## 配置
@@ -38,14 +37,15 @@
 
 当然也可配置浏览器中已有的cookie，但是过期之后需要再次手动更新
 
 ```commandline
 pcs-get --set-token your_csrftoken
 pcs-get --set-session your_sessionid
 ```
+
 浏览器获取现有cookie看这里
 ![get-token-session](https://raw.githubusercontent.com/BladesOfTime/pure-img-holder/main/pcs-get/get-token-session.png)
 
 ## 使用
 
 建议建新包存放协议类文件，比如需求包是livepass，新建protocol目录作为协议包，先cd到此路径再执行本脚本
```

### Comparing `pcs-get-0.9.8/pcs_get.egg-info/PKG-INFO` & `pcs-get-0.9.9/pcs_get.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcs-get
-Version: 0.9.8
+Version: 0.9.9
 Summary: the spider for pcs-protocol
 Home-page: https://git.sysop.bigo.sg/zhoujianwei.garen/pcs-get
 Author: zhoujianwei.garen
 Author-email: zhoujianwei.garen@bigo.com
 License: GPLv3+
 Keywords: pcs,bigo,spider
 Platform: all
@@ -33,15 +33,14 @@
          --set-user,         - 可选项，用户名（oa账号），用于cookie过期时的自动登录
          --set-password,     - 可选项，密码，用于cookie过期时的自动登录
          --set-lang,         - 协议文件格式，可选：java(默认), kotlin, kotlin-marshallize(TODO)，swift(TODO), oc(TODO)
          -h, --help,         - 帮助
          -v, --version,      - 查看版本
 ```
 
-
 ## 安装
 
 ```commandline
 pip install pcs-get
 ```
 
 ## 配置
@@ -57,14 +56,15 @@
 
 当然也可配置浏览器中已有的cookie，但是过期之后需要再次手动更新
 
 ```commandline
 pcs-get --set-token your_csrftoken
 pcs-get --set-session your_sessionid
 ```
+
 浏览器获取现有cookie看这里
 ![get-token-session](https://raw.githubusercontent.com/BladesOfTime/pure-img-holder/main/pcs-get/get-token-session.png)
 
 ## 使用
 
 建议建新包存放协议类文件，比如需求包是livepass，新建protocol目录作为协议包，先cd到此路径再执行本脚本
```

### Comparing `pcs-get-0.9.8/pcsget/biz/config.py` & `pcs-get-0.9.9/pcsget/biz/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         curr_cfg_json[K_TOKEN] = kw[K_TOKEN]
         actual_updated = True
     if K_DEBUG in kw:
         curr_cfg_json[K_DEBUG] = kw[K_DEBUG]
         actual_updated = True
 
     if actual_updated:
-        n_cfg_json = json.dumps(curr_cfg_json, encoding='utf-8')
+        n_cfg_json = json.dumps(curr_cfg_json)
         with open(_get_config_file_path(), 'w') as fp:
             fp.write(n_cfg_json)
             i("config for %s was updated!" % str(kw.keys()))
     else:
         e("none config was updated!")
```

### Comparing `pcs-get-0.9.8/pcsget/biz/log.py` & `pcs-get-0.9.9/pcsget/biz/log.py`

 * *Files identical despite different names*

### Comparing `pcs-get-0.9.8/pcsget/biz/login.py` & `pcs-get-0.9.9/pcsget/biz/login.py`

 * *Files identical despite different names*

### Comparing `pcs-get-0.9.8/pcsget/biz/sync.py` & `pcs-get-0.9.9/pcsget/biz/sync.py`

 * *Files identical despite different names*

### Comparing `pcs-get-0.9.8/pcsget/biz/utils.py` & `pcs-get-0.9.9/pcsget/biz/utils.py`

 * *Files identical despite different names*

### Comparing `pcs-get-0.9.8/pcsget/cmdline.py` & `pcs-get-0.9.9/pcsget/cmdline.py`

 * *Files identical despite different names*

### Comparing `pcs-get-0.9.8/setup.py` & `pcs-get-0.9.9/setup.py`

 * *Files identical despite different names*

