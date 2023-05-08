# Comparing `tmp/vidcardshare-0.1.2.tar.gz` & `tmp/vidcardshare-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidcardshare-0.1.2.tar", max compression
+gzip compressed data, was "vidcardshare-0.1.3.tar", max compression
```

## Comparing `vidcardshare-0.1.2.tar` & `vidcardshare-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       60 2023-05-07 23:44:32.772934 vidcardshare-0.1.2/README.md
--rwxr-xr-x   0        0        0     3941 2023-05-07 21:37:59.860401 vidcardshare-0.1.2/assets/index.html.tpl
--rwxr-xr-x   0        0        0      759 2023-05-07 20:43:56.000000 vidcardshare-0.1.2/assets/script.js
--rwxr-xr-x   0        0        0     6496 2023-05-07 21:31:56.704323 vidcardshare-0.1.2/assets/style.css.tpl
--rw-r--r--   0        0        0      538 2023-05-08 01:00:15.052631 vidcardshare-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-07 21:15:03.156150 vidcardshare-0.1.2/vidcardshare/__init__.py
--rw-r--r--   0        0        0     7968 2023-05-08 01:00:02.256634 vidcardshare-0.1.2/vidcardshare/main.py
--rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 vidcardshare-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     9025 2023-05-08 01:12:44.827677 vidcardshare-0.1.3/README.md
+-rwxr-xr-x   0        0        0     3941 2023-05-07 21:37:59.860401 vidcardshare-0.1.3/assets/index.html.tpl
+-rwxr-xr-x   0        0        0      759 2023-05-07 20:43:56.000000 vidcardshare-0.1.3/assets/script.js
+-rwxr-xr-x   0        0        0     6496 2023-05-07 21:31:56.704323 vidcardshare-0.1.3/assets/style.css.tpl
+-rw-r--r--   0        0        0      696 2023-05-08 02:30:37.909376 vidcardshare-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-07 21:15:03.156150 vidcardshare-0.1.3/vidcardshare/__init__.py
+-rw-r--r--   0        0        0     9535 2023-05-08 02:29:39.657338 vidcardshare-0.1.3/vidcardshare/main.py
+-rw-r--r--   0        0        0     9582 1970-01-01 00:00:00.000000 vidcardshare-0.1.3/PKG-INFO
```

### Comparing `vidcardshare-0.1.2/assets/index.html.tpl` & `vidcardshare-0.1.3/assets/index.html.tpl`

 * *Files identical despite different names*

### Comparing `vidcardshare-0.1.2/assets/script.js` & `vidcardshare-0.1.3/assets/script.js`

 * *Files identical despite different names*

### Comparing `vidcardshare-0.1.2/assets/style.css.tpl` & `vidcardshare-0.1.3/assets/style.css.tpl`

 * *Files identical despite different names*

### Comparing `vidcardshare-0.1.2/pyproject.toml` & `vidcardshare-0.1.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vidcardshare"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Arno V <bcda0276@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/arnos-stuff/vidcardshare.git"
 include = [
     {'path' = 'assets/*'}
 ]
@@ -16,10 +16,18 @@
 pytube = "^15.0.0"
 flask = "^2.3.2"
 
 [tool.poetry.scripts]
 vidcardshare = "vidcardshare.main:app"
 vidcsh = "vidcardshare.main:app"
 
+[tool.poetry.group.dev.dependencies]
+mike = "^1.1.2"
+mkdocs = "^1.4.3"
+mkgendocs = "^0.9.2"
+mkdocs-material = "^9.1.9"
+pillow = "^9.5.0"
+cairosvg = "^2.7.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `vidcardshare-0.1.2/vidcardshare/main.py` & `vidcardshare-0.1.3/vidcardshare/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import typer
 import jinja2 as jj
 import typer_tinydb as ttdb
 import shutil
 
