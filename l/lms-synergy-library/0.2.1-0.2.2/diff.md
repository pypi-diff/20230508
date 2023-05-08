# Comparing `tmp/lms_synergy_library-0.2.1.tar.gz` & `tmp/lms_synergy_library-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lms_synergy_library-0.2.1.tar", last modified: Sat May  6 12:40:10 2023, max compression
+gzip compressed data, was "lms_synergy_library-0.2.2.tar", last modified: Mon May  8 18:24:04 2023, max compression
```

## Comparing `lms_synergy_library-0.2.1.tar` & `lms_synergy_library-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:40:10.723807 lms_synergy_library-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-06 12:39:31.000000 lms_synergy_library-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-06 12:40:10.723807 lms_synergy_library-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-06 12:39:31.000000 lms_synergy_library-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:40:10.723807 lms_synergy_library-0.2.1/lms_synergy_library/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-06 12:39:31.000000 lms_synergy_library-0.2.1/lms_synergy_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-06 12:39:31.000000 lms_synergy_library-0.2.1/lms_synergy_library/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-06 12:39:31.000000 lms_synergy_library-0.2.1/lms_synergy_library/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27518 2023-05-06 12:39:31.000000 lms_synergy_library-0.2.1/lms_synergy_library/lms_synergy_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-06 12:39:31.000000 lms_synergy_library-0.2.1/lms_synergy_library/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:40:10.723807 lms_synergy_library-0.2.1/lms_synergy_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-06 12:40:10.000000 lms_synergy_library-0.2.1/lms_synergy_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-06 12:40:10.000000 lms_synergy_library-0.2.1/lms_synergy_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 12:40:10.000000 lms_synergy_library-0.2.1/lms_synergy_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-06 12:40:10.000000 lms_synergy_library-0.2.1/lms_synergy_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 12:40:10.000000 lms_synergy_library-0.2.1/lms_synergy_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-06 12:39:31.000000 lms_synergy_library-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 12:40:10.723807 lms_synergy_library-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:40:10.723807 lms_synergy_library-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-06 12:39:31.000000 lms_synergy_library-0.2.1/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:24:04.554385 lms_synergy_library-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-08 18:23:36.000000 lms_synergy_library-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-08 18:24:04.554385 lms_synergy_library-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-08 18:23:36.000000 lms_synergy_library-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:24:04.554385 lms_synergy_library-0.2.2/lms_synergy_library/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 18:23:36.000000 lms_synergy_library-0.2.2/lms_synergy_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-08 18:23:36.000000 lms_synergy_library-0.2.2/lms_synergy_library/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-08 18:23:36.000000 lms_synergy_library-0.2.2/lms_synergy_library/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32844 2023-05-08 18:23:36.000000 lms_synergy_library-0.2.2/lms_synergy_library/lms_synergy_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-08 18:23:36.000000 lms_synergy_library-0.2.2/lms_synergy_library/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:24:04.554385 lms_synergy_library-0.2.2/lms_synergy_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-08 18:24:04.000000 lms_synergy_library-0.2.2/lms_synergy_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-08 18:24:04.000000 lms_synergy_library-0.2.2/lms_synergy_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:24:04.000000 lms_synergy_library-0.2.2/lms_synergy_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-08 18:24:04.000000 lms_synergy_library-0.2.2/lms_synergy_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 18:24:04.000000 lms_synergy_library-0.2.2/lms_synergy_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-08 18:23:36.000000 lms_synergy_library-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:24:04.554385 lms_synergy_library-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:24:04.554385 lms_synergy_library-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-08 18:23:36.000000 lms_synergy_library-0.2.2/tests/tests.py
```

### Comparing `lms_synergy_library-0.2.1/LICENSE` & `lms_synergy_library-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lms_synergy_library-0.2.1/PKG-INFO` & `lms_synergy_library-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lms_synergy_library
-Version: 0.2.1
+Version: 0.2.2
 Summary: A library that allows you to work with LMS
 Author-email: Nikita Kovinjko <kotorkovsciy@gmail.com>
 Project-URL: Homepage, https://github.com/kotorkovsciy/lms-synergy-library
 Project-URL: Bug Tracker, https://github.com/kotorkovsciy/lms-synergy-library/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -65,14 +65,20 @@
 
 # get notifications archive
 lms.get_notify_archive()
 
 # get unread messages
 lms.get_unread_messages()
 
