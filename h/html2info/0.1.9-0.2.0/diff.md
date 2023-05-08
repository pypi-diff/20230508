# Comparing `tmp/html2info-0.1.9.tar.gz` & `tmp/html2info-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2info-0.1.9.tar", last modified: Fri May  5 19:17:15 2023, max compression
+gzip compressed data, was "html2info-0.2.0.tar", last modified: Mon May  8 02:27:39 2023, max compression
```

## Comparing `html2info-0.1.9.tar` & `html2info-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-05 19:17:15.536865 html2info-0.1.9/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-05-05 19:17:15.536865 html2info-0.1.9/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5278 2023-04-20 20:54:37.000000 html2info-0.1.9/README.md
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-05 19:17:15.536865 html2info-0.1.9/html2info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 18:56:39.000000 html2info-0.1.9/html2info/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6157 2023-05-05 19:14:12.000000 html2info-0.1.9/html2info/linkedin.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      439 2023-04-23 00:43:09.000000 html2info-0.1.9/html2info/types.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      190 2023-04-19 19:16:29.000000 html2info-0.1.9/html2info/utils.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-05 19:17:15.536865 html2info-0.1.9/html2info.egg-info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-05-05 19:17:15.000000 html2info-0.1.9/html2info.egg-info/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      279 2023-05-05 19:17:15.000000 html2info-0.1.9/html2info.egg-info/SOURCES.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-05-05 19:17:15.000000 html2info-0.1.9/html2info.egg-info/dependency_links.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       23 2023-05-05 19:17:15.000000 html2info-0.1.9/html2info.egg-info/requires.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       10 2023-05-05 19:17:15.000000 html2info-0.1.9/html2info.egg-info/top_level.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1475 2023-04-23 00:41:00.000000 html2info-0.1.9/pyproject.toml
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-05-05 19:17:15.536865 html2info-0.1.9/setup.cfg
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1360 2023-05-05 19:16:44.000000 html2info-0.1.9/setup.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-08 02:27:39.284418 html2info-0.2.0/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     8303 2023-05-08 02:27:39.280418 html2info-0.2.0/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     7568 2023-05-08 02:27:33.000000 html2info-0.2.0/README.md
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-08 02:27:39.280418 html2info-0.2.0/html2info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 18:56:39.000000 html2info-0.2.0/html2info/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     4737 2023-05-08 02:27:33.000000 html2info-0.2.0/html2info/kaggle.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6140 2023-05-08 02:27:33.000000 html2info-0.2.0/html2info/linkedin.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-08 02:27:39.280418 html2info-0.2.0/html2info/types/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-05-08 02:27:33.000000 html2info-0.2.0/html2info/types/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      461 2023-05-08 02:27:33.000000 html2info-0.2.0/html2info/types/kaggle.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      439 2023-05-08 02:27:33.000000 html2info-0.2.0/html2info/types/linkedin.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      190 2023-04-19 19:16:29.000000 html2info-0.2.0/html2info/utils.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-08 02:27:39.280418 html2info-0.2.0/html2info.egg-info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     8303 2023-05-08 02:27:39.000000 html2info-0.2.0/html2info.egg-info/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      362 2023-05-08 02:27:39.000000 html2info-0.2.0/html2info.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-05-08 02:27:39.000000 html2info-0.2.0/html2info.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       43 2023-05-08 02:27:39.000000 html2info-0.2.0/html2info.egg-info/requires.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       10 2023-05-08 02:27:39.000000 html2info-0.2.0/html2info.egg-info/top_level.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1475 2023-04-23 00:41:00.000000 html2info-0.2.0/pyproject.toml
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-05-08 02:27:39.284418 html2info-0.2.0/setup.cfg
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1360 2023-05-08 02:27:33.000000 html2info-0.2.0/setup.py
```

### Comparing `html2info-0.1.9/PKG-INFO` & `html2info-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2info
-Version: 0.1.9
+Version: 0.2.0
 Summary: A package to parse raw HTML and return structured information.
 Author: Vladimir Iglovikov
 Author-email: iglovikov@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,28 +34,30 @@
 pip install html2info
 ```
 
 ## Usage
 
 Here's an example of how to use html2info:
 
+### LinkedIn
+
 ```python
 from html2info.linkedin import Person
 
