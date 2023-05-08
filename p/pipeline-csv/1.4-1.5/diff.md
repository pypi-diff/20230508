# Comparing `tmp/pipeline_csv-1.4.tar.gz` & `tmp/pipeline_csv-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_csv-1.4.tar", last modified: Thu May  4 09:46:50 2023, max compression
+gzip compressed data, was "pipeline_csv-1.5.tar", last modified: Mon May  8 07:01:45 2023, max compression
```

## Comparing `pipeline_csv-1.4.tar` & `pipeline_csv-1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 09:46:50.290238 pipeline_csv-1.4/
--rw-rw-rw-   0        0        0     1094 2023-03-13 10:59:03.000000 pipeline_csv-1.4/LICENSE
--rw-rw-rw-   0        0        0       60 2023-03-14 17:31:18.000000 pipeline_csv-1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     7171 2023-05-04 09:46:50.290238 pipeline_csv-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     6634 2023-05-04 09:42:35.000000 pipeline_csv-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 09:46:50.274612 pipeline_csv-1.4/pipeline_csv/
--rw-rw-rw-   0        0        0      701 2023-03-15 17:59:16.000000 pipeline_csv-1.4/pipeline_csv/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 09:46:50.290238 pipeline_csv-1.4/pipeline_csv/csvfile/
--rw-rw-rw-   0        0        0    13051 2023-05-04 09:42:35.000000 pipeline_csv-1.4/pipeline_csv/csvfile/README.md
--rw-rw-rw-   0        0        0    10055 2023-05-04 09:42:35.000000 pipeline_csv-1.4/pipeline_csv/csvfile/__init__.py
--rw-rw-rw-   0        0        0    16783 2023-05-04 09:42:35.000000 pipeline_csv-1.4/pipeline_csv/csvfile/row.py
--rw-rw-rw-   0        0        0     4765 2023-05-04 09:42:35.000000 pipeline_csv-1.4/pipeline_csv/csvfile/tubes.py
--rw-rw-rw-   0        0        0     5965 2023-03-29 13:25:05.000000 pipeline_csv-1.4/pipeline_csv/oegiv.py
--rw-rw-rw-   0        0        0     2267 2023-04-14 04:49:03.000000 pipeline_csv-1.4/pipeline_csv/orientation.py
-drwxrwxrwx   0        0        0        0 2023-05-04 09:46:50.290238 pipeline_csv-1.4/pipeline_csv.egg-info/
--rw-rw-rw-   0        0        0     7171 2023-05-04 09:46:50.000000 pipeline_csv-1.4/pipeline_csv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-05-04 09:46:50.000000 pipeline_csv-1.4/pipeline_csv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 09:46:50.000000 pipeline_csv-1.4/pipeline_csv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-04 09:46:50.000000 pipeline_csv-1.4/pipeline_csv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2023-03-14 17:31:18.000000 pipeline_csv-1.4/pyproject.toml
--rw-rw-rw-   0        0        0      664 2023-05-04 09:46:50.305864 pipeline_csv-1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 07:01:45.342965 pipeline_csv-1.5/
+-rw-rw-rw-   0        0        0     1094 2023-03-13 10:59:03.000000 pipeline_csv-1.5/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-03-14 17:31:18.000000 pipeline_csv-1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     7171 2023-05-08 07:01:45.342965 pipeline_csv-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6634 2023-05-04 09:42:35.000000 pipeline_csv-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 07:01:45.311714 pipeline_csv-1.5/pipeline_csv/
+-rw-rw-rw-   0        0        0      701 2023-03-15 17:59:16.000000 pipeline_csv-1.5/pipeline_csv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:01:45.342965 pipeline_csv-1.5/pipeline_csv/csvfile/
+-rw-rw-rw-   0        0        0    13072 2023-05-05 10:15:19.000000 pipeline_csv-1.5/pipeline_csv/csvfile/README.md
+-rw-rw-rw-   0        0        0    10238 2023-05-06 10:11:21.000000 pipeline_csv-1.5/pipeline_csv/csvfile/__init__.py
+-rw-rw-rw-   0        0        0    16783 2023-05-04 09:42:35.000000 pipeline_csv-1.5/pipeline_csv/csvfile/row.py
+-rw-rw-rw-   0        0        0     4943 2023-05-06 10:11:21.000000 pipeline_csv-1.5/pipeline_csv/csvfile/tubes.py
+-rw-rw-rw-   0        0        0     5965 2023-03-29 13:25:05.000000 pipeline_csv-1.5/pipeline_csv/oegiv.py
+-rw-rw-rw-   0        0        0     2267 2023-04-14 04:49:03.000000 pipeline_csv-1.5/pipeline_csv/orientation.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:01:45.327340 pipeline_csv-1.5/pipeline_csv.egg-info/
+-rw-rw-rw-   0        0        0     7171 2023-05-08 07:01:45.000000 pipeline_csv-1.5/pipeline_csv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-05-08 07:01:45.000000 pipeline_csv-1.5/pipeline_csv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 07:01:45.000000 pipeline_csv-1.5/pipeline_csv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-08 07:01:45.000000 pipeline_csv-1.5/pipeline_csv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2023-03-14 17:31:18.000000 pipeline_csv-1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      664 2023-05-08 07:01:45.342965 pipeline_csv-1.5/setup.cfg
```

### Comparing `pipeline_csv-1.4/LICENSE` & `pipeline_csv-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.4/PKG-INFO` & `pipeline_csv-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline_csv
-Version: 1.4
+Version: 1.5
 Summary: Pipeline inline inspection data as CSV file.
 Home-page: https://github.com/vb64/pipeline.csv
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
 Project-URL: Bug Tracker, https://github.com/vb64/pipeline.csv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pipeline_csv-1.4/README.md` & `pipeline_csv-1.5/README.md`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.4/pipeline_csv/__init__.py` & `pipeline_csv-1.5/pipeline_csv/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.4/pipeline_csv/csvfile/README.md` & `pipeline_csv-1.5/pipeline_csv/csvfile/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,14 @@
 
 Номер колонки '16' заголовок 'DistML'
 
 Если задано, то должно содержать уникальный для данной колонки идентификатор обьекта (строка).
 
 ### Колонки, используемые для привязки обьектов к маркерам и швам в экспресс-отчете InspectionViewer
 
