# Comparing `tmp/streamlit-nightly-1.9.3.dev20220531.tar.gz` & `tmp/streamlit-nightly-1.9.3.dev20220601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-nightly-1.9.3.dev20220531.tar", last modified: Wed Jun  1 07:01:51 2022, max compression
+gzip compressed data, was "streamlit-nightly-1.9.3.dev20220601.tar", last modified: Thu Jun  2 07:05:28 2022, max compression
```

## Comparing `streamlit-nightly-1.9.3.dev20220531.tar` & `streamlit-nightly-1.9.3.dev20220601.tar`

### file list

```diff
@@ -1,399 +1,399 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.671564 streamlit-nightly-1.9.3.dev20220531/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      108 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)      546 2022-06-01 07:01:51.671564 streamlit-nightly-1.9.3.dev20220531/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1731 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/Pipfile
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.599562 streamlit-nightly-1.9.3.dev20220531/bin/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/bin/streamlit.cmd
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-06-01 07:01:51.671564 streamlit-nightly-1.9.3.dev20220531/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3238 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.607562 streamlit-nightly-1.9.3.dev20220531/streamlit/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16714 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      841 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    28095 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/app_session.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4062 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/beta_util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13093 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/bootstrap.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.607562 streamlit-nightly-1.9.3.dev20220531/streamlit/caching/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1560 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/caching/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3426 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/caching/cache_errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11558 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/caching/cache_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12558 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/caching/hashing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16779 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/caching/memo_decorator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9718 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/caching/singleton_decorator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2229 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/case_converters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9858 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2255 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/code_util.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.607562 streamlit-nightly-1.9.3.dev20220531/streamlit/commands/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      582 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/commands/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10711 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/commands/page_config.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.607562 streamlit-nightly-1.9.3.dev20220531/streamlit/components/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      582 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/components/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.607562 streamlit-nightly-1.9.3.dev20220531/streamlit/components/v1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      979 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/components/v1/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10869 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/components/v1/component_arrow.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15672 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/components/v1/components.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    34852 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10503 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/config_option.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3898 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/config_util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8600 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5951 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/cursor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    32979 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/delta_generator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      779 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/development.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3806 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/echo.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.615563 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      582 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2803 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/alert.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12606 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/arrow.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12380 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/arrow_altair.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6215 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/arrow_vega_lite.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1279 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/balloons.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3542 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/bokeh_chart.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13754 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/button.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7898 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/camera_input.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5268 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/checkbox.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6244 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/color_picker.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17734 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/dataframe_selector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4213 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/deck_gl_json_chart.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4745 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/doc_string.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2488 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/empty.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9050 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/exception.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14457 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/file_uploader.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9356 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/form.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4080 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/graphviz_chart.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4195 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/iframe.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15127 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/image.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2903 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/json.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9343 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/layouts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12572 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/legacy_altair.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16970 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/legacy_data_frame.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6461 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/legacy_vega_lite.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.615563 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/lib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      582 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/lib/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3350 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/lib/dicttools.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6251 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/map.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9158 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/markdown.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9701 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/media.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8015 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/metric.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8602 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/multiselect.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11530 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/number_input.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7613 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/plotly_chart.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2651 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/progress.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5661 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/pyplot.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7202 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/radio.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9098 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/select_slider.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6756 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/selectbox.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20203 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/slider.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1240 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/snow.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1355 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/text.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12862 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/text_widgets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16793 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/time_widgets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2816 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9360 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/elements/write.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1722 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/env_util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3451 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/error_util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3295 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5848 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/file_util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2321 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/folder_black_list.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8766 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/forward_msg_cache.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5510 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/forward_msg_queue.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5200 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/git_util.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.615563 streamlit-nightly-1.9.3.dev20220531/streamlit/hello/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1708 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/hello/Hello.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      582 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/hello/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      957 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/hello/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11090 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/in_memory_file_manager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3591 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/js_number.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.615563 streamlit-nightly-1.9.3.dev20220531/streamlit/legacy_caching/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      830 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/legacy_caching/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25025 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/legacy_caching/caching.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35383 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/legacy_caching/hashing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3801 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/logger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5563 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/magic.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2372 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/metrics_util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2960 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/net_util.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.627563 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3854 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Alert_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2867 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/AppPage_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3282 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/ArrowNamedDataSet_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4173 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/ArrowVegaLiteChart_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4916 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Arrow_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2435 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Audio_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6014 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/BackMsg_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1993 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Balloons_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11785 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Block_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2922 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/BokehChart_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4602 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Button_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3785 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/CameraInput_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5048 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Checkbox_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3752 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/ClientState_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5138 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/ColorPicker_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12039 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Common_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14749 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Components_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    32146 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/DataFrame_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6369 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/DateInput_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3010 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/DeckGlJsonChart_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5385 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Delta_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3764 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/DocString_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4738 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/DownloadButton_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    40666 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Element_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1476 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Empty_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3782 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Exception_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1944 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Favicon_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5185 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/FileUploader_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18087 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/ForwardMsg_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5383 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/GitInfo_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3012 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/GraphVizChart_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4633 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/IFrame_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4509 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Image_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2334 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Json_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2846 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Markdown_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5997 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Metric_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5537 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/MultiSelect_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3210 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/NamedDataSet_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22754 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/NewSession_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9283 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/NumberInput_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9326 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/PageConfig_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1978 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/PageInfo_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2029 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/PageNotFound_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2322 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/PagesChanged_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5230 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/PlotlyChart_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1941 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Progress_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5833 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Radio_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1760 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/RootContainer_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5488 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Selectbox_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4305 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/SessionEvent_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2499 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/SessionState_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9129 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Slider_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1884 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Snow_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1941 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Spinner_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6391 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/TextArea_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7810 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/TextInput_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1896 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Text_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5090 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/TimeInput_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4048 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/VegaLiteChart_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3953 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Video_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12593 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/WidgetStates_pb2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      634 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    45888 2022-06-01 06:55:28.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/proto/openmetrics_data_model_pb2.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.627563 streamlit-nightly-1.9.3.dev20220531/streamlit/scriptrunner/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1034 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/scriptrunner/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6963 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/scriptrunner/script_requests.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5505 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/scriptrunner/script_run_context.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25624 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/scriptrunner/script_runner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8523 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/secrets.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.627563 streamlit-nightly-1.9.3.dev20220531/streamlit/server/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      582 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/server/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11623 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/server/routes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    29831 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/server/server.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5619 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/server/server_util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6192 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/server/upload_file_request_handler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3734 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/session_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6324 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/source_util.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.627563 streamlit-nightly-1.9.3.dev20220531/streamlit/state/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1254 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/state/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4287 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/state/safe_session_state.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24504 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/state/session_state.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4800 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/state/session_state_proxy.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10075 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/state/widgets.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.627563 streamlit-nightly-1.9.3.dev20220531/streamlit/static/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6954 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/asset-manifest.json
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.627563 streamlit-nightly-1.9.3.dev20220531/streamlit/static/assets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20638 2022-06-01 06:55:39.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/assets/streamlit.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1019 2022-06-01 06:55:39.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/favicon.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5458 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/index.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.595562 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.627563 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/css/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24409 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/css/5.71be5c0a.chunk.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)    33703 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/css/6.f5138d60.chunk.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3661 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/css/main.b46f6fce.chunk.css
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.647563 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19618 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/0.ef7179b6.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)  1003852 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/1.ea083f70.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      909 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/1.ea083f70.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)    46028 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/10.d2cd45a6.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      487 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/10.d2cd45a6.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)    66784 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/11.a36d3f16.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3144 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/12.f0ddb2c7.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4853 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/13.9142a513.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25259 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/14.4d84a801.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7580 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/15.b61c8d5b.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/15.b61c8d5b.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)    28968 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/16.ff784cb4.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1296 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/17.6db121fe.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/17.6db121fe.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15395 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/18.ab9c4fb3.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/18.ab9c4fb3.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)    86181 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/19.043576b8.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    67908 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/2.0814613e.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14901 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/20.4abf2fb8.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7519 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/21.769edc45.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/21.769edc45.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8013 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/22.d4351be2.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12890 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/23.08ec44e5.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/23.08ec44e5.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14672 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/24.43c227be.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/24.43c227be.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)  3681397 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/25.29d7e67c.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1672 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/25.29d7e67c.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1783 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/26.863c29d4.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/26.863c29d4.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8283 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/27.b4f335bf.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6390 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/28.00d19381.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/28.00d19381.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      626 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/29.c3c952bf.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/29.c3c952bf.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1141 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/30.49c473d5.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/30.49c473d5.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8314 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/31.4af97f56.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/31.4af97f56.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      630 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/32.9559ed87.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/32.9559ed87.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1356 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/33.a2ce6fbb.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/33.a2ce6fbb.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1012 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/34.1e212433.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/34.1e212433.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6539 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/35.b59c5077.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/35.b59c5077.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      991 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/36.99569331.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/36.99569331.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      620 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/37.7ef44d13.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/37.7ef44d13.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15899 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/38.62c81bdf.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1920 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/39.1f72212f.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7799 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/40.9ed83ae7.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/40.9ed83ae7.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3597 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/41.b9c54715.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      875 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/42.8c4d632a.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/42.8c4d632a.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3930 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/43.01ad2d0e.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1950 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/44.06630483.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6017 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/45.5041f7ee.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2532 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/46.c256aff5.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16428 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/47.1612ef69.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)  3357072 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/5.df97478a.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6571 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/5.df97478a.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)  2275527 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/6.fb896514.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      407 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/6.fb896514.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)   155908 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/7.a6db62e9.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       85 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/7.a6db62e9.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)   312042 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/8.1d990c70.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)  2211457 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/9.b5b265f7.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)   624104 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/main.dec7ff8d.chunk.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1231 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/main.dec7ff8d.chunk.js.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4418 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/runtime-main.16f01d5f.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.663564 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    28076 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)    63632 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_AMS-Regular.853be924.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)    33516 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12368 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fb.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6912 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90d.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7716 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12344 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d38.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6908 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7656 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa2.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13296 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501ba.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19584 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b37.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11348 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11316 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13208 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac5.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19572 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b54.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)    29912 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25324 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Bold.39890742.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)    51336 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Bold.8169508b.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16780 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19412 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    32968 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb2.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)    33580 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19676 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Italic.fd947498.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16988 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f7.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)    30772 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    53580 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26272 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Regular.f650f111.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18668 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    31196 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16400 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16440 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)    31308 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Math-Italic.8a5f9363.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18748 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Math-Italic.96759856.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24504 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f499.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12216 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a92.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14408 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458a.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12028 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d38.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14112 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfa.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22364 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12316 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19436 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10344 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10588 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Script-Regular.073b3402.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9644 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16648 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba524.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6496 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12228 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b5.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5468 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5208 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6188 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70a.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11508 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c183.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4420 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7588 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3624 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10364 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5980 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd802.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4928 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf25.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16028 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd.woff
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13568 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f7.woff2
--rw-r--r--   0 circleci  (3434) circleci  (3434)    27556 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d76.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)   191568 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceCodePro-Bold.52ac8f30.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)   155288 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceCodePro-BoldItalic.05b61807.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)   161376 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceCodePro-Italic.454577c2.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)   192740 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceCodePro-Regular.70cc7ff2.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)   191792 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceCodePro-SemiBold.4d4c53c0.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)   155568 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.2f5470bc.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)   267388 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSansPro-Bold.12e6acd2.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)    94132 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSansPro-BoldItalic.7c4f9b00.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)    94816 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSansPro-Italic.3c01996d.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)   269108 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSansPro-Regular.efa76f83.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)   268280 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSansPro-SemiBold.43cc81b4.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)    94512 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.c30987e2.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)   229740 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSerifPro-Bold.bada4fe1.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)   172748 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSerifPro-BoldItalic.9f9b1eb2.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)   169568 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSerifPro-Italic.90931d6a.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)   226812 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSerifPro-Regular.6f22301c.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)   229596 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSerifPro-SemiBold.b27cb117.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)   172816 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.1266f2c1.ttf
--rw-r--r--   0 circleci  (3434) circleci  (3434)    73528 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/flake-0.beded754.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    86179 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/flake-1.8077dc15.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    92182 2022-06-01 07:01:40.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/flake-2.e3f07d06.png
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.595562 streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.663564 streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/bokeh/
--rw-r--r--   0 circleci  (3434) circleci  (3434)   799179 2022-06-01 06:55:39.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/bokeh/bokeh-2.4.1.min.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    88828 2022-06-01 06:55:39.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/bokeh/bokeh-api-2.4.1.min.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)   185643 2022-06-01 06:55:39.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/bokeh/bokeh-gl-2.4.1.min.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)  1756732 2022-06-01 06:55:39.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/bokeh/bokeh-mathjax-2.4.1.min.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)   292438 2022-06-01 06:55:39.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/bokeh/bokeh-tables-2.4.1.min.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)   251390 2022-06-01 06:55:39.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/bokeh/bokeh-widgets-2.4.1.min.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.671564 streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/viz/
--rw-r--r--   0 circleci  (3434) circleci  (3434)  7055772 2022-06-01 06:55:39.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/viz/viz-1.8.0.min.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1063 2022-06-01 06:55:39.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/viz/viz.js-LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5322 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/stats.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3525 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/string_util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1566 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/temporary_directory.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11638 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/type_util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10904 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/uploaded_file_manager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2259 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/url_util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1098 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/user_info.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4407 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3147 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/version.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.671564 streamlit-nightly-1.9.3.dev20220531/streamlit/watcher/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/watcher/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13598 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/watcher/event_based_path_watcher.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7530 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/watcher/local_sources_watcher.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5665 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/watcher/path_watcher.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3552 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/watcher/polling_path_watcher.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5106 2022-06-01 06:51:09.000000 streamlit-nightly-1.9.3.dev20220531/streamlit/watcher/util.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:01:51.671564 streamlit-nightly-1.9.3.dev20220531/streamlit_nightly.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      546 2022-06-01 07:01:50.000000 streamlit-nightly-1.9.3.dev20220531/streamlit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16057 2022-06-01 07:01:50.000000 streamlit-nightly-1.9.3.dev20220531/streamlit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-01 07:01:50.000000 streamlit-nightly-1.9.3.dev20220531/streamlit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       50 2022-06-01 07:01:50.000000 streamlit-nightly-1.9.3.dev20220531/streamlit_nightly.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-01 06:55:36.000000 streamlit-nightly-1.9.3.dev20220531/streamlit_nightly.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      331 2022-06-01 07:01:50.000000 streamlit-nightly-1.9.3.dev20220531/streamlit_nightly.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-06-01 07:01:50.000000 streamlit-nightly-1.9.3.dev20220531/streamlit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.203282 streamlit-nightly-1.9.3.dev20220601/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      108 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      546 2022-06-02 07:05:28.203282 streamlit-nightly-1.9.3.dev20220601/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1731 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/Pipfile
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.135282 streamlit-nightly-1.9.3.dev20220601/bin/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/bin/streamlit.cmd
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-06-02 07:05:28.203282 streamlit-nightly-1.9.3.dev20220601/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3238 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.139282 streamlit-nightly-1.9.3.dev20220601/streamlit/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16714 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      841 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    28095 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/app_session.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4062 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/beta_util.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13093 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/bootstrap.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.139282 streamlit-nightly-1.9.3.dev20220601/streamlit/caching/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1560 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/caching/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3426 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/caching/cache_errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11558 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/caching/cache_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12558 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/caching/hashing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16779 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/caching/memo_decorator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9718 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/caching/singleton_decorator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2229 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/case_converters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9858 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2255 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/code_util.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.139282 streamlit-nightly-1.9.3.dev20220601/streamlit/commands/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      582 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/commands/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10711 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/commands/page_config.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.139282 streamlit-nightly-1.9.3.dev20220601/streamlit/components/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      582 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/components/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.139282 streamlit-nightly-1.9.3.dev20220601/streamlit/components/v1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      979 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/components/v1/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10869 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/components/v1/component_arrow.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15672 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/components/v1/components.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    34852 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10503 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/config_option.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3898 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/config_util.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8600 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5951 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/cursor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    32979 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/delta_generator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      779 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/development.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3806 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/echo.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.147282 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      582 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2803 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/alert.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12606 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/arrow.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12380 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/arrow_altair.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6215 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/arrow_vega_lite.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1279 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/balloons.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3542 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/bokeh_chart.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13754 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/button.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7898 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/camera_input.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5268 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/checkbox.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6244 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/color_picker.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17734 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/dataframe_selector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4213 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/deck_gl_json_chart.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4745 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/doc_string.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2488 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/empty.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9050 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/exception.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14457 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/file_uploader.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9356 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/form.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4080 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/graphviz_chart.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4195 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/iframe.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15127 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/image.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2903 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/json.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9343 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/layouts.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12572 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/legacy_altair.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16970 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/legacy_data_frame.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6461 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/legacy_vega_lite.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.147282 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/lib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      582 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/lib/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3350 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/lib/dicttools.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6251 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/map.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9158 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/markdown.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9701 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/media.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8015 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/metric.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8602 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/multiselect.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11530 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/number_input.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7613 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/plotly_chart.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2651 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/progress.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5661 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/pyplot.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7202 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/radio.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9098 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/select_slider.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6756 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/selectbox.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20203 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/slider.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1240 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/snow.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1355 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/text.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12862 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/text_widgets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16793 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/time_widgets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2816 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9360 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/elements/write.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1722 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/env_util.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3451 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/error_util.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3295 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5848 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/file_util.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2321 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/folder_black_list.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8766 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/forward_msg_cache.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5510 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/forward_msg_queue.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5200 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/git_util.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.147282 streamlit-nightly-1.9.3.dev20220601/streamlit/hello/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1708 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/hello/Hello.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      582 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/hello/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      957 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/hello/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11090 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/in_memory_file_manager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3591 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/js_number.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.147282 streamlit-nightly-1.9.3.dev20220601/streamlit/legacy_caching/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      830 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/legacy_caching/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25025 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/legacy_caching/caching.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35383 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/legacy_caching/hashing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3801 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/logger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5563 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/magic.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2372 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/metrics_util.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2960 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/net_util.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.155282 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3854 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Alert_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2867 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/AppPage_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3282 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/ArrowNamedDataSet_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4173 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/ArrowVegaLiteChart_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4916 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Arrow_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2435 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Audio_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6014 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/BackMsg_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1993 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Balloons_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11785 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Block_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2922 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/BokehChart_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4602 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Button_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3785 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/CameraInput_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5048 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Checkbox_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3752 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/ClientState_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5138 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/ColorPicker_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12039 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Common_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14749 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Components_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    32146 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/DataFrame_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6369 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/DateInput_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3010 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/DeckGlJsonChart_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5385 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Delta_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3764 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/DocString_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4738 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/DownloadButton_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    40666 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Element_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1476 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Empty_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3782 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Exception_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1944 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Favicon_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5185 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/FileUploader_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18087 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/ForwardMsg_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5383 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/GitInfo_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3012 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/GraphVizChart_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4633 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/IFrame_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4509 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Image_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2334 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Json_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2846 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Markdown_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5997 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Metric_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5537 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/MultiSelect_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3210 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/NamedDataSet_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22754 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/NewSession_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9283 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/NumberInput_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9326 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/PageConfig_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1978 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/PageInfo_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2029 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/PageNotFound_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2322 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/PagesChanged_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5230 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/PlotlyChart_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1941 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Progress_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5833 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Radio_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1760 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/RootContainer_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5488 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Selectbox_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4305 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/SessionEvent_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2499 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/SessionState_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9129 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Slider_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1884 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Snow_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1941 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Spinner_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6391 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/TextArea_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7810 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/TextInput_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1896 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Text_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5090 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/TimeInput_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4048 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/VegaLiteChart_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3953 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Video_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12593 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/WidgetStates_pb2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      634 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    45888 2022-06-02 06:58:59.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/proto/openmetrics_data_model_pb2.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.155282 streamlit-nightly-1.9.3.dev20220601/streamlit/scriptrunner/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1034 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/scriptrunner/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6963 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/scriptrunner/script_requests.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5505 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/scriptrunner/script_run_context.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25624 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/scriptrunner/script_runner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8523 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/secrets.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.155282 streamlit-nightly-1.9.3.dev20220601/streamlit/server/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      582 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/server/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11623 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/server/routes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    29831 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/server/server.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5619 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/server/server_util.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6192 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/server/upload_file_request_handler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3734 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/session_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6324 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/source_util.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.155282 streamlit-nightly-1.9.3.dev20220601/streamlit/state/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1254 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/state/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4287 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/state/safe_session_state.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    24504 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/state/session_state.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4800 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/state/session_state_proxy.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10075 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/state/widgets.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.159282 streamlit-nightly-1.9.3.dev20220601/streamlit/static/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6954 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/asset-manifest.json
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.159282 streamlit-nightly-1.9.3.dev20220601/streamlit/static/assets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20638 2022-06-02 06:59:11.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/assets/streamlit.css
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1019 2022-06-02 06:59:11.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/favicon.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5458 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/index.html
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.131282 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.159282 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/css/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    24409 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/css/5.71be5c0a.chunk.css
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    33703 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/css/6.f5138d60.chunk.css
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3661 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/css/main.b46f6fce.chunk.css
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.179282 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19618 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/0.ef7179b6.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)  1003852 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/1.ea083f70.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      909 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/1.ea083f70.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    46028 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/10.d2cd45a6.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      487 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/10.d2cd45a6.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    66784 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/11.a36d3f16.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3144 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/12.f0ddb2c7.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4853 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/13.9142a513.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25259 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/14.4d84a801.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7580 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/15.b61c8d5b.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/15.b61c8d5b.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    28968 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/16.ff784cb4.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1296 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/17.6db121fe.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/17.6db121fe.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15395 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/18.ab9c4fb3.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/18.ab9c4fb3.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    86181 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/19.043576b8.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    67908 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/2.0814613e.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14901 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/20.4abf2fb8.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7519 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/21.769edc45.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/21.769edc45.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8013 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/22.d4351be2.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12890 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/23.08ec44e5.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/23.08ec44e5.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14672 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/24.43c227be.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/24.43c227be.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)  3681397 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/25.29d7e67c.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1672 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/25.29d7e67c.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1783 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/26.863c29d4.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/26.863c29d4.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8283 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/27.b4f335bf.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6390 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/28.00d19381.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/28.00d19381.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      626 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/29.c3c952bf.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/29.c3c952bf.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1141 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/30.49c473d5.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/30.49c473d5.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8314 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/31.4af97f56.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/31.4af97f56.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      630 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/32.9559ed87.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/32.9559ed87.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1356 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/33.a2ce6fbb.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/33.a2ce6fbb.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1012 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/34.1e212433.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/34.1e212433.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6539 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/35.b59c5077.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/35.b59c5077.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      991 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/36.99569331.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/36.99569331.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      620 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/37.7ef44d13.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/37.7ef44d13.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15899 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/38.62c81bdf.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1920 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/39.1f72212f.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7799 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/40.9ed83ae7.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/40.9ed83ae7.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3597 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/41.b9c54715.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      875 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/42.8c4d632a.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/42.8c4d632a.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3930 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/43.01ad2d0e.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1950 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/44.06630483.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6017 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/45.5041f7ee.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2532 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/46.c256aff5.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16428 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/47.1612ef69.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)  3357072 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/5.df97478a.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6571 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/5.df97478a.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)  2275527 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/6.fb896514.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      407 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/6.fb896514.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   155908 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/7.a6db62e9.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       85 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/7.a6db62e9.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   312042 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/8.1d990c70.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)  2211457 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/9.b5b265f7.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   624084 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/main.468e22f6.chunk.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1231 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/main.468e22f6.chunk.js.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4418 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/runtime-main.16f01d5f.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.191282 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    28076 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    63632 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_AMS-Regular.853be924.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    33516 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12368 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fb.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6912 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90d.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7716 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12344 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d38.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6908 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7656 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa2.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13296 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501ba.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19584 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b37.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11348 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11316 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13208 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac5.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19572 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b54.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    29912 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25324 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Bold.39890742.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    51336 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Bold.8169508b.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16780 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19412 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    32968 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb2.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    33580 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19676 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Italic.fd947498.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16988 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f7.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    30772 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    53580 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26272 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Regular.f650f111.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18668 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    31196 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16400 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16440 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    31308 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Math-Italic.8a5f9363.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18748 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Math-Italic.96759856.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    24504 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f499.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12216 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a92.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14408 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458a.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12028 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d38.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14112 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfa.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22364 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12316 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19436 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10344 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10588 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Script-Regular.073b3402.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9644 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16648 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba524.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6496 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12228 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b5.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5468 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5208 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6188 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70a.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11508 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c183.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4420 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7588 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3624 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10364 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5980 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd802.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4928 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf25.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16028 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd.woff
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13568 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f7.woff2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    27556 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d76.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   191568 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceCodePro-Bold.52ac8f30.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   155288 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceCodePro-BoldItalic.05b61807.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   161376 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceCodePro-Italic.454577c2.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   192740 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceCodePro-Regular.70cc7ff2.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   191792 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceCodePro-SemiBold.4d4c53c0.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   155568 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.2f5470bc.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   267388 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSansPro-Bold.12e6acd2.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    94132 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSansPro-BoldItalic.7c4f9b00.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    94816 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSansPro-Italic.3c01996d.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   269108 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSansPro-Regular.efa76f83.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   268280 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSansPro-SemiBold.43cc81b4.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    94512 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.c30987e2.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   229740 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSerifPro-Bold.bada4fe1.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   172748 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSerifPro-BoldItalic.9f9b1eb2.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   169568 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSerifPro-Italic.90931d6a.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   226812 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSerifPro-Regular.6f22301c.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   229596 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSerifPro-SemiBold.b27cb117.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   172816 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.1266f2c1.ttf
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    73528 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/flake-0.beded754.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    86179 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/flake-1.8077dc15.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    92182 2022-06-02 07:05:18.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/flake-2.e3f07d06.png
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.135282 streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.195282 streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/bokeh/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   799179 2022-06-02 06:59:11.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/bokeh/bokeh-2.4.1.min.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    88828 2022-06-02 06:59:11.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/bokeh/bokeh-api-2.4.1.min.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   185643 2022-06-02 06:59:11.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/bokeh/bokeh-gl-2.4.1.min.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)  1756732 2022-06-02 06:59:11.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/bokeh/bokeh-mathjax-2.4.1.min.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   292438 2022-06-02 06:59:11.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/bokeh/bokeh-tables-2.4.1.min.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   251390 2022-06-02 06:59:11.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/bokeh/bokeh-widgets-2.4.1.min.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.199282 streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/viz/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)  7055772 2022-06-02 06:59:11.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/viz/viz-1.8.0.min.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1063 2022-06-02 06:59:11.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/viz/viz.js-LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5322 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/stats.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3525 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/string_util.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1566 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/temporary_directory.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11638 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/type_util.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10904 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/uploaded_file_manager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2259 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/url_util.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1373 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/user_info.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4407 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/util.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3147 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/version.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.199282 streamlit-nightly-1.9.3.dev20220601/streamlit/watcher/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/watcher/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13598 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/watcher/event_based_path_watcher.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7530 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/watcher/local_sources_watcher.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5665 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/watcher/path_watcher.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3552 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/watcher/polling_path_watcher.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5106 2022-06-02 06:54:44.000000 streamlit-nightly-1.9.3.dev20220601/streamlit/watcher/util.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-02 07:05:28.203282 streamlit-nightly-1.9.3.dev20220601/streamlit_nightly.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      546 2022-06-02 07:05:26.000000 streamlit-nightly-1.9.3.dev20220601/streamlit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16057 2022-06-02 07:05:26.000000 streamlit-nightly-1.9.3.dev20220601/streamlit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-02 07:05:26.000000 streamlit-nightly-1.9.3.dev20220601/streamlit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       50 2022-06-02 07:05:26.000000 streamlit-nightly-1.9.3.dev20220601/streamlit_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-02 06:59:07.000000 streamlit-nightly-1.9.3.dev20220601/streamlit_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      331 2022-06-02 07:05:26.000000 streamlit-nightly-1.9.3.dev20220601/streamlit_nightly.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-06-02 07:05:26.000000 streamlit-nightly-1.9.3.dev20220601/streamlit_nightly.egg-info/top_level.txt
```

### Comparing `streamlit-nightly-1.9.3.dev20220531/PKG-INFO` & `streamlit-nightly-1.9.3.dev20220601/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: streamlit-nightly
-Version: 1.9.3.dev20220531
+Version: 1.9.3.dev20220601
 Summary: The fastest way to build data apps in Python
 Home-page: https://streamlit.io
 Author: Streamlit Inc
 Author-email: hello@streamlit.io
 License: Apache 2
 Project-URL: Source, https://github.com/streamlit/streamlit
 Description: Streamlit's open-source app framework is the easiest way for data scientists and machine learning engineers to create beautiful, performant apps in only a few hours! All in pure Python. All for free.
