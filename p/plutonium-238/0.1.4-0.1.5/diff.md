# Comparing `tmp/plutonium-238-0.1.4.tar.gz` & `tmp/plutonium-238-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutonium-238-0.1.4.tar", last modified: Thu Mar  2 07:11:23 2023, max compression
+gzip compressed data, was "plutonium-238-0.1.5.tar", last modified: Mon May  8 16:08:38 2023, max compression
```

## Comparing `plutonium-238-0.1.4.tar` & `plutonium-238-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-03-02 07:11:23.940514 plutonium-238-0.1.4/
--rw-r--r--   0 john       (501) staff       (20)      868 2023-03-02 07:11:23.940315 plutonium-238-0.1.4/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)       34 2023-03-02 03:59:40.000000 plutonium-238-0.1.4/README.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-03-02 07:11:23.936335 plutonium-238-0.1.4/plutonium/
--rw-r--r--   0 john       (501) staff       (20)        0 2023-01-17 14:47:08.000000 plutonium-238-0.1.4/plutonium/__init__.py
--rw-r--r--   0 john       (501) staff       (20)     9246 2023-03-02 04:01:58.000000 plutonium-238-0.1.4/plutonium/cli.py
--rw-r--r--   0 john       (501) staff       (20)     2870 2023-03-02 07:11:12.000000 plutonium-238-0.1.4/plutonium/config.py
--rw-r--r--   0 john       (501) staff       (20)    11840 2023-02-28 07:34:30.000000 plutonium-238-0.1.4/plutonium/utils.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-03-02 07:11:23.939412 plutonium-238-0.1.4/plutonium_238.egg-info/
--rw-r--r--   0 john       (501) staff       (20)      868 2023-03-02 07:11:23.000000 plutonium-238-0.1.4/plutonium_238.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      320 2023-03-02 07:11:23.000000 plutonium-238-0.1.4/plutonium_238.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2023-03-02 07:11:23.000000 plutonium-238-0.1.4/plutonium_238.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)       50 2023-03-02 07:11:23.000000 plutonium-238-0.1.4/plutonium_238.egg-info/entry_points.txt
--rw-r--r--   0 john       (501) staff       (20)        9 2023-03-02 07:11:23.000000 plutonium-238-0.1.4/plutonium_238.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)       10 2023-03-02 07:11:23.000000 plutonium-238-0.1.4/plutonium_238.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)       38 2023-03-02 07:11:23.940787 plutonium-238-0.1.4/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)     1205 2023-03-02 07:10:37.000000 plutonium-238-0.1.4/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-08 16:08:38.105626 plutonium-238-0.1.5/
+-rw-r--r--   0 john       (501) staff       (20)      868 2023-05-08 16:08:38.105420 plutonium-238-0.1.5/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)       34 2023-03-02 03:59:40.000000 plutonium-238-0.1.5/README.md
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-08 16:08:38.101536 plutonium-238-0.1.5/plutonium/
+-rw-r--r--   0 john       (501) staff       (20)        0 2023-01-17 14:47:08.000000 plutonium-238-0.1.5/plutonium/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)    10433 2023-05-08 16:07:57.000000 plutonium-238-0.1.5/plutonium/cli.py
+-rw-r--r--   0 john       (501) staff       (20)     4391 2023-05-08 15:48:01.000000 plutonium-238-0.1.5/plutonium/config.py
+-rw-r--r--   0 john       (501) staff       (20)    12000 2023-05-08 15:59:36.000000 plutonium-238-0.1.5/plutonium/utils.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-08 16:08:38.104886 plutonium-238-0.1.5/plutonium_238.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)      868 2023-05-08 16:08:38.000000 plutonium-238-0.1.5/plutonium_238.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      320 2023-05-08 16:08:38.000000 plutonium-238-0.1.5/plutonium_238.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2023-05-08 16:08:38.000000 plutonium-238-0.1.5/plutonium_238.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)       50 2023-05-08 16:08:38.000000 plutonium-238-0.1.5/plutonium_238.egg-info/entry_points.txt
+-rw-r--r--   0 john       (501) staff       (20)        9 2023-05-08 16:08:38.000000 plutonium-238-0.1.5/plutonium_238.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)       10 2023-05-08 16:08:38.000000 plutonium-238-0.1.5/plutonium_238.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)       38 2023-05-08 16:08:38.105676 plutonium-238-0.1.5/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)     1205 2023-05-08 16:08:29.000000 plutonium-238-0.1.5/setup.py
```

### Comparing `plutonium-238-0.1.4/PKG-INFO` & `plutonium-238-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutonium-238
-Version: 0.1.4
+Version: 0.1.5
 Summary: SCA Agent, Copyright@Plutonium
 Home-page: https://www.google.com
 Author: tom
 Author-email: tom@google.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `plutonium-238-0.1.4/plutonium/cli.py` & `plutonium-238-0.1.5/plutonium/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,45 @@
+import json
 import os
 import argparse
 from plutonium.utils import logger, VoyagerDetect
 from plutonium.config import (
-    BOM_FILENAME,
-    LOG_FILENAME,
     VOYAGER_SERVER,
     VOYAGER_USERNAME,
     VOYAGER_PASSWORD,
     VOYAGER_TOKEN,
     GOVERNANCE_TOKEN,
+    LOG_FILENAME,
     LOGO
 )
 
-def init_data(data_dir):
-    if not os.path.exists(data_dir):
-        try:
-            os.makedirs(data_dir)
-        except Exception as e:
-            logger.error(e)
-
 def init_parse():
-
     parser = argparse.ArgumentParser(
         description="SCA Agent based on Cdxgen and internal project Voyager I, for application dependencies and risk discovery。"
     )
     parser.add_argument(
         "-t",
         "--type",
         dest="type",
         required=True,
         help="project/image/package/project_file/image_file/package_file",
     )
     parser.add_argument(
-        "--data-dir",
-        default=os.path.join(os.getcwd(), "data"),
-        dest="data_dir",
-        help="Running data directory",
-    )
-    parser.add_argument(
         "-l",
         "--language",
         dest="language",
         default=None,
         help="project language",
     )
     parser.add_argument(
         "--target",
         dest="target",
         help="Source directory or container image or binary file",
     )
+    # sca分析参数
     parser.add_argument(
         "--no-error",
         action="store_true",
         default=False,
         dest="noerror",
         help="Continue on error to prevent build from breaking",
     )
@@ -67,14 +54,33 @@
         "--deep",
         action="store_true",
         default=False,
         dest="deep_scan",
         help="Perform deep scan by passing this --deep argument to cdxgen. Useful while scanning docker images and OS packages.",
     )
     parser.add_argument(
+        "--package_cmd",
+        action="store_true",
+        default=False,
+        help="是否通过包命令解析软件",
+    )
+    parser.add_argument(
+        "--package_file",
+        action="store_true",
+        default=False,
+        help="是否获取包文件数据",
+    )
+    parser.add_argument(
+        "--docker_file",
+        action="store_true",
+        default=False,
+        help="是否获取dockerfile数据",
+    )
+    # 服务端参数
+    parser.add_argument(
         "--voyager-server",
         default=VOYAGER_SERVER,
         dest="voyager_server",
         help="Voyager server url. Eg: https://api.voyager.com",
     )
     parser.add_argument(
         "--voyager-username",
@@ -96,27 +102,27 @@
     )
     parser.add_argument(
         "--governance-token",
         default=GOVERNANCE_TOKEN,
         dest="governance_token",
         help="Governance token for token based submission",
     )
+    # 项目参数信息
     parser.add_argument(
         "--project_name",
         help="project name",
     )
     parser.add_argument(
         "--project_repository_url",
         help="project repository url",
     )
     parser.add_argument(
         "--project_user",
         help="project user",
     )
-    # project branch
     parser.add_argument(
         "--project_branch",
         help="project branch",
     )
     parser.add_argument(
         "--project_file",
         help="project file",
@@ -129,31 +135,15 @@
         "--project_service_name",
         help="project service name",
     )
     parser.add_argument(
         "--project_commit_id",
         help="project commit id",
     )
-
-    parser.add_argument(
-        "--depscan",
-        action="store_true",
-        default=False,
-        dest="depscan",
-        help="Try to scan vulnerabilities using depscan",
-    )
-    parser.add_argument(
-        "--trivy",
-        action="store_true",
-        default=False,
-        dest="trivy",
-        help="Try to scan vulnerabilities using trivy",
-    )
-
-    # 镜像信息
+    # 镜像参数信息
     parser.add_argument(
         "--image_name",
         help="镜像名称",
     )
     parser.add_argument(
         "--image_file",
         help="镜像文件",
@@ -182,25 +172,25 @@
     )
     parser.add_argument(
         "--deploy_pro_env",
         action="store_true",
         default=False,
         help="部署环境为正式环境",
     )
-
+    parser.add_argument(
+        "--extra_data",
+        help="附加参数a=b&c=d",
+    )
     parser.print_help()
     return parser.parse_args()
 
 
 def main():
     print(LOGO)
     args = init_parse()
-    init_data(args.data_dir)
-    target = args.target
-    # Detect the project types and perform the right type of scan
     data = {
         'op_type': 'create_project_governance',
         'type': args.type,
         'governance_token': args.governance_token if args.governance_token else GOVERNANCE_TOKEN,
         # 项目信息
         'language': args.language,
         # 镜像类
@@ -214,91 +204,113 @@
         'project_name': args.project_name,
         'project_branch': args.project_branch,
         'project_user': args.project_user,
         'project_commit_id': args.project_commit_id,
         'project_pod': args.project_pod,
         'project_service_name': args.project_service_name,
         'project_repository_url': args.project_repository_url,
-        # 包类，暂时不用
-
+        # 附加参数
+        'extra_data': args.extra_data,
     }
     attach_files = [
         # 提交的名称前缀需要与scan_log_detail的type一致
         # 项目文件
         # ('attach_file', ('2.md', open('./todo.md', 'rb'),)),
         # ('core_files_list', ('pom.xml', open('./todo.md', 'rb'), )),
         # ('core_files_list', ('package.json.lock', open('./todo.md', 'rb'), )),
         # ('sbom_files_list', ('sca_cdxgen.json', open('./voyager.json', 'rb'),)),
         # ('sbom_files_list', ('sca_dependency_tree.txt', open('./todo.md', 'rb'), )),
         # ('vul_files_list', ('vul_veinmind.json', open('./todo.md', 'rb'), )),
     ]
-    # if args.project_file:
-    #     try:
-    #         attach_files.append(
-    #             ('attach_file', (args.project_file.split('.')[0], open(args.project_file, 'rb'),)),
-    #         )
-    #     except Exception as e:
-    #         logger.error(e)
     detector = VoyagerDetect(
         token=args.voyager_token if args.voyager_token else VOYAGER_TOKEN,
         url=args.voyager_server if args.voyager_server else VOYAGER_SERVER,
         username=args.voyager_username if args.voyager_username else VOYAGER_USERNAME,
         password=args.voyager_password if args.voyager_password else VOYAGER_PASSWORD,
     )
+    # 项目安全检测
     if args.type in ['project', 'project_file']:
-        sca_status = detector.sca_analysis(args.language, args.data_dir+'/'+BOM_FILENAME, target, args.deep_scan)
-        if not sca_status:
-            logger.debug("Bom file {} was not created successfully")
-        try:
-            attach_files.append(
-                ('sbom_files_list', (BOM_FILENAME, open(args.data_dir+'/'+BOM_FILENAME, 'rb'),)),
-            )
-        except Exception as e:
-            logger.error(e)
-        # # 如果开启漏洞，执行漏洞扫描
-        if args.depscan:
-            logger.info('开始基于depscan进行漏洞扫描')
-        if args.trivy:
-            logger.info('开始基于trivy进行漏洞扫描')
-        # 上传数据到后端
-        print(data)
-        # run_log进行上传
-        # 将run.log进行复制
-        try:
-            attach_files.append(
-                ('core_files_list', (LOG_FILENAME, open(LOG_FILENAME, 'rb'),)),
-            )
-        except Exception as e:
-            logger.error(e)
-        scan_status = detector.scan(data, attach_files)
+        # 如果是项目文件
+        if args.project_file:
+            try:
+                attach_files.append(
+                    ('attach_file', (args.project_file.split('/')[-1].split('.')[0], open(args.project_file, 'rb'),)),
+                )
+            except Exception as e:
+                logger.error(e)
+        else:
+            # 需要在项目目录下进行sca分析，并进行结果上传
+            sca_data = detector.sca_analysis(language=args.language, src_dir=args.target,
+                                               sca_tool=True, package_cmd=args.package_cmd,
+                                               package_file=args.package_file,
+                                               docker_file=args.docker_file,
+                                               deep=args.deep_scan)
+            # 获取sca工具获取的sbom文件
+            for item in sca_data['sca_tool']:
+                try:
+                    attach_files.append(
+                        ('sbom_files_list', (item['result'].split('/')[-1], open(item['result'], 'rb'),)),
+                    )
+                except Exception as e:
+                    logger.error(e)
+            # 逐个遍历命令结果数据
+            # 将sbom数据放置到data里
+            if args.package_cmd:
+                try:
+                    data['package_cmd'] = json.dumps(sca_data['package_cmd'])
+                except Exception as e:
+                    logger.error(e)
+            if args.package_file:
+                for item in sca_data['package_file']:
+                    try:
+                        # 名称添加package_file前缀
+                        attach_files.append(
+                            (
+                            'sbom_files_list', ('package_file_'+item.split('/')[-1], open(item, 'rb'),)),
+                        )
+                    except Exception as e:
+                        logger.error(e)
+            if args.docker_file:
+                for item in sca_data['docker_file']:
+                    try:
+                        # 名称添加package_file前缀
+                        attach_files.append(
+                            (
+                            'sbom_files_list', ('docker_file_'+item.split('/')[-1], open(item, 'rb'),)),
+                        )
+                    except Exception as e:
+                        logger.error(e)
+            
+            # 封装运行记录、包文件、通过命令获取的包文件内容
+            try:
+                attach_files.append(
+                    ('core_files_list', (LOG_FILENAME.split('/')[-1], open(LOG_FILENAME, 'rb'),)),
+                )
+            except Exception as e:
+                logger.error(e)
+        scan_status = detector.base_scan(data, attach_files)
         print(scan_status)
+    # 镜像安全检测
     elif args.type in ['image', 'image_file']:
-        print(data)
         if args.image_file:
             try:
                 attach_files.append(
                     ('attach_file', (args.image_file.split('/')[-1].split('.')[0], open(args.image_file, 'rb'),)),
                 )
             except Exception as e:
                 logger.error(e)
-        print(data)
-        print(attach_files)
         # run_log进行上传
         try:
             attach_files.append(
                 ('core_files_list', (LOG_FILENAME, open(LOG_FILENAME, 'rb'),)),
             )
         except Exception as e:
             logger.error(e)
         scan_status = detector.scan(data, attach_files)
         print(scan_status)
+    # 软件包检测
     elif args.type in ['package','package_file']:
         pass
     else:
         pass
-    # if scan_status['success']:
-    #     print(scan_status['message'])
-    # else:
-    #     print(scan_status['message'])
-
 if __name__ == '__main__':
     main()
```