-url = "https://www.linkedin.com/in/iglovikov/"
+url = "https://www.linkedin.com/in/iglovikov"
 raw_data = "..."  # Raw HTML content of the LinkedIn page
 
 person = Person(url, raw_data)
 person.parse()
 print(person.to_dict())
 ```
 
 ```json
 {
-    "linkedin_url": "https://www.linkedin.com/in/iglovikov/",
+    "linkedin_url": "https://www.linkedin.com/in/iglovikov",
     "name": "Vladimir Iglovikov",
     "title": "Kaggle Grandmaster. Co-creator of Albumentations.AI",
     "location": "San Francisco, California, United States",
     "profile_photo_link": "https://media.licdn.com/dms/image/C4D03AQFDvheHDkAQlw/profile-displayphoto-shrink_400_400/0/1654539436934?e=1687392000&v=beta&t=OX7WrIprduo-xWEvrRKNzYdqcqG6bdzDtlm6LWuHbIE",
     "about": "• Advisor and Angel investor.\n• Co-creator, Albumentations.AI: Open-source library with 30k daily downloads, adopted by top Computer Vision companies & Kaggle competition winners\n• Former Staff ML Engineer, Lyft Level5 (Autonomous Vehicles): Led Deep Learning model development & integration for Self-Driving & Ride Sharing\n• Kaggle Grandmaster: Multiple ML competition wins\n• Author: 20+ publications in Deep Learning for Medical, Satellite, Street View, and Natural Images",
     "experience": [
       {
@@ -113,7 +115,80 @@
         "dates": "2001 - 2010",
         "university_link": "https://www.linkedin.com/company/15099991/",
         "image_link": "https://media.licdn.com/dms/image/C560BAQHWUjwogE235A/company-logo_100_100/0/1519863922741?e=1689811200&v=beta&t=DSpsTKY_AcMrmzWY1592EvCClph4M_TVOLdNSDpOg2I"
       }
     ]
   }
 ```
+
+### Kaggle
+
+```python
+from html2info.kaggle import Person
+
+url = "https://www.kaggle.com/iglovikov"
+raw_data = "..."  # Raw HTML content of the LinkedIn page
+
+person = Person(url, raw_data)
+person.parse()
+print(person.to_dict())
+```
+
+```json
+{
+    "url": "https://www.kaggle.com/iglovikov",
+    "name": "Vladimir Iglovikov",
+    "title": "CEO  at ternaus.com",
+    "location": "San Francisco, California, United States",
+    "profile_photo_link": "https://storage.googleapis.com/kaggle-avatars/images/286455-fb.jpg",
+    "social_network_links": [
+      "https://github.com/ternaus",
+      "https://twitter.com/viglovikov",
+      "https://www.linkedin.com/in/iglovikov",
+      "https://salesbrain.tech/"
+    ],
+    "personal_website_link": "https://salesbrain.tech/",
+    "num_followers": 1534,
+    "competitions_summary": {
+      "tier": "grandmaster",
+      "tier_image": "/static/images/tiers/grandmaster@48.png",
+      "medals": {
+        "gold": 5,
+        "silver": 9,
+        "bronze": 8
+      },
+      "highest_rank": 19
+    },
+    "datasets_summary": {
+      "tier": "contributor",
+      "tier_image": "/static/images/tiers/contributor@48.png",
+      "medals": {
+        "gold": 0,
+        "silver": 0,
+        "bronze": 0
+      },
+      "highest_rank": -1
+    },
+    "notebooks_summary": {
+      "tier": "contributor",
+      "tier_image": "/static/images/tiers/contributor@48.png",
+      "medals": {
+        "gold": 1,
+        "silver": 1,
+        "bronze": 1
+      },
+      "highest_rank": -1
+    },
+    "discussion_summary": {
+      "tier": "master",
+      "tier_image": "/static/images/tiers/master@48.png",
+      "medals": {
+        "gold": 52,
+        "silver": 26,
+        "bronze": 177
+      },
+      "highest_rank": 6
+    },
+    "bio": "* CEO at Ternaus Inc\n* Staff Computer Vision Engineer at Level5 Engineering Center, Lyft Inc (2017-2021)\n* Senior Data Scientist at TrueAccord (2016-2017)\n* Data Scientist at Bidgely (2015-2016)\n* PhD in theoretical Condensed Matter Physics at University of California, Davis (2010-2015)\n* MS in theoretical High Energy Physics at Saint Petersburg State University (2001-2010)\n* Спецназ ВДВ . Медаль за воинскую доблесть за вторую Чеченскую. (2002-2004)\n"
+  }
+
+```
```

