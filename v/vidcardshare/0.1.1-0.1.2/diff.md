# Comparing `tmp/vidcardshare-0.1.1.tar.gz` & `tmp/vidcardshare-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidcardshare-0.1.1.tar", max compression
+gzip compressed data, was "vidcardshare-0.1.2.tar", max compression
```

## Comparing `vidcardshare-0.1.1.tar` & `vidcardshare-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       60 2023-05-07 23:44:32.772934 vidcardshare-0.1.1/README.md
--rwxr-xr-x   0        0        0     3941 2023-05-07 21:37:59.860401 vidcardshare-0.1.1/assets/index.html.tpl
--rwxr-xr-x   0        0        0      759 2023-05-07 20:43:56.000000 vidcardshare-0.1.1/assets/script.js
--rwxr-xr-x   0        0        0     6496 2023-05-07 21:31:56.704323 vidcardshare-0.1.1/assets/style.css.tpl
--rw-r--r--   0        0        0      521 2023-05-08 00:04:42.380973 vidcardshare-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-07 21:15:03.156150 vidcardshare-0.1.1/vidcardshare/__init__.py
--rw-r--r--   0        0        0     6648 2023-05-07 23:41:17.416926 vidcardshare-0.1.1/vidcardshare/main.py
--rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 vidcardshare-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-05-07 23:44:32.772934 vidcardshare-0.1.2/README.md
+-rwxr-xr-x   0        0        0     3941 2023-05-07 21:37:59.860401 vidcardshare-0.1.2/assets/index.html.tpl
+-rwxr-xr-x   0        0        0      759 2023-05-07 20:43:56.000000 vidcardshare-0.1.2/assets/script.js
+-rwxr-xr-x   0        0        0     6496 2023-05-07 21:31:56.704323 vidcardshare-0.1.2/assets/style.css.tpl
+-rw-r--r--   0        0        0      538 2023-05-08 01:00:15.052631 vidcardshare-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-07 21:15:03.156150 vidcardshare-0.1.2/vidcardshare/__init__.py
+-rw-r--r--   0        0        0     7968 2023-05-08 01:00:02.256634 vidcardshare-0.1.2/vidcardshare/main.py
+-rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 vidcardshare-0.1.2/PKG-INFO
```

### Comparing `vidcardshare-0.1.1/assets/index.html.tpl` & `vidcardshare-0.1.2/assets/index.html.tpl`

 * *Files identical despite different names*

### Comparing `vidcardshare-0.1.1/assets/script.js` & `vidcardshare-0.1.2/assets/script.js`

 * *Files identical despite different names*

### Comparing `vidcardshare-0.1.1/assets/style.css.tpl` & `vidcardshare-0.1.2/assets/style.css.tpl`

 * *Files identical despite different names*

### Comparing `vidcardshare-0.1.1/pyproject.toml` & `vidcardshare-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "vidcardshare"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Arno V <bcda0276@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/arnos-stuff/vidcardshare.git"
 include = [
     {'path' = 'assets/*'}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer-tinydb = "^0.1.4"
 jinja2 = "^3.1.2"
 pytube = "^15.0.0"
+flask = "^2.3.2"
 
 [tool.poetry.scripts]
 vidcardshare = "vidcardshare.main:app"
 vidcsh = "vidcardshare.main:app"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `vidcardshare-0.1.1/vidcardshare/main.py` & `vidcardshare-0.1.2/vidcardshare/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typer
 import jinja2 as jj
 import typer_tinydb as ttdb
 import shutil
 
 from pathlib import Path
+from flask import send_from_directory, Flask, make_response, render_template
 from pytube import YouTube
 
 Pkg = Path(__file__).parent
 Root = Pkg.parent
 Assets = Root / 'assets'
 cssTemplateFile = Assets / 'style.css.tpl'
 htmlTemplateFile = Assets / 'index.html.tpl'
@@ -36,14 +37,17 @@
     "https://i.imgur.com/ThKEz2i.png",
     "https://imgur.com/uKXnoi0",
     "https://www.youtube.com/embed/dQw4w9WgXcQ",
     '#',
     '#'
 ]
 
+DEFAULT_BUILD_DIR = Path().home() / '.vidcardshare'
+DEFAULT_BUILD_PATH = DEFAULT_BUILD_DIR / 'video-website'
+DEFAULT_BUILD_PATH.mkdir(parents=True, exist_ok=True)
 
 def attemptGetVarsDB(*vars, **kwargs):
     """Checks the variables have been declared"""
     return {
         var : ttdb.getValue(var) for var in vars
     } | kwargs
     
@@ -96,25 +100,30 @@
         twitter_handle: str = typer.Option(
             '#',
             '-tw', '--twitter-handle',
             show_default=False,
             help="Just your twitter handle, without the @ (ex: @joe => joe)"
         ),
         out_path: Path = typer.Option(
-            "./video-website.zip",
+            DEFAULT_BUILD_PATH,
             '-o', '--out-dir',
             help="Where to output the zipped website"
         ),
         youtube_quality: int = typer.Option(
             1080,
             '-yq', '--youtube-quality',
             help="If your link is a youtube link, what quality to download it in."
-        )
+        ),
+        keep_archive_only: bool = typer.Option(
+            False,
+            '-k', '--keep-archive-only', help="Whether to remove everything but the archive after build."
+        )            
     ):
-    variables = attemptGetVarsDB(*VARIABLES, video_url=video_url, github_repo=github_repo, twitter_handle=twitter_handle)
+
+    variables = attemptGetVarsDB(*VARIABLES, background_image_url=background_image_url, profile_picture_url=profile_picture_url, video_url=video_url, github_repo=github_repo, twitter_handle=twitter_handle)
     missing, message = promptVarsMissing(**variables)
     
     video = variables['video_url']
     pic = variables['profile_picture_url']
     bg = variables['background_image_url']
     
     names = [
@@ -142,20 +151,43 @@
                 video = f"{name}_youtube.mp4"
                 variables['video_url'] = video
         ttdb.console.print("✅[green] All variables set.[/green][yellow] Let's build ! 🚀[/yellow]")
         cssTpl = jj.Template(cssTemplateFile.read_text()).render(variables)
         htmlTpl = jj.Template(htmlTemplateFile.read_text()).render(variables)
         base = out_path.parent
         archive = out_path.stem
-        root = out_path.parent / out_path.stem
+        root = out_path.parent / out_path.stem if out_path.suffix else out_path
+        fmt = out_path.suffix.replace('.','') or 'zip'
         root.mkdir(exist_ok=True)
         (root / 'index.html').write_text(htmlTpl)
         (root / 'style.css').write_text(cssTpl)
         shutil.copyfile(Assets/'script.js', root / 'script.js')
         for item in [bg, pic, video]:
             if (pitm := Path(item)).is_file():
                 shutil.copyfile(pitm, root / pitm.name)
-        shutil.make_archive(base_dir=base,base_name=archive, root_dir=root, format=out_path.suffix.replace('.',''))
+        shutil.make_archive(base_dir=base,base_name=archive, root_dir=root, format=fmt)
         ttdb.console.print(f"✅[green] Built archive at {root}")
-        shutil.rmtree(root)
+        if keep_archive_only:
+            shutil.rmtree(root)
         for vid in Path().cwd().glob("*.mp4"):
             vid.unlink()
+
+
+@app.command("serve", help="""Serves your site locally, if you built it. Else attempts to build first, then serve.""")
+def serve(
+        out_path: Path = typer.Option(
+            DEFAULT_BUILD_PATH,
+            '-o', '--out-dir',
+            help="Where to output the website files"
+        ),
+    ):
+    server = Flask(
+        root_path=out_path,
+        import_name=__name__,
+        static_folder="")
+    if not out_path.exists():
+        build(**dict(zip(VARIABLES, DEFAULTS)), youtube_quality=1080, out_path=out_path)
+    
+    @server.route('/<path:path>')
+    def send_report(path):
+        return send_from_directory(out_path, 'index.html')
+    server.run(host='localhost', port=5000, debug=True)
```

### Comparing `vidcardshare-0.1.1/PKG-INFO` & `vidcardshare-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: vidcardshare
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Home-page: https://github.com/arnos-stuff/vidcardshare.git
 Author: Arno V
 Author-email: bcda0276@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pytube (>=15.0.0,<16.0.0)
 Requires-Dist: typer-tinydb (>=0.1.4,<0.2.0)
 Description-Content-Type: text/markdown
 
 # Make mini video-sharing card-like websites
```