--   04 ObjectName Текст до 20 символов длиной.
--   16 DistML Дистанция до маркера слева в мм.
 -   17 DistMR Дистанция до маркера справа в мм.
 -   18 DistStL Дистанция до стыка слева в мм.
 -   19 DistStR Дистанция до стыка справа в мм.
 -   20 LinkStL Имя шва слева к которому привязан объект - значение из поля  ObjectName. Текст до 20 символов длиной.
 -   21 LinkStR Имя шва справа к которому привязан объект - значение из поля  ObjectName. Текст до 20 символов длиной.
 -   22 LinkML Имя маркера слева к которому привязан объект - значение из поля  ObjectName. Текст до 20 символов длиной.
 -   23 LinkMR Имя маркера справа к которому привязан объект - значение из поля  ObjectName. Текст до 20 символов длиной.
@@ -85,29 +83,31 @@
 -   14 MPoint_Dist
 -   15 Type_Def
 
 ### Швы
 
 Если значение колонки 02 TypeObject установлено в 0 (Шов)
 
-Колонка 03 Object_Code должна содержать код 0, а колонка 05 Object_Code_T должна содержать текст 'Шов'.
+Колонка 03 Object_Code должна содержать код 0
 
-Колонка 04 ObjectName может содержать пользовательский номер трубы (произвольная строка в кодировке win-1251).
+Колонка 04 ObjectName может содержать пользовательский номер трубы (произвольная строка).
+
+Колонка 05 Object_Code_T может содержать текстовое название обьекта, например 'Шов'.
 
 Колонка 09 Depth_min может содержать радиус изгиба трубы в ее диаметрах (с плавающей точкой).
 
 Колонка 10 Depth_max может содержать минимальное проходное сечение трубы в мм (строка).
 
 Остальные колонки должны быть пустыми.
 
 ### Маркеры
 
 Если значение колонки 02 TypeObject установлено в 1 (Маркер)
 