### Comparing `html2info-0.1.9/README.md` & `html2info-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -15,28 +15,30 @@
 pip install html2info
 ```
 
 ## Usage
 
 Here's an example of how to use html2info:
 
+### LinkedIn
+
 ```python
 from html2info.linkedin import Person
 
-url = "https://www.linkedin.com/in/iglovikov/"
+url = "https://www.linkedin.com/in/iglovikov"
 raw_data = "..."  # Raw HTML content of the LinkedIn page
 
 person = Person(url, raw_data)
 person.parse()
 print(person.to_dict())
 ```
 
 ```json
 {
-    "linkedin_url": "https://www.linkedin.com/in/iglovikov/",
+    "linkedin_url": "https://www.linkedin.com/in/iglovikov",
     "name": "Vladimir Iglovikov",
     "title": "Kaggle Grandmaster. Co-creator of Albumentations.AI",
     "location": "San Francisco, California, United States",
     "profile_photo_link": "https://media.licdn.com/dms/image/C4D03AQFDvheHDkAQlw/profile-displayphoto-shrink_400_400/0/1654539436934?e=1687392000&v=beta&t=OX7WrIprduo-xWEvrRKNzYdqcqG6bdzDtlm6LWuHbIE",
     "about": "• Advisor and Angel investor.\n• Co-creator, Albumentations.AI: Open-source library with 30k daily downloads, adopted by top Computer Vision companies & Kaggle competition winners\n• Former Staff ML Engineer, Lyft Level5 (Autonomous Vehicles): Led Deep Learning model development & integration for Self-Driving & Ride Sharing\n• Kaggle Grandmaster: Multiple ML competition wins\n• Author: 20+ publications in Deep Learning for Medical, Satellite, Street View, and Natural Images",
     "experience": [
       {
@@ -94,7 +96,80 @@
         "dates": "2001 - 2010",
         "university_link": "https://www.linkedin.com/company/15099991/",
         "image_link": "https://media.licdn.com/dms/image/C560BAQHWUjwogE235A/company-logo_100_100/0/1519863922741?e=1689811200&v=beta&t=DSpsTKY_AcMrmzWY1592EvCClph4M_TVOLdNSDpOg2I"
       }
     ]
   }
 ```
+
+### Kaggle
+
+```python
+from html2info.kaggle import Person
+
+url = "https://www.kaggle.com/iglovikov"
+raw_data = "..."  # Raw HTML content of the LinkedIn page
+
+person = Person(url, raw_data)
+person.parse()
+print(person.to_dict())
+```
+
+```json
+{
+    "url": "https://www.kaggle.com/iglovikov",
+    "name": "Vladimir Iglovikov",
+    "title": "CEO  at ternaus.com",
+    "location": "San Francisco, California, United States",
+    "profile_photo_link": "https://storage.googleapis.com/kaggle-avatars/images/286455-fb.jpg",
+    "social_network_links": [
+      "https://github.com/ternaus",
+      "https://twitter.com/viglovikov",
+      "https://www.linkedin.com/in/iglovikov",
+      "https://salesbrain.tech/"
+    ],
+    "personal_website_link": "https://salesbrain.tech/",
+    "num_followers": 1534,
+    "competitions_summary": {
+      "tier": "grandmaster",
+      "tier_image": "/static/images/tiers/grandmaster@48.png",
+      "medals": {
+        "gold": 5,
+        "silver": 9,
+        "bronze": 8
+      },
+      "highest_rank": 19
+    },
+    "datasets_summary": {
+      "tier": "contributor",
+      "tier_image": "/static/images/tiers/contributor@48.png",
+      "medals": {
+        "gold": 0,
+        "silver": 0,
+        "bronze": 0
+      },
+      "highest_rank": -1
+    },
+    "notebooks_summary": {
+      "tier": "contributor",
+      "tier_image": "/static/images/tiers/contributor@48.png",
+      "medals": {
+        "gold": 1,
+        "silver": 1,
+        "bronze": 1
+      },
+      "highest_rank": -1
+    },
+    "discussion_summary": {
+      "tier": "master",
+      "tier_image": "/static/images/tiers/master@48.png",
+      "medals": {
+        "gold": 52,
+        "silver": 26,
+        "bronze": 177
+      },
+      "highest_rank": 6
+    },
+    "bio": "* CEO at Ternaus Inc\n* Staff Computer Vision Engineer at Level5 Engineering Center, Lyft Inc (2017-2021)\n* Senior Data Scientist at TrueAccord (2016-2017)\n* Data Scientist at Bidgely (2015-2016)\n* PhD in theoretical Condensed Matter Physics at University of California, Davis (2010-2015)\n* MS in theoretical High Energy Physics at Saint Petersburg State University (2001-2010)\n* Спецназ ВДВ . Медаль за воинскую доблесть за вторую Чеченскую. (2002-2004)\n"
+  }
+
+```
```