```

### Comparing `streamlit-nightly-1.9.3.dev20220531/Pipfile` & `streamlit-nightly-1.9.3.dev20220601/Pipfile`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/setup.py` & `streamlit-nightly-1.9.3.dev20220601/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         from pipenv.utils import convert_deps_to_pip
 except:
     exit_msg = (
         "pipenv is required to package Streamlit. Please install pipenv and try again."
     )
     sys.exit(exit_msg)
 
-VERSION = "1.9.3.dev20220531"  # PEP-440
+VERSION = "1.9.3.dev20220601"  # PEP-440
 
 NAME = "streamlit-nightly"
 
 DESCRIPTION = "The fastest way to build data apps in Python"
 
 LONG_DESCRIPTION = (
     "Streamlit's open-source app framework is the easiest way "
```

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/__init__.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/__main__.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/__main__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/app_session.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/app_session.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/beta_util.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/beta_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/bootstrap.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/bootstrap.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/caching/__init__.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/caching/cache_errors.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/caching/cache_errors.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/caching/cache_utils.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/caching/cache_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/caching/hashing.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/caching/memo_decorator.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/caching/memo_decorator.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/caching/singleton_decorator.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/caching/singleton_decorator.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/case_converters.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/case_converters.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/cli.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/cli.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/code_util.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/code_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/commands/__init__.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/commands/page_config.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/commands/page_config.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/components/__init__.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/components/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/components/v1/__init__.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/components/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/components/v1/component_arrow.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/components/v1/component_arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/components/v1/components.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/components/v1/components.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/config.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/config.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/config_option.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/config_option.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/config_util.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/config_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/credentials.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/credentials.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/cursor.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/cursor.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/delta_generator.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/delta_generator.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/development.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/development.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/echo.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/echo.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/__init__.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/alert.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/alert.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/arrow.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/arrow_altair.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/arrow_altair.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/arrow_vega_lite.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/arrow_vega_lite.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/balloons.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/balloons.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/bokeh_chart.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/bokeh_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/button.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/button.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/camera_input.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/camera_input.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/checkbox.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/checkbox.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/color_picker.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/color_picker.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/dataframe_selector.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/dataframe_selector.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/deck_gl_json_chart.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/deck_gl_json_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/doc_string.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/doc_string.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/empty.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/empty.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/exception.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/exception.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/file_uploader.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/file_uploader.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/form.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/form.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/graphviz_chart.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/graphviz_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/iframe.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/iframe.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/image.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/image.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/json.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/json.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/layouts.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/layouts.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/legacy_altair.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/legacy_altair.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/legacy_data_frame.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/legacy_data_frame.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/legacy_vega_lite.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/legacy_vega_lite.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/lib/__init__.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/lib/dicttools.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/lib/dicttools.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/map.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/map.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/markdown.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/markdown.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/media.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/media.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/metric.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/metric.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/multiselect.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/multiselect.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/number_input.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/number_input.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/plotly_chart.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/progress.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/progress.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/pyplot.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/pyplot.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/radio.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/radio.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/select_slider.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/select_slider.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/selectbox.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/selectbox.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/slider.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/slider.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/snow.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/snow.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/text.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/text.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/text_widgets.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/text_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/time_widgets.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/time_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/utils.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/elements/write.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/elements/write.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/env_util.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/env_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/error_util.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/error_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/errors.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/errors.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/file_util.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/file_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/folder_black_list.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/folder_black_list.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/forward_msg_cache.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/forward_msg_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/forward_msg_queue.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/forward_msg_queue.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/git_util.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/git_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/hello/Hello.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/hello/Hello.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/hello/__init__.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/hello/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/hello/utils.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/hello/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/in_memory_file_manager.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/in_memory_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/js_number.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/js_number.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/legacy_caching/__init__.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/legacy_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/legacy_caching/caching.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/legacy_caching/caching.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/legacy_caching/hashing.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/legacy_caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/logger.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/logger.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/magic.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/magic.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/metrics_util.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/metrics_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/net_util.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/net_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Alert_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Alert_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/AppPage_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/AppPage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/ArrowNamedDataSet_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/ArrowNamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/ArrowVegaLiteChart_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/ArrowVegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Arrow_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Arrow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Audio_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Audio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/BackMsg_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/BackMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Balloons_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Balloons_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Block_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Block_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/BokehChart_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/BokehChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Button_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Button_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/CameraInput_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/CameraInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Checkbox_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Checkbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/ClientState_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/ClientState_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/ColorPicker_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/ColorPicker_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Common_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Components_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Components_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/DataFrame_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/DataFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/DateInput_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/DateInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/DeckGlJsonChart_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/DeckGlJsonChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Delta_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Delta_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/DocString_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/DocString_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/DownloadButton_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/DownloadButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Element_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Element_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Empty_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Empty_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Exception_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Exception_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Favicon_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Favicon_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/FileUploader_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/FileUploader_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/ForwardMsg_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/ForwardMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/GitInfo_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/GitInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/GraphVizChart_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/GraphVizChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/IFrame_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/IFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Image_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Image_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Json_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Json_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Markdown_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Markdown_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Metric_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Metric_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/MultiSelect_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/MultiSelect_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/NamedDataSet_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/NamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/NewSession_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/NewSession_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/NumberInput_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/NumberInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/PageConfig_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/PageConfig_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/PageInfo_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/PageInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/PageNotFound_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/PageNotFound_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/PagesChanged_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/PagesChanged_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/PlotlyChart_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/PlotlyChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Progress_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Progress_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Radio_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Radio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/RootContainer_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/RootContainer_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Selectbox_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Selectbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/SessionEvent_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/SessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/SessionState_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/SessionState_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Slider_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Slider_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Snow_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Snow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Spinner_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Spinner_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/TextArea_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/TextArea_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/TextInput_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/TextInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Text_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Text_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/TimeInput_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/TimeInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/VegaLiteChart_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/VegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/Video_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/Video_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/WidgetStates_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/WidgetStates_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/__init__.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/proto/openmetrics_data_model_pb2.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/proto/openmetrics_data_model_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/scriptrunner/__init__.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/scriptrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/scriptrunner/script_requests.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/scriptrunner/script_requests.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/scriptrunner/script_run_context.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/scriptrunner/script_run_context.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/scriptrunner/script_runner.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/scriptrunner/script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/secrets.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/secrets.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/server/__init__.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/server/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/server/routes.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/server/routes.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/server/server.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/server/server.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/server/server_util.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/server/server_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/server/upload_file_request_handler.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/server/upload_file_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/session_data.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/session_data.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/source_util.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/source_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/state/__init__.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/state/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/state/safe_session_state.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/state/safe_session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/state/session_state.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/state/session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/state/session_state_proxy.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/state/session_state_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/state/widgets.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/state/widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/asset-manifest.json` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/asset-manifest.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9092261904761905%*

 * *Differences: {"'entrypoints'": "{insert: [(4, 'static/js/main.468e22f6.chunk.js')], delete: [4]}",*

 * * "'files'": "{'main.js': './static/js/main.468e22f6.chunk.js', "*

 * *            "'static/js/main.468e22f6.chunk.js.LICENSE.txt': "*

 * *            "'./static/js/main.468e22f6.chunk.js.LICENSE.txt', delete: "*

 * *            "['static/js/main.dec7ff8d.chunk.js.LICENSE.txt']}"}*

```diff
@@ -1,19 +1,19 @@
 {
     "entrypoints": [
         "static/js/runtime-main.16f01d5f.js",
         "static/css/5.71be5c0a.chunk.css",
         "static/js/5.df97478a.chunk.js",
         "static/css/main.b46f6fce.chunk.css",
-        "static/js/main.dec7ff8d.chunk.js"
+        "static/js/main.468e22f6.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
         "main.css": "./static/css/main.b46f6fce.chunk.css",
-        "main.js": "./static/js/main.dec7ff8d.chunk.js",
+        "main.js": "./static/js/main.468e22f6.chunk.js",
         "runtime-main.js": "./static/js/runtime-main.16f01d5f.js",
         "static/css/5.71be5c0a.chunk.css": "./static/css/5.71be5c0a.chunk.css",
         "static/css/6.f5138d60.chunk.css": "./static/css/6.f5138d60.chunk.css",
         "static/js/0.ef7179b6.chunk.js": "./static/js/0.ef7179b6.chunk.js",
         "static/js/1.ea083f70.chunk.js": "./static/js/1.ea083f70.chunk.js",
         "static/js/1.ea083f70.chunk.js.LICENSE.txt": "./static/js/1.ea083f70.chunk.js.LICENSE.txt",
         "static/js/10.d2cd45a6.chunk.js": "./static/js/10.d2cd45a6.chunk.js",
@@ -80,15 +80,15 @@
         "static/js/5.df97478a.chunk.js.LICENSE.txt": "./static/js/5.df97478a.chunk.js.LICENSE.txt",
         "static/js/6.fb896514.chunk.js": "./static/js/6.fb896514.chunk.js",
         "static/js/6.fb896514.chunk.js.LICENSE.txt": "./static/js/6.fb896514.chunk.js.LICENSE.txt",
         "static/js/7.a6db62e9.chunk.js": "./static/js/7.a6db62e9.chunk.js",
         "static/js/7.a6db62e9.chunk.js.LICENSE.txt": "./static/js/7.a6db62e9.chunk.js.LICENSE.txt",
         "static/js/8.1d990c70.chunk.js": "./static/js/8.1d990c70.chunk.js",
         "static/js/9.b5b265f7.chunk.js": "./static/js/9.b5b265f7.chunk.js",
-        "static/js/main.dec7ff8d.chunk.js.LICENSE.txt": "./static/js/main.dec7ff8d.chunk.js.LICENSE.txt",
+        "static/js/main.468e22f6.chunk.js.LICENSE.txt": "./static/js/main.468e22f6.chunk.js.LICENSE.txt",
         "static/media/flake-0.beded754.png": "./static/media/flake-0.beded754.png",
         "static/media/flake-1.8077dc15.png": "./static/media/flake-1.8077dc15.png",
         "static/media/flake-2.e3f07d06.png": "./static/media/flake-2.e3f07d06.png",
         "static/media/katex.min.css": "./static/media/KaTeX_Typewriter-Regular.c5c02d76.ttf",
         "static/media/theme.scss": "./static/media/SourceSerifPro-SemiBoldItalic.1266f2c1.ttf"
     }
 }
