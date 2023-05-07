# Comparing `tmp/git-nautilus-icons-2.0.3.tar.gz` & `tmp/git-nautilus-icons-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-nautilus-icons-2.0.3.tar", last modified: Tue Apr  5 09:17:25 2022, max compression
+gzip compressed data, was "git-nautilus-icons-2.1.0.tar", last modified: Sun May  7 23:30:33 2023, max compression
```

## Comparing `git-nautilus-icons-2.0.3.tar` & `git-nautilus-icons-2.1.0.tar`

### file list

```diff
@@ -1,638 +1,638 @@
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.091052 git-nautilus-icons-2.0.3/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)       33 2020-05-26 17:10:28.000000 git-nautilus-icons-2.0.3/.gitignore
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     1299 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/LICENSE
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      322 2022-04-05 09:17:25.091052 git-nautilus-icons-2.0.3/PKG-INFO
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     6705 2022-04-05 02:42:00.000000 git-nautilus-icons-2.0.3/README.md
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.041052 git-nautilus-icons-2.0.3/distro_icons/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     1908 2020-05-26 16:55:34.000000 git-nautilus-icons-2.0.3/distro_icons/arch.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     1971 2020-05-26 16:55:35.000000 git-nautilus-icons-2.0.3/distro_icons/debian.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2689 2020-05-26 16:55:36.000000 git-nautilus-icons-2.0.3/distro_icons/linux.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      310 2020-05-26 16:55:37.000000 git-nautilus-icons-2.0.3/distro_icons/manjaro.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      937 2020-05-26 16:55:38.000000 git-nautilus-icons-2.0.3/distro_icons/mint.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9892 2020-05-26 16:55:38.000000 git-nautilus-icons-2.0.3/distro_icons/pop.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     1179 2020-05-26 16:55:39.000000 git-nautilus-icons-2.0.3/distro_icons/ubuntu.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    33705 2021-03-13 23:11:58.000000 git-nautilus-icons-2.0.3/git-nautilus-icons.py
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.041052 git-nautilus-icons-2.0.3/git_nautilus_icons.egg-info/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      322 2022-04-05 09:17:24.000000 git-nautilus-icons-2.0.3/git_nautilus_icons.egg-info/PKG-INFO
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    34150 2022-04-05 09:17:24.000000 git-nautilus-icons-2.0.3/git_nautilus_icons.egg-info/SOURCES.txt
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        1 2022-04-05 09:17:24.000000 git-nautilus-icons-2.0.3/git_nautilus_icons.egg-info/dependency_links.txt
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        1 2022-04-05 09:17:24.000000 git-nautilus-icons-2.0.3/git_nautilus_icons.egg-info/top_level.txt
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.044385 git-nautilus-icons-2.0.3/icon_testing_dir/
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.044385 git-nautilus-icons-2.0.3/icon_testing_dir/01 clean repo/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/01 clean repo/.dummy_file
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.044385 git-nautilus-icons-2.0.3/icon_testing_dir/02 clean repo ahead of remote/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/02 clean repo ahead of remote/.dummy_file
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/03 ignored
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/04 clean
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/05 untracked
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/06 unstaged changes
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.044385 git-nautilus-icons-2.0.3/icon_testing_dir/07 unstaged deletion/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/07 unstaged deletion/.dummy_file
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/08 staged changes
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/09 staged rename
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/10 staged new file
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.044385 git-nautilus-icons-2.0.3/icon_testing_dir/11 staged deletion/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/11 staged deletion/.dummy_file
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/12 staged deletion, restored in work tree
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/13 staged and unstaged changes
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/14 staged rename, unstaged changes
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/15 staged new file, unstaged changes
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.044385 git-nautilus-icons-2.0.3/icon_testing_dir/16 staged changes, unstaged deletion/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/16 staged changes, unstaged deletion/.dummy_file
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.044385 git-nautilus-icons-2.0.3/icon_testing_dir/17 staged rename, unstaged deletion/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/17 staged rename, unstaged deletion/.dummy_file
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.044385 git-nautilus-icons-2.0.3/icon_testing_dir/18 staged new file, unstaged deletion/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/18 staged new file, unstaged deletion/.dummy_file
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/19 unmerged, both added
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/20 unmerged, both modified
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.044385 git-nautilus-icons-2.0.3/icon_testing_dir/21 unmerged, changed by them, deleted by us/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/21 unmerged, changed by them, deleted by us/.dummy_file
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/22 unmerged, changed by us, deleted by them
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.044385 git-nautilus-icons-2.0.3/icon_testing_dir/23 repo with clean index and untracked files/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/23 repo with clean index and untracked files/.dummy_file
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.044385 git-nautilus-icons-2.0.3/icon_testing_dir/24 repo with staged and unstaged deletions/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icon_testing_dir/24 repo with staged and unstaged deletions/.dummy_file
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.044385 git-nautilus-icons-2.0.3/icons/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5940 2020-05-23 23:56:34.000000 git-nautilus-icons-2.0.3/icons/generate_icons.py
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.037719 git-nautilus-icons-2.0.3/icons/hicolor/
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.037719 git-nautilus-icons-2.0.3/icons/hicolor/12x12/
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.051052 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4642 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-dotgit.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-untracked.svg
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.037719 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.054386 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4642 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-dotgit.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-untracked.svg
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.037719 git-nautilus-icons-2.0.3/icons/hicolor/16x16/
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.061052 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4644 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-dotgit.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-untracked.svg
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.037719 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.067719 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4644 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-dotgit.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-untracked.svg
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.037719 git-nautilus-icons-2.0.3/icons/hicolor/8x8/
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.074386 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-added-clean.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-added-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-added-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-added-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-added-clean.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-added-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-added-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-added-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-clean-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-clean.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-deleted-clean.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-deleted-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-deleted-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-deleted-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-modified-clean.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-modified-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-modified-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-modified-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-renamed-clean.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-renamed-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-renamed-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-renamed-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-unmerged-added-unmerged-added.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-clean-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-clean.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-deleted-clean.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-deleted-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-deleted-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-deleted-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2010 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-dotgit.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-modified-clean.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-modified-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-modified-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-modified-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-renamed-clean.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-renamed-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-renamed-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-renamed-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-added-clean.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-added-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-added-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-added-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-clean-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-clean.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-deleted-clean.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-deleted-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-deleted-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-deleted-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-modified-clean.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-modified-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-modified-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-modified-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-renamed-clean.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-renamed-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-renamed-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-renamed-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-unmerged-added-unmerged-added.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-unmerged-deleted-unmerged-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-unmerged-modified-unmerged-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-unmerged-modified-unmerged-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-unmerged-added-unmerged-added.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-unmerged-deleted-unmerged-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-unmerged-modified-unmerged-deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-unmerged-modified-unmerged-modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-untracked.png
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.037719 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.081052 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4642 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-dotgit.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-untracked.svg
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.037719 git-nautilus-icons-2.0.3/icons/hicolor/scalable/
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.087719 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4977 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     6012 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5050 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5617 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11238 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12273 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11311 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11878 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12374 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9086 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11068 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12103 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11141 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11708 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    10121 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11851 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12886 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11924 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12491 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9159 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    13988 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    15023 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    14061 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    14628 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    18823 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    18139 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    18135 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    18309 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9726 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     6113 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2825 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4807 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5842 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4880 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5447 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3860 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4600 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-dotgit.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5590 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     6625 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5663 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     6230 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2898 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     7727 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     8762 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     7800 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     8367 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-added-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    10235 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-added-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9273 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-added-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9840 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-added-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    10336 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-clean-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     7048 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9030 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-deleted-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    10065 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-deleted-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9103 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-deleted-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9670 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-deleted-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     8083 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9813 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-modified-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    10848 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-modified-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9886 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-modified-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    10453 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-modified-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     7121 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11950 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-renamed-clean.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12985 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-renamed-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12023 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-renamed-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12590 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-renamed-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    16785 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    16101 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    16097 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    16271 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     7688 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-untracked.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12562 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-unmerged-added-unmerged-added.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11878 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-unmerged-deleted-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11874 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-unmerged-modified-unmerged-deleted.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12048 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-unmerged-modified-unmerged-modified.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3465 2020-05-23 23:55:25.000000 git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-untracked.svg
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.087719 git-nautilus-icons-2.0.3/icons/sub_icons/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2652 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/added-l.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2452 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/ahead.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3296 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/clean-l.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3264 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/clean-r.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2491 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/deleted-l.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4057 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/deleted-r.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5027 2020-05-23 23:54:43.000000 git-nautilus-icons-2.0.3/icons/sub_icons/dotgit-r.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3486 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/modified-l.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3379 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/modified-r.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5400 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/renamed-l.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5062 2020-05-23 23:55:13.000000 git-nautilus-icons-2.0.3/icons/sub_icons/repo.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     6956 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/unmerged-added-l.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5950 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/unmerged-added-r.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     6634 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/unmerged-deleted-l.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5624 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/unmerged-deleted-r.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     6894 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/unmerged-modified-l.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5888 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/unmerged-modified-r.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4651 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/unmerged-simple.svg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3973 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/sub_icons/untracked-r.svg
-drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2022-04-05 09:17:25.091052 git-nautilus-icons-2.0.3/icons/tiny_icons/
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/tiny_icons/clean.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/tiny_icons/deleted.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2010 2020-05-23 22:58:16.000000 git-nautilus-icons-2.0.3/icons/tiny_icons/dotgit.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/tiny_icons/modified.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/tiny_icons/unmerged.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/icons/tiny_icons/untracked.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    73067 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/key.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      107 2020-05-26 17:04:28.000000 git-nautilus-icons-2.0.3/pyproject.toml
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    72597 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/screenshot_caja.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    43233 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/screenshot_nautilus.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    99171 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/screenshot_nemo.png
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)       38 2022-04-05 09:17:25.091052 git-nautilus-icons-2.0.3/setup.cfg
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)      840 2022-04-05 02:42:00.000000 git-nautilus-icons-2.0.3/setup.py
--rw-r--r--   0 bilbo     (1000) bilbo     (1000)    33935 2019-11-27 03:51:24.000000 git-nautilus-icons-2.0.3/small_icons.png
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:33.026836 git-nautilus-icons-2.1.0/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)       33 2020-05-26 17:10:28.000000 git-nautilus-icons-2.1.0/.gitignore
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     1299 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/LICENSE
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      294 2023-05-07 23:30:33.026836 git-nautilus-icons-2.1.0/PKG-INFO
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     6705 2022-04-05 02:42:00.000000 git-nautilus-icons-2.1.0/README.md
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.963503 git-nautilus-icons-2.1.0/distro_icons/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     1908 2020-05-26 16:55:34.000000 git-nautilus-icons-2.1.0/distro_icons/arch.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     1971 2020-05-26 16:55:35.000000 git-nautilus-icons-2.1.0/distro_icons/debian.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2689 2020-05-26 16:55:36.000000 git-nautilus-icons-2.1.0/distro_icons/linux.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      310 2020-05-26 16:55:37.000000 git-nautilus-icons-2.1.0/distro_icons/manjaro.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      937 2020-05-26 16:55:38.000000 git-nautilus-icons-2.1.0/distro_icons/mint.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9892 2020-05-26 16:55:38.000000 git-nautilus-icons-2.1.0/distro_icons/pop.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     1179 2020-05-26 16:55:39.000000 git-nautilus-icons-2.1.0/distro_icons/ubuntu.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    33799 2023-05-07 23:30:10.000000 git-nautilus-icons-2.1.0/git-nautilus-icons.py
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.963503 git-nautilus-icons-2.1.0/git_nautilus_icons.egg-info/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      294 2023-05-07 23:30:32.000000 git-nautilus-icons-2.1.0/git_nautilus_icons.egg-info/PKG-INFO
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    34150 2023-05-07 23:30:32.000000 git-nautilus-icons-2.1.0/git_nautilus_icons.egg-info/SOURCES.txt
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        1 2023-05-07 23:30:32.000000 git-nautilus-icons-2.1.0/git_nautilus_icons.egg-info/dependency_links.txt
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        1 2023-05-07 23:30:32.000000 git-nautilus-icons-2.1.0/git_nautilus_icons.egg-info/top_level.txt
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.966836 git-nautilus-icons-2.1.0/icon_testing_dir/
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.966836 git-nautilus-icons-2.1.0/icon_testing_dir/01 clean repo/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/01 clean repo/.dummy_file
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.966836 git-nautilus-icons-2.1.0/icon_testing_dir/02 clean repo ahead of remote/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/02 clean repo ahead of remote/.dummy_file
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/03 ignored
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/04 clean
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/05 untracked
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/06 unstaged changes
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.966836 git-nautilus-icons-2.1.0/icon_testing_dir/07 unstaged deletion/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/07 unstaged deletion/.dummy_file
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/08 staged changes
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/09 staged rename
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/10 staged new file
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.966836 git-nautilus-icons-2.1.0/icon_testing_dir/11 staged deletion/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/11 staged deletion/.dummy_file
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/12 staged deletion, restored in work tree
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/13 staged and unstaged changes
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/14 staged rename, unstaged changes
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/15 staged new file, unstaged changes
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.966836 git-nautilus-icons-2.1.0/icon_testing_dir/16 staged changes, unstaged deletion/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/16 staged changes, unstaged deletion/.dummy_file
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.966836 git-nautilus-icons-2.1.0/icon_testing_dir/17 staged rename, unstaged deletion/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/17 staged rename, unstaged deletion/.dummy_file
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.966836 git-nautilus-icons-2.1.0/icon_testing_dir/18 staged new file, unstaged deletion/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/18 staged new file, unstaged deletion/.dummy_file
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/19 unmerged, both added
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/20 unmerged, both modified
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.966836 git-nautilus-icons-2.1.0/icon_testing_dir/21 unmerged, changed by them, deleted by us/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/21 unmerged, changed by them, deleted by us/.dummy_file
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/22 unmerged, changed by us, deleted by them
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.966836 git-nautilus-icons-2.1.0/icon_testing_dir/23 repo with clean index and untracked files/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/23 repo with clean index and untracked files/.dummy_file
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.966836 git-nautilus-icons-2.1.0/icon_testing_dir/24 repo with staged and unstaged deletions/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)        0 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icon_testing_dir/24 repo with staged and unstaged deletions/.dummy_file
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.966836 git-nautilus-icons-2.1.0/icons/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5940 2020-05-23 23:56:34.000000 git-nautilus-icons-2.1.0/icons/generate_icons.py
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.963503 git-nautilus-icons-2.1.0/icons/hicolor/
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.960169 git-nautilus-icons-2.1.0/icons/hicolor/12x12/
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.973502 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4642 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-dotgit.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-untracked.svg
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.960169 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.980169 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4642 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-dotgit.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-untracked.svg
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.960169 git-nautilus-icons-2.1.0/icons/hicolor/16x16/
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.990169 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4644 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-dotgit.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-untracked.svg
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.960169 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.996836 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4644 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-dotgit.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2869 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3904 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2942 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4218 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3509 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-untracked.svg
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.963503 git-nautilus-icons-2.1.0/icons/hicolor/8x8/
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:33.003502 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-added-clean.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-added-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-added-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-added-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-added-clean.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-added-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-added-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-added-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-clean-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-clean.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-deleted-clean.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-deleted-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-deleted-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-deleted-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-modified-clean.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-modified-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-modified-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-modified-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-renamed-clean.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-renamed-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-renamed-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-renamed-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-unmerged-added-unmerged-added.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-clean-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-clean.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-deleted-clean.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-deleted-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-deleted-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-deleted-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2010 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-dotgit.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-modified-clean.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-modified-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-modified-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-modified-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-renamed-clean.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-renamed-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-renamed-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-renamed-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-added-clean.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-added-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-added-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-added-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-clean-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-clean.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-deleted-clean.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-deleted-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-deleted-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-deleted-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-modified-clean.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-modified-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-modified-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-modified-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-renamed-clean.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-renamed-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-renamed-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-renamed-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-unmerged-added-unmerged-added.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-unmerged-deleted-unmerged-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-unmerged-modified-unmerged-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-unmerged-modified-unmerged-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-unmerged-added-unmerged-added.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-unmerged-deleted-unmerged-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-unmerged-modified-unmerged-deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-unmerged-modified-unmerged-modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-untracked.png
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.963503 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:33.013502 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4642 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-dotgit.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2867 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3902 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2940 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4216 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3507 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-untracked.svg
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:32.963503 git-nautilus-icons-2.1.0/icons/hicolor/scalable/
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:33.023502 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4977 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     6012 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5050 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5617 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11238 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12273 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11311 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11878 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12374 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9086 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11068 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12103 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11141 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11708 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    10121 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11851 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12886 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11924 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12491 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9159 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    13988 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    15023 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    14061 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    14628 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    18823 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    18139 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    18135 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    18309 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9726 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     6113 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2825 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4807 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5842 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4880 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5447 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3860 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4600 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-dotgit.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5590 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     6625 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5663 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     6230 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2898 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     7727 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     8762 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     7800 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     8367 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9200 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-added-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    10235 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-added-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9273 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-added-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9840 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-added-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    10336 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-clean-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     7048 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9030 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-deleted-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    10065 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-deleted-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9103 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-deleted-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9670 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-deleted-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     8083 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9813 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-modified-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    10848 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-modified-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     9886 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-modified-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    10453 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-modified-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     7121 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11950 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-renamed-clean.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12985 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-renamed-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12023 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-renamed-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12590 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-renamed-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    16785 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    16101 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    16097 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    16271 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     7688 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-untracked.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12562 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-unmerged-added-unmerged-added.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11878 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-unmerged-deleted-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    11874 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-unmerged-modified-unmerged-deleted.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    12048 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-unmerged-modified-unmerged-modified.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3465 2020-05-23 23:55:25.000000 git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-untracked.svg
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:33.023502 git-nautilus-icons-2.1.0/icons/sub_icons/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2652 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/added-l.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2452 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/ahead.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3296 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/clean-l.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3264 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/clean-r.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2491 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/deleted-l.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4057 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/deleted-r.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5027 2020-05-23 23:54:43.000000 git-nautilus-icons-2.1.0/icons/sub_icons/dotgit-r.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3486 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/modified-l.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3379 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/modified-r.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5400 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/renamed-l.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5062 2020-05-23 23:55:13.000000 git-nautilus-icons-2.1.0/icons/sub_icons/repo.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     6956 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/unmerged-added-l.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5950 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/unmerged-added-r.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     6634 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/unmerged-deleted-l.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5624 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/unmerged-deleted-r.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     6894 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/unmerged-modified-l.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     5888 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/unmerged-modified-r.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     4651 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/unmerged-simple.svg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     3973 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/sub_icons/untracked-r.svg
+drwxr-xr-x   0 bilbo     (1000) bilbo     (1000)        0 2023-05-07 23:30:33.026836 git-nautilus-icons-2.1.0/icons/tiny_icons/
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      390 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/tiny_icons/clean.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      200 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/tiny_icons/deleted.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2010 2020-05-23 22:58:16.000000 git-nautilus-icons-2.1.0/icons/tiny_icons/dotgit.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2063 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/tiny_icons/modified.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      345 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/tiny_icons/unmerged.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)     2132 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/icons/tiny_icons/untracked.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    73067 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/key.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      107 2020-05-26 17:04:28.000000 git-nautilus-icons-2.1.0/pyproject.toml
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    72597 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/screenshot_caja.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    43233 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/screenshot_nautilus.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    99171 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/screenshot_nemo.png
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)       38 2023-05-07 23:30:33.026836 git-nautilus-icons-2.1.0/setup.cfg
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)      840 2022-04-05 02:42:00.000000 git-nautilus-icons-2.1.0/setup.py
+-rw-r--r--   0 bilbo     (1000) bilbo     (1000)    33935 2019-11-27 03:51:24.000000 git-nautilus-icons-2.1.0/small_icons.png
```

### Comparing `git-nautilus-icons-2.0.3/LICENSE` & `git-nautilus-icons-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/README.md` & `git-nautilus-icons-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/distro_icons/arch.png` & `git-nautilus-icons-2.1.0/distro_icons/arch.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/distro_icons/debian.png` & `git-nautilus-icons-2.1.0/distro_icons/debian.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/distro_icons/linux.png` & `git-nautilus-icons-2.1.0/distro_icons/linux.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/distro_icons/mint.png` & `git-nautilus-icons-2.1.0/distro_icons/mint.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/distro_icons/pop.png` & `git-nautilus-icons-2.1.0/distro_icons/pop.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/distro_icons/ubuntu.png` & `git-nautilus-icons-2.1.0/distro_icons/ubuntu.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/git-nautilus-icons.py` & `git-nautilus-icons-2.1.0/git-nautilus-icons.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,18 @@
     if sys.argv[0] == 'nemo':
         gi.require_version('Nemo', '3.0')
         from gi.repository import Nemo as Nautilus
     elif sys.argv[0] == 'caja':
         gi.require_version('Caja', '2.0')
         from gi.repository import Caja as Nautilus
     else:
