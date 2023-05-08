# Comparing `tmp/gpt-chat-cli-0.1.1.tar.gz` & `tmp/gpt-chat-cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-chat-cli-0.1.1.tar", last modified: Sat May  6 22:06:28 2023, max compression
+gzip compressed data, was "gpt-chat-cli-0.1.2.tar", last modified: Mon May  8 21:52:04 2023, max compression
```

## Comparing `gpt-chat-cli-0.1.1.tar` & `gpt-chat-cli-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 22:06:28.691866 gpt-chat-cli-0.1.1/
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     1052 2023-05-04 23:39:54.000000 gpt-chat-cli-0.1.1/LICENSE
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10705 2023-05-06 22:06:28.691866 gpt-chat-cli-0.1.1/PKG-INFO
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10176 2023-05-06 22:03:39.000000 gpt-chat-cli-0.1.1/README.md
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      587 2023-05-06 22:05:07.000000 gpt-chat-cli-0.1.1/pyproject.toml
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       38 2023-05-06 22:06:28.691866 gpt-chat-cli-0.1.1/setup.cfg
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      441 2023-05-06 22:05:13.000000 gpt-chat-cli-0.1.1/setup.py
-drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 22:06:28.688532 gpt-chat-cli-0.1.1/src/
-drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 22:06:28.688532 gpt-chat-cli-0.1.1/src/gpt_chat_cli/
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-05 05:27:20.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli/__init__.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10360 2023-05-06 20:06:24.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli/argparsing.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     5690 2023-05-06 10:40:40.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli/chat_colorizer.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     1979 2023-05-06 19:56:25.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli/color.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     8587 2023-05-06 19:57:38.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli/gcli.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     2873 2023-05-06 21:24:43.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli/openai_wrappers.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     9556 2023-05-06 10:41:58.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli/streaming_lexer.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       18 2023-05-06 22:05:24.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli/version.py
-drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 22:06:28.691866 gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10705 2023-05-06 22:06:28.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/PKG-INFO
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      559 2023-05-06 22:06:28.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/SOURCES.txt
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)        1 2023-05-06 22:06:28.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/dependency_links.txt
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       56 2023-05-06 22:06:28.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/entry_points.txt
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       43 2023-05-06 22:06:28.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/requires.txt
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       13 2023-05-06 22:06:28.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/top_level.txt
-drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 22:06:28.691866 gpt-chat-cli-0.1.1/tests/
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     5409 2023-05-06 07:11:24.000000 gpt-chat-cli-0.1.1/tests/test_streaming_lexer.py
+drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-08 21:52:04.972420 gpt-chat-cli-0.1.2/
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     1052 2023-05-04 23:39:54.000000 gpt-chat-cli-0.1.2/LICENSE
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    12036 2023-05-08 21:52:04.972420 gpt-chat-cli-0.1.2/PKG-INFO
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    11507 2023-05-06 23:08:59.000000 gpt-chat-cli-0.1.2/README.md
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      587 2023-05-08 21:44:34.000000 gpt-chat-cli-0.1.2/pyproject.toml
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       38 2023-05-08 21:52:04.972420 gpt-chat-cli-0.1.2/setup.cfg
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      441 2023-05-08 21:44:26.000000 gpt-chat-cli-0.1.2/setup.py
+drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-08 21:52:04.969087 gpt-chat-cli-0.1.2/src/
+drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-08 21:52:04.972420 gpt-chat-cli-0.1.2/src/gpt_chat_cli/
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-05 05:27:20.000000 gpt-chat-cli-0.1.2/src/gpt_chat_cli/__init__.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10360 2023-05-06 20:06:24.000000 gpt-chat-cli-0.1.2/src/gpt_chat_cli/argparsing.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     5132 2023-05-06 22:21:07.000000 gpt-chat-cli-0.1.2/src/gpt_chat_cli/chat_colorizer.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     1979 2023-05-08 21:41:23.000000 gpt-chat-cli-0.1.2/src/gpt_chat_cli/color.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     9244 2023-05-08 21:41:19.000000 gpt-chat-cli-0.1.2/src/gpt_chat_cli/gcli.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     2873 2023-05-06 21:24:43.000000 gpt-chat-cli-0.1.2/src/gpt_chat_cli/openai_wrappers.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     9556 2023-05-06 10:41:58.000000 gpt-chat-cli-0.1.2/src/gpt_chat_cli/streaming_lexer.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       18 2023-05-08 21:44:09.000000 gpt-chat-cli-0.1.2/src/gpt_chat_cli/version.py
+drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-08 21:52:04.972420 gpt-chat-cli-0.1.2/src/gpt_chat_cli.egg-info/
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    12036 2023-05-08 21:52:04.000000 gpt-chat-cli-0.1.2/src/gpt_chat_cli.egg-info/PKG-INFO
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      559 2023-05-08 21:52:04.000000 gpt-chat-cli-0.1.2/src/gpt_chat_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)        1 2023-05-08 21:52:04.000000 gpt-chat-cli-0.1.2/src/gpt_chat_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       56 2023-05-08 21:52:04.000000 gpt-chat-cli-0.1.2/src/gpt_chat_cli.egg-info/entry_points.txt
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       43 2023-05-08 21:52:04.000000 gpt-chat-cli-0.1.2/src/gpt_chat_cli.egg-info/requires.txt
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       13 2023-05-08 21:52:04.000000 gpt-chat-cli-0.1.2/src/gpt_chat_cli.egg-info/top_level.txt
+drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-08 21:52:04.972420 gpt-chat-cli-0.1.2/tests/
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     5409 2023-05-06 07:11:24.000000 gpt-chat-cli-0.1.2/tests/test_streaming_lexer.py
```

### Comparing `gpt-chat-cli-0.1.1/LICENSE` & `gpt-chat-cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-chat-cli-0.1.1/PKG-INFO` & `gpt-chat-cli-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: gpt-chat-cli
-Version: 0.1.1
-Summary: A simple ChatGPT terminal CLI
-Author: Flu0r1ne
-Author-email: Flu0r1ne <flu0r1ne@flu0r1ne.net>
-Project-URL: Homepage, https://github.com/flu0r1ne/gpt-chat-cli
-Project-URL: Bug Tracker, https://github.com/flu0r1ne/gpt-chat-cli/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 gpt-chat-cli: a simple yet powerful ChatGPT CLI
 -----------------------------------------------
 
 ## Introduction
 
 `gpt-chat-cli` is a simple, general purpose ChatGPT CLI. It brings the power of ChatGPT to the command line. It aims to be easy to use and highly configurable.
 