```

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/assets/streamlit.css` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/assets/streamlit.css`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/favicon.png` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/index.html` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><title>Streamlit</title><script src="./vendor/viz/viz-1.8.0.min.js" type="javascript/worker"></script><script src="./vendor/bokeh/bokeh-2.4.1.min.js"></script><script src="./vendor/bokeh/bokeh-widgets-2.4.1.min.js"></script><script src="./vendor/bokeh/bokeh-tables-2.4.1.min.js"></script><script src="./vendor/bokeh/bokeh-api-2.4.1.min.js"></script><script src="./vendor/bokeh/bokeh-gl-2.4.1.min.js"></script><script src="./vendor/bokeh/bokeh-mathjax-2.4.1.min.js"></script><link href="./static/css/5.71be5c0a.chunk.css" rel="stylesheet"><link href="./static/css/main.b46f6fce.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var c,n,o=t[0],a=t[1],u=t[2],i=0,s=[];i<o.length;i++)n=o[i],Object.prototype.hasOwnProperty.call(f,n)&&f[n]&&s.push(f[n][0]),f[n]=0;for(c in a)Object.prototype.hasOwnProperty.call(a,c)&&(e[c]=a[c]);for(l&&l(t);s.length;)s.shift()();return d.push.apply(d,u||[]),r()}function r(){for(var e,t=0;t<d.length;t++){for(var r=d[t],c=!0,n=1;n<r.length;n++){var a=r[n];0!==f[a]&&(c=!1)}c&&(d.splice(t--,1),e=o(o.s=r[0]))}return e}var c={},n={4:0},f={4:0},d=[];function o(t){if(c[t])return c[t].exports;var r=c[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,o),r.l=!0,r.exports}o.e=function(e){var t=[];n[e]?t.push(n[e]):0!==n[e]&&{6:1}[e]&&t.push(n[e]=new Promise((function(t,r){for(var c="static/css/"+({}[e]||e)+"."+{0:"31d6cfe0",1:"31d6cfe0",2:"31d6cfe0",6:"f5138d60",7:"31d6cfe0",8:"31d6cfe0",9:"31d6cfe0",10:"31d6cfe0",11:"31d6cfe0",12:"31d6cfe0",13:"31d6cfe0",14:"31d6cfe0",15:"31d6cfe0",16:"31d6cfe0",17:"31d6cfe0",18:"31d6cfe0",19:"31d6cfe0",20:"31d6cfe0",21:"31d6cfe0",22:"31d6cfe0",23:"31d6cfe0",24:"31d6cfe0",25:"31d6cfe0",26:"31d6cfe0",27:"31d6cfe0",28:"31d6cfe0",29:"31d6cfe0",30:"31d6cfe0",31:"31d6cfe0",32:"31d6cfe0",33:"31d6cfe0",34:"31d6cfe0",35:"31d6cfe0",36:"31d6cfe0",37:"31d6cfe0",38:"31d6cfe0",39:"31d6cfe0",40:"31d6cfe0",41:"31d6cfe0",42:"31d6cfe0",43:"31d6cfe0",44:"31d6cfe0",45:"31d6cfe0",46:"31d6cfe0",47:"31d6cfe0"}[e]+".chunk.css",f=o.p+c,d=document.getElementsByTagName("link"),a=0;a<d.length;a++){var u=(l=d[a]).getAttribute("data-href")||l.getAttribute("href");if("stylesheet"===l.rel&&(u===c||u===f))return t()}var i=document.getElementsByTagName("style");for(a=0;a<i.length;a++){var l;if((u=(l=i[a]).getAttribute("data-href"))===c||u===f)return t()}var s=document.createElement("link");s.rel="stylesheet",s.type="text/css",s.onload=t,s.onerror=function(t){var c=t&&t.target&&t.target.src||f,d=new Error("Loading CSS chunk "+e+" failed.\n("+c+")");d.code="CSS_CHUNK_LOAD_FAILED",d.request=c,delete n[e],s.parentNode.removeChild(s),r(d)},s.href=f,document.getElementsByTagName("head")[0].appendChild(s)})).then((function(){n[e]=0})));var r=f[e];if(0!==r)if(r)t.push(r[2]);else{var c=new Promise((function(t,c){r=f[e]=[t,c]}));t.push(r[2]=c);var d,a=document.createElement("script");a.charset="utf-8",a.timeout=120,o.nc&&a.setAttribute("nonce",o.nc),a.src=function(e){return o.p+"static/js/"+({}[e]||e)+"."+{0:"ef7179b6",1:"ea083f70",2:"0814613e",6:"fb896514",7:"a6db62e9",8:"1d990c70",9:"b5b265f7",10:"d2cd45a6",11:"a36d3f16",12:"f0ddb2c7",13:"9142a513",14:"4d84a801",15:"b61c8d5b",16:"ff784cb4",17:"6db121fe",18:"ab9c4fb3",19:"043576b8",20:"4abf2fb8",21:"769edc45",22:"d4351be2",23:"08ec44e5",24:"43c227be",25:"29d7e67c",26:"863c29d4",27:"b4f335bf",28:"00d19381",29:"c3c952bf",30:"49c473d5",31:"4af97f56",32:"9559ed87",33:"a2ce6fbb",34:"1e212433",35:"b59c5077",36:"99569331",37:"7ef44d13",38:"62c81bdf",39:"1f72212f",40:"9ed83ae7",41:"b9c54715",42:"8c4d632a",43:"01ad2d0e",44:"06630483",45:"5041f7ee",46:"c256aff5",47:"1612ef69"}[e]+".chunk.js"}(e);var u=new Error;d=function(t){a.onerror=a.onload=null,clearTimeout(i);var r=f[e];if(0!==r){if(r){var c=t&&("load"===t.type?"missing":t.type),n=t&&t.target&&t.target.src;u.message="Loading chunk "+e+" failed.\n("+c+": "+n+")",u.name="ChunkLoadError",u.type=c,u.request=n,r[1](u)}f[e]=void 0}};var i=setTimeout((function(){d({type:"timeout",target:a})}),12e4);a.onerror=a.onload=d,document.head.appendChild(a)}return Promise.all(t)},o.m=e,o.c=c,o.d=function(e,t,r){o.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},o.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},o.t=function(e,t){if(1&t&&(e=o(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(o.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var c in e)o.d(r,c,function(t){return e[t]}.bind(null,c));return r},o.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return o.d(t,"a",t),t},o.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},o.p="./",o.oe=function(e){throw console.error(e),e};var a=this["webpackJsonpstreamlit-browser"]=this["webpackJsonpstreamlit-browser"]||[],u=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var l=u;r()}([])</script><script src="./static/js/5.df97478a.chunk.js"></script><script src="./static/js/main.dec7ff8d.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><title>Streamlit</title><script src="./vendor/viz/viz-1.8.0.min.js" type="javascript/worker"></script><script src="./vendor/bokeh/bokeh-2.4.1.min.js"></script><script src="./vendor/bokeh/bokeh-widgets-2.4.1.min.js"></script><script src="./vendor/bokeh/bokeh-tables-2.4.1.min.js"></script><script src="./vendor/bokeh/bokeh-api-2.4.1.min.js"></script><script src="./vendor/bokeh/bokeh-gl-2.4.1.min.js"></script><script src="./vendor/bokeh/bokeh-mathjax-2.4.1.min.js"></script><link href="./static/css/5.71be5c0a.chunk.css" rel="stylesheet"><link href="./static/css/main.b46f6fce.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var c,n,o=t[0],a=t[1],u=t[2],i=0,s=[];i<o.length;i++)n=o[i],Object.prototype.hasOwnProperty.call(f,n)&&f[n]&&s.push(f[n][0]),f[n]=0;for(c in a)Object.prototype.hasOwnProperty.call(a,c)&&(e[c]=a[c]);for(l&&l(t);s.length;)s.shift()();return d.push.apply(d,u||[]),r()}function r(){for(var e,t=0;t<d.length;t++){for(var r=d[t],c=!0,n=1;n<r.length;n++){var a=r[n];0!==f[a]&&(c=!1)}c&&(d.splice(t--,1),e=o(o.s=r[0]))}return e}var c={},n={4:0},f={4:0},d=[];function o(t){if(c[t])return c[t].exports;var r=c[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,o),r.l=!0,r.exports}o.e=function(e){var t=[];n[e]?t.push(n[e]):0!==n[e]&&{6:1}[e]&&t.push(n[e]=new Promise((function(t,r){for(var c="static/css/"+({}[e]||e)+"."+{0:"31d6cfe0",1:"31d6cfe0",2:"31d6cfe0",6:"f5138d60",7:"31d6cfe0",8:"31d6cfe0",9:"31d6cfe0",10:"31d6cfe0",11:"31d6cfe0",12:"31d6cfe0",13:"31d6cfe0",14:"31d6cfe0",15:"31d6cfe0",16:"31d6cfe0",17:"31d6cfe0",18:"31d6cfe0",19:"31d6cfe0",20:"31d6cfe0",21:"31d6cfe0",22:"31d6cfe0",23:"31d6cfe0",24:"31d6cfe0",25:"31d6cfe0",26:"31d6cfe0",27:"31d6cfe0",28:"31d6cfe0",29:"31d6cfe0",30:"31d6cfe0",31:"31d6cfe0",32:"31d6cfe0",33:"31d6cfe0",34:"31d6cfe0",35:"31d6cfe0",36:"31d6cfe0",37:"31d6cfe0",38:"31d6cfe0",39:"31d6cfe0",40:"31d6cfe0",41:"31d6cfe0",42:"31d6cfe0",43:"31d6cfe0",44:"31d6cfe0",45:"31d6cfe0",46:"31d6cfe0",47:"31d6cfe0"}[e]+".chunk.css",f=o.p+c,d=document.getElementsByTagName("link"),a=0;a<d.length;a++){var u=(l=d[a]).getAttribute("data-href")||l.getAttribute("href");if("stylesheet"===l.rel&&(u===c||u===f))return t()}var i=document.getElementsByTagName("style");for(a=0;a<i.length;a++){var l;if((u=(l=i[a]).getAttribute("data-href"))===c||u===f)return t()}var s=document.createElement("link");s.rel="stylesheet",s.type="text/css",s.onload=t,s.onerror=function(t){var c=t&&t.target&&t.target.src||f,d=new Error("Loading CSS chunk "+e+" failed.\n("+c+")");d.code="CSS_CHUNK_LOAD_FAILED",d.request=c,delete n[e],s.parentNode.removeChild(s),r(d)},s.href=f,document.getElementsByTagName("head")[0].appendChild(s)})).then((function(){n[e]=0})));var r=f[e];if(0!==r)if(r)t.push(r[2]);else{var c=new Promise((function(t,c){r=f[e]=[t,c]}));t.push(r[2]=c);var d,a=document.createElement("script");a.charset="utf-8",a.timeout=120,o.nc&&a.setAttribute("nonce",o.nc),a.src=function(e){return o.p+"static/js/"+({}[e]||e)+"."+{0:"ef7179b6",1:"ea083f70",2:"0814613e",6:"fb896514",7:"a6db62e9",8:"1d990c70",9:"b5b265f7",10:"d2cd45a6",11:"a36d3f16",12:"f0ddb2c7",13:"9142a513",14:"4d84a801",15:"b61c8d5b",16:"ff784cb4",17:"6db121fe",18:"ab9c4fb3",19:"043576b8",20:"4abf2fb8",21:"769edc45",22:"d4351be2",23:"08ec44e5",24:"43c227be",25:"29d7e67c",26:"863c29d4",27:"b4f335bf",28:"00d19381",29:"c3c952bf",30:"49c473d5",31:"4af97f56",32:"9559ed87",33:"a2ce6fbb",34:"1e212433",35:"b59c5077",36:"99569331",37:"7ef44d13",38:"62c81bdf",39:"1f72212f",40:"9ed83ae7",41:"b9c54715",42:"8c4d632a",43:"01ad2d0e",44:"06630483",45:"5041f7ee",46:"c256aff5",47:"1612ef69"}[e]+".chunk.js"}(e);var u=new Error;d=function(t){a.onerror=a.onload=null,clearTimeout(i);var r=f[e];if(0!==r){if(r){var c=t&&("load"===t.type?"missing":t.type),n=t&&t.target&&t.target.src;u.message="Loading chunk "+e+" failed.\n("+c+": "+n+")",u.name="ChunkLoadError",u.type=c,u.request=n,r[1](u)}f[e]=void 0}};var i=setTimeout((function(){d({type:"timeout",target:a})}),12e4);a.onerror=a.onload=d,document.head.appendChild(a)}return Promise.all(t)},o.m=e,o.c=c,o.d=function(e,t,r){o.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},o.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},o.t=function(e,t){if(1&t&&(e=o(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(o.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var c in e)o.d(r,c,function(t){return e[t]}.bind(null,c));return r},o.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return o.d(t,"a",t),t},o.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},o.p="./",o.oe=function(e){throw console.error(e),e};var a=this["webpackJsonpstreamlit-browser"]=this["webpackJsonpstreamlit-browser"]||[],u=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var l=u;r()}([])</script><script src="./static/js/5.df97478a.chunk.js"></script><script src="./static/js/main.468e22f6.chunk.js"></script></body></html>
```

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/css/5.71be5c0a.chunk.css` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/css/5.71be5c0a.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/css/6.f5138d60.chunk.css` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/css/6.f5138d60.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/css/main.b46f6fce.chunk.css` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/css/main.b46f6fce.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/0.ef7179b6.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/0.ef7179b6.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/1.ea083f70.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/1.ea083f70.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/1.ea083f70.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/1.ea083f70.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/10.d2cd45a6.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/10.d2cd45a6.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/11.a36d3f16.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/11.a36d3f16.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/12.f0ddb2c7.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/12.f0ddb2c7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/13.9142a513.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/13.9142a513.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/14.4d84a801.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/14.4d84a801.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/15.b61c8d5b.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/15.b61c8d5b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/15.b61c8d5b.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/15.b61c8d5b.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/16.ff784cb4.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/16.ff784cb4.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/17.6db121fe.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/17.6db121fe.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/17.6db121fe.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/17.6db121fe.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/18.ab9c4fb3.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/18.ab9c4fb3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/18.ab9c4fb3.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/18.ab9c4fb3.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/19.043576b8.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/19.043576b8.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/2.0814613e.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/2.0814613e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/20.4abf2fb8.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/20.4abf2fb8.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/21.769edc45.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/21.769edc45.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/21.769edc45.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/21.769edc45.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/22.d4351be2.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/22.d4351be2.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/23.08ec44e5.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/23.08ec44e5.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/23.08ec44e5.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/23.08ec44e5.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/24.43c227be.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/24.43c227be.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/24.43c227be.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/24.43c227be.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/25.29d7e67c.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/25.29d7e67c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/25.29d7e67c.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/25.29d7e67c.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/26.863c29d4.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/26.863c29d4.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/26.863c29d4.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/26.863c29d4.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/27.b4f335bf.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/27.b4f335bf.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/28.00d19381.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/28.00d19381.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/28.00d19381.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/28.00d19381.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/29.c3c952bf.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/29.c3c952bf.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/29.c3c952bf.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/29.c3c952bf.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/30.49c473d5.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/30.49c473d5.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/30.49c473d5.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/30.49c473d5.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/31.4af97f56.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/31.4af97f56.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/31.4af97f56.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/31.4af97f56.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/32.9559ed87.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/32.9559ed87.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/32.9559ed87.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/32.9559ed87.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/33.a2ce6fbb.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/33.a2ce6fbb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/33.a2ce6fbb.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/33.a2ce6fbb.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/34.1e212433.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/34.1e212433.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/34.1e212433.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/34.1e212433.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/35.b59c5077.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/35.b59c5077.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/35.b59c5077.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/35.b59c5077.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/36.99569331.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/36.99569331.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/36.99569331.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/36.99569331.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/37.7ef44d13.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/37.7ef44d13.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/37.7ef44d13.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/37.7ef44d13.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/38.62c81bdf.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/38.62c81bdf.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/39.1f72212f.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/39.1f72212f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/40.9ed83ae7.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/40.9ed83ae7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/40.9ed83ae7.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/40.9ed83ae7.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/41.b9c54715.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/41.b9c54715.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/42.8c4d632a.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/42.8c4d632a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/42.8c4d632a.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/42.8c4d632a.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/43.01ad2d0e.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/43.01ad2d0e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/44.06630483.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/44.06630483.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/45.5041f7ee.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/45.5041f7ee.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/46.c256aff5.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/46.c256aff5.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/47.1612ef69.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/47.1612ef69.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/5.df97478a.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/5.df97478a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/5.df97478a.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/5.df97478a.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/6.fb896514.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/6.fb896514.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/7.a6db62e9.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/7.a6db62e9.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/8.1d990c70.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/8.1d990c70.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/9.b5b265f7.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/9.b5b265f7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/main.dec7ff8d.chunk.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/main.468e22f6.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.dec7ff8d.chunk.js.LICENSE.txt */
+/*! For license information please see main.468e22f6.chunk.js.LICENSE.txt */
 (this["webpackJsonpstreamlit-browser"] = this["webpackJsonpstreamlit-browser"] || []).push([
     [3], {
         108: function(e, t, n) {
             "use strict";
             n.d(t, "a", (function() {
                 return $
             }));
@@ -9318,18 +9318,15 @@
                         background: t.colors.bgColor,
                         zIndex: t.zIndices.fullscreenWrapper,
                         padding: t.spacing.md,
                         paddingTop: t.sizes.headerHeight,
                         overflow: ["auto", "overlay"],
                         display: "flex",
                         alignItems: "center",
-                        justifyContent: "center",
-                        div: {
-                            margin: "auto"
-                        }
+                        justifyContent: "center"
                     } : {})
                 }), ""),
                 v = n(1),
                 j = function(e) {
                     Object(l.a)(n, e);
                     var t = Object(s.a)(n);
```

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/main.dec7ff8d.chunk.js.LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/main.468e22f6.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/js/runtime-main.16f01d5f.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/js/runtime-main.16f01d5f.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_AMS-Regular.853be924.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_AMS-Regular.853be924.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fb.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fb.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90d.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d38.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d38.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa2.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa2.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501ba.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501ba.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b37.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b37.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac5.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac5.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b54.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b54.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Bold.39890742.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Bold.39890742.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Bold.8169508b.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Bold.8169508b.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb2.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Italic.fd947498.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Italic.fd947498.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f7.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f7.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Main-Regular.f650f111.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Main-Regular.f650f111.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Math-Italic.8a5f9363.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Math-Italic.8a5f9363.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Math-Italic.96759856.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Math-Italic.96759856.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f499.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f499.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a92.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a92.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458a.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458a.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d38.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d38.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfa.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfa.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Script-Regular.073b3402.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Script-Regular.073b3402.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba524.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba524.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b5.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b5.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70a.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70a.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c183.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c183.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd802.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd802.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf25.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf25.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd.woff` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f7.woff2` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f7.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d76.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d76.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceCodePro-Bold.52ac8f30.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceCodePro-Bold.52ac8f30.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceCodePro-BoldItalic.05b61807.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceCodePro-BoldItalic.05b61807.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceCodePro-Italic.454577c2.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceCodePro-Italic.454577c2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceCodePro-Regular.70cc7ff2.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceCodePro-Regular.70cc7ff2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceCodePro-SemiBold.4d4c53c0.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceCodePro-SemiBold.4d4c53c0.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.2f5470bc.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.2f5470bc.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSansPro-Bold.12e6acd2.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSansPro-Bold.12e6acd2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSansPro-BoldItalic.7c4f9b00.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSansPro-BoldItalic.7c4f9b00.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSansPro-Italic.3c01996d.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSansPro-Italic.3c01996d.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSansPro-Regular.efa76f83.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSansPro-Regular.efa76f83.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSansPro-SemiBold.43cc81b4.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSansPro-SemiBold.43cc81b4.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.c30987e2.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.c30987e2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSerifPro-Bold.bada4fe1.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSerifPro-Bold.bada4fe1.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSerifPro-BoldItalic.9f9b1eb2.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSerifPro-BoldItalic.9f9b1eb2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSerifPro-Italic.90931d6a.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSerifPro-Italic.90931d6a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSerifPro-Regular.6f22301c.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSerifPro-Regular.6f22301c.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSerifPro-SemiBold.b27cb117.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSerifPro-SemiBold.b27cb117.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.1266f2c1.ttf` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.1266f2c1.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/flake-0.beded754.png` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/flake-0.beded754.png`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/flake-1.8077dc15.png` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/flake-1.8077dc15.png`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/static/media/flake-2.e3f07d06.png` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/static/media/flake-2.e3f07d06.png`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/bokeh/bokeh-2.4.1.min.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/bokeh/bokeh-2.4.1.min.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/bokeh/bokeh-api-2.4.1.min.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/bokeh/bokeh-api-2.4.1.min.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/bokeh/bokeh-gl-2.4.1.min.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/bokeh/bokeh-gl-2.4.1.min.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/bokeh/bokeh-mathjax-2.4.1.min.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/bokeh/bokeh-mathjax-2.4.1.min.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/bokeh/bokeh-tables-2.4.1.min.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/bokeh/bokeh-tables-2.4.1.min.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/bokeh/bokeh-widgets-2.4.1.min.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/bokeh/bokeh-widgets-2.4.1.min.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/viz/viz-1.8.0.min.js` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/viz/viz-1.8.0.min.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/static/vendor/viz/viz.js-LICENSE.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit/static/vendor/viz/viz.js-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/stats.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/stats.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/string_util.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/string_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/temporary_directory.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/temporary_directory.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/type_util.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/type_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/uploaded_file_manager.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/url_util.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/url_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/util.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/version.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/version.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/watcher/__init__.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/watcher/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/watcher/event_based_path_watcher.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/watcher/event_based_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/watcher/local_sources_watcher.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/watcher/local_sources_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/watcher/path_watcher.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/watcher/path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/watcher/polling_path_watcher.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/watcher/polling_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit/watcher/util.py` & `streamlit-nightly-1.9.3.dev20220601/streamlit/watcher/util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit_nightly.egg-info/PKG-INFO` & `streamlit-nightly-1.9.3.dev20220601/streamlit_nightly.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: streamlit-nightly
-Version: 1.9.3.dev20220531
+Version: 1.9.3.dev20220601
 Summary: The fastest way to build data apps in Python
 Home-page: https://streamlit.io
 Author: Streamlit Inc
 Author-email: hello@streamlit.io
 License: Apache 2
 Project-URL: Source, https://github.com/streamlit/streamlit
 Description: Streamlit's open-source app framework is the easiest way for data scientists and machine learning engineers to create beautiful, performant apps in only a few hours! All in pure Python. All for free.
