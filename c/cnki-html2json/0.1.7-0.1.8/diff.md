# Comparing `tmp/cnki_html2json-0.1.7.tar.gz` & `tmp/cnki_html2json-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnki_html2json-0.1.7.tar", last modified: Sat May  6 17:11:00 2023, max compression
+gzip compressed data, was "cnki_html2json-0.1.8.tar", last modified: Mon May  8 08:03:51 2023, max compression
```

## Comparing `cnki_html2json-0.1.7.tar` & `cnki_html2json-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:11:00.791724 cnki_html2json-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-06 17:10:44.000000 cnki_html2json-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-06 17:11:00.791724 cnki_html2json-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-06 17:10:44.000000 cnki_html2json-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:11:00.791724 cnki_html2json-0.1.7/cnki_html2json/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-06 17:10:44.000000 cnki_html2json-0.1.7/cnki_html2json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-06 17:10:44.000000 cnki_html2json-0.1.7/cnki_html2json/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-05-06 17:10:44.000000 cnki_html2json-0.1.7/cnki_html2json/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-06 17:10:44.000000 cnki_html2json-0.1.7/cnki_html2json/html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-06 17:10:44.000000 cnki_html2json-0.1.7/cnki_html2json/parse_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-06 17:10:44.000000 cnki_html2json-0.1.7/cnki_html2json/recognize_slider_coordinate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:11:00.791724 cnki_html2json-0.1.7/cnki_html2json.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-06 17:11:00.000000 cnki_html2json-0.1.7/cnki_html2json.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-06 17:11:00.000000 cnki_html2json-0.1.7/cnki_html2json.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 17:11:00.000000 cnki_html2json-0.1.7/cnki_html2json.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-06 17:11:00.000000 cnki_html2json-0.1.7/cnki_html2json.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 17:11:00.000000 cnki_html2json-0.1.7/cnki_html2json.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 17:11:00.000000 cnki_html2json-0.1.7/cnki_html2json.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 17:11:00.791724 cnki_html2json-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-06 17:10:44.000000 cnki_html2json-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:11:00.791724 cnki_html2json-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-06 17:10:44.000000 cnki_html2json-0.1.7/tests/test_html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-06 17:10:44.000000 cnki_html2json-0.1.7/tests/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:03:51.173741 cnki_html2json-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-08 08:03:51.173741 cnki_html2json-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:03:51.173741 cnki_html2json-0.1.8/cnki_html2json/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/cnki_html2json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/cnki_html2json/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/cnki_html2json/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/cnki_html2json/html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/cnki_html2json/parse_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/cnki_html2json/recognize_slider_coordinate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:03:51.173741 cnki_html2json-0.1.8/cnki_html2json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-08 08:03:51.000000 cnki_html2json-0.1.8/cnki_html2json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-08 08:03:51.000000 cnki_html2json-0.1.8/cnki_html2json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:03:51.000000 cnki_html2json-0.1.8/cnki_html2json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 08:03:51.000000 cnki_html2json-0.1.8/cnki_html2json.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 08:03:51.000000 cnki_html2json-0.1.8/cnki_html2json.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 08:03:51.000000 cnki_html2json-0.1.8/cnki_html2json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:03:51.173741 cnki_html2json-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:03:51.173741 cnki_html2json-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/tests/test_html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/tests/test_metadata.py
```

### Comparing `cnki_html2json-0.1.7/LICENSE` & `cnki_html2json-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.7/PKG-INFO` & `cnki_html2json-0.1.8/cnki_html2json.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cnki_html2json
-Version: 0.1.7
+Name: cnki-html2json
+Version: 0.1.8
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Intended Audience :: Developers
@@ -22,14 +22,15 @@
 License-File: LICENSE
 
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
 
 最近更新：  
+- `v0.1.8` 优化爬虫策略，适当提高了爬取速度；
 - `v0.1.5` 对解析论文html的方式进行重构，提高了解析的准确率；
 
 核心功能：
 - 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
 - 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
 - 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
   - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
@@ -96,15 +97,15 @@
 | -m | --mode | 模式，可选值为 `raw(default)`、`structure`、`plain`|
 | -b | --browser | 浏览器类型，可选值为 `Chrome(default)`、`Edge`、`Firefox`|
 | -save | --save_path | 下载文件的保存路径，默认为当前目录的 `dataset` 文件夹 |
 | -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
 | -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，</br>日志将保存在 `save_path` 下的 `log` 文件夹中 |
 
 > 如果未指定保存路径，将下载结果默认保存在当前目录下的 `dataset` 文件夹下;  