@@ -80,15 +65,15 @@
 Press Control-D to exit
 [#] What linux command prints a list of all open TCP sockets on port 8080?
 [gpt-3.5-turbo-0301] You can use the `lsof` (list open files) command to list all
 open TCP sockets on a specific port. The command to list all open TCP sockets on
 port 8080 is `sudo lsof -i :8080`
 
 
-[#] Can do do this with ss?
+[#] Can you do this with ss?
 [gpt-3.5-turbo-0301] Yes, you can also use the `ss` (socket statistics) command to
 list all open TCP sockets on port 8080. The command to list all open TCP sockets
 on port 8080 using `ss` is `sudo ss -tlnp 'sport = :8080'`
 ```
 
 `gpt-chat-cli` respects pipes and redirects, so you can use it in combination with other command-line tools:
 
@@ -219,14 +204,64 @@
 
 1. Naming: The function name `quicksort` is not very descriptive. It would be better to name it something like `quicksort_entries_by_access_time` to make it clear what it does.
 
 ...
 [#]
 ```
 
+Create a bash alias for a particular model:
+
+```
+$ alias gpt3='gpt-chat-cli -m gpt-3.5-turbo'
+$ gpt3
+[#] ...
+```
+
+Of course, custom scripting can extend the capabilities. For example, this `bash` function will suggest commands to accomplish tasks on the command line:
+
+```bash
+function cmd {
+	local request="$1"
+	local shell=$(basename "${SHELL}")
+
+	local os=""
+
+	if command -v lsb_release >/dev/null 2>&1; then
+		os="$ lsb_release -a\n$(lsb_release -a)\n"
+	fi
+
+	local kernel=""
+
+	if command -v uname >/dev/null 2>&1; then
+		kernel="$ uname -s -r\n$(uname -s -r)\n"
+	fi
+
+	local prompt=""
+
+	prompt="${prompt}Suggest a command to be run in the $shell to accomplish the following task:\n\n"
+	prompt="${prompt}$request\n\n"
+	prompt="${prompt}Please output the command and a short description\n\n"
+
+	if [ -n "${os}" ] || [ -n "${kernel}" ]; then
+		prompt="${prompt}Here is some additional info about the system:\n\n${os}${kernel}"
+	fi
+
+	printf "$prompt" | gpt-chat-cli
+}
+```
+
+```
+$ cmd "test if ip forwarding is enabled"
+[gpt-3.5-turbo-0301] You can use the `sysctl` command to test if IP forwarding is enabled. Here's the command you can run in your zsh shell:
+
+sysctl net.ipv4.ip_forward
+
+This command will return `net.ipv4.ip_forward = 0` if IP forwarding is disabled and `net.ipv4.ip_forward = 1` if IP forwarding is enabled.
+```
+
 #### Known Issues
 
 There are a couple known issues. PRs are accepted:
 
 1. `gpt-chat-cli` lacks shell completion
 2. `gpt-chat-cli` does not track token usage. Ideally, it should gracefully handle long messages and remove messages from the chat history if the number of tokens in the context is exceeded. If the tokens exceed the model's context, the following error will occur:
```

### Comparing `gpt-chat-cli-0.1.1/README.md` & `gpt-chat-cli-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: gpt-chat-cli
+Version: 0.1.2
+Summary: A simple ChatGPT terminal CLI
+Author: Flu0r1ne
+Author-email: Flu0r1ne <flu0r1ne@flu0r1ne.net>
+Project-URL: Homepage, https://github.com/flu0r1ne/gpt-chat-cli
+Project-URL: Bug Tracker, https://github.com/flu0r1ne/gpt-chat-cli/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 gpt-chat-cli: a simple yet powerful ChatGPT CLI
 -----------------------------------------------
 
 ## Introduction
 
 `gpt-chat-cli` is a simple, general purpose ChatGPT CLI. It brings the power of ChatGPT to the command line. It aims to be easy to use and highly configurable.
 
@@ -65,15 +80,15 @@
 Press Control-D to exit
 [#] What linux command prints a list of all open TCP sockets on port 8080?
 [gpt-3.5-turbo-0301] You can use the `lsof` (list open files) command to list all
 open TCP sockets on a specific port. The command to list all open TCP sockets on
 port 8080 is `sudo lsof -i :8080`
 
 
-[#] Can do do this with ss?
+[#] Can you do this with ss?
 [gpt-3.5-turbo-0301] Yes, you can also use the `ss` (socket statistics) command to
 list all open TCP sockets on port 8080. The command to list all open TCP sockets
 on port 8080 using `ss` is `sudo ss -tlnp 'sport = :8080'`
 ```
 
 `gpt-chat-cli` respects pipes and redirects, so you can use it in combination with other command-line tools:
 
@@ -204,14 +219,64 @@
 
 1. Naming: The function name `quicksort` is not very descriptive. It would be better to name it something like `quicksort_entries_by_access_time` to make it clear what it does.
 
 ...
 [#]
 ```
 
+Create a bash alias for a particular model:
+
+```
+$ alias gpt3='gpt-chat-cli -m gpt-3.5-turbo'
+$ gpt3
+[#] ...
+```
+
+Of course, custom scripting can extend the capabilities. For example, this `bash` function will suggest commands to accomplish tasks on the command line:
+
+```bash
+function cmd {
+	local request="$1"
+	local shell=$(basename "${SHELL}")
+
+	local os=""
+
+	if command -v lsb_release >/dev/null 2>&1; then
+		os="$ lsb_release -a\n$(lsb_release -a)\n"
+	fi
+
+	local kernel=""
+
+	if command -v uname >/dev/null 2>&1; then
+		kernel="$ uname -s -r\n$(uname -s -r)\n"
+	fi
+
+	local prompt=""
+
+	prompt="${prompt}Suggest a command to be run in the $shell to accomplish the following task:\n\n"
+	prompt="${prompt}$request\n\n"
+	prompt="${prompt}Please output the command and a short description\n\n"
+
+	if [ -n "${os}" ] || [ -n "${kernel}" ]; then
+		prompt="${prompt}Here is some additional info about the system:\n\n${os}${kernel}"
+	fi
+
+	printf "$prompt" | gpt-chat-cli
+}
+```
+
+```
+$ cmd "test if ip forwarding is enabled"
+[gpt-3.5-turbo-0301] You can use the `sysctl` command to test if IP forwarding is enabled. Here's the command you can run in your zsh shell:
+
+sysctl net.ipv4.ip_forward
+
+This command will return `net.ipv4.ip_forward = 0` if IP forwarding is disabled and `net.ipv4.ip_forward = 1` if IP forwarding is enabled.
+```
+
 #### Known Issues
 
 There are a couple known issues. PRs are accepted:
 
 1. `gpt-chat-cli` lacks shell completion
 2. `gpt-chat-cli` does not track token usage. Ideally, it should gracefully handle long messages and remove messages from the chat history if the number of tokens in the context is exceeded. If the tokens exceed the model's context, the following error will occur:
```

### Comparing `gpt-chat-cli-0.1.1/pyproject.toml` & `gpt-chat-cli-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpt-chat-cli"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Flu0r1ne", email="flu0r1ne@flu0r1ne.net" },
 ]
 description = "A simple ChatGPT terminal CLI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `gpt-chat-cli-0.1.1/src/gpt_chat_cli/argparsing.py` & `gpt-chat-cli-0.1.2/src/gpt_chat_cli/argparsing.py`

 * *Files identical despite different names*

### Comparing `gpt-chat-cli-0.1.1/src/gpt_chat_cli/chat_colorizer.py` & `gpt-chat-cli-0.1.2/src/gpt_chat_cli/chat_colorizer.py`

 * *Files 19% similar despite different names*

```diff
@@ -212,56 +212,7 @@
 
                 print( f'{self.color_code.WHITE}{token.content}{self.color_code.RESET}', end='', flush=True )
                 self.text_emitted = True
 
 
     def finish( self : "ChatColorizer" ):
         self.lexer.finish()
-
-
-# content = '''
-# Rust code:
-
-# ```rust
-# fn main() {
-#     let x = 5;
-#     let y = 10;
-#     let z = x + y;
-#     println!("The value of z is {}", z);
-# }
-# ```
-
-# Python code:
-
-# ```python
-# x = 5
-# y = 10
-# z = x + y
-# print("The value of z is", z)
-# ```
-
-# Unknown code:
-
-# ```
-# x = 5
-# y = 10
-# z = x + y
-# print("The value of z is", z)
-# ```
-
-
-# Testing
-
-# ```python
-# x = 5
-# y = 10
-# z = x + y
-# print("The value of z is", z)
-
-# '''
-
-# highlighter = ChatColorizer()
-
-# highlighter.add_chunk(content)
-# highlighter.finish()
-
-# highlighter.print()
```

### Comparing `gpt-chat-cli-0.1.1/src/gpt_chat_cli/color.py` & `gpt-chat-cli-0.1.2/src/gpt_chat_cli/color.py`

 * *Files identical despite different names*

### Comparing `gpt-chat-cli-0.1.1/src/gpt_chat_cli/gcli.py` & `gpt-chat-cli-0.1.2/src/gpt_chat_cli/gcli.py`

 * *Files 8% similar despite different names*

```diff
@@ -215,26 +215,47 @@
 def cmd_version():
     print(f'version {VERSION}')
 
 def cmd_list_models():
     for model in list_models():
         print(model)
 
+def surround_ansi_escapes(prompt, start = "\x01", end = "\x02"):
+        '''
+        Fixes issue on Linux with the readline module
+        See: https://github.com/python/cpython/issues/61539
+        '''
+        escaped = False
+        result = ""
+
+        for c in prompt:
+                if c == "\x1b" and not escaped:
+                        result += start + c
+                        escaped = True
+                elif c.isalpha() and escaped:
+                        result += c + end
+                        escaped = False
+                else:
+                        result += c
+
+        return result
+
 def cmd_interactive(args : Arguments):
 
     enable_emacs_editing()
 
     COLOR_CODE = get_color_codes(no_color = not args.display_args.color)
 
     completion_args = args.completion_args
     display_args = args.display_args
 
     hist = [ get_system_message( args.system_message ) ]
 
     PROMPT = f'[{COLOR_CODE.WHITE}#{COLOR_CODE.RESET}] '
+    PROMPT = surround_ansi_escapes(PROMPT)
 
     def prompt_message() -> bool:
 
         # Control-D closes the input stream
         try:
             message = input( PROMPT )
         except (EOFError, KeyboardInterrupt):
```

### Comparing `gpt-chat-cli-0.1.1/src/gpt_chat_cli/openai_wrappers.py` & `gpt-chat-cli-0.1.2/src/gpt_chat_cli/openai_wrappers.py`

 * *Files identical despite different names*

### Comparing `gpt-chat-cli-0.1.1/src/gpt_chat_cli/streaming_lexer.py` & `gpt-chat-cli-0.1.2/src/gpt_chat_cli/streaming_lexer.py`

 * *Files identical despite different names*

### Comparing `gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/PKG-INFO` & `gpt-chat-cli-0.1.2/src/gpt_chat_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-chat-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple ChatGPT terminal CLI
 Author: Flu0r1ne
 Author-email: Flu0r1ne <flu0r1ne@flu0r1ne.net>
 Project-URL: Homepage, https://github.com/flu0r1ne/gpt-chat-cli
 Project-URL: Bug Tracker, https://github.com/flu0r1ne/gpt-chat-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -80,15 +80,15 @@
 Press Control-D to exit
 [#] What linux command prints a list of all open TCP sockets on port 8080?
 [gpt-3.5-turbo-0301] You can use the `lsof` (list open files) command to list all
 open TCP sockets on a specific port. The command to list all open TCP sockets on
 port 8080 is `sudo lsof -i :8080`
 
 
-[#] Can do do this with ss?
+[#] Can you do this with ss?
 [gpt-3.5-turbo-0301] Yes, you can also use the `ss` (socket statistics) command to
 list all open TCP sockets on port 8080. The command to list all open TCP sockets
 on port 8080 using `ss` is `sudo ss -tlnp 'sport = :8080'`
 ```
 
 `gpt-chat-cli` respects pipes and redirects, so you can use it in combination with other command-line tools:
 
@@ -219,14 +219,64 @@
 
 1. Naming: The function name `quicksort` is not very descriptive. It would be better to name it something like `quicksort_entries_by_access_time` to make it clear what it does.
 
 ...
 [#]
 ```
 
+Create a bash alias for a particular model:
+
+```
+$ alias gpt3='gpt-chat-cli -m gpt-3.5-turbo'
+$ gpt3
+[#] ...
+```
+
+Of course, custom scripting can extend the capabilities. For example, this `bash` function will suggest commands to accomplish tasks on the command line:
+
+```bash
+function cmd {
+	local request="$1"
+	local shell=$(basename "${SHELL}")
+
+	local os=""
+
+	if command -v lsb_release >/dev/null 2>&1; then
+		os="$ lsb_release -a\n$(lsb_release -a)\n"
+	fi
+
+	local kernel=""
+
+	if command -v uname >/dev/null 2>&1; then
+		kernel="$ uname -s -r\n$(uname -s -r)\n"
+	fi
+
+	local prompt=""
+
+	prompt="${prompt}Suggest a command to be run in the $shell to accomplish the following task:\n\n"
+	prompt="${prompt}$request\n\n"
+	prompt="${prompt}Please output the command and a short description\n\n"
+
+	if [ -n "${os}" ] || [ -n "${kernel}" ]; then
+		prompt="${prompt}Here is some additional info about the system:\n\n${os}${kernel}"
+	fi
+
+	printf "$prompt" | gpt-chat-cli
+}
+```
+
+```
+$ cmd "test if ip forwarding is enabled"
+[gpt-3.5-turbo-0301] You can use the `sysctl` command to test if IP forwarding is enabled. Here's the command you can run in your zsh shell:
+
+sysctl net.ipv4.ip_forward
+
+This command will return `net.ipv4.ip_forward = 0` if IP forwarding is disabled and `net.ipv4.ip_forward = 1` if IP forwarding is enabled.
+```
+
 #### Known Issues
 
 There are a couple known issues. PRs are accepted:
 
 1. `gpt-chat-cli` lacks shell completion
 2. `gpt-chat-cli` does not track token usage. Ideally, it should gracefully handle long messages and remove messages from the chat history if the number of tokens in the context is exceeded. If the tokens exceed the model's context, the following error will occur:
```

### Comparing `gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/SOURCES.txt` & `gpt-chat-cli-0.1.2/src/gpt_chat_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-chat-cli-0.1.1/tests/test_streaming_lexer.py` & `gpt-chat-cli-0.1.2/tests/test_streaming_lexer.py`

 * *Files identical despite different names*