```

### Comparing `streamlit-nightly-1.9.3.dev20220531/streamlit_nightly.egg-info/SOURCES.txt` & `streamlit-nightly-1.9.3.dev20220601/streamlit_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -260,16 +260,16 @@
 streamlit/static/static/js/5.df97478a.chunk.js.LICENSE.txt
 streamlit/static/static/js/6.fb896514.chunk.js
 streamlit/static/static/js/6.fb896514.chunk.js.LICENSE.txt
 streamlit/static/static/js/7.a6db62e9.chunk.js
 streamlit/static/static/js/7.a6db62e9.chunk.js.LICENSE.txt
 streamlit/static/static/js/8.1d990c70.chunk.js
 streamlit/static/static/js/9.b5b265f7.chunk.js
-streamlit/static/static/js/main.dec7ff8d.chunk.js
-streamlit/static/static/js/main.dec7ff8d.chunk.js.LICENSE.txt
+streamlit/static/static/js/main.468e22f6.chunk.js
+streamlit/static/static/js/main.468e22f6.chunk.js.LICENSE.txt
 streamlit/static/static/js/runtime-main.16f01d5f.js
 streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a.woff2
 streamlit/static/static/media/KaTeX_AMS-Regular.853be924.ttf
 streamlit/static/static/media/KaTeX_AMS-Regular.d562e886.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fb.ttf
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90d.woff2
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535.woff
```

