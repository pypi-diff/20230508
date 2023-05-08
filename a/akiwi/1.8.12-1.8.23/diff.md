# Comparing `tmp/akiwi-1.8.12.tar.gz` & `tmp/akiwi-1.8.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akiwi-1.8.12.tar", last modified: Thu Mar  2 04:01:07 2023, max compression
+gzip compressed data, was "akiwi-1.8.23.tar", last modified: Mon May  8 13:10:09 2023, max compression
```

## Comparing `akiwi-1.8.12.tar` & `akiwi-1.8.23.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 wish      (1000) wish      (1000)        0 2023-03-02 04:01:07.810169 akiwi-1.8.12/
--rw-rw-r--   0 wish      (1000) wish      (1000)      231 2023-03-02 04:01:07.810169 akiwi-1.8.12/PKG-INFO
--rw-rw-r--   0 wish      (1000) wish      (1000)       38 2023-02-09 14:35:55.000000 akiwi-1.8.12/README.md
-drwxrwxr-x   0 wish      (1000) wish      (1000)        0 2023-03-02 04:01:07.798169 akiwi-1.8.12/akiwi/
--rw-rw-r--   0 wish      (1000) wish      (1000)        0 2023-02-12 06:35:23.000000 akiwi-1.8.12/akiwi/__init__.py
--rw-rw-r--   0 wish      (1000) wish      (1000)      174 2023-02-14 13:56:39.000000 akiwi-1.8.12/akiwi/__main__.py
--rw-rw-r--   0 wish      (1000) wish      (1000)    49150 2023-03-02 04:00:39.000000 akiwi-1.8.12/akiwi/app.py
-drwxrwxr-x   0 wish      (1000) wish      (1000)        0 2023-03-02 04:01:07.810169 akiwi-1.8.12/akiwi/bin/
--rw-rw-r--   0 wish      (1000) wish      (1000)      660 2023-03-02 02:24:29.000000 akiwi-1.8.12/akiwi/bin/kiwi.sh-temp
--rw-rw-r--   0 wish      (1000) wish      (1000)     1419 2023-02-12 03:33:02.000000 akiwi-1.8.12/akiwi/check.py
--rw-rw-r--   0 wish      (1000) wish      (1000)     4918 2023-02-17 13:00:11.000000 akiwi-1.8.12/akiwi/http.py
--rw-rw-r--   0 wish      (1000) wish      (1000)     8874 2023-03-02 03:58:50.000000 akiwi-1.8.12/akiwi/utils.py
--rw-rw-r--   0 wish      (1000) wish      (1000)       20 2023-03-02 04:00:24.000000 akiwi-1.8.12/akiwi/version.py
-drwxrwxr-x   0 wish      (1000) wish      (1000)        0 2023-03-02 04:01:07.810169 akiwi-1.8.12/akiwi.egg-info/
--rw-rw-r--   0 wish      (1000) wish      (1000)      231 2023-03-02 04:01:07.000000 akiwi-1.8.12/akiwi.egg-info/PKG-INFO
--rw-rw-r--   0 wish      (1000) wish      (1000)      355 2023-03-02 04:01:07.000000 akiwi-1.8.12/akiwi.egg-info/SOURCES.txt
--rw-rw-r--   0 wish      (1000) wish      (1000)        1 2023-03-02 04:01:07.000000 akiwi-1.8.12/akiwi.egg-info/dependency_links.txt
--rw-rw-r--   0 wish      (1000) wish      (1000)       45 2023-03-02 04:01:07.000000 akiwi-1.8.12/akiwi.egg-info/entry_points.txt
--rw-rw-r--   0 wish      (1000) wish      (1000)        1 2023-02-11 02:08:48.000000 akiwi-1.8.12/akiwi.egg-info/not-zip-safe
--rw-rw-r--   0 wish      (1000) wish      (1000)       22 2023-03-02 04:01:07.000000 akiwi-1.8.12/akiwi.egg-info/requires.txt
--rw-rw-r--   0 wish      (1000) wish      (1000)        6 2023-03-02 04:01:07.000000 akiwi-1.8.12/akiwi.egg-info/top_level.txt
--rw-rw-r--   0 wish      (1000) wish      (1000)       38 2023-03-02 04:01:07.810169 akiwi-1.8.12/setup.cfg
--rw-rw-r--   0 wish      (1000) wish      (1000)     1017 2023-02-21 13:26:47.000000 akiwi-1.8.12/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 13:10:09.228276 akiwi-1.8.23/
+-rw-r--r--   0 root         (0) root         (0)      231 2023-05-08 13:10:09.224276 akiwi-1.8.23/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 12:59:35.000000 akiwi-1.8.23/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 13:10:09.212276 akiwi-1.8.23/akiwi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 12:59:35.000000 akiwi-1.8.23/akiwi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-05-08 12:59:35.000000 akiwi-1.8.23/akiwi/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    51470 2023-05-08 12:59:35.000000 akiwi-1.8.23/akiwi/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 13:10:09.224276 akiwi-1.8.23/akiwi/bin/
+-rw-r--r--   0 root         (0) root         (0)      660 2023-05-08 12:59:35.000000 akiwi-1.8.23/akiwi/bin/kiwi.sh-temp
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-05-08 12:59:35.000000 akiwi-1.8.23/akiwi/check.py
+-rw-r--r--   0 root         (0) root         (0)     4918 2023-05-08 12:59:35.000000 akiwi-1.8.23/akiwi/http.py
+-rw-r--r--   0 root         (0) root         (0)     8881 2023-05-08 12:59:35.000000 akiwi-1.8.23/akiwi/utils.py
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-08 12:59:35.000000 akiwi-1.8.23/akiwi/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 13:10:09.220276 akiwi-1.8.23/akiwi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      231 2023-05-08 13:10:08.000000 akiwi-1.8.23/akiwi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-08 13:10:09.000000 akiwi-1.8.23/akiwi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 13:10:08.000000 akiwi-1.8.23/akiwi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-08 13:10:08.000000 akiwi-1.8.23/akiwi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 13:05:59.000000 akiwi-1.8.23/akiwi.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-08 13:10:08.000000 akiwi-1.8.23/akiwi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-08 13:10:08.000000 akiwi-1.8.23/akiwi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 13:10:09.228276 akiwi-1.8.23/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-08 12:59:35.000000 akiwi-1.8.23/setup.py
```

### Comparing `akiwi-1.8.12/akiwi/app.py` & `akiwi-1.8.23/akiwi/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 from urllib.parse import urlencode
 from . import http
 from . import utils
 from . import version
 from collections import OrderedDict
 
 __None_Env_Name__ = ""
