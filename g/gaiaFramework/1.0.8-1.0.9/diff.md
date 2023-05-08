# Comparing `tmp/gaiaFramework-1.0.8.tar.gz` & `tmp/gaiaFramework-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gaiaFramework-1.0.8.tar", last modified: Thu Mar 30 10:29:50 2023, max compression
+gzip compressed data, was "dist\gaiaFramework-1.0.9.tar", last modified: Thu May  4 06:46:00 2023, max compression
```

## Comparing `gaiaFramework-1.0.8.tar` & `gaiaFramework-1.0.9.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:50.090350 gaiaFramework-1.0.8/
--rw-rw-rw-   0        0        0     1586 2023-03-30 10:29:50.090350 gaiaFramework-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1358 2023-03-29 15:58:50.000000 gaiaFramework-1.0.8/README.md
--rw-rw-rw-   0        0        0    28324 2023-03-30 10:27:08.000000 gaiaFramework-1.0.8/api_cli.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:49.965352 gaiaFramework-1.0.8/gaiaFramework.egg-info/
--rw-rw-rw-   0        0        0     1586 2023-03-30 10:29:49.000000 gaiaFramework-1.0.8/gaiaFramework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5400 2023-03-30 10:29:49.000000 gaiaFramework-1.0.8/gaiaFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 10:29:49.000000 gaiaFramework-1.0.8/gaiaFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-03-30 10:29:49.000000 gaiaFramework-1.0.8/gaiaFramework.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      327 2023-03-30 10:29:49.000000 gaiaFramework-1.0.8/gaiaFramework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-03-30 10:29:49.000000 gaiaFramework-1.0.8/gaiaFramework.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:49.966353 gaiaFramework-1.0.8/gaiaframework/
--rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:49.967351 gaiaFramework-1.0.8/gaiaframework/base/
--rw-rw-rw-   0        0        0      209 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/base/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:49.971352 gaiaFramework-1.0.8/gaiaframework/base/cloud_eval/
--rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/base/cloud_eval/__init__.py
--rw-rw-rw-   0        0        0     4861 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/base/cloud_eval/cloud_eval_client_base.py
--rw-rw-rw-   0        0        0     5127 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/base/cloud_eval/worker.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:49.980353 gaiaFramework-1.0.8/gaiaframework/base/common/
--rw-rw-rw-   0        0        0      237 2023-03-29 15:58:50.000000 gaiaFramework-1.0.8/gaiaframework/base/common/__init__.py
--rw-rw-rw-   0        0        0      281 2023-03-30 10:04:02.000000 gaiaFramework-1.0.8/gaiaframework/base/common/async_iterator.py
--rw-rw-rw-   0        0        0     3474 2023-03-30 09:45:57.000000 gaiaFramework-1.0.8/gaiaframework/base/common/component.py
--rw-rw-rw-   0        0        0     4781 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/base/common/functions.py
--rw-rw-rw-   0        0        0      314 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/base/common/object.py
--rw-rw-rw-   0        0        0    37143 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/base/common/regex_handler.py
--rw-rw-rw-   0        0        0     1067 2023-03-30 09:57:53.000000 gaiaFramework-1.0.8/gaiaframework/base/common/streaming_generations.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:49.983353 gaiaFramework-1.0.8/gaiaframework/base/pipeline/
--rw-rw-rw-   0        0        0      330 2023-03-29 15:58:50.000000 gaiaFramework-1.0.8/gaiaframework/base/pipeline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:49.985352 gaiaFramework-1.0.8/gaiaframework/base/pipeline/artifacts/
--rw-rw-rw-   0        0        0       89 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/base/pipeline/artifacts/__init__.py
--rw-rw-rw-   0        0        0     7906 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/base/pipeline/artifacts/shared_artifacts.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:49.986351 gaiaFramework-1.0.8/gaiaframework/base/pipeline/forcers/
--rw-rw-rw-   0        0        0       89 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/base/pipeline/forcers/__init__.py
--rw-rw-rw-   0        0        0     4623 2023-03-30 09:54:12.000000 gaiaFramework-1.0.8/gaiaframework/base/pipeline/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:49.989352 gaiaFramework-1.0.8/gaiaframework/base/pipeline/postprocessor/
--rw-rw-rw-   0        0        0       86 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/base/pipeline/postprocessor/__init__.py
--rw-rw-rw-   0        0        0     1660 2023-03-30 09:44:46.000000 gaiaFramework-1.0.8/gaiaframework/base/pipeline/postprocessor/postprocess.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:49.991352 gaiaFramework-1.0.8/gaiaframework/base/pipeline/predictables/
--rw-rw-rw-   0        0        0       83 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/base/pipeline/predictables/__init__.py
--rw-rw-rw-   0        0        0      850 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/base/pipeline/predictables/predictable.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:49.992352 gaiaFramework-1.0.8/gaiaframework/base/pipeline/predictors/
--rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/base/pipeline/predictors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:49.993353 gaiaFramework-1.0.8/gaiaframework/base/pipeline/preprocessor/
--rw-rw-rw-   0        0        0       83 2023-03-29 15:58:50.000000 gaiaFramework-1.0.8/gaiaframework/base/pipeline/preprocessor/__init__.py
--rw-rw-rw-   0        0        0     2445 2023-03-30 09:50:51.000000 gaiaFramework-1.0.8/gaiaframework/base/pipeline/preprocessor/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:49.994352 gaiaFramework-1.0.8/gaiaframework/base/server/
--rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/base/server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:49.995352 gaiaFramework-1.0.8/gaiaframework/base/testable/
--rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/base/testable/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:49.998351 gaiaFramework-1.0.8/gaiaframework/base/tester/
--rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/base/tester/__init__.py
--rw-rw-rw-   0        0        0     7535 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/base/tester/evaluator_logic.py
--rw-rw-rw-   0        0        0     6491 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/base/tester/tester_logic.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:49.999354 gaiaFramework-1.0.8/gaiaframework/base/trainer/
--rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/base/trainer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:50.016355 gaiaFramework-1.0.8/gaiaframework/cli/
--rw-rw-rw-   0        0        0     2196 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/.gitignore
--rw-rw-rw-   0        0        0      258 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/__init__.py
--rw-rw-rw-   0        0        0       84 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/allow_commands.py
--rw-rw-rw-   0        0        0      265 2023-03-27 06:15:44.000000 gaiaFramework-1.0.8/gaiaframework/cli/config.json
--rw-rw-rw-   0        0        0       65 2022-06-15 14:26:55.000000 gaiaFramework-1.0.8/gaiaframework/cli/cors_allowed_origins.json
--rw-rw-rw-   0        0        0      764 2023-03-30 09:46:44.000000 gaiaFramework-1.0.8/gaiaframework/cli/forcer_template.py
--rw-rw-rw-   0        0        0     1248 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/cli/labelizer_template.py
--rw-rw-rw-   0        0        0     2748 2023-03-29 15:58:50.000000 gaiaFramework-1.0.8/gaiaframework/cli/main_template.py
--rw-rw-rw-   0        0        0     3479 2023-03-30 10:01:09.000000 gaiaFramework-1.0.8/gaiaframework/cli/pipeline_template.py
--rw-rw-rw-   0        0        0     1570 2023-03-30 09:58:42.000000 gaiaFramework-1.0.8/gaiaframework/cli/pipeline_test_template.py
--rw-rw-rw-   0        0        0     2928 2023-03-30 09:44:46.000000 gaiaFramework-1.0.8/gaiaframework/cli/postprocess_template.py
--rw-rw-rw-   0        0        0      904 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/cli/predictable_template.py
--rw-rw-rw-   0        0        0     2283 2023-03-30 09:45:17.000000 gaiaFramework-1.0.8/gaiaframework/cli/predictor_template.py
--rw-rw-rw-   0        0        0     4184 2023-03-30 09:45:41.000000 gaiaFramework-1.0.8/gaiaframework/cli/preprocess_template.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:50.024351 gaiaFramework-1.0.8/gaiaframework/cli/schema/
--rw-rw-rw-   0        0        0      113 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/schema/__init__.py
--rw-rw-rw-   0        0        0       87 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/schema/__init___template.py
--rw-rw-rw-   0        0        0      127 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/schema/inputs_template.py
--rw-rw-rw-   0        0        0      127 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/schema/outputs_template.py
--rw-rw-rw-   0        0        0      554 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/schema/test_input_template.py
--rw-rw-rw-   0        0        0      881 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/schema/test_output_template.py
--rw-rw-rw-   0        0        0      525 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/cli/shared_artifacts_template.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:50.033351 gaiaFramework-1.0.8/gaiaframework/cli/tester/
--rw-rw-rw-   0        0        0      170 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:50.051351 gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/
--rw-rw-rw-   0        0        0      148 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/.cloud_eval_env
--rw-rw-rw-   0        0        0      301 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/Dockerfile_base
--rw-rw-rw-   0        0        0     3375 2023-02-19 16:01:10.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/Dockerfile_batch_processor
--rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/__init__.py
--rw-rw-rw-   0        0        0      581 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/auto_model_eval.sh
--rw-rw-rw-   0        0        0      184 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/batch_entrypoint.sh
--rw-rw-rw-   0        0        0      741 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/build_worker.sh
--rw-rw-rw-   0        0        0     1155 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/cloud_eval_client.py
--rw-rw-rw-   0        0        0      286 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/create_ecr_repo_if_needed.sh
--rw-rw-rw-   0        0        0      359 2023-03-27 09:49:11.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/dvc_download_artifacts_s3.sh
--rw-rw-rw-   0        0        0       87 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/eval_on_cloud.sh
--rw-rw-rw-   0        0        0     1829 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/eval_on_cloud_proc.sh
--rw-rw-rw-   0        0        0      492 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/gunicorn.conf.py
--rw-rw-rw-   0        0        0      752 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/tag_version.sh
--rw-rw-rw-   0        0        0      228 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/untag_version.sh
--rw-rw-rw-   0        0        0     1725 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/dataset_template.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:50.069352 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/
--rw-rw-rw-   0        0        0     3013 2023-02-19 16:01:09.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/Dockerfile
--rw-rw-rw-   0        0        0        0 2022-06-15 14:26:55.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/Jenkinsfile
--rw-rw-rw-   0        0        0        0 2022-06-15 14:26:55.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/Jenkinsfile_dozi
--rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:50.075353 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/deploy/
--rw-rw-rw-   0        0        0      476 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/deploy/app-gcp_gae-pr.yaml
--rw-rw-rw-   0        0        0      649 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/deploy/app-gcp_gae-prd.yaml
--rw-rw-rw-   0        0        0      421 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/deploy/app-gcp_gae-rollback.yaml
--rw-rw-rw-   0        0        0      646 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/deploy/app-gcp_gae-stg.yaml
--rw-rw-rw-   0        0        0      745 2022-06-15 14:26:55.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/deploy/jenkins.env
--rw-rw-rw-   0        0        0      234 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/docker_build_run.sh
--rw-rw-rw-   0        0        0      313 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/dvc_add.sh
--rw-rw-rw-   0        0        0      412 2023-03-29 09:05:51.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/dvc_download_artifacts.sh
--rw-rw-rw-   0        0        0      412 2023-03-29 08:32:38.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/dvc_download_artifacts_google.sh
--rw-rw-rw-   0        0        0      603 2023-03-29 09:04:57.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/dvc_init.sh
--rw-rw-rw-   0        0        0      603 2023-03-29 08:33:10.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/dvc_init_google.sh
--rw-rw-rw-   0        0        0       73 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/dvc_push.sh
--rw-rw-rw-   0        0        0      239 2023-03-27 07:13:27.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/git_init.sh
--rw-rw-rw-   0        0        0      491 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/gunicorn.conf.py
--rw-rw-rw-   0        0        0     1183 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/locustfile.py
--rw-rw-rw-   0        0        0       23 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/requirements_docker.txt
--rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/sample.csv
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:50.079352 gaiaFramework-1.0.8/gaiaframework/cli/tester/dsp/
--rw-rw-rw-   0        0        0      877 2022-06-15 14:26:55.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/dsp/add_experiment_template.py
--rw-rw-rw-   0        0        0      941 2022-06-15 14:26:55.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/dsp/get_dataset_options_template.py
--rw-rw-rw-   0        0        0      993 2023-02-19 16:02:38.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/dsp/get_model_options_template.py
--rw-rw-rw-   0        0        0      379 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/evaluator_template.py
--rw-rw-rw-   0        0        0     9122 2023-03-29 15:58:50.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/general_tester_template.py
--rw-rw-rw-   0        0        0     3578 2023-03-29 15:58:51.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/reporter_template.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:29:50.088350 gaiaFramework-1.0.8/gaiaframework/cli/tester/server/
--rw-rw-rw-   0        0        0      260 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/server/__init__.py
--rw-rw-rw-   0        0        0       71 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/server/__init___template.py
--rw-rw-rw-   0        0        0     5872 2023-03-30 10:23:30.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/server/main_template.py
--rw-rw-rw-   0        0        0      657 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/server/pool_template.py
--rw-rw-rw-   0        0        0     4105 2023-03-29 15:58:50.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/server/server_template_old.py
--rw-rw-rw-   0        0        0     1739 2023-03-30 10:26:37.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/server/test_server_post_stream_template.py
--rw-rw-rw-   0        0        0     1823 2022-06-15 12:42:01.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/server/test_server_post_template.py
--rw-rw-rw-   0        0        0     4468 2023-03-27 09:49:11.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/server/token_generator_template.py
--rw-rw-rw-   0        0        0    17998 2023-03-29 15:58:50.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/tester_template.py
--rw-rw-rw-   0        0        0      398 2023-03-29 15:58:50.000000 gaiaFramework-1.0.8/gaiaframework/cli/tester/trainer_template.py
--rw-rw-rw-   0        0        0       42 2023-03-30 10:29:50.090350 gaiaFramework-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3042 2023-03-30 10:01:20.000000 gaiaFramework-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.535242 gaiaFramework-1.0.9/
+-rw-rw-rw-   0        0        0     1586 2023-05-04 06:46:00.530213 gaiaFramework-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1358 2023-03-29 15:58:50.000000 gaiaFramework-1.0.9/README.md
+-rw-rw-rw-   0        0        0    28324 2023-03-30 10:27:08.000000 gaiaFramework-1.0.9/api_cli.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.270211 gaiaFramework-1.0.9/gaiaFramework.egg-info/
+-rw-rw-rw-   0        0        0     1586 2023-05-04 06:45:59.000000 gaiaFramework-1.0.9/gaiaFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5400 2023-05-04 06:46:00.000000 gaiaFramework-1.0.9/gaiaFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 06:45:59.000000 gaiaFramework-1.0.9/gaiaFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-05-04 06:45:59.000000 gaiaFramework-1.0.9/gaiaFramework.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      327 2023-05-04 06:45:59.000000 gaiaFramework-1.0.9/gaiaFramework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-04 06:45:59.000000 gaiaFramework-1.0.9/gaiaFramework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.275211 gaiaFramework-1.0.9/gaiaframework/
+-rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.275211 gaiaFramework-1.0.9/gaiaframework/base/
+-rw-rw-rw-   0        0        0      209 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.285211 gaiaFramework-1.0.9/gaiaframework/base/cloud_eval/
+-rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/base/cloud_eval/__init__.py
+-rw-rw-rw-   0        0        0     4861 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/base/cloud_eval/cloud_eval_client_base.py
+-rw-rw-rw-   0        0        0     5127 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/base/cloud_eval/worker.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.305214 gaiaFramework-1.0.9/gaiaframework/base/common/
+-rw-rw-rw-   0        0        0      237 2023-03-29 15:58:50.000000 gaiaFramework-1.0.9/gaiaframework/base/common/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-03-30 10:04:02.000000 gaiaFramework-1.0.9/gaiaframework/base/common/async_iterator.py
+-rw-rw-rw-   0        0        0     3474 2023-03-30 09:45:57.000000 gaiaFramework-1.0.9/gaiaframework/base/common/component.py
+-rw-rw-rw-   0        0        0     4781 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/base/common/functions.py
+-rw-rw-rw-   0        0        0      314 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/base/common/object.py
+-rw-rw-rw-   0        0        0    37143 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/base/common/regex_handler.py
+-rw-rw-rw-   0        0        0     1067 2023-03-30 09:57:53.000000 gaiaFramework-1.0.9/gaiaframework/base/common/streaming_generations.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.310214 gaiaFramework-1.0.9/gaiaframework/base/pipeline/
+-rw-rw-rw-   0        0        0      330 2023-03-29 15:58:50.000000 gaiaFramework-1.0.9/gaiaframework/base/pipeline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.315212 gaiaFramework-1.0.9/gaiaframework/base/pipeline/artifacts/
+-rw-rw-rw-   0        0        0       89 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/base/pipeline/artifacts/__init__.py
+-rw-rw-rw-   0        0        0     7906 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/base/pipeline/artifacts/shared_artifacts.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.320212 gaiaFramework-1.0.9/gaiaframework/base/pipeline/forcers/
+-rw-rw-rw-   0        0        0       89 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/base/pipeline/forcers/__init__.py
+-rw-rw-rw-   0        0        0     4623 2023-03-30 09:54:12.000000 gaiaFramework-1.0.9/gaiaframework/base/pipeline/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.320212 gaiaFramework-1.0.9/gaiaframework/base/pipeline/postprocessor/
+-rw-rw-rw-   0        0        0       86 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/base/pipeline/postprocessor/__init__.py
+-rw-rw-rw-   0        0        0     1660 2023-03-30 09:44:46.000000 gaiaFramework-1.0.9/gaiaframework/base/pipeline/postprocessor/postprocess.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.330215 gaiaFramework-1.0.9/gaiaframework/base/pipeline/predictables/
+-rw-rw-rw-   0        0        0       83 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/base/pipeline/predictables/__init__.py
+-rw-rw-rw-   0        0        0      850 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/base/pipeline/predictables/predictable.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.330215 gaiaFramework-1.0.9/gaiaframework/base/pipeline/predictors/
+-rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/base/pipeline/predictors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.335213 gaiaFramework-1.0.9/gaiaframework/base/pipeline/preprocessor/
+-rw-rw-rw-   0        0        0       83 2023-03-29 15:58:50.000000 gaiaFramework-1.0.9/gaiaframework/base/pipeline/preprocessor/__init__.py
+-rw-rw-rw-   0        0        0     2445 2023-03-30 09:50:51.000000 gaiaFramework-1.0.9/gaiaframework/base/pipeline/preprocessor/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.335213 gaiaFramework-1.0.9/gaiaframework/base/server/
+-rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/base/server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.340212 gaiaFramework-1.0.9/gaiaframework/base/testable/
+-rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/base/testable/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.345213 gaiaFramework-1.0.9/gaiaframework/base/tester/
+-rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/base/tester/__init__.py
+-rw-rw-rw-   0        0        0     7535 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/base/tester/evaluator_logic.py
+-rw-rw-rw-   0        0        0     6491 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/base/tester/tester_logic.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.345213 gaiaFramework-1.0.9/gaiaframework/base/trainer/
+-rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/base/trainer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.385214 gaiaFramework-1.0.9/gaiaframework/cli/
+-rw-rw-rw-   0        0        0     2196 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/.gitignore
+-rw-rw-rw-   0        0        0      258 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/__init__.py
+-rw-rw-rw-   0        0        0       84 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/allow_commands.py
+-rw-rw-rw-   0        0        0      265 2023-03-27 06:15:44.000000 gaiaFramework-1.0.9/gaiaframework/cli/config.json
+-rw-rw-rw-   0        0        0       65 2022-06-15 14:26:55.000000 gaiaFramework-1.0.9/gaiaframework/cli/cors_allowed_origins.json
+-rw-rw-rw-   0        0        0      764 2023-03-30 09:46:44.000000 gaiaFramework-1.0.9/gaiaframework/cli/forcer_template.py
+-rw-rw-rw-   0        0        0     1248 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/cli/labelizer_template.py
+-rw-rw-rw-   0        0        0     2748 2023-03-29 15:58:50.000000 gaiaFramework-1.0.9/gaiaframework/cli/main_template.py
+-rw-rw-rw-   0        0        0     3479 2023-03-30 10:01:09.000000 gaiaFramework-1.0.9/gaiaframework/cli/pipeline_template.py
+-rw-rw-rw-   0        0        0     1570 2023-03-30 10:48:08.000000 gaiaFramework-1.0.9/gaiaframework/cli/pipeline_test_template.py
+-rw-rw-rw-   0        0        0     2928 2023-03-30 09:44:46.000000 gaiaFramework-1.0.9/gaiaframework/cli/postprocess_template.py
+-rw-rw-rw-   0        0        0      904 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/cli/predictable_template.py
+-rw-rw-rw-   0        0        0     2283 2023-03-30 09:45:17.000000 gaiaFramework-1.0.9/gaiaframework/cli/predictor_template.py
+-rw-rw-rw-   0        0        0     4184 2023-03-30 09:45:41.000000 gaiaFramework-1.0.9/gaiaframework/cli/preprocess_template.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.400214 gaiaFramework-1.0.9/gaiaframework/cli/schema/
+-rw-rw-rw-   0        0        0      113 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/schema/__init__.py
+-rw-rw-rw-   0        0        0       87 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/schema/__init___template.py
+-rw-rw-rw-   0        0        0      127 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/schema/inputs_template.py
+-rw-rw-rw-   0        0        0      127 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/schema/outputs_template.py
+-rw-rw-rw-   0        0        0      554 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/schema/test_input_template.py
+-rw-rw-rw-   0        0        0      881 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/schema/test_output_template.py
+-rw-rw-rw-   0        0        0      525 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/cli/shared_artifacts_template.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.420212 gaiaFramework-1.0.9/gaiaframework/cli/tester/
+-rw-rw-rw-   0        0        0      170 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.455212 gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/
+-rw-rw-rw-   0        0        0      148 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/.cloud_eval_env
+-rw-rw-rw-   0        0        0      301 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/Dockerfile_base
+-rw-rw-rw-   0        0        0     3375 2023-02-19 16:01:10.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/Dockerfile_batch_processor
+-rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/__init__.py
+-rw-rw-rw-   0        0        0      581 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/auto_model_eval.sh
+-rw-rw-rw-   0        0        0      184 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/batch_entrypoint.sh
+-rw-rw-rw-   0        0        0      741 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/build_worker.sh
+-rw-rw-rw-   0        0        0     1155 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/cloud_eval_client.py
+-rw-rw-rw-   0        0        0      286 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/create_ecr_repo_if_needed.sh
+-rw-rw-rw-   0        0        0      359 2023-03-27 09:49:11.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/dvc_download_artifacts_s3.sh
+-rw-rw-rw-   0        0        0       87 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/eval_on_cloud.sh
+-rw-rw-rw-   0        0        0     1829 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/eval_on_cloud_proc.sh
+-rw-rw-rw-   0        0        0      492 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/gunicorn.conf.py
+-rw-rw-rw-   0        0        0      752 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/tag_version.sh
+-rw-rw-rw-   0        0        0      228 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/untag_version.sh
+-rw-rw-rw-   0        0        0     1725 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/dataset_template.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.495211 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/
+-rw-rw-rw-   0        0        0     3013 2023-02-19 16:01:09.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/Dockerfile
+-rw-rw-rw-   0        0        0        0 2022-06-15 14:26:55.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/Jenkinsfile
+-rw-rw-rw-   0        0        0        0 2022-06-15 14:26:55.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/Jenkinsfile_dozi
+-rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.505210 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/deploy/
+-rw-rw-rw-   0        0        0      476 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/deploy/app-gcp_gae-pr.yaml
+-rw-rw-rw-   0        0        0      649 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/deploy/app-gcp_gae-prd.yaml
+-rw-rw-rw-   0        0        0      421 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/deploy/app-gcp_gae-rollback.yaml
+-rw-rw-rw-   0        0        0      646 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/deploy/app-gcp_gae-stg.yaml
+-rw-rw-rw-   0        0        0      745 2022-06-15 14:26:55.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/deploy/jenkins.env
+-rw-rw-rw-   0        0        0      234 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/docker_build_run.sh
+-rw-rw-rw-   0        0        0      313 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/dvc_add.sh
+-rw-rw-rw-   0        0        0      412 2023-03-29 09:05:51.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/dvc_download_artifacts.sh
+-rw-rw-rw-   0        0        0      412 2023-03-29 08:32:38.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/dvc_download_artifacts_google.sh
+-rw-rw-rw-   0        0        0      603 2023-03-29 09:04:57.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/dvc_init.sh
+-rw-rw-rw-   0        0        0      603 2023-03-29 08:33:10.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/dvc_init_google.sh
+-rw-rw-rw-   0        0        0       73 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/dvc_push.sh
+-rw-rw-rw-   0        0        0      239 2023-03-27 07:13:27.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/git_init.sh
+-rw-rw-rw-   0        0        0      491 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/gunicorn.conf.py
+-rw-rw-rw-   0        0        0     1183 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/locustfile.py
+-rw-rw-rw-   0        0        0       22 2023-05-04 06:45:03.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/requirements_docker.txt
+-rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/sample.csv
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.510211 gaiaFramework-1.0.9/gaiaframework/cli/tester/dsp/
+-rw-rw-rw-   0        0        0      877 2022-06-15 14:26:55.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/dsp/add_experiment_template.py
+-rw-rw-rw-   0        0        0      941 2022-06-15 14:26:55.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/dsp/get_dataset_options_template.py
+-rw-rw-rw-   0        0        0      993 2023-02-19 16:02:38.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/dsp/get_model_options_template.py
+-rw-rw-rw-   0        0        0      379 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/evaluator_template.py
+-rw-rw-rw-   0        0        0     9122 2023-03-29 15:58:50.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/general_tester_template.py
+-rw-rw-rw-   0        0        0     3578 2023-03-29 15:58:51.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/reporter_template.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:46:00.530213 gaiaFramework-1.0.9/gaiaframework/cli/tester/server/
+-rw-rw-rw-   0        0        0      260 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/server/__init__.py
+-rw-rw-rw-   0        0        0       71 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/server/__init___template.py
+-rw-rw-rw-   0        0        0     5872 2023-03-30 10:48:25.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/server/main_template.py
+-rw-rw-rw-   0        0        0      657 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/server/pool_template.py
+-rw-rw-rw-   0        0        0     4105 2023-03-29 15:58:50.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/server/server_template_old.py
+-rw-rw-rw-   0        0        0     1739 2023-03-30 10:26:37.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/server/test_server_post_stream_template.py
+-rw-rw-rw-   0        0        0     1823 2022-06-15 12:42:01.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/server/test_server_post_template.py
+-rw-rw-rw-   0        0        0     4468 2023-03-27 09:49:11.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/server/token_generator_template.py
+-rw-rw-rw-   0        0        0    17998 2023-03-29 15:58:50.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/tester_template.py
+-rw-rw-rw-   0        0        0      398 2023-03-29 15:58:50.000000 gaiaFramework-1.0.9/gaiaframework/cli/tester/trainer_template.py
+-rw-rw-rw-   0        0        0       42 2023-05-04 06:46:00.535242 gaiaFramework-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3078 2023-05-04 06:45:03.000000 gaiaFramework-1.0.9/setup.py
```

### Comparing `gaiaFramework-1.0.8/PKG-INFO` & `gaiaFramework-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaiaFramework
-Version: 1.0.8
+Version: 1.0.9
 Summary: Data science framework library
 Home-page: UNKNOWN
 Author: oribrau@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gaiaFramework-1.0.8/README.md` & `gaiaFramework-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/api_cli.py` & `gaiaFramework-1.0.9/api_cli.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaFramework.egg-info/PKG-INFO` & `gaiaFramework-1.0.9/gaiaFramework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaiaFramework
-Version: 1.0.8
+Version: 1.0.9
 Summary: Data science framework library
 Home-page: UNKNOWN
 Author: oribrau@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gaiaFramework-1.0.8/gaiaFramework.egg-info/SOURCES.txt` & `gaiaFramework-1.0.9/gaiaFramework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/base/cloud_eval/cloud_eval_client_base.py` & `gaiaFramework-1.0.9/gaiaframework/base/cloud_eval/cloud_eval_client_base.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/base/cloud_eval/worker.py` & `gaiaFramework-1.0.9/gaiaframework/base/cloud_eval/worker.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/base/common/component.py` & `gaiaFramework-1.0.9/gaiaframework/base/common/component.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/base/common/functions.py` & `gaiaFramework-1.0.9/gaiaframework/base/common/functions.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/base/common/regex_handler.py` & `gaiaFramework-1.0.9/gaiaframework/base/common/regex_handler.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/base/common/streaming_generations.py` & `gaiaFramework-1.0.9/gaiaframework/base/common/streaming_generations.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/base/pipeline/artifacts/shared_artifacts.py` & `gaiaFramework-1.0.9/gaiaframework/base/pipeline/artifacts/shared_artifacts.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/base/pipeline/pipeline.py` & `gaiaFramework-1.0.9/gaiaframework/base/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/base/pipeline/postprocessor/postprocess.py` & `gaiaFramework-1.0.9/gaiaframework/base/pipeline/postprocessor/postprocess.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/base/pipeline/predictables/predictable.py` & `gaiaFramework-1.0.9/gaiaframework/base/pipeline/predictables/predictable.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/base/pipeline/preprocessor/preprocess.py` & `gaiaFramework-1.0.9/gaiaframework/base/pipeline/preprocessor/preprocess.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/base/tester/evaluator_logic.py` & `gaiaFramework-1.0.9/gaiaframework/base/tester/evaluator_logic.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/base/tester/tester_logic.py` & `gaiaFramework-1.0.9/gaiaframework/base/tester/tester_logic.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/.gitignore` & `gaiaFramework-1.0.9/gaiaframework/cli/.gitignore`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/forcer_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/forcer_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/labelizer_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/labelizer_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/main_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/main_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/pipeline_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/pipeline_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/pipeline_test_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/pipeline_test_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/postprocess_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/postprocess_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/predictable_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/predictable_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/predictor_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/predictor_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/preprocess_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/preprocess_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/schema/test_input_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/schema/test_input_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/schema/test_output_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/schema/test_output_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/shared_artifacts_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/shared_artifacts_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/Dockerfile_batch_processor` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/Dockerfile_batch_processor`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/auto_model_eval.sh` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/auto_model_eval.sh`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/build_worker.sh` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/build_worker.sh`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/cloud_eval_client.py` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/cloud_eval_client.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/eval_on_cloud_proc.sh` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/eval_on_cloud_proc.sh`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/cloud_eval/tag_version.sh` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/cloud_eval/tag_version.sh`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/dataset_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/dataset_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/Dockerfile` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/Dockerfile`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/deploy/app-gcp_gae-prd.yaml` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/deploy/app-gcp_gae-prd.yaml`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/deploy/app-gcp_gae-stg.yaml` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/deploy/app-gcp_gae-stg.yaml`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/deploy/jenkins.env` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/deploy/jenkins.env`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/dvc_init.sh` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/dvc_init.sh`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/dvc_init_google.sh` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/dvc_init_google.sh`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/deploy_files/locustfile.py` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/deploy_files/locustfile.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/dsp/add_experiment_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/dsp/add_experiment_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/dsp/get_dataset_options_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/dsp/get_dataset_options_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/dsp/get_model_options_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/dsp/get_model_options_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/general_tester_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/general_tester_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/reporter_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/reporter_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/server/main_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/server/main_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/server/pool_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/server/pool_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/server/server_template_old.py` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/server/server_template_old.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/server/test_server_post_stream_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/server/test_server_post_stream_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/server/test_server_post_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/server/test_server_post_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/server/token_generator_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/server/token_generator_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/gaiaframework/cli/tester/tester_template.py` & `gaiaFramework-1.0.9/gaiaframework/cli/tester/tester_template.py`

 * *Files identical despite different names*

### Comparing `gaiaFramework-1.0.8/setup.py` & `gaiaFramework-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
     def run(self):
         """After calling the super class implementation, this function removes
         the dist directory if it exists."""
         super().run()
         if os.path.exists(".eggs"):
             rmtree(".eggs")
-        if os.path.exists(f"{package_name}.egg-info"):
-            rmtree(f"{package_name}.egg-info")
+        if os.path.exists(f"{package_name.replace('-', '_')}.egg-info"):
+            rmtree(f"{package_name.replace('-', '_')}.egg-info")
         if os.path.exists("dist"):
             rmtree("dist")
 
 def package_files(directory):
     paths = []
     for (path, directories, filenames) in os.walk(directory):
         for filename in filenames:
@@ -47,15 +47,15 @@
 
     packages=find_packages(include=['gaiaframework*']),
     package_data={'': ['config.json', 'cors_allowed_origins.json', '.gitignore'] + extra_files + cloud_eval_extra_files + dsp_files},
     entry_points='''
         [console_scripts]
         gaia-cli=api_cli:cli
     ''',
-    version='1.0.8',
+    version='1.0.9',
     description='Data science framework library',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     # url='http://pypi.python.org/pypi/PackageName/',
     author='oribrau@gmail.com',
     license='MIT',
     install_requires=required,
```