### Comparing `plutonium-238-0.1.4/plutonium/utils.py` & `plutonium-238-0.1.5/plutonium/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,81 @@
 import subprocess
 import logging
 import os
 import sys
 import shutil
 import requests
 import plutonium.config as config
-
-# log format
-formatter = logging.Formatter(config.LOG_FORMAT)
+from uuid import uuid4
 logger = logging.getLogger(__name__)
-
-# file logger
+formatter = logging.Formatter(config.LOG_FORMAT)
 file_handler = logging.FileHandler(config.LOG_FILENAME)
 file_handler.setFormatter(formatter)
-
-# console logger
 console_handler = logging.StreamHandler()
 console_handler.setFormatter(formatter)
-
-# init logger
 logger.addHandler(file_handler)
 logger.addHandler(console_handler)
 logger.setLevel(config.LOG_LEVEL)
-
+# 忽略目录
 def filter_ignored_dirs(dirs):
-    """
-    Method to filter directory list to remove ignored directories
-    :param dirs: Directories to ignore
-    :return: Filtered directory list
-    """
     [
         dirs.remove(d)
         for d in list(dirs)
         if d.lower() in config.ignore_directories or d.startswith(".")
     ]
     return dirs
-
+# 查找python依赖文件
 def find_python_reqfiles(path):