+__Bash_Name__     = "~/.bashrc"
+
+if platform.system().lower() == "darwin":
+    __Bash_Name__ = "~/.zshrc"
 
 class ChangeCWD:
     def __init__(self, dir):
         self.dir = os.path.abspath(dir)
         self.old = os.path.abspath(os.getcwd())
     
     def __enter__(self):
@@ -83,28 +87,34 @@
         self.CONFIG_JSON  = os.path.join(self.CACHE_ROOT, "config.json")
         self.CURRENT_ENV  = "base"
         self.VENV_JSON    = os.path.join(self.VENV_DIR, f"{self.CURRENT_ENV}.json")
         self.INSTALLED_LIBS_JSON  = os.path.join(self.CACHE_ROOT, "libs.json")
         self.OS_NAME     = platform.system().lower()
         self.PY_VERSION  = ".".join(sys.version.split(".")[:2])
         self.CWD         = os.path.abspath(os.path.curdir)
-        self.PYINCLUDE_DIR = paths.get("include", "")
-        self.PYLIB_NAME  = sysconfig.get_config_var("LIBRARY").replace("lib", "").replace(".so", "").replace(".a", "")
-        self.PYLIB_PATH  = sysconfig.get_config_var("LIBDIR")
+        self.PYTHON_INCLUDE = paths.get("include", "")
+
+        def get_config_var(name):
+            if sysconfig.get_config_var(name) is None:
+                return ""
+            return sysconfig.get_config_var(name)
+
+        self.PYTHON_LINK = get_config_var("LIBRARY").replace("lib", "").replace(".so", "").replace(".a", "")
+        self.PYTHON_LIB  = get_config_var("LIBDIR")
         self.DATA_DIR    = os.path.join(self.CACHE_ROOT, "data")
         self.PKG_DIR     = os.path.join(self.CACHE_ROOT, "pkg")
         self.LIB_DIR     = os.path.join(self.CACHE_ROOT, "lib")
         self.CODE_DIR    = os.path.join(self.CACHE_ROOT, "code")
         os.makedirs(self.CACHE_ROOT, exist_ok=True)
         os.makedirs(self.DATA_DIR, exist_ok=True)
         os.makedirs(self.PKG_DIR,  exist_ok=True)
         os.makedirs(self.LIB_DIR,  exist_ok=True)
         os.makedirs(self.CODE_DIR, exist_ok=True)
         os.makedirs(self.VENV_DIR, exist_ok=True)
