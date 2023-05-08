# Comparing `tmp/inductiva-0.0.8.tar.gz` & `tmp/inductiva-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inductiva-0.0.8.tar", last modified: Fri Apr 14 11:33:31 2023, max compression
+gzip compressed data, was "inductiva-0.0.9.tar", last modified: Fri Apr 14 13:02:50 2023, max compression
```

## Comparing `inductiva-0.0.8.tar` & `inductiva-0.0.9.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       43 2023-04-14 10:18:54.000000 inductiva-0.0.8/MANIFEST.in
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3570 2023-04-14 11:33:31.458069 inductiva-0.0.8/PKG-INFO
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3196 2023-04-14 10:18:54.000000 inductiva-0.0.8/README.md
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      387 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/api/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      122 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/api/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    13042 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/api/methods.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      805 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    60856 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/api_client.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/apis/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      214 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1421 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/path_to_api.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/apis/paths/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      243 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/paths/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      112 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/paths/admin_user.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      137 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/paths/admin_user_username_tasks.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      114 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/paths/task_submit.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      126 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/paths/task_task_id_input.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      124 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/paths/task_task_id_kill.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/paths/task_task_id_output.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/paths/task_task_id_status.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      400 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/tag_to_api.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/apis/tags/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/tags/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      622 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/tags/admin_api.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      916 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/tags/tasks_api.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    16615 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/configuration.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4590 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/exceptions.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/model/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      350 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/model/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2759 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/model/body_upload_task_input.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3636 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/model/http_validation_error.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4386 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/model/new_user.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4682 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/model/queue_status.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3628 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/model/task_request.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6465 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/model/task_status.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     7930 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/model/validation_error.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/models/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      843 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/models/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/paths/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      617 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/paths/admin_user/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      311 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/admin_user/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12303 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/admin_user/post.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/paths/admin_user_username_tasks/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      341 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/admin_user_username_tasks/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10351 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/admin_user_username_tasks/get.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/paths/task_submit/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      313 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_submit/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12455 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_submit/post.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/paths/task_task_id_input/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      327 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_task_id_input/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    15178 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_task_id_input/post.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/paths/task_task_id_kill/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      325 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_task_id_kill/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10501 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_task_id_kill/post.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/paths/task_task_id_output/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_task_id_output/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10463 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_task_id_output/get.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/paths/task_task_id_status/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_task_id_status/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10400 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_task_id_status/get.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    11962 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/rest.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)   103899 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/schemas.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/core/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      120 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/core/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/core/cupy/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       85 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/core/cupy/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      379 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/core/cupy/linalg.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      586 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/core/math.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/core/slepc/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       64 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/core/slepc/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      491 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/core/slepc/linalg.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      333 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/core/test.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      102 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/exceptions.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/fluids/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      571 2023-04-14 11:15:16.000000 inductiva-0.0.8/inductiva/fluids/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1002 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/fluid_types.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/fluids/post_processing/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/post_processing/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     5247 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/post_processing/splishsplash.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/fluids/scenarios/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      250 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1610 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/_post_processing.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/fluids/scenarios/dam_break/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       74 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/dam_break/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2670 2023-04-14 11:15:16.000000 inductiva-0.0.8/inductiva/fluids/scenarios/dam_break/dam_break.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       78 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     7904 2023-04-14 11:15:16.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/fluid_block.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4230 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1350 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      700 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/unit_box.obj
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      182 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8868 2023-04-14 11:29:18.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1914 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     9181 2023-04-14 11:29:18.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6444 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2507 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/shapes.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/fluids/simulators/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      203 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/simulators/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1121 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/simulators/dualsphysics.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1288 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/simulators/openfoam.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1084 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/simulators/splishsplash.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1065 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/simulators/swash.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      995 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/simulators/xbeach.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/molecules/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       74 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/molecules/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/molecules/simulators/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       71 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/molecules/simulators/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1312 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/molecules/simulators/gromacs.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1353 2023-04-14 11:15:16.000000 inductiva-0.0.8/inductiva/scenarios.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/simulation/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       76 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/simulation/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1938 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/simulation/simulator.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      142 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/types.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/utils/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8337 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/data.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2159 2023-04-14 11:15:16.000000 inductiva-0.0.8/inductiva/utils/files.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      783 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/files_test.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1720 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/flags.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1672 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/meta.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      272 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/misc.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      750 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/misc_test.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      509 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/templates.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    14282 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/visualization.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva.egg-info/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3570 2023-04-14 11:33:31.000000 inductiva-0.0.8/inductiva.egg-info/PKG-INFO
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4134 2023-04-14 11:33:31.000000 inductiva-0.0.8/inductiva.egg-info/SOURCES.txt
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        1 2023-04-14 11:33:31.000000 inductiva-0.0.8/inductiva.egg-info/dependency_links.txt
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      175 2023-04-14 11:33:31.000000 inductiva-0.0.8/inductiva.egg-info/requires.txt
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       10 2023-04-14 11:33:31.000000 inductiva-0.0.8/inductiva.egg-info/top_level.txt
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       87 2023-04-14 10:18:54.000000 inductiva-0.0.8/pyproject.toml
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      779 2023-04-14 11:33:31.458069 inductiva-0.0.8/setup.cfg
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       56 2023-04-14 10:18:54.000000 inductiva-0.0.8/setup.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       43 2023-04-14 10:18:54.000000 inductiva-0.0.9/MANIFEST.in
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3650 2023-04-14 13:02:50.492152 inductiva-0.0.9/PKG-INFO
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3276 2023-04-14 13:02:29.000000 inductiva-0.0.9/README.md
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      387 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/api/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      122 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/api/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    13042 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/api/methods.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      805 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    60856 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/api_client.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/apis/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      214 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1421 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/path_to_api.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/apis/paths/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      243 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/paths/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      112 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/paths/admin_user.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      137 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/paths/admin_user_username_tasks.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      114 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/paths/task_submit.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      126 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/paths/task_task_id_input.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      124 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/paths/task_task_id_kill.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/paths/task_task_id_output.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/paths/task_task_id_status.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      400 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/tag_to_api.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/apis/tags/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/tags/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      622 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/tags/admin_api.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      916 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/tags/tasks_api.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    16615 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/configuration.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4590 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/exceptions.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/model/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      350 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/model/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2759 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/model/body_upload_task_input.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3636 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/model/http_validation_error.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4386 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/model/new_user.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4682 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/model/queue_status.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3628 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/model/task_request.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6465 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/model/task_status.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     7930 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/model/validation_error.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/models/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      843 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/models/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/paths/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      617 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/paths/admin_user/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      311 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/admin_user/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12303 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/admin_user/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/paths/admin_user_username_tasks/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      341 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/admin_user_username_tasks/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10351 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/admin_user_username_tasks/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/paths/task_submit/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      313 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_submit/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12455 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_submit/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/paths/task_task_id_input/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      327 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_task_id_input/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    15178 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_task_id_input/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/paths/task_task_id_kill/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      325 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_task_id_kill/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10501 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_task_id_kill/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/paths/task_task_id_output/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_task_id_output/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10463 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_task_id_output/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/paths/task_task_id_status/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_task_id_status/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10400 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_task_id_status/get.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    11962 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/rest.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)   103899 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/schemas.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/core/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      120 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/core/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/core/cupy/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       85 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/core/cupy/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      379 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/core/cupy/linalg.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      586 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/core/math.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/core/slepc/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       64 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/core/slepc/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      491 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/core/slepc/linalg.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      333 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/core/test.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      102 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/exceptions.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/fluids/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      571 2023-04-14 11:15:16.000000 inductiva-0.0.9/inductiva/fluids/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1002 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/fluid_types.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/fluids/post_processing/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/post_processing/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     5247 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/post_processing/splishsplash.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/fluids/scenarios/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      250 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1748 2023-04-14 13:02:29.000000 inductiva-0.0.9/inductiva/fluids/scenarios/_post_processing.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/fluids/scenarios/dam_break/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       74 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/dam_break/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2670 2023-04-14 11:15:16.000000 inductiva-0.0.9/inductiva/fluids/scenarios/dam_break/dam_break.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       78 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     7904 2023-04-14 11:15:16.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/fluid_block.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4230 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1350 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      700 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/unit_box.obj
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      182 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8868 2023-04-14 11:29:18.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1914 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     9181 2023-04-14 11:29:18.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6444 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2507 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/shapes.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/fluids/simulators/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      203 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/simulators/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1121 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/simulators/dualsphysics.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1288 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/simulators/openfoam.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1084 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/simulators/splishsplash.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1065 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/simulators/swash.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      995 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/simulators/xbeach.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/molecules/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       74 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/molecules/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/molecules/simulators/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       71 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/molecules/simulators/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1312 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/molecules/simulators/gromacs.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1353 2023-04-14 11:15:16.000000 inductiva-0.0.9/inductiva/scenarios.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/simulation/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       76 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/simulation/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1938 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/simulation/simulator.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      142 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/types.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/utils/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/utils/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8337 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/utils/data.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2159 2023-04-14 11:15:16.000000 inductiva-0.0.9/inductiva/utils/files.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      783 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/utils/files_test.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1720 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/utils/flags.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1672 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/utils/meta.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      272 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/utils/misc.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      750 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/utils/misc_test.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      509 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/utils/templates.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    14281 2023-04-14 13:02:29.000000 inductiva-0.0.9/inductiva/utils/visualization.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva.egg-info/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3650 2023-04-14 13:02:50.000000 inductiva-0.0.9/inductiva.egg-info/PKG-INFO
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4134 2023-04-14 13:02:50.000000 inductiva-0.0.9/inductiva.egg-info/SOURCES.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        1 2023-04-14 13:02:50.000000 inductiva-0.0.9/inductiva.egg-info/dependency_links.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      175 2023-04-14 13:02:50.000000 inductiva-0.0.9/inductiva.egg-info/requires.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       10 2023-04-14 13:02:50.000000 inductiva-0.0.9/inductiva.egg-info/top_level.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       87 2023-04-14 10:18:54.000000 inductiva-0.0.9/pyproject.toml
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      779 2023-04-14 13:02:50.492152 inductiva-0.0.9/setup.cfg
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       56 2023-04-14 10:18:54.000000 inductiva-0.0.9/setup.py
```

### Comparing `inductiva-0.0.8/PKG-INFO` & `inductiva-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: inductiva
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python client for the Inductiva API
 Home-page: https://github.com/inductiva/inductiva
 Author: Inductiva Research Labs
 Author-email: contact@inductiva.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-![Python package](https://github.com/inductiva/inductiva/actions/workflows/python-package.yml/badge.svg)
+
+[![Python package](https://github.com/inductiva/inductiva/actions/workflows/python-package.yml/badge.svg)](https://github.com/inductiva/inductiva/actions/workflows/python-package.yml)
 
 ![linkedin_header](https://user-images.githubusercontent.com/104431973/231184851-0ce34289-593e-4832-aaa2-9aae652113f5.jpg)
 
 ## Large scale simulations made simple
 
 Inductiva API provides dozens of open-source physical simulation packages from your laptop. Users can start simulating right away, with no hardware setup issues and no software configuration headaches. Additionally, we provide a transparent way to scale your simulations to the next-level with one-line of code.
```

### Comparing `inductiva-0.0.8/README.md` & `inductiva-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-![Python package](https://github.com/inductiva/inductiva/actions/workflows/python-package.yml/badge.svg)
+
+[![Python package](https://github.com/inductiva/inductiva/actions/workflows/python-package.yml/badge.svg)](https://github.com/inductiva/inductiva/actions/workflows/python-package.yml)
 
 ![linkedin_header](https://user-images.githubusercontent.com/104431973/231184851-0ce34289-593e-4832-aaa2-9aae652113f5.jpg)
 
 ## Large scale simulations made simple
 
 Inductiva API provides dozens of open-source physical simulation packages from your laptop. Users can start simulating right away, with no hardware setup issues and no software configuration headaches. Additionally, we provide a transparent way to scale your simulations to the next-level with one-line of code.
```

### Comparing `inductiva-0.0.8/inductiva/api/methods.py` & `inductiva-0.0.9/inductiva/api/methods.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/__init__.py` & `inductiva-0.0.9/inductiva/client/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/api_client.py` & `inductiva-0.0.9/inductiva/client/api_client.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/apis/path_to_api.py` & `inductiva-0.0.9/inductiva/client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/apis/tags/admin_api.py` & `inductiva-0.0.9/inductiva/client/apis/tags/admin_api.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/apis/tags/tasks_api.py` & `inductiva-0.0.9/inductiva/client/apis/tags/tasks_api.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/configuration.py` & `inductiva-0.0.9/inductiva/client/configuration.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/exceptions.py` & `inductiva-0.0.9/inductiva/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/model/body_upload_task_input.py` & `inductiva-0.0.9/inductiva/client/model/body_upload_task_input.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/model/http_validation_error.py` & `inductiva-0.0.9/inductiva/client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/model/new_user.py` & `inductiva-0.0.9/inductiva/client/model/new_user.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/model/queue_status.py` & `inductiva-0.0.9/inductiva/client/model/queue_status.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/model/task_request.py` & `inductiva-0.0.9/inductiva/client/model/task_request.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/model/task_status.py` & `inductiva-0.0.9/inductiva/client/model/task_status.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/model/validation_error.py` & `inductiva-0.0.9/inductiva/client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/models/__init__.py` & `inductiva-0.0.9/inductiva/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/paths/__init__.py` & `inductiva-0.0.9/inductiva/client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/paths/admin_user/post.py` & `inductiva-0.0.9/inductiva/client/paths/admin_user/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/paths/admin_user_username_tasks/get.py` & `inductiva-0.0.9/inductiva/client/paths/admin_user_username_tasks/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/paths/task_submit/post.py` & `inductiva-0.0.9/inductiva/client/paths/task_submit/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/paths/task_task_id_input/post.py` & `inductiva-0.0.9/inductiva/client/paths/task_task_id_input/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/paths/task_task_id_kill/post.py` & `inductiva-0.0.9/inductiva/client/paths/task_task_id_kill/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/paths/task_task_id_output/get.py` & `inductiva-0.0.9/inductiva/client/paths/task_task_id_output/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/paths/task_task_id_status/get.py` & `inductiva-0.0.9/inductiva/client/paths/task_task_id_status/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/rest.py` & `inductiva-0.0.9/inductiva/client/rest.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/client/schemas.py` & `inductiva-0.0.9/inductiva/client/schemas.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/core/math.py` & `inductiva-0.0.9/inductiva/core/math.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/__init__.py` & `inductiva-0.0.9/inductiva/fluids/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/fluid_types.py` & `inductiva-0.0.9/inductiva/fluids/fluid_types.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/post_processing/splishsplash.py` & `inductiva-0.0.9/inductiva/fluids/post_processing/splishsplash.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/scenarios/_post_processing.py` & `inductiva-0.0.9/inductiva/fluids/scenarios/_post_processing.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,18 @@
         """Initializes a `SimulationOutput` object.
 
         Args:
             sim_output_path: Path to simulation output files.
             """
         self.sim_output_dir = sim_output_path
 
-    def render(self, fps: int = 10, color: str = "blue"):
+    def render(self,
+               virtual_display: bool = True,
+               fps: int = 10,
+               color: str = "blue"):
         """Render the simulation as a movie.
 
         Args:
         fps: Number of frames per second to use in the movie. Renders a
             subset of the vtk files to create the movie.
             Default: 10.
         color: The color of the markers in the simulation.
@@ -32,14 +35,15 @@
 
         vtk_dir = os.path.join(self.sim_output_dir, "vtk")
 
         movie_path = os.path.join(self.sim_output_dir, "movie.mp4")
 
         create_movie_from_vtk(vtk_dir,
                               movie_path,
+                              virtual_display=virtual_display,
                               camera=[(3., 3., 2.), (0., 0., 0.), (1., 1., 2.)],
                               fps=fps,
                               color=color)
 
         with open(movie_path, "rb") as file_path:
             mp4 = file_path.read()
         movie_url = "data:video/mp4;base64," + b64encode(mp4).decode()
```

### Comparing `inductiva-0.0.8/inductiva/fluids/scenarios/dam_break/dam_break.py` & `inductiva-0.0.9/inductiva/fluids/scenarios/dam_break/dam_break.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/fluid_block.py` & `inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/fluid_block.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja` & `inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja` & `inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/unit_box.obj` & `inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/unit_box.obj`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py` & `inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja` & `inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py` & `inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py` & `inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/shapes.py` & `inductiva-0.0.9/inductiva/fluids/shapes.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/simulators/dualsphysics.py` & `inductiva-0.0.9/inductiva/fluids/simulators/dualsphysics.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/simulators/openfoam.py` & `inductiva-0.0.9/inductiva/fluids/simulators/openfoam.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/simulators/splishsplash.py` & `inductiva-0.0.9/inductiva/fluids/simulators/splishsplash.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/simulators/swash.py` & `inductiva-0.0.9/inductiva/fluids/simulators/swash.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/fluids/simulators/xbeach.py` & `inductiva-0.0.9/inductiva/fluids/simulators/xbeach.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/molecules/simulators/gromacs.py` & `inductiva-0.0.9/inductiva/molecules/simulators/gromacs.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/scenarios.py` & `inductiva-0.0.9/inductiva/scenarios.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/simulation/simulator.py` & `inductiva-0.0.9/inductiva/simulation/simulator.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/utils/data.py` & `inductiva-0.0.9/inductiva/utils/data.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/utils/files.py` & `inductiva-0.0.9/inductiva/utils/files.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/utils/files_test.py` & `inductiva-0.0.9/inductiva/utils/files_test.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/utils/flags.py` & `inductiva-0.0.9/inductiva/utils/flags.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/utils/meta.py` & `inductiva-0.0.9/inductiva/utils/meta.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/utils/misc_test.py` & `inductiva-0.0.9/inductiva/utils/misc_test.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/inductiva/utils/visualization.py` & `inductiva-0.0.9/inductiva/utils/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         writer.append_data(imageio.imread(frame_path))
 
     writer.close()
 
 
 def create_movie_from_vtk(vtk_output_dir: str,
                           movie_path: str,
-                          virtual_display: bool = False,
+                          virtual_display: bool = True,
                           scalars: str = None,
                           scalar_limits: Optional[List[float]] = None,
                           camera=None,
                           color: str = "blue",
                           cmap: str = None,
                           fps: int = 10) -> None:
     """Creates movie from a series of vtk files.
```

### Comparing `inductiva-0.0.8/inductiva.egg-info/PKG-INFO` & `inductiva-0.0.9/inductiva.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: inductiva
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python client for the Inductiva API
 Home-page: https://github.com/inductiva/inductiva
 Author: Inductiva Research Labs
 Author-email: contact@inductiva.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-![Python package](https://github.com/inductiva/inductiva/actions/workflows/python-package.yml/badge.svg)
+
+[![Python package](https://github.com/inductiva/inductiva/actions/workflows/python-package.yml/badge.svg)](https://github.com/inductiva/inductiva/actions/workflows/python-package.yml)
 
 ![linkedin_header](https://user-images.githubusercontent.com/104431973/231184851-0ce34289-593e-4832-aaa2-9aae652113f5.jpg)
 
 ## Large scale simulations made simple
 
 Inductiva API provides dozens of open-source physical simulation packages from your laptop. Users can start simulating right away, with no hardware setup issues and no software configuration headaches. Additionally, we provide a transparent way to scale your simulations to the next-level with one-line of code.
```

### Comparing `inductiva-0.0.8/inductiva.egg-info/SOURCES.txt` & `inductiva-0.0.9/inductiva.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.8/setup.cfg` & `inductiva-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = inductiva
-version = 0.0.8
+version = 0.0.9
 description = Python client for the Inductiva API
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Inductiva Research Labs
 author_email = contact@inductiva.ai
 url = https://github.com/inductiva/inductiva
 classifiers =
```