+# get marks
+lms.get_marks()
+
+# get events
+lms.get_events()
+
 ```
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
```

### Comparing `lms_synergy_library-0.2.1/README.md` & `lms_synergy_library-0.2.2/lms_synergy_library.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: lms-synergy-library
+Version: 0.2.2
+Summary: A library that allows you to work with LMS
+Author-email: Nikita Kovinjko <kotorkovsciy@gmail.com>
+Project-URL: Homepage, https://github.com/kotorkovsciy/lms-synergy-library
+Project-URL: Bug Tracker, https://github.com/kotorkovsciy/lms-synergy-library/issues
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # lms-synergy-library
 
 This unofficial library is a collection of useful functions for the LMS Synergy platform.
 
 ## Installation
 
 ```bash
@@ -50,14 +65,20 @@
 
 # get notifications archive
 lms.get_notify_archive()
 
 # get unread messages
 lms.get_unread_messages()
 
+# get marks
+lms.get_marks()
+
+# get events
+lms.get_events()
+
 ```
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
```

### Comparing `lms_synergy_library-0.2.1/lms_synergy_library/constants.py` & `lms_synergy_library-0.2.2/lms_synergy_library/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,11 +6,12 @@
 URL_SCHEDULE: Final[str] = "%s/schedule/academ" % URL
 URL_NEWS: Final[str] = "%s/announce" % URL
 URL_EDUCATION: Final[str] = "%s/student/up" % URL
 URL_NOTIFY: Final[str] = "%s/student/notifications" % URL
 URL_NOTIFY_ARCHIVE: Final[str] = "%s/archive" % URL_NOTIFY
 URL_MESSAGES: Final[str] = "%s/messages/listing" % URL
 URL_MESSAGES_UNREAD: Final[str] = "%s/status/unread" % URL_MESSAGES
+URL_JOURNAL: Final[str] = "%s/student/journal" % URL
 URLS_LANGUAGES: Final[dict] = {
         "ru": "%s/user/lng/1" % URL,
         "en": "%s/user/lng/2" % URL,
 }
```

### Comparing `lms_synergy_library-0.2.1/lms_synergy_library/lms_synergy_library.py` & `lms_synergy_library-0.2.2/lms_synergy_library/lms_synergy_library.py`

 * *Files 9% similar despite different names*

```diff
@@ -594,21 +594,26 @@
             )
             if currentScore == "": currentScore = "-"
 
             finalGrade: str = clean_data.remove_many_spaces(
                 tr.find_all("td")[4].text
             )
             if finalGrade == "": finalGrade = "-"