-        
+
         self.ACCESS_TOKEN = ""
         self.dynamic_keys = [
             "ACCESS_TOKEN", "SERVER", "CURRENT_ENV"
         ]
         self.INSTALLED_LIBS = {}
         self.VENV           = {"libs":{}, "macros":{}, "envars":{}}
         self.setup()
@@ -122,21 +132,21 @@
     def get_dict(self):
         return {
             "SERVER"     : self.SERVER,
             "CACHE_ROOT" : self.CACHE_ROOT,
             "CONFIG_JSON" : self.CONFIG_JSON,
             "VENV_JSON" : self.VENV_JSON,
             "INSTALLED_LIBS_JSON" : self.INSTALLED_LIBS_JSON,
-            "PYINCLUDE_DIR": self.PYINCLUDE_DIR,
+            "PYTHON_INCLUDE": self.PYTHON_INCLUDE,
             "CURRENT_ENV": self.CURRENT_ENV,
             "OS_NAME" : self.OS_NAME,
             "PY_VERSION" : self.PY_VERSION,
             "CWD" :       self.CWD,
-            "PYLIB_NAME" : self.PYLIB_NAME,
-            "PYLIB_PATH" : self.PYLIB_PATH,
+            "PYTHON_LINK" : self.PYTHON_LINK,
+            "PYTHON_LIB" : self.PYTHON_LIB,
             "DATA_DIR" : self.DATA_DIR,
             "PKG_DIR" : self.PKG_DIR,
             "LIB_DIR" : self.LIB_DIR,
             "CODE_DIR" : self.CODE_DIR,
             "ACCESS_TOKEN" : self.ACCESS_TOKEN
         }
 
@@ -148,15 +158,15 @@
                 if key in self.dynamic_keys:
                     if cfg[key] is not None:
                         setattr(self, key, cfg[key])
                 else:
                     utils.vprint(f"Unknow config name {key}")
         else:
             self.dump_config()
-        
+
         cfg = utils.loadjson_dict(self.INSTALLED_LIBS_JSON)
         if cfg is not None:
             self.INSTALLED_LIBS = cfg
 
         if self.CURRENT_ENV != __None_Env_Name__:
             self.VENV_JSON  = os.path.join(self.VENV_DIR, f"{self.CURRENT_ENV}.json")
             cfg = utils.loadjson_dict(self.VENV_JSON)
@@ -185,15 +195,15 @@
     def __repr__(self):
         sb  = ["Config:"]
         dic = self.get_dict()
         for key in dic:
             val = dic[key]
             sb.append(f"   {key} = {val}")
         return "\n".join(sb)
-    
+
     def create_env(self, name, copyfrom):
 
         if copyfrom is not None:
             env_file  = os.path.join(self.VENV_DIR, f"{copyfrom}.json")
             if not os.path.exists(env_file):
                 utils.gprint(f"Invalid enviroment '{copyfrom}'")
                 return False
@@ -224,15 +234,15 @@
             utils.gprint("You can not execute activate directly, you must use the posix shell to make the environment variables take effect.")
             return False
 
         env_json  = os.path.join(self.VENV_DIR, f"{name}.json")
         if not os.path.exists(env_json):
             utils.gprint(f"Not exists virtual enviroment: {name}")
             return False
-        
+
         cfg = utils.loadjson_dict(env_json)
         if cfg is None:
             utils.gprint(f"Failed to load the virtual enviroment: {name}")
             return False
 
         self.VENV_JSON  = env_json
         self.VENV = cfg
@@ -242,15 +252,15 @@
         self.CURRENT_ENVARS = self.VENV.get("envars", {})
         vars_map = self.get_dict()
         for key in vars_map:
             os.environ["KIWI_" + key] = vars_map[key]
 
         for key in self.CURRENT_MACROS:
             os.environ["KIWI_" + key] = self.parse_lib_value_ref(self.CURRENT_MACROS[key])
-            
+
         ret_ok = self.dump_venv() and self.dump_config()
         self.print_current_envars_exporter()
         return ret_ok
 
     def deactivate_env(self):
 
         if not utils.shellposix:
