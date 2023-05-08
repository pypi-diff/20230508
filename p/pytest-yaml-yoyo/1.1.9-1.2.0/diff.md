# Comparing `tmp/pytest-yaml-yoyo-1.1.9.tar.gz` & `tmp/pytest-yaml-yoyo-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytest-yaml-yoyo-1.1.9.tar", last modified: Tue Mar 21 06:32:04 2023, max compression
+gzip compressed data, was "dist\pytest-yaml-yoyo-1.2.0.tar", last modified: Mon May  8 00:53:51 2023, max compression
```

## Comparing `pytest-yaml-yoyo-1.1.9.tar` & `pytest-yaml-yoyo-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 06:32:03.980587 pytest-yaml-yoyo-1.1.9/
--rw-rw-rw-   0        0        0    21942 2023-03-21 06:32:03.979591 pytest-yaml-yoyo-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0    21443 2022-12-14 00:24:42.000000 pytest-yaml-yoyo-1.1.9/README.rst
--rw-rw-rw-   0        0        0       42 2023-03-21 06:32:03.980587 pytest-yaml-yoyo-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1347 2023-03-20 11:05:26.000000 pytest-yaml-yoyo-1.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-21 06:32:03.829279 pytest-yaml-yoyo-1.1.9/src/
-drwxrwxrwx   0        0        0        0 2023-03-21 06:32:03.966597 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/
--rw-rw-rw-   0        0        0        0 2022-11-23 03:54:21.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/__init__.py
--rw-rw-rw-   0        0        0     2872 2023-03-17 11:21:02.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/create_funtion.py
--rw-rw-rw-   0        0        0     2057 2022-12-13 01:48:02.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/db.py
--rw-rw-rw-   0        0        0      238 2022-12-09 13:49:56.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/exceptions.py
--rw-rw-rw-   0        0        0     3701 2023-03-20 11:05:26.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/extract.py
--rw-rw-rw-   0        0        0     2059 2022-12-13 02:02:05.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/http_session.py
--rw-rw-rw-   0        0        0     2431 2023-03-21 06:10:09.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/log.py
--rw-rw-rw-   0        0        0      991 2022-12-16 14:42:13.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/my_builtins.py
--rw-rw-rw-   0        0        0        0 2022-11-22 02:43:10.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/parser.py
--rw-rw-rw-   0        0        0     8780 2023-03-17 11:21:02.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/plugin.py
--rw-rw-rw-   0        0        0     4122 2023-03-17 11:21:02.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/render_template_obj.py
--rw-rw-rw-   0        0        0     1854 2022-12-14 00:10:53.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/report_notify.py
--rw-rw-rw-   0        0        0    24389 2023-03-21 06:10:09.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/runner.py
--rw-rw-rw-   0        0        0     7722 2023-02-15 14:36:54.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/swagger_parser.py
--rw-rw-rw-   0        0        0     3202 2023-03-21 06:20:06.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/validate.py
-drwxrwxrwx   0        0        0        0 2023-03-21 06:32:03.977566 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo.egg-info/
--rw-rw-rw-   0        0        0    21942 2023-03-21 06:32:03.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-03-21 06:32:03.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 06:32:03.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-03-21 06:32:03.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      188 2023-03-21 06:32:03.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-03-21 06:32:03.000000 pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 00:53:51.287394 pytest-yaml-yoyo-1.2.0/
+-rw-rw-rw-   0        0        0    21942 2023-05-08 00:53:51.286394 pytest-yaml-yoyo-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    21443 2022-12-14 00:24:42.000000 pytest-yaml-yoyo-1.2.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-08 00:53:51.287394 pytest-yaml-yoyo-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1347 2023-05-08 00:50:03.000000 pytest-yaml-yoyo-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 00:53:51.251592 pytest-yaml-yoyo-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 00:53:51.277442 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/
+-rw-rw-rw-   0        0        0        0 2022-11-23 03:54:21.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/__init__.py
+-rw-rw-rw-   0        0        0     2874 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/create_funtion.py
+-rw-rw-rw-   0        0        0     2057 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/db.py
+-rw-rw-rw-   0        0        0      238 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/exceptions.py
+-rw-rw-rw-   0        0        0     3741 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/extract.py
+-rw-rw-rw-   0        0        0     2059 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/http_session.py
+-rw-rw-rw-   0        0        0     2431 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/log.py
+-rw-rw-rw-   0        0        0      991 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/my_builtins.py
+-rw-rw-rw-   0        0        0        0 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/parser.py
+-rw-rw-rw-   0        0        0     8780 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/plugin.py
+-rw-rw-rw-   0        0        0     4122 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/render_template_obj.py
+-rw-rw-rw-   0        0        0     1854 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/report_notify.py
+-rw-rw-rw-   0        0        0     1447 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/request_session.py
+-rw-rw-rw-   0        0        0    26263 2023-05-08 00:53:10.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/runner.py
+-rw-rw-rw-   0        0        0     7722 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/swagger_parser.py
+-rw-rw-rw-   0        0        0     3380 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/validate.py
+drwxrwxrwx   0        0        0        0 2023-05-08 00:53:51.285397 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/
+-rw-rw-rw-   0        0        0    21942 2023-05-08 00:53:51.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      839 2023-05-08 00:53:51.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 00:53:51.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-08 00:53:51.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      188 2023-05-08 00:53:51.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-08 00:53:51.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/top_level.txt
```

### Comparing `pytest-yaml-yoyo-1.1.9/PKG-INFO` & `pytest-yaml-yoyo-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-yoyo
-Version: 1.1.9
+Version: 1.2.0
 Summary: http/https API run by yaml
 Home-page: https://github.com/yoyoketang/pytest-yaml-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,pytest-yaml-yoyo
 Classifier: Framework :: Pytest
