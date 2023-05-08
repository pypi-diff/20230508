# Comparing `tmp/letterboxd_stats-0.1.8.tar.gz` & `tmp/letterboxd_stats-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letterboxd_stats-0.1.8.tar", last modified: Tue Apr 18 12:52:03 2023, max compression
+gzip compressed data, was "letterboxd_stats-0.1.9.tar", last modified: Wed Apr 19 13:56:27 2023, max compression
```

## Comparing `letterboxd_stats-0.1.8.tar` & `letterboxd_stats-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-18 12:52:03.478683 letterboxd_stats-0.1.8/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.1.8/LICENCE
--rw-rw-r--   0 marco     (1001) marco     (1001)     2963 2023-04-18 12:52:03.478683 letterboxd_stats-0.1.8/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)     2445 2023-04-13 13:31:47.000000 letterboxd_stats-0.1.8/README.md
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-18 12:52:03.478683 letterboxd_stats-0.1.8/letterboxd_stats/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1460 2023-04-17 21:29:59.000000 letterboxd_stats-0.1.8/letterboxd_stats/__init__.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     5222 2023-04-17 23:43:40.000000 letterboxd_stats-0.1.8/letterboxd_stats/cli.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     3992 2023-04-17 23:53:40.000000 letterboxd_stats-0.1.8/letterboxd_stats/data.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     3519 2023-04-17 23:55:20.000000 letterboxd_stats-0.1.8/letterboxd_stats/main.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     2949 2023-04-17 23:56:08.000000 letterboxd_stats-0.1.8/letterboxd_stats/tmdb.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     5736 2023-04-18 12:45:43.000000 letterboxd_stats-0.1.8/letterboxd_stats/web_scraper.py
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-18 12:52:03.478683 letterboxd_stats-0.1.8/letterboxd_stats.egg-info/
--rw-rw-r--   0 marco     (1001) marco     (1001)     2963 2023-04-18 12:52:03.000000 letterboxd_stats-0.1.8/letterboxd_stats.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-04-18 12:52:03.000000 letterboxd_stats-0.1.8/letterboxd_stats.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-04-18 12:52:03.000000 letterboxd_stats-0.1.8/letterboxd_stats.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-04-18 12:52:03.000000 letterboxd_stats-0.1.8/letterboxd_stats.egg-info/entry_points.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      126 2023-04-18 12:52:03.000000 letterboxd_stats-0.1.8/letterboxd_stats.egg-info/requires.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-04-18 12:52:03.000000 letterboxd_stats-0.1.8/letterboxd_stats.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      865 2023-04-17 23:56:33.000000 letterboxd_stats-0.1.8/pyproject.toml
--rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-04-18 12:52:03.478683 letterboxd_stats-0.1.8/setup.cfg
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-19 13:56:27.229184 letterboxd_stats-0.1.9/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.1.9/LICENCE
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-04-19 13:56:27.229184 letterboxd_stats-0.1.9/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2446 2023-04-19 13:52:38.000000 letterboxd_stats-0.1.9/README.md
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-19 13:56:27.229184 letterboxd_stats-0.1.9/letterboxd_stats/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1462 2023-04-19 13:54:12.000000 letterboxd_stats-0.1.9/letterboxd_stats/__init__.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     5222 2023-04-17 23:43:40.000000 letterboxd_stats-0.1.9/letterboxd_stats/cli.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     3992 2023-04-17 23:53:40.000000 letterboxd_stats-0.1.9/letterboxd_stats/data.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2942 2023-04-19 13:53:53.000000 letterboxd_stats-0.1.9/letterboxd_stats/main.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2949 2023-04-17 23:56:08.000000 letterboxd_stats-0.1.9/letterboxd_stats/tmdb.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     6026 2023-04-19 13:44:08.000000 letterboxd_stats-0.1.9/letterboxd_stats/web_scraper.py
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-19 13:56:27.229184 letterboxd_stats-0.1.9/letterboxd_stats.egg-info/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-04-19 13:56:27.000000 letterboxd_stats-0.1.9/letterboxd_stats.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-04-19 13:56:27.000000 letterboxd_stats-0.1.9/letterboxd_stats.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-04-19 13:56:27.000000 letterboxd_stats-0.1.9/letterboxd_stats.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-04-19 13:56:27.000000 letterboxd_stats-0.1.9/letterboxd_stats.egg-info/entry_points.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      126 2023-04-19 13:56:27.000000 letterboxd_stats-0.1.9/letterboxd_stats.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-04-19 13:56:27.000000 letterboxd_stats-0.1.9/letterboxd_stats.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      865 2023-04-19 13:56:00.000000 letterboxd_stats-0.1.9/pyproject.toml
+-rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-04-19 13:56:27.229184 letterboxd_stats-0.1.9/setup.cfg
```

### Comparing `letterboxd_stats-0.1.8/LICENCE` & `letterboxd_stats-0.1.9/LICENCE`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.1.8/PKG-INFO` & `letterboxd_stats-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letterboxd_stats
-Version: 0.1.8
+Version: 0.1.9
 Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -67,15 +67,15 @@
 options:
   -h, --help            show this help message and exit
   -s SEARCH, --search SEARCH
                         Search for a director
   -S SEARCH_FILM, --search-film SEARCH_FILM
                         Search for a film.
   -d, --download        Download letterboxd data from your account
-  -W, --wishlist        show wishlist
+  -W, --watchlist       show watchlist
   -D, --diary           show diary
   -R, --ratings         show ratings
   -L, --lists           show lists
   -l LIMIT, --limit LIMIT
                         limit the number of items of your wishlist/diary
   -c CONFIG_FOLDER, --config_folder CONFIG_FOLDER
                         Specifiy the folder of your config.toml file
```

