# Comparing `tmp/streamlink-5.5.0.tar.gz` & `tmp/streamlink-5.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlink-5.5.0.tar", last modified: Fri May  5 04:21:56 2023, max compression
+gzip compressed data, was "streamlink-5.5.1.tar", last modified: Mon May  8 00:33:07 2023, max compression
```

## Comparing `streamlink-5.5.0.tar` & `streamlink-5.5.1.tar`

### file list

```diff
@@ -1,575 +1,575 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.609623 streamlink-5.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-05 04:20:47.000000 streamlink-5.5.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    75451 2023-05-05 04:20:47.000000 streamlink-5.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-05 04:20:47.000000 streamlink-5.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-05 04:20:47.000000 streamlink-5.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-05 04:21:56.609623 streamlink-5.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-05 04:20:47.000000 streamlink-5.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.493620 streamlink-5.5.0/completions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.497620 streamlink-5.5.0/completions/bash/
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-05-05 04:21:38.000000 streamlink-5.5.0/completions/bash/streamlink
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.501620 streamlink-5.5.0/completions/zsh/
--rw-r--r--   0 runner    (1001) docker     (123)    33215 2023-05-05 04:21:39.000000 streamlink-5.5.0/completions/zsh/_streamlink
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-05 04:20:47.000000 streamlink-5.5.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.505620 streamlink-5.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_applications.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.493620 streamlink-5.5.0/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.505620 streamlink-5.5.0/docs/_build/man/
--rw-r--r--   0 runner    (1001) docker     (123)    37912 2023-05-05 04:21:45.000000 streamlink-5.5.0/docs/_build/man/streamlink.1
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_man.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.505620 streamlink-5.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/icon-ffmpeg.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/icon-python.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/opengraph-image.png
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.505620 streamlink-5.5.0/docs/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_static/styles/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.505620 streamlink-5.5.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_templates/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.509620 streamlink-5.5.0/docs/_templates/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_templates/sidebar/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/_templates/sidebar/github-buttons.html
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/api_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/applications.rst
--rw-r--r--   0 runner    (1001) docker     (123)    75451 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.509620 streamlink-5.5.0/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/plugin-sideloading.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.509620 streamlink-5.5.0/docs/cli/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/plugins/crunchyroll.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/plugins/twitch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/protocols.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/proxy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/deprecations.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/docutils.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/donate.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/ext_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/ext_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/ext_html_template_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/ext_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/ext_releaseref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24181 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/issues.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/players.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs/thirdparty.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-05 04:20:47.000000 streamlink-5.5.0/docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-05-05 04:20:47.000000 streamlink-5.5.0/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-05 04:20:47.000000 streamlink-5.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-05 04:21:56.609623 streamlink-5.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-05 04:20:47.000000 streamlink-5.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.493620 streamlink-5.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.613623 streamlink-5.5.0/src/streamlink/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-05 04:21:56.613623 streamlink-5.5.0/src/streamlink/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.513620 streamlink-5.5.0/src/streamlink/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/packages/requests_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.513620 streamlink-5.5.0/src/streamlink/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.517620 streamlink-5.5.0/src/streamlink/plugin/api/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/http_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/useragents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.517620 streamlink-5.5.0/src/streamlink/plugin/api/validate/
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/validate/_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/validate/_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/validate/_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/validate/_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/api/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)    25759 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.549621 streamlink-5.5.0/src/streamlink/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/abematv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/adultswim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/afreeca.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/albavision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/aloula.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/app17.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ard_live.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ard_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/artetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/atpchallenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/atresplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/bbciplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/bfmtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/bigo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/bilibili.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/blazetv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/bloomberg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/booyah.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/brightcove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/btv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/cbsnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/cdnbg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ceskatelevize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/cinergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/clubbingtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/cmmedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/cnews.py
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/crunchyroll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/dash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/delfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/deutschewelle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/dlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/dogan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/dogus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/drdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/earthcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/euronews.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/filmon.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/foxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/galatasaraytv.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/goltelevision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/goodgame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/gulli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/hiplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/hls.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/htv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/huajiao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/huya.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/idf1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/indihometv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/invintus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/kugou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/linelive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/livestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ltv_lsm_lv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/mdstrm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/mediaklikk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/mediavitrina.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/mildom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/mitele.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/mjunoon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/mrtmk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/n13tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/nhkworld.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/nicolive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/nimotv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/nos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/nownews.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/nrk.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ntv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/okru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/olympicchannel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/oneplusone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/onetv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/openrectv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/pandalive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/picarto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/piczel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/pixiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/pluto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/pluzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/qq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/radiko.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/radionet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/raiplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/reuters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/rtbf.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/rtpa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/rtpplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/rtve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/rtvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ruv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/sbscokr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/showroom.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/sportal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/sportschau.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ssh101.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/stadium.py
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/steam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/streann.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/stv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/svtplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/swisstxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/telefe.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/telemadrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tf1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/trovo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/turkuvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tv360.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tv3cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tv4play.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tv5monde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tv8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tv999.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tvibo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tviplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tvp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tvrby.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tvrplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/tvtoya.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/twitcasting.py
--rw-r--r--   0 runner    (1001) docker     (123)    26292 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ustreamtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/ustvnow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/vidio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/vimeo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/vinhlongtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/vk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/vkplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/vlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/vtvgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/wasd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/webtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/welt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/wwenetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/youtube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/yupptv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/zattoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/zdf_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/zeenews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/zengatv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/plugins/zhanqi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25474 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.549621 streamlink-5.5.0/src/streamlink/stream/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13506 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/dash.py
--rw-r--r--   0 runner    (1001) docker     (123)    34203 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/dash_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/ffmpegmux.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/filtered.py
--rw-r--r--   0 runner    (1001) docker     (123)    31062 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/hls.py
--rw-r--r--   0 runner    (1001) docker     (123)    20611 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/hls_playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/segmented.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/stream/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/user_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.553622 streamlink-5.5.0/src/streamlink/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/args.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/l10n.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/named_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/processoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.513620 streamlink-5.5.0/src/streamlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-05 04:21:56.000000 streamlink-5.5.0/src/streamlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-05-05 04:21:56.000000 streamlink-5.5.0/src/streamlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 04:21:56.000000 streamlink-5.5.0/src/streamlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 04:21:56.000000 streamlink-5.5.0/src/streamlink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-05 04:21:56.000000 streamlink-5.5.0/src/streamlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-05 04:21:56.000000 streamlink-5.5.0/src/streamlink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.553622 streamlink-5.5.0/src/streamlink_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44541 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32105 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.557622 streamlink-5.5.0/src/streamlink_cli/output/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/output/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/output/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/output/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/output/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/streamrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.557622 streamlink-5.5.0/src/streamlink_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/utils/player.py
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-05 04:20:47.000000 streamlink-5.5.0/src/streamlink_cli/utils/versioncheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.561622 streamlink-5.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.561622 streamlink-5.5.0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.561622 streamlink-5.5.0/tests/cli/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/output/test_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/output/test_playeroutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_cmdline_player_fifo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_cmdline_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    38283 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_main_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_main_setup_config_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    23059 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/test_streamrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.565622 streamlink-5.5.0/tests/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/utils/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/utils/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/cli/utils/test_versioncheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.565622 streamlink-5.5.0/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/mixins/stream_hls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.565622 streamlink-5.5.0/tests/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.565622 streamlink-5.5.0/tests/plugin/override/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugin/override/testplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugin/testplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugin/testplugin_invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugin/testplugin_missing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.597623 streamlink-5.5.0/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_abematv.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_adultswim.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_afreeca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_albavision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_aloula.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_app17.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ard_live.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ard_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_artetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_atpchallenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_atresplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_bbciplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_bfmtv.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_bigo.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_bilibili.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_blazetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_bloomberg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_booyah.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_brightcove.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_btv.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_cbsnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_cdnbg.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ceskatelevize.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_cinergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_clubbingtv.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_cmmedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_cnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_crunchyroll.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_delfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_deutschewelle.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_dlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_dogan.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_dogus.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_drdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_earthcam.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_euronews.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_filmon.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_foxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_galatasaraytv.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_goltelevision.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_goodgame.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_googledrive.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_gulli.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_hiplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_htv.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_huajiao.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_huya.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_idf1.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_indihometv.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_invintus.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_kugou.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_linelive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_livestream.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ltv_lsm_lv.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_mdstrm.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_mediaklikk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_mediavitrina.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_mildom.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_mitele.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_mjunoon.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_mrtmk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_n13tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_nhkworld.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_nicolive.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_nimotv.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_nos.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_nownews.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_nrk.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ntv.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_okru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_olympicchannel.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_oneplusone.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_onetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_openrectv.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_pandalive.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_picarto.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_piczel.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_pixiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_pluto.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_pluzz.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_qq.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_radiko.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_radionet.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_raiplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_reuters.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_rtbf.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_rtpa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_rtpplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_rtve.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_rtvs.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ruv.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_sbscokr.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_showroom.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_sportal.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_sportschau.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ssh101.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_stadium.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_steam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_streann.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_stv.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_svtplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_swisstxt.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_telefe.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_telemadrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tf1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_trovo.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_turkuvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tv360.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tv3cat.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tv4play.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tv5monde.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tv8.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tv999.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tvibo.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tviplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tvp.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tvrby.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tvrplus.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_tvtoya.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_twitcasting.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ustreamtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_ustvnow.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_vidio.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_vimeo.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_vinhlongtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_vk.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_vkplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_vlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_vtvgo.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_wasd.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_webtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_welt.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_wwenetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_youtube.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_yupptv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_zattoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_zdf_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_zeenews.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_zengatv.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/plugins/test_zhanqi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.597623 streamlink-5.5.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.497620 streamlink-5.5.0/tests/resources/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.601623 streamlink-5.5.0/tests/resources/cli/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/cli/config/custom
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/cli/config/primary
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/cli/config/primary.testplugin
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/cli/config/secondary
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/cli/config/secondary.testplugin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.601623 streamlink-5.5.0/tests/resources/dash/
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_1.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_10.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_11_static.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_2.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_3.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_8.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_9.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_nested_baseurls.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_no_segment_list_or_template.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_segment_list.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_segments_byterange.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_segments_dynamic_number.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_static_no_publish_time.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/dash/test_timeline_ids.mpd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.605623 streamlink-5.5.0/tests/resources/hls/
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/hls/test_1.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/hls/test_2.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/hls/test_date.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/hls/test_master.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/resources/hls/test_master_twitch_vod.m3u8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.605623 streamlink-5.5.0/tests/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_dash_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_ffmpegmux.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    29307 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_hls_filtered.py
--rw-r--r--   0 runner    (1001) docker     (123)    18847 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_hls_playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_stream_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_stream_to_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/stream/test_stream_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_api_http_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    48733 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_api_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_api_websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10255 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_plugin_userinput.py
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23342 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/test_streamlink_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.609623 streamlink-5.5.0/tests/testutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/testutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/testutils/handshake.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/testutils/test_handshake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:56.609623 streamlink-5.5.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_l10n.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_named_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_processoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-05 04:20:47.000000 streamlink-5.5.0/tests/utils/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.068640 streamlink-5.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-08 00:32:02.000000 streamlink-5.5.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    75916 2023-05-08 00:32:02.000000 streamlink-5.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-08 00:32:02.000000 streamlink-5.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-08 00:32:02.000000 streamlink-5.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-08 00:33:07.068640 streamlink-5.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-08 00:32:02.000000 streamlink-5.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.952640 streamlink-5.5.1/completions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.960640 streamlink-5.5.1/completions/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-05-08 00:32:50.000000 streamlink-5.5.1/completions/bash/streamlink
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.960640 streamlink-5.5.1/completions/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)    33215 2023-05-08 00:32:50.000000 streamlink-5.5.1/completions/zsh/_streamlink
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-08 00:32:02.000000 streamlink-5.5.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.964640 streamlink-5.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_applications.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.952640 streamlink-5.5.1/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.964640 streamlink-5.5.1/docs/_build/man/
+-rw-r--r--   0 runner    (1001) docker     (123)    37912 2023-05-08 00:32:56.000000 streamlink-5.5.1/docs/_build/man/streamlink.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_man.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.964640 streamlink-5.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/icon-ffmpeg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/icon-python.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/opengraph-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.964640 streamlink-5.5.1/docs/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/styles/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.964640 streamlink-5.5.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.964640 streamlink-5.5.1/docs/_templates/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_templates/sidebar/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_templates/sidebar/github-buttons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/api_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/applications.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    75916 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.968640 streamlink-5.5.1/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/plugin-sideloading.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.968640 streamlink-5.5.1/docs/cli/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/plugins/crunchyroll.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/plugins/twitch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/protocols.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/proxy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/deprecations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/docutils.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/donate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/ext_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/ext_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/ext_html_template_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/ext_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/ext_releaseref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24181 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/issues.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/players.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/thirdparty.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-05-08 00:32:02.000000 streamlink-5.5.1/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-08 00:32:02.000000 streamlink-5.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-08 00:33:07.072640 streamlink-5.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-08 00:32:02.000000 streamlink-5.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.952640 streamlink-5.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.076640 streamlink-5.5.1/src/streamlink/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-08 00:33:07.076640 streamlink-5.5.1/src/streamlink/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.972640 streamlink-5.5.1/src/streamlink/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/packages/requests_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.972640 streamlink-5.5.1/src/streamlink/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.972640 streamlink-5.5.1/src/streamlink/plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/http_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/useragents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.972640 streamlink-5.5.1/src/streamlink/plugin/api/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/validate/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/validate/_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/validate/_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/validate/_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25759 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.004640 streamlink-5.5.1/src/streamlink/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/abematv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/adultswim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/afreeca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/albavision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/aloula.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/app17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ard_live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ard_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/artetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/atpchallenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/atresplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/bbciplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/bfmtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/bigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/bilibili.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/blazetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/bloomberg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/booyah.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/brightcove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/btv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/cbsnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/cdnbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ceskatelevize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/cinergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/clubbingtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/cmmedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/cnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/crunchyroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/delfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/deutschewelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/dlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/dogan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/dogus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/drdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/earthcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/euronews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/filmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/foxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/galatasaraytv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/goltelevision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/goodgame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/gulli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/hiplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/htv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/huajiao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/huya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/idf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/indihometv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/invintus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/kugou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/linelive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/livestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ltv_lsm_lv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/mdstrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/mediaklikk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/mediavitrina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/mildom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/mitele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/mjunoon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/mrtmk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/n13tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/nhkworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/nicolive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/nimotv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/nos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/nownews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/nrk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ntv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/okru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/olympicchannel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/oneplusone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/onetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/openrectv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/pandalive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/picarto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/piczel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/pixiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/pluto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/pluzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/qq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/radiko.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/radionet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/raiplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/reuters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/rtbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/rtpa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/rtpplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/rtve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/rtvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ruv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/sbscokr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/showroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/sportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/sportschau.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ssh101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/stadium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/steam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/streann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/stv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/svtplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/swisstxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/telefe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/telemadrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/trovo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/turkuvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tv360.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tv3cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tv4play.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tv5monde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tv8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tv999.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tvibo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tviplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tvrby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tvrplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tvtoya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/twitcasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26292 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ustreamtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ustvnow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/vidio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/vinhlongtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/vk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/vkplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/vlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/vtvgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/wasd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/webtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/welt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/wwenetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/yupptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/zattoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/zdf_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/zeenews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/zengatv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/zhanqi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25474 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.008640 streamlink-5.5.1/src/streamlink/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13506 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34203 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/dash_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/ffmpegmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/filtered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32100 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20611 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/hls_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/segmented.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/user_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.012640 streamlink-5.5.1/src/streamlink/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/l10n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/named_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/processoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.972640 streamlink-5.5.1/src/streamlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-08 00:33:06.000000 streamlink-5.5.1/src/streamlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-05-08 00:33:06.000000 streamlink-5.5.1/src/streamlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 00:33:06.000000 streamlink-5.5.1/src/streamlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 00:33:06.000000 streamlink-5.5.1/src/streamlink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-08 00:33:06.000000 streamlink-5.5.1/src/streamlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-08 00:33:06.000000 streamlink-5.5.1/src/streamlink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.012640 streamlink-5.5.1/src/streamlink_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44541 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32105 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.016640 streamlink-5.5.1/src/streamlink_cli/output/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/output/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/output/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/output/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/output/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/streamrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.016640 streamlink-5.5.1/src/streamlink_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/utils/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/utils/versioncheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.020640 streamlink-5.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.020640 streamlink-5.5.1/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.020640 streamlink-5.5.1/tests/cli/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/output/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/output/test_playeroutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_cmdline_player_fifo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_cmdline_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38283 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_main_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_main_setup_config_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23059 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_streamrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.024640 streamlink-5.5.1/tests/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/utils/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/utils/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/utils/test_versioncheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.024640 streamlink-5.5.1/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/mixins/stream_hls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.024640 streamlink-5.5.1/tests/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.024640 streamlink-5.5.1/tests/plugin/override/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugin/override/testplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugin/testplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugin/testplugin_invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugin/testplugin_missing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.056640 streamlink-5.5.1/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_abematv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_adultswim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_afreeca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_albavision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_aloula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_app17.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ard_live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ard_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_artetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_atpchallenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_atresplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_bbciplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_bfmtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_bigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_bilibili.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_blazetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_bloomberg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_booyah.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_brightcove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_btv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_cbsnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_cdnbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ceskatelevize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_cinergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_clubbingtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_cmmedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_cnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_crunchyroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_delfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_deutschewelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_dlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_dogan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_dogus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_drdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_earthcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_euronews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_filmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_foxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_galatasaraytv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_goltelevision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_goodgame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_gulli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_hiplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_htv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_huajiao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_huya.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_idf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_indihometv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_invintus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_kugou.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_linelive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_livestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ltv_lsm_lv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_mdstrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_mediaklikk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_mediavitrina.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_mildom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_mitele.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_mjunoon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_mrtmk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_n13tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_nhkworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_nicolive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_nimotv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_nos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_nownews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_nrk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ntv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_okru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_olympicchannel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_oneplusone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_onetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_openrectv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_pandalive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_picarto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_piczel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_pixiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_pluto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_pluzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_qq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_radiko.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_radionet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_raiplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_reuters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_rtbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_rtpa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_rtpplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_rtve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_rtvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ruv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_sbscokr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_showroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_sportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_sportschau.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ssh101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_stadium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_steam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_streann.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_stv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_svtplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_swisstxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_telefe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_telemadrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_trovo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_turkuvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tv360.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tv3cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tv4play.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tv5monde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tv8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tv999.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tvibo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tviplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tvrby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tvrplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tvtoya.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_twitcasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ustreamtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ustvnow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_vidio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_vinhlongtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_vk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_vkplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_vlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_vtvgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_wasd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_webtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_welt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_wwenetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_yupptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_zattoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_zdf_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_zeenews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_zengatv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_zhanqi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.056640 streamlink-5.5.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.956640 streamlink-5.5.1/tests/resources/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.056640 streamlink-5.5.1/tests/resources/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/cli/config/custom
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/cli/config/primary
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/cli/config/primary.testplugin
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/cli/config/secondary
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/cli/config/secondary.testplugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.060640 streamlink-5.5.1/tests/resources/dash/
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_1.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_10.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_11_static.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_2.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_3.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_8.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_9.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_nested_baseurls.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_no_segment_list_or_template.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_segment_list.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_segments_byterange.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_segments_dynamic_number.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_static_no_publish_time.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_timeline_ids.mpd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.060640 streamlink-5.5.1/tests/resources/hls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/hls/test_1.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/hls/test_2.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/hls/test_date.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/hls/test_master.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/hls/test_master_twitch_vod.m3u8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.064640 streamlink-5.5.1/tests/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_dash_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_ffmpegmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_hls_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18847 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_hls_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_stream_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_stream_to_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_stream_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/test_api_http_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48733 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/test_api_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/test_api_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10255 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_plugin_userinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23342 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_streamlink_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.068640 streamlink-5.5.1/tests/testutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/testutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/testutils/handshake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/testutils/test_handshake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.068640 streamlink-5.5.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_l10n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_named_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_processoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_url.py
```

### Comparing `streamlink-5.5.0/CHANGELOG.md` & `streamlink-5.5.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Changelog
 