```

### Comparing `pytest-yaml-yoyo-1.1.9/README.rst` & `pytest-yaml-yoyo-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.1.9/setup.py` & `pytest-yaml-yoyo-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 作者-上海悠悠 微信wx:283340479
 # blog地址 https://www.cnblogs.com/yoyoketang/
 """
 
 setup(
     name='pytest-yaml-yoyo',
     url='https://github.com/yoyoketang/pytest-yaml-yoyo',
-    version='v1.1.9',
+    version='v1.2.0',
     author="上海-悠悠",
     author_email='283340479@qq.com',
     description='http/https API run by yaml',
     long_description=open("README.rst", encoding='utf-8').read(),
     package_dir={"": "src"},
     packages=["pytest_yaml_yoyo"],
     classifiers=[
```

### Comparing `pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/create_funtion.py` & `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/create_funtion.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -82,8 +82,8 @@
     d.__file__ = filename
     try:
         with open(filename, "r", encoding="utf-8") as config_file:
             exec(compile(config_file.read(), filename, "exec"), d.__dict__)
     except ImportError as e:
         print("fail to read config file: {}".format(filename))
         raise e
-    return d
+    return d
```

### Comparing `pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/db.py` & `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/db.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/extract.py` & `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     :param response: Response Obj
     :param extract_expression: 取值表达式
     :return: 返回取值后的结果
     """
     if not isinstance(extract_expression, str):
         return extract_expression
     res = {
-        "headers": response.headers,
-        "cookies": dict(response.cookies)
+        "headers": response.headers if response else {},
+        "cookies": dict(response.cookies if response else {})
     }
     if extract_expression in ["status_code", "url", "ok", "encoding", "text"]:
         return getattr(response, extract_expression)
     elif extract_expression.startswith('headers') or extract_expression.startswith('cookies'):
         return extract_by_jmespath(res, extract_expression)
     elif extract_expression.startswith('body') or extract_expression.startswith('content'):
         try:
```

### Comparing `pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/http_session.py` & `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/http_session.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/log.py` & `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/log.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/my_builtins.py` & `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/my_builtins.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/plugin.py` & `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/render_template_obj.py` & `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/render_template_obj.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/report_notify.py` & `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/report_notify.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/runner.py` & `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import inspect
 import allure
 from .log import log
 from .db import ConnectMysql
 import mimetypes
 from requests_toolbelt import MultipartEncoder
 import time
+import json
 
 
 class RunYaml(object):
     """ 运行yaml """
 
     def __init__(self, raw: dict, module: types.ModuleType, g: dict):
         self.raw = raw   # 读取yaml 原始数据
@@ -65,80 +66,96 @@
             else:
                 case[case_name] = [case_value]
 
             def execute_yaml_case(args):
                 # 获取被调用函数名称
                 log.info(f'执行文件-> {self.module.__name__}.yml')
                 log.info(f'base_url-> {base_url or args.get("request").config.option.base_url}')
-                log.info(f'variables-> {self.module_variable}')
+                log.info(f'config variables-> {self.module_variable}')
                 call_function_name = inspect.getframeinfo(inspect.currentframe().f_back)[2]
                 log.info(f'运行用例-> {call_function_name}')
                 # 添加 allure 报告--> story
                 allure.dynamic.feature(f'{self.module.__name__}.yml')
 