+            
+            url: str = tr.find_all("td")[1].find("a")
+            if url: url = "%s%s" % (URL, url["href"])
+            else: url = "-"
 
             disciplines.append(
                 {
                     "title": title,
                     "typeOfControl": typeOfControl,
                     "currentScore": currentScore,
-                    "finalGrade": finalGrade
+                    "finalGrade": finalGrade,
+                    "url": url
                 }
             )
         
         return disciplines
 
     def get_pesonal_curators(self) -> list:
         """Returns personal curators
@@ -922,7 +927,149 @@
                         "subject": subject,
                         "date": date,
                         "url": url
                     }
                 )
 
         return messages
+    
+    def get_marks(self) -> list:
+        """Returns marks
+
+        :return: marks
+        :rtype: list
+
+        :Example:
+
+        >>> from lms_synergy_library import LMS
+        >>> lms = LMS(login="demo", password="demo")
+        >>> marks = lms.get_marks()
+        >>> # marks
+        >>> # [
+        >>> #   {
+        >>> #       "discipline": "Discipline",
+        >>> #       "type_discipline": "Type_discipline",
+        >>> #       "teacher": "Teacher",
+        >>> #       "date_discipline": "Date_discipline",
+        >>> #       "time_discipline": "Time_discipline",
+        >>> #       "mark": "Mark",
+        >>> #       "hours": "Hours"
+        >>> #   },
+        >>> # ]
+        """
+
+        soup: bs = SoupLms.get_soup_journal(
+                session=self.session,
+                language=self.language,
+                cookies=self.cookies,
+                proxies=self.proxy,
+        )
+        
+        table: bs = soup.find("table", {"class": "table-list dataTable"})
+        marks: list = []
+
+        for tr in table.find_all("tr", {"id": "entryId"}):
+            if len(tr.find_all("td")) == 1:
+                return marks
+            else:
+                discipline: str = clean_data.remove_many_spaces(tr.find_all("td")[0].text)
+                type_discipline: str = clean_data.remove_many_spaces(tr.find_all("td")[1].text)
+                teacher: str = clean_data.remove_many_spaces(tr.find_all("td")[2].text)
+                date_discipline: str = clean_data.remove_many_spaces(tr.find_all("td")[3].text)
+                time_discipline: str = clean_data.remove_many_spaces(tr.find_all("td")[4].text)
+                mark: str = clean_data.remove_many_spaces(tr.find_all("td")[5].text)
+                hours: str = clean_data.remove_many_spaces(tr.find_all("td")[6].text)
+
+                marks.append(
+                    {
+                        "discipline": discipline,
+                        "type_discipline": type_discipline,
+                        "teacher": teacher,
+                        "date_discipline": date_discipline,
+                        "time_discipline": time_discipline,
+                        "mark": mark,
+                        "hours": hours
+                    }
+                )
+
+        return marks
+    
+    def get_events(self):
+        """Returns event
+
+        :return: event
+        :rtype: list
+
+        :Example:
+
+        >>> from lms_synergy_library import LMS
+        >>> lms = LMS(login="demo", password="demo")
+        >>> events = lms.get_events()
+        >>> # events
+        >>> # [
+        >>> #   {
+        >>> #       "discipline": {
+        >>> #               "current_grade": "Current_grade",
+        >>> #               "events": [
+        >>> #                           {
+        >>> #                               "name": "Name",
+        >>> #                               "access": "Access",
+        >>> #                               "max_grade": "Max_grade",
+        >>> #                               "result": "Result",
+        >>> #                               "url": "Url"
+        >>> #                           },
+        >>> #               ]
+        >>> #       },
+        >>> #   },       
+        >>> # ]
+        """
+
+        disciplines = self.get_disciplines()
+        info_disciplines = []
+
+        for discipline in disciplines:
+            if discipline["url"] == "-":
+                continue
+            soup: bs = SoupLms.get_soup_events(
+                session=self.session,
+                language=self.language,
+                cookies=self.cookies,
+                proxies=self.proxy,
+                url=discipline["url"]
+            )
+
+            table: bs = soup.find("table", {"class": "table-list"})
+            events: list = []
+
+            for tr in table.find("tbody").find_all("tr"):
+                if len(tr.find_all("td")) == 1:
+                    continue
+                name: str = clean_data.remove_many_spaces(tr.find_all("td")[0].text)
+                access: str = clean_data.remove_many_spaces(tr.find_all("td")[1].text)
+                max_grade: str = clean_data.remove_many_spaces(tr.find_all("td")[2].text)
+                result: str = clean_data.remove_many_spaces(tr.find_all("td")[3].text)
+                if result == "": result = "-"
+                url: str = tr.find_all("td")[0].find("a")
+                if url: url = "%s%s" % (URL, url["href"])
+                else: url = "-"
+
+                events.append(
+                    {
+                        "name": name,
+                        "access": access,
+                        "max_grade": max_grade,
+                        "result": result,
+                        "url": url
+                    }
+                )
+            
+            current_grade = table.find("tfoot").find_all("td")
+
+            info_disciplines.append(
+                {
+                    discipline["title"]: {
+                        "current_grade": clean_data.remove_many_spaces(current_grade[-1].text), 
+                        "events": events
+                    },
+                }
+            )
+        return info_disciplines
```

### Comparing `lms_synergy_library-0.2.1/lms_synergy_library/utils.py` & `lms_synergy_library-0.2.2/lms_synergy_library/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from requests import Response, Session
 from bs4 import BeautifulSoup as bs
 from .constants import URL_EDUCATION, URL_NEWS, URL_SCHEDULE, URLS_LANGUAGES, URL_NOTIFY,\
-     URL_NOTIFY_ARCHIVE, URL_MESSAGES_UNREAD, URL
+     URL_NOTIFY_ARCHIVE, URL_MESSAGES_UNREAD, URL, URL_JOURNAL
 from .exceptions import PageNotExist
 
 
 class clean_data:
     @staticmethod
     def remove_many_spaces(string):
         return " ".join(string.split())
@@ -341,7 +341,56 @@
                 proxies=proxies
             )
             soup = bs(response.content, 'html.parser')
             paginator_links: bs = soup.select('.paginator a')
             next_link = "%s%s" % (URL, paginator_links[-1]["href"])
 
         return amount_pages
+    
+    @staticmethod
+    def get_soup_journal(session: Session, language: str, cookies: dict, proxies: dict) -> bs:
+        """ Returns journal
+
+        :param session: Session
+        :param language: Language
+        :param cookies: Cookies
+        :param proxies: Proxies
+
+        :type session: Session
+        :type language: str
+        :type cookies: dict
+        :type proxies: dict
+
+        :return: Journal page
+        :rtype: bs4.BeautifulSoup
+        """
+        session.get(URLS_LANGUAGES[language], cookies=cookies, proxies=proxies)
+
+        response: Response = session.get(URL_JOURNAL, cookies=cookies, proxies=proxies)
+
+        return bs(response.text, "html.parser")
+    
+    @staticmethod
+    def get_soup_events(session: Session, language: str, cookies: dict, proxies: dict, url: str) -> bs:
+        """ Returns soup events
+
+        :param session: Session
+        :param language: Language
+        :param cookies: Cookies
+        :param proxies: Proxies
+        :param url: Url
+
+        :type session: Session
+        :type language: str
+        :type cookies: dict
+        :type proxies: dict
+        :type url: str
+
+        :return: Soup events
+        :rtype: bs4.BeautifulSoup
+        """
+        
+        session.get(URLS_LANGUAGES[language], cookies=cookies, proxies=proxies)
+
+        response: Response = session.get(url, cookies=cookies, proxies=proxies)
+
+        return bs(response.text, "html.parser")
```

### Comparing `lms_synergy_library-0.2.1/lms_synergy_library.egg-info/PKG-INFO` & `lms_synergy_library-0.2.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: lms-synergy-library
-Version: 0.2.1
-Summary: A library that allows you to work with LMS
-Author-email: Nikita Kovinjko <kotorkovsciy@gmail.com>
-Project-URL: Homepage, https://github.com/kotorkovsciy/lms-synergy-library
-Project-URL: Bug Tracker, https://github.com/kotorkovsciy/lms-synergy-library/issues
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # lms-synergy-library
 
 This unofficial library is a collection of useful functions for the LMS Synergy platform.
 
 ## Installation
 
 ```bash
@@ -65,14 +50,20 @@
 
 # get notifications archive
 lms.get_notify_archive()
 
 # get unread messages
 lms.get_unread_messages()
 
+# get marks
+lms.get_marks()
+
+# get events
+lms.get_events()
+
 ```
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
```

### Comparing `lms_synergy_library-0.2.1/pyproject.toml` & `lms_synergy_library-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lms_synergy_library"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     {name = "Nikita Kovinjko", email = "kotorkovsciy@gmail.com"},
 ]
 description = "A library that allows you to work with LMS"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

