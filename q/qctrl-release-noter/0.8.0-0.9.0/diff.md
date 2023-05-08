# Comparing `tmp/qctrl_release_noter-0.8.0.tar.gz` & `tmp/qctrl_release_noter-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_release_noter-0.8.0.tar", max compression
+gzip compressed data, was "qctrl_release_noter-0.9.0.tar", max compression
```

## Comparing `qctrl_release_noter-0.8.0.tar` & `qctrl_release_noter-0.9.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    10141 2023-05-04 03:30:09.926798 qctrl_release_noter-0.8.0/LICENSE
--rw-r--r--   0        0        0      477 2023-05-04 03:30:09.926798 qctrl_release_noter-0.8.0/README.md
--rw-r--r--   0        0        0     2415 2023-05-04 03:30:28.163180 qctrl_release_noter-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      707 2023-05-04 03:30:28.167180 qctrl_release_noter-0.8.0/qctrlreleasenoter/__init__.py
--rw-r--r--   0        0        0     2405 2023-05-04 03:30:09.926798 qctrl_release_noter-0.8.0/qctrlreleasenoter/cli.py
--rw-r--r--   0        0        0    12707 2023-05-04 03:30:09.926798 qctrl_release_noter-0.8.0/qctrlreleasenoter/generate_release_notes.py
--rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 qctrl_release_noter-0.8.0/setup.py
--rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 qctrl_release_noter-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    10141 2023-05-08 05:05:24.788696 qctrl_release_noter-0.9.0/LICENSE
+-rw-r--r--   0        0        0      575 2023-05-08 05:05:24.788696 qctrl_release_noter-0.9.0/README.md
+-rw-r--r--   0        0        0     2415 2023-05-08 05:05:43.480800 qctrl_release_noter-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      707 2023-05-08 05:05:43.484800 qctrl_release_noter-0.9.0/qctrlreleasenoter/__init__.py
+-rw-r--r--   0        0        0     2796 2023-05-08 05:05:24.788696 qctrl_release_noter-0.9.0/qctrlreleasenoter/cli.py
+-rw-r--r--   0        0        0    12956 2023-05-08 05:05:24.788696 qctrl_release_noter-0.9.0/qctrlreleasenoter/generate_release_notes.py
+-rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 qctrl_release_noter-0.9.0/setup.py
+-rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 qctrl_release_noter-0.9.0/PKG-INFO
```

### Comparing `qctrl_release_noter-0.8.0/LICENSE` & `qctrl_release_noter-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_release_noter-0.8.0/pyproject.toml` & `qctrl_release_noter-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-release-noter"
-version = "0.8.0"
+version = "0.9.0"
 description = "Q-CTRL Release Noter"
 license = "Apache-2.0"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
```

### Comparing `qctrl_release_noter-0.8.0/qctrlreleasenoter/__init__.py` & `qctrl_release_noter-0.9.0/qctrlreleasenoter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 A Python package for generating the recommended release notes.
 """
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 __author__ = "Q-CTRL <support@q-ctrl.com>"
```

### Comparing `qctrl_release_noter-0.8.0/qctrlreleasenoter/cli.py` & `qctrl_release_noter-0.9.0/qctrlreleasenoter/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,20 +16,24 @@
 """
 import click
 from git import (
     InvalidGitRepositoryError,
     Repo,
 )
 