-    """
-    Method to find python requirements files
-
-    Args:
-      path Project dir
-    Returns:
-      List of python requirement files
-    """
     result = []
     req_files = [
         "requirements.txt",
         "Pipfile",
         "poetry.lock",
         "Pipfile.lock",
         "conda.yml",
     ]
     for root, dirs, files in os.walk(path):
         filter_ignored_dirs(dirs)
         for name in req_files:
             if name in files:
                 result.append(os.path.join(root, name))
     return result
-
+# 判断是否是二进制字符
 def is_binary_string(content):
-    """
-    Method to check if the given content is a binary string
-    """
     textchars = bytearray({7, 8, 9, 10, 12, 13, 27} | set(range(0x20, 0x100)) - {0x7F})
     return bool(content.translate(None, textchars))
-
+# 判断是否是二进制文件
 def is_exe(src):
-    """Detect if the source is a binary file
-    :param src: Source path
-    :return True if binary file. False otherwise.
-    """
     if os.path.isfile(src):
         try:
             return is_binary_string(open(src, "rb").read(1024))
         except Exception:
             return False
     return False
-
+# 查找指定后缀文件
 def find_files(src, src_ext_name, quick=False, filter=True):
-    """
-    Method to find files with given extenstion
-    """
     result = []
     for root, dirs, files in os.walk(src):
         if filter:
             filter_ignored_dirs(dirs)
         for file in files:
             if file == src_ext_name or file.endswith(src_ext_name):
                 result.append(os.path.join(root, file))
                 if quick:
                     return result
     return result