-> 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (自动过滑块验证)
+> 由于提取的是文献正文，1分钟大概能下载4篇文献，可以放到夜间运行 (自动过滑块验证)
 
 ```python
 # 也可以在代码中调用爬虫，可选参数参考上方的参数说明
 from cnki_html2json.crawl import start_crawl
 start_crawl(start_paper_index=1,end_paper_index=100,mode='raw',log=True)
 ```
```

### Comparing `cnki_html2json-0.1.7/README.md` & `cnki_html2json-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
 
 最近更新：  
+- `v0.1.8` 优化爬虫策略，适当提高了爬取速度；
 - `v0.1.5` 对解析论文html的方式进行重构，提高了解析的准确率；
 
 核心功能：
 - 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
 - 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
 - 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
   - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
@@ -73,15 +74,15 @@
 | -m | --mode | 模式，可选值为 `raw(default)`、`structure`、`plain`|
 | -b | --browser | 浏览器类型，可选值为 `Chrome(default)`、`Edge`、`Firefox`|
 | -save | --save_path | 下载文件的保存路径，默认为当前目录的 `dataset` 文件夹 |
 | -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
 | -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，</br>日志将保存在 `save_path` 下的 `log` 文件夹中 |
 
 > 如果未指定保存路径，将下载结果默认保存在当前目录下的 `dataset` 文件夹下;  
-> 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (自动过滑块验证)
+> 由于提取的是文献正文，1分钟大概能下载4篇文献，可以放到夜间运行 (自动过滑块验证)
 
 ```python
 # 也可以在代码中调用爬虫，可选参数参考上方的参数说明
 from cnki_html2json.crawl import start_crawl
 start_crawl(start_paper_index=1,end_paper_index=100,mode='raw',log=True)
 ```
```

### Comparing `cnki_html2json-0.1.7/cnki_html2json/cli.py` & `cnki_html2json-0.1.8/cnki_html2json/cli.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.7/cnki_html2json/crawl.py` & `cnki_html2json-0.1.8/cnki_html2json/crawl.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.support.wait import WebDriverWait
+import requests
 import time
 import os
 import json
 import random
 import sys
 import math
 from loguru import logger
@@ -34,33 +35,43 @@
         x = recognize_slider_coordinate.recognize_slider(back_img_str, cut_img_str)[0]
 
         slider = driver.find_element(By.XPATH, "/html/body/div/div/div/div[2]/div/div[2]/div/div")
         ActionChains(driver).drag_and_drop_by_offset(slider, x*1.29, 0).perform()
         time.sleep(5)
     return recogize_count
 
-def obtain_paper_html(paper_url:str,driver,mode:str)->dict:
+def obtain_paper_html(url_index:int,url:str,mode:str,session,driver)->dict:
     """获取论文的html页面,返回全部内容"""
 
-    driver.execute_script("window.open('about:blank', '_blank');")
-    # 获取所有窗口的句柄
-    handles = driver.window_handles
-    driver.switch_to.window(handles[-1])
-    driver.get(paper_url)
-    time.sleep(3)
-
-    metadata_html = driver.page_source
-    metadata = parse_metadata.Parse(metadata_html).extract_metadata()
+    paper_metadata = session.get(url).text
+    metadata = parse_metadata.Parse(paper_metadata).extract_metadata()
     
     # 点击进入html页面
     try:
-        driver.find_element(By.XPATH,'//*[@id="DownLoadParts"]/div[2]/ul/li[2]/a').click()
+        driver.find_element(By.XPATH,f'//tbody/tr[{url_index}]/td[@class="operat"]/a[@class="icon-html"]').click()
     except:
         logger.error('论文未提供html页面')
         return concat_content(metadata,{'body_text':None,'citation':None})
+
+    # driver.execute_script("window.open('about:blank', '_blank');")
+    # 获取所有窗口的句柄
+        # handles = driver.window_handles
+        # driver.switch_to.window(handles[-1])
+    # driver.get(paper_url)
+    # time.sleep(3)
+
+    # metadata_html = driver.page_source
+    # metadata = parse_metadata.Parse(metadata_html).extract_metadata()
+    
+    # 点击进入html页面
+    # try:
+    #     driver.find_element(By.XPATH,'//*[@id="DownLoadParts"]/div[2]/ul/li[2]/a').click()
+    # except:
+    #     logger.error('论文未提供html页面')
+    #     return concat_content(metadata,{'body_text':None,'citation':None})
     
     else:
         handles = driver.window_handles
         driver.switch_to.window(handles[-1])
         # time.sleep(10)
         # 将固定等待10s改为动态等待，直到页面加载完成
         wait = WebDriverWait(driver, 15, 1)
