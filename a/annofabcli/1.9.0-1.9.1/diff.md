# Comparing `tmp/annofabcli-1.9.0.tar.gz` & `tmp/annofabcli-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/annofabcli-1.9.0.tar", last modified: Tue Sep 10 05:57:06 2019, max compression
+gzip compressed data, was "dist/annofabcli-1.9.1.tar", last modified: Thu Sep 12 03:42:28 2019, max compression
```

## Comparing `annofabcli-1.9.0.tar` & `annofabcli-1.9.1.tar`

### file list

```diff
@@ -1,79 +1,89 @@
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-10 05:57:06.000000 annofabcli-1.9.0/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    37274 2019-09-10 05:57:06.000000 annofabcli-1.9.0/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    30600 2019-09-10 05:52:12.000000 annofabcli-1.9.0/README.md
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      276 2019-07-20 09:23:53.000000 annofabcli-1.9.0/annofabcli/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2428 2019-09-04 07:35:37.000000 annofabcli-1.9.0/annofabcli/__main__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       22 2019-09-10 05:53:19.000000 annofabcli-1.9.0/annofabcli/__version__.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli/annotation/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-07-28 11:21:58.000000 annofabcli-1.9.0/annofabcli/annotation/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    11373 2019-09-04 08:21:24.000000 annofabcli-1.9.0/annofabcli/annotation/list_annotation_count.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      700 2019-08-19 03:21:09.000000 annofabcli-1.9.0/annofabcli/annotation/subcommand_annotation.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli/annotation_specs/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-07-20 11:40:41.000000 annofabcli-1.9.0/annofabcli/annotation_specs/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3809 2019-07-26 01:34:58.000000 annofabcli-1.9.0/annofabcli/annotation_specs/list_annotation_specs_label.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2701 2019-08-06 11:48:17.000000 annofabcli-1.9.0/annofabcli/annotation_specs/print_label_color.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      868 2019-08-19 03:21:09.000000 annofabcli-1.9.0/annofabcli/annotation_specs/subcommand_annotation_specs.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli/common/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-05-28 03:12:51.000000 annofabcli-1.9.0/annofabcli/common/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    15798 2019-09-04 08:21:24.000000 annofabcli-1.9.0/annofabcli/common/cli.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      717 2019-08-05 09:45:02.000000 annofabcli-1.9.0/annofabcli/common/enums.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1460 2019-09-04 08:21:24.000000 annofabcli-1.9.0/annofabcli/common/exceptions.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    17787 2019-09-04 08:21:24.000000 annofabcli-1.9.0/annofabcli/common/facade.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     9810 2019-09-04 07:35:37.000000 annofabcli-1.9.0/annofabcli/common/image.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      433 2019-05-30 12:14:43.000000 annofabcli-1.9.0/annofabcli/common/typing.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7383 2019-09-10 05:52:12.000000 annofabcli-1.9.0/annofabcli/common/utils.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7767 2019-08-05 12:10:09.000000 annofabcli-1.9.0/annofabcli/common/visualize.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli/data/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      695 2019-07-04 13:35:34.000000 annofabcli-1.9.0/annofabcli/data/logging.yaml
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    13201 2019-07-26 09:55:42.000000 annofabcli-1.9.0/annofabcli/deprecated_register_annotation_from_full_zip.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    16606 2019-08-30 03:35:43.000000 annofabcli-1.9.0/annofabcli/deprecated_write_annotation_image.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli/filesystem/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-08-17 11:02:53.000000 annofabcli-1.9.0/annofabcli/filesystem/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      748 2019-08-19 14:08:37.000000 annofabcli-1.9.0/annofabcli/filesystem/subcommand_filesystem.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7634 2019-08-30 03:35:43.000000 annofabcli-1.9.0/annofabcli/filesystem/write_annotation_image.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli/input_data/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-07-17 08:26:34.000000 annofabcli-1.9.0/annofabcli/input_data/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7841 2019-09-04 08:21:24.000000 annofabcli-1.9.0/annofabcli/input_data/list_input_data.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7330 2019-09-10 05:52:12.000000 annofabcli-1.9.0/annofabcli/input_data/put_input_data.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      784 2019-09-10 05:52:12.000000 annofabcli-1.9.0/annofabcli/input_data/subcommand_input_data.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli/inspection_comment/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-07-17 08:49:28.000000 annofabcli-1.9.0/annofabcli/inspection_comment/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5552 2019-08-06 12:31:59.000000 annofabcli-1.9.0/annofabcli/inspection_comment/list_inspections.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3446 2019-08-06 12:31:55.000000 annofabcli-1.9.0/annofabcli/inspection_comment/list_unprocessed_inspections.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      860 2019-08-19 03:21:09.000000 annofabcli-1.9.0/annofabcli/inspection_comment/subcommand_inspection_comment.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli/instruction/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-08-06 06:18:37.000000 annofabcli-1.9.0/annofabcli/instruction/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      685 2019-08-19 03:21:09.000000 annofabcli-1.9.0/annofabcli/instruction/subcommand_instruction.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3323 2019-08-06 08:56:17.000000 annofabcli-1.9.0/annofabcli/instruction/upload_instruction.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli/project/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-07-17 11:07:49.000000 annofabcli-1.9.0/annofabcli/project/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6544 2019-09-10 05:52:12.000000 annofabcli-1.9.0/annofabcli/project/copy_project.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    16365 2019-08-06 12:31:58.000000 annofabcli-1.9.0/annofabcli/project/diff_projects.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4698 2019-07-26 01:48:27.000000 annofabcli-1.9.0/annofabcli/project/download.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      857 2019-09-04 08:21:24.000000 annofabcli-1.9.0/annofabcli/project/subcommand_project.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli/project_member/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-07-17 10:58:44.000000 annofabcli-1.9.0/annofabcli/project_member/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6950 2019-09-09 08:29:11.000000 annofabcli-1.9.0/annofabcli/project_member/copy_project_members.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4746 2019-08-06 12:31:57.000000 annofabcli-1.9.0/annofabcli/project_member/delete_users.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5020 2019-08-06 12:31:45.000000 annofabcli-1.9.0/annofabcli/project_member/invite_users.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7563 2019-08-28 10:40:51.000000 annofabcli-1.9.0/annofabcli/project_member/list_users.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     8867 2019-09-10 05:52:12.000000 annofabcli-1.9.0/annofabcli/project_member/put_project_members.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1180 2019-08-28 08:13:43.000000 annofabcli-1.9.0/annofabcli/project_member/subcommand_project_member.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli/task/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-07-17 08:26:34.000000 annofabcli-1.9.0/annofabcli/task/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4264 2019-07-26 01:45:07.000000 annofabcli-1.9.0/annofabcli/task/cancel_acceptance.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5333 2019-08-30 03:35:43.000000 annofabcli-1.9.0/annofabcli/task/change_operator.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     9926 2019-08-06 12:30:17.000000 annofabcli-1.9.0/annofabcli/task/complete_tasks.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6144 2019-09-04 08:21:24.000000 annofabcli-1.9.0/annofabcli/task/list_tasks.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    10503 2019-08-28 11:33:59.000000 annofabcli-1.9.0/annofabcli/task/reject_tasks.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1024 2019-08-30 03:35:43.000000 annofabcli-1.9.0/annofabcli/task/subcommand_task.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli.egg-info/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    37274 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2390 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli.egg-info/dependency_links.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       57 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli.egg-info/entry_points.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      123 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli.egg-info/requires.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       11 2019-09-10 05:57:06.000000 annofabcli-1.9.0/annofabcli.egg-info/top_level.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1592 2019-09-10 05:57:06.000000 annofabcli-1.9.0/setup.cfg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1842 2019-09-10 05:52:12.000000 annofabcli-1.9.0/setup.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 03:42:28.000000 annofabcli-1.9.1/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    37274 2019-09-12 03:42:28.000000 annofabcli-1.9.1/PKG-INFO
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    30600 2019-09-10 05:52:12.000000 annofabcli-1.9.1/README.md
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      276 2019-07-20 09:23:53.000000 annofabcli-1.9.1/annofabcli/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2428 2019-09-04 07:35:37.000000 annofabcli-1.9.1/annofabcli/__main__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       22 2019-09-12 03:35:29.000000 annofabcli-1.9.1/annofabcli/__version__.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli/annotation/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-07-28 11:21:58.000000 annofabcli-1.9.1/annofabcli/annotation/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    11373 2019-09-04 08:21:24.000000 annofabcli-1.9.1/annofabcli/annotation/list_annotation_count.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      700 2019-08-19 03:21:09.000000 annofabcli-1.9.1/annofabcli/annotation/subcommand_annotation.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli/annotation_specs/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-07-20 11:40:41.000000 annofabcli-1.9.1/annofabcli/annotation_specs/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3809 2019-07-26 01:34:58.000000 annofabcli-1.9.1/annofabcli/annotation_specs/list_annotation_specs_label.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2701 2019-08-06 11:48:17.000000 annofabcli-1.9.1/annofabcli/annotation_specs/print_label_color.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      868 2019-08-19 03:21:09.000000 annofabcli-1.9.1/annofabcli/annotation_specs/subcommand_annotation_specs.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli/common/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-05-28 03:12:51.000000 annofabcli-1.9.1/annofabcli/common/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    15798 2019-09-04 08:21:24.000000 annofabcli-1.9.1/annofabcli/common/cli.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      717 2019-08-05 09:45:02.000000 annofabcli-1.9.1/annofabcli/common/enums.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1460 2019-09-04 08:21:24.000000 annofabcli-1.9.1/annofabcli/common/exceptions.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    17787 2019-09-04 08:21:24.000000 annofabcli-1.9.1/annofabcli/common/facade.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     9810 2019-09-04 07:35:37.000000 annofabcli-1.9.1/annofabcli/common/image.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      433 2019-05-30 12:14:43.000000 annofabcli-1.9.1/annofabcli/common/typing.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7383 2019-09-10 05:52:12.000000 annofabcli-1.9.1/annofabcli/common/utils.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7767 2019-08-05 12:10:09.000000 annofabcli-1.9.1/annofabcli/common/visualize.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli/data/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      695 2019-07-04 13:35:34.000000 annofabcli-1.9.1/annofabcli/data/logging.yaml
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    13201 2019-07-26 09:55:42.000000 annofabcli-1.9.1/annofabcli/deprecated_register_annotation_from_full_zip.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    16606 2019-08-30 03:35:43.000000 annofabcli-1.9.1/annofabcli/deprecated_write_annotation_image.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli/filesystem/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-08-17 11:02:53.000000 annofabcli-1.9.1/annofabcli/filesystem/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      748 2019-08-19 14:08:37.000000 annofabcli-1.9.1/annofabcli/filesystem/subcommand_filesystem.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7634 2019-08-30 03:35:43.000000 annofabcli-1.9.1/annofabcli/filesystem/write_annotation_image.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli/input_data/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-07-17 08:26:34.000000 annofabcli-1.9.1/annofabcli/input_data/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7841 2019-09-04 08:21:24.000000 annofabcli-1.9.1/annofabcli/input_data/list_input_data.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7330 2019-09-10 05:52:12.000000 annofabcli-1.9.1/annofabcli/input_data/put_input_data.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      784 2019-09-10 05:52:12.000000 annofabcli-1.9.1/annofabcli/input_data/subcommand_input_data.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli/inspection_comment/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-07-17 08:49:28.000000 annofabcli-1.9.1/annofabcli/inspection_comment/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5552 2019-08-06 12:31:59.000000 annofabcli-1.9.1/annofabcli/inspection_comment/list_inspections.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3446 2019-08-06 12:31:55.000000 annofabcli-1.9.1/annofabcli/inspection_comment/list_unprocessed_inspections.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      860 2019-08-19 03:21:09.000000 annofabcli-1.9.1/annofabcli/inspection_comment/subcommand_inspection_comment.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli/instruction/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-08-06 06:18:37.000000 annofabcli-1.9.1/annofabcli/instruction/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      685 2019-08-19 03:21:09.000000 annofabcli-1.9.1/annofabcli/instruction/subcommand_instruction.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3323 2019-08-06 08:56:17.000000 annofabcli-1.9.1/annofabcli/instruction/upload_instruction.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli/project/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-07-17 11:07:49.000000 annofabcli-1.9.1/annofabcli/project/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6544 2019-09-10 05:52:12.000000 annofabcli-1.9.1/annofabcli/project/copy_project.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    16365 2019-08-06 12:31:58.000000 annofabcli-1.9.1/annofabcli/project/diff_projects.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4698 2019-07-26 01:48:27.000000 annofabcli-1.9.1/annofabcli/project/download.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      857 2019-09-04 08:21:24.000000 annofabcli-1.9.1/annofabcli/project/subcommand_project.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli/project_member/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-07-17 10:58:44.000000 annofabcli-1.9.1/annofabcli/project_member/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6950 2019-09-09 08:29:11.000000 annofabcli-1.9.1/annofabcli/project_member/copy_project_members.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4746 2019-08-06 12:31:57.000000 annofabcli-1.9.1/annofabcli/project_member/delete_users.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5020 2019-08-06 12:31:45.000000 annofabcli-1.9.1/annofabcli/project_member/invite_users.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7563 2019-08-28 10:40:51.000000 annofabcli-1.9.1/annofabcli/project_member/list_users.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     8867 2019-09-10 05:52:12.000000 annofabcli-1.9.1/annofabcli/project_member/put_project_members.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1180 2019-08-28 08:13:43.000000 annofabcli-1.9.1/annofabcli/project_member/subcommand_project_member.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli/statistics/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-07-17 10:58:44.000000 annofabcli-1.9.1/annofabcli/statistics/__init__.py
+-rwxrwxr-x   0 vagrant   (1000) vagrant   (1000)      253 2019-09-04 07:35:37.000000 annofabcli-1.9.1/annofabcli/statistics/annofab_typing.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    12364 2019-09-04 07:35:37.000000 annofabcli-1.9.1/annofabcli/statistics/database.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    10471 2019-09-04 08:21:24.000000 annofabcli-1.9.1/annofabcli/statistics/graph.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      668 2019-09-04 07:35:37.000000 annofabcli-1.9.1/annofabcli/statistics/subcommand_statistics.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    21603 2019-09-04 07:35:37.000000 annofabcli-1.9.1/annofabcli/statistics/table.py
+-rwxrwxr-x   0 vagrant   (1000) vagrant   (1000)     7150 2019-09-04 07:35:37.000000 annofabcli-1.9.1/annofabcli/statistics/tsv.py
+-rwxrwxr-x   0 vagrant   (1000) vagrant   (1000)      868 2019-09-04 07:35:37.000000 annofabcli-1.9.1/annofabcli/statistics/utils.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6342 2019-09-04 08:21:24.000000 annofabcli-1.9.1/annofabcli/statistics/visualize_statistics.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli/task/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-07-17 08:26:34.000000 annofabcli-1.9.1/annofabcli/task/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4264 2019-07-26 01:45:07.000000 annofabcli-1.9.1/annofabcli/task/cancel_acceptance.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5333 2019-08-30 03:35:43.000000 annofabcli-1.9.1/annofabcli/task/change_operator.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     9926 2019-08-06 12:30:17.000000 annofabcli-1.9.1/annofabcli/task/complete_tasks.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6144 2019-09-04 08:21:24.000000 annofabcli-1.9.1/annofabcli/task/list_tasks.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    10503 2019-08-28 11:33:59.000000 annofabcli-1.9.1/annofabcli/task/reject_tasks.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1024 2019-08-30 03:35:43.000000 annofabcli-1.9.1/annofabcli/task/subcommand_task.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli.egg-info/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    37274 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli.egg-info/PKG-INFO
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2713 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli.egg-info/SOURCES.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli.egg-info/dependency_links.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       57 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli.egg-info/entry_points.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      123 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli.egg-info/requires.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       11 2019-09-12 03:42:28.000000 annofabcli-1.9.1/annofabcli.egg-info/top_level.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1592 2019-09-12 03:42:28.000000 annofabcli-1.9.1/setup.cfg
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1842 2019-09-10 05:52:12.000000 annofabcli-1.9.1/setup.py
```

### Comparing `annofabcli-1.9.0/PKG-INFO` & `annofabcli-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annofabcli
-Version: 1.9.0
+Version: 1.9.1
 Summary: Utility Command Line Interface for AnnoFab
 Home-page: https://github.com/kurusugawa-computer/annofab-cli
 Author: yuji38kwmt
 Author-email: yuji38kwmt@gmail.com
 Maintainer: yuji38kwmt
 License: MIT
 Description: # 概要