-
+# 获取路径
 def resource_path(relative_path):
     try:
         base_path = sys._MEIPASS
     except Exception:
         base_path = os.path.dirname(__file__)
     return os.path.join(base_path, relative_path)
-
+# 执行命令
 def exec_tool(args, cwd=None, stdout=subprocess.PIPE):
-    """
-    Convenience method to invoke cli tools
-
-    Args:
-      args cli command and args
-    """
     try:
         logger.debug('Executing "{}"'.format(" ".join(args)))
         if os.environ.get("FETCH_LICENSE"):
             logger.debug(
                 "License information would be fetched from the registry. This would take several minutes ..."
             )
         cp = subprocess.run(
@@ -121,103 +85,159 @@
             cwd=cwd,
             env=os.environ.copy(),
             check=False,
             shell=False,
             encoding="utf-8",
         )
         logger.debug(cp.stdout)
+        return cp.stdout
     except Exception as e:
         logger.exception(e)
-
-def detect_language_type(src_dir):
-    """Detect project type by looking for certain files
-
-    :param src_dir: Source directory
-
-    :return List of detected types
-    """
-    # container image support
-    if (
-        "docker.io" in src_dir
-        or "quay.io" in src_dir
-        or ":latest" in src_dir
-        or "@sha256" in src_dir
-        or src_dir.endswith(".tar")
-        or src_dir.endswith(".tar.gz")
-    ):
-        return ["docker"]
-    # Check if the source is an exe file. Assume go for all binaries for now
-    if is_exe(src_dir):
-        return ["go", "binary"]
-    project_types = []
+        return str(e)
+# 检测项目开发语言
+# go/python/java/nodejs
+def detect_project_language(src_dir):
     if find_python_reqfiles(src_dir):