@@ -71,21 +82,20 @@
         recogize_count = process_slider(driver)
         
         if recogize_count > 0:
             logger.info(f'验证码识别{recogize_count}次后通过')
 
         paper_raw_html = driver.page_source
         paper_dict = html2json.ExtractContent(paper_raw_html).extract(mode)
-        driver.close()
+        driver.close() # 关闭当前窗口
+        driver.switch_to.window(handles[0]) # 切换回原窗口
+        
         if not paper_dict:
             logger.error('无法解析html页面')
         return concat_content(metadata,paper_dict) # type: ignore
-      
-    finally:
-        driver.switch_to.window(handles[0]) 
 
 def concat_content(metadata,paper_dict:dict)->dict:
     """将论文的元数据和正文内容合并"""
     return {**metadata,**paper_dict}
 
 def jump_page(current_page:int,start_page:int,driver):
     """
@@ -107,16 +117,15 @@
             break
         
         else:
             driver.execute_script('window.scrollTo(0,0)')
             driver.find_element(By.XPATH,f'//a[@id="page{visible_page_index[-1]}"]').click()
             time.sleep(3)
             current_page = visible_page_index[-1]
-
-        
+     
 def start_crawl(start_paper_index=1,end_paper_index=None,mode='raw',browser_type='Chrome',log=True,save_path='dataset',wait_time=120):
     """爬取cnki网站的论文
     start_paper_index: 开始爬取的论文索引，默认为1
     end_paper_index: 结束爬取的论文索引，默认为None，即爬取到最后
     mode: 模式，structure|plain|raw，默认为raw
     save_path: 下载文件的保存路径，默认为当前目录的<dataset>文件夹
     log: 是否保存日志，默认为True
@@ -150,18 +159,15 @@
     # 启动浏览器
     if browser_type=='Chrome':
         driver = webdriver.Chrome()
     elif browser_type=='Firefox':
         driver = webdriver.Firefox()
     elif browser_type=='Edge':
         driver = webdriver.Edge()
-    # elif browser_type=='Safari':
-    #     driver = webdriver.Safari()
     else:
-        logger.error('不支持的浏览器类型')
         raise ValueError('请选用合适的浏览器，程序已退出')
 
     logger.info(f'已启动 {browser_type} 浏览器')
     driver.get('https://kns.cnki.net/kns8/AdvSearch')
     
     # 完成检索的等待时间
     time.sleep(wait_time)
@@ -181,76 +187,86 @@
         avaiable_records_num = min([total_records_num,end_paper_index,6000])
     else:
         avaiable_records_num = min([total_records_num,6000])
     
     need_download_num = avaiable_records_num-start_paper_index+1
     logger.info(f'总文献数量 {total_records_num}; 可下载到第 {avaiable_records_num} 篇' )
     
-    start_page = start_paper_index//papers_per_page+1
+    if start_paper_index%papers_per_page==0:
+        start_page = start_paper_index//papers_per_page
+    else:
+        start_page = start_paper_index//papers_per_page+1
     
     # 总页数
     # total_page_num = int(driver.find_element(By.XPATH,'//*[@id="countPageDiv"]/span[2]').text.split('/')[1])
     # print(f'总页数{total_page_num}')
     
     # 跳转到指定开始页面
     current_page = int(driver.find_element(By.XPATH,'//*[@id="countPageDiv"]/span[2]').text.split('/')[0])
     if current_page < start_page:
         jump_page(current_page,start_page,driver)
         current_page = start_page
     logger.info(f'将从第 {start_paper_index} 篇文献开始下载')
     logger.info(f'模式设置为 {mode}')
-    minutes = math.ceil(need_download_num/3)
+    minutes = math.ceil(need_download_num/4)
     if minutes < 60:
         logger.info(f'预计耗时 {minutes} 分钟')
     else:
         logger.info(f'预计耗时 {minutes//60} 小时 {minutes%60} 分钟')
     
     # 下载文献数据
+    session = requests.Session()
     current_paper_index = start_paper_index
     visited_urls = set()
     while current_paper_index < avaiable_records_num+1:
-        current_url_list = obtain_page_papers_url(driver)[current_paper_index%papers_per_page-1:]  
-        for url in current_url_list:
+
+        if current_paper_index%papers_per_page==0:
+            current_url_list = obtain_page_papers_url(driver)[papers_per_page-1:]
+            start = papers_per_page
+        else:
+            current_url_list = obtain_page_papers_url(driver)[current_paper_index%papers_per_page-1:]  
+            start = current_paper_index%papers_per_page
+            
+        for url_index, url in enumerate(current_url_list,start=start):
             
             # 避免重复下载
             if url in visited_urls:
-                logger.error(f'已下载过 {url}')
+                logger.info(f'已下载过 {url}')
+                current_paper_index += 1
                 continue
             else:
                 visited_urls.add(url)
 