@@ -261,18 +271,18 @@
         self.VENV = {"libs":{}, "macros":{}, "envars":{}}
         self.CURRENT_ENV = __None_Env_Name__
         self.CURRENT_MACROS = self.VENV.get("macros", {})
         self.CURRENT_LIBS   = self.VENV.get("libs", {})
         self.CURRENT_ENVARS = self.VENV.get("envars", {})
         if not self.dump_config():
             return False
-        
+
         self.print_original_env_exporter()
         return True
-    
+
     def print_current_envars_exporter(self):
 
         if self.CURRENT_ENV == __None_Env_Name__:
             self.print_original_env_exporter()
             return True
 
         if not utils.shellposix:
@@ -326,78 +336,90 @@
         # if "KIWI_OLD_PS1" in os.environ:
         #     old_ps1 = os.environ["KIWI_OLD_PS1"]
         #     utils.cmdprint(f"export PS1=\"{old_ps1}\"")
 
         for key in ["PATH", "LD_LIBRARY_PATH", "PYTHONPATH"]:
             utils.cmdprint(f"export {key}=$KIWI_OLD_{key}")
         return True
-    
+
     def check_package(self, name, version_min=None, version_max=None):
 
         if name not in self.CURRENT_LIBS:
             return False, None, None
-        
+
         version, folder_name, description = self.CURRENT_LIBS[name]
         if utils.version_limit(version, version_min, version_max):
             return True, version, folder_name
-        
+
         return False, "", ""
 
 class Actions:
     def __init__(self, app):
         self.app : Application = app
         self.cfg : Config = app.cfg
 
     def private_run_cmd(self, args, _addi_args):
-        
+
         cmd = args.cmd
         if not hasattr(self, cmd):
             return False
 
         del args.__dict__["cmd"]
         return getattr(self, cmd)(args, _addi_args)
 
     def __rmtree(self, dir):
         dir = dir.strip()
         if dir == "." or dir == ".." or dir == "/":
             utils.vprint(f"Can not remove directory [{dir}]")
             return
 
         if os.path.exists(dir):
-            utils.vprint(f"Remove directory: {dir}")
-            shutil.rmtree(dir)
+            if os.path.islink(dir):
+                utils.vprint(f"Remove directory link: {dir}")
+                os.remove(dir)
+            else:
+                utils.vprint(f"Remove directory tree: {dir}")
+                shutil.rmtree(dir)
 
-    def __run_requirement(self, file):
+    def __run_requirement(self, file, args):
         utils.vprint(f"Run requirement script file: {file} at {os.getcwd()}")
         try:
+            update_flag = ""
+            if hasattr(args, "update") and args.update:
+                update_flag = " -update"
+
+            force_flag = ""
+            if hasattr(args, "force") and args.force:
+                force_flag = " -force"
+
             lines = open(file, "r").read().split("\n")
             for line in lines:
                 line = line.strip()
                 if line.startswith("#") or line == "":
                     continue
 
                 if line.startswith("@"):
                     if len(line) < 3: return False
-                    utils.vprint(f"Run data command: {line[1:]}")
-                    if not self.app.run_with_command(f"getd {line[1:]}"):
+                    utils.vprint(f"Run data command: {line[1:]}{update_flag}")
+                    if not self.app.run_with_command(f"getd {line[1:]}{update_flag}"):
                         return False
                 elif line.startswith("$"):
                     if len(line) < 3: return False
-                    utils.vprint(f"Run repo command: {line[1:]}")
-                    if not self.app.run_with_command(f"get {line[1:]}"):
+                    utils.vprint(f"Run repo command: {line[1:]}{update_flag}")
+                    if not self.app.run_with_command(f"get {line[1:]}{update_flag}"):
                         return False
                 elif line == "rep":
                     utils.vprint(f"Run install command: {line}")
                     if not self.app.run_with_command(line):
                         return False
                 elif line.startswith(">"):
                     utils.gprint(line[1:])
                 else:
-                    utils.vprint(f"Run install command: {line}")
-                    if not self.app.run_with_command(f"install {line}"):
+                    utils.vprint(f"Run install command: {line}{update_flag}{force_flag}")
+                    if not self.app.run_with_command(f"install {line}{update_flag}{force_flag}"):
                         return False
             return True
         except Exception as e:
             traceback.print_exc()
         return False
 
     def __run_py(self, file, args):
