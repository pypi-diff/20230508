# Comparing `tmp/gsbg-0.1.1.tar.gz` & `tmp/gsbg-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsbg-0.1.1.tar", last modified: Sun Apr 30 15:17:50 2023, max compression
+gzip compressed data, was "gsbg-0.1.2.tar", last modified: Mon May  8 14:50:18 2023, max compression
```

## Comparing `gsbg-0.1.1.tar` & `gsbg-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:17:50.763956 gsbg-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-30 15:17:40.000000 gsbg-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 15:17:40.000000 gsbg-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-30 15:17:50.763956 gsbg-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-30 15:17:40.000000 gsbg-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:17:50.763956 gsbg-0.1.1/gsbg/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-30 15:17:40.000000 gsbg-0.1.1/gsbg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-04-30 15:17:40.000000 gsbg-0.1.1/gsbg/google_scholar_badge_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:17:50.763956 gsbg-0.1.1/gsbg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-30 15:17:50.000000 gsbg-0.1.1/gsbg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-30 15:17:50.000000 gsbg-0.1.1/gsbg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 15:17:50.000000 gsbg-0.1.1/gsbg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 15:17:50.000000 gsbg-0.1.1/gsbg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 15:17:50.000000 gsbg-0.1.1/gsbg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 15:17:50.763956 gsbg-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-30 15:17:40.000000 gsbg-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:50:18.779058 gsbg-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 14:50:10.000000 gsbg-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-08 14:50:10.000000 gsbg-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-08 14:50:18.779058 gsbg-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-08 14:50:10.000000 gsbg-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:50:18.775058 gsbg-0.1.2/gsbg/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-08 14:50:10.000000 gsbg-0.1.2/gsbg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-05-08 14:50:10.000000 gsbg-0.1.2/gsbg/google_scholar_badge_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:50:18.779058 gsbg-0.1.2/gsbg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-08 14:50:18.000000 gsbg-0.1.2/gsbg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-08 14:50:18.000000 gsbg-0.1.2/gsbg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:50:18.000000 gsbg-0.1.2/gsbg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-08 14:50:18.000000 gsbg-0.1.2/gsbg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 14:50:18.000000 gsbg-0.1.2/gsbg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 14:50:18.779058 gsbg-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-08 14:50:10.000000 gsbg-0.1.2/setup.py
```

### Comparing `gsbg-0.1.1/LICENSE` & `gsbg-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gsbg-0.1.1/PKG-INFO` & `gsbg-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: gsbg
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool for Google Scholar citation badge generation.
-Home-page: https://github.com/WenjieDu/GoogleScholarBadgeGenerator
-Download-URL: https://github.com/WenjieDu/GoogleScholarBadgeGenerator/archive/main.zip
+Home-page: https://github.com/WenjieDu/Google_Scholar_Badge_Generator
+Download-URL: https://github.com/WenjieDu/Google_Scholar_Badge_Generator/archive/main.zip
 Author: Wenjie Du
 Author-email: wenjay.du@gmail.com
 License: GPL-3.0