-            paper_content = obtain_paper_html(url,driver,mode)
+            paper_content = obtain_paper_html(url_index,url,mode,session,driver)
             if paper_content['body_text'] is not None:
                 with open(f'{save_path}/{current_paper_index}.json','w',encoding='utf-8') as f:
                     json.dump(paper_content,f,ensure_ascii=False,indent=4)
-                    logger.info(f'success {current_paper_index} {paper_content["metadata"]["title"]}')
+                    logger.info(f'success {current_paper_index} {url_index} {paper_content["metadata"]["title"]}')
             else:
-                logger.error(f'fail {current_paper_index} {paper_content["metadata"]["title"]}')
+                logger.error(f'fail {current_paper_index} {url_index} {paper_content["metadata"]["title"]}')
             time.sleep(random.randint(3,5))
             current_paper_index += 1
         
             if current_paper_index == avaiable_records_num+1:
                 logger.info('下载完成')
                 driver.quit()
                 sys.exit()
                 
         logger.info(f'第 {current_page} 页下载完成')
         
         # 点击下一页
         driver.find_element(By.ID,'PageNext').click()
 
-        time.sleep(5)
-
+        # time.sleep(5)
         # 关闭第一页之外的其他窗口
-        handles = driver.window_handles
-        for i in range(1,len(handles)):
-            driver.switch_to.window(handles[i])
-            time.sleep(1)
-            driver.close()
-    
-        driver.switch_to.window(handles[0])
-        time.sleep(60)
+        # handles = driver.window_handles
+        # for i in range(1,len(handles)):
+        #     driver.switch_to.window(handles[i])
+        #     time.sleep(1)
+        #     driver.close()
+        # driver.switch_to.window(handles[0])
+        wait_seconds = random.randint(60,120)
+        logger.info(f'等待 {wait_seconds} 秒')
+        time.sleep(wait_seconds)
         current_page += 1
-
-        if current_page%100 == 0:
-            time.sleep(300)
-            
+        # if current_page%100 == 0:
+        #     time.sleep(300)
```

### Comparing `cnki_html2json-0.1.7/cnki_html2json/html2json.py` & `cnki_html2json-0.1.8/cnki_html2json/html2json.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.7/cnki_html2json/parse_metadata.py` & `cnki_html2json-0.1.8/cnki_html2json/parse_metadata.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.7/cnki_html2json/recognize_slider_coordinate.py` & `cnki_html2json-0.1.8/cnki_html2json/recognize_slider_coordinate.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.7/cnki_html2json.egg-info/PKG-INFO` & `cnki_html2json-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cnki-html2json
-Version: 0.1.7
+Name: cnki_html2json
+Version: 0.1.8
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Intended Audience :: Developers
@@ -22,14 +22,15 @@
 License-File: LICENSE
 
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
 
 最近更新：  
+- `v0.1.8` 优化爬虫策略，适当提高了爬取速度；
 - `v0.1.5` 对解析论文html的方式进行重构，提高了解析的准确率；
 
 核心功能：
 - 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
 - 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
 - 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
   - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
@@ -96,15 +97,15 @@
 | -m | --mode | 模式，可选值为 `raw(default)`、`structure`、`plain`|
 | -b | --browser | 浏览器类型，可选值为 `Chrome(default)`、`Edge`、`Firefox`|
 | -save | --save_path | 下载文件的保存路径，默认为当前目录的 `dataset` 文件夹 |
 | -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
 | -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，</br>日志将保存在 `save_path` 下的 `log` 文件夹中 |
 
 > 如果未指定保存路径，将下载结果默认保存在当前目录下的 `dataset` 文件夹下;  
-> 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (自动过滑块验证)
+> 由于提取的是文献正文，1分钟大概能下载4篇文献，可以放到夜间运行 (自动过滑块验证)
 
 ```python
 # 也可以在代码中调用爬虫，可选参数参考上方的参数说明
 from cnki_html2json.crawl import start_crawl
 start_crawl(start_paper_index=1,end_paper_index=100,mode='raw',log=True)
 ```
```

### Comparing `cnki_html2json-0.1.7/setup.py` & `cnki_html2json-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name="cnki_html2json",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.1.7",
+    version="0.1.8",
     description="A package to convert cnki html to json",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["cnki","text-structure","crawler"],
     license="MIT",
     url="https://github.com/doublessay/cnki-html2json",
     packages=["cnki_html2json"],
```

### Comparing `cnki_html2json-0.1.7/tests/test_html2json.py` & `cnki_html2json-0.1.8/tests/test_html2json.py`

 * *Files identical despite different names*

