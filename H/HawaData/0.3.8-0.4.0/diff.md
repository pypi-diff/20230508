# Comparing `tmp/HawaData-0.3.8.tar.gz` & `tmp/HawaData-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.3.8.tar", last modified: Fri May  5 09:22:50 2023, max compression
+gzip compressed data, was "HawaData-0.4.0.tar", last modified: Mon May  8 13:08:22 2023, max compression
```

## Comparing `HawaData-0.3.8.tar` & `HawaData-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:22:50.280458 HawaData-0.3.8/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:22:50.275068 HawaData-0.3.8/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2250 2023-05-05 09:22:50.000000 HawaData-0.3.8/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      484 2023-05-05 09:22:50.000000 HawaData-0.3.8/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-05 09:22:50.000000 HawaData-0.3.8/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-05 09:22:50.000000 HawaData-0.3.8/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2250 2023-05-05 09:22:50.280193 HawaData-0.3.8/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.3.8/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:22:50.275602 HawaData-0.3.8/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.3.8/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:22:50.276708 HawaData-0.3.8/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.3.8/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.3.8/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.3.8/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.3.8/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:22:50.277807 HawaData-0.3.8/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.3.8/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     8901 2023-05-05 09:20:15.000000 HawaData-0.3.8/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5177 2023-05-05 08:28:22.000000 HawaData-0.3.8/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.3.8/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.3.8/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:22:50.278714 HawaData-0.3.8/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.3.8/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.3.8/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.3.8/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:22:50.279570 HawaData-0.3.8/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.3.8/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    22995 2023-05-05 09:08:17.000000 HawaData-0.3.8/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.3.8/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-05 09:22:50.280532 HawaData-0.3.8/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.3.8/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:22:50.279853 HawaData-0.3.8/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.3.8/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-08 13:08:22.203111 HawaData-0.4.0/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-08 13:08:22.192704 HawaData-0.4.0/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2278 2023-05-08 13:08:22.000000 HawaData-0.4.0/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      484 2023-05-08 13:08:22.000000 HawaData-0.4.0/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-08 13:08:22.000000 HawaData-0.4.0/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-08 13:08:22.000000 HawaData-0.4.0/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2278 2023-05-08 13:08:22.202600 HawaData-0.4.0/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.4.0/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-08 13:08:22.193224 HawaData-0.4.0/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.4.0/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-08 13:08:22.195043 HawaData-0.4.0/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.4.0/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.4.0/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.4.0/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.4.0/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-08 13:08:22.196756 HawaData-0.4.0/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.4.0/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     9040 2023-05-08 13:08:04.000000 HawaData-0.4.0/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5320 2023-05-08 13:06:08.000000 HawaData-0.4.0/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.4.0/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.4.0/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-08 13:08:22.198373 HawaData-0.4.0/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.4.0/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.4.0/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.4.0/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-08 13:08:22.200748 HawaData-0.4.0/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.4.0/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    22995 2023-05-05 09:08:17.000000 HawaData-0.4.0/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.4.0/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-08 13:08:22.203266 HawaData-0.4.0/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.4.0/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-08 13:08:22.201611 HawaData-0.4.0/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.4.0/test/test_query.py
```

### Comparing `HawaData-0.3.8/HawaData.egg-info/PKG-INFO` & `HawaData-0.4.0/HawaData.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.3.8
+Version: 0.4.0
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -79,7 +79,8 @@
 - 0.3.2 performance improvement by nickname/username、cronbach_alpha、code_word
 - 0.3.3 performance improvement by grade
 - 0.3.4 up to py3.11
 - 0.3.5 fix engine encoding
 - 0.3.6 update sqlarchemy to 2+
 - 0.3.7 update pandas to 2+
 - 0.3.8 fix loss data
+- 0.4.0 add case project_id
```

### Comparing `HawaData-0.3.8/PKG-INFO` & `HawaData-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.3.8
+Version: 0.4.0
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -79,7 +79,8 @@
 - 0.3.2 performance improvement by nickname/username、cronbach_alpha、code_word
 - 0.3.3 performance improvement by grade
 - 0.3.4 up to py3.11
 - 0.3.5 fix engine encoding
 - 0.3.6 update sqlarchemy to 2+
 - 0.3.7 update pandas to 2+
 - 0.3.8 fix loss data
+- 0.4.0 add case project_id
```

### Comparing `HawaData-0.3.8/README.md` & `HawaData-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.8/hawa/base/db.py` & `HawaData-0.4.0/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.8/hawa/base/init.py` & `HawaData-0.4.0/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.8/hawa/common/data.py` & `HawaData-0.4.0/hawa/common/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """通用的 report data 构造器，支持 校、区、市、省、全国级别的通用报告数据构造"""
 import json
+from collections import Counter
 from dataclasses import dataclass, field
 from typing import Optional, ClassVar, Any, Set
 
 import pandas as pd
 import pendulum
 from munch import Munch
 
@@ -46,14 +47,15 @@
     # 原始数据
 
     school_ids: list[int] = field(default_factory=list)
     schools: pd.DataFrame = field(default_factory=pd.DataFrame)
 
     cases: pd.DataFrame = field(default_factory=pd.DataFrame)
     case_ids: list[int] = field(default_factory=list)