-from qctrlreleasenoter.generate_release_notes import generate_note
+from qctrlreleasenoter.generate_release_notes import (
+    generate_note,
+    pull_latest_changes,
+)
 
 
 @click.command(
     help="""
-    Prints release notes for the commits between the latest tag and `branch`.
+    Prints release notes for the commits between the latest tag and `branch`
+    for the specified repository.
 
     Commits are expected to follow the Conventional Commits specification
     (https://www.conventionalcommits.org/en/v1.0.0/). That is, messages are
     typically expected to be of the form:
 
         \b
         <kind>: <title>
@@ -57,29 +61,44 @@
     "--branch",
     default="master",
     help="Branch on which the release will be made (defaults to master).",
 )
 @click.option(
     "--ignore/--no-ignore",
     default=True,
-    help="Whether to ignore commits from robot@q-ctrl.com (defaults to True).",
+    help="Whether to ignore commits from robot@q-ctrl.com (defaults to --ignore).",
 )
 @click.option(
     "--github",
     is_flag=True,
     default=False,
     help="Open GitHub with the release notes prefilled.",
 )
 @click.option(
     "--phase",
     type=click.Choice(["stable", "alpha", "beta"]),
     default="stable",
     help="Select the phase for the release (defaults to stable).",
 )
-def main(branch, ignore, github, phase):
+@click.option(
+    "--pull/--no-pull",
+    default=True,
+    help="Pulls the latest changes from remote for the specified --branch (defaults to --pull).",
+)
+@click.argument(
+    "path",
+    default=".",
+    type=click.Path(exists=True),
+)
+def main(branch, ignore, github, path, phase, pull):
     """
     Main entry to generate the release note.
     """
     try:
-        generate_note(branch, ignore, github, phase, repo=Repo("."))
+        repo = Repo(path)
     except InvalidGitRepositoryError as err:
         raise RuntimeError("The current directory is not a valid repository.") from err
+
+    if pull:
+        pull_latest_changes(branch, repo)
+
+    generate_note(branch, ignore, github, phase, repo)
```

### Comparing `qctrl_release_noter-0.8.0/qctrlreleasenoter/generate_release_notes.py` & `qctrl_release_noter-0.9.0/qctrlreleasenoter/generate_release_notes.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,22 @@
             )
             self.unknowns.append(convert_to_past_tense(item.title))
         else:
             pr_type = getattr(self, item.kind.name.lower())
             pr_type.append(convert_to_past_tense(item.title))
 
 
+def pull_latest_changes(branch, repo):
+    """
+    Pulls the latest changes from remote for the specified `branch`.
+    """
+    repo.git.checkout(branch)
+    repo.remotes.origin.pull()
+
+
 def generate_note(branch, ignore, github, phase, repo):
     """
     Generate release notes for the commits between the latest tag and `branch`.
     """
 
     # Filter to tags that look like versions, and then find the most recent.
     tags = filter(lambda tag: isinstance(parse(tag.name), Version), repo.tags)
@@ -154,17 +162,19 @@
         return
 
     # Suggest a new version number based on the changes we found.
     # If this is the first release, starting from "0.0.0".
     version = Version("0.0.0") if latest_tag_name is None else parse(latest_tag_name)
     assert isinstance(version, Version)
     project_name = None
-
     # Attempts to fetch the name of the project from the README title.
-    readme_locations = [".github/README.md", "README.md"]
+    readme_locations = [
+        f"{repo.working_dir}/.github/README.md",
+        f"{repo.working_dir}/README.md",
+    ]
     for filepath in readme_locations:
         if Path(filepath).is_file():
             with open(filepath, "r", encoding="utf8") as file:
                 header = re.search(
                     "^(?: *)#(?: *)(.+)(?: *)$", file.read(), re.MULTILINE
                 )
             if header is not None:
```

### Comparing `qctrl_release_noter-0.8.0/setup.py` & `qctrl_release_noter-0.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'pyinflect>=0.5.1,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['release_noter = qctrlreleasenoter.cli:main']}
 
 setup_kwargs = {
     'name': 'qctrl-release-noter',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Q-CTRL Release Noter',
-    'long_description': '# Q-CTRL Release Noter\n\nThe Q-CTRL Release Noter Python package provides a command line tool that generates the\nrecommended release notes for a GitHub package from Q-CTRL.\n\n## Installation\n\nInstall the Q-CTRL Release Noter with:\n\n```shell\npip install qctrl-release-noter\n```\n\n## Usage\n\nIn the repository whose release notes you want to generate, run:\n\n```shell\nrelease_noter\n```\n\nTo prefill the information on the GitHub release page, use:\n\n```shell\nrelease_noter --github\n```\n',
+    'long_description': '# Q-CTRL Release Noter\n\nThe Q-CTRL Release Noter Python package provides a command line tool that generates the\nrecommended release notes for a GitHub package from Q-CTRL.\n\n## Installation\n\nInstall the Q-CTRL Release Noter with:\n\n```shell\npip install qctrl-release-noter\n```\n\n## Usage\n\nIn the repository whose release notes you want to generate, run:\n\n```shell\nrelease_noter\n```\n\nYou can also specify the path of the repository:\n\n```shell\nrelease_noter /path/to/repository\n```\n\nTo prefill the information on the GitHub release page, use:\n\n```shell\nrelease_noter --github\n```\n',
     'author': 'Q-CTRL',
     'author_email': 'support@q-ctrl.com',
     'maintainer': 'Q-CTRL',
     'maintainer_email': 'support@q-ctrl.com',
     'url': 'https://q-ctrl.com',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `qctrl_release_noter-0.8.0/PKG-INFO` & `qctrl_release_noter-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-release-noter
-Version: 0.8.0
+Version: 0.9.0
 Summary: Q-CTRL Release Noter
 Home-page: https://q-ctrl.com
 License: Apache-2.0
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -60,13 +60,19 @@
 
 In the repository whose release notes you want to generate, run:
 
 ```shell
 release_noter
 ```
 
+You can also specify the path of the repository:
+
+```shell
+release_noter /path/to/repository
+```
+
 To prefill the information on the GitHub release page, use:
 
 ```shell
 release_noter --github
 ```
```