@@ -414,15 +436,15 @@
             utils.remove(temp_code_file)
             result =  getattr(m, "run")(self.app, args)
             ddir = os.path.join(code_dir, "__pycache__")
             self.__rmtree(ddir)
         except Exception as e:
             traceback.print_exc()
             result = False
-        
+
         self.__rmtree(".kiwi/__pycache__")
         return result
 
     def __run_bash(self, file):
         utils.vprint(f"Run bash script file: {file} at {os.getcwd()}")
 
         try:
@@ -432,15 +454,15 @@
             code = os.system(f'bash \"{temp_code_file}\"')
             utils.remove(temp_code_file)
             return code == 0
         except Exception as e:
             traceback.print_exc()
             return False
 
-    def __run_link(self, file):
+    def __run_link(self, file, delfile=True):
         if not os.path.exists(file):
             return False
 
         try:
             dir = os.path.realpath(os.path.dirname(file))
             with ChangeCWD(dir):
                 utils.vprint(f"Run link script file: {file} at {os.getcwd()}")
@@ -462,29 +484,35 @@
                     op    = opts[0]
                     param = opts[1]
                     if op == "link":
                         ps = param.split(" ")
                         if len(ps) == 2:
                             fa = os.path.abspath(ps[0])
                             fb = os.path.abspath(ps[1])
-                            utils.vprint(f"Run link command: ln -s \"{fa}\" \"{fb}\"")
+                            if os.path.exists(fb):
+                                utils.vprint(f"Remove the old link file: {fb}")
+                                os.remove(fb)
 
+                            utils.vprint(f"Run link command: ln -s \"{fa}\" \"{fb}\"")
                             if os.system(f"ln -s \"{fa}\" \"{fb}\"") != 0:
                                 utils.gprint(f"Failed to run command: ln -s \"{fa}\" \"{fb}\"")
                                 return False
                         elif len(ps) == 1:
                             fa = os.path.abspath(ps[0])
                             p  = ps[0].rfind(".so")
                             if p == -1:
                                 utils.gprint(f"Can not process this command: {line}")
                                 return
 
                             fb = os.path.abspath(ps[0][:p+3])
-                            utils.vprint(f"Run link command: ln -s \"{fa}\" \"{fb}\"")
+                            if os.path.exists(fb):
+                                utils.vprint(f"Remove the old link file: {fb}")
+                                os.remove(fb)
 
+                            utils.vprint(f"Run link command: ln -s \"{fa}\" \"{fb}\"")
                             if os.system(f"ln -s \"{fa}\" \"{fb}\"") != 0:
                                 utils.gprint(f"Failed to run command: ln -s \"{fa}\" \"{fb}\"")
                                 return False
                         else:
                             utils.gprint(f"Invalid command in line: {i}, {line}")
                             return False
 
@@ -498,26 +526,27 @@
                     elif op == "headpy":
                         utils.vprint(f"Run headpy: {param}")
 
                         headpyfile = param
                         if not os.path.exists(headpyfile):
                             utils.gprint(f"File not exists: {headpyfile}")
                             return False
-                        
+
                         lines = open(headpyfile, "r", encoding="utf-8").read().split("\n")
                         if len(lines) < 1:
                             utils.gprint(f"Invalid file to headpy: {headpyfile}")
                             return False
-                        
+
                         lines[0] = f"#!{sys.executable}"
                         open(headpyfile, "w").write("\n".join(lines))
                     else:
                         utils.gprint(f"Unknow command: {line}")
 
-            utils.remove(file)
+            if delfile:
+                utils.remove(file)
             return True
         except Exception as e:
             traceback.print_exc()
             return False
 
     def __atomatic_run(self, work_dir, args):
         with ChangeCWD(work_dir):
@@ -536,15 +565,15 @@
                     return False
             else:
                 utils.vprint(f"The non-existent file {auto_config_file}")
 
             auto_config_file = "kiwi.required"
             if os.path.exists(auto_config_file):
                 utils.vprint(f"Run automatic script {auto_config_file}")
-                if not self.__run_requirement(auto_config_file):
+                if not self.__run_requirement(auto_config_file, args):
                     return False
             else:
                 utils.vprint(f"The non-existent file {auto_config_file}")
         return True
 
     def __register_lib(self, folder_name, lib_file):
         try:
@@ -601,36 +630,36 @@
             for key in attributes:
                 if key not in ["NAME", "VERSION", "DESCRIPTION", "PATH", "LD_LIBRARY_PATH", "PYTHONPATH"]:
                     utils.vprint(f"Register macro: {key} = {attributes[key]}")
                     self.cfg.CURRENT_MACROS[key] = {"value": attributes[key], "ref": folder_name}
 
             if not self.cfg.dump_venv():
                 return False
-            
+
             self.cfg.print_current_envars_exporter()
             return self.cfg.dump_venv()
         except Exception as e:
             traceback.print_exc()
             utils.gprint(f"Failed to register lib {folder_name}")
             pass
         return False
 
     def __replace_variable(self, directory, filter, inverse=False):
-        
+
         if directory is None:
             directory = os.path.abspath(".")
-        
+
         default_list = ".json;makefile;cmakelists.txt;.sh;.bash"
         filter_list  = default_list
         if filter is not None:
             filter_list = filter
 
         select_names = [
-            "DATA_DIR", "CODE_DIR", "PKG_DIR", "LIB_DIR", "PYLIB_NAME", "PYLIB_PATH", "CWD",
-            "CACHE_ROOT", "PYLIB_NAME", "PYINCLUDE_DIR"
+            "DATA_DIR", "CODE_DIR", "PKG_DIR", "LIB_DIR", "PYTHON_LINK", "PYTHON_LIB", "CWD",
+            "CACHE_ROOT", "PYTHON_INCLUDE"
         ]
         if inverse:
             vars_map  = {self.cfg.parse_lib_value_ref(self.cfg.CURRENT_MACROS[key]):key for key in self.cfg.CURRENT_MACROS}
             vars_dict = self.cfg.get_dict()
             for name in select_names:
                 vars_map[vars_dict[name]] = name
 
@@ -667,24 +696,33 @@
         templ_bashrc = f'''{bashrc_token_begin}
 # !! Contents within this block are managed by 'kiwi init' !!
 if [ -f \"{kiwi_sh}\" ]; then
     . \"{kiwi_sh}\"
     kiwi activate
 fi
 {bashrc_token_end}'''
-        bashrc_content = open(os.path.expanduser("~/.bashrc"), "r").read()
-        p0 = bashrc_content.find(bashrc_token_begin)
-        p1 = bashrc_content.find(bashrc_token_end)
+
+        bash_file = os.path.expanduser(__Bash_Name__)
+        if not os.path.exists(bash_file):
+            utils.vprint(f"Not found file: {bash_file}")
+            return False
+
+        old_bashrc_content = open(os.path.expanduser(__Bash_Name__), "r").read()
+        p0 = old_bashrc_content.find(bashrc_token_begin)
+        p1 = old_bashrc_content.find(bashrc_token_end)
         if p0 != -1 and p1 != -1:
-            bashrc_content = bashrc_content[:p0] + templ_bashrc + bashrc_content[p1+len(bashrc_token_end):]
+            new_bashrc_content = old_bashrc_content[:p0] + templ_bashrc + old_bashrc_content[p1+len(bashrc_token_end):]
         else:
-            bashrc_content += "\n" + templ_bashrc + "\n"
+            new_bashrc_content = old_bashrc_content + "\n" + templ_bashrc + "\n"
 
-        utils.vprint(f"Add specific scripts to bashrc to support kiwi running.")
-        open(os.path.expanduser("~/.bashrc"), "w").write(bashrc_content)
+        if old_bashrc_content != new_bashrc_content:
+            utils.vprint(f"Add specific scripts to bashrc to support kiwi running.")
+            open(os.path.expanduser(__Bash_Name__), "w").write(new_bashrc_content)
+        else:
+            utils.vprint(f"Bashrc has no changed.")
         # utils.gprint("The initialization is complete and you can restart the terminal to take effect the corresponding changes.")
         
         kiwi_sh_lines = open(kiwi_sh_temp, "r").read().split("\n")
         kiwi_exe = sys.argv[0]
         dst_value = f"export KIWI_EXE='{kiwi_exe}'"
         kiwi_sh_lines[0] = dst_value
 
@@ -721,26 +759,31 @@
                 utils.vprint(f"[install {folder_name}] Since the installation directory already exists and is registered, we do not do anything without force")
                 return True
             
         if not args.normtree:
             self.__rmtree(install_to)
 
         os.environ["KIWI_PKG_INSTALL_TO"] = install_to
