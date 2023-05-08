# Comparing `tmp/calcure-2.9.1.tar.gz` & `tmp/calcure-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcure-2.9.1.tar", last modified: Sat May  6 06:51:01 2023, max compression
+gzip compressed data, was "calcure-2.9.2.tar", last modified: Mon May  8 07:58:30 2023, max compression
```

## Comparing `calcure-2.9.1.tar` & `calcure-2.9.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-06 06:51:01.751570 calcure-2.9.1/
--rw-r--r--   0 r         (1000) r         (1000)     1071 2023-03-01 08:49:55.000000 calcure-2.9.1/LICENSE
--rw-r--r--   0 r         (1000) r         (1000)     3908 2023-05-06 06:51:01.751570 calcure-2.9.1/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)     3145 2023-03-02 07:55:45.000000 calcure-2.9.1/README.md
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-06 06:51:01.751570 calcure-2.9.1/calcure/
--rw-r--r--   0 r         (1000) r         (1000)    41704 2023-05-06 06:48:22.000000 calcure-2.9.1/calcure/__main__.py
--rw-r--r--   0 r         (1000) r         (1000)     2551 2023-03-02 07:54:07.000000 calcure-2.9.1/calcure/calendars.py
--rw-r--r--   0 r         (1000) r         (1000)     4162 2023-03-04 12:39:25.000000 calcure-2.9.1/calcure/colors.py
--rw-r--r--   0 r         (1000) r         (1000)    20458 2023-05-06 06:48:33.000000 calcure-2.9.1/calcure/configuration.py
--rw-r--r--   0 r         (1000) r         (1000)    25533 2023-05-04 11:25:37.000000 calcure-2.9.1/calcure/controls.py
--rw-r--r--   0 r         (1000) r         (1000)    13499 2023-05-04 11:25:39.000000 calcure-2.9.1/calcure/data.py
--rw-r--r--   0 r         (1000) r         (1000)     3564 2023-05-03 20:15:00.000000 calcure-2.9.1/calcure/dialogues.py
--rw-r--r--   0 r         (1000) r         (1000)     1071 2023-05-04 12:44:35.000000 calcure-2.9.1/calcure/errors.py
--rw-r--r--   0 r         (1000) r         (1000)     3689 2023-05-03 19:07:39.000000 calcure-2.9.1/calcure/importers.py
--rw-r--r--   0 r         (1000) r         (1000)    14637 2023-05-04 10:09:19.000000 calcure-2.9.1/calcure/loaders.py
--rw-r--r--   0 r         (1000) r         (1000)     2550 2023-03-01 08:49:55.000000 calcure-2.9.1/calcure/savers.py
--rw-r--r--   0 r         (1000) r         (1000)     4725 2023-05-06 06:48:16.000000 calcure-2.9.1/calcure/screen.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-06 06:51:01.751570 calcure-2.9.1/calcure/translations/
--rw-r--r--   0 r         (1000) r         (1000)     5793 2023-05-04 11:34:28.000000 calcure-2.9.1/calcure/translations/br.py
--rw-r--r--   0 r         (1000) r         (1000)     5289 2023-05-04 11:33:46.000000 calcure-2.9.1/calcure/translations/en.py
--rw-r--r--   0 r         (1000) r         (1000)     6251 2023-05-04 11:37:01.000000 calcure-2.9.1/calcure/translations/fr.py
--rw-r--r--   0 r         (1000) r         (1000)     6283 2023-05-04 11:34:29.000000 calcure-2.9.1/calcure/translations/it.py
--rw-r--r--   0 r         (1000) r         (1000)     8277 2023-05-04 11:34:30.000000 calcure-2.9.1/calcure/translations/ru.py
--rw-r--r--   0 r         (1000) r         (1000)     6134 2023-05-04 11:34:30.000000 calcure-2.9.1/calcure/translations/tr.py
--rw-r--r--   0 r         (1000) r         (1000)     5433 2023-05-04 11:36:18.000000 calcure-2.9.1/calcure/translations/zh.py
--rw-r--r--   0 r         (1000) r         (1000)      989 2023-05-06 06:48:14.000000 calcure-2.9.1/calcure/weather.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-06 06:51:01.751570 calcure-2.9.1/calcure.egg-info/
--rw-r--r--   0 r         (1000) r         (1000)     3908 2023-05-06 06:51:01.000000 calcure-2.9.1/calcure.egg-info/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)      672 2023-05-06 06:51:01.000000 calcure-2.9.1/calcure.egg-info/SOURCES.txt
--rw-r--r--   0 r         (1000) r         (1000)        1 2023-05-06 06:51:01.000000 calcure-2.9.1/calcure.egg-info/dependency_links.txt
--rw-r--r--   0 r         (1000) r         (1000)       49 2023-05-06 06:51:01.000000 calcure-2.9.1/calcure.egg-info/entry_points.txt
--rw-r--r--   0 r         (1000) r         (1000)       23 2023-05-06 06:51:01.000000 calcure-2.9.1/calcure.egg-info/requires.txt
--rw-r--r--   0 r         (1000) r         (1000)        8 2023-05-06 06:51:01.000000 calcure-2.9.1/calcure.egg-info/top_level.txt
--rw-r--r--   0 r         (1000) r         (1000)       91 2023-03-01 08:49:55.000000 calcure-2.9.1/pyproject.toml
--rw-r--r--   0 r         (1000) r         (1000)       38 2023-05-06 06:51:01.751570 calcure-2.9.1/setup.cfg
--rw-r--r--   0 r         (1000) r         (1000)     1427 2023-03-01 08:49:55.000000 calcure-2.9.1/setup.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-08 07:58:30.196696 calcure-2.9.2/
+-rw-r--r--   0 r         (1000) r         (1000)     1071 2023-03-01 08:49:55.000000 calcure-2.9.2/LICENSE
+-rw-r--r--   0 r         (1000) r         (1000)     3908 2023-05-08 07:58:30.196696 calcure-2.9.2/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)     3145 2023-03-02 07:55:45.000000 calcure-2.9.2/README.md
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-08 07:58:30.193363 calcure-2.9.2/calcure/
+-rw-r--r--   0 r         (1000) r         (1000)    42043 2023-05-08 07:56:13.000000 calcure-2.9.2/calcure/__main__.py
+-rw-r--r--   0 r         (1000) r         (1000)     2551 2023-03-02 07:54:07.000000 calcure-2.9.2/calcure/calendars.py
+-rw-r--r--   0 r         (1000) r         (1000)     4162 2023-03-04 12:39:25.000000 calcure-2.9.2/calcure/colors.py
+-rw-r--r--   0 r         (1000) r         (1000)    20458 2023-05-08 07:56:23.000000 calcure-2.9.2/calcure/configuration.py
+-rw-r--r--   0 r         (1000) r         (1000)    25533 2023-05-08 07:56:33.000000 calcure-2.9.2/calcure/controls.py
+-rw-r--r--   0 r         (1000) r         (1000)    13499 2023-05-08 07:53:30.000000 calcure-2.9.2/calcure/data.py
+-rw-r--r--   0 r         (1000) r         (1000)     3512 2023-05-08 07:54:09.000000 calcure-2.9.2/calcure/dialogues.py
+-rw-r--r--   0 r         (1000) r         (1000)     1572 2023-05-08 07:55:03.000000 calcure-2.9.2/calcure/errors.py
+-rw-r--r--   0 r         (1000) r         (1000)     3689 2023-05-03 19:07:39.000000 calcure-2.9.2/calcure/importers.py
+-rw-r--r--   0 r         (1000) r         (1000)    14637 2023-05-04 10:09:19.000000 calcure-2.9.2/calcure/loaders.py
+-rw-r--r--   0 r         (1000) r         (1000)     2550 2023-03-01 08:49:55.000000 calcure-2.9.2/calcure/savers.py
+-rw-r--r--   0 r         (1000) r         (1000)     4725 2023-05-06 11:03:23.000000 calcure-2.9.2/calcure/screen.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-08 07:58:30.196696 calcure-2.9.2/calcure/translations/
+-rw-r--r--   0 r         (1000) r         (1000)     5832 2023-05-08 07:19:10.000000 calcure-2.9.2/calcure/translations/br.py
+-rw-r--r--   0 r         (1000) r         (1000)     5328 2023-05-08 07:19:11.000000 calcure-2.9.2/calcure/translations/en.py
+-rw-r--r--   0 r         (1000) r         (1000)     6293 2023-05-08 07:19:09.000000 calcure-2.9.2/calcure/translations/fr.py
+-rw-r--r--   0 r         (1000) r         (1000)     6325 2023-05-08 07:19:08.000000 calcure-2.9.2/calcure/translations/it.py
+-rw-r--r--   0 r         (1000) r         (1000)     8334 2023-05-08 07:19:07.000000 calcure-2.9.2/calcure/translations/ru.py
+-rw-r--r--   0 r         (1000) r         (1000)     6173 2023-05-08 07:20:42.000000 calcure-2.9.2/calcure/translations/tr.py
+-rw-r--r--   0 r         (1000) r         (1000)     5472 2023-05-08 07:19:38.000000 calcure-2.9.2/calcure/translations/zh.py
+-rw-r--r--   0 r         (1000) r         (1000)      989 2023-05-06 06:48:14.000000 calcure-2.9.2/calcure/weather.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-08 07:58:30.193363 calcure-2.9.2/calcure.egg-info/
+-rw-r--r--   0 r         (1000) r         (1000)     3908 2023-05-08 07:58:30.000000 calcure-2.9.2/calcure.egg-info/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)      672 2023-05-08 07:58:30.000000 calcure-2.9.2/calcure.egg-info/SOURCES.txt
+-rw-r--r--   0 r         (1000) r         (1000)        1 2023-05-08 07:58:30.000000 calcure-2.9.2/calcure.egg-info/dependency_links.txt
+-rw-r--r--   0 r         (1000) r         (1000)       49 2023-05-08 07:58:30.000000 calcure-2.9.2/calcure.egg-info/entry_points.txt
+-rw-r--r--   0 r         (1000) r         (1000)       23 2023-05-08 07:58:30.000000 calcure-2.9.2/calcure.egg-info/requires.txt
+-rw-r--r--   0 r         (1000) r         (1000)        8 2023-05-08 07:58:30.000000 calcure-2.9.2/calcure.egg-info/top_level.txt
+-rw-r--r--   0 r         (1000) r         (1000)       91 2023-03-01 08:49:55.000000 calcure-2.9.2/pyproject.toml
+-rw-r--r--   0 r         (1000) r         (1000)       38 2023-05-08 07:58:30.196696 calcure-2.9.2/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1000)     1427 2023-03-01 08:49:55.000000 calcure-2.9.2/setup.py
```

### Comparing `calcure-2.9.1/LICENSE` & `calcure-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `calcure-2.9.1/PKG-INFO` & `calcure-2.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcure
-Version: 2.9.1
+Version: 2.9.2
 Summary: Modern TUI calendar and task manager
 Home-page: https://github.com/anufrievroman/calcure
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calcure-2.9.1/README.md` & `calcure-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `calcure-2.9.1/calcure/__main__.py` & `calcure-2.9.2/calcure/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     from calcure.translations.tr import *
 elif cf.LANG == "zh":
     from calcure.translations.zh import *
 else:
     from calcure.translations.en import *
 
 