-        project_types.append("python")
+        return "python"
     if find_files(src_dir, "pom.xml", quick=True) or find_files(
-        src_dir, ".gradle", quick=True
+            src_dir, ".gradle", quick=True
     ):
-        project_types.append("java")
-    if find_files(src_dir, ".gradle.kts", quick=True):
-        project_types.append("kotlin")
-    if find_files(src_dir, "build.sbt", quick=True):
-        project_types.append("scala")
+        return "java"
     if (
-        find_files(src_dir, "package.json", quick=True)
-        or find_files(src_dir, "yarn.lock", quick=True)
-        or find_files(src_dir, "rush.json", quick=True)
+            find_files(src_dir, "package.json", quick=True)
+            or find_files(src_dir, "yarn.lock", quick=True)
+            or find_files(src_dir, "rush.json", quick=True)
     ):
-        project_types.append("nodejs")
+        return "nodejs"
     if find_files(src_dir, "go.sum", quick=True) or find_files(
-        src_dir, "Gopkg.lock", quick=True
-    ):
-        project_types.append("go")
-    if find_files(src_dir, "Cargo.lock", quick=True):
-        project_types.append("rust")
-    if find_files(src_dir, "composer.json", quick=True):
-        project_types.append("php")
-    if find_files(src_dir, ".csproj", quick=True):
-        project_types.append("dotnet")
-    if find_files(src_dir, "Gemfile", quick=True) or find_files(
-        src_dir, "Gemfile.lock", quick=True
-    ):
-        project_types.append("ruby")
-    if find_files(src_dir, "deps.edn", quick=True) or find_files(
-        src_dir, "project.clj", quick=True
-    ):
-        project_types.append("clojure")
-    if find_files(src_dir, "conan.lock", quick=True) or find_files(
-        src_dir, "conanfile.txt", quick=True
-    ):
-        project_types.append("cpp")
-    if find_files(src_dir, "pubspec.lock", quick=True) or find_files(
-        src_dir, "pubspec.yaml", quick=True
-    ):
-        project_types.append("dart")
-    if find_files(src_dir, "cabal.project.freeze", quick=True):
-        project_types.append("haskell")
-    if find_files(src_dir, "mix.lock", quick=True):
-        project_types.append("elixir")
-    if find_files(
-        os.path.join(src_dir, ".github", "workflows"), ".yml", quick=True, filter=False
+            src_dir, "Gopkg.lock", quick=True
     ):