-        shutil.copytree(directory, install_to, dirs_exist_ok=True)
+        if args.symlink:
+            utils.vprint(f"Symbol link {directory} to {install_to}")
+            os.symlink(directory, install_to, target_is_directory=True)
+        else:
+            utils.vprint(f"Copy files {directory} to {install_to}")
+            shutil.copytree(directory, install_to, dirs_exist_ok=True)
 
         if not args.disable_run:
             if not self.__atomatic_run(install_to, args):
                 return False
         else:
             utils.vprint(f"Do not run any automatic scripts, because disable_run is set.")
         
         utils.gprint(f"Install to {install_to}")
         link_file = os.path.abspath(os.path.join(install_to, ".kiwi.link"))
         if os.path.exists(link_file):
-            if not self.__run_link(link_file):
+            if not self.__run_link(link_file, delfile=not args.symlink):
                 return False
 
         lib_file = os.path.abspath(os.path.join(install_to, ".kiwi.lib"))
         if os.path.exists(lib_file):
             return self.__register_lib(folder_name, lib_file)
         return True
 
@@ -760,15 +803,26 @@
 
         setattr(self.cfg, args.key, args.value)
         self.cfg.dump_config()
         utils.gprint("Success!")
         return True
 
     def auth(self, args : argparse.Namespace, addi_args):
-        setattr(self.cfg, "ACCESS_TOKEN", args.token)
+
+        token = args.token
+        if token is None:
+            user_name = input("User Name: ").strip().replace(" ", "")
+            password  = input("Password: ").strip().replace(" ", "")
+            result = http.request_text(f"{self.cfg.SERVER}/authc/login?loginName={user_name}&password={password}")
+            if result is None:
+                return False
+            
+            token  = result["security_key"]
+
+        setattr(self.cfg, "ACCESS_TOKEN", token)
         self.cfg.dump_config()
         utils.gprint("Success!")
         return True
 
     def get(self, args : argparse.Namespace, addi_args):
         repo = args.repo
         if repo.find("/") == -1:
@@ -850,15 +904,15 @@
         #     utils.vprint(f"Do not run any automatic scripts, because disable_run is set.")
         return True
 
     def install(self, args : argparse.Namespace, addi_args):
 
         if args.pkg is None:
             if os.path.exists("kiwi.required"):
-                return self.__run_requirement("kiwi.required")
+                return self.__run_requirement("kiwi.required", args)
             else:
                 utils.gprint("The command 'install' need a pkg augment.")
                 return False
 
         if os.path.isdir(args.pkg):
             return self.__local_install(args, addi_args)
 
@@ -951,16 +1005,16 @@
         return True
 
     def macros(self, args : argparse.Namespace, addi_args):
 
         utils.gprint(f"{len(self.cfg.CURRENT_MACROS)} macros found:")
 
         select_names = [
-            "DATA_DIR", "CODE_DIR", "PKG_DIR", "LIB_DIR", "PYLIB_PATH",
-            "CACHE_ROOT", "PYLIB_NAME", "PYINCLUDE_DIR"
+            "DATA_DIR", "CODE_DIR", "PKG_DIR", "LIB_DIR", "PYTHON_LIB",
+            "CACHE_ROOT", "PYTHON_LINK", "PYTHON_INCLUDE"
         ]
         vars_dict = self.cfg.get_dict()
         vars_map  = {}
         for name in select_names:
             vars_map[name] = vars_dict[name]
 
         for i, key in enumerate(self.cfg.CURRENT_MACROS):
@@ -1011,15 +1065,15 @@
 
         file    = args.runfile
         workdir = args.workdir
 
         already_run_required = False
         if file is None:
             if os.path.exists("kiwi.required"):
-                already_run_required = self.__run_requirement("kiwi.required")
+                already_run_required = self.__run_requirement("kiwi.required", args)
                 if not already_run_required:
                     return False
             
             file = os.path.abspath(".kiwi/auto.py")
             if not os.path.exists(file):
                 cwd = os.path.abspath(os.getcwd())
                 p = cwd.rfind("/")
@@ -1037,15 +1091,16 @@
                     while p != -1:
                         file = os.path.join(cwd[:p], ".kiwi/auto.sh")
                         if os.path.exists(file):
                             break
                         p = cwd.rfind("/", 0, p)
 
         if not os.path.exists(file):
