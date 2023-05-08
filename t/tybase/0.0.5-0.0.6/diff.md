# Comparing `tmp/tybase-0.0.5.tar.gz` & `tmp/tybase-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tybase-0.0.5.tar", last modified: Mon May  8 08:52:20 2023, max compression
+gzip compressed data, was "tybase-0.0.6.tar", last modified: Mon May  8 10:39:26 2023, max compression
```

## Comparing `tybase-0.0.5.tar` & `tybase-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 08:52:20.863182 tybase-0.0.5/
--rw-rw-rw-   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.0.5/MANIFEST.in
--rw-r--r--   0 zhangte    (501) staff       (20)      624 2023-05-08 08:52:20.862877 tybase-0.0.5/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      156 2023-05-08 08:46:36.000000 tybase-0.0.5/README.md
--rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-05-08 08:52:20.863308 tybase-0.0.5/setup.cfg
--rw-rw-rw-   0 zhangte    (501) staff       (20)      793 2023-05-08 08:52:12.000000 tybase-0.0.5/setup.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 08:52:20.836342 tybase-0.0.5/tybase/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.0.5/tybase/__init__.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 08:52:20.839189 tybase-0.0.5/tybase/baidu/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.0.5/tybase/baidu/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4126 2023-05-05 10:37:20.000000 tybase-0.0.5/tybase/baidu/kw_tool.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.0.5/tybase/datatest.txt
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 08:52:20.854578 tybase-0.0.5/tybase/lc/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.0.5/tybase/lc/__init__.py
--rw-r--r--   0 zhangte    (501) staff       (20)     2421 2023-05-08 08:46:18.000000 tybase-0.0.5/tybase/lc/eg1.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.0.5/tybase/tytest.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 08:52:20.838543 tybase-0.0.5/tybase.egg-info/
--rw-rw-rw-   0 zhangte    (501) staff       (20)      624 2023-05-08 08:52:20.000000 tybase-0.0.5/tybase.egg-info/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      323 2023-05-08 08:52:20.000000 tybase-0.0.5/tybase.egg-info/SOURCES.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)        1 2023-05-08 08:52:20.000000 tybase-0.0.5/tybase.egg-info/dependency_links.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)       20 2023-05-08 08:52:20.000000 tybase-0.0.5/tybase.egg-info/requires.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)        7 2023-05-08 08:52:20.000000 tybase-0.0.5/tybase.egg-info/top_level.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 10:39:26.002058 tybase-0.0.6/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.0.6/MANIFEST.in
+-rw-r--r--   0 zhangte    (501) staff       (20)      609 2023-05-08 10:39:26.001777 tybase-0.0.6/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      156 2023-05-08 08:46:36.000000 tybase-0.0.6/README.md
+-rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-05-08 10:39:26.002177 tybase-0.0.6/setup.cfg
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      778 2023-05-08 10:38:38.000000 tybase-0.0.6/setup.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 10:39:25.948550 tybase-0.0.6/tybase/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.0.6/tybase/__init__.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 10:39:25.952005 tybase-0.0.6/tybase/baidu/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.0.6/tybase/baidu/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4126 2023-05-05 10:37:20.000000 tybase-0.0.6/tybase/baidu/kw_tool.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.0.6/tybase/datatest.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 10:39:25.968680 tybase-0.0.6/tybase/lc/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.0.6/tybase/lc/__init__.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.0.6/tybase/lc/eg1.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.0.6/tybase/tytest.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 10:39:25.951270 tybase-0.0.6/tybase.egg-info/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      609 2023-05-08 10:39:25.000000 tybase-0.0.6/tybase.egg-info/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      323 2023-05-08 10:39:25.000000 tybase-0.0.6/tybase.egg-info/SOURCES.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        1 2023-05-08 10:39:25.000000 tybase-0.0.6/tybase.egg-info/dependency_links.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)       20 2023-05-08 10:39:25.000000 tybase-0.0.6/tybase.egg-info/requires.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        7 2023-05-08 10:39:25.000000 tybase-0.0.6/tybase.egg-info/top_level.txt
```

### Comparing `tybase-0.0.5/PKG-INFO` & `tybase-0.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.0.5
-Summary: 新增lc.eg1,用于协助llm生成prompt
+Version: 0.0.6
+Summary: 封装eg1,成为一个类
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `tybase-0.0.5/setup.py` & `tybase-0.0.6/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tybase',
-    version='0.0.5',
+    version='0.0.6',
     include_package_data=True,
-    description='新增lc.eg1,用于协助llm生成prompt',
+    description='封装eg1,成为一个类',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',  # 版本描述
     author='Tuya',
     author_email='353335447@qq.com',
     url='https://github.com/yourusername/your_package',
     packages=find_packages(),
     install_requires=[
```

### Comparing `tybase-0.0.5/tybase/baidu/kw_tool.py` & `tybase-0.0.6/tybase/baidu/kw_tool.py`

 * *Files identical despite different names*

### Comparing `tybase-0.0.5/tybase/lc/eg1.py` & `tybase-0.0.6/tybase/lc/eg1.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,82 +2,84 @@
 from langchain import PromptTemplate, LLMChain
 from langchain.prompts.chat import (
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
 )
 # 这就是我们依次运行这两条链的整体链。
 from langchain.chains import SequentialChain
