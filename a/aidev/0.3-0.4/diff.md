# Comparing `tmp/aidev-0.3.tar.gz` & `tmp/aidev-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aidev-0.3.tar", last modified: Sun Apr 30 16:46:42 2023, max compression
+gzip compressed data, was "aidev-0.4.tar", last modified: Mon May  8 07:09:47 2023, max compression
```

## Comparing `aidev-0.3.tar` & `aidev-0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-30 16:46:42.596883 aidev-0.3/
--rw-r--r--   0 voidful    (501) staff       (20)      128 2023-04-30 16:46:42.596737 aidev-0.3/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)     4697 2023-04-30 16:45:13.000000 aidev-0.3/README.md
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-30 16:46:42.595532 aidev-0.3/aidev/
--rw-r--r--   0 voidful    (501) staff       (20)       23 2023-04-06 19:53:32.000000 aidev-0.3/aidev/__init__.py
--rw-r--r--   0 voidful    (501) staff       (20)     1869 2023-04-07 07:38:13.000000 aidev-0.3/aidev/config_manager.py
--rw-r--r--   0 voidful    (501) staff       (20)      472 2023-04-30 16:44:43.000000 aidev-0.3/aidev/config_utils.py
--rw-r--r--   0 voidful    (501) staff       (20)     3924 2023-04-30 16:43:37.000000 aidev-0.3/aidev/helpers.py
--rw-r--r--   0 voidful    (501) staff       (20)     1943 2023-04-30 16:44:43.000000 aidev-0.3/aidev/main.py
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-30 16:46:42.596536 aidev-0.3/aidev.egg-info/
--rw-r--r--   0 voidful    (501) staff       (20)      128 2023-04-30 16:46:42.000000 aidev-0.3/aidev.egg-info/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)      289 2023-04-30 16:46:42.000000 aidev-0.3/aidev.egg-info/SOURCES.txt
--rw-r--r--   0 voidful    (501) staff       (20)        1 2023-04-30 16:46:42.000000 aidev-0.3/aidev.egg-info/dependency_links.txt
--rw-r--r--   0 voidful    (501) staff       (20)       88 2023-04-30 16:46:42.000000 aidev-0.3/aidev.egg-info/entry_points.txt
--rw-r--r--   0 voidful    (501) staff       (20)       23 2023-04-30 16:46:42.000000 aidev-0.3/aidev.egg-info/requires.txt
--rw-r--r--   0 voidful    (501) staff       (20)        6 2023-04-30 16:46:42.000000 aidev-0.3/aidev.egg-info/top_level.txt
--rw-r--r--   0 voidful    (501) staff       (20)       38 2023-04-30 16:46:42.596932 aidev-0.3/setup.cfg
--rw-r--r--   0 voidful    (501) staff       (20)      367 2023-04-30 16:44:43.000000 aidev-0.3/setup.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-05-08 07:09:47.022100 aidev-0.4/
+-rw-r--r--   0 voidful    (501) staff       (20)      128 2023-05-08 07:09:47.021953 aidev-0.4/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)     4546 2023-05-08 05:26:48.000000 aidev-0.4/README.md
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-05-08 07:09:47.020904 aidev-0.4/aidev/
+-rw-r--r--   0 voidful    (501) staff       (20)       23 2023-04-06 19:53:32.000000 aidev-0.4/aidev/__init__.py
+-rw-r--r--   0 voidful    (501) staff       (20)     1869 2023-04-07 07:38:13.000000 aidev-0.4/aidev/config_manager.py
+-rw-r--r--   0 voidful    (501) staff       (20)      472 2023-05-08 04:54:48.000000 aidev-0.4/aidev/config_utils.py
+-rw-r--r--   0 voidful    (501) staff       (20)     6513 2023-05-08 06:12:19.000000 aidev-0.4/aidev/helpers.py
+-rw-r--r--   0 voidful    (501) staff       (20)     4093 2023-05-08 05:57:55.000000 aidev-0.4/aidev/main.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-05-08 07:09:47.021766 aidev-0.4/aidev.egg-info/
+-rw-r--r--   0 voidful    (501) staff       (20)      128 2023-05-08 07:09:46.000000 aidev-0.4/aidev.egg-info/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)      289 2023-05-08 07:09:46.000000 aidev-0.4/aidev.egg-info/SOURCES.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        1 2023-05-08 07:09:46.000000 aidev-0.4/aidev.egg-info/dependency_links.txt
+-rw-r--r--   0 voidful    (501) staff       (20)       88 2023-05-08 07:09:46.000000 aidev-0.4/aidev.egg-info/entry_points.txt
+-rw-r--r--   0 voidful    (501) staff       (20)       23 2023-05-08 07:09:46.000000 aidev-0.4/aidev.egg-info/requires.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        6 2023-05-08 07:09:46.000000 aidev-0.4/aidev.egg-info/top_level.txt
+-rw-r--r--   0 voidful    (501) staff       (20)       38 2023-05-08 07:09:47.022157 aidev-0.4/setup.cfg
+-rw-r--r--   0 voidful    (501) staff       (20)      367 2023-05-08 07:09:44.000000 aidev-0.4/setup.py
```

### Comparing `aidev-0.3/README.md` & `aidev-0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -19,17 +19,14 @@
     </a>
     <a href="https://github.com/voidful/aidev">
         <img alt="Download" src="https://img.shields.io/pypi/dm/aidev">
     </a>
     <a href="https://github.com/voidful/aidev">
         <img alt="Last Commit" src="https://img.shields.io/github/last-commit/voidful/aidev">
     </a>