```

### Comparing `annofabcli-1.9.0/README.md` & `annofabcli-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/__main__.py` & `annofabcli-1.9.1/annofabcli/__main__.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/annotation/list_annotation_count.py` & `annofabcli-1.9.1/annofabcli/annotation/list_annotation_count.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/annotation/subcommand_annotation.py` & `annofabcli-1.9.1/annofabcli/annotation/subcommand_annotation.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/annotation_specs/list_annotation_specs_label.py` & `annofabcli-1.9.1/annofabcli/annotation_specs/list_annotation_specs_label.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/annotation_specs/print_label_color.py` & `annofabcli-1.9.1/annofabcli/annotation_specs/print_label_color.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/annotation_specs/subcommand_annotation_specs.py` & `annofabcli-1.9.1/annofabcli/annotation_specs/subcommand_annotation_specs.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/common/cli.py` & `annofabcli-1.9.1/annofabcli/common/cli.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/common/enums.py` & `annofabcli-1.9.1/annofabcli/common/enums.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/common/exceptions.py` & `annofabcli-1.9.1/annofabcli/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/common/facade.py` & `annofabcli-1.9.1/annofabcli/common/facade.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/common/image.py` & `annofabcli-1.9.1/annofabcli/common/image.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/common/utils.py` & `annofabcli-1.9.1/annofabcli/common/utils.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/common/visualize.py` & `annofabcli-1.9.1/annofabcli/common/visualize.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/data/logging.yaml` & `annofabcli-1.9.1/annofabcli/data/logging.yaml`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/deprecated_register_annotation_from_full_zip.py` & `annofabcli-1.9.1/annofabcli/deprecated_register_annotation_from_full_zip.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/deprecated_write_annotation_image.py` & `annofabcli-1.9.1/annofabcli/deprecated_write_annotation_image.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/filesystem/subcommand_filesystem.py` & `annofabcli-1.9.1/annofabcli/filesystem/subcommand_filesystem.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/filesystem/write_annotation_image.py` & `annofabcli-1.9.1/annofabcli/filesystem/write_annotation_image.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/input_data/list_input_data.py` & `annofabcli-1.9.1/annofabcli/input_data/list_input_data.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/input_data/put_input_data.py` & `annofabcli-1.9.1/annofabcli/input_data/put_input_data.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/input_data/subcommand_input_data.py` & `annofabcli-1.9.1/annofabcli/input_data/subcommand_input_data.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/inspection_comment/list_inspections.py` & `annofabcli-1.9.1/annofabcli/inspection_comment/list_inspections.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/inspection_comment/list_unprocessed_inspections.py` & `annofabcli-1.9.1/annofabcli/inspection_comment/list_unprocessed_inspections.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/inspection_comment/subcommand_inspection_comment.py` & `annofabcli-1.9.1/annofabcli/inspection_comment/subcommand_inspection_comment.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/instruction/subcommand_instruction.py` & `annofabcli-1.9.1/annofabcli/instruction/subcommand_instruction.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/instruction/upload_instruction.py` & `annofabcli-1.9.1/annofabcli/instruction/upload_instruction.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/project/copy_project.py` & `annofabcli-1.9.1/annofabcli/project/copy_project.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/project/diff_projects.py` & `annofabcli-1.9.1/annofabcli/project/diff_projects.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/project/download.py` & `annofabcli-1.9.1/annofabcli/project/download.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/project/subcommand_project.py` & `annofabcli-1.9.1/annofabcli/project/subcommand_project.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/project_member/copy_project_members.py` & `annofabcli-1.9.1/annofabcli/project_member/copy_project_members.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/project_member/delete_users.py` & `annofabcli-1.9.1/annofabcli/project_member/delete_users.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/project_member/invite_users.py` & `annofabcli-1.9.1/annofabcli/project_member/invite_users.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/project_member/list_users.py` & `annofabcli-1.9.1/annofabcli/project_member/list_users.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/project_member/put_project_members.py` & `annofabcli-1.9.1/annofabcli/project_member/put_project_members.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/project_member/subcommand_project_member.py` & `annofabcli-1.9.1/annofabcli/project_member/subcommand_project_member.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/task/cancel_acceptance.py` & `annofabcli-1.9.1/annofabcli/task/cancel_acceptance.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/task/change_operator.py` & `annofabcli-1.9.1/annofabcli/task/change_operator.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/task/complete_tasks.py` & `annofabcli-1.9.1/annofabcli/task/complete_tasks.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/task/list_tasks.py` & `annofabcli-1.9.1/annofabcli/task/list_tasks.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/task/reject_tasks.py` & `annofabcli-1.9.1/annofabcli/task/reject_tasks.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli/task/subcommand_task.py` & `annofabcli-1.9.1/annofabcli/task/subcommand_task.py`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/annofabcli.egg-info/PKG-INFO` & `annofabcli-1.9.1/annofabcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annofabcli
-Version: 1.9.0
+Version: 1.9.1
 Summary: Utility Command Line Interface for AnnoFab
 Home-page: https://github.com/kurusugawa-computer/annofab-cli
 Author: yuji38kwmt
 Author-email: yuji38kwmt@gmail.com
 Maintainer: yuji38kwmt
 License: MIT
 Description: # 概要