-            if already_run_required: return True
+            if already_run_required: 
+                return self.app.run_with_command("rep")
             utils.gprint("Can not found any auto script to run.")
             return False
 
         if workdir is None:
             workdir = os.path.dirname(os.path.dirname(file))
 
         with ChangeCWD(workdir):
@@ -1069,14 +1124,15 @@
                 args.__dict__.update(kwargs_map)
 
             ret = True
             if file.endswith(".py"):
                 ret = self.__run_py(file, args)
             elif file.endswith(".sh"):
                 ret = self.__run_bash(file)
+            ret = ret and self.app.run_with_command("rep")
             return ret
 
     def search(self, args : argparse.Namespace, addi_args):
         param = urlencode({"key": args.key, "accessToken": self.cfg.ACCESS_TOKEN})
         url = f"{self.cfg.SERVER}/public/search/list?" + param
         data = http.request_text(url)
         if data is None:
@@ -1111,15 +1167,15 @@
         c.add_argument("-disable-run", action="store_true", help="Disable auto run")
 
         c = cmd.add_cmd("run", "Run the project automation script")
         c.add_argument("-runfile", type=str, help="script file, default is .kiwi/auto.py or .kiwi/auto.sh")
         c.add_argument("-workdir", type=str, help="workspace dir, default is solution dir")
 
         c = cmd.add_cmd("auth", "Set auth ACCESS_TOKEN")
-        c.add_argument("token", type=str, help="Access token name")
+        c.add_argument("token", nargs="?", type=str, help="Access token name")
 
         c = cmd.add_cmd("getd", "Get data from server")
         c.add_argument("data", type=str, help="data name")
         c.add_argument("-update", action="store_true", help="Force update")
         c.add_argument("-save", type=str, help="Unzipped folder")
         c.add_argument("-rmtree", action="store_true", help="Unzip the data after remove the save folder.")
 
@@ -1149,14 +1205,15 @@
         c = cmd.add_cmd("install", "Install package from server")
         c.add_argument("pkg", nargs="?", type=str, help="package name")
         c.add_argument("-update", action="store_true", help="Force update")
         c.add_argument("-save", type=str, help="Unzipped folder")
         c.add_argument("-normtree", action="store_true", help="Unzip the data after remove the save folder.")
         c.add_argument("-disable-run", action="store_true", help="Disable auto run")
         c.add_argument("-force", action="store_true", help="Ignore existing installations and enforce them")
+        c.add_argument("-symlink", action="store_true", help="For local installations, only symbol link without copying files")
 
         c = cmd.add_cmd("search", "Search solution / data / package")
         c.add_argument("key", type=str, help="search name")
 
         c = cmd.add_cmd("qr", "下载手写AI微信二维码，以联系到手写AI")
         self.cmd = cmd
```

### Comparing `akiwi-1.8.12/akiwi/bin/kiwi.sh-temp` & `akiwi-1.8.23/akiwi/bin/kiwi.sh-temp`

 * *Files identical despite different names*

### Comparing `akiwi-1.8.12/akiwi/check.py` & `akiwi-1.8.23/akiwi/check.py`

 * *Files identical despite different names*

### Comparing `akiwi-1.8.12/akiwi/http.py` & `akiwi-1.8.23/akiwi/http.py`

 * *Files identical despite different names*

### Comparing `akiwi-1.8.12/akiwi/utils.py` & `akiwi-1.8.23/akiwi/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,20 +13,21 @@
         if shellposix:
             kwargs["file"] = sys.stderr
         print(*args, **kwargs)
 
 def gprint(msg, *args, **kwargs):
     if shellposix:
         kwargs["file"] = sys.stderr
-    msg = text_format_to_color(msg)
+
+    msg = text_format_to_color(str(msg))
     print(msg, *args, **kwargs)
 
 def cmdprint(cmd):
     if not shellposix:
-        print("Please restart the terminal to enable kiwi")
+        vprint("Please restart the terminal to enable kiwi")
         return
     print(f"@kiwicmd {cmd}")
 
 def get_python_link_name(pydll_path, os_name):
     if os_name == "linux":
         for so in os.listdir(pydll_path):
             if so.startswith("libpython") and not so.endswith(".so") and so.find(".so") != -1:
```

### Comparing `akiwi-1.8.12/setup.py` & `akiwi-1.8.23/setup.py`

 * *Files identical despite different names*