### Comparing `html2info-0.1.9/html2info/linkedin.py` & `html2info-0.2.0/html2info/linkedin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import re
 from typing import Optional
 
 from bs4 import BeautifulSoup
 
-from html2info.types import EducationType, ExperienceType
+from html2info.types.linkedin import EducationType, ExperienceType
 
 
 class Person:
     def __init__(self, linkedin_url: str, raw_html: str) -> None:
         self.soup = BeautifulSoup(raw_html, "html.parser")
         self.linkedin_url = linkedin_url.strip().rstrip("/")
 
         self.name = None
         self.title = None
         self.location = None
         self.profile_photo_link = None
         self.about = None
         self.experience: list[ExperienceType] = []
         self.education_list: list[EducationType] = []
-        self.about = None
 
     def parse(self):
         self.name = self.soup.find("h1").text.strip()
         self.title = self.soup.find("div", class_="text-body-medium").text.strip()
 
         self.location = self.soup.find("span", class_="text-body-small inline t-black--light break-words").text.strip()
```

### Comparing `html2info-0.1.9/html2info.egg-info/PKG-INFO` & `html2info-0.2.0/html2info.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2info
-Version: 0.1.9
+Version: 0.2.0
 Summary: A package to parse raw HTML and return structured information.
 Author: Vladimir Iglovikov
 Author-email: iglovikov@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,28 +34,30 @@
 pip install html2info
 ```
 
 ## Usage
 
 Here's an example of how to use html2info:
 
+### LinkedIn
+
 ```python
 from html2info.linkedin import Person
 