-Колонка 03 Object_Code должна содержать код объекта, а колонка 05 Object_Code_T должна содержать текст, соответствующий данному коду.
+Колонка 03 Object_Code должна содержать код объекта
 
 -   0 Кран
 -   1 Маркер 
 -   2 Маркер магнитный
 -   3 Отвод-врезка
 -   4 Тройник
 -   5 Патрон начало
@@ -116,21 +116,23 @@
 -   8 Пригруз
 -   9 Отвод (поворот) начало
 -   10 Отвод (поворот) конец
 -   11 Особенность 
 -   12 Гнутая секция
 -   13 Сегмент поворота
 
+Колонка 05 Object_Code_T может содержать текстовое название обьекта, например 'Кран'.
+
 Остальные колонки должны быть пустыми.
 
 ### Дефекты
 
 Если значение колонки 02 TypeObject установлено в 2 (Дефект)
 
-Колонка 03 Object_Code должна содержать один из следующих кодов, а колонка 05 Object_Code_T должна содержать текст, соответствующий данному коду.
+Колонка 03 Object_Code должна содержать один из следующих кодов.
 
 -   0 Коррозия 
 -   1 Механическое повреждение
 -   2 Вмятина
 -   3 Вмятина с дефектами потери металла
 -   4 Гофра
 -   5 Аномалия кольцевого шва
@@ -144,14 +146,16 @@
 -   13 Расслоение
 -   14 Аномалия продольного шва
 -   15 Аномалия спирального шва
 -   16 Эллипсность 
 -   17 Поджиг 
 -   18 Зашлифовка
 
+Колонка 05 Object_Code_T может содержать текстовое название обьекта, например 'Коррозия'.
+
 Остальные колонки должны содержать параметры дефекта
 
 -   07 Length Длина в мм
 -   08 Width Ширина в мм
 -   09 Depth_min Минимальная глубина в %
 -   10 Depth_max Максимальная глубина в %
 -   11 OrientTD Начало угловой ориентации в формате "часы,минуты"
@@ -167,15 +171,17 @@
 -   2 внутренняя
 -   3 внутристенная коррозия
 
 ### Изменение толщины стенки трубы
 
 Если значение колонки 02 TypeObject установлено в 3 (Переход толщины)
 
-Колонка 03 Object_Code должна содержать код 0, а колонка 05 Object_Code_T должна содержать текст 'Изменение толщины стенки трубы'.
+Колонка 03 Object_Code должна содержать код 0
+
+Колонка 05 Object_Code_T может содержать текстовое название обьекта, например 'Изменение толщины стенки трубы'.
 
 Колонка 10 Depth_max должна содержать значение толщины стенки трубы в десятых долях миллиметра.
 Например, значение 107 соответствует тольщине стенки в 10.7 мм.
 
 Остальные колонки должны быть пустыми.
 
 ### Продольный шов
@@ -193,15 +199,17 @@
 
 Остальные колонки должны быть пустыми.
 
 ### Категория трубопровода
 
 Если значение колонки 02 TypeObject установлено в 5 (Категория трубопровода)
 
-Колонка 03 Object_Code должна содержать код 0, а колонка 05 Object_Code_T должна содержать текст 'Категория трубопровода'.
+Колонка 03 Object_Code должна содержать код 0.
+
+Колонка 05 Object_Code_T может содержать текстовое название обьекта, например 'Категория трубопровода'.
 
 Колонка 10 Depth_max должна содержать код категории трубопровода.
 
 Остальные колонки должны быть пустыми.
 
 ## Схема использования колонок по типам обьектов