-        project_types.append("github")
-    # jars
-    if "java" not in project_types and find_files(src_dir, ".jar", quick=True):
-        project_types.append("jar")
-    # Jenkins plugins or plain old jars
-    if "java" not in project_types and find_files(src_dir, ".hpi", quick=True):
-        project_types.append("jenkins")
-    if find_files(src_dir, ".yml", quick=True) or find_files(
-        src_dir, ".yaml", quick=True
-    ):
-        project_types.append("yaml-manifest")
-    return project_types
+        return "go"
 
+    return "other"
 
-class VoyagerDetect():
+# 通过cdxgen来生成sbom
+def sca_by_cdxgen(language, bom_file, src_dir=".", deep=False):
+    result = {
+        'status': False,
+        'data': None,
+        'message': ''
+    }
+    cdxgen_cmd = os.environ.get("CDXGEN_CMD", "cdxgen")
+    if not shutil.which(cdxgen_cmd):
+        local_bin = resource_path(
+            os.path.join(
+                "local_bin", "cdxgen.exe" if sys.platform == "win32" else "cdxgen"
+            )
+        )
+        if not os.path.exists(local_bin):
+            result['message'] = 'command not found'
+            return result
+        try:
+            cdxgen_cmd = local_bin
+            # Set the plugins directory as an environment variable
+            os.environ["CDXGEN_PLUGINS_DIR"] = resource_path("local_bin")
+        except Exception as e:
+            result['message'] = e
+            return result
+    if language:
+        sca_args = [cdxgen_cmd, "-r", "-t", language, "-o", bom_file]
+    else:
+        sca_args = [cdxgen_cmd, "-o", bom_file]
+    if deep:
+        sca_args.append("--deep")
+    sca_args.append(src_dir)
+    print(sca_args)
+    exec_tool(sca_args, )
+    result['status'] = True
+    result['data'] = ' '.join(sca_args)
+    return result
+
+# 获取sca分析
+def get_sca_info(src_dir, language=None, sca_tool=True, package_cmd=True, package_file=True,docker_file=True, deep=False):
+    result = {
+        'language': '',
+        # 通过sca工具分析
+        'sca_tool': [],
+        # 通过命令读取的结果
+        'package_cmd': [],
+        # 通过包文件读取
+        'package_file': [],
+        'docker_file': [],
+    }
+    if not language:
+        language = detect_project_language(src_dir)
+    result['language'] = language
+
+    # 1.通过cdxgen来生成
+    cdxgen_sbom_file = config.SCA_TOOLS['cdxgen']['sbom_file'].format(uuid4().hex)
+    cdxgen_result = sca_by_cdxgen(language, cdxgen_sbom_file, src_dir)
+    cdxgen_item = {
+        'tool': 'cdxgen',
+        'cmd': cdxgen_result['data'],
+        'result': cdxgen_sbom_file if cdxgen_result['status'] else cdxgen_result['message']
+    }
+    result['sca_tool'].append(cdxgen_item)
+    
+    # 2.通过包列举命令获取包信息
+    if package_cmd:
+        for i in config.LANG_PACKAGE_CMD[language]:
+            # 若不同语言继续有细分，可在此进行各个语言的处理
+            if language == 'python':
+                try:
+                    item = {
+                        'cmd': i,
+                        'result': None
+                    }
+                    # 虚拟环境
+                    if os.path.exists(src_dir + '/venv'):
+                        res = exec_tool((src_dir + '/venv/bin/' + i).split(), cwd=src_dir)
+                        item['result'] = res
+                    else:
+                        res = exec_tool(i.split(), cwd=src_dir)
+                        item['result'] = res
+                    result['package_cmd'].append(item)
+                except Exception as e:
+                    logger.error(e)
+            else:
+                try:
+                    item = {
+                        'cmd': i,
+                        'result': None
+                    }
+                    res = exec_tool(i.split(), cwd=src_dir)
+                    item['result'] = res
+                    result['package_cmd'].append(item)
+                except Exception as e:
+                    logger.error(e)
+    # 3.读取依赖文件
+    if package_file:
+        for i in config.LANG_PACKAGE_FILE[language]:
+            if os.path.exists(src_dir + '/' + i):
+                logger.info('存在包文件-{}'.format(src_dir + '/' + i))
+                result['package_file'].append(src_dir + '/' + i)
+    # 4.读取dockerfile
+    if docker_file:
+        for i in config.DOCKER_FILE_LIST:
+            if os.path.exists(src_dir + '/' + i):
+                logger.info('存在dockerfile文件-{}'.format(src_dir + '/' + i))
+                result['docker_file'].append(src_dir + '/' + i)
+    return result
+
+# 基础工具检测
+def base_tool_check():
+    pass
+
+# 依赖工具安装
+def base_tool_install():
+    pass
 