+## streamlink 5.5.1 (2023-05-08)
+
+Patch release:
+
+- Fixed: shifting time offset when reloading HLS playlists ([#5321](https://github.com/streamlink/streamlink/pull/5321))
+- Fixed: import of `create_urllib3_context` on `urllib3 <2.0.0` ([#5333](https://github.com/streamlink/streamlink/pull/5333))
+- Fixed: Vimeo plugin ([#5331](https://github.com/streamlink/streamlink/pull/5331))
+
+[Full changelog](https://github.com/streamlink/streamlink/compare/5.5.0...5.5.1)
+
+
 ## streamlink 5.5.0 (2023-05-05)
 
 Release highlights:
 
 - Added: `--no-config` ([#5314](https://github.com/streamlink/streamlink/pull/5314))
 - Added: `--player-external-http-interface` ([#5295](https://github.com/streamlink/streamlink/pull/5295))
 - Fixed: M3U8 attribute parsing issue ([#5307](https://github.com/streamlink/streamlink/pull/5307))
```

### Comparing `streamlink-5.5.0/LICENSE` & `streamlink-5.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/PKG-INFO` & `streamlink-5.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink
-Version: 5.5.0
+Version: 5.5.1
 Summary: Streamlink is a command-line utility that extracts streams from various services and pipes them into a video player of choice.
 Home-page: https://github.com/streamlink/streamlink
 Author: Streamlink
 Author-email: streamlink@protonmail.com
 License: Simplified BSD
 Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlink Version: 5.5.0 Summary: Streamlink is a
+Metadata-Version: 2.1 Name: streamlink Version: 5.5.1 Summary: Streamlink is a
 command-line utility that extracts streams from various services and pipes them
 into a video player of choice. Home-page: https://github.com/streamlink/
 streamlink Author: Streamlink Author-email: streamlink@protonmail.com License:
 Simplified BSD Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues Project-
 URL: Source, https://github.com/streamlink/streamlink Project-URL: Funding,
 https://streamlink.github.io/latest/donate.html Classifier: Development Status
```

### Comparing `streamlink-5.5.0/README.md` & `streamlink-5.5.1/README.md`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/completions/bash/streamlink` & `streamlink-5.5.1/completions/bash/streamlink`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/completions/zsh/_streamlink` & `streamlink-5.5.1/completions/zsh/_streamlink`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/Makefile` & `streamlink-5.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/_build/man/streamlink.1` & `streamlink-5.5.1/docs/_build/man/streamlink.1`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "STREAMLINK" "1" "May 05, 2023" "5.5.0" "Streamlink"
+.TH "STREAMLINK" "1" "May 08, 2023" "5.5.1" "Streamlink"
 .SH NAME
 streamlink \- extracts streams from various services and pipes them into a video player of choice
 .SH SYNOPSIS
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
```

### Comparing `streamlink-5.5.0/docs/_man.rst` & `streamlink-5.5.1/docs/_man.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/_static/apple-touch-icon.png` & `streamlink-5.5.1/docs/_static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/_static/favicon-16x16.png` & `streamlink-5.5.1/docs/_static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/_static/favicon-32x32.png` & `streamlink-5.5.1/docs/_static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/_static/favicon.ico` & `streamlink-5.5.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/_static/icon-ffmpeg.svg` & `streamlink-5.5.1/docs/_static/icon-ffmpeg.svg`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/_static/icon-python.svg` & `streamlink-5.5.1/docs/_static/icon-python.svg`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/_static/icon.svg` & `streamlink-5.5.1/docs/_static/icon.svg`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/_static/opengraph-image.png` & `streamlink-5.5.1/docs/_static/opengraph-image.png`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/_static/styles/custom.css` & `streamlink-5.5.1/docs/_static/styles/custom.css`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/_templates/base.html` & `streamlink-5.5.1/docs/_templates/base.html`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/_templates/sidebar/brand.html` & `streamlink-5.5.1/docs/_templates/sidebar/brand.html`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/_templates/sidebar/github-buttons.html` & `streamlink-5.5.1/docs/_templates/sidebar/github-buttons.html`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/api.rst` & `streamlink-5.5.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/api_guide.rst` & `streamlink-5.5.1/docs/api_guide.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/applications.rst` & `streamlink-5.5.1/docs/applications.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/changelog.md` & `streamlink-5.5.1/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Changelog
 
+## streamlink 5.5.1 (2023-05-08)
+
+Patch release:
+
+- Fixed: shifting time offset when reloading HLS playlists ([#5321](https://github.com/streamlink/streamlink/pull/5321))
+- Fixed: import of `create_urllib3_context` on `urllib3 <2.0.0` ([#5333](https://github.com/streamlink/streamlink/pull/5333))
+- Fixed: Vimeo plugin ([#5331](https://github.com/streamlink/streamlink/pull/5331))
+
+[Full changelog](https://github.com/streamlink/streamlink/compare/5.5.0...5.5.1)
+
+
 ## streamlink 5.5.0 (2023-05-05)
 
 Release highlights:
 
 - Added: `--no-config` ([#5314](https://github.com/streamlink/streamlink/pull/5314))
 - Added: `--player-external-http-interface` ([#5295](https://github.com/streamlink/streamlink/pull/5295))
 - Fixed: M3U8 attribute parsing issue ([#5307](https://github.com/streamlink/streamlink/pull/5307))
```

### Comparing `streamlink-5.5.0/docs/cli/config.rst` & `streamlink-5.5.1/docs/cli/config.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/cli/metadata.rst` & `streamlink-5.5.1/docs/cli/metadata.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/cli/plugin-sideloading.rst` & `streamlink-5.5.1/docs/cli/plugin-sideloading.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/cli/plugins/crunchyroll.rst` & `streamlink-5.5.1/docs/cli/plugins/crunchyroll.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/cli/plugins/twitch.rst` & `streamlink-5.5.1/docs/cli/plugins/twitch.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/cli/protocols.rst` & `streamlink-5.5.1/docs/cli/protocols.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/cli/proxy.rst` & `streamlink-5.5.1/docs/cli/proxy.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/cli/tutorial.rst` & `streamlink-5.5.1/docs/cli/tutorial.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/cli.rst` & `streamlink-5.5.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/conf.py` & `streamlink-5.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/deprecations.rst` & `streamlink-5.5.1/docs/deprecations.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/developing.rst` & `streamlink-5.5.1/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/donate.rst` & `streamlink-5.5.1/docs/donate.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/ext_argparse.py` & `streamlink-5.5.1/docs/ext_argparse.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/ext_github.py` & `streamlink-5.5.1/docs/ext_github.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/ext_plugins.py` & `streamlink-5.5.1/docs/ext_plugins.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/ext_releaseref.py` & `streamlink-5.5.1/docs/ext_releaseref.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/index.rst` & `streamlink-5.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/install.rst` & `streamlink-5.5.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/issues.rst` & `streamlink-5.5.1/docs/issues.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/players.rst` & `streamlink-5.5.1/docs/players.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/docs/thirdparty.rst` & `streamlink-5.5.1/docs/thirdparty.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/icon.svg` & `streamlink-5.5.1/icon.svg`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/pyproject.toml` & `streamlink-5.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/setup.cfg` & `streamlink-5.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/setup.py` & `streamlink-5.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/__init__.py` & `streamlink-5.5.1/src/streamlink/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/_version.py` & `streamlink-5.5.1/src/streamlink/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
     return get_version(
         project_dir=Path(streamlink.__file__).parents[2],
     )
 
 
 # The following _get_version() call will get replaced by versioningit with a static version string when building streamlink
 # `pip install .` / `pip wheel .` / `python setup.py build` / `python setup.py bdist_wheel` / etc.
-__version__ = "5.5.0"
+__version__ = "5.5.1"
```

### Comparing `streamlink-5.5.0/src/streamlink/api.py` & `streamlink-5.5.1/src/streamlink/api.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/buffers.py` & `streamlink-5.5.1/src/streamlink/buffers.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/cache.py` & `streamlink-5.5.1/src/streamlink/cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/exceptions.py` & `streamlink-5.5.1/src/streamlink/exceptions.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/logger.py` & `streamlink-5.5.1/src/streamlink/logger.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/options.py` & `streamlink-5.5.1/src/streamlink/options.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/packages/requests_file.py` & `streamlink-5.5.1/src/streamlink/packages/requests_file.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugin/__init__.py` & `streamlink-5.5.1/src/streamlink/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugin/api/http_session.py` & `streamlink-5.5.1/src/streamlink/plugin/api/http_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 
 from streamlink.exceptions import PluginError
 from streamlink.packages.requests_file import FileAdapter
 from streamlink.plugin.api import useragents
 from streamlink.utils.parse import parse_json, parse_xml
 
 
+try:
+    from urllib3.util import create_urllib3_context  # type: ignore[attr-defined]
+except ImportError:  # pragma: no cover
+    # urllib3 <2.0.0 compat import
+    from urllib3.util.ssl_ import create_urllib3_context
+
+
 # urllib3>=2.0.0: enforce_content_length now defaults to True (keep the override for backwards compatibility)
 class _HTTPResponse(urllib3.response.HTTPResponse):
     def __init__(self, *args, **kwargs):
         # Always enforce content length validation!
         # This fixes a bug in requests which doesn't raise errors on HTTP responses where
         # the "Content-Length" header doesn't match the response's body length.
         # https://github.com/psf/requests/issues/4956#issuecomment-573325001
@@ -184,26 +191,26 @@
             res = schema.validate(res.text, name="response text", exception=PluginError)
 
         return res
 
 
 class TLSNoDHAdapter(HTTPAdapter):
     def init_poolmanager(self, *args, **kwargs):
-        ctx = urllib3.util.create_urllib3_context()
+        ctx = create_urllib3_context()
         ctx.load_default_certs()
         ciphers = ":".join(cipher.get("name") for cipher in ctx.get_ciphers())
         ciphers += ":!DH"
         ctx.set_ciphers(ciphers)
         kwargs["ssl_context"] = ctx
         return super().init_poolmanager(*args, **kwargs)
 
 
 class TLSSecLevel1Adapter(HTTPAdapter):
     def init_poolmanager(self, *args, **kwargs):
-        ctx = urllib3.util.create_urllib3_context()
+        ctx = create_urllib3_context()
         ctx.load_default_certs()
         ctx.set_ciphers("DEFAULT:@SECLEVEL=1")
         kwargs["ssl_context"] = ctx
         return super().init_poolmanager(*args, **kwargs)
 
 
 __all__ = ["HTTPSession", "TLSNoDHAdapter", "TLSSecLevel1Adapter"]
```

### Comparing `streamlink-5.5.0/src/streamlink/plugin/api/useragents.py` & `streamlink-5.5.1/src/streamlink/plugin/api/useragents.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugin/api/validate/__init__.py` & `streamlink-5.5.1/src/streamlink/plugin/api/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugin/api/validate/_exception.py` & `streamlink-5.5.1/src/streamlink/plugin/api/validate/_exception.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugin/api/validate/_schemas.py` & `streamlink-5.5.1/src/streamlink/plugin/api/validate/_schemas.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugin/api/validate/_validate.py` & `streamlink-5.5.1/src/streamlink/plugin/api/validate/_validate.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugin/api/validate/_validators.py` & `streamlink-5.5.1/src/streamlink/plugin/api/validate/_validators.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugin/api/websocket.py` & `streamlink-5.5.1/src/streamlink/plugin/api/websocket.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugin/plugin.py` & `streamlink-5.5.1/src/streamlink/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/abematv.py` & `streamlink-5.5.1/src/streamlink/plugins/abematv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/adultswim.py` & `streamlink-5.5.1/src/streamlink/plugins/adultswim.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/afreeca.py` & `streamlink-5.5.1/src/streamlink/plugins/afreeca.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/albavision.py` & `streamlink-5.5.1/src/streamlink/plugins/albavision.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/aloula.py` & `streamlink-5.5.1/src/streamlink/plugins/aloula.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/app17.py` & `streamlink-5.5.1/src/streamlink/plugins/app17.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/ard_live.py` & `streamlink-5.5.1/src/streamlink/plugins/ard_live.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/ard_mediathek.py` & `streamlink-5.5.1/src/streamlink/plugins/ard_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/artetv.py` & `streamlink-5.5.1/src/streamlink/plugins/artetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/atpchallenger.py` & `streamlink-5.5.1/src/streamlink/plugins/atpchallenger.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/atresplayer.py` & `streamlink-5.5.1/src/streamlink/plugins/atresplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/bbciplayer.py` & `streamlink-5.5.1/src/streamlink/plugins/bbciplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/bfmtv.py` & `streamlink-5.5.1/src/streamlink/plugins/bfmtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/bigo.py` & `streamlink-5.5.1/src/streamlink/plugins/bigo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/bilibili.py` & `streamlink-5.5.1/src/streamlink/plugins/bilibili.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/blazetv.py` & `streamlink-5.5.1/src/streamlink/plugins/blazetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/bloomberg.py` & `streamlink-5.5.1/src/streamlink/plugins/bloomberg.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/booyah.py` & `streamlink-5.5.1/src/streamlink/plugins/booyah.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/brightcove.py` & `streamlink-5.5.1/src/streamlink/plugins/brightcove.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/btv.py` & `streamlink-5.5.1/src/streamlink/plugins/btv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/cbsnews.py` & `streamlink-5.5.1/src/streamlink/plugins/cbsnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/cdnbg.py` & `streamlink-5.5.1/src/streamlink/plugins/cdnbg.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/ceskatelevize.py` & `streamlink-5.5.1/src/streamlink/plugins/ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/cinergroup.py` & `streamlink-5.5.1/src/streamlink/plugins/cinergroup.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/clubbingtv.py` & `streamlink-5.5.1/src/streamlink/plugins/clubbingtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/cmmedia.py` & `streamlink-5.5.1/src/streamlink/plugins/cmmedia.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/cnews.py` & `streamlink-5.5.1/src/streamlink/plugins/cnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/crunchyroll.py` & `streamlink-5.5.1/src/streamlink/plugins/crunchyroll.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/dailymotion.py` & `streamlink-5.5.1/src/streamlink/plugins/dailymotion.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/dash.py` & `streamlink-5.5.1/src/streamlink/plugins/dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/delfi.py` & `streamlink-5.5.1/src/streamlink/plugins/delfi.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/deutschewelle.py` & `streamlink-5.5.1/src/streamlink/plugins/deutschewelle.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/dlive.py` & `streamlink-5.5.1/src/streamlink/plugins/dlive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/dogan.py` & `streamlink-5.5.1/src/streamlink/plugins/dogan.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/dogus.py` & `streamlink-5.5.1/src/streamlink/plugins/dogus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/drdk.py` & `streamlink-5.5.1/src/streamlink/plugins/drdk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/earthcam.py` & `streamlink-5.5.1/src/streamlink/plugins/earthcam.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/euronews.py` & `streamlink-5.5.1/src/streamlink/plugins/euronews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/facebook.py` & `streamlink-5.5.1/src/streamlink/plugins/facebook.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/filmon.py` & `streamlink-5.5.1/src/streamlink/plugins/filmon.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/foxtr.py` & `streamlink-5.5.1/src/streamlink/plugins/foxtr.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/galatasaraytv.py` & `streamlink-5.5.1/src/streamlink/plugins/galatasaraytv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/goltelevision.py` & `streamlink-5.5.1/src/streamlink/plugins/goltelevision.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/goodgame.py` & `streamlink-5.5.1/src/streamlink/plugins/goodgame.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/googledrive.py` & `streamlink-5.5.1/src/streamlink/plugins/googledrive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/gulli.py` & `streamlink-5.5.1/src/streamlink/plugins/gulli.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/hiplayer.py` & `streamlink-5.5.1/src/streamlink/plugins/hiplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/hls.py` & `streamlink-5.5.1/src/streamlink/plugins/hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/http.py` & `streamlink-5.5.1/src/streamlink/plugins/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/htv.py` & `streamlink-5.5.1/src/streamlink/plugins/htv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/huajiao.py` & `streamlink-5.5.1/src/streamlink/plugins/huajiao.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/huya.py` & `streamlink-5.5.1/src/streamlink/plugins/huya.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/idf1.py` & `streamlink-5.5.1/src/streamlink/plugins/idf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/indihometv.py` & `streamlink-5.5.1/src/streamlink/plugins/indihometv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/invintus.py` & `streamlink-5.5.1/src/streamlink/plugins/invintus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/kugou.py` & `streamlink-5.5.1/src/streamlink/plugins/kugou.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/linelive.py` & `streamlink-5.5.1/src/streamlink/plugins/linelive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/livestream.py` & `streamlink-5.5.1/src/streamlink/plugins/livestream.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/lnk.py` & `streamlink-5.5.1/src/streamlink/plugins/lnk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/lrt.py` & `streamlink-5.5.1/src/streamlink/plugins/lrt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/ltv_lsm_lv.py` & `streamlink-5.5.1/src/streamlink/plugins/ltv_lsm_lv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/mdstrm.py` & `streamlink-5.5.1/src/streamlink/plugins/mdstrm.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/mediaklikk.py` & `streamlink-5.5.1/src/streamlink/plugins/mediaklikk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/mediavitrina.py` & `streamlink-5.5.1/src/streamlink/plugins/mediavitrina.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/mildom.py` & `streamlink-5.5.1/src/streamlink/plugins/mildom.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/mitele.py` & `streamlink-5.5.1/src/streamlink/plugins/mitele.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/mixcloud.py` & `streamlink-5.5.1/src/streamlink/plugins/mixcloud.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/mjunoon.py` & `streamlink-5.5.1/src/streamlink/plugins/mjunoon.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/mrtmk.py` & `streamlink-5.5.1/src/streamlink/plugins/mrtmk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/n13tv.py` & `streamlink-5.5.1/src/streamlink/plugins/n13tv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/nhkworld.py` & `streamlink-5.5.1/src/streamlink/plugins/nhkworld.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/nicolive.py` & `streamlink-5.5.1/src/streamlink/plugins/nicolive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/nimotv.py` & `streamlink-5.5.1/src/streamlink/plugins/nimotv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/nos.py` & `streamlink-5.5.1/src/streamlink/plugins/nos.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/nownews.py` & `streamlink-5.5.1/src/streamlink/plugins/nownews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/nrk.py` & `streamlink-5.5.1/src/streamlink/plugins/nrk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/ntv.py` & `streamlink-5.5.1/src/streamlink/plugins/ntv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/okru.py` & `streamlink-5.5.1/src/streamlink/plugins/okru.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/olympicchannel.py` & `streamlink-5.5.1/src/streamlink/plugins/olympicchannel.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/oneplusone.py` & `streamlink-5.5.1/src/streamlink/plugins/oneplusone.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/onetv.py` & `streamlink-5.5.1/src/streamlink/plugins/onetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/openrectv.py` & `streamlink-5.5.1/src/streamlink/plugins/openrectv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/pandalive.py` & `streamlink-5.5.1/src/streamlink/plugins/pandalive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/picarto.py` & `streamlink-5.5.1/src/streamlink/plugins/picarto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/piczel.py` & `streamlink-5.5.1/src/streamlink/plugins/piczel.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/pixiv.py` & `streamlink-5.5.1/src/streamlink/plugins/pixiv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/pluto.py` & `streamlink-5.5.1/src/streamlink/plugins/pluto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/pluzz.py` & `streamlink-5.5.1/src/streamlink/plugins/pluzz.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/qq.py` & `streamlink-5.5.1/src/streamlink/plugins/qq.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/radiko.py` & `streamlink-5.5.1/src/streamlink/plugins/radiko.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/radionet.py` & `streamlink-5.5.1/src/streamlink/plugins/radionet.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/raiplay.py` & `streamlink-5.5.1/src/streamlink/plugins/raiplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/reuters.py` & `streamlink-5.5.1/src/streamlink/plugins/reuters.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/rtbf.py` & `streamlink-5.5.1/src/streamlink/plugins/rtbf.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/rtpa.py` & `streamlink-5.5.1/src/streamlink/plugins/rtpa.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/rtpplay.py` & `streamlink-5.5.1/src/streamlink/plugins/rtpplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/rtve.py` & `streamlink-5.5.1/src/streamlink/plugins/rtve.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/rtvs.py` & `streamlink-5.5.1/src/streamlink/plugins/rtvs.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/ruv.py` & `streamlink-5.5.1/src/streamlink/plugins/ruv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/sbscokr.py` & `streamlink-5.5.1/src/streamlink/plugins/sbscokr.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/showroom.py` & `streamlink-5.5.1/src/streamlink/plugins/showroom.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/sportal.py` & `streamlink-5.5.1/src/streamlink/plugins/sportal.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/sportschau.py` & `streamlink-5.5.1/src/streamlink/plugins/sportschau.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/ssh101.py` & `streamlink-5.5.1/src/streamlink/plugins/ssh101.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/stadium.py` & `streamlink-5.5.1/src/streamlink/plugins/stadium.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/steam.py` & `streamlink-5.5.1/src/streamlink/plugins/steam.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/streamable.py` & `streamlink-5.5.1/src/streamlink/plugins/streamable.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/streann.py` & `streamlink-5.5.1/src/streamlink/plugins/streann.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/stv.py` & `streamlink-5.5.1/src/streamlink/plugins/stv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/svtplay.py` & `streamlink-5.5.1/src/streamlink/plugins/svtplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/swisstxt.py` & `streamlink-5.5.1/src/streamlink/plugins/swisstxt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/telefe.py` & `streamlink-5.5.1/src/streamlink/plugins/telefe.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/telemadrid.py` & `streamlink-5.5.1/src/streamlink/plugins/telemadrid.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/tf1.py` & `streamlink-5.5.1/src/streamlink/plugins/tf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/trovo.py` & `streamlink-5.5.1/src/streamlink/plugins/trovo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/turkuvaz.py` & `streamlink-5.5.1/src/streamlink/plugins/turkuvaz.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/tv360.py` & `streamlink-5.5.1/src/streamlink/plugins/tv360.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/tv3cat.py` & `streamlink-5.5.1/src/streamlink/plugins/tv3cat.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/tv4play.py` & `streamlink-5.5.1/src/streamlink/plugins/tv4play.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/tv5monde.py` & `streamlink-5.5.1/src/streamlink/plugins/tv5monde.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/tv8.py` & `streamlink-5.5.1/src/streamlink/plugins/tv8.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/tv999.py` & `streamlink-5.5.1/src/streamlink/plugins/tv999.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/tvibo.py` & `streamlink-5.5.1/src/streamlink/plugins/tvibo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/tviplayer.py` & `streamlink-5.5.1/src/streamlink/plugins/tviplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/tvp.py` & `streamlink-5.5.1/src/streamlink/plugins/tvp.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/tvrby.py` & `streamlink-5.5.1/src/streamlink/plugins/tvrby.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/tvrplus.py` & `streamlink-5.5.1/src/streamlink/plugins/tvrplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/tvtoya.py` & `streamlink-5.5.1/src/streamlink/plugins/tvtoya.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/twitcasting.py` & `streamlink-5.5.1/src/streamlink/plugins/twitcasting.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/twitch.py` & `streamlink-5.5.1/src/streamlink/plugins/twitch.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/ustreamtv.py` & `streamlink-5.5.1/src/streamlink/plugins/ustreamtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/ustvnow.py` & `streamlink-5.5.1/src/streamlink/plugins/ustvnow.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/vidio.py` & `streamlink-5.5.1/src/streamlink/plugins/vidio.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/vimeo.py` & `streamlink-5.5.1/src/streamlink/plugins/vimeo.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,31 +4,34 @@
 $type live, vod
 $notes Password protected streams are not supported
 """
 
 import logging
 import re
 from html import unescape as html_unescape
-from urllib.parse import urlparse
+from urllib.parse import urljoin, urlparse
 
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.dash import DASHStream
 from streamlink.stream.ffmpegmux import MuxedStream
 from streamlink.stream.hls import HLSStream
 from streamlink.stream.http import HTTPStream
+from streamlink.utils.url import update_scheme
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(
     r"https?://(player\.vimeo\.com/video/\d+|(www\.)?vimeo\.com/.+)",
 ))
 class Vimeo(Plugin):
+    VIEWER_URL = "https://vimeo.com/_next/viewer"
+    OEMBED_URL = "https://vimeo.com/api/oembed.json"
     _config_url_re = re.compile(r'(?:"config_url"|\bdata-config-url)\s*[:=]\s*(".+?")')
     _config_re = re.compile(r"playerConfig\s*=\s*({.+?})\s*var")
     _config_url_schema = validate.Schema(
         validate.transform(_config_url_re.search),
         validate.any(
             None,
             validate.Schema(
@@ -57,19 +60,57 @@
         },
     )
     _player_schema = validate.Schema(
         validate.transform(_config_re.search),
         validate.any(None, validate.Schema(validate.get(1), _config_schema)),
     )
 
+    def get_config_url(self) -> str:
+        jwt, api_url = self.session.http.get(
+            self.VIEWER_URL,
+            schema=validate.Schema(
+                validate.parse_json(),
+                {
+                    "jwt": str,
+                    "apiUrl": str,
+                },
+                validate.union_get("jwt", "apiUrl"),
+            ),
+        )
+        uri = self.session.http.get(
+            self.OEMBED_URL,
+            params={"url": self.url},
+            schema=validate.Schema(
+                validate.parse_json(),
+                {"uri": str},
+                validate.get("uri"),
+            ),
+        )
+        player_config_url = urljoin(update_scheme("https://", api_url), uri)
+
+        return self.session.http.get(
+            player_config_url,
+            params={"fields": "config_url"},
+            headers={"Authorization": f"jwt {jwt}"},
+            schema=validate.Schema(
+                validate.parse_json(),
+                {"config_url": validate.url()},
+                validate.get("config_url"),
+            ),
+        )
+
     def _get_streams(self):
         if "player.vimeo.com" in self.url:
             data = self.session.http.get(self.url, schema=self._player_schema)
         else:
             api_url = self.session.http.get(self.url, schema=self._config_url_schema)
+
+            if not api_url:
+                api_url = self.get_config_url()
+
             if not api_url:
                 return
             data = self.session.http.get(api_url, schema=self._config_schema)
 
         videos = data["request"]["files"]
         streams = []
```

### Comparing `streamlink-5.5.0/src/streamlink/plugins/vinhlongtv.py` & `streamlink-5.5.1/src/streamlink/plugins/vinhlongtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/vk.py` & `streamlink-5.5.1/src/streamlink/plugins/vk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/vkplay.py` & `streamlink-5.5.1/src/streamlink/plugins/vkplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/vlive.py` & `streamlink-5.5.1/src/streamlink/plugins/vlive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/vtvgo.py` & `streamlink-5.5.1/src/streamlink/plugins/vtvgo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/wasd.py` & `streamlink-5.5.1/src/streamlink/plugins/wasd.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/webtv.py` & `streamlink-5.5.1/src/streamlink/plugins/webtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/welt.py` & `streamlink-5.5.1/src/streamlink/plugins/welt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/wwenetwork.py` & `streamlink-5.5.1/src/streamlink/plugins/wwenetwork.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/youtube.py` & `streamlink-5.5.1/src/streamlink/plugins/youtube.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/yupptv.py` & `streamlink-5.5.1/src/streamlink/plugins/yupptv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/zattoo.py` & `streamlink-5.5.1/src/streamlink/plugins/zattoo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/zdf_mediathek.py` & `streamlink-5.5.1/src/streamlink/plugins/zdf_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/zeenews.py` & `streamlink-5.5.1/src/streamlink/plugins/zeenews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/zengatv.py` & `streamlink-5.5.1/src/streamlink/plugins/zengatv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/plugins/zhanqi.py` & `streamlink-5.5.1/src/streamlink/plugins/zhanqi.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/session.py` & `streamlink-5.5.1/src/streamlink/session.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/stream/dash.py` & `streamlink-5.5.1/src/streamlink/stream/dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/stream/dash_manifest.py` & `streamlink-5.5.1/src/streamlink/stream/dash_manifest.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/stream/ffmpegmux.py` & `streamlink-5.5.1/src/streamlink/stream/ffmpegmux.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/stream/file.py` & `streamlink-5.5.1/src/streamlink/stream/file.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/stream/filtered.py` & `streamlink-5.5.1/src/streamlink/stream/filtered.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/stream/hls.py` & `streamlink-5.5.1/src/streamlink/stream/hls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import re
 import struct
 from concurrent.futures import Future
+from datetime import datetime, timedelta
 from typing import Any, Dict, List, NamedTuple, Optional, Tuple, Union
 from urllib.parse import urlparse
 
 # noinspection PyPackageRequirements
 from Crypto.Cipher import AES
 
 # noinspection PyPackageRequirements
@@ -18,14 +19,15 @@
 from streamlink.stream.ffmpegmux import FFMPEGMuxer, MuxedStream
 from streamlink.stream.filtered import FilteredStream
 from streamlink.stream.hls_playlist import M3U8, ByteRange, Key, Map, Media, Segment, load as load_hls_playlist
 from streamlink.stream.http import HTTPStream
 from streamlink.stream.segmented import SegmentedStreamReader, SegmentedStreamWorker, SegmentedStreamWriter
 from streamlink.utils.cache import LRUCache
 from streamlink.utils.formatter import Formatter
+from streamlink.utils.times import now
 
 
 log = logging.getLogger(__name__)
 
 
 class Sequence(NamedTuple):
     num: int
@@ -293,14 +295,15 @@
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
         self.playlist_changed = False
         self.playlist_end: Optional[int] = None
         self.playlist_sequence: int = -1
         self.playlist_sequences: List[Sequence] = []
+        self.playlist_reload_last: datetime = now()
         self.playlist_reload_time: float = 6
         self.playlist_reload_time_override = self.session.options.get("hls-playlist-reload-time")
         self.playlist_reload_retries = self.session.options.get("hls-playlist-reload-attempts")
         self.live_edge = self.session.options.get("hls-live-edge")
         self.duration_offset_start = int(self.stream.start_offset + (self.session.options.get("hls-start-offset") or 0))
         self.duration_limit = self.stream.duration or (
             int(self.session.options.get("hls-duration")) if self.session.options.get("hls-duration") else None)
@@ -408,14 +411,15 @@
             d += sequence.segment.duration
             default = sequence.num
 
         # could not skip far enough, so return the default
         return default
 
     def iter_segments(self):
+        self.playlist_reload_last = now()
         try:
             self.reload_playlist()
         except StreamError as err:
             log.error(f"{err}")
             self.reader.close()
             return
 
@@ -453,15 +457,28 @@
                 # End of stream
                 stream_end = self.playlist_end is not None and sequence.num >= self.playlist_end
                 if self.closed or stream_end:
                     return
 
                 self.playlist_sequence = sequence.num + 1
 
-            if self.wait(self.playlist_reload_time):
+            # Exclude playlist fetch+processing time from the overall playlist reload time
+            # and reload playlist in a strict time interval
+            time_completed = now()
+            time_elapsed = max(0.0, (time_completed - self.playlist_reload_last).total_seconds())
+            time_wait = max(0.0, self.playlist_reload_time - time_elapsed)
+            if self.wait(time_wait):
+                if time_wait > 0:
+                    # If we had to wait, then don't call now() twice and instead reference the timestamp from before
+                    # the wait() call, to prevent a shifting time offset due to the execution time.
+                    self.playlist_reload_last = time_completed + timedelta(seconds=time_wait)
+                else:
+                    # Otherwise, get the current time, as the reload interval already has shifted.
+                    self.playlist_reload_last = now()
+
                 try:
                     self.reload_playlist()
                 except StreamError as err:
                     log.warning(f"Failed to reload playlist: {err}")
 
 
 class HLSStreamReader(FilteredStream, SegmentedStreamReader):
```

### Comparing `streamlink-5.5.0/src/streamlink/stream/hls_playlist.py` & `streamlink-5.5.1/src/streamlink/stream/hls_playlist.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/stream/http.py` & `streamlink-5.5.1/src/streamlink/stream/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/stream/segmented.py` & `streamlink-5.5.1/src/streamlink/stream/segmented.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/stream/stream.py` & `streamlink-5.5.1/src/streamlink/stream/stream.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/stream/wrappers.py` & `streamlink-5.5.1/src/streamlink/stream/wrappers.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/user_input.py` & `streamlink-5.5.1/src/streamlink/user_input.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/utils/__init__.py` & `streamlink-5.5.1/src/streamlink/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/utils/args.py` & `streamlink-5.5.1/src/streamlink/utils/args.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/utils/cache.py` & `streamlink-5.5.1/src/streamlink/utils/cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/utils/crypto.py` & `streamlink-5.5.1/src/streamlink/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/utils/data.py` & `streamlink-5.5.1/src/streamlink/utils/data.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/utils/formatter.py` & `streamlink-5.5.1/src/streamlink/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/utils/l10n.py` & `streamlink-5.5.1/src/streamlink/utils/l10n.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/utils/named_pipe.py` & `streamlink-5.5.1/src/streamlink/utils/named_pipe.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/utils/parse.py` & `streamlink-5.5.1/src/streamlink/utils/parse.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/utils/processoutput.py` & `streamlink-5.5.1/src/streamlink/utils/processoutput.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/utils/times.py` & `streamlink-5.5.1/src/streamlink/utils/times.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink/utils/url.py` & `streamlink-5.5.1/src/streamlink/utils/url.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink.egg-info/PKG-INFO` & `streamlink-5.5.1/src/streamlink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink
-Version: 5.5.0
+Version: 5.5.1
 Summary: Streamlink is a command-line utility that extracts streams from various services and pipes them into a video player of choice.
 Home-page: https://github.com/streamlink/streamlink
 Author: Streamlink
 Author-email: streamlink@protonmail.com
 License: Simplified BSD
 Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlink Version: 5.5.0 Summary: Streamlink is a
+Metadata-Version: 2.1 Name: streamlink Version: 5.5.1 Summary: Streamlink is a
 command-line utility that extracts streams from various services and pipes them
 into a video player of choice. Home-page: https://github.com/streamlink/
 streamlink Author: Streamlink Author-email: streamlink@protonmail.com License:
 Simplified BSD Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues Project-
 URL: Source, https://github.com/streamlink/streamlink Project-URL: Funding,
 https://streamlink.github.io/latest/donate.html Classifier: Development Status
```

### Comparing `streamlink-5.5.0/src/streamlink.egg-info/SOURCES.txt` & `streamlink-5.5.1/src/streamlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink_cli/argparser.py` & `streamlink-5.5.1/src/streamlink_cli/argparser.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink_cli/compat.py` & `streamlink-5.5.1/src/streamlink_cli/compat.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink_cli/console.py` & `streamlink-5.5.1/src/streamlink_cli/console.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink_cli/constants.py` & `streamlink-5.5.1/src/streamlink_cli/constants.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink_cli/main.py` & `streamlink-5.5.1/src/streamlink_cli/main.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink_cli/output/abc.py` & `streamlink-5.5.1/src/streamlink_cli/output/abc.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink_cli/output/file.py` & `streamlink-5.5.1/src/streamlink_cli/output/file.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink_cli/output/http.py` & `streamlink-5.5.1/src/streamlink_cli/output/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink_cli/output/player.py` & `streamlink-5.5.1/src/streamlink_cli/output/player.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink_cli/streamrunner.py` & `streamlink-5.5.1/src/streamlink_cli/streamrunner.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink_cli/utils/__init__.py` & `streamlink-5.5.1/src/streamlink_cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink_cli/utils/formatter.py` & `streamlink-5.5.1/src/streamlink_cli/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink_cli/utils/path.py` & `streamlink-5.5.1/src/streamlink_cli/utils/path.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink_cli/utils/player.py` & `streamlink-5.5.1/src/streamlink_cli/utils/player.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink_cli/utils/progress.py` & `streamlink-5.5.1/src/streamlink_cli/utils/progress.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/src/streamlink_cli/utils/versioncheck.py` & `streamlink-5.5.1/src/streamlink_cli/utils/versioncheck.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/__init__.py` & `streamlink-5.5.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/cli/output/test_output.py` & `streamlink-5.5.1/tests/cli/output/test_output.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/cli/output/test_playeroutput.py` & `streamlink-5.5.1/tests/cli/output/test_playeroutput.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/cli/test_argparser.py` & `streamlink-5.5.1/tests/cli/test_argparser.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/cli/test_cmdline.py` & `streamlink-5.5.1/tests/cli/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/cli/test_cmdline_player_fifo.py` & `streamlink-5.5.1/tests/cli/test_cmdline_player_fifo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/cli/test_cmdline_title.py` & `streamlink-5.5.1/tests/cli/test_cmdline_title.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/cli/test_console.py` & `streamlink-5.5.1/tests/cli/test_console.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/cli/test_main.py` & `streamlink-5.5.1/tests/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/cli/test_main_formatter.py` & `streamlink-5.5.1/tests/cli/test_main_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/cli/test_main_setup_config_args.py` & `streamlink-5.5.1/tests/cli/test_main_setup_config_args.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/cli/test_streamrunner.py` & `streamlink-5.5.1/tests/cli/test_streamrunner.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/cli/utils/test_formatter.py` & `streamlink-5.5.1/tests/cli/utils/test_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/cli/utils/test_path.py` & `streamlink-5.5.1/tests/cli/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/cli/utils/test_progress.py` & `streamlink-5.5.1/tests/cli/utils/test_progress.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/cli/utils/test_versioncheck.py` & `streamlink-5.5.1/tests/cli/utils/test_versioncheck.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/conftest.py` & `streamlink-5.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/mixins/stream_hls.py` & `streamlink-5.5.1/tests/mixins/stream_hls.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from threading import Event, Thread
 from typing import List
 from unittest.mock import patch
 
 import requests_mock
 
 from streamlink import Streamlink
-from streamlink.stream.hls import HLSStream, HLSStreamWriter as _HLSStreamWriter
+from streamlink.stream.hls import HLSStream, HLSStreamWorker as _HLSStreamWorker, HLSStreamWriter as _HLSStreamWriter
 from tests.testutils.handshake import Handshake
 
 
 TIMEOUT_AWAIT_READ = 5
 TIMEOUT_AWAIT_READ_ONCE = 5
 TIMEOUT_AWAIT_WRITE = 60  # https://github.com/streamlink/streamlink/issues/3868
+TIMEOUT_AWAIT_PLAYLIST_RELOAD = 5
+TIMEOUT_AWAIT_PLAYLIST_WAIT = 5
 TIMEOUT_AWAIT_CLOSE = 5
 
 
 class HLSItemBase:
     path = ""
 
     def url(self, namespace):
@@ -86,14 +88,31 @@
         return "#EXTINF:{duration:.3f},{title}\n{path}".format(
             duration=self.duration,
             title=self.title,
             path=self.path if self.path_relative else self.url(namespace),
         )
 
 
+class EventedHLSStreamWorker(_HLSStreamWorker):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.handshake_reload = Handshake()
+        self.handshake_wait = Handshake()
+        self.time_wait = None
+
+    def reload_playlist(self):
+        with self.handshake_reload():
+            return super().reload_playlist()
+
+    def wait(self, time):
+        self.time_wait = time
+        with self.handshake_wait():
+            return not self.closed
+
+
 class EventedHLSStreamWriter(_HLSStreamWriter):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.handshake = Handshake()
 
     def _futures_put(self, item):
         self.futures.put_nowait(item)
@@ -226,14 +245,24 @@
     def await_close(self, timeout=TIMEOUT_AWAIT_CLOSE):
         thread = self.thread
         thread.reader.writer.join(timeout)
         thread.reader.worker.join(timeout)
         thread.join(timeout)
         assert self.thread.reader.closed, "Stream reader is closed"
 
+    def await_playlist_reload(self, timeout=TIMEOUT_AWAIT_PLAYLIST_RELOAD) -> None:
+        worker: EventedHLSStreamWorker = self.thread.reader.worker  # type: ignore[assignment]
+        assert worker.is_alive()
+        assert worker.handshake_reload.step(timeout)
+
+    def await_playlist_wait(self, timeout=TIMEOUT_AWAIT_PLAYLIST_WAIT) -> None:
+        worker: EventedHLSStreamWorker = self.thread.reader.worker  # type: ignore[assignment]
+        assert worker.is_alive()
+        assert worker.handshake_wait.step(timeout)
+
     # make write calls on the write-thread and wait until it has finished
     def await_write(self, write_calls=1, timeout=TIMEOUT_AWAIT_WRITE) -> None:
         writer: EventedHLSStreamWriter = self.thread.reader.writer  # type: ignore[assignment]
         assert writer.is_alive()
         for _ in range(write_calls):
             assert writer.handshake.step(timeout)
```

### Comparing `streamlink-5.5.0/tests/plugin/testplugin.py` & `streamlink-5.5.1/tests/plugin/testplugin.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/__init__.py` & `streamlink-5.5.1/tests/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/conftest.py` & `streamlink-5.5.1/tests/plugins/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_abematv.py` & `streamlink-5.5.1/tests/plugins/test_abematv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_adultswim.py` & `streamlink-5.5.1/tests/plugins/test_adultswim.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_afreeca.py` & `streamlink-5.5.1/tests/plugins/test_afreeca.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_albavision.py` & `streamlink-5.5.1/tests/plugins/test_albavision.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_aloula.py` & `streamlink-5.5.1/tests/plugins/test_aloula.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_ard_mediathek.py` & `streamlink-5.5.1/tests/plugins/test_ard_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_artetv.py` & `streamlink-5.5.1/tests/plugins/test_artetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_atpchallenger.py` & `streamlink-5.5.1/tests/plugins/test_atpchallenger.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_atresplayer.py` & `streamlink-5.5.1/tests/plugins/test_atresplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_bbciplayer.py` & `streamlink-5.5.1/tests/plugins/test_bbciplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_bfmtv.py` & `streamlink-5.5.1/tests/plugins/test_bfmtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_bigo.py` & `streamlink-5.5.1/tests/plugins/test_bigo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_blazetv.py` & `streamlink-5.5.1/tests/plugins/test_blazetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_bloomberg.py` & `streamlink-5.5.1/tests/plugins/test_bloomberg.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_booyah.py` & `streamlink-5.5.1/tests/plugins/test_booyah.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_cbsnews.py` & `streamlink-5.5.1/tests/plugins/test_cbsnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_cdnbg.py` & `streamlink-5.5.1/tests/plugins/test_cdnbg.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_ceskatelevize.py` & `streamlink-5.5.1/tests/plugins/test_ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_cinergroup.py` & `streamlink-5.5.1/tests/plugins/test_cinergroup.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_cmmedia.py` & `streamlink-5.5.1/tests/plugins/test_cmmedia.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_crunchyroll.py` & `streamlink-5.5.1/tests/plugins/test_crunchyroll.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_dailymotion.py` & `streamlink-5.5.1/tests/plugins/test_dailymotion.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_dash.py` & `streamlink-5.5.1/tests/plugins/test_dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_delfi.py` & `streamlink-5.5.1/tests/plugins/test_delfi.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_deutschewelle.py` & `streamlink-5.5.1/tests/plugins/test_deutschewelle.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_dogan.py` & `streamlink-5.5.1/tests/plugins/test_dogan.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_drdk.py` & `streamlink-5.5.1/tests/plugins/test_drdk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_euronews.py` & `streamlink-5.5.1/tests/plugins/test_euronews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_facebook.py` & `streamlink-5.5.1/tests/plugins/test_facebook.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_filmon.py` & `streamlink-5.5.1/tests/plugins/test_filmon.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_goltelevision.py` & `streamlink-5.5.1/tests/plugins/test_goltelevision.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_gulli.py` & `streamlink-5.5.1/tests/plugins/test_gulli.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_htv.py` & `streamlink-5.5.1/tests/plugins/test_htv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_idf1.py` & `streamlink-5.5.1/tests/plugins/test_idf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_invintus.py` & `streamlink-5.5.1/tests/plugins/test_invintus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_kugou.py` & `streamlink-5.5.1/tests/plugins/test_kugou.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_livestream.py` & `streamlink-5.5.1/tests/plugins/test_livestream.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_lnk.py` & `streamlink-5.5.1/tests/plugins/test_lnk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_lrt.py` & `streamlink-5.5.1/tests/plugins/test_lrt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_ltv_lsm_lv.py` & `streamlink-5.5.1/tests/plugins/test_ltv_lsm_lv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_mdstrm.py` & `streamlink-5.5.1/tests/plugins/test_mdstrm.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_mediaklikk.py` & `streamlink-5.5.1/tests/plugins/test_mediaklikk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_mediavitrina.py` & `streamlink-5.5.1/tests/plugins/test_mediavitrina.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_mitele.py` & `streamlink-5.5.1/tests/plugins/test_mitele.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_mixcloud.py` & `streamlink-5.5.1/tests/plugins/test_mixcloud.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_n13tv.py` & `streamlink-5.5.1/tests/plugins/test_n13tv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_nicolive.py` & `streamlink-5.5.1/tests/plugins/test_nicolive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_nos.py` & `streamlink-5.5.1/tests/plugins/test_nos.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_nrk.py` & `streamlink-5.5.1/tests/plugins/test_nrk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_olympicchannel.py` & `streamlink-5.5.1/tests/plugins/test_olympicchannel.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_oneplusone.py` & `streamlink-5.5.1/tests/plugins/test_oneplusone.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_onetv.py` & `streamlink-5.5.1/tests/plugins/test_onetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_pandalive.py` & `streamlink-5.5.1/tests/plugins/test_pandalive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_picarto.py` & `streamlink-5.5.1/tests/plugins/test_picarto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_pluto.py` & `streamlink-5.5.1/tests/plugins/test_pluto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_pluzz.py` & `streamlink-5.5.1/tests/plugins/test_pluzz.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_radionet.py` & `streamlink-5.5.1/tests/plugins/test_radionet.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_raiplay.py` & `streamlink-5.5.1/tests/plugins/test_raiplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_reuters.py` & `streamlink-5.5.1/tests/plugins/test_reuters.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_rtbf.py` & `streamlink-5.5.1/tests/plugins/test_rtbf.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_rtpplay.py` & `streamlink-5.5.1/tests/plugins/test_rtpplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_rtve.py` & `streamlink-5.5.1/tests/plugins/test_rtve.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_ruv.py` & `streamlink-5.5.1/tests/plugins/test_ruv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_sbscokr.py` & `streamlink-5.5.1/tests/plugins/test_sbscokr.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_showroom.py` & `streamlink-5.5.1/tests/plugins/test_showroom.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_steam.py` & `streamlink-5.5.1/tests/plugins/test_steam.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_stream.py` & `streamlink-5.5.1/tests/plugins/test_stream.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_streann.py` & `streamlink-5.5.1/tests/plugins/test_streann.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_svtplay.py` & `streamlink-5.5.1/tests/plugins/test_svtplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_swisstxt.py` & `streamlink-5.5.1/tests/plugins/test_swisstxt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_telefe.py` & `streamlink-5.5.1/tests/plugins/test_telefe.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_tf1.py` & `streamlink-5.5.1/tests/plugins/test_tf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_trovo.py` & `streamlink-5.5.1/tests/plugins/test_trovo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_turkuvaz.py` & `streamlink-5.5.1/tests/plugins/test_turkuvaz.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_tv4play.py` & `streamlink-5.5.1/tests/plugins/test_tv4play.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_tv5monde.py` & `streamlink-5.5.1/tests/plugins/test_tv5monde.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_tvp.py` & `streamlink-5.5.1/tests/plugins/test_tvp.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_tvrby.py` & `streamlink-5.5.1/tests/plugins/test_tvrby.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_tvrplus.py` & `streamlink-5.5.1/tests/plugins/test_tvrplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_twitch.py` & `streamlink-5.5.1/tests/plugins/test_twitch.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_ustreamtv.py` & `streamlink-5.5.1/tests/plugins/test_ustreamtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_ustvnow.py` & `streamlink-5.5.1/tests/plugins/test_ustvnow.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_vimeo.py` & `streamlink-5.5.1/tests/plugins/test_vimeo.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 from tests.plugins import PluginCanHandleUrl
 
 
 class TestPluginCanHandleUrlVimeo(PluginCanHandleUrl):
     __plugin__ = Vimeo
 
     should_match = [
-        "https://vimeo.com/237163735",
+        "https://vimeo.com/783455878",
         "https://vimeo.com/channels/music/176894130",
         "https://vimeo.com/album/3706071/video/148903960",
-        "https://vimeo.com/ondemand/surveyopenspace/92630739",
+        "https://vimeo.com/ondemand/worldoftomorrow3/467204924",
         "https://vimeo.com/ondemand/100footsurfingdays",
         "https://player.vimeo.com/video/176894130",
+        "https://vimeo.com/771745400/840d05200c",
     ]
 
     should_not_match = [
         "https://www.vimeo.com/",
     ]
```

### Comparing `streamlink-5.5.0/tests/plugins/test_vinhlongtv.py` & `streamlink-5.5.1/tests/plugins/test_vinhlongtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_vk.py` & `streamlink-5.5.1/tests/plugins/test_vk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_vtvgo.py` & `streamlink-5.5.1/tests/plugins/test_vtvgo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_webtv.py` & `streamlink-5.5.1/tests/plugins/test_webtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_welt.py` & `streamlink-5.5.1/tests/plugins/test_welt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_youtube.py` & `streamlink-5.5.1/tests/plugins/test_youtube.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_zattoo.py` & `streamlink-5.5.1/tests/plugins/test_zattoo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_zdf_mediathek.py` & `streamlink-5.5.1/tests/plugins/test_zdf_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/plugins/test_zengatv.py` & `streamlink-5.5.1/tests/plugins/test_zengatv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/__init__.py` & `streamlink-5.5.1/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/dash/test_1.mpd` & `streamlink-5.5.1/tests/resources/dash/test_1.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/dash/test_10.mpd` & `streamlink-5.5.1/tests/resources/dash/test_10.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/dash/test_11_static.mpd` & `streamlink-5.5.1/tests/resources/dash/test_11_static.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/dash/test_2.mpd` & `streamlink-5.5.1/tests/resources/dash/test_2.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/dash/test_3.mpd` & `streamlink-5.5.1/tests/resources/dash/test_3.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/dash/test_8.mpd` & `streamlink-5.5.1/tests/resources/dash/test_8.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/dash/test_9.mpd` & `streamlink-5.5.1/tests/resources/dash/test_9.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd` & `streamlink-5.5.1/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd` & `streamlink-5.5.1/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/dash/test_nested_baseurls.mpd` & `streamlink-5.5.1/tests/resources/dash/test_nested_baseurls.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/dash/test_no_segment_list_or_template.mpd` & `streamlink-5.5.1/tests/resources/dash/test_no_segment_list_or_template.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/dash/test_segment_list.mpd` & `streamlink-5.5.1/tests/resources/dash/test_segment_list.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/dash/test_segments_byterange.mpd` & `streamlink-5.5.1/tests/resources/dash/test_segments_byterange.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/dash/test_segments_dynamic_number.mpd` & `streamlink-5.5.1/tests/resources/dash/test_segments_dynamic_number.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/dash/test_static_no_publish_time.mpd` & `streamlink-5.5.1/tests/resources/dash/test_static_no_publish_time.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/dash/test_timeline_ids.mpd` & `streamlink-5.5.1/tests/resources/dash/test_timeline_ids.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/hls/test_1.m3u8` & `streamlink-5.5.1/tests/resources/hls/test_1.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/hls/test_2.m3u8` & `streamlink-5.5.1/tests/resources/hls/test_2.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/hls/test_date.m3u8` & `streamlink-5.5.1/tests/resources/hls/test_date.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/hls/test_master.m3u8` & `streamlink-5.5.1/tests/resources/hls/test_master.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/resources/hls/test_master_twitch_vod.m3u8` & `streamlink-5.5.1/tests/resources/hls/test_master_twitch_vod.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/stream/test_dash.py` & `streamlink-5.5.1/tests/stream/test_dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/stream/test_dash_parser.py` & `streamlink-5.5.1/tests/stream/test_dash_parser.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/stream/test_ffmpegmux.py` & `streamlink-5.5.1/tests/stream/test_ffmpegmux.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/stream/test_file.py` & `streamlink-5.5.1/tests/stream/test_file.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/stream/test_hls.py` & `streamlink-5.5.1/tests/stream/test_hls.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import os
 import typing
 import unittest
+from datetime import datetime, timedelta, timezone
 from threading import Event
 from unittest.mock import Mock, call, patch
 
+import freezegun
 import pytest
 import requests_mock
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad
 from requests.exceptions import InvalidSchema
 
 from streamlink.session import Streamlink
 from streamlink.stream.hls import HLSStream, HLSStreamReader, MuxedHLSStream
 from streamlink.stream.hls_playlist import M3U8Parser
-from tests.mixins.stream_hls import EventedHLSStreamWriter, Playlist, Segment, Tag, TestMixinStreamHLS
+from tests.mixins.stream_hls import EventedHLSStreamWorker, EventedHLSStreamWriter, Playlist, Segment, Tag, TestMixinStreamHLS
 from tests.resources import text
 
 
+EPOCH = datetime(2000, 1, 1, 0, 0, 0, 0, tzinfo=timezone.utc)
+ONE_SECOND = timedelta(seconds=1.0)
+
+
 class EncryptedBase:
     content: bytes
     content_plain: bytes
 
     def __init__(self, num, key, iv, *args, content=None, padding=b"", append=b"", **kwargs):
         super().__init__(num, *args, **kwargs)
         aesCipher = AES.new(key, AES.MODE_CBC, iv)
@@ -114,20 +120,28 @@
         stream = HLSStream(session, "http://mocked/foo", url_master="http://mocked/master.m3u8")
 
         assert stream.multivariant is None
         assert stream.url == "http://mocked/foo"
         assert stream.url_master == "http://mocked/master.m3u8"
 
 
-class EventedHLSReader(HLSStreamReader):
+class EventedWorkerHLSStreamReader(HLSStreamReader):
+    __worker__ = EventedHLSStreamWorker
+
+
+class EventedWriterHLSStreamReader(HLSStreamReader):
     __writer__ = EventedHLSStreamWriter
 
 
-class EventedHLSStream(HLSStream):
-    __reader__ = EventedHLSReader
+class EventedWorkerHLSStream(HLSStream):
+    __reader__ = EventedWorkerHLSStreamReader
+
+
+class EventedWriterHLSStream(HLSStream):
+    __reader__ = EventedWriterHLSStreamReader
 
 
 @patch("streamlink.stream.hls.HLSStreamWorker.wait", Mock(return_value=True))
 class TestHLSStream(TestMixinStreamHLS, unittest.TestCase):
     def get_session(self, options=None, *args, **kwargs):
         session = super().get_session(options)
         session.set_option("hls-live-edge", 3)
@@ -169,17 +183,121 @@
             map1, segments[1], map1, segments[2], map1, segments[3],
             map1, segments[4], map2, segments[5], map2, segments[6], segments[7],
         ])
         assert self.called(map1, once=True), "Downloads first map only once"
         assert self.called(map2, once=True), "Downloads second map only once"
 
 
+class TestHLSStreamWorker(TestMixinStreamHLS, unittest.TestCase):
+    __stream__ = EventedWorkerHLSStream
+
+    OPTIONS = {"stream-timeout": 1}
+
+    def tearDown(self) -> None:
+        worker: EventedHLSStreamWorker = self.thread.reader.worker  # type: ignore[assignment]
+        # don't await the handshakes on error
+        worker.handshake_wait.go()
+        worker.handshake_reload.go()
+        return super().tearDown()
+
+    def get_session(self, options=None, *args, **kwargs):
+        return super().get_session({**self.OPTIONS, **(options or {})}, *args, **kwargs)
+
+    def test_playlist_reload_offset(self) -> None:
+        thread, segments = self.subject(
+            start=False,
+            playlists=[
+                Playlist(0, targetduration=5, segments=[Segment(0)]),
+                Playlist(1, targetduration=5, segments=[Segment(1)]),
+                Playlist(2, targetduration=5, segments=[Segment(2)]),
+                Playlist(3, targetduration=5, segments=[Segment(3)]),
+                Playlist(4, targetduration=5, segments=[Segment(4)], end=True),
+            ],
+        )
+        worker: EventedHLSStreamWorker = thread.reader.worker
+        targetduration = ONE_SECOND * 5
+
+        with freezegun.freeze_time(EPOCH) as frozen_time:
+            self.start()
+
+            assert worker.handshake_reload.wait_ready(1), "Arrives at initial playlist reload"
+            assert worker.playlist_reload_last == EPOCH, "Sets the initial value of the last reload time"
+
+            # adjust clock and reload playlist: let it take one second
+            frozen_time.move_to(worker.playlist_reload_last + ONE_SECOND)
+            self.await_playlist_reload()
+            assert worker.playlist_reload_time == 5.0, "Uses the playlist's targetduration as reload time"
+
+            # time_completed = 00:00:01; time_elapsed = 1s
+            assert worker.handshake_wait.wait_ready(1), "Arrives at first wait() call"
+            assert worker.playlist_sequence == 1, "Has queued first segment"
+            assert worker.time_wait == 4.0, "Waits for 4 seconds out of the 5 seconds reload time"
+            self.await_playlist_wait()
+
+            assert worker.handshake_reload.wait_ready(1), "Arrives at second playlist reload"
+            assert worker.playlist_reload_last == EPOCH + targetduration, \
+                "Last reload time is the sum of reload+wait time (=targetduration)"
+
+            # adjust clock and reload playlist: let it exceed targetduration by two seconds
+            frozen_time.move_to(worker.playlist_reload_last + targetduration + ONE_SECOND * 2)
+            self.await_playlist_reload()
+            assert worker.playlist_reload_time == 5.0, "Uses the playlist's targetduration as reload time"
+
+            # time_completed = 00:00:12; time_elapsed = 7s (exceeded 5s targetduration)
+            assert worker.handshake_wait.wait_ready(1), "Arrives at second wait() call"
+            assert worker.playlist_sequence == 2, "Has queued second segment"
+            assert worker.time_wait == 0.0, "Doesn't wait when reloading took too long"
+            self.await_playlist_wait()
+
+            assert worker.handshake_reload.wait_ready(1), "Arrives at third playlist reload"
+            assert worker.playlist_reload_last == EPOCH + targetduration * 2 + ONE_SECOND * 2, \
+                "Sets last reload time to current time when reloading took too long (changes the interval)"
+
+            # adjust clock and reload playlist: let it take one second again
+            frozen_time.move_to(worker.playlist_reload_last + ONE_SECOND)
+            self.await_playlist_reload()
+            assert worker.playlist_reload_time == 5.0, "Uses the playlist's targetduration as reload time"
+
+            # time_completed = 00:00:13; time_elapsed = 1s
+            assert worker.handshake_wait.wait_ready(1), "Arrives at third wait() call"
+            assert worker.playlist_sequence == 3, "Has queued third segment"
+            assert worker.time_wait == 4.0, "Waits for 4 seconds out of the 5 seconds reload time"
+            self.await_playlist_wait()
+
+            assert worker.handshake_reload.wait_ready(1), "Arrives at fourth playlist reload"
+            assert worker.playlist_reload_last == EPOCH + targetduration * 3 + ONE_SECOND * 2, \
+                "Last reload time is the sum of reload+wait time (=targetduration) of the changed interval"
+
+            # adjust clock and reload playlist: simulate no fetch+processing delay
+            frozen_time.move_to(worker.playlist_reload_last)
+            self.await_playlist_reload()
+            assert worker.playlist_reload_time == 5.0, "Uses the playlist's targetduration as reload time"
+
+            # time_completed = 00:00:17; time_elapsed = 0s
+            assert worker.handshake_wait.wait_ready(1), "Arrives at fourth wait() call"
+            assert worker.playlist_sequence == 4, "Has queued fourth segment"
+            assert worker.time_wait == 5.0, "Waits for the whole reload time"
+            self.await_playlist_wait()
+
+            assert worker.handshake_reload.wait_ready(1), "Arrives at fifth playlist reload"
+            assert worker.playlist_reload_last == EPOCH + targetduration * 4 + ONE_SECOND * 2, \
+                "Last reload time is the sum of reload+wait time (no delay)"
+
+            # adjusting the clock is not needed anymore
+            self.await_playlist_reload()
+            assert self.await_read(read_all=True) == self.content(segments)
+            self.await_close()
+            assert worker.playlist_sequence == 4, "Doesn't update sequence number once ended"
+            assert not worker.handshake_wait.wait_ready(0), "Doesn't wait once ended"
+            assert not worker.handshake_reload.wait_ready(0), "Doesn't reload playlist once ended"
+
+
 @patch("streamlink.stream.hls.HLSStreamWorker.wait", Mock(return_value=True))
 class TestHLSStreamByterange(TestMixinStreamHLS, unittest.TestCase):
-    __stream__ = EventedHLSStream
+    __stream__ = EventedWriterHLSStream
 
     # The dummy segments in the error tests are required because the writer's run loop would otherwise continue forever
     # due to the segment's future result being None (no requests result), and we can't await the end of the stream
     # without waiting for the stream's timeout error. The dummy segments ensure that we can call await_write for these
     # successful segments, so we can close the stream afterwards and safely make the test assertions.
     # The EventedHLSStreamWriter could also implement await_fetch, but this is unnecessarily more complex than it already is.
 
@@ -268,15 +386,15 @@
         assert self.mocks[self.url(s3)].last_request._request.headers["Range"] == "bytes=15-25"
         assert self.mocks[self.url(s4)].last_request._request.headers["Range"] == "bytes=13-29"
         assert self.mocks[self.url(s5)].last_request._request.headers["Range"] == "bytes=30-48"
 
 
 @patch("streamlink.stream.hls.HLSStreamWorker.wait", Mock(return_value=True))
 class TestHLSStreamEncrypted(TestMixinStreamHLS, unittest.TestCase):
-    __stream__ = EventedHLSStream
+    __stream__ = EventedWriterHLSStream
 
     def get_session(self, options=None, *args, **kwargs):
         session = super().get_session(options)
         session.set_option("hls-live-edge", 3)
         session.set_option("http-headers", {"X-FOO": "BAR"})
 
         return session
@@ -568,15 +686,15 @@
         time = self.subject([Playlist(0, [], end=True, targetduration=0)], reload_time="default")
         assert time == 6, "sets reload time to 6 seconds when no data is available"
 
 
 @patch("streamlink.stream.hls.log")
 @patch("streamlink.stream.hls.HLSStreamWorker.wait", Mock(return_value=True))
 class TestHlsPlaylistParseErrors(TestMixinStreamHLS, unittest.TestCase):
-    __stream__ = EventedHLSStream
+    __stream__ = EventedWriterHLSStream
 
     class FakePlaylist(typing.NamedTuple):
         is_master: bool = False
         iframes_only: bool = False
 
     class InvalidPlaylist(Playlist):
         def build(self, *args, **kwargs):
```

### Comparing `streamlink-5.5.0/tests/stream/test_hls_filtered.py` & `streamlink-5.5.1/tests/stream/test_hls_filtered.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/stream/test_hls_playlist.py` & `streamlink-5.5.1/tests/stream/test_hls_playlist.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/stream/test_stream_json.py` & `streamlink-5.5.1/tests/stream/test_stream_json.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/stream/test_stream_to_url.py` & `streamlink-5.5.1/tests/stream/test_stream_to_url.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/stream/test_stream_wrappers.py` & `streamlink-5.5.1/tests/stream/test_stream_wrappers.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/test_api_http_session.py` & `streamlink-5.5.1/tests/test_api_http_session.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/test_api_validate.py` & `streamlink-5.5.1/tests/test_api_validate.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/test_api_websocket.py` & `streamlink-5.5.1/tests/test_api_websocket.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/test_buffers.py` & `streamlink-5.5.1/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/test_cache.py` & `streamlink-5.5.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/test_logger.py` & `streamlink-5.5.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/test_options.py` & `streamlink-5.5.1/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/test_plugin.py` & `streamlink-5.5.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/test_plugin_userinput.py` & `streamlink-5.5.1/tests/test_plugin_userinput.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/test_plugins.py` & `streamlink-5.5.1/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/test_session.py` & `streamlink-5.5.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/test_streamlink_api.py` & `streamlink-5.5.1/tests/test_streamlink_api.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/testutils/handshake.py` & `streamlink-5.5.1/tests/testutils/handshake.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/testutils/test_handshake.py` & `streamlink-5.5.1/tests/testutils/test_handshake.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/utils/test_args.py` & `streamlink-5.5.1/tests/utils/test_args.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/utils/test_cache.py` & `streamlink-5.5.1/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/utils/test_crypto.py` & `streamlink-5.5.1/tests/utils/test_crypto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/utils/test_data.py` & `streamlink-5.5.1/tests/utils/test_data.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/utils/test_formatter.py` & `streamlink-5.5.1/tests/utils/test_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/utils/test_l10n.py` & `streamlink-5.5.1/tests/utils/test_l10n.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/utils/test_module.py` & `streamlink-5.5.1/tests/utils/test_module.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/utils/test_named_pipe.py` & `streamlink-5.5.1/tests/utils/test_named_pipe.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/utils/test_parse.py` & `streamlink-5.5.1/tests/utils/test_parse.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/utils/test_processoutput.py` & `streamlink-5.5.1/tests/utils/test_processoutput.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/utils/test_times.py` & `streamlink-5.5.1/tests/utils/test_times.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.0/tests/utils/test_url.py` & `streamlink-5.5.1/tests/utils/test_url.py`

 * *Files identical despite different names*