-__version__ = "2.9.1"
+__version__ = "2.9.2"
 
 
 def read_items_from_user_arguments(screen, user_tasks, user_events, task_saver_csv, event_saver_csv):
     """Read --task and --event flags from user arguments to create new tasks or events"""
     try:
         opts, _ = getopt.getopt(sys.argv[1:], "pjhvi", ["folder=", "config=", "task=", "event="])
         for opt, arg in opts:
@@ -228,15 +228,15 @@
     def render(self):
         """Render the list of tasks"""
         if not self.user_tasks.items and not self.user_ics_tasks.items and cf.SHOW_NOTHING_PLANNED:
             self.display_line(self.y, self.x, MSG_TS_NOTHING, Color.UNIMPORTANT)
         for index, task in enumerate(self.user_tasks.items):
             task_view = TaskView(self.stdscr, self.y, self.x, task, self.screen)
             task_view.render()
-            if self.screen.selection_mode:
+            if self.screen.selection_mode and self.screen.state == AppState.JOURNAL:
                 self.display_line(self.y, self.x, str(index + 1), Color.ACTIVE_PANE)
             self.y += 1
 
         self.y += 1
         for index, task in enumerate(self.user_ics_tasks.items):
             task_view = TaskView(self.stdscr, self.y, self.x, task, self.screen)
             task_view.render()
