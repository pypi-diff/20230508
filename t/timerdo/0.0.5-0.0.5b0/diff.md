# Comparing `tmp/timerdo-0.0.5.tar.gz` & `tmp/timerdo-0.0.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timerdo-0.0.5.tar", last modified: Mon May  8 14:28:44 2023, max compression
+gzip compressed data, was "timerdo-0.0.5b0.tar", last modified: Thu May  4 20:20:13 2023, max compression
```

## Comparing `timerdo-0.0.5.tar` & `timerdo-0.0.5b0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       30 2023-05-08 14:27:54.795274 timerdo-0.0.5/.coveragerc
--rw-r--r--   0        0        0       99 2023-05-08 14:27:54.795274 timerdo-0.0.5/.flake8
--rw-r--r--   0        0        0      569 2023-05-08 14:27:54.795274 timerdo-0.0.5/.github/workflows/publish_docs.yml
--rw-r--r--   0        0        0      506 2023-05-08 14:27:54.795274 timerdo-0.0.5/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0      566 2023-05-08 14:27:54.795274 timerdo-0.0.5/.github/workflows/test_suite.yml
--rw-r--r--   0        0        0      101 2023-05-08 14:27:54.795274 timerdo-0.0.5/.gitignore
--rw-r--r--   0        0        0      292 2023-05-08 14:27:54.795274 timerdo-0.0.5/Makefile
--rw-r--r--   0        0        0     1793 2023-05-08 14:27:54.795274 timerdo-0.0.5/README.md
--rw-r--r--   0        0        0     1211 2023-05-08 14:27:54.795274 timerdo-0.0.5/UNLICENSE
--rw-r--r--   0        0        0     3399 2023-05-08 14:27:54.795274 timerdo-0.0.5/docs/cli_reference.md
--rw-r--r--   0        0        0    37426 2023-05-08 14:27:54.799274 timerdo-0.0.5/docs/img/favicon.png
--rw-r--r--   0        0        0    76201 2023-05-08 14:27:54.799274 timerdo-0.0.5/docs/img/logo.png
--rw-r--r--   0        0        0    75292 2023-05-08 14:27:54.799274 timerdo-0.0.5/docs/img/screenshot_timerdo_report.png
--rw-r--r--   0        0        0    13786 2023-05-08 14:27:54.799274 timerdo-0.0.5/docs/img/timerdo_no_args.png
--rw-r--r--   0        0        0     1891 2023-05-08 14:27:54.799274 timerdo-0.0.5/docs/index.md
--rw-r--r--   0        0        0     2502 2023-05-08 14:27:54.799274 timerdo-0.0.5/docs/install.md
--rw-r--r--   0        0        0     4267 2023-05-08 14:27:54.799274 timerdo-0.0.5/docs/start.md
--rw-r--r--   0        0        0       48 2023-05-08 14:27:54.799274 timerdo-0.0.5/docs/stylesheets/extra.css
--rw-r--r--   0        0        0    20401 2023-05-08 14:27:54.799274 timerdo-0.0.5/docs/tutorial_1.md
--rw-r--r--   0        0        0    11859 2023-05-08 14:27:54.799274 timerdo-0.0.5/docs/tutorial_2.md
--rw-r--r--   0        0        0      164 2023-05-08 14:27:54.799274 timerdo-0.0.5/includes/abbreviations.md
--rw-r--r--   0        0        0     2240 2023-05-08 14:27:54.799274 timerdo-0.0.5/mkdocs.yml
--rw-r--r--   0        0        0     1242 2023-05-08 14:27:54.799274 timerdo-0.0.5/pyproject.toml
--rwxr-xr-x   0        0        0      210 2023-05-08 14:27:54.799274 timerdo-0.0.5/scripts/bootstrap.sh
--rw-r--r--   0        0        0      157 2023-05-08 14:27:54.799274 timerdo-0.0.5/scripts/build_cli_ref.sh
--rw-r--r--   0        0        0      816 2023-05-08 14:27:54.799274 timerdo-0.0.5/scripts/docs_db.py
--rwxr-xr-x   0        0        0      241 2023-05-08 14:27:54.799274 timerdo-0.0.5/scripts/docs_preview.sh
--rwxr-xr-x   0        0        0      101 2023-05-08 14:27:54.799274 timerdo-0.0.5/scripts/docs_publish.sh
--rwxr-xr-x   0        0        0      354 2023-05-08 14:27:54.799274 timerdo-0.0.5/scripts/format.sh
--rw-r--r--   0        0        0      207 2023-05-08 14:27:54.799274 timerdo-0.0.5/scripts/gen_docs_db.sh
--rwxr-xr-x   0        0        0      110 2023-05-08 14:27:54.799274 timerdo-0.0.5/scripts/publish.sh
--rwxr-xr-x   0        0        0      277 2023-05-08 14:27:54.799274 timerdo-0.0.5/scripts/tests.sh
--rw-r--r--   0        0        0        0 2023-05-08 14:27:54.799274 timerdo-0.0.5/test/__init__.py
--rw-r--r--   0        0        0     1128 2023-05-08 14:27:54.799274 timerdo-0.0.5/test/conftest.py
--rw-r--r--   0        0        0     6422 2023-05-08 14:27:54.799274 timerdo-0.0.5/test/test_core.py
--rw-r--r--   0        0        0     2556 2023-05-08 14:27:54.799274 timerdo-0.0.5/test/test_main.py
--rw-r--r--   0        0        0      100 2023-05-08 14:27:54.799274 timerdo-0.0.5/timerdo/__init__.py
--rw-r--r--   0        0        0      955 2023-05-08 14:27:54.799274 timerdo-0.0.5/timerdo/config.py
--rw-r--r--   0        0        0    11736 2023-05-08 14:27:54.799274 timerdo-0.0.5/timerdo/core.py
--rw-r--r--   0        0        0     1075 2023-05-08 14:27:54.803274 timerdo-0.0.5/timerdo/database.py
--rw-r--r--   0        0        0      630 2023-05-08 14:27:54.803274 timerdo-0.0.5/timerdo/exceptions.py
--rw-r--r--   0        0        0     5414 2023-05-08 14:27:54.803274 timerdo-0.0.5/timerdo/main.py
--rw-r--r--   0        0        0     1681 2023-05-08 14:27:54.803274 timerdo-0.0.5/timerdo/models.py
--rw-r--r--   0        0        0     3066 1970-01-01 00:00:00.000000 timerdo-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/.coveragerc
+-rw-r--r--   0        0        0       99 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/.flake8
+-rw-r--r--   0        0        0      569 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/.github/workflows/publish_docs.yml
+-rw-r--r--   0        0        0      506 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0      566 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/.github/workflows/test_suite.yml
+-rw-r--r--   0        0        0      101 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/.gitignore
+-rw-r--r--   0        0        0      292 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/Makefile
+-rw-r--r--   0        0        0     1793 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/README.md
+-rw-r--r--   0        0        0     1211 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/UNLICENSE
+-rw-r--r--   0        0        0     3400 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/cli_reference.md
+-rw-r--r--   0        0        0    37426 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/img/favicon.png
+-rw-r--r--   0        0        0    76201 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/img/logo.png
+-rw-r--r--   0        0        0    75292 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/img/screenshot_timerdo_report.png
+-rw-r--r--   0        0        0    13786 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/img/timerdo_no_args.png
+-rw-r--r--   0        0        0     1891 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/index.md
+-rw-r--r--   0        0        0     2502 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/install.md
+-rw-r--r--   0        0        0     4267 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/start.md
+-rw-r--r--   0        0        0       48 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0    19982 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/tutorial_1.md
+-rw-r--r--   0        0        0      376 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/tutorial_2.md
+-rw-r--r--   0        0        0      138 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/includes/abbreviations.md
+-rw-r--r--   0        0        0     2240 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/mkdocs.yml
+-rw-r--r--   0        0        0     1242 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/pyproject.toml
+-rwxr-xr-x   0        0        0      210 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/scripts/bootstrap.sh
+-rw-r--r--   0        0        0      157 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/scripts/build_cli_ref.sh
+-rw-r--r--   0        0        0      816 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/scripts/docs_db.py
+-rwxr-xr-x   0        0        0      241 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/scripts/docs_preview.sh
+-rwxr-xr-x   0        0        0      101 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/scripts/docs_publish.sh
+-rwxr-xr-x   0        0        0      354 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/scripts/format.sh
+-rw-r--r--   0        0        0      207 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/scripts/gen_docs_db.sh
+-rwxr-xr-x   0        0        0      110 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/scripts/publish.sh
+-rwxr-xr-x   0        0        0      277 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/scripts/tests.sh
+-rw-r--r--   0        0        0        0 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/test/__init__.py
+-rw-r--r--   0        0        0     1128 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/test/conftest.py
+-rw-r--r--   0        0        0     6422 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/test/test_core.py
+-rw-r--r--   0        0        0     2557 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/test/test_main.py
+-rw-r--r--   0        0        0      101 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/timerdo/__init__.py
+-rw-r--r--   0        0        0      955 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/timerdo/config.py
+-rw-r--r--   0        0        0    11736 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/timerdo/core.py
+-rw-r--r--   0        0        0     1075 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/timerdo/database.py
+-rw-r--r--   0        0        0      630 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/timerdo/exceptions.py
+-rw-r--r--   0        0        0     5417 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/timerdo/main.py
+-rw-r--r--   0        0        0     1681 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/timerdo/models.py
+-rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 timerdo-0.0.5b0/PKG-INFO
```

### Comparing `timerdo-0.0.5/.github/workflows/publish_docs.yml` & `timerdo-0.0.5b0/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/.github/workflows/test_suite.yml` & `timerdo-0.0.5b0/.github/workflows/test_suite.yml`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/README.md` & `timerdo-0.0.5b0/README.md`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/UNLICENSE` & `timerdo-0.0.5b0/UNLICENSE`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/docs/cli_reference.md` & `timerdo-0.0.5b0/docs/cli_reference.md`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 ```console
 $ timerdo report [OPTIONS]
 ```
 
 **Options**:
 
 * `-d, --done`: Return also tasks with Done status.
