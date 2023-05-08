# Comparing `tmp/AutoCython-jianjun-1.3.2.tar.gz` & `tmp/AutoCython-jianjun-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCython-jianjun-1.3.2.tar", last modified: Mon Mar  6 07:23:12 2023, max compression
+gzip compressed data, was "AutoCython-jianjun-1.3.3.tar", last modified: Mon May  8 12:01:39 2023, max compression
```

## Comparing `AutoCython-jianjun-1.3.2.tar` & `AutoCython-jianjun-1.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-06 07:23:12.695297 AutoCython-jianjun-1.3.2/
-drwxrwxrwx   0        0        0        0 2023-03-06 07:23:12.690310 AutoCython-jianjun-1.3.2/AutoCython/
--rw-rw-rw-   0        0        0    23940 2023-03-06 07:22:17.000000 AutoCython-jianjun-1.3.2/AutoCython/AutoCython.py
--rw-rw-rw-   0        0        0      456 2021-09-07 07:03:00.000000 AutoCython-jianjun-1.3.2/AutoCython/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 07:23:12.694299 AutoCython-jianjun-1.3.2/AutoCython_jianjun.egg-info/
--rw-rw-rw-   0        0        0     7864 2023-03-06 07:23:12.000000 AutoCython-jianjun-1.3.2/AutoCython_jianjun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-03-06 07:23:12.000000 AutoCython-jianjun-1.3.2/AutoCython_jianjun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 07:23:12.000000 AutoCython-jianjun-1.3.2/AutoCython_jianjun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-03-06 07:23:12.000000 AutoCython-jianjun-1.3.2/AutoCython_jianjun.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-03-06 07:23:12.000000 AutoCython-jianjun-1.3.2/AutoCython_jianjun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18431 2021-04-19 08:51:39.000000 AutoCython-jianjun-1.3.2/LICENSE
--rw-rw-rw-   0        0        0     7864 2023-03-06 07:23:12.695297 AutoCython-jianjun-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     7553 2022-11-23 08:25:21.000000 AutoCython-jianjun-1.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-03-06 07:23:12.695297 AutoCython-jianjun-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      706 2023-03-06 07:12:26.000000 AutoCython-jianjun-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:01:39.496991 AutoCython-jianjun-1.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-08 12:01:39.492004 AutoCython-jianjun-1.3.3/AutoCython/
+-rw-rw-rw-   0        0        0    24051 2023-05-08 12:00:42.000000 AutoCython-jianjun-1.3.3/AutoCython/AutoCython.py
+-rw-rw-rw-   0        0        0      456 2023-05-08 12:00:59.000000 AutoCython-jianjun-1.3.3/AutoCython/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:01:39.495994 AutoCython-jianjun-1.3.3/AutoCython_jianjun.egg-info/
+-rw-rw-rw-   0        0        0     4437 2023-05-08 12:01:39.000000 AutoCython-jianjun-1.3.3/AutoCython_jianjun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-08 12:01:39.000000 AutoCython-jianjun-1.3.3/AutoCython_jianjun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 12:01:39.000000 AutoCython-jianjun-1.3.3/AutoCython_jianjun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-08 12:01:39.000000 AutoCython-jianjun-1.3.3/AutoCython_jianjun.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 12:01:39.000000 AutoCython-jianjun-1.3.3/AutoCython_jianjun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    18431 2021-04-19 08:51:39.000000 AutoCython-jianjun-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0     4437 2023-05-08 12:01:39.496991 AutoCython-jianjun-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4126 2023-03-24 08:02:16.000000 AutoCython-jianjun-1.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 12:01:39.496991 AutoCython-jianjun-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      706 2023-05-08 12:01:04.000000 AutoCython-jianjun-1.3.3/setup.py
```

### Comparing `AutoCython-jianjun-1.3.2/AutoCython/AutoCython.py` & `AutoCython-jianjun-1.3.3/AutoCython/AutoCython.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         else:
             # utf-8
             self.out = po.stdout.read().decode()
             self.err = po.stderr.read().decode()
 
 class AutoCython():
 
-    def __init__(self, compile_path='.', exclude=[], mode='f', delete=['b','p','c']):
+    def __init__(self, compile_path='.', exclude=[], mode='f', delete=['b','p','c'], python_cmd="python"):
         """[summary]
 
         [description]
             初始化编译参数
         Parameters
         ----------
         compile_path : {str}, optional
@@ -101,14 +101,15 @@
 
         # 编译后需要删除的目录
         self.delete = delete
 
         # 注意源代码里不要有build文件夹
         self._setup_file_str = '#!/use/bin/dev python\n# -*- coding: utf-8 -*-\nfrom distutils.core import setup\nfrom Cython.Build import cythonize\nsetup(ext_modules = cythonize("{0}"))'
         self._Popen_cmd = 'python {0} build_ext --inplace'
+        self._Popen_cmd = self._Popen_cmd.replace("python", python_cmd)
 
     def _fitter_path(self, path : str) -> str:
         """ 让一个路径的分隔符统一为当前系统下的 """
         return path.replace('/', self._sp).replace('\\', self._sp).rstrip(self._sp)
 
     def _get_all_file_list(self, path='.', file_type=[], file_name=[]) -> list:
         """ 获取某个目录下的某类文件或某文件名路径列表 """
@@ -471,14 +472,14 @@
 
         if self.a_file_flag:
             ac = AutoCython()
             ac._Popen_cmd = ac._Popen_cmd.replace("python", self.python_cmd)
             ac.compile_file(self.file_path, wait=True, delete=self.delete, complicating=False)
             sys.exit()
 
-        return self.compile_path, self.exclude, self.mode, self.delete
+        return self.compile_path, self.exclude, self.mode, self.delete, self.python_cmd
 
 if __name__ == '__main__':
     """ CMD """
     ac = AutoCython(*AC_getopt_argv().geto())
 
     ac.compile()
```

### Comparing `AutoCython-jianjun-1.3.2/LICENSE` & `AutoCython-jianjun-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCython-jianjun-1.3.2/setup.py` & `AutoCython-jianjun-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setup(
     name = 'AutoCython-jianjun',
-    version = '1.3.2',
+    version = '1.3.3',
     author = 'jianjun',
     author_email = '910667956@qq.com',
     url = 'https://github.com/EVA-JianJun/AutoCython',
     description = u'自动Cython，使用Cython批量编译.py文件为.pyd文件！',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = ["AutoCython"],
```