+from rich.prompt import Prompt, Confirm
 from pathlib import Path
 from flask import send_from_directory, Flask, make_response, render_template
 from pytube import YouTube
 
 Pkg = Path(__file__).parent
 Root = Pkg.parent
 Assets = Root / 'assets'
 cssTemplateFile = Assets / 'style.css.tpl'
 htmlTemplateFile = Assets / 'index.html.tpl'
 
 app = typer.Typer(
-    name="vidshare",
+    name="vidcardshare",
     help="Quickly make a small website to share one video, with a card and your name on it + description.",
     no_args_is_help=True,
     rich_help_panel='rich',
     rich_markup_mode='rich'
 )
 
 info = ttdb.cfg.registered_commands
@@ -46,16 +47,32 @@
 DEFAULT_BUILD_PATH.mkdir(parents=True, exist_ok=True)
 
 def attemptGetVarsDB(*vars, **kwargs):
     """Checks the variables have been declared"""
     return {
         var : ttdb.getValue(var) for var in vars
     } | kwargs
-    
+
 def promptVarsMissing(**variables):
+    """Checks if any of the variables are missing, and returns a string
+    containing the missing variables.
+
+    Parameters
+    ----------
+    variables : dict
+        A dictionary where the keys are the variable names and the values
+        are the variable values.
+
+    Returns
+    -------
+    bool
+        True if any of the variables are missing, False otherwise.
+    str
+        A string containing the missing variables.
+    """
     missing = "[bold red]🚩 There are missing variables:[/bold red]\n"
     okay = "[bold green]✅ The following variables are correctly set:[/bold green]\n"
     defaults = "[bold yellow]📦 The following variables are set to the default package value:[/bold yellow]\n"
     misses, oks, defts = False, False, False
     for i, (name, val) in enumerate(variables.items()):
         if not val:
             misses = True
@@ -67,15 +84,35 @@
             oks = True
             okay += f'[green]({i}) {name} (with value = [dim]{val}[/dim])\n[/green]'
         
     rets = ''
     rets += missing if misses else ''
     rets += defaults if defts else ''
     rets += okay if oks else ''
