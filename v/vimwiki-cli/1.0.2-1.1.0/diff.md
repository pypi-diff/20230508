# Comparing `tmp/vimwiki-cli-1.0.2.tar.gz` & `tmp/vimwiki-cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vimwiki-cli-1.0.2.tar", last modified: Sun Sep  4 21:57:08 2022, max compression
+gzip compressed data, was "vimwiki-cli-1.1.0.tar", last modified: Mon May  8 17:51:39 2023, max compression
```

## Comparing `vimwiki-cli-1.0.2.tar` & `vimwiki-cli-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 21:57:08.160626 vimwiki-cli-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-09-04 21:56:53.000000 vimwiki-cli-1.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     3204 2022-09-04 21:56:53.000000 vimwiki-cli-1.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-09-04 21:56:53.000000 vimwiki-cli-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-09-04 21:56:53.000000 vimwiki-cli-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7230 2022-09-04 21:57:08.160626 vimwiki-cli-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6149 2022-09-04 21:56:53.000000 vimwiki-cli-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-04 21:56:53.000000 vimwiki-cli-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-09-04 21:57:08.160626 vimwiki-cli-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-09-04 21:56:53.000000 vimwiki-cli-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 21:57:08.160626 vimwiki-cli-1.0.2/vimwiki_cli/
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-09-04 21:56:53.000000 vimwiki-cli-1.0.2/vimwiki_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4561 2022-09-04 21:56:53.000000 vimwiki-cli-1.0.2/vimwiki_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-09-04 21:56:53.000000 vimwiki-cli-1.0.2/vimwiki_cli/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     2262 2022-09-04 21:56:53.000000 vimwiki-cli-1.0.2/vimwiki_cli/diary.py
--rw-r--r--   0 runner    (1001) docker     (121)     4476 2022-09-04 21:56:53.000000 vimwiki-cli-1.0.2/vimwiki_cli/editor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-09-04 21:56:53.000000 vimwiki-cli-1.0.2/vimwiki_cli/tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     4902 2022-09-04 21:56:53.000000 vimwiki-cli-1.0.2/vimwiki_cli/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 21:57:08.160626 vimwiki-cli-1.0.2/vimwiki_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7230 2022-09-04 21:57:08.000000 vimwiki-cli-1.0.2/vimwiki_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-09-04 21:57:08.000000 vimwiki-cli-1.0.2/vimwiki_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-04 21:57:08.000000 vimwiki-cli-1.0.2/vimwiki_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-04 21:57:08.000000 vimwiki-cli-1.0.2/vimwiki_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-09-04 21:57:08.000000 vimwiki-cli-1.0.2/vimwiki_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-04 21:57:08.000000 vimwiki-cli-1.0.2/vimwiki_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:51:39.643575 vimwiki-cli-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-05-08 17:51:39.643575 vimwiki-cli-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-08 17:51:39.643575 vimwiki-cli-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:51:39.643575 vimwiki-cli-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/tests/test_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/tests/test_wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:51:39.643575 vimwiki-cli-1.1.0/vimwiki_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/vimwiki_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/vimwiki_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/vimwiki_cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/vimwiki_cli/diary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/vimwiki_cli/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/vimwiki_cli/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-08 17:51:26.000000 vimwiki-cli-1.1.0/vimwiki_cli/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:51:39.643575 vimwiki-cli-1.1.0/vimwiki_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-05-08 17:51:39.000000 vimwiki-cli-1.1.0/vimwiki_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-08 17:51:39.000000 vimwiki-cli-1.1.0/vimwiki_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:51:39.000000 vimwiki-cli-1.1.0/vimwiki_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 17:51:39.000000 vimwiki-cli-1.1.0/vimwiki_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-08 17:51:39.000000 vimwiki-cli-1.1.0/vimwiki_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 17:51:39.000000 vimwiki-cli-1.1.0/vimwiki_cli.egg-info/top_level.txt
```

### Comparing `vimwiki-cli-1.0.2/CHANGELOG.md` & `vimwiki-cli-1.1.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v1.1.0] - 2023-05-08
+
+### Added
+
+- Add support for `VimwikiAll2HTML[!]` ([jfishe](https://github.com/jfishe))
+
+### Changed
+
+- Update documentation
+- Add `vimwiki.allhtml` to `scripts/pre-commit.sh`
+
 ## [v1.0.2] - 2022-09-04
 
 ### Changed
 
 - Fix PyPI documentation
 
 ## [v1.0.1] - 2022-09-04
@@ -28,11 +39,12 @@
 
 - Remove support for Python 3.6
 
 ## [v1.0.0] - 2021-05-04
 
 Initial release
 
-[Unreleased]: https://github.com/sstallion/vimwiki-cli/compare/v1.0.2...HEAD
+[Unreleased]: https://github.com/sstallion/vimwiki-cli/compare/v1.1.0...HEAD
+[v1.1.0]: https://github.com/sstallion/vimwiki-cli/releases/tag/v1.1.0
 [v1.0.2]: https://github.com/sstallion/vimwiki-cli/releases/tag/v1.0.2
 [v1.0.1]: https://github.com/sstallion/vimwiki-cli/releases/tag/v1.0.1
 [v1.0.0]: https://github.com/sstallion/vimwiki-cli/releases/tag/v1.0.0
```

### Comparing `vimwiki-cli-1.0.2/CONTRIBUTING.md` & `vimwiki-cli-1.1.0/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     $ python -m pycodestyle
     $ python -m pytest
 
 At a minimum, there should be no test regressions and additional tests should be
 added for new functionality. If user-facing changes are introduced, be sure add
 an entry to the `Unreleased` section in [CHANGELOG.md][3].
 
-With that out of the way, you may now commit your changes and create a
-[pull request][4] against the `master` branch for review!
+Finally, commit your changes and create a [pull request][4] against the `master`
+branch for review.
 
 ## Making New Releases
 
 Making new releases is automated by GitHub Actions. Releases should only be
 created from the `master` branch; as such `master` should be passing tests at
 all times.
```

### Comparing `vimwiki-cli-1.0.2/LICENSE` & `vimwiki-cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vimwiki-cli-1.0.2/PKG-INFO` & `vimwiki-cli-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vimwiki-cli
-Version: 1.0.2
+Version: 1.1.0
 Summary: Vimwiki Command-Line Interface
 Home-page: https://github.com/sstallion/vimwiki-cli
 Author: Steven Stallion
 Author-email: sstallion@gmail.com
 License: BSD-2-Clause
 Keywords: cli vim vimwiki wiki
 Classifier: Development Status :: 5 - Production/Stable
@@ -70,14 +70,15 @@
 
 Each CLI command corresponds to one or more Ex commands executed in the editor.
 The following table details the mapping between these commands:
 
 | CLI Command                             | Ex Commands                                                         |
 |-----------------------------------------|---------------------------------------------------------------------|
 | `vimwiki`                               | `:VimwikiIndex`                                                     |
+| `vimwiki all-html`                      | `:VimwikiIndex \| VimwikiAll2HTML`                                  |
 | `vimwiki check-links`                   | `:VimwikiIndex \| VimwikiCheckLinks`                                |
 | `vimwiki diary`                         | `:VimwikiDiaryIndex`                                                |
 | `vimwiki diary generate-links`          | `:VimwikiDiaryIndex \| VimwikiDiaryGenerateLinks`                   |
 | `vimwiki diary today`                   | `:VimwikiMakeDiaryNote`                                             |
 | `vimwiki diary tomorrow`                | `:VimwikiMakeTomorrowDiaryNote`                                     |
 | `vimwiki diary yesterday`               | `:VimwikiMakeYesterdayDiaryNote`                                    |
 | `vimwiki generate-links PAGE PATTERN`   | `:VimwikiIndex \| VimwikiGoto PAGE \| VimwikiGenerateLinks PATTERN` |
@@ -113,14 +114,15 @@
 | `vimwiki.options`            | Extra options to pass to the `vimwiki` command |
 | `vimwiki.linkspage`          | Page which contains generated links            |
 | `vimwiki.taglinkspage`       | Page which contains generated tag links        |
 | `vimwiki.generatelinks`      | Generate links before commit (bool)            |
 | `vimwiki.generatediarylinks` | Generate diary links before commit (bool)      |
 | `vimwiki.generatetaglinks`   | Generate tag links before commit (bool)        |
 | `vimwiki.rebuildtags`        | Rebuild tag metadata before commit (bool)      |
+| `vimwiki.allhtml`            | Convert wiki to HTML before commit (bool)      |
 
 For example, to configure the hook to rebuild tag metadata and generate tag
 links in the `Tags` page before commit, issue:
 
     $ git config vimwiki.taglinkspage Tags
     $ git config vimwiki.generatetaglinks true
     $ git config vimwiki.rebuildtags true
```

### Comparing `vimwiki-cli-1.0.2/README.md` & `vimwiki-cli-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 Each CLI command corresponds to one or more Ex commands executed in the editor.
 The following table details the mapping between these commands:
 
 | CLI Command                             | Ex Commands                                                         |
 |-----------------------------------------|---------------------------------------------------------------------|
 | `vimwiki`                               | `:VimwikiIndex`                                                     |
+| `vimwiki all-html`                      | `:VimwikiIndex \| VimwikiAll2HTML`                                  |
 | `vimwiki check-links`                   | `:VimwikiIndex \| VimwikiCheckLinks`                                |
 | `vimwiki diary`                         | `:VimwikiDiaryIndex`                                                |
 | `vimwiki diary generate-links`          | `:VimwikiDiaryIndex \| VimwikiDiaryGenerateLinks`                   |
 | `vimwiki diary today`                   | `:VimwikiMakeDiaryNote`                                             |
 | `vimwiki diary tomorrow`                | `:VimwikiMakeTomorrowDiaryNote`                                     |
 | `vimwiki diary yesterday`               | `:VimwikiMakeYesterdayDiaryNote`                                    |
 | `vimwiki generate-links PAGE PATTERN`   | `:VimwikiIndex \| VimwikiGoto PAGE \| VimwikiGenerateLinks PATTERN` |
@@ -84,14 +85,15 @@
 | `vimwiki.options`            | Extra options to pass to the `vimwiki` command |
 | `vimwiki.linkspage`          | Page which contains generated links            |
 | `vimwiki.taglinkspage`       | Page which contains generated tag links        |
 | `vimwiki.generatelinks`      | Generate links before commit (bool)            |
 | `vimwiki.generatediarylinks` | Generate diary links before commit (bool)      |
 | `vimwiki.generatetaglinks`   | Generate tag links before commit (bool)        |
 | `vimwiki.rebuildtags`        | Rebuild tag metadata before commit (bool)      |
+| `vimwiki.allhtml`            | Convert wiki to HTML before commit (bool)      |
 
 For example, to configure the hook to rebuild tag metadata and generate tag
 links in the `Tags` page before commit, issue:
 
     $ git config vimwiki.taglinkspage Tags
     $ git config vimwiki.generatetaglinks true
     $ git config vimwiki.rebuildtags true
```

### Comparing `vimwiki-cli-1.0.2/setup.cfg` & `vimwiki-cli-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.2
+current_version = 1.1.0
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
 
 [bumpversion:file:vimwiki_cli/__init__.py]
 search = __version__ = '{current_version}'
```

### Comparing `vimwiki-cli-1.0.2/setup.py` & `vimwiki-cli-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 dirname = os.path.dirname(os.path.abspath(__file__))
 with open(os.path.join(dirname, 'README.md')) as f:
     long_description = f.read()
 
 setup(name='vimwiki-cli',
-      version='1.0.2',
+      version='1.1.0',
       description='Vimwiki Command-Line Interface',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Steven Stallion',
       author_email='sstallion@gmail.com',
       url='https://github.com/sstallion/vimwiki-cli',
       packages=find_packages(),
```

### Comparing `vimwiki-cli-1.0.2/vimwiki_cli/__init__.py` & `vimwiki-cli-1.1.0/vimwiki_cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
 # OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 # HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
 # OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
 # SUCH DAMAGE.
 
-__version__ = '1.0.2'
+__version__ = '1.1.0'
```

### Comparing `vimwiki-cli-1.0.2/vimwiki_cli/__main__.py` & `vimwiki-cli-1.1.0/vimwiki_cli/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from .diary import diary
 from .tags import tags
 
 logger = logging.getLogger(__name__)
 
 
 @click.group(context_settings=CONTEXT_SETTINGS, invoke_without_command=True,
-             epilog='Please report issues to https://github.com/sstallion/vimwiki-cli/issues.')
+             epilog='Report issues to https://github.com/sstallion/vimwiki-cli/issues.')
 @click.option('--editor',
               help='Editor to launch, defaults to $EDITOR or vim.')
 @click.option('--count', type=int,
               help='Index of wiki to open.')
 @click.option('--select', is_flag=True,
               help='Select wiki from interactive list.')
 @click.option('--open-matches', is_flag=True,
@@ -78,14 +78,23 @@
 
     make_wiki(ctx, *args, **kwargs)
     if ctx.invoked_subcommand is None:
         ctx.invoke(index)
 
 
 @cli.command()
+@click.option('--all', is_flag=True,
+              help='Rebuild all files, not just those that are newer.')
+@pass_wiki
+def all_html(wiki, all):
+    """Convert all wiki pages to HTML."""
+    wiki.all_html(all)
+
+
+@cli.command()
 @pass_wiki
 def check_links(wiki):
     """Search files and check reachability of links."""
     wiki.check_links()
 
 
 @cli.command()
```

### Comparing `vimwiki-cli-1.0.2/vimwiki_cli/context.py` & `vimwiki-cli-1.1.0/vimwiki_cli/context.py`

 * *Files identical despite different names*

### Comparing `vimwiki-cli-1.0.2/vimwiki_cli/diary.py` & `vimwiki-cli-1.1.0/vimwiki_cli/diary.py`

 * *Files identical despite different names*

### Comparing `vimwiki-cli-1.0.2/vimwiki_cli/editor.py` & `vimwiki-cli-1.1.0/vimwiki_cli/editor.py`

 * *Files identical despite different names*

### Comparing `vimwiki-cli-1.0.2/vimwiki_cli/tags.py` & `vimwiki-cli-1.1.0/vimwiki_cli/tags.py`

 * *Files identical despite different names*

### Comparing `vimwiki-cli-1.0.2/vimwiki_cli/wiki.py` & `vimwiki-cli-1.1.0/vimwiki_cli/wiki.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,19 @@
                      interactive=False, write_quit=True).run()
 
     def diary_generate_links(self):
         """Create or update an overview of diary pages."""
         DiaryCommand(self, 'VimwikiDiaryGenerateLinks',
                      interactive=False, write_quit=True).run()
 
+    def all_html(self, all=False):
+        """Convert all wiki pages to HTML."""
+        LocalCommand(self, 'silent! VimwikiAll2HTML' + ('!' if all else ''),
+                     interactive=False, quit=True).run()
+
     def check_links(self):
         """Search files and check reachability of links."""
         LocalCommand(self, 'VimwikiCheckLinks').run()
 
     def rebuild_tags(self, all=False):
         """Rebuild tag metadata."""
         LocalCommand(self, 'VimwikiRebuildTags' + ('!' if all else ''),
```

### Comparing `vimwiki-cli-1.0.2/vimwiki_cli.egg-info/PKG-INFO` & `vimwiki-cli-1.1.0/vimwiki_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vimwiki-cli
-Version: 1.0.2
+Version: 1.1.0
 Summary: Vimwiki Command-Line Interface
 Home-page: https://github.com/sstallion/vimwiki-cli
 Author: Steven Stallion
 Author-email: sstallion@gmail.com
 License: BSD-2-Clause
 Keywords: cli vim vimwiki wiki
 Classifier: Development Status :: 5 - Production/Stable
@@ -70,14 +70,15 @@
 
 Each CLI command corresponds to one or more Ex commands executed in the editor.
 The following table details the mapping between these commands:
 
 | CLI Command                             | Ex Commands                                                         |
 |-----------------------------------------|---------------------------------------------------------------------|
 | `vimwiki`                               | `:VimwikiIndex`                                                     |
+| `vimwiki all-html`                      | `:VimwikiIndex \| VimwikiAll2HTML`                                  |
 | `vimwiki check-links`                   | `:VimwikiIndex \| VimwikiCheckLinks`                                |
 | `vimwiki diary`                         | `:VimwikiDiaryIndex`                                                |
 | `vimwiki diary generate-links`          | `:VimwikiDiaryIndex \| VimwikiDiaryGenerateLinks`                   |
 | `vimwiki diary today`                   | `:VimwikiMakeDiaryNote`                                             |
 | `vimwiki diary tomorrow`                | `:VimwikiMakeTomorrowDiaryNote`                                     |
 | `vimwiki diary yesterday`               | `:VimwikiMakeYesterdayDiaryNote`                                    |
 | `vimwiki generate-links PAGE PATTERN`   | `:VimwikiIndex \| VimwikiGoto PAGE \| VimwikiGenerateLinks PATTERN` |
@@ -113,14 +114,15 @@
 | `vimwiki.options`            | Extra options to pass to the `vimwiki` command |
 | `vimwiki.linkspage`          | Page which contains generated links            |
 | `vimwiki.taglinkspage`       | Page which contains generated tag links        |
 | `vimwiki.generatelinks`      | Generate links before commit (bool)            |
 | `vimwiki.generatediarylinks` | Generate diary links before commit (bool)      |
 | `vimwiki.generatetaglinks`   | Generate tag links before commit (bool)        |
 | `vimwiki.rebuildtags`        | Rebuild tag metadata before commit (bool)      |
+| `vimwiki.allhtml`            | Convert wiki to HTML before commit (bool)      |
 
 For example, to configure the hook to rebuild tag metadata and generate tag
 links in the `Tags` page before commit, issue:
 
     $ git config vimwiki.taglinkspage Tags
     $ git config vimwiki.generatetaglinks true
     $ git config vimwiki.rebuildtags true
```