### Comparing `letterboxd_stats-0.1.8/README.md` & `letterboxd_stats-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 options:
   -h, --help            show this help message and exit
   -s SEARCH, --search SEARCH
                         Search for a director
   -S SEARCH_FILM, --search-film SEARCH_FILM
                         Search for a film.
   -d, --download        Download letterboxd data from your account
-  -W, --wishlist        show wishlist
+  -W, --watchlist       show watchlist
   -D, --diary           show diary
   -R, --ratings         show ratings
   -L, --lists           show lists
   -l LIMIT, --limit LIMIT
                         limit the number of items of your wishlist/diary
   -c CONFIG_FOLDER, --config_folder CONFIG_FOLDER
                         Specifiy the folder of your config.toml file
```

### Comparing `letterboxd_stats-0.1.8/letterboxd_stats/__init__.py` & `letterboxd_stats-0.1.9/letterboxd_stats/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 parser.add_argument("-S", "--search-film", help="Search for a film.")
 parser.add_argument(
     "-d",
     "--download",
     help="Download letterboxd data from your account",
     action="store_true",
 )
-parser.add_argument("-W", "--wishlist", help="show wishlist", action="store_true")
+parser.add_argument("-W", "--watchlist", help="show watchlist", action="store_true")
 parser.add_argument("-D", "--diary", help="show diary", action="store_true")
 parser.add_argument("-R", "--ratings", help="show ratings", action="store_true")
 parser.add_argument("-L", "--lists", help="show lists", action="store_true")
 parser.add_argument("-l", "--limit", help="limit the number of items of your wishlist/diary", type=int)
 parser.add_argument("-c", "--config_folder", help="Specifiy the folder of your config.toml file")
```

### Comparing `letterboxd_stats-0.1.8/letterboxd_stats/cli.py` & `letterboxd_stats-0.1.9/letterboxd_stats/cli.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.1.8/letterboxd_stats/data.py` & `letterboxd_stats-0.1.9/letterboxd_stats/data.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.1.8/letterboxd_stats/main.py` & `letterboxd_stats-0.1.9/letterboxd_stats/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from letterboxd_stats import tmdb
 from letterboxd_stats import data
 from letterboxd_stats import web_scraper as ws
 import os
 from letterboxd_stats import args, config
 
+DATA_FILES = {"Watchlist": "watchlist.csv", "Diary": "diary.csv", "Ratings": "ratings.csv", "Lists": "lists"}
+
 
 def try_command(command, args):
     try:
         command(*args)
     except Exception as e:
         print(e)
 
@@ -33,15 +35,14 @@
 
 
 def search_person(args_search: str):
     df, name = tmdb.get_person(args_search)
     path = os.path.expanduser(os.path.join(config["root_folder"], "static", "watched.csv"))
     check_path(path)
     movie_id, search_film = data.read_watched_films(df, path, name)
-    print(search_film)
     letterboxd_url = ws.search_film(search_film)
     if movie_id is not None:
         tmdb.get_movie_detail(movie_id, ws.create_movie_url(letterboxd_url, "film_page"))
 
 
 def search_film(args_search_film: str):
     film_url = ws.search_film(args_search_film, True)
@@ -50,54 +51,37 @@
     answer = ws.select_optional_operation()
     if answer != "Exit":
         downloader = ws.Downloader()
         downloader.login()
         downloader.perform_operation(answer, film_url)
 
 
-def get_wishlist(args_limit, args_ascending):
-    path = os.path.expanduser(os.path.join(config["root_folder"], "static", "watchlist.csv"))
-    check_path(path)
-    letterboxd_url = data.open_file("Watchlist", path, args_limit, args_ascending)
-    get_movie_detail_from_url(letterboxd_url)
-
-
-def get_diary(args_limit, args_ascending):
-    path = os.path.expanduser(os.path.join(config["root_folder"], "static", "diary.csv"))
-    check_path(path)
-    letterboxd_url = data.open_file("Diary", path, args_limit, args_ascending)
-    get_movie_detail_from_url(letterboxd_url, True)
-
-
-def get_ratings(args_limit, args_ascending):
-    path = os.path.expanduser(os.path.join(config["root_folder"], "static", "ratings.csv"))
-    check_path(path)
-    letterboxd_url = data.open_file("Ratings", path, args_limit, args_ascending)
-    get_movie_detail_from_url(letterboxd_url)
-
-
-def get_lists(args_limit, args_ascending):
-    path = os.path.expanduser(os.path.join(config["root_folder"], "static", "lists"))
+def get_data(args_limit, args_ascending, data_type):
+    path = os.path.expanduser(os.path.join(config["root_folder"], "static", DATA_FILES[data_type]))
     check_path(path)