+
+# 服务端检测
+class VoyagerDetect():
     def __init__(self, token=None, url=None, username=None, password=None):
         self.api_url = url
         self.api_token = token
         self.api_username = username
         self.api_password = password
         self.req = requests.Session()
 
@@ -266,14 +286,15 @@
             else:
                 # token失效，使用账号密码登录
                 login_status['message'] = 'token失效，使用账号密码登录'
 
         if self.api_username and self.api_password:
             # 获取认证token
             token = self.get_new_token()
+            # logger.info(token)
             if token:
                 self.api_token = token
                 headers = {
                     # 注意Token后有空格
                     'Authorization': 'Token ' + self.api_token
                 }
                 self.req.headers = headers
@@ -282,74 +303,48 @@
                 login_status['message'] = '无法生成访问token，账号密码可能错误'
         else:
             login_status['message'] = '请提供API账号以及密码信息'
         logger.info(login_status['message'])
         return login_status
 
     # sca分析
-    def sca_analysis(self, project_type, bom_file, src_dir=".", deep=False):
-        """Method to create BOM file by executing cdxgen command
-
-        :param project_type: Project type
-        :param bom_file: BOM file
-        :param src_dir: Source directory
-
-        :returns True if the command was executed. False if the executable was not found.
-        """
-        cdxgen_cmd = os.environ.get("CDXGEN_CMD", "cdxgen")
-        if not shutil.which(cdxgen_cmd):
-            local_bin = resource_path(
-                os.path.join(
-                    "local_bin", "cdxgen.exe" if sys.platform == "win32" else "cdxgen"
-                )
-            )
-            if not os.path.exists(local_bin):
-                logger.warning(
-                    "{} command not found. Please install using npm install @appthreat/cdxgen or set PATH variable".format(
-                        cdxgen_cmd
-                    )
-                )
-                return False
-            try:
-                cdxgen_cmd = local_bin
-                # Set the plugins directory as an environment variable
-                os.environ["CDXGEN_PLUGINS_DIR"] = resource_path("local_bin")
-            except Exception as e:
-                pass
-        if project_type:
-            if project_type in ("docker"):
-                logger.info(
-                    f"Generating Software Bill-of-Materials for container image {src_dir}. This might take a few mins ..."
-                )
-            sca_args = [cdxgen_cmd, "-r", "-t", project_type, "-o", bom_file]
-            if deep or project_type in ("jar", "jenkins"):
-                sca_args.append("--deep")
-                logger.info("About to perform deep scan. This would take a while ...")
-        else:
-            sca_args = [cdxgen_cmd, "-o", bom_file]
-        sca_args.append(src_dir)
-        print(sca_args)
-        exec_tool(['ls', '/app'],)
-        exec_tool(sca_args,)
-        return os.path.exists(bom_file)
+    def sca_analysis(self, language, src_dir=".", sca_tool=True, package_cmd=True, package_file=True, docker_file=True, deep=False):
+        result = get_sca_info(language=language, src_dir=src_dir, sca_tool=sca_tool,
+                              package_cmd=package_cmd, package_file=package_file,docker_file=docker_file, deep=deep)
+        return result
 