-url = "https://www.linkedin.com/in/iglovikov/"
+url = "https://www.linkedin.com/in/iglovikov"
 raw_data = "..."  # Raw HTML content of the LinkedIn page
 
 person = Person(url, raw_data)
 person.parse()
 print(person.to_dict())
 ```
 
 ```json
 {
-    "linkedin_url": "https://www.linkedin.com/in/iglovikov/",
+    "linkedin_url": "https://www.linkedin.com/in/iglovikov",
     "name": "Vladimir Iglovikov",
     "title": "Kaggle Grandmaster. Co-creator of Albumentations.AI",
     "location": "San Francisco, California, United States",
     "profile_photo_link": "https://media.licdn.com/dms/image/C4D03AQFDvheHDkAQlw/profile-displayphoto-shrink_400_400/0/1654539436934?e=1687392000&v=beta&t=OX7WrIprduo-xWEvrRKNzYdqcqG6bdzDtlm6LWuHbIE",
     "about": "• Advisor and Angel investor.\n• Co-creator, Albumentations.AI: Open-source library with 30k daily downloads, adopted by top Computer Vision companies & Kaggle competition winners\n• Former Staff ML Engineer, Lyft Level5 (Autonomous Vehicles): Led Deep Learning model development & integration for Self-Driving & Ride Sharing\n• Kaggle Grandmaster: Multiple ML competition wins\n• Author: 20+ publications in Deep Learning for Medical, Satellite, Street View, and Natural Images",
     "experience": [
       {
@@ -113,7 +115,80 @@
         "dates": "2001 - 2010",
         "university_link": "https://www.linkedin.com/company/15099991/",
         "image_link": "https://media.licdn.com/dms/image/C560BAQHWUjwogE235A/company-logo_100_100/0/1519863922741?e=1689811200&v=beta&t=DSpsTKY_AcMrmzWY1592EvCClph4M_TVOLdNSDpOg2I"
       }
     ]
   }
 ```
+
+### Kaggle
+
+```python
+from html2info.kaggle import Person
+
+url = "https://www.kaggle.com/iglovikov"
+raw_data = "..."  # Raw HTML content of the LinkedIn page
+
+person = Person(url, raw_data)
+person.parse()
+print(person.to_dict())
+```
+
+```json
+{
+    "url": "https://www.kaggle.com/iglovikov",
+    "name": "Vladimir Iglovikov",
+    "title": "CEO  at ternaus.com",
+    "location": "San Francisco, California, United States",
+    "profile_photo_link": "https://storage.googleapis.com/kaggle-avatars/images/286455-fb.jpg",
+    "social_network_links": [
+      "https://github.com/ternaus",
+      "https://twitter.com/viglovikov",
+      "https://www.linkedin.com/in/iglovikov",
+      "https://salesbrain.tech/"
+    ],
+    "personal_website_link": "https://salesbrain.tech/",
+    "num_followers": 1534,
+    "competitions_summary": {
+      "tier": "grandmaster",
+      "tier_image": "/static/images/tiers/grandmaster@48.png",
+      "medals": {
+        "gold": 5,
+        "silver": 9,
+        "bronze": 8
+      },
+      "highest_rank": 19
+    },
+    "datasets_summary": {
+      "tier": "contributor",
+      "tier_image": "/static/images/tiers/contributor@48.png",
+      "medals": {
+        "gold": 0,
+        "silver": 0,
+        "bronze": 0
+      },
+      "highest_rank": -1
+    },
+    "notebooks_summary": {
+      "tier": "contributor",
+      "tier_image": "/static/images/tiers/contributor@48.png",
+      "medals": {
+        "gold": 1,
+        "silver": 1,
+        "bronze": 1
+      },
+      "highest_rank": -1
+    },
+    "discussion_summary": {
+      "tier": "master",
+      "tier_image": "/static/images/tiers/master@48.png",
+      "medals": {
+        "gold": 52,
+        "silver": 26,
+        "bronze": 177
+      },
+      "highest_rank": 6
+    },
+    "bio": "* CEO at Ternaus Inc\n* Staff Computer Vision Engineer at Level5 Engineering Center, Lyft Inc (2017-2021)\n* Senior Data Scientist at TrueAccord (2016-2017)\n* Data Scientist at Bidgely (2015-2016)\n* PhD in theoretical Condensed Matter Physics at University of California, Davis (2010-2015)\n* MS in theoretical High Energy Physics at Saint Petersburg State University (2001-2010)\n* Спецназ ВДВ . Медаль за воинскую доблесть за вторую Чеченскую. (2002-2004)\n"
+  }
+
+```
```

### Comparing `html2info-0.1.9/pyproject.toml` & `html2info-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `html2info-0.1.9/setup.py` & `html2info-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="html2info",  # Replace with your package name
-    version="0.1.9",  # Replace with your package version
+    version="0.2.0",  # Replace with your package version
     author="Vladimir Iglovikov",  # Replace with your name
     author_email="iglovikov@gmail.com",  # Replace with your email
     description="A package to parse raw HTML and return structured information.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
     classifiers=[
```