-* `-t, --tag TEXT`: Filter tags.
+* `-t, --tags TEXT`: Filter tags.
 * `-i, --init [%Y-%m-%d]`: Timeframe's lower boundary.
 * `-e, --end [%Y-%m-%d]`: Timeframe's upper boundary.
 * `-o, --order-by TEXT`: Column to order by.
 * `-a, --asc`: If ordered by it will be in ascending order.
 * `--help`: Show this message and exit.
 
 ## `timerdo start`
```

### Comparing `timerdo-0.0.5/docs/img/favicon.png` & `timerdo-0.0.5b0/docs/img/favicon.png`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/docs/img/logo.png` & `timerdo-0.0.5b0/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/docs/img/screenshot_timerdo_report.png` & `timerdo-0.0.5b0/docs/img/screenshot_timerdo_report.png`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/docs/img/timerdo_no_args.png` & `timerdo-0.0.5b0/docs/img/timerdo_no_args.png`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/docs/index.md` & `timerdo-0.0.5b0/docs/index.md`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/docs/install.md` & `timerdo-0.0.5b0/docs/install.md`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/docs/start.md` & `timerdo-0.0.5b0/docs/start.md`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/docs/tutorial_1.md` & `timerdo-0.0.5b0/docs/tutorial_1.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# User Guide (CUD of CRUD Tasks) - Timer, Delete and Update
+# User Guide - CUD from CRUD
 
 CRUD is an acronym. They are the four basic operations for persistent storage[^1]
 
 !!! info "*TL;DR*"
 
     In this section we'll discuss all the features in depth so if you are already using
     Timerdo and in a hurry, just go straight to any section or to the [reference](cli_reference.md).