-    letterboxd_url = data.open_list(path, args_limit, args_ascending)
-    get_movie_detail_from_url(letterboxd_url)
+    letterboxd_url = (
+        data.open_file(data_type, path, args_limit, args_ascending)
+        if data_type != "Lists"
+        else data.open_list(path, args_limit, args_ascending)
+    )
+    get_movie_detail_from_url(letterboxd_url, data_type == "Diary")
 
 
 def main():
     if args.download:
         try_command(download_data, ())
     if args.search:
         try_command(search_person, (args.search,))
     if args.search_film:
         try_command(search_film, (args.search_film,))
-    if args.wishlist:
-        try_command(get_wishlist, (args.limit, config["CLI"]["ascending"]))
+    if args.watchlist:
+        try_command(get_data, (args.limit, config["CLI"]["ascending"], "Watchlist"))
     if args.diary:
-        try_command(get_diary, (args.limit, config["CLI"]["ascending"]))
+        try_command(get_data, (args.limit, config["CLI"]["ascending"], "Diary"))
     if args.ratings:
-        try_command(get_ratings, (args.limit, config["CLI"]["ascending"]))
+        try_command(get_data, (args.limit, config["CLI"]["ascending"], "Ratings"))
     if args.lists:
-        try_command(get_lists, (args.limit, config["CLI"]["ascending"]))
+        try_command(get_data, (args.limit, config["CLI"]["ascending"], "Lists"))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `letterboxd_stats-0.1.8/letterboxd_stats/tmdb.py` & `letterboxd_stats-0.1.9/letterboxd_stats/tmdb.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.1.8/letterboxd_stats/web_scraper.py` & `letterboxd_stats-0.1.9/letterboxd_stats/web_scraper.py`

 * *Files 12% similar despite different names*

```diff
@@ -115,21 +115,24 @@
 def search_film(title: str, allow_selection=False):
     search_url = URL + OPERATIONS_URLS["search"](title)
     res = requests.get(search_url)
     if res.status_code != 200:
         raise ConnectionError("It's been impossible to retireve the Letterboxd page")
     search_page = html.fromstring(res.text)
     if allow_selection:
-        titles = search_page.xpath("//div[@class='film-detail-content']")
-        if len(titles) == 0:
+        movie_list = search_page.xpath("//div[@class='film-detail-content']")
+        if len(movie_list) == 0:
             raise ValueError(f"No film found with search query {title}")
+        titles = [movie.xpath("./h2/span/a")[0].text.rstrip() for movie in movie_list]
+        years = [
+            f"({year[0].text}) " if len(year := movie.xpath("./h2/span//small/a")) > 0 else "" for movie in movie_list
+        ]
+        directors = [movie.xpath("./p/a")[0].text for movie in movie_list]
+        links = [movie.xpath("./h2/span/a")[0].get("href") for movie in movie_list]
         title_years_directors_links = {
-            f"{t.xpath('./h2/span/a')[0].text.rstrip()} "
-            + f"({t.xpath('./h2/span//small/a')[0].text}) - "
-            + f"{t.xpath('./p/a')[0].text}": t.xpath("./h2/span/a")[0].get("href")
-            for t in titles
+            f"{title} {year}- {director}": link for title, year, director, link in zip(titles, years, directors, links)
         }
         selected_film = cli.select_value(list(title_years_directors_links.keys()), "Select your film")
         title_url = title_years_directors_links[selected_film].split("/")[-2]
     else:
         title_url = search_page.xpath("//span[@class='film-title-wrapper']/a")[0].get("href").split("/")[-2]
     return title_url
```

### Comparing `letterboxd_stats-0.1.8/letterboxd_stats.egg-info/PKG-INFO` & `letterboxd_stats-0.1.9/letterboxd_stats.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letterboxd-stats
-Version: 0.1.8
+Version: 0.1.9
 Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -67,15 +67,15 @@
 options:
   -h, --help            show this help message and exit
   -s SEARCH, --search SEARCH
                         Search for a director
   -S SEARCH_FILM, --search-film SEARCH_FILM
                         Search for a film.
   -d, --download        Download letterboxd data from your account
-  -W, --wishlist        show wishlist
+  -W, --watchlist       show watchlist
   -D, --diary           show diary
   -R, --ratings         show ratings
   -L, --lists           show lists
   -l LIMIT, --limit LIMIT
                         limit the number of items of your wishlist/diary
   -c CONFIG_FOLDER, --config_folder CONFIG_FOLDER
                         Specifiy the folder of your config.toml file
```

### Comparing `letterboxd_stats-0.1.8/pyproject.toml` & `letterboxd_stats-0.1.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "letterboxd_stats"
-version = "0.1.8"
+version = "0.1.9"
 authors = [{ name = "mBaratta96" }]
 description = "Get information about your Letterboxd activity."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
```

