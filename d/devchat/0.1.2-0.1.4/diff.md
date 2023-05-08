# Comparing `tmp/devchat-0.1.2.tar.gz` & `tmp/devchat-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devchat-0.1.2.tar", last modified: Sun Apr 23 13:55:37 2023, max compression
+gzip compressed data, was "devchat-0.1.4.tar", last modified: Mon May  8 09:08:26 2023, max compression
```

## Comparing `devchat-0.1.2.tar` & `devchat-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,35 @@
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-04-23 13:55:37.042240 devchat-0.1.2/
--rw-r--r--   0 basicthinker   (501) staff       (20)    11357 2023-04-17 07:54:02.000000 devchat-0.1.2/LICENSE
--rw-r--r--   0 basicthinker   (501) staff       (20)       73 2023-04-23 13:55:37.042102 devchat-0.1.2/PKG-INFO
--rw-r--r--   0 basicthinker   (501) staff       (20)       44 2023-04-17 09:53:56.000000 devchat-0.1.2/README.md
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-04-23 13:55:37.040339 devchat-0.1.2/devchat/
--rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-04-17 08:20:09.000000 devchat-0.1.2/devchat/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     4607 2023-04-23 12:43:58.000000 devchat-0.1.2/devchat/_cli.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-04-23 13:55:37.041356 devchat-0.1.2/devchat/chat/
--rw-r--r--   0 basicthinker   (501) staff       (20)       43 2023-04-23 12:43:58.000000 devchat-0.1.2/devchat/chat/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1203 2023-04-23 12:43:58.000000 devchat-0.1.2/devchat/chat/chat.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     3198 2023-04-23 12:43:58.000000 devchat-0.1.2/devchat/chat/openai_chat.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     2999 2023-04-23 12:43:58.000000 devchat-0.1.2/devchat/message.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     3687 2023-04-23 12:43:58.000000 devchat-0.1.2/devchat/prompt.py
--rw-r--r--   0 basicthinker   (501) staff       (20)      332 2023-04-23 12:43:58.000000 devchat-0.1.2/devchat/utils.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-04-23 13:55:37.040993 devchat-0.1.2/devchat.egg-info/
--rw-r--r--   0 basicthinker   (501) staff       (20)       73 2023-04-23 13:55:37.000000 devchat-0.1.2/devchat.egg-info/PKG-INFO
--rw-r--r--   0 basicthinker   (501) staff       (20)      454 2023-04-23 13:55:37.000000 devchat-0.1.2/devchat.egg-info/SOURCES.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)        1 2023-04-23 13:55:37.000000 devchat-0.1.2/devchat.egg-info/dependency_links.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)       46 2023-04-23 13:55:37.000000 devchat-0.1.2/devchat.egg-info/entry_points.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)       78 2023-04-23 13:55:37.000000 devchat-0.1.2/devchat.egg-info/requires.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)        8 2023-04-23 13:55:37.000000 devchat-0.1.2/devchat.egg-info/top_level.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)      102 2023-04-17 09:50:08.000000 devchat-0.1.2/pyproject.toml
--rw-r--r--   0 basicthinker   (501) staff       (20)       38 2023-04-23 13:55:37.042277 devchat-0.1.2/setup.cfg
--rw-r--r--   0 basicthinker   (501) staff       (20)      347 2023-04-23 13:49:04.000000 devchat-0.1.2/setup.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-04-23 13:55:37.041884 devchat-0.1.2/tests/
--rw-r--r--   0 basicthinker   (501) staff       (20)     1175 2023-04-23 12:43:58.000000 devchat-0.1.2/tests/test_cli.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     2049 2023-04-23 12:43:58.000000 devchat-0.1.2/tests/test_message.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     3033 2023-04-23 12:43:58.000000 devchat-0.1.2/tests/test_prompt.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-08 09:08:26.267629 devchat-0.1.4/
+-rw-r--r--   0 basicthinker   (501) staff       (20)    11357 2023-05-05 13:17:54.000000 devchat-0.1.4/LICENSE
+-rw-r--r--   0 basicthinker   (501) staff       (20)      227 2023-05-08 09:08:26.267445 devchat-0.1.4/PKG-INFO
+-rw-r--r--   0 basicthinker   (501) staff       (20)       44 2023-05-05 13:17:54.000000 devchat-0.1.4/README.md
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-08 09:08:26.264187 devchat-0.1.4/devchat/
+-rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.4/devchat/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5399 2023-05-08 04:39:28.000000 devchat-0.1.4/devchat/_cli.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     4363 2023-05-08 03:39:48.000000 devchat-0.1.4/devchat/assistant.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1464 2023-05-05 13:17:54.000000 devchat-0.1.4/devchat/chat.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)      614 2023-05-07 23:44:52.000000 devchat-0.1.4/devchat/message.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-08 09:08:26.265987 devchat-0.1.4/devchat/openai/
+-rw-r--r--   0 basicthinker   (501) staff       (20)      248 2023-05-05 13:17:54.000000 devchat-0.1.4/devchat/openai/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     3402 2023-05-08 03:20:19.000000 devchat-0.1.4/devchat/openai/openai_chat.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1561 2023-05-07 23:44:52.000000 devchat-0.1.4/devchat/openai/openai_message.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5332 2023-05-07 23:44:52.000000 devchat-0.1.4/devchat/openai/openai_prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5891 2023-05-08 03:39:48.000000 devchat-0.1.4/devchat/prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     3568 2023-05-08 03:39:48.000000 devchat-0.1.4/devchat/store.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     3783 2023-05-07 23:44:52.000000 devchat-0.1.4/devchat/utils.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-08 09:08:26.265090 devchat-0.1.4/devchat.egg-info/
+-rw-r--r--   0 basicthinker   (501) staff       (20)      227 2023-05-08 09:08:26.000000 devchat-0.1.4/devchat.egg-info/PKG-INFO
+-rw-r--r--   0 basicthinker   (501) staff       (20)      628 2023-05-08 09:08:26.000000 devchat-0.1.4/devchat.egg-info/SOURCES.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)        1 2023-05-08 09:08:26.000000 devchat-0.1.4/devchat.egg-info/dependency_links.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)       46 2023-05-08 09:08:26.000000 devchat-0.1.4/devchat.egg-info/entry_points.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)      100 2023-05-08 09:08:26.000000 devchat-0.1.4/devchat.egg-info/requires.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)       14 2023-05-08 09:08:26.000000 devchat-0.1.4/devchat.egg-info/top_level.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)      102 2023-05-05 13:17:54.000000 devchat-0.1.4/pyproject.toml
+-rw-r--r--   0 basicthinker   (501) staff       (20)       38 2023-05-08 09:08:26.267666 devchat-0.1.4/setup.cfg
+-rw-r--r--   0 basicthinker   (501) staff       (20)      547 2023-05-08 09:07:10.000000 devchat-0.1.4/setup.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-08 09:08:26.267191 devchat-0.1.4/tests/
+-rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.4/tests/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     3899 2023-05-08 03:39:48.000000 devchat-0.1.4/tests/test_cli.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1809 2023-05-07 23:44:52.000000 devchat-0.1.4/tests/test_openai_message.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5908 2023-05-07 23:44:52.000000 devchat-0.1.4/tests/test_openai_prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     2303 2023-05-05 15:34:17.000000 devchat-0.1.4/tests/test_store.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1225 2023-05-07 23:44:52.000000 devchat-0.1.4/tests/test_utils.py
```

### Comparing `devchat-0.1.2/LICENSE` & `devchat-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `devchat-0.1.2/devchat/_cli.py` & `devchat-0.1.4/devchat/_cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,167 +1,178 @@
 """
 This module contains the main function for the DevChat CLI.
 """
+from contextlib import contextmanager
+import json
+import os
+import sys
+from typing import List, Optional, Tuple
+import rich_click as click
+from devchat.store import Store
+from devchat.openai import OpenAIChatConfig, OpenAIChat
+from devchat.assistant import Assistant
+from devchat.utils import find_git_root, git_ignore, parse_files
 
 
-from typing import Optional
-import json
-import click
-from pydantic import ValidationError
-from devchat.message import Message
-from devchat.chat.openai_chat import OpenAIChatConfig, OpenAIChat
-from devchat.prompt import Prompt
+click.rich_click.USE_MARKDOWN = True
 
 
-@click.command()
-@click.argument('content', required=False)
-@click.option('-h', '--help', is_flag=True, help='Show the help message and exit.')
-def main(content: Optional[str], help: bool):
-    """
-    Main function to run the chat application.
+@click.group()
+def main():
+    """DevChat CLI: A command-line interface for the DevChat chatbot."""
+
+
+@contextmanager
+def handle_errors():
+    """Handle errors in the CLI."""
+    try:
+        yield
+    except Exception as error:
+        click.echo(f"Error: {error}", err=True)
+        sys.exit(os.EX_SOFTWARE)
 
-    This function initializes the chat system based on the specified large language model (LLM),
-    and performs interactions with the user by sending prompts and retrieving responses.
-    """
-    if help:
-        print_help()
-        return
 
-    if content is None:
-        content = click.get_text_stream('stdin').read()
+def init_dir() -> Tuple[dict, Store]:
+    git_root = find_git_root()
+    chat_dir = os.path.join(git_root, ".chat")
+    if not os.path.exists(chat_dir):
+        os.makedirs(chat_dir)
 
     default_config_data = {
-        'llm': 'OpenAI',
+        'model': 'gpt-3.5-turbo',
+        'provider': 'OpenAI',
         'OpenAI': {
-            'model': 'gpt-3.5-turbo',
             'temperature': 0.2
         }
     }
 
     try:
-        with open('.chatconfig.json', 'r', encoding='utf-8') as file:
+        with open(os.path.join(chat_dir, 'config.json'), 'r', encoding='utf-8') as file:
             config_data = json.load(file)
     except FileNotFoundError:
         config_data = default_config_data
 
-    message = Message("user", content)
-
-    llm = config_data.get('llm')
-
-    if llm == 'OpenAI':
-        try:
-            openai_config = OpenAIChatConfig(**config_data['OpenAI'])
-            chat = OpenAIChat(openai_config)
-            prompt = Prompt(chat.config.model)
-            chat.prompt([message])
-
-            if openai_config.stream:
-                response_iterator = chat.stream_response()
-                for response_chunk in response_iterator:
-                    delta_str = prompt.append_response(str(response_chunk))
-                    if delta_str is None:
-                        click.echo()
-                    else:
-                        click.echo(delta_str, nl=False)
-                for i in range(1, len(prompt.responses)):
-                    click.echo(f"[{i}]: {prompt.responses[i].content}")
-
-            else:
-                response_str = str(chat.complete_response())
-                prompt.set_response(response_str)
-                if len(prompt.responses) == 1:
-                    click.echo(prompt.responses[0].content)
-                else:
-                    for index, response in prompt.responses.items():
-                        click.echo(f"[{index}]: {response.content}")
-
-        except ValidationError as error:
-            click.echo(f"Error: {error}")
-    else:
-        click.echo(f"Unknown LLM: {llm}")
+    store = Store(chat_dir)
+    git_ignore(git_root, store.graph_path, store.db_path)
+    return config_data, store
 
 
-def print_help():
-    """
-    Print the help message for the DevChat CLI.
+@main.command()
+@click.argument('content', required=False)
+@click.option('-p', '--parent', help='Input the parent prompt hash to continue the conversation.')
+@click.option('-r', '--reference', multiple=True,
+              help='Input one or more specific previous prompts to include in the current prompt.')
+@click.option('-i', '--instruct', multiple=True,
+              help='Add one or more files to the prompt as instructions.')
+@click.option('-c', '--context', multiple=True,
+              help='Add one or more files to the prompt as a context.')
+@click.option('-m', '--model', help='Specify the model to use for the prompt.')
+def prompt(content: Optional[str], parent: Optional[str], reference: Optional[List[str]],
+           instruct: Optional[List[str]], context: Optional[List[str]], model: Optional[str]):
     """
-    help_text = """
-    This manual provides instructions on how to use the DevChat CLI,
-    a command-line interface for interacting with a large language model (LLM).
-
-    Usage
-    -----
-
-    To use the DevChat CLI, run the following command:
-
-    ```
-    devchat [OPTIONS] [CONTENT]
-    ```
-
-    Arguments
-    ---------
-
-    - `content` (optional): One or more lines of text for the Message object.
-                            If not provided, the CLI will read from standard input.
-
-    Options
-    -------
+    Main function to run the chat application.
 
-    - `-h`, `--help`: Show the help message and exit.
+    This function initializes the chat system based on the specified large language model (LLM),
+    and performs interactions with the user by sending prompts and retrieving responses.
 
     Examples
     --------
 
-    ### Single-line input
-
     To send a single-line message to the LLM, provide the content as an argument:
 
+    ```bash
+    devchat prompt "What is the capital of France?"
     ```
-    devchat "What is the capital of France?"
-    ```
-
-    ### Multi-line input using here-doc
 
     To send a multi-line message to the LLM, use the here-doc syntax:
 
     ```bash
-    devchat << EOF
+    devchat prompt << 'EOF'
     What is the capital of France?
     Can you tell me more about its history?
     EOF
     ```
 