-    return misses, rets
+    return (1 if misses else -1 if defts else 0), rets
+    
+
+
+def checkSourcesDownload(sources: list, variables: dict, youtube_quality: int = 1080):
+    """Function to check if sources are valid files or urls and download them if necessary. Uses PyTube."""
+    for item, name in sources:
+        if (pitm := Path(item)).is_file():
+                variables[name] = pitm.name
+        elif 'www.youtube.com' in item:
+            ttdb.console.print(f"📦 Downloading youtube video in {youtube_quality}p quality", style='yellow')
+            yt = YouTube(item).streams.filter(progressive=True, file_extension='mp4').get_by_resolution(f"{youtube_quality}p")
+            if yt:
+                yt.download(filename=f"{name}_youtube.mp4")
+            else:
+                anyvid = YouTube(item).streams.filter(progressive=True, file_extension='mp4').order_by('resolution').desc().first()               
+                anyvid.download(filename=f"{name}_youtube.mp4")
+            ttdb.upsert_param(name, f"{name}_youtube.mp4")
+            video = f"{name}_youtube.mp4"
+            variables['video_url'] = video
+    return variables
 
 
 @app.command("build", help="""Assuming every parameter was provided, gives you a single zipped archive with your mini website in it. Just put it wherever :)\n❗ [red] Don't miss out ! [/red] you can also add build parameters using [yellow]`var set`[/yellow], type [yellow]`vidshare var`[/yellow] to know more !""")
 def build(
         background_image_url: str = typer.Argument(
             default="https://storage.googleapis.com/open.data.arnov.dev/static/branding/topo-bright.png",
             show_default=False,
@@ -132,58 +169,65 @@
             'video_url',
         ]
     
     if missing:
         ttdb.console.print(message)
         typer.Exit(1)
     else:
-        for item, name in zip([bg, pic, video], names):
-            if (pitm := Path(item)).is_file():
-                variables[name] = pitm.name
-            elif 'www.youtube.com' in item:
-                ttdb.console.print(f"📦 Downloading youtube video in {youtube_quality}p quality", style='yellow')
-                yt = YouTube(item).streams.filter(progressive=True, file_extension='mp4').get_by_resolution(f"{youtube_quality}p")
-                if yt:
-                    yt.download(filename=f"{name}_youtube.mp4")
-                else:
-                    anyvid = YouTube(item).streams.filter(progressive=True, file_extension='mp4').order_by('resolution').desc().first()               
-                    anyvid.download(filename=f"{name}_youtube.mp4")
-                ttdb.upsert_param(name, f"{name}_youtube.mp4")
-                video = f"{name}_youtube.mp4"
-                variables['video_url'] = video
-        ttdb.console.print("✅[green] All variables set.[/green][yellow] Let's build ! 🚀[/yellow]")
-        cssTpl = jj.Template(cssTemplateFile.read_text()).render(variables)
-        htmlTpl = jj.Template(htmlTemplateFile.read_text()).render(variables)
-        base = out_path.parent
-        archive = out_path.stem
-        root = out_path.parent / out_path.stem if out_path.suffix else out_path
-        fmt = out_path.suffix.replace('.','') or 'zip'
-        root.mkdir(exist_ok=True)
-        (root / 'index.html').write_text(htmlTpl)
-        (root / 'style.css').write_text(cssTpl)
-        shutil.copyfile(Assets/'script.js', root / 'script.js')
-        for item in [bg, pic, video]:
-            if (pitm := Path(item)).is_file():
-                shutil.copyfile(pitm, root / pitm.name)
-        shutil.make_archive(base_dir=base,base_name=archive, root_dir=root, format=fmt)
-        ttdb.console.print(f"✅[green] Built archive at {root}")
-        if keep_archive_only:
-            shutil.rmtree(root)
-        for vid in Path().cwd().glob("*.mp4"):
-            vid.unlink()
+        if missing == -1:
+            ttdb.console.print(message)
+            build_ok = Confirm.ask("Do you still want to build anyway ?", default=False)
+        
+        else:
+            build_ok = True
+            
+        if build_ok:
+            variables = checkSourcesDownload(sources=zip([bg, pic, video], names), variables=variables, youtube_quality=youtube_quality)    
+            ttdb.console.print("✅[green] All variables set.[/green][yellow] Let's build ! 🚀[/yellow]")
+            cssTpl = jj.Template(cssTemplateFile.read_text()).render(variables)
+            htmlTpl = jj.Template(htmlTemplateFile.read_text()).render(variables)
+            base = out_path.parent
+            ttdb.upsert_param('build_path', out_path.parent)
+            archive = out_path.stem
+            root = out_path.parent / out_path.stem if out_path.suffix else out_path
+            fmt = out_path.suffix.replace('.','') or 'zip'
+            root.mkdir(exist_ok=True)
+            (root / 'index.html').write_text(htmlTpl)
+            (root / 'style.css').write_text(cssTpl)
+            shutil.copyfile(Assets/'script.js', root / 'script.js')
+            for item in [bg, pic, video]:
+                if (pitm := Path(item)).is_file():
+                    shutil.copyfile(pitm, root / pitm.name)
+            shutil.make_archive(base_dir=root,base_name=archive, root_dir=root, format=fmt)
+            ttdb.console.print(f"✅[green] Built archive at {root}")
+            if keep_archive_only:
+                shutil.rmtree(root)
+            for vid in Path().cwd().glob("*.mp4"):
+                vid.unlink()
+            
+            
+@app.command('clean', help="Removes existing files at the build location")
+def clean(
+    absolute_path: Path = typer.Option(None, '-a', '--abs-path')
+    ):
+    if absolute_path:
+        shutil.rmtree(absolute_path)
+    elif bpath := ttdb.getValue('build_path'):
+        shutil.rmtree(bpath)
 
 
 @app.command("serve", help="""Serves your site locally, if you built it. Else attempts to build first, then serve.""")
 def serve(
         out_path: Path = typer.Option(
             DEFAULT_BUILD_PATH,
             '-o', '--out-dir',
             help="Where to output the website files"
         ),
     ):
+    """Servers a Flask App of the server built on localhost:5000"""
     server = Flask(
         root_path=out_path,
         import_name=__name__,
         static_folder="")
     if not out_path.exists():
         build(**dict(zip(VARIABLES, DEFAULTS)), youtube_quality=1080, out_path=out_path)
```