@@ -426,15 +426,16 @@
         # Show user events:
         for event in self.user_events.items:
             if index >= self.y_cell - 1 and self.screen.calendar_state == CalState.MONTHLY:
                 self.display_line(self.y + self.y_cell - 2, self.x, self.hidden_events_sign, Color.EVENTS)
             else:
                 user_event_view = UserEventView(self.stdscr, self.y + index, self.x, event, self.screen)
                 user_event_view.render()
-                if self.screen.selection_mode and self.is_selection_day:
+
+                if self.screen.selection_mode and self.is_selection_day and self.screen.state == AppState.CALENDAR:
                     self.display_line(self.y + index, self.x, str(index + self.index_offset + 1), Color.ACTIVE_PANE)
             index += 1
 
         # Show repeated user events and events from ics:
         for event_list in [self.repeated_user_events.items, self.user_ics_events.items]:
             for event in event_list:
                 if index >= self.y_cell - 1 and self.screen.calendar_state == CalState.MONTHLY:
@@ -580,15 +581,21 @@
         self.screen = screen
         self.error = error
 
     def render(self):
         """Render this view on the screen"""
         if self.error.has_occured:
             clear_line(self.stdscr, self.screen.y_max - 2)
-            self.display_line(self.screen.y_max - 2, 0, MSG_ERRORS, Color.IMPORTANT)
+
+            # Depending on error type, display different messages:
+            if self.error.number_of_errors > 1 or "ERROR" in self.error.type:
+                self.display_line(self.screen.y_max - 2, 0, MSG_ERRORS, Color.IMPORTANT)
+            else:
+                self.display_line(self.screen.y_max - 2, 0, MSG_INPUT, Color.HINTS)
+
             self.error.clear_buffer()
 
 
 class SeparatorView(View):
     """Display the separator in the split screen"""
 
     def __init__(self, stdscr, y, x, screen):