-  <a href="https://github.com/voidful/aidev">
-        <img src="https://visitor-badge.glitch.me/badge?page_id=voidful.aidev" alt="Visitor" />
-    </a>
 </div>
 
 ---
 
 ## 🌟 Features
 
 - Run mock tests on your latest code changes before committing, powered by AI
@@ -78,25 +75,25 @@
 - **Threshold**: Set the confidence threshold for the AI-generated results (ranging from 0.0 to 1.0).
 - **Engine**: Choose the GPT engine to use (e.g., "gpt-3.5-turbo", "gpt-4", "gpt-4-32k").
 - **Max Tokens**: Specify the maximum number of tokens in the AI-generated response.
 - **Language**: Set the output language for the AI-generated response.
 
 #### Configuration management:
 
-The `aidev-config` CLI command allows you to view, add, update, or remove configuration settings. The command
-provides a user-friendly interface to manage your settings.
+The `aidev-config` CLI command allows you to view, add, update, or remove configuration settings. The command provides a
+user-friendly interface to manage your settings.
 
 To set up and manage the configuration, follow these steps:
 
 1. Run the `aidev-config` command with the desired subcommand, e.g., `aidev-config set-api-key <your-api-key>`.
 2. The CLI will update the configuration with the provided value.
 3. Use `aidev-config show-config` to view the current configuration settings.
 
-The main CLI tool, `aidev`, reads the configuration settings and applies them when generating AI responses, ensuring
-a customized experience based on your preferences.
+The main CLI tool, `aidev`, reads the configuration settings and applies them when generating AI responses, ensuring a
+customized experience based on your preferences.
 
 ### 📚 How it works
 
 AI Test harnesses the power of OpenAI's GPT-4 to provide real-time assistance for developers. When you run the CLI tool
 with your code changes, it performs the following steps:
 
 - Retrieve code changes: The tool first runs git diff to capture the latest code changes in your repository.
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
                                fail afterward?
              Introducing an AI-powered(Chatgpt/gpt4) solution to
                      â¨ Run mock tests before committing
      ð Get valuable suggestions to improve your code before you commit
 ð  Automatically generate unit tests for your code changes before committing
    ð Generate insightful commit messages automatically based on your code
                                     changes
-                   [PyPI] [Download] [Last_Commit] [Visitor]
+                        [PyPI] [Download] [Last_Commit]
 --- ## ð Features - Run mock tests on your latest code changes before
 committing, powered by AI - Get actionable code improvement suggestions to
 optimize your codebase - Automatically generate unit tests for your code
 changes, saving you time and effort - Easy-to-use CLI with configuration
 options for a tailored experience - Improve code quality, reduce technical
 debt, and increase confidence in your commits ## ð¦ Installation Install the
 AI Test package using pip: ```bash pip install aidev ``` ## ð Quick Start
```

### Comparing `aidev-0.3/aidev/config_manager.py` & `aidev-0.4/aidev/config_manager.py`

 * *Files identical despite different names*