-    # 2.进行扫描
+    # 0.4旧版本的流水线卡点的扫描
     def scan(self, data, files):
         login_status = self.login()
         if login_status['status']:
             if files:
                 response = self.req.post(self.api_url + 'api/scan/detect/', data=data, files=files)
             else:
                 response = self.req.post(self.api_url + 'api/scan/detect/', data=data, files=[ ('files', ('', None, )),])
             return response.json()
         else:
             return login_status
 
 
-    # 3.获取扫描结果或报告
+    # 获取扫描结果或报告
     def get_scan_result(self, task_id):
         login_status = self.login()
         if login_status['status']:
             response = self.req.get(self.api_url + 'api/scan/scan-log/?task_id={}'.format(task_id),)
             return response.json()
         else:
             return login_status
+    
+    # 新版的与服务端交互
+    def base_scan(self, data, files):
+        login_status = self.login()
+        if login_status['status']:
+            if files:
+                response = self.req.post(self.api_url + config.VOYAGER_BASE_SCAN_API, data=data, files=files)
+            else:
+                response = self.req.post(self.api_url + config.VOYAGER_BASE_SCAN_API, data=data, files=[('files', ('', None,)), ])
+            return response.json()
+        else:
+            return login_status['message']
+    
+
+
```

### Comparing `plutonium-238-0.1.4/plutonium_238.egg-info/PKG-INFO` & `plutonium-238-0.1.5/plutonium_238.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutonium-238
-Version: 0.1.4
+Version: 0.1.5
 Summary: SCA Agent, Copyright@Plutonium
 Home-page: https://www.google.com
 Author: tom
 Author-email: tom@google.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `plutonium-238-0.1.4/setup.py` & `plutonium-238-0.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plutonium-238",
-    version="0.1.4",
+    version="0.1.5",
     author="tom",
     author_email="tom@google.com",
     description="SCA Agent, Copyright@Plutonium",
     entry_points={
         "console_scripts": ["plutonium=plutonium.cli:main",]
     },
     license="MIT",
```

