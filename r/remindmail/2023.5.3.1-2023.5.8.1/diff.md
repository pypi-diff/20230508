# Comparing `tmp/remindmail-2023.5.3.1.tar.gz` & `tmp/remindmail-2023.5.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2023.5.3.1.tar", last modified: Wed May  3 20:03:47 2023, max compression
+gzip compressed data, was "remindmail-2023.5.8.1.tar", last modified: Mon May  8 18:42:02 2023, max compression
```

## Comparing `remindmail-2023.5.3.1.tar` & `remindmail-2023.5.8.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-03 20:03:47.013663 remindmail-2023.5.3.1/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.5.3.1/LICENSE.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11997 2023-05-03 20:03:47.013663 remindmail-2023.5.3.1/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11649 2023-04-19 21:19:01.000000 remindmail-2023.5.3.1/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.5.3.1/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-05-03 20:03:47.013663 remindmail-2023.5.3.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-03 20:03:47.013663 remindmail-2023.5.3.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-03 20:03:47.013663 remindmail-2023.5.3.1/src/remind/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-04-30 04:24:17.000000 remindmail-2023.5.3.1/src/remind/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3323 2023-04-30 04:24:17.000000 remindmail-2023.5.3.1/src/remind/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2405 2023-04-30 04:24:17.000000 remindmail-2023.5.3.1/src/remind/reminder.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    25030 2023-05-03 20:03:29.000000 remindmail-2023.5.3.1/src/remind/remindmail.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     8189 2023-04-30 04:24:17.000000 remindmail-2023.5.3.1/src/remind/remindmail_utils.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-03 20:03:47.013663 remindmail-2023.5.3.1/src/remindmail.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11997 2023-05-03 20:03:47.000000 remindmail-2023.5.3.1/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      363 2023-05-03 20:03:47.000000 remindmail-2023.5.3.1/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-05-03 20:03:47.000000 remindmail-2023.5.3.1/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2023-05-03 20:03:47.000000 remindmail-2023.5.3.1/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-05-03 20:03:47.000000 remindmail-2023.5.3.1/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-08 18:42:02.052849 remindmail-2023.5.8.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.5.8.1/LICENSE.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11997 2023-05-08 18:42:02.052849 remindmail-2023.5.8.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11649 2023-04-19 21:19:01.000000 remindmail-2023.5.8.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.5.8.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-05-08 18:42:02.052849 remindmail-2023.5.8.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-08 18:42:02.048849 remindmail-2023.5.8.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-08 18:42:02.052849 remindmail-2023.5.8.1/src/remind/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-04-30 04:24:17.000000 remindmail-2023.5.8.1/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3323 2023-04-30 04:24:17.000000 remindmail-2023.5.8.1/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2405 2023-04-30 04:24:17.000000 remindmail-2023.5.8.1/src/remind/reminder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    25030 2023-05-03 20:03:29.000000 remindmail-2023.5.8.1/src/remind/remindmail.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     8342 2023-05-08 18:33:48.000000 remindmail-2023.5.8.1/src/remind/remindmail_utils.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-08 18:42:02.052849 remindmail-2023.5.8.1/src/remindmail.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11997 2023-05-08 18:42:02.000000 remindmail-2023.5.8.1/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      363 2023-05-08 18:42:02.000000 remindmail-2023.5.8.1/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-05-08 18:42:02.000000 remindmail-2023.5.8.1/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2023-05-08 18:42:02.000000 remindmail-2023.5.8.1/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-05-08 18:42:02.000000 remindmail-2023.5.8.1/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2023.5.3.1/LICENSE.md` & `remindmail-2023.5.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2023.5.3.1/PKG-INFO` & `remindmail-2023.5.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2023.5.3.1
+Version: 2023.5.8.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `remindmail-2023.5.3.1/README.md` & `remindmail-2023.5.8.1/README.md`

 * *Files identical despite different names*

### Comparing `remindmail-2023.5.3.1/setup.cfg` & `remindmail-2023.5.8.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = remindmail
-version = 2023.05.03.1
+version = 2023.05.08.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls =
```

### Comparing `remindmail-2023.5.3.1/src/remind/__main__.py` & `remindmail-2023.5.8.1/src/remind/__main__.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.5.3.1/src/remind/reminder.py` & `remindmail-2023.5.8.1/src/remind/reminder.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.5.3.1/src/remind/remindmail.py` & `remindmail-2023.5.8.1/src/remind/remindmail.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.5.3.1/src/remind/remindmail_utils.py` & `remindmail-2023.5.8.1/src/remind/remindmail_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,16 @@
             # user's timezone not saved in `cab`; get timezone based on IP
             print("Checking timezone...")
             response = requests.get('https://ipapi.co/json/', timeout=10)
 
             # parse the response JSON to get the user's timezone
             if response.status_code == 200:
                 data = response.json()
-                user_timezone = self.cab.put("remindmail", "timezone", data.get('timezone'))
+                user_timezone = self.cab.put(
+                    "remindmail", "timezone", data.get('timezone'))
                 print(f"Set timezone: {user_timezone}")
             else:
                 print("Could not parse timezone; using UTC")
                 return datetime.datetime.utcnow()
 
         timezone = pytz.timezone(user_timezone)
 
@@ -66,15 +67,14 @@
         utc_time = now + datetime.timedelta(seconds=offset)
 
         # convert the UTC time to the number of seconds since January 1, 1970
         unix_time = int(utc_time.timestamp())
 
         return unix_time
 
-
     def print_reminders_file(self, param=None):
         """
         Displays the scheduled reminders in remind.py, formatted with line numbers
         Usage: remindmail ls
         Parameters:
         - param: string; currently unused
 
@@ -204,14 +204,17 @@
                            f" and set path -> edit -> remind -> sync to true"
                            f" to enable cloud syncing."))
         sys.exit()
 
     def send_email(self, subject, body, method="Terminal", is_quiet=False):
         """A helper function to call mail.send"""
 
+        sent_today = self.cab.get("remindmail", "sent_today") or 0
+        self.cab.put("remindmail", "sent_today", sent_today + 1)
+
         print(f"Sending: {subject}")
 
         if body:
             subject = f"{subject} [See Notes]"
 
         body += f"<br><br>Sent via {method}"
```

### Comparing `remindmail-2023.5.3.1/src/remindmail.egg-info/PKG-INFO` & `remindmail-2023.5.8.1/src/remindmail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2023.5.3.1
+Version: 2023.5.8.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