-
-import os
 import json
 
 
-# 获取角色的Chain
-def chain_role():
-    prompt_base = """
-    [机器人信息]:
-    ```
-    {prompt_info}\n
-    {desc}
-    ```
-
-    通过以上的[角色信息],我应该用什么样的格式向这个机器人输入内容? 可以把输入的内容举{num}个例子,每个例子的长度不要超过中文20个汉字,示例如下:
-
-    输入示例: xxx
-
-    不用返回机器人回复,只需要输出[输入示例]的内容即可
-
-    """
-
-    human_message_prompt = HumanMessagePromptTemplate(
-        prompt=PromptTemplate(
-            template=prompt_base,
-            input_variables=["prompt_info", "desc", "num"],
+class GetPrompt():
+    def __init__(self, openai_api_key, role_temperature: float = 0.3):
+        self.openai_api_key = openai_api_key
+        self.role_temperature = role_temperature
+
+    def chain_role(self):
+        prompt_base = """
+            [机器人信息]:
+            ```
+            {prompt_info}\n
+            {desc}
+            ```
+        
+            通过以上的[角色信息],我应该用什么样的格式向这个机器人输入内容? 可以把输入的内容举{num}个例子,每个例子的长度不要超过中文20个汉字,示例如下:
+        
+            输入示例: xxx
+        
+            不用返回机器人回复,只需要输出[输入示例]的内容即可
+        
+            """
+
+        human_message_prompt = HumanMessagePromptTemplate(
+            prompt=PromptTemplate(
+                template=prompt_base,
+                input_variables=["prompt_info", "desc", "num"],
+            )
         )
-    )
-
-    chat_prompt_template = ChatPromptTemplate.from_messages([human_message_prompt])
-    return LLMChain(llm=ChatOpenAI(temperature=0.3), prompt=chat_prompt_template, output_key="example")
-
-
-def chain_json():
-    prompt_json = """
-    请提取下面文本中的所有"输入示例"里面的**内容**,返回成一个list,可以直接用json解析
-
-    ```
-    {example}
-    ```
 
-    """
-
-    human_message_prompt = HumanMessagePromptTemplate(
-        prompt=PromptTemplate(
-            template=prompt_json,
-            input_variables=["example"],
+        chat_prompt_template = ChatPromptTemplate.from_messages([human_message_prompt])
+        return LLMChain(llm=ChatOpenAI(temperature=self.role_temperature, openai_api_key=self.openai_api_key),
+                        prompt=chat_prompt_template, output_key="example")
+
+    def chain_json(self):
+        prompt_json = """
+        请提取下面文本中的所有"输入示例"里面的**内容**,返回成一个list,可以直接用json解析
+    
+        ```
+        {example}
+        ```
+    
+        """
+
+        human_message_prompt = HumanMessagePromptTemplate(
+            prompt=PromptTemplate(
+                template=prompt_json,
+                input_variables=["example"],
+            )
         )
-    )
-
-    chat_prompt_template = ChatPromptTemplate.from_messages([human_message_prompt])
-    return LLMChain(llm=ChatOpenAI(temperature=0), prompt=chat_prompt_template, output_key="example_json")
-
 
-def get_prompt_eg(prompt, desc, num=4):
-    """
-
-    :param prompt: 系统设定的指令
-    :param desc:   系统设定的描述语
-    :param num:    需要生成的指令数量
-    :return:       ( json )的str,需要自己再解析一下
-    """
-    overall_chain = SequentialChain(
-        chains=[chain_role(), chain_json()],
-        input_variables=["prompt_info", "desc", "num"],
-        # Here we return multiple variables
-        output_variables=["example", "example_json"],
-        verbose=True)
+        chat_prompt_template = ChatPromptTemplate.from_messages([human_message_prompt])
+        return LLMChain(llm=ChatOpenAI(temperature=0, openai_api_key=self.openai_api_key),
+                        prompt=chat_prompt_template, output_key="example_json")
+
+    def main(self, prompt, desc, num=4):
+        """
+
+        :param prompt: 系统设定的指令
+        :param desc:   系统设定的描述语
+        :param num:    需要生成的指令数量
+        :return:       ( json )的str,需要自己再解析一下
+        """
+        overall_chain = SequentialChain(
+            chains=[self.chain_role(), self.chain_json()],
+            input_variables=["prompt_info", "desc", "num"],
+            # Here we return multiple variables
+            output_variables=["example", "example_json"],
+            verbose=True)
 
-    inputs = {"prompt_info": prompt, "desc": desc, "num": num}  # 参数传递就这样传递
-    return json.loads(overall_chain(inputs)["example_json"])
+        inputs = {"prompt_info": prompt, "desc": desc, "num": num}  # 参数传递就这样传递
+        return json.loads(overall_chain(inputs)["example_json"])
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `tybase-0.0.5/tybase.egg-info/PKG-INFO` & `tybase-0.0.6/tybase.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.0.5
-Summary: 新增lc.eg1,用于协助llm生成prompt
+Version: 0.0.6
+Summary: 封装eg1,成为一个类
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