```

### Comparing `annofabcli-1.9.0/annofabcli.egg-info/SOURCES.txt` & `annofabcli-1.9.1/annofabcli.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -51,14 +51,23 @@
 annofabcli/project_member/__init__.py
 annofabcli/project_member/copy_project_members.py
 annofabcli/project_member/delete_users.py
 annofabcli/project_member/invite_users.py
 annofabcli/project_member/list_users.py
 annofabcli/project_member/put_project_members.py
 annofabcli/project_member/subcommand_project_member.py
+annofabcli/statistics/__init__.py
+annofabcli/statistics/annofab_typing.py
+annofabcli/statistics/database.py
+annofabcli/statistics/graph.py
+annofabcli/statistics/subcommand_statistics.py
+annofabcli/statistics/table.py
+annofabcli/statistics/tsv.py
+annofabcli/statistics/utils.py
+annofabcli/statistics/visualize_statistics.py
 annofabcli/task/__init__.py
 annofabcli/task/cancel_acceptance.py
 annofabcli/task/change_operator.py
 annofabcli/task/complete_tasks.py
 annofabcli/task/list_tasks.py
 annofabcli/task/reject_tasks.py
 annofabcli/task/subcommand_task.py
```

### Comparing `annofabcli-1.9.0/setup.cfg` & `annofabcli-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `annofabcli-1.9.0/setup.py` & `annofabcli-1.9.1/setup.py`

 * *Files identical despite different names*