```

### Comparing `pipeline_csv-1.4/pipeline_csv/csvfile/__init__.py` & `pipeline_csv-1.5/pipeline_csv/csvfile/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,25 +307,32 @@
         from .tubes import Tube
 
         tube = None
         auto_num = 1
         for row in sorted(self.data, key=lambda val: int(val.dist_od)):
             if row.is_weld:
                 if tube:
-                    tube.finalize(row.dist_od, warns)
+                    tube.finalize(row.dist_od)
                     auto_num += 1
                 yield tube
                 tube = Tube(row, self.stream, str(auto_num))
             else:
                 if tube:
                     tube.add_object(row)
                 else:
-                    warns.append("Object before first weld: {}".format(row))
+                    self.add_warn("Object before first weld: {}".format(row), warns)
 
-    def get_tubes(self, warns):
+    @staticmethod
+    def add_warn(msg, warns):
+        """Add message to warn list."""
+        if warns is not None:
+            warns.append(msg)
+        return warns
+
+    def get_tubes(self, warns=None):
         """Return ready iterator for tubes in csv data."""
         tubes = self._create_tubes_iterator(warns)
         try:
             next(tubes)
         except StopIteration:
             return []
```

### Comparing `pipeline_csv-1.4/pipeline_csv/csvfile/row.py` & `pipeline_csv-1.5/pipeline_csv/csvfile/row.py`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.4/pipeline_csv/csvfile/tubes.py` & `pipeline_csv-1.5/pipeline_csv/csvfile/tubes.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     def __str__(self):
         """Return as text."""
         return "Tube len {} wall {}".format(
           self.length,
           self.thick
         )
 
-    def finalize(self, dist, _warns):
+    def finalize(self, dist):
         """Finalize tube data at given dist."""
         self.length = int(dist) - self.dist
         self.thick = self.stream.thick
         self.category = self.stream.category
 
     def add_object(self, row):
         """Add data to tube from csv row."""
@@ -157,7 +157,11 @@
             text = self.seams[0].orient_td
         elif self.typ == TypeHorWeld.SECOND:
             text = self.seams[0].orient_td + ' / ' + self.seams[0].orient_bd
         elif self.typ == TypeHorWeld.SPIRAL:
             text = ' / '.join([i.orient_td for i in self.seams])
 
         return text
+
+    def features(self):
+        """Return defects and lineobjects of the pipe, arranged by distance."""
+        return sorted(self.lineobjects + self.defects, key=lambda i: i.dist)
```

### Comparing `pipeline_csv-1.4/pipeline_csv/oegiv.py` & `pipeline_csv-1.5/pipeline_csv/oegiv.py`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.4/pipeline_csv/orientation.py` & `pipeline_csv-1.5/pipeline_csv/orientation.py`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.4/pipeline_csv.egg-info/PKG-INFO` & `pipeline_csv-1.5/pipeline_csv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-csv
-Version: 1.4
+Version: 1.5
 Summary: Pipeline inline inspection data as CSV file.
 Home-page: https://github.com/vb64/pipeline.csv
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
 Project-URL: Bug Tracker, https://github.com/vb64/pipeline.csv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pipeline_csv-1.4/setup.cfg` & `pipeline_csv-1.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6970 656c 696e 655f 6373 760d   = pipeline_csv.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e34 0d0a  .version = 1.4..
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e35 0d0a  .version = 1.5..
 00000030: 6175 7468 6f72 203d 2056 6974 616c 7920  author = Vitaly 
 00000040: 426f 676f 6d6f 6c6f 760d 0a61 7574 686f  Bogomolov..autho
 00000050: 725f 656d 6169 6c20 3d20 6d61 696c 4076  r_email = mail@v
 00000060: 6974 616c 792d 626f 676f 6d6f 6c6f 762e  italy-bogomolov.
 00000070: 7275 0d0a 6465 7363 7269 7074 696f 6e20  ru..description 
 00000080: 3d20 5069 7065 6c69 6e65 2069 6e6c 696e  = Pipeline inlin
 00000090: 6520 696e 7370 6563 7469 6f6e 2064 6174  e inspection dat
```