+    case_project_ids: Counter = field(default_factory=Counter)
 
     answers: pd.DataFrame = field(default_factory=pd.DataFrame)
 
     students: pd.DataFrame = field(default_factory=pd.DataFrame)
     student_ids: list[int] = field(default_factory=list)
     student_count: Optional[int] = None
 
@@ -121,14 +123,15 @@
             paper_ids=paper_ids,
             valid_to_start=start_stamp_str,
             valid_to_end=end_stamp_str,
         )
         if self.cases.empty:
             raise Exception(f'no cases:{self.meta_unit} {self.school_ids}')
         self.case_ids = self.cases['id'].tolist()
+        self.case_project_ids = Counter(self.cases['project_id'].tolist())
         project.logger.debug(f'cases: {len(self.cases)}')
 
     def _to_init_e_answers(self):
         self.answers = self.query.query_answers(case_ids=self.case_ids)
         project.logger.debug(f'answers: {len(self.answers)}')
 
     def _to_init_f_students(self):
@@ -210,16 +213,15 @@
     def get_last_year_miss(self, grade: int):
         key = f'{project.REDIS_PREFIX}{self.last_year_num}:data'
         data = json.loads(self.redis.conn.get(key))
         try:
             grade_data = data[str(grade)]
         except KeyError:
             temp_key = f'{project.REDIS_PREFIX}{self.last_year_num - 1}:data'
-            print(temp_key,'tk')
-            temp_cache_data=self.redis.conn.get(temp_key)
+            temp_cache_data = self.redis.conn.get(temp_key)
             if temp_cache_data:
                 temp_data = json.loads(temp_cache_data)
                 grade_data = temp_data[str(grade - 1)]
             else:
                 grade_data = data[str(3)]
 
         grade_data['people']['grade'] = f"{grade}年级"
```

### Comparing `HawaData-0.3.8/hawa/common/query.py` & `HawaData-0.4.0/hawa/common/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,45 +55,47 @@
         return pd.read_sql(text(sql), self.db.engine_conn)
 
     def query_cases(
             self, school_ids: list[int], paper_ids: list[int],
             valid_to_start: str, valid_to_end: str,
     ):
         if len(paper_ids) == 0:
-            return []
+            return pd.DataFrame()
         elif len(paper_ids) == 1:
             paper_sql = f"and c.paper_id={paper_ids[0]}"
         else:
             paper_sql = f"and c.paper_id in {tuple(paper_ids)}"
 
         if len(school_ids) == 0:
-            return []
+            return pd.DataFrame()
         elif len(school_ids) == 1:
             school_sql = f"and cs.school_id={school_ids[0]}"
         else:
             school_sql = f"and cs.school_id in {tuple(school_ids)}"
 
         sql = f"select c.id,c.name,c.valid_from,c.valid_to,c.client_id,c.created," \
-              f"c.paper_id,c.is_cleared " \
+              f"c.paper_id,c.is_cleared, cp.name project_name, c.project_id " \
               f"from cases c " \
               f"inner join case_schools cs on c.id=cs.case_id " \
+              f"inner join case_projects cp on c.project_id=cp.id " \
               f"where  is_cleared=1 and valid_to between '{valid_to_start}' and '{valid_to_end}'" \
               f" {school_sql} {paper_sql};"
         cases = pd.read_sql(text(sql), self.db.engine_conn).drop_duplicates(subset=['id'])
         return cases
 
     def query_answers(self, case_ids: list[int]):
         answer_cols = "id, student_id, item_id, case_id, answer, score, created, valid"
         if len(case_ids) == 0:
             return []
         elif len(case_ids) == 1:
             sql = f"select {answer_cols} from answers where case_id={case_ids[0]} and valid=1;"
         else:
             sql = f"select {answer_cols} from answers where case_id in {tuple(case_ids)} and valid=1;"
-        answers = pd.read_sql(text(sql), self.db.engine_conn).drop_duplicates(subset=['case_id', 'student_id', 'item_id'])
+        answers = pd.read_sql(text(sql), self.db.engine_conn).drop_duplicates(
+            subset=['case_id', 'student_id', 'item_id'])
         return answers
 
     def query_students(self, student_ids: list[int]):
         user_cols = "id, username, first_name, last_name, nickname, gender, role, source, created, " \
                     "unit_id, client_id, extra"
         sql = f"select {user_cols} from users where id in {tuple(student_ids)} and length(id)>=18;"
         students = pd.read_sql(text(sql), self.db.engine_conn).drop_duplicates(subset=['id'])
```

### Comparing `HawaData-0.3.8/hawa/common/utils.py` & `HawaData-0.4.0/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.8/hawa/config.py` & `HawaData-0.4.0/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.8/hawa/paper/health.py` & `HawaData-0.4.0/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.8/hawa/paper/mht.py` & `HawaData-0.4.0/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.8/setup.py` & `HawaData-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.8/test/test_query.py` & `HawaData-0.4.0/test/test_query.py`

 * *Files identical despite different names*