-        gi.require_version('Nautilus', '3.0')
+        try:
+            gi.require_version('Nautilus', '3.0')
+        except ValueError:
+            gi.require_version('Nautilus', '4.0')
         from gi.repository import Nautilus
 
 
 BLACKLIST_TEMPLATE = """# git-{nautilus,nemo,caja}-icons blacklist file.
 #
 # The extension will ignore files in any directories listed in this file, and any of
 # their subdirectories.
```

### Comparing `git-nautilus-icons-2.0.3/git_nautilus_icons.egg-info/SOURCES.txt` & `git-nautilus-icons-2.1.0/git_nautilus_icons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/generate_icons.py` & `git-nautilus-icons-2.1.0/icons/generate_icons.py`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-ahead-repo-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-ahead-repo-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-dotgit.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-dotgit.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-repo-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-repo-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12/emblems/git-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12/emblems/git-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-ahead-repo-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-ahead-repo-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-dotgit.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-dotgit.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-repo-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-repo-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/12x12@2/emblems/git-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/12x12@2/emblems/git-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-ahead-repo-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-ahead-repo-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-dotgit.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-dotgit.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-repo-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-repo-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16/emblems/git-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16/emblems/git-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-ahead-repo-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-ahead-repo-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-dotgit.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-dotgit.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-repo-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-repo-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/16x16@2/emblems/git-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/16x16@2/emblems/git-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-added-modified.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-added-modified.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-added-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-added-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-added-modified.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-added-modified.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-added-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-added-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-clean-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-clean-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-deleted-modified.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-deleted-modified.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-deleted-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-deleted-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-modified-modified.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-modified-modified.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-modified-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-modified-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-modified.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-modified.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-renamed-modified.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-renamed-modified.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-renamed-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-renamed-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-ahead-repo-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-ahead-repo-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-clean-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-clean-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-deleted-modified.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-deleted-modified.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-deleted-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-deleted-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-dotgit.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-dotgit.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-modified-modified.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-modified-modified.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-modified-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-modified-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-modified.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-modified.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-renamed-modified.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-renamed-modified.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-renamed-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-renamed-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-added-modified.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-added-modified.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-added-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-added-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-clean-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-clean-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-deleted-modified.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-deleted-modified.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-deleted-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-deleted-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-modified-modified.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-modified-modified.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-modified-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-modified-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-modified.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-modified.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-renamed-modified.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-renamed-modified.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-renamed-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-renamed-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-repo-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-repo-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8/emblems/git-untracked.png` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8/emblems/git-untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-ahead-repo-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-ahead-repo-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-dotgit.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-dotgit.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-repo-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-repo-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/8x8@2/emblems/git-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/8x8@2/emblems/git-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-ahead-repo-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-ahead-repo-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-dotgit.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-dotgit.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-added-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-added-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-added-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-added-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-added-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-added-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-added-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-added-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-clean-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-clean-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-deleted-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-deleted-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-deleted-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-deleted-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-deleted-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-deleted-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-deleted-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-deleted-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-modified-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-modified-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-modified-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-modified-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-modified-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-modified-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-modified-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-modified-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-renamed-clean.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-renamed-clean.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-renamed-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-renamed-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-renamed-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-renamed-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-renamed-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-renamed-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-repo-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-repo-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-unmerged-added-unmerged-added.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-unmerged-added-unmerged-added.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-unmerged-deleted-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-unmerged-deleted-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-unmerged-modified-unmerged-deleted.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-unmerged-modified-unmerged-deleted.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-unmerged-modified-unmerged-modified.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-unmerged-modified-unmerged-modified.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/hicolor/scalable/emblems/git-untracked.svg` & `git-nautilus-icons-2.1.0/icons/hicolor/scalable/emblems/git-untracked.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/added-l.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/added-l.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/ahead.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/ahead.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/clean-l.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/clean-l.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/clean-r.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/clean-r.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/deleted-l.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/deleted-l.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/deleted-r.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/deleted-r.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/dotgit-r.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/dotgit-r.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/modified-l.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/modified-l.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/modified-r.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/modified-r.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/renamed-l.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/renamed-l.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/repo.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/repo.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/unmerged-added-l.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/unmerged-added-l.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/unmerged-added-r.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/unmerged-added-r.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/unmerged-deleted-l.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/unmerged-deleted-l.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/unmerged-deleted-r.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/unmerged-deleted-r.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/unmerged-modified-l.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/unmerged-modified-l.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/unmerged-modified-r.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/unmerged-modified-r.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/unmerged-simple.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/unmerged-simple.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/sub_icons/untracked-r.svg` & `git-nautilus-icons-2.1.0/icons/sub_icons/untracked-r.svg`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/tiny_icons/dotgit.png` & `git-nautilus-icons-2.1.0/icons/tiny_icons/dotgit.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/tiny_icons/modified.png` & `git-nautilus-icons-2.1.0/icons/tiny_icons/modified.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/icons/tiny_icons/untracked.png` & `git-nautilus-icons-2.1.0/icons/tiny_icons/untracked.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/key.png` & `git-nautilus-icons-2.1.0/key.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/screenshot_caja.png` & `git-nautilus-icons-2.1.0/screenshot_caja.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/screenshot_nautilus.png` & `git-nautilus-icons-2.1.0/screenshot_nautilus.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/screenshot_nemo.png` & `git-nautilus-icons-2.1.0/screenshot_nemo.png`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/setup.py` & `git-nautilus-icons-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `git-nautilus-icons-2.0.3/small_icons.png` & `git-nautilus-icons-2.1.0/small_icons.png`

 * *Files identical despite different names*