+                # 更新 fixture 的值 到context
+                self.context.update(args)
                 for step in case[call_function_name]:
                     # 添加 allure 报告--> title
                     allure.dynamic.title(call_function_name)
                     response = None
                     api_validate = []
                     step_name = step.get('name', 'not step name')
+                    step_context = self.context.copy()  # 步骤变量
                     # 添加 allure 报告--> step
                     with allure.step(step_name):
                         pass
                     if 'validate' not in step.keys():
                         step['validate'] = []
                     for item, value in step.items():
                         # 执行用例里面的方法
                         if item == 'name':
                             pass          # noqa
+                        elif item == 'variables':    # step 步骤变量获取
+                            copy_value = copy.deepcopy(value)
+                            if not isinstance(copy_value, dict):
+                                log.error('step variables->variables must be dict type!')
+                            else:
+                                step_variables_value = render_template_obj.rend_template_any(
+                                    copy_value, **self.context
+                                )
+                                step_context.update(step_variables_value)
                         elif item == 'api':
                             root_dir = args.get('request').config.rootdir   # 内置request 获取root_dir
                             api_path = Path(root_dir).joinpath(value)
                             raw_api = yaml.safe_load(api_path.open(encoding='utf-8'))
                             api_validate = raw_api.get('validate', [])
                             copy_value = copy.deepcopy(raw_api.get('request'))  # 深拷贝一份新的value
-                            response = self.run_request(args, copy_value, config_hooks, base_url)
+                            response = self.run_request(args, copy_value, config_hooks, base_url, context=step_context)
                         elif item == 'request':
                             copy_value = copy.deepcopy(value)  # 深拷贝一份新的value
-                            response = self.run_request(args, copy_value, config_hooks, base_url)
+                            copy_config_hooks = copy.deepcopy(config_hooks)
+                            response = self.run_request(args, copy_value, copy_config_hooks, base_url, context=step_context)
                         elif item == 'extract':
                             # 提取变量
                             copy_value = copy.deepcopy(value)
-                            extract_value = render_template_obj.rend_template_any(copy_value, **self.context)
+                            extract_value = render_template_obj.rend_template_any(copy_value, **step_context)
                             extract_result = self.extract_response(response, extract_value)
-                            log.info(f'extract 提取变量-> {extract_result}')
+                            log.info(f'extract  提取变量-> {extract_result}')
                             # 添加到模块变量
                             self.module_variable.update(extract_result)
+                            # 添加到步骤变量
+                            step_context.update(extract_result)
                             if isinstance(self.module_variable, dict):
                                 self.context.update(self.module_variable)    # 加载模块变量
                         elif item == 'validate':
                             copy_value = copy.deepcopy(value)
                             # 合并校验
                             copy_value.extend([v for v in api_validate if v not in copy_value])
-                            validate_value = render_template_obj.rend_template_any(copy_value, **self.context)
+                            validate_value = render_template_obj.rend_template_any(copy_value, **step_context)
                             log.info(f'validate 校验内容-> {validate_value}')
                             self.validate_response(response, validate_value)
                         elif item == 'sleep':
-                            sleep_value = render_template_obj.rend_template_any(value, **self.context)
+                            sleep_value = render_template_obj.rend_template_any(value, **step_context)
                             try:
                                 log.info(f'sleep time: {sleep_value}')
                                 time.sleep(sleep_value)
                             except Exception as msg:
                                 log.error(f'Run error: sleep value must be int or float, error msg: {msg}')
                         elif item == 'skip':
-                            skip_reason = render_template_obj.rend_template_any(value, **self.context)
+                            skip_reason = render_template_obj.rend_template_any(value, **step_context)
                             import pytest
                             pytest.skip(skip_reason)
                         elif item == 'skipif':   # noqa
-                            if_exp = render_template_obj.rend_template_any(value, **self.context)
+                            if_exp = render_template_obj.rend_template_any(value, **step_context)
                             log.info(f'skipif : {eval(str(if_exp))}')  # noqa
                             if eval(str(if_exp)):
                                 import pytest
                                 pytest.skip(str(if_exp))
                         else:
+                            value = render_template_obj.rend_template_any(value, **step_context)
                             try:
                                 eval(item)(value)
                             except Exception as msg:
                                 raise exceptions.ParserError(f'Parsers error: {msg}') from None
 
             f = create_funtion.create_function_from_parameters(
                 func=execute_yaml_case,
@@ -151,49 +168,59 @@
 
             # 向 module 中加入函数
             setattr(self.module, str(case_name), f)
             if config_params:
                 # 向 module 中加参数化数据的属性
                 setattr(self.module, 'params_data', config_params)
 
-    def run_request(self, args, copy_value, config_hooks, base_url):
+    def run_request(self, args, copy_value, config_hooks, base_url, context=None):
         """运行request请求"""
         request_session = args.get('requests_function') or args.get('requests_module') or args.get('requests_session')
         # 加载参数化的值和fixture的值
-        self.context.update(args)
-        request_value = render_template_obj.rend_template_any(copy_value, **self.context)
+        if context is None:
+            request_value = render_template_obj.rend_template_any(copy_value, **self.context)
+        else:
+            request_value = render_template_obj.rend_template_any(copy_value, **context)
         # request 请求参数预处理
         request_pre = self.request_hooks(config_hooks, request_value)
         if request_pre:
             # 执行 pre request 预处理
-            self.context.update({"req": request_value})
-            self.run_request_hooks(request_pre, request_value)
+            if context:
+                context.update({"req": request_value})
+            else:
+                self.context.update({"req": request_value})
+            self.run_request_hooks(request_pre, request_value, context=context)
         # request请求 带上hooks "response"参数
         self.response_hooks(config_hooks, request_value)
 
         # multipart/form-data 文件上传支持
         root_dir = args.get('request').config.rootdir  # 内置request 获取root_dir
         request_value = self.multipart_encoder_request(request_value, root_dir)
 
-        log.info(f'--------  request info ----------\n'
-                 f'{request_value.get("method", "")} {request_value.get("url", "")}\n'
-                 f'{request_value}\n'
-                 )
-
+        log.info(f'--------  request info ----------')
+        log.info(f'raw    -> {request_value}')
+        log.debug(f'method -> {request_value.get("method", "")}')
+        log.debug(f'url    -> {request_value.get("url", "")}')
+        request_headers = request_session.headers
+        if request_value.get("headers", {}):
+            request_headers.update(request_value.get("headers", {}))
+        log.debug(f'headers-> {request_headers}')
+        if request_value.get('json'):
+            log.debug(f'json   -> {json.dumps(request_value.get("json", {}))}')
+        else:
+            log.debug(f'data   -> {request_value.get("data", {})}')
         response = request_session.send_request(
             base_url=base_url,
             **request_value
         )
-
-        log.info(f'------  response info  {getattr(response, "status_code")} {getattr(response, "reason", "")}  '
-                 f'{getattr(response, "elapsed", "").total_seconds() if getattr(response, "elapsed", "") else ""}s'
-                 f'------\n url: {getattr(response, "url", "")} \n'
-                 f'headers:\n     {getattr(response, "headers", "")}\n'
-                 f'body:\n     {getattr(response, "text", "")}\n'
-                 )
+        log.info(f'------  response info  {getattr(response, "status_code")} {getattr(response, "reason", "")}')
+        log.info(f'耗时: {getattr(response, "elapsed", "").total_seconds() if getattr(response, "elapsed", "") else ""}s')
+        log.debug(f'url: {getattr(response, "url", "")}')
+        log.debug(f'headers:{getattr(response, "headers", "")}')
+        log.info(f'text:  {getattr(response, "text", "")}')
         return response
 
     @staticmethod
     def function_parameters(config_fixtures) -> list:
         """ 测试函数传 fixture """
         # 测试函数的默认请求参数
         function_parameters = [
@@ -318,41 +345,44 @@
         if 'request' in config_hooks.keys():
             config_request_hooks = config_hooks.get('request')
             if isinstance(config_request_hooks, str):
                 # 字符串切成list
                 config_request_hooks = [item.strip(" ") for item in config_request_hooks.split(',')]
         req_request_hooks = request_value.get('hooks', {})
         if 'request' in req_request_hooks.keys():
-            req_hooks = req_request_hooks.get('request')
+            req_hooks = req_request_hooks.pop('request')
             if isinstance(req_hooks, str):
                 # 字符串切成list
                 req_hooks = [item.strip(" ") for item in req_hooks.split(',')]
             for h in req_hooks:
                 config_request_hooks.append(h)
         # 更新 request_value
         if config_request_hooks:
             hooks = self.hooks_event({'request': config_request_hooks})
             # 去掉值为空的response 事件
             new_hooks = {key: value for key, value in hooks.items() if value}
             return new_hooks
         return {'request': []}
 
-    def run_request_hooks(self, request_pre: dict, request_value):
+    def run_request_hooks(self, request_pre: dict, request_value, context=None):
         """执行请求预处理hooks内容
         request_pre: 待执行的预处理函数
         """
         funcs = request_pre.get('request', [])
         if not funcs:
             return request_value
         import inspect
         for fun in funcs:
             # 获取函数对象的入参
             ars = [arg_name for arg_name, v in inspect.signature(fun).parameters.items()]
             if 'req' in ars:
-                fun(self.context.get('req'))
+                if context:
+                    fun(context.get('req'))
+                else:
+                    fun(self.context.get('req'))
             else:
                 fun()
         return request_value
 
     def response_hooks(self, config_hooks: dict, request_value: dict) -> dict:
         """ 合并全局config_hooks 和 单个请求 hooks 参数
             config_hooks = {
@@ -388,15 +418,15 @@
             # 去掉值为空的response 事件
             new_hooks = {key: value for key, value in hooks.items() if value}
             request_value['hooks'] = new_hooks
         return request_value
 
     @staticmethod
     def extract_response(response, extract_obj: dict):
-        """提取返回结果, 添加到module_variable 模块变量"""
+        """extract 提取返回结果"""
         extract_result = {}
         if isinstance(extract_obj, dict):
             for extract_var, extract_expression in extract_obj.items():
                 extract_var_value = extract.extract_by_object(response, extract_expression)  # 实际结果
                 extract_result[extract_var] = extract_var_value
             return extract_result
         else:
@@ -434,15 +464,15 @@
                     validate.length_less_than_or_equals(actual_value, expect_value)
                 elif check_type in ["contains"]:
                     validate.contains(actual_value, expect_value)
                 else:
                     if hasattr(validate, check_type):
                         getattr(validate, check_type)(actual_value, expect_value)
                     else:
-                        print(f'{check_type}  not valid check type')
+                        log.error(f'{check_type}  not valid check type')
 
     def execute_mysql(self):
         """执行 mysql 操作"""
         env_obj = self.g.get('env')    # 获取环境配置
         if not hasattr(env_obj, 'MYSQL_HOST'):
             return {
                 "query_sql": lambda x: log.error("MYSQL_HOST not found in config.py"),
```

### Comparing `pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/swagger_parser.py` & `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo/validate.py` & `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/validate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 Built-in validate comparators.
 """
 import re
 
 
 def equals(check_value, expect_value):
-    assert check_value == expect_value, f'{check_value} == {expect_value})'
+    check_value = None if check_value == 'None' else check_value
+    expect_value = None if expect_value == 'None' else expect_value
+    assert check_value == expect_value, f'{check_value}->{type(check_value)} == {expect_value}->{type(expect_value)})'
 
 
 def less_than(check_value, expect_value):
     assert check_value < expect_value, f'{check_value} < {expect_value})'
 
 
 def less_than_or_equals(check_value, expect_value):
```

### Comparing `pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo.egg-info/PKG-INFO` & `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-yoyo
-Version: 1.1.9
+Version: 1.2.0
 Summary: http/https API run by yaml
 Home-page: https://github.com/yoyoketang/pytest-yaml-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,pytest-yaml-yoyo
 Classifier: Framework :: Pytest
```

### Comparing `pytest-yaml-yoyo-1.1.9/src/pytest_yaml_yoyo.egg-info/SOURCES.txt` & `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/pytest_yaml_yoyo/http_session.py
 src/pytest_yaml_yoyo/log.py
 src/pytest_yaml_yoyo/my_builtins.py
 src/pytest_yaml_yoyo/parser.py
 src/pytest_yaml_yoyo/plugin.py
 src/pytest_yaml_yoyo/render_template_obj.py
 src/pytest_yaml_yoyo/report_notify.py
+src/pytest_yaml_yoyo/request_session.py
 src/pytest_yaml_yoyo/runner.py
 src/pytest_yaml_yoyo/swagger_parser.py
 src/pytest_yaml_yoyo/validate.py
 src/pytest_yaml_yoyo.egg-info/PKG-INFO
 src/pytest_yaml_yoyo.egg-info/SOURCES.txt
 src/pytest_yaml_yoyo.egg-info/dependency_links.txt
 src/pytest_yaml_yoyo.egg-info/entry_points.txt
```