@@ -118,22 +118,22 @@
 and the structure is year-month-day as in 1789-07-14.
 
 Let's try it out:
 
 ```shell
 $ timerdo task "my second task with options" --tag "user guide tag" -d 2023-05-10
 $ timerdo report
-    --/-- More things above --/--
+    --/-- 
 
 ╭────┬────────────┬─────────────────────────────┬────────────┬────────┬─────────────────╮
 │ ID │       Date │ Task                        │   Deadline │ Status │      Time       │
 ├────┼────────────┼─────────────────────────────┼────────────┼────────┼─────────────────┤
 │  3 │ 2023-05-04 │ My Second Task With Options │ 2023-05-10 │ To Do  │ 0 days 00:00:00 │
 
-    --/-- More things below --/--
+    --/--
 ```
 Here we used the `--deadline` shortcut (`-d`).
 
 ??? danger "Technicalities" 
     `--deadline` is in the CLI API a `#!python datetime` and not a `#!python date` as [Typer](https://typer.tiangolo.com/) -
     the library for building CLI apps I used - doesn't support `#!python date`. 
     However the Timerdo core treats it as a `#!python date` and the data model maps it as `date` as well.
@@ -221,31 +221,31 @@
 
 
 ## delete
 
 Until now you didn't make a mistake :clap:. But you know, humans make mistakes.
 Let's say your are human and made a miskate. The very first solution is to throw it away.
 
-To delete a entry you have 2 arguments `table` and `id`.
+To delete a entry you have to arguments `table` and `id`.
 
 `table` are: `[task|timer]`. It works in the same way of `status`. `id` you already know.
 Each table has its own ids.
 
 ```shell
 $ timerdo delete timer 1
 $ timerdo report
-    --/-- More things above --/--                                            
+    --/--                                                                    
 ╭────┬────────────┬───────────────────────┬──────────┬────────┬─────────────────╮
 │ ID │       Date │ Task                  │ Deadline │ Status │      Time       │
 ├────┼────────────┼───────────────────────┼──────────┼────────┼─────────────────┤
 │  1 │ 2023-05-04 │ <your task goes here> │          │ Doing  │ 0 days 00:00:00 │
 ╰────┴────────────┴───────────────────────┴──────────┴────────┴─────────────────╯
-    --/-- More things below --/--
+    --/--
 ```
-??? warning
+!!! warning
     If you delete a task, all timers linked to that task will be deleted as well.
 
 Sometimes everything is almost correctly and you don't want to delete everything.
 The next topic will show you how to update your data.
 
 ??? warning "Under construction :factory_worker:"
     Up to this point you can query using sql script (I'll show later on) to create personal
@@ -253,24 +253,15 @@
     
     This is, so far, the only way to view the Timer table.
 
     You can copy and past the script when the time comes: "SELECT * FROM timer_list"
 
     These are the planned steps:
 
-    **Reports**
-
-    - [ ] Create one simple timer reports with period filter.
-    - [ ] Create one simple task report with period filter.
-    - [ ] Create a CLI entry point to call both functions from one subcommand (like edit or delete).
-    
-    **Delete**
-    
-    - [ ] Update delete function to delete batches by *tag*.
-    - [ ] Update delete function to delete by *creation* period.
+    - [ ] Create two simple reports with full table. One for each table.
 
 
 ## Update
 
 In Timerdo you can `edit` both tables, but one row at a time.
 You have basically two commands `task` and `timer` and each one you have a
 required argument `id`, or the row you want to edit, and as options as the number
```

### Comparing `timerdo-0.0.5/mkdocs.yml` & `timerdo-0.0.5b0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/pyproject.toml` & `timerdo-0.0.5b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/scripts/docs_db.py` & `timerdo-0.0.5b0/scripts/docs_db.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/test/conftest.py` & `timerdo-0.0.5b0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/test/test_core.py` & `timerdo-0.0.5b0/test/test_core.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/test/test_main.py` & `timerdo-0.0.5b0/test/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 def test_delete_task():
     result = runner.invoke(app, ['delete', 'task', '1'])
     assert result.exit_code == 0
 
 
 def test_report():
     result = runner.invoke(
-        app, ['report', '--order-by', 'test', '--tag', 'test']
+        app, ['report', '--order-by', 'test', '--tags', 'test']
     )
     assert f'from 1789-07-14 until {datetime.now().date()}' in result.stdout
 
 
 def test_report_date():
     result = runner.invoke(
         app, ['report', '--init', '1988-10-10', '--end', '2022-10-10']
```

### Comparing `timerdo-0.0.5/timerdo/config.py` & `timerdo-0.0.5b0/timerdo/config.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/timerdo/core.py` & `timerdo-0.0.5b0/timerdo/core.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/timerdo/database.py` & `timerdo-0.0.5b0/timerdo/database.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/timerdo/exceptions.py` & `timerdo-0.0.5b0/timerdo/exceptions.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/timerdo/main.py` & `timerdo-0.0.5b0/timerdo/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,16 +108,16 @@
 
 
 @app.command("report")
 def report_tasks(
     status: bool = typer.Option(
         False, "--done", "-d", help="Return also tasks with Done status."
     ),
-    tag: Optional[list[str]] = typer.Option(
-        None, "--tag", "-t", help="Filter tags."
+    tags: Optional[list[str]] = typer.Option(
+        None, "--tags", "-t", help="Filter tags."
     ),
     init: Optional[datetime] = typer.Option(
         None,
         "--init",
         "-i",
         help="Timeframe's lower boundary.",
         formats=["%Y-%m-%d"],
@@ -139,15 +139,15 @@
         help="If ordered by it will be in ascending order.",
     ),
 ) -> NoReturn:
     """Print reports."""
     print_report(
         list_tasks_with_time(
             status=status,
-            tags=tag,
+            tags=tags,
             init=init,
             end=end,
             order_by=order_by,
             asc=asc,
         ),
         init=init,
         end=end,
```

### Comparing `timerdo-0.0.5/timerdo/models.py` & `timerdo-0.0.5b0/timerdo/models.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.5/PKG-INFO` & `timerdo-0.0.5b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timerdo
-Version: 0.0.5
+Version: 0.0.5b0
 Summary: Minimalist to-do list with built-in timer to keep your tasks on track.
 Author-email: Caio Mescouto Terra de Souza <caiomescouto@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: sqlalchemy >=2.0.4, <2.1
 Requires-Dist: typer >=0.7.0, <0.9
 Requires-Dist: rich >=13.3, <13.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timerdo Version: 0.0.5 Summary: Minimalist to-do
+Metadata-Version: 2.1 Name: timerdo Version: 0.0.5b0 Summary: Minimalist to-do
 list with built-in timer to keep your tasks on track. Author-email: Caio
 Mescouto Terra de Souza
 gmail.com> Requires-Python: >=3.11 Description-Content-Type: text/markdown
 Requires-Dist: sqlalchemy >=2.0.4, <2.1 Requires-Dist: typer >=0.7.0, <0.9
 Requires-Dist: rich >=13.3, <13.4 Requires-Dist: pandas[performance,feather]
 >=2.0.1, <2.1 Requires-Dist: black >=23.1, <23.2 ; extra == "dev" Requires-
 Dist: flake8 >=6.0, <6.1 ; extra == "dev" Requires-Dist: isort >=5.12, <5.13 ;
```