```

### Comparing `calcure-2.9.1/calcure/calendars.py` & `calcure-2.9.2/calcure/calendars.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.1/calcure/colors.py` & `calcure-2.9.2/calcure/colors.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.1/calcure/configuration.py` & `calcure-2.9.2/calcure/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,15 @@
                     self.DEFAULT_VIEW = AppState.JOURNAL
                 elif opt == '-d':
                     self.DEFAULT_VIEW = AppState.JOURNAL
                 elif opt in ('-h'):
                     self.DEFAULT_VIEW = AppState.HELP
                 elif opt in ('-v'):
                     self.DEFAULT_VIEW = AppState.EXIT
-                    print ('Calcure - version 2.9.1')
+                    print ('Calcure - version 2.9.2')
                 elif opt in ('-i'):
                     self.USE_PERSIAN_CALENDAR = True
         except getopt.GetoptError as e_message:
             logging.error("Invalid user arguments. %s", e_message)
             pass
```

### Comparing `calcure-2.9.1/calcure/controls.py` & `calcure-2.9.2/calcure/controls.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.1/calcure/data.py` & `calcure-2.9.2/calcure/data.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.1/calcure/dialogues.py` & `calcure-2.9.2/calcure/dialogues.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,40 +40,40 @@
 
 def input_integer(stdscr, y, x, question):
     """Ask user for an integer number and check if it is an integer"""
     number = input_string(stdscr, y, x, question, 3)
     try:
         number = int(number) - 1
     except ValueError:
-        logging.warning("Incorrect input of integer %s.", number)
+        logging.warning("Incorrect number input.")
         return None
     return number
 
 
 def input_day(stdscr, y, x, prompt_string):
     """Ask user for an integer number and check if it is an integer"""
     number = input_string(stdscr, y, x, prompt_string, 2)
     try:
         number = int(number)
     except ValueError:
-        logging.warning("Incorrect input of day %s.", number)
+        logging.warning("Incorrect day input.")
         return None
     return number
 
 
 def input_date(stdscr, y, x, prompt_string):
     """Ask user to input date in YYYY/MM/DD format and check if it was valid entry"""
     date_unformated = input_string(stdscr, y, x, prompt_string, 10)
     try:
         year = int(date_unformated.split("/")[0])
         month = int(date_unformated.split("/")[1])
         day = int(date_unformated.split("/")[2])
         return year, month, day
     except (ValueError, IndexError):
-        logging.warning("Incorrect input of date %s.", date_unformated)
+        logging.warning("Incorrect date input.")
         return None, None, None
 
 
 def input_frequency(stdscr, y, x, question):
     """Ask user for the frequency of event repetitions"""
     freq = input_string(stdscr, y, x, question, 2)
     if freq == 'd':
```

### Comparing `calcure-2.9.1/calcure/errors.py` & `calcure-2.9.2/calcure/errors.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,32 +3,47 @@
 import logging
 import io
 
 from calcure.configuration import cf
 
 
 class Error():
-    """Error messages displayed to the user"""
+    """Error messages displayed to the user.
+    Different errors have different purposes:
+    ERROR type is reserved for loading errors;
+    WARNING type is reserved for incorrect user input;"""
 
     def __init__(self):
         self.buffer = io.StringIO()
         self.file = f"{cf.config_folder}/info.log"
 
-    def get_error_text(self):
-        """Returns string with the text of the error"""
-        return self.buffer.getvalue()
-
-    def clear_buffer(self):
-        """Clear the buffer containing errors"""
-        self.buffer = io.StringIO()
-
     @property
     def has_occured(self):
         """Has any errors occured?"""