-Keywords: Google Scholar,citation,citation number,badge,svg,generating
+Keywords: Google Scholar,citation,citation number,shields.io,badge,svg,generating
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -19,16 +19,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GoogleScholar Badge Generator
 
 [shields.io](https://shields.io) does not provide an API to help generate citation badges of articles/profiles 
 on Google Scholar. Therefore, I create this repository to build us such a tool.
-Need citation badges but cannot find a proper tool? Try GSBG!
+Need citation badges but cannot find a proper tool? Try GSBG! You can even make yourself a GoogleScholar version of shields.io with GitHub actions! Take a look at [Usage](-usage) below. 
 
+Please star🌟 this repo to help others notice GSBG if you think it is useful. Thank you!
 
 ## ❖ Installation
 You can install GSBG via pip: `pip install gsbg`, or from the latest source code: 
 `pip install https://github.com/WenjieDu/Google_Scholar_Badge_Generator/archive/main.zip`.
 
 ## ❖ Usage
 Apart from the below examples, you can also integrate GSBG with GitHub workflows to automatically generate badges
```

#### html2text {}

```diff
@@ -1,34 +1,36 @@
-Metadata-Version: 2.1 Name: gsbg Version: 0.1.1 Summary: A tool for Google
+Metadata-Version: 2.1 Name: gsbg Version: 0.1.2 Summary: A tool for Google
 Scholar citation badge generation. Home-page: https://github.com/WenjieDu/
-GoogleScholarBadgeGenerator Download-URL: https://github.com/WenjieDu/
-GoogleScholarBadgeGenerator/archive/main.zip Author: Wenjie Du Author-email:
+Google_Scholar_Badge_Generator Download-URL: https://github.com/WenjieDu/
+Google_Scholar_Badge_Generator/archive/main.zip Author: Wenjie Du Author-email:
 wenjay.du@gmail.com License: GPL-3.0 Keywords: Google Scholar,citation,citation
-number,badge,svg,generating Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Education Classifier: Intended Audience :: Science/Research Classifier: License
-:: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5 Description-Content-Type: text/markdown License-File:
-LICENSE # GoogleScholar Badge Generator [shields.io](https://shields.io) does
-not provide an API to help generate citation badges of articles/profiles on
-Google Scholar. Therefore, I create this repository to build us such a tool.
-Need citation badges but cannot find a proper tool? Try GSBG! ## â
-Installation You can install GSBG via pip: `pip install gsbg`, or from the
-latest source code: `pip install https://github.com/WenjieDu/
-Google_Scholar_Badge_Generator/archive/main.zip`. ## â Usage Apart from the
-below examples, you can also integrate GSBG with GitHub workflows to
-automatically generate badges for your articles/profiles, save them in your
-repo, and update them periodically. Please take a look at [https://github.com/
-WenjieDu/WenjieDu](https://github.com/WenjieDu/WenjieDu) for an example. The
-workflow [.github/workflows/gene_citation_badges.yml](https://github.com/
-WenjieDu/WenjieDu/blob/main/.github/workflows/gene_citation_badges.yml) will
-regularly run the generating script [scripts/gene_google_scholar_badges.py]
-(https://github.com/WenjieDu/WenjieDu/blob/main/scripts/
-gene_google_scholar_badges.py) to maintain the badges under [figs/
+number,shields.io,badge,svg,generating Classifier: Development Status :: 4 -
+Beta Classifier: Intended Audience :: Developers Classifier: Intended Audience
+:: Education Classifier: Intended Audience :: Science/Research Classifier:
+License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Requires-Python: >=3.5 Description-Content-Type: text/markdown License-
+File: LICENSE # GoogleScholar Badge Generator [shields.io](https://shields.io)
+does not provide an API to help generate citation badges of articles/profiles
+on Google Scholar. Therefore, I create this repository to build us such a tool.
+Need citation badges but cannot find a proper tool? Try GSBG! You can even make
+yourself a GoogleScholar version of shields.io with GitHub actions! Take a look
+at [Usage](-usage) below. Please starð this repo to help others notice GSBG
+if you think it is useful. Thank you! ## â Installation You can install GSBG
+via pip: `pip install gsbg`, or from the latest source code: `pip install
+https://github.com/WenjieDu/Google_Scholar_Badge_Generator/archive/main.zip`.
+## â Usage Apart from the below examples, you can also integrate GSBG with
+GitHub workflows to automatically generate badges for your articles/profiles,
+save them in your repo, and update them periodically. Please take a look at
+[https://github.com/WenjieDu/WenjieDu](https://github.com/WenjieDu/WenjieDu)
+for an example. The workflow [.github/workflows/gene_citation_badges.yml]
+(https://github.com/WenjieDu/WenjieDu/blob/main/.github/workflows/
+gene_citation_badges.yml) will regularly run the generating script [scripts/
+gene_google_scholar_badges.py](https://github.com/WenjieDu/WenjieDu/blob/main/
+scripts/gene_google_scholar_badges.py) to maintain the badges under [figs/
 citation_badges](https://github.com/WenjieDu/WenjieDu/tree/main/figs/
 citation_badges). You can fork my repo and modify the script and the workflow
 to fit your own needs. If you meet any question, please [raise an issue](https:
 //github.com/WenjieDu/Google_Scholar_Badge_Generator/issues). I'll try my best
 to help. ```python import gsbg article_link = "https://scholar.google.com/
 citations?view_op=view_citation&hl=en&user=j9qvUg0AAAAJ&citation_for_view=j9qvUg0AAAAJ:
 Y0pCki6q_DkC" profile_link = "https://scholar.google.com/
```

### Comparing `gsbg-0.1.1/README.md` & `gsbg-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # GoogleScholar Badge Generator
 
 [shields.io](https://shields.io) does not provide an API to help generate citation badges of articles/profiles 
 on Google Scholar. Therefore, I create this repository to build us such a tool.
-Need citation badges but cannot find a proper tool? Try GSBG!
+Need citation badges but cannot find a proper tool? Try GSBG! You can even make yourself a GoogleScholar version of shields.io with GitHub actions! Take a look at [Usage](-usage) below. 
 
+Please star🌟 this repo to help others notice GSBG if you think it is useful. Thank you!
 
 ## ❖ Installation
 You can install GSBG via pip: `pip install gsbg`, or from the latest source code: 
 `pip install https://github.com/WenjieDu/Google_Scholar_Badge_Generator/archive/main.zip`.
 
 ## ❖ Usage
 Apart from the below examples, you can also integrate GSBG with GitHub workflows to automatically generate badges
```

#### html2text {}

```diff
@@ -1,28 +1,30 @@
 # GoogleScholar Badge Generator [shields.io](https://shields.io) does not
 provide an API to help generate citation badges of articles/profiles on Google
 Scholar. Therefore, I create this repository to build us such a tool. Need
-citation badges but cannot find a proper tool? Try GSBG! ## â Installation
-You can install GSBG via pip: `pip install gsbg`, or from the latest source
-code: `pip install https://github.com/WenjieDu/Google_Scholar_Badge_Generator/
-archive/main.zip`. ## â Usage Apart from the below examples, you can also
-integrate GSBG with GitHub workflows to automatically generate badges for your
-articles/profiles, save them in your repo, and update them periodically. Please
-take a look at [https://github.com/WenjieDu/WenjieDu](https://github.com/
-WenjieDu/WenjieDu) for an example. The workflow [.github/workflows/
-gene_citation_badges.yml](https://github.com/WenjieDu/WenjieDu/blob/
-main/.github/workflows/gene_citation_badges.yml) will regularly run the
-generating script [scripts/gene_google_scholar_badges.py](https://github.com/
-WenjieDu/WenjieDu/blob/main/scripts/gene_google_scholar_badges.py) to maintain
-the badges under [figs/citation_badges](https://github.com/WenjieDu/WenjieDu/
-tree/main/figs/citation_badges). You can fork my repo and modify the script and
-the workflow to fit your own needs. If you meet any question, please [raise an
-issue](https://github.com/WenjieDu/Google_Scholar_Badge_Generator/issues). I'll
-try my best to help. ```python import gsbg article_link = "https://
-scholar.google.com/
+citation badges but cannot find a proper tool? Try GSBG! You can even make
+yourself a GoogleScholar version of shields.io with GitHub actions! Take a look
+at [Usage](-usage) below. Please starð this repo to help others notice GSBG
+if you think it is useful. Thank you! ## â Installation You can install GSBG
+via pip: `pip install gsbg`, or from the latest source code: `pip install
+https://github.com/WenjieDu/Google_Scholar_Badge_Generator/archive/main.zip`.
+## â Usage Apart from the below examples, you can also integrate GSBG with
+GitHub workflows to automatically generate badges for your articles/profiles,
+save them in your repo, and update them periodically. Please take a look at
+[https://github.com/WenjieDu/WenjieDu](https://github.com/WenjieDu/WenjieDu)
+for an example. The workflow [.github/workflows/gene_citation_badges.yml]
+(https://github.com/WenjieDu/WenjieDu/blob/main/.github/workflows/
+gene_citation_badges.yml) will regularly run the generating script [scripts/
+gene_google_scholar_badges.py](https://github.com/WenjieDu/WenjieDu/blob/main/
+scripts/gene_google_scholar_badges.py) to maintain the badges under [figs/
+citation_badges](https://github.com/WenjieDu/WenjieDu/tree/main/figs/
+citation_badges). You can fork my repo and modify the script and the workflow
+to fit your own needs. If you meet any question, please [raise an issue](https:
+//github.com/WenjieDu/Google_Scholar_Badge_Generator/issues). I'll try my best
+to help. ```python import gsbg article_link = "https://scholar.google.com/
 citations?view_op=view_citation&hl=en&user=j9qvUg0AAAAJ&citation_for_view=j9qvUg0AAAAJ:
 Y0pCki6q_DkC" profile_link = "https://scholar.google.com/
 citations?user=j9qvUg0AAAAJ&hl=en" article_citation_num =
 gsbg.fetch_article_citation_num(article_link) profile_citation_num =
 gsbg.fetch_profile_citation_num(profile_link) gsbg.gene_citation_badge_link
 ( link='https://scholar.google.com/citations?user=j9qvUg0AAAAJ&hl=en',
 link_type="profile", ) gsbg.gene_citation_badge_svg( link='https://
```

### Comparing `gsbg-0.1.1/gsbg/google_scholar_badge_generator.py` & `gsbg-0.1.2/gsbg/google_scholar_badge_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """
 Storing the functions of GSBG.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
+import logging
 import os
 import random
 import warnings
 
 import requests
 from bs4 import BeautifulSoup, element
 
+logging.basicConfig(
+    level=logging.INFO, format="%(asctime)s [%(levelname)s]: %(message)s"
+)
+
+
 MIRROR_SITES = {
     "scholar.lanfanshu.cn": "True",  # 'True' means this mirror site is in Chinese
 }
 
-ARTICLE_CITATION_SELECTOR = (
-    "#gsc_oci_table > div > div.gsc_oci_value > div > a"
-)
+ARTICLE_CITATION_SELECTOR = "#gsc_oci_table > div > div.gsc_oci_value > div > a"
 PROFILE_CITATION_SELECTOR = "#gsc_rsb_st > tbody > tr:nth-child(1) > td:nth-child(2)"
 
 USER_AGENTS = [
     "Mozilla/4.0 (compatible; MSIE 6.0; Windows NT 5.1; SV1; AcooBrowser; .NET CLR 1.1.4322; .NET CLR 2.0.50727)",
     "Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.0; Acoo Browser; SLCC1; .NET CLR 2.0.50727; Media Center PC 5.0; .NET CLR 3.0.04506)",
     "Mozilla/4.0 (compatible; MSIE 7.0; AOL 9.5; AOLBuild 4337.35; Windows NT 5.1; .NET CLR 1.1.4322; .NET CLR 2.0.50727)",
     "Mozilla/5.0 (Windows; U; MSIE 9.0; Windows NT 9.0; en-US)",
@@ -65,20 +69,20 @@
         "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
         "Accept-Language": "en-US,en;q=0.5",
         "Connection": "keep-alive",
         "Accept-Encoding": "gzip, deflate",
     }
 
 
-def apply_mirror_site(link):
+def apply_mirror_sites(link):
     site_to_use = random.choice(list(MIRROR_SITES.keys()))
-    print(f"Applying the mirror site '{site_to_use}'")
+    logging.info(f"Applying the mirror site '{site_to_use}'")
     os.environ["GS_MIRROR_SITE_IN_CHINESE"] = MIRROR_SITES[site_to_use]
     new_link = link.replace("scholar.google.com", site_to_use)
-    print(f"The updated URL is: {new_link}")
+    logging.info(f"The updated URL is: {new_link}")
     return new_link
 
 
 def fetch_selected_element_from_page(selector: str, page_url: str) -> element.Tag:
     """Fetch the selected element from the given page.
 
     Parameters
@@ -91,22 +95,22 @@
 
     Returns
     -------
     selected : bs4.element.Tag,
         The element selected by the given selector on the given page.
 
     """
-    if os.getenv("APPLY_MIRROR_SITE", "False") == "True":
-        page_url = apply_mirror_site(page_url)
+    if os.getenv("APPLY_MIRROR_SITES", "False") == "True":
+        page_url = apply_mirror_sites(page_url)
 
     page = requests.get(page_url, headers=get_header()).text
     soup = BeautifulSoup(page, "html.parser")
     selected = soup.select_one(selector)
     if selected is None:
-        print(soup.prettify())
+        logging.error(soup.prettify())
         raise RuntimeError(
             f"Cannot find the element selected by {selector} on {page_url}. "
             f"This may caused by an invalid selector, an invalid page_url. "
             f"The reason also may be your IP address got blocked by the server. "
             f"The fetch html page got printed above, please check it to find more details."
         )
     return selected
@@ -229,10 +233,10 @@
         os.makedirs(path_to_save, exist_ok=True)
         if not svg_name.endswith(".svg"):
             svg_name = f"{svg_name}.svg"
         saving_path = os.path.join(path_to_save, svg_name)
         with open(saving_path, "wb") as file_handle:
             file_handle.write(requests.get(link).content)
     except Exception as e:
-        print("Generating failed.")
+        logging.error("Generating failed.")
         raise e
-    print(f"Saved to {saving_path}. Please check out your badge there.")
+    logging.info(f"Saved to {saving_path}. Please check out your badge there.")
```

### Comparing `gsbg-0.1.1/gsbg.egg-info/PKG-INFO` & `gsbg-0.1.2/gsbg.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: gsbg
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool for Google Scholar citation badge generation.
-Home-page: https://github.com/WenjieDu/GoogleScholarBadgeGenerator
-Download-URL: https://github.com/WenjieDu/GoogleScholarBadgeGenerator/archive/main.zip
+Home-page: https://github.com/WenjieDu/Google_Scholar_Badge_Generator
+Download-URL: https://github.com/WenjieDu/Google_Scholar_Badge_Generator/archive/main.zip
 Author: Wenjie Du
 Author-email: wenjay.du@gmail.com
 License: GPL-3.0
-Keywords: Google Scholar,citation,citation number,badge,svg,generating
+Keywords: Google Scholar,citation,citation number,shields.io,badge,svg,generating
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -19,16 +19,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GoogleScholar Badge Generator
 
 [shields.io](https://shields.io) does not provide an API to help generate citation badges of articles/profiles 
 on Google Scholar. Therefore, I create this repository to build us such a tool.
-Need citation badges but cannot find a proper tool? Try GSBG!
+Need citation badges but cannot find a proper tool? Try GSBG! You can even make yourself a GoogleScholar version of shields.io with GitHub actions! Take a look at [Usage](-usage) below. 
 
+Please star🌟 this repo to help others notice GSBG if you think it is useful. Thank you!
 
 ## ❖ Installation
 You can install GSBG via pip: `pip install gsbg`, or from the latest source code: 
 `pip install https://github.com/WenjieDu/Google_Scholar_Badge_Generator/archive/main.zip`.
 
 ## ❖ Usage
 Apart from the below examples, you can also integrate GSBG with GitHub workflows to automatically generate badges
```

#### html2text {}

```diff
@@ -1,34 +1,36 @@
-Metadata-Version: 2.1 Name: gsbg Version: 0.1.1 Summary: A tool for Google
+Metadata-Version: 2.1 Name: gsbg Version: 0.1.2 Summary: A tool for Google
 Scholar citation badge generation. Home-page: https://github.com/WenjieDu/
-GoogleScholarBadgeGenerator Download-URL: https://github.com/WenjieDu/
-GoogleScholarBadgeGenerator/archive/main.zip Author: Wenjie Du Author-email:
+Google_Scholar_Badge_Generator Download-URL: https://github.com/WenjieDu/
+Google_Scholar_Badge_Generator/archive/main.zip Author: Wenjie Du Author-email:
 wenjay.du@gmail.com License: GPL-3.0 Keywords: Google Scholar,citation,citation
-number,badge,svg,generating Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Education Classifier: Intended Audience :: Science/Research Classifier: License
-:: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5 Description-Content-Type: text/markdown License-File:
-LICENSE # GoogleScholar Badge Generator [shields.io](https://shields.io) does
-not provide an API to help generate citation badges of articles/profiles on
-Google Scholar. Therefore, I create this repository to build us such a tool.
-Need citation badges but cannot find a proper tool? Try GSBG! ## â
-Installation You can install GSBG via pip: `pip install gsbg`, or from the
-latest source code: `pip install https://github.com/WenjieDu/
-Google_Scholar_Badge_Generator/archive/main.zip`. ## â Usage Apart from the
-below examples, you can also integrate GSBG with GitHub workflows to
-automatically generate badges for your articles/profiles, save them in your
-repo, and update them periodically. Please take a look at [https://github.com/
-WenjieDu/WenjieDu](https://github.com/WenjieDu/WenjieDu) for an example. The
-workflow [.github/workflows/gene_citation_badges.yml](https://github.com/
-WenjieDu/WenjieDu/blob/main/.github/workflows/gene_citation_badges.yml) will
-regularly run the generating script [scripts/gene_google_scholar_badges.py]
-(https://github.com/WenjieDu/WenjieDu/blob/main/scripts/
-gene_google_scholar_badges.py) to maintain the badges under [figs/
+number,shields.io,badge,svg,generating Classifier: Development Status :: 4 -
+Beta Classifier: Intended Audience :: Developers Classifier: Intended Audience
+:: Education Classifier: Intended Audience :: Science/Research Classifier:
+License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Requires-Python: >=3.5 Description-Content-Type: text/markdown License-
+File: LICENSE # GoogleScholar Badge Generator [shields.io](https://shields.io)
+does not provide an API to help generate citation badges of articles/profiles
+on Google Scholar. Therefore, I create this repository to build us such a tool.
+Need citation badges but cannot find a proper tool? Try GSBG! You can even make
+yourself a GoogleScholar version of shields.io with GitHub actions! Take a look
+at [Usage](-usage) below. Please starð this repo to help others notice GSBG
+if you think it is useful. Thank you! ## â Installation You can install GSBG
+via pip: `pip install gsbg`, or from the latest source code: `pip install
+https://github.com/WenjieDu/Google_Scholar_Badge_Generator/archive/main.zip`.
+## â Usage Apart from the below examples, you can also integrate GSBG with
+GitHub workflows to automatically generate badges for your articles/profiles,
+save them in your repo, and update them periodically. Please take a look at
+[https://github.com/WenjieDu/WenjieDu](https://github.com/WenjieDu/WenjieDu)
+for an example. The workflow [.github/workflows/gene_citation_badges.yml]
+(https://github.com/WenjieDu/WenjieDu/blob/main/.github/workflows/
+gene_citation_badges.yml) will regularly run the generating script [scripts/
+gene_google_scholar_badges.py](https://github.com/WenjieDu/WenjieDu/blob/main/
+scripts/gene_google_scholar_badges.py) to maintain the badges under [figs/
 citation_badges](https://github.com/WenjieDu/WenjieDu/tree/main/figs/
 citation_badges). You can fork my repo and modify the script and the workflow
 to fit your own needs. If you meet any question, please [raise an issue](https:
 //github.com/WenjieDu/Google_Scholar_Badge_Generator/issues). I'll try my best
 to help. ```python import gsbg article_link = "https://scholar.google.com/
 citations?view_op=view_citation&hl=en&user=j9qvUg0AAAAJ&citation_for_view=j9qvUg0AAAAJ:
 Y0pCki6q_DkC" profile_link = "https://scholar.google.com/
```

### Comparing `gsbg-0.1.1/setup.py` & `gsbg-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,20 +19,21 @@
     version=__version__,
     description="A tool for Google Scholar citation badge generation.",
     long_description=README,
     long_description_content_type="text/markdown",
     license="GPL-3.0",
     author="Wenjie Du",
     author_email="wenjay.du@gmail.com",
-    url="https://github.com/WenjieDu/GoogleScholarBadgeGenerator",
-    download_url="https://github.com/WenjieDu/GoogleScholarBadgeGenerator/archive/main.zip",
+    url="https://github.com/WenjieDu/Google_Scholar_Badge_Generator",
+    download_url="https://github.com/WenjieDu/Google_Scholar_Badge_Generator/archive/main.zip",
     keywords=[
         "Google Scholar",
         "citation",
         "citation number",
+        "shields.io",
         "badge",
         "svg",
         "generating",
     ],
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