+    Note the quotes around EOF in the first line, to prevent the shell from expanding variables.
+
     Configuration
     -------------
 
     The DevChat CLI reads its configuration from a file `.chatconfig.json` in the current directory.
     If the file is not found, it uses the following default configuration:
-
     ```json
     {
-        "llm": "OpenAI",
+        "model": "gpt-3.5-turbo",
+        "provider": "OpenAI",
         "OpenAI": {
-            "model": "gpt-3.5-turbo",
             "temperature": 0.2
         }
     }
     ```
 
     To customize the configuration, create a `.chatconfig.json` file in the current directory and
     modify the settings as needed. We recoommend the following settings:
+    ```json
     {
-        "llm": "OpenAI",
+        "model": "gpt-4",
+        "provider": "OpenAI",
         "OpenAI": {
-            "model": "gpt-4",
             "temperature": 0.2,
             "stream": true
         }
     }
+    ```
 
-    Note: If you are using an OpenAI's model, you must have an API key to use the CLI.
-    Run the following command line before using the CLI:
+    Note: To use OpenAI's APIs, you must have an API key to run the CLI.
+    Run the following command line with your API key:
 
     ```bash
     export OPENAI_API_KEY="sk-..."
     ```
+
     """
-    click.echo(help_text)
+    config, store = init_dir()
+
+    with handle_errors():
+        if content is None:
+            content = click.get_text_stream('stdin').read()
+
+        if content == '':
+            return
+
+        instruct_contents = parse_files(instruct)
+        context_contents = parse_files(context)
+
+        provider = config.get('provider')
+        if provider == 'OpenAI':
+            if model is None:
+                model = config['model']
+            openai_config = OpenAIChatConfig(model=model, **config['OpenAI'])
+
+            chat = OpenAIChat(openai_config)
+
+            openai_asisstant = Assistant(chat, store)
+            openai_asisstant.make_prompt(content, instruct_contents, context_contents,
+                                         parent, reference)
+
+            for response in openai_asisstant.iterate_response():
+                click.echo(response, nl=False)
+        else:
+            click.echo(f"Error: Invalid LLM in configuration '{provider}'", err=True)
+            sys.exit(os.EX_DATAERR)
+
+
+@main.command()
+@click.option('--skip', default=0, help='Skip number prompts before showing the prompt history.')
+@click.option('--max-count', default=100, help='Limit the number of commits to output.')
+def log(skip, max_count):
+    """
+    Show the prompt history.
+    """
+    _, store = init_dir()
+
+    recent_prompts = store.select_recent(skip, skip + max_count)
+
+    logs = []
+    for record in recent_prompts:
+        logs.append(record.shortlog())
+    click.echo(json.dumps(logs, indent=2))
```