-        return self.get_error_text() != ""
+        return self.buffer.getvalue() != ""
+
+    @property
+    def number_of_errors(self):
+        """Return the number of different errors in the buffer"""
+        return self.buffer.getvalue().count("[")
+
+    @property
+    def text(self):
+        """Return the string with the text of the error"""
+        return self.buffer.getvalue().split("] ")[1]
+
+    @property
+    def type(self):
+        """Return the string with type of the error"""
+        return self.buffer.getvalue().split("] ")[0]
+
+    def clear_buffer(self):
+        """Clear the buffer containing errors"""
+        self.buffer.seek(0)
+        self.buffer.truncate(0)
 
 
 # Initialise error:
 error = Error()
 
 # Start logging:
 logging.basicConfig(level=logging.INFO,
```

### Comparing `calcure-2.9.1/calcure/importers.py` & `calcure-2.9.2/calcure/importers.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.1/calcure/loaders.py` & `calcure-2.9.2/calcure/loaders.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.1/calcure/savers.py` & `calcure-2.9.2/calcure/savers.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.1/calcure/screen.py` & `calcure-2.9.2/calcure/screen.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.1/calcure/translations/br.py` & `calcure-2.9.2/calcure/translations/br.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 MSG_TS_DEAD_ADD   = "Adicionar data limite da tarefa número: "
 MSG_TS_DEAD_DEL   = "Remover data limite da tarefa número: "
 MSG_TS_DEAD_DATE  = "Adicionar data limite em (AAAA/MM/DD): "
 MSG_WEATHER       = "Clima está carregando..."
 MSG_ERRORS        = "Errors have occurred. See info.log file in your config folder."
 MSG_GOTO          = "Go to date (YYYY/MM/DD): "
 MSG_GOTO_D        = "Go to date: "
+MSG_INPUT         = "Incorrect input."
 
 CALENDAR_HINT     = "Espaço · Mudar para diário   a · Adicionar evento  n/p · Mudar mês   ? · Todas as combinações de teclas"
 CALENDAR_HINT_D   = "Espaço · Mudar para diário   a · Adicionar evento  n/p · Mudar dia   ? · Todas as combinações de teclas"
 JOURNAL_HINT      = "Espaço · Mudar para calendar   a · Adicionar tarefa   d · Feito   i · Importante   ? · Todas as combinações de teclas"
 
 DAYS = ["SEGUNDA", "TERÇA", "QUARTA", "QUINTA", "SEXTA", "SÁBADO", "DOMINGO"]
 DAYS_PERSIAN = ["SHANBEH", "YEKSHANBEH", "DOSHANBEH", "SESHANBEH", "CHAHARSHANBEH", "PANJSHANBEH", "JOMEH"]
```

### Comparing `calcure-2.9.1/calcure/translations/en.py` & `calcure-2.9.2/calcure/translations/en.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 MSG_TS_NOTHING    = "Nothing planned..."
 MSG_TS_PRIVACY    = "Toggle privacy of task number: "
 MSG_TS_DEAD_ADD   = "Add deadline for task number: "
 MSG_TS_DEAD_DEL   = "Remove deadline of the task number: "
 MSG_TS_DEAD_DATE  = "Add deadline on (YYYY/MM/DD): "
 MSG_WEATHER       = "Weather is loading..."
 MSG_ERRORS        = "Errors have occurred. See info.log in your config folder."
+MSG_INPUT         = "Incorrect input."
 MSG_GOTO          = "Go to date (YYYY/MM/DD): "
 MSG_GOTO_D        = "Go to date: "
 
 CALENDAR_HINT     = "Space · Switch to journal   a · Add event  n/p · Change month   ? · All keybindings"
 CALENDAR_HINT_D   = "Space · Switch to journal   a · Add event  n/p · Change day   ? · All keybindings"
 JOURNAL_HINT      = "Space · Switch to calendar   a · Add task   d · Done   i · Important   ? · All keybindings"
```

### Comparing `calcure-2.9.1/calcure/translations/fr.py` & `calcure-2.9.2/calcure/translations/fr.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 MSG_TS_DEAD_ADD   = "Ajouter le deadline pour la tâche numéro: "
 MSG_TS_DEAD_DEL   = "Supprimer le deadline de la tâche numéro: "
 MSG_TS_DEAD_DATE  = "Ajouter le deadline (AAAA/MM/JJ): "
 MSG_WEATHER       = "La météo se charge..."
 MSG_ERRORS        = "Des erreurs se sont produites. Voir info.log dans votre dossier de configuration."
 MSG_GOTO          = "Aller au (YYYY/MM/DD): "
 MSG_GOTO_D        = "Aller au: "
+MSG_INPUT         = "Entrée incorrecte."
 
 CALENDAR_HINT     = "Espace · Passer au journal  a · Ajouter un événement  n/p · Changer de mois  ? · Aider"
 CALENDAR_HINT_D   = "Espace · Passer au journal  a · Ajouter un événement  n/p · Changer de jour  ? · All keybindings"
 JOURNAL_HINT      = "Espace · Passer au calendrier  a · Ajouter une tâche  d · Terminé  i · Important  ? · All keybindings"
 
 DAYS = ["LUNDI", "MARDI", "MERCREDI", "JEUDI", "VENDREDI", "SAMEDI", "DIMANCHE"]
 DAYS_PERSIAN = ["SHANBEH", "YEKSHANBEH", "DOSHANBEH", "SESHANBEH", "CHAHARSHANBEH", "PANJSHANBEH", "JOMEH"]
```

### Comparing `calcure-2.9.1/calcure/translations/it.py` & `calcure-2.9.2/calcure/translations/it.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 MSG_TS_DEAD_ADD   = "Aggiungi una scadenza per l'attività con numero: "
 MSG_TS_DEAD_DEL   = "Rimuovi la scadenza per l'attività con numero: "
 MSG_TS_DEAD_DATE  = "Aggiungi una scandeza per il (AAAA/MM/GG): "
 MSG_WEATHER       = "Caricamento del meteo..."
 MSG_ERRORS        = "Errors have occurred. See info.log file in your config folder."
 MSG_GOTO          = "Vai alla data (YYYY/MM/DD): "
 MSG_GOTO_D        = "Vai alla data: "
+MSG_INPUT         = "Inserimento errato."
 
 CALENDAR_HINT     = "Barra spaziatrice · Passa al diario   a · Aggiungi un evento  n/p · Cambia mese   ? · Mostra tutte le scorciatoie"
 CALENDAR_HINT_D   = "Barra spaziatrice · Passa al diario   a · Aggiungi un evento  n/p · Cambia giorno  ? · Mostra tutte le scorciatoie"
 JOURNAL_HINT      = "Barra spaziatrice · Passa al calendario   a · Add task   d · Finito   i · Importante   ? · Mostra tutte le scorciatoie"
 
 DAYS = ["LUNEDÌ", "MARTEDÌ", "MERCOLEDÌ", "GIOVEDÌ", "VENERDì", "SABATO", "DOMENICA"]
 DAYS_PERSIAN = ["SHANBEH", "YEKSHANBEH", "DOSHANBEH", "SESHANBEH", "CHAHARSHANBEH", "PANJSHANBEH", "JOMEH"]
```

### Comparing `calcure-2.9.1/calcure/translations/ru.py` & `calcure-2.9.2/calcure/translations/ru.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 MSG_TS_DEAD_ADD   = "Добавить дедлайн к задаче номер: "
 MSG_TS_DEAD_DEL   = "Удалить дедлайн задачи номер: "
 MSG_TS_DEAD_DATE  = "Установить дедлайн на (YYYY/MM/DD): "
 MSG_WEATHER       = "Загружается информации о погоде..."
 MSG_ERRORS        = "Возникли ошибки. Детали в info.log файле в конфиг директории."
 MSG_GOTO          = "Перейти к дате (YYYY/MM/DD): "
 MSG_GOTO_D        = "Перейти к дате: "
+MSG_INPUT         = "Некорректный ввод."
 
 CALENDAR_HINT     = "Пробел · Переключить на журнал   a · Новое событие  n/p · Сменить месяц   ? · Клавиши"
 CALENDAR_HINT_D   = "Пробел · Переключить на журнал   a · Новое событие  n/p · Сменить день   ? · Клавиши"
 JOURNAL_HINT      = "Пробел · Переключить на календарь   a · Новая задача   d · Выполнено   h · Важно   ? · Клавиши"
 
 DAYS         = ["ПОНЕДЕЛЬНИК", "ВТОРНИК", "СРЕДА", "ЧЕТВЕРГ", "ПЯТНИЦА", "СУББОТА", "ВОСКРЕСЕНЬЕ"]
 DAYS_PERSIAN = ["SHANBEH", "YEKSHANBEH", "DOSHANBEH", "SESHANBEH", "CHAHARSHANBEH", "PANJSHANBEH", "JOMEH"]
```

### Comparing `calcure-2.9.1/calcure/translations/tr.py` & `calcure-2.9.2/calcure/translations/tr.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 MSG_TS_DEAD_ADD   = "Görev numarası için son tarih ekle: "
 MSG_TS_DEAD_DEL   = "Görev numarasının son tarihini kaldırın: "
 MSG_TS_DEAD_DATE  = "Son tarih ekleyin (YYYY/MM/DD): "
 MSG_WEATHER       = "Hava durumu yükleniyor..."
 MSG_ERRORS        = "Errors have occurred. See info.log in your config folder."
 MSG_GOTO          = "Go to date (YYYY/MM/DD): "
 MSG_GOTO_G        = "Go to date: "
+MSG_INPUT         = "Incorrect input."
 
 CALENDAR_HINT     = "Space · Günlüğe geç   a · Etkinlik ekle  n/p · Ayı değiştir   ? · Tüm tuş atamaları"
 CALENDAR_HINT_D   = "Space · Günlüğe geç   a · Etkinlik ekle  n/p · Günü değiştir   ? · Tüm tuş atamaları"
 JOURNAL_HINT      = "Space · Takvime geç   a · Görev ekle   d · Tamamlandı   i · Önemli   ? · Tüm tuş atamaları"
 
 DAYS = ["PAZARTESİ", "SALI", "ÇARŞAMBA", "PERŞEMBE", "CUMA", "CUMARTESİ", "PAZAR"]
 DAYS_PERSIAN = ["SHANBEH", "YEKSHANBEH", "DOSHANBEH", "SESHANBEH", "CHAHARSHANBEH", "PANJSHANBEH", "JOMEH"]
```

### Comparing `calcure-2.9.1/calcure/translations/zh.py` & `calcure-2.9.2/calcure/translations/zh.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 MSG_TS_PRIVACY    = "切换为隐私模式的事件号码: "
 MSG_TS_DEAD_ADD   = "增加截至日期为事件号码: "
 MSG_TS_DEAD_DEL   = "移除截止日期为事件号码: "
 MSG_TS_DEAD_DATE  = "增加截至日期在(YYYY/MM/DD): "
 MSG_WEATHER       = "天气插件正在加载..."
 MSG_ERRORS        = "Errors have occurred. See info.log in your config folder."
 MSG_GOTO          = "Go to date (YYYY/MM/DD): "
+MSG_INPUT         = "Incorrect input."
 
 CALENDAR_HINT     = "Space · 转换到通知栏   a · 增加事件  n/p · 改变月   ? · 所有键位绑定"
 CALENDAR_HINT_D   = "Space · 转换到通知栏   a · 增加事件  n/p · 改变日   ? · 所有键位绑定"
 JOURNAL_HINT      = "Space · 转换到日历栏   a · 增加任务   v · 已完成   i · 重要的   ? · 所有键位绑定"
 
 DAYS = ["周一", "周二", "周三", "周四", "周五", "周六", "周日"]
 DAYS_PERSIAN = ["SHANBEH", "YEKSHANBEH", "DOSHANBEH", "SESHANBEH", "CHAHARSHANBEH", "PANJSHANBEH", "JOMEH"]
```

### Comparing `calcure-2.9.1/calcure/weather.py` & `calcure-2.9.2/calcure/weather.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.1/calcure.egg-info/PKG-INFO` & `calcure-2.9.2/calcure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcure
-Version: 2.9.1
+Version: 2.9.2
 Summary: Modern TUI calendar and task manager
 Home-page: https://github.com/anufrievroman/calcure
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calcure-2.9.1/calcure.egg-info/SOURCES.txt` & `calcure-2.9.2/calcure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calcure-2.9.1/setup.py` & `calcure-2.9.2/setup.py`

 * *Files identical despite different names*

