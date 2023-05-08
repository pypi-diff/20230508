# Comparing `tmp/matlab-proxy-0.5.8.tar.gz` & `tmp/matlab-proxy-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matlab-proxy-0.5.8.tar", last modified: Fri Feb 24 07:04:31 2023, max compression
+gzip compressed data, was "matlab-proxy-0.5.9.tar", last modified: Wed Apr 26 05:20:09 2023, max compression
```

## Comparing `matlab-proxy-0.5.8.tar` & `matlab-proxy-0.5.9.tar`

### file list

```diff
@@ -1,164 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.741066 matlab-proxy-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-02-24 07:04:31.741066 matlab-proxy-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.725065 matlab-proxy-0.5.8/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/README.md
--rw-r--r--   0 runner    (1001) docker     (123)  1276762 2023-02-24 07:04:12.000000 matlab-proxy-0.5.8/gui/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.725065 matlab-proxy-0.5.8/gui/public/
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/public/authorization.html
--rw-r--r--   0 runner    (1001) docker     (123)   121457 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/public/bootstrap.3.4.1.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   130876 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/public/navbar.css
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/public/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/public/signin.css
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/public/token.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.729065 matlab-proxy-0.5.8/gui/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.729065 matlab-proxy-0.5.8/gui/src/actionCreators/
--rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/actionCreators/actionCreators.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/actionCreators/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.729065 matlab-proxy-0.5.8/gui/src/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/actions/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.721065 matlab-proxy-0.5.8/gui/src/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.729065 matlab-proxy-0.5.8/gui/src/components/App/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.721065 matlab-proxy-0.5.8/gui/src/components/App/3p/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.729065 matlab-proxy-0.5.8/gui/src/components/App/3p/css/
--rw-r--r--   0 runner    (1001) docker     (123)   121200 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   153678 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/css/site7.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.733065 matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks-eps.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks-eps.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks-eps.woff
--rw-r--r--   0 runner    (1001) docker     (123)   289658 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks-pictograms.svg
--rw-r--r--   0 runner    (1001) docker     (123)    70212 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    70288 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks-pictograms.woff
--rw-r--r--   0 runner    (1001) docker     (123)   138707 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks.svg
--rw-r--r--   0 runner    (1001) docker     (123)    38656 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    38732 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.721065 matlab-proxy-0.5.8/gui/src/components/App/3p/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.733065 matlab-proxy-0.5.8/gui/src/components/App/3p/images/bug_reports/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/images/bug_reports/workaround.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.721065 matlab-proxy-0.5.8/gui/src/components/App/3p/images/responsive/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.733065 matlab-proxy-0.5.8/gui/src/components/App/3p/images/responsive/global/
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/3p/images/responsive/global/ico-sprite.png
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/App.css
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/App.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/App/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.733065 matlab-proxy-0.5.8/gui/src/components/Confirmation/
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Confirmation/Confirmation.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Confirmation/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.733065 matlab-proxy-0.5.8/gui/src/components/Controls/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Controls/Controls.css
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Controls/Controls.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Controls/feedback.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Controls/help.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Controls/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Controls/restart.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Controls/sign-out.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Controls/start.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Controls/stop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Controls/terminate.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.733065 matlab-proxy-0.5.8/gui/src/components/Error/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Error/Error.css
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Error/Error.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Error/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.733065 matlab-proxy-0.5.8/gui/src/components/Help/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Help/Help.css
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Help/Help.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Help/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.733065 matlab-proxy-0.5.8/gui/src/components/Information/
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Information/Information.css
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Information/Information.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Information/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.733065 matlab-proxy-0.5.8/gui/src/components/LicensingGatherer/
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/LicensingGatherer/LicensingGatherer.css
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/LicensingGatherer/MHLM.js
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/LicensingGatherer/NLM.js
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/LicensingGatherer/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.737066 matlab-proxy-0.5.8/gui/src/components/MatlabJsd/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/MatlabJsd/MatlabJsd.css
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/MatlabJsd/MatlabJsd.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/MatlabJsd/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.737066 matlab-proxy-0.5.8/gui/src/components/Overlay/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Overlay/Overlay.css
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Overlay/Overlay.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/Overlay/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.737066 matlab-proxy-0.5.8/gui/src/components/OverlayTrigger/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/OverlayTrigger/OverlayTrigger.css
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/OverlayTrigger/arrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/OverlayTrigger/gripper.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/OverlayTrigger/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/OverlayTrigger/trigger-error.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/components/OverlayTrigger/trigger-ok.svg
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/jest.config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.737066 matlab-proxy-0.5.8/gui/src/reducers/
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/reducers/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/reducers/reducers.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.737066 matlab-proxy-0.5.8/gui/src/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/selectors/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/selectors/selectors.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/serviceWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/setupTests.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.721065 matlab-proxy-0.5.8/gui/src/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.737066 matlab-proxy-0.5.8/gui/src/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/gui/src/test/utils/react-test.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.737066 matlab-proxy-0.5.8/matlab_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23776 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    44905 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/app_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/default_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/devel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.737066 matlab-proxy-0.5.8/matlab_proxy/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/icons/matlab.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.737066 matlab-proxy-0.5.8/matlab_proxy/matlab/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1532 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/matlab/startup.m
--rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.741066 matlab-proxy-0.5.8/matlab_proxy/util/
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/util/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/util/list_servers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/util/mw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.741066 matlab-proxy-0.5.8/matlab_proxy/util/mwi/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/util/mwi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/util/mwi/custom_http_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.741066 matlab-proxy-0.5.8/matlab_proxy/util/mwi/embedded_connector/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/util/mwi/embedded_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/util/mwi/embedded_connector/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/util/mwi/embedded_connector/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/util/mwi/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/util/mwi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/util/mwi/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/util/mwi/token_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/util/mwi/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/util/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/matlab_proxy/util/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 07:04:31.737066 matlab-proxy-0.5.8/matlab_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-02-24 07:03:51.000000 matlab-proxy-0.5.8/matlab_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-02-24 07:03:51.000000 matlab-proxy-0.5.8/matlab_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 07:03:51.000000 matlab-proxy-0.5.8/matlab_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-24 07:03:51.000000 matlab-proxy-0.5.8/matlab_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 07:03:51.000000 matlab-proxy-0.5.8/matlab_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-24 07:03:51.000000 matlab-proxy-0.5.8/matlab_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-24 07:03:51.000000 matlab-proxy-0.5.8/matlab_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-24 07:04:31.741066 matlab-proxy-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-02-24 07:03:18.000000 matlab-proxy-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.964679 matlab-proxy-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-04-26 05:20:09.964679 matlab-proxy-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.952679 matlab-proxy-0.5.9/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)  1276762 2023-04-26 05:19:52.000000 matlab-proxy-0.5.9/gui/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.952679 matlab-proxy-0.5.9/gui/public/
+-rw-r--r--   0 runner    (1001) docker     (123)   130876 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.952679 matlab-proxy-0.5.9/gui/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.952679 matlab-proxy-0.5.9/gui/src/actionCreators/
+-rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/actionCreators/actionCreators.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/actionCreators/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.952679 matlab-proxy-0.5.9/gui/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/actions/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.948679 matlab-proxy-0.5.9/gui/src/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.952679 matlab-proxy-0.5.9/gui/src/components/App/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.948679 matlab-proxy-0.5.9/gui/src/components/App/3p/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.952679 matlab-proxy-0.5.9/gui/src/components/App/3p/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   121200 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   153678 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/css/site7.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.956679 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-eps.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-eps.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-eps.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   289658 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-pictograms.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    70212 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    70288 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-pictograms.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   138707 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    38656 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    38732 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.948679 matlab-proxy-0.5.9/gui/src/components/App/3p/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.956679 matlab-proxy-0.5.9/gui/src/components/App/3p/images/bug_reports/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/images/bug_reports/workaround.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.948679 matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.956679 matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-sprite.png
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/App.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/App.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)   220290 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/MATLAB-env-blur.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.956679 matlab-proxy-0.5.9/gui/src/components/Confirmation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Confirmation/Confirmation.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Confirmation/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.956679 matlab-proxy-0.5.9/gui/src/components/Controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/Controls.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/Controls.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/feedback.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/help.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/restart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/sign-out.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/start.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/terminate.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.956679 matlab-proxy-0.5.9/gui/src/components/Error/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Error/Error.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Error/Error.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Error/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.956679 matlab-proxy-0.5.9/gui/src/components/Help/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Help/Help.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Help/Help.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Help/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/gui/src/components/Information/
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Information/Information.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Information/Information.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Information/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/LicensingGatherer.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/MHLM.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/NLM.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/gui/src/components/MatlabJsd/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/MatlabJsd/MatlabJsd.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/MatlabJsd/MatlabJsd.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/MatlabJsd/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/gui/src/components/Overlay/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Overlay/Overlay.css
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Overlay/Overlay.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Overlay/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/OverlayTrigger.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/gripper.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/trigger-error.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/trigger-ok.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/jest.config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/gui/src/reducers/
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/reducers/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14469 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/reducers/reducers.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/gui/src/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/selectors/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/selectors/selectors.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/serviceWorker.js
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/setupTests.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.948679 matlab-proxy-0.5.9/gui/src/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/gui/src/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/test/utils/react-test.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/matlab_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23827 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44905 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/app_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/default_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/devel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/matlab_proxy/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/icons/matlab.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/matlab_proxy/matlab/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1532 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/matlab/startup.m
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.964679 matlab-proxy-0.5.9/matlab_proxy/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/list_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.964679 matlab-proxy-0.5.9/matlab_proxy/util/mwi/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/custom_http_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.964679 matlab-proxy-0.5.9/matlab_proxy/util/mwi/embedded_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/embedded_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/embedded_connector/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/embedded_connector/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/token_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/matlab_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-04-26 05:19:30.000000 matlab-proxy-0.5.9/matlab_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-04-26 05:19:30.000000 matlab-proxy-0.5.9/matlab_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:19:30.000000 matlab-proxy-0.5.9/matlab_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-26 05:19:30.000000 matlab-proxy-0.5.9/matlab_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:19:30.000000 matlab-proxy-0.5.9/matlab_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-26 05:19:30.000000 matlab-proxy-0.5.9/matlab_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 05:19:30.000000 matlab-proxy-0.5.9/matlab_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 05:20:09.964679 matlab-proxy-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/setup.py
```

### Comparing `matlab-proxy-0.5.8/LICENSE.md` & `matlab-proxy-0.5.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/PKG-INFO` & `matlab-proxy-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matlab-proxy
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python® package enables you to launch MATLAB® and access it from a web browser.
 Home-page: https://github.com/mathworks/matlab-proxy/
 Author: The MathWorks, Inc.
 Author-email: cloud@mathworks.com
 License: MATHWORKS CLOUD REFERENCE ARCHITECTURE LICENSE
 Description: # MATLAB Proxy
         [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mathworks/matlab-proxy/run-tests.yml?branch=main&logo=github)](https://github.com/mathworks/matlab-proxy/actions) &nbsp; [![PyPI badge](https://img.shields.io/pypi/v/matlab-proxy.svg?logo=pypi)](https://pypi.python.org/pypi/matlab-proxy) &nbsp;  [![codecov](https://codecov.io/gh/mathworks/matlab-proxy/branch/main/graph/badge.svg?token=ZW3SESKCSS)](https://codecov.io/gh/mathworks/matlab-proxy) &nbsp; [![Downloads](https://static.pepy.tech/personalized-badge/matlab-proxy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20downloads/month)](https://pepy.tech/project/matlab-proxy)
```

### Comparing `matlab-proxy-0.5.8/README.md` & `matlab-proxy-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/README.md` & `matlab-proxy-0.5.9/gui/README.md`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/package-lock.json` & `matlab-proxy-0.5.9/gui/package-lock.json`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/package.json` & `matlab-proxy-0.5.9/gui/package.json`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/public/bootstrap.3.4.1.min.css` & `matlab-proxy-0.5.9/gui/src/components/App/3p/css/bootstrap.min.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 /*!
- * Bootstrap v3.4.1 (https://getbootstrap.com/)
- * Copyright 2011-2019 Twitter, Inc.
+ * Bootstrap v3.3.7 (http://getbootstrap.com)
+ * Copyright 2011-2016 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
- *//*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */html{font-family:sans-serif;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%}body{margin:0}article,aside,details,figcaption,figure,footer,header,hgroup,main,menu,nav,section,summary{display:block}audio,canvas,progress,video{display:inline-block;vertical-align:baseline}audio:not([controls]){display:none;height:0}[hidden],template{display:none}a{background-color:transparent}a:active,a:hover{outline:0}abbr[title]{border-bottom:none;text-decoration:underline;-webkit-text-decoration:underline dotted;-moz-text-decoration:underline dotted;text-decoration:underline dotted}b,strong{font-weight:700}dfn{font-style:italic}h1{font-size:2em;margin:.67em 0}mark{background:#ff0;color:#000}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sup{top:-.5em}sub{bottom:-.25em}img{border:0}svg:not(:root){overflow:hidden}figure{margin:1em 40px}hr{-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box;height:0}pre{overflow:auto}code,kbd,pre,samp{font-family:monospace,monospace;font-size:1em}button,input,optgroup,select,textarea{color:inherit;font:inherit;margin:0}button{overflow:visible}button,select{text-transform:none}button,html input[type=button],input[type=reset],input[type=submit]{-webkit-appearance:button;cursor:pointer}button[disabled],html input[disabled]{cursor:default}button::-moz-focus-inner,input::-moz-focus-inner{border:0;padding:0}input{line-height:normal}input[type=checkbox],input[type=radio]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;padding:0}input[type=number]::-webkit-inner-spin-button,input[type=number]::-webkit-outer-spin-button{height:auto}input[type=search]{-webkit-appearance:textfield;-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box}input[type=search]::-webkit-search-cancel-button,input[type=search]::-webkit-search-decoration{-webkit-appearance:none}fieldset{border:1px solid silver;margin:0 2px;padding:.35em .625em .75em}legend{border:0;padding:0}textarea{overflow:auto}optgroup{font-weight:700}table{border-collapse:collapse;border-spacing:0}td,th{padding:0}/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */@media print{*,:after,:before{color:#000!important;text-shadow:none!important;background:0 0!important;-webkit-box-shadow:none!important;box-shadow:none!important}a,a:visited{text-decoration:underline}a[href]:after{content:" (" attr(href) ")"}abbr[title]:after{content:" (" attr(title) ")"}a[href^="#"]:after,a[href^="javascript:"]:after{content:""}blockquote,pre{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}img,tr{page-break-inside:avoid}img{max-width:100%!important}h2,h3,p{orphans:3;widows:3}h2,h3{page-break-after:avoid}.navbar{display:none}.btn>.caret,.dropup>.btn>.caret{border-top-color:#000!important}.label{border:1px solid #000}.table{border-collapse:collapse!important}.table td,.table th{background-color:#fff!important}.table-bordered td,.table-bordered th{border:1px solid #ddd!important}}@font-face{font-family:"Glyphicons Halflings";src:url(../fonts/glyphicons-halflings-regular.eot);src:url(../fonts/glyphicons-halflings-regular.eot?#iefix) format("embedded-opentype"),url(../fonts/glyphicons-halflings-regular.woff2) format("woff2"),url(../fonts/glyphicons-halflings-regular.woff) format("woff"),url(../fonts/glyphicons-halflings-regular.ttf) format("truetype"),url(../fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular) format("svg")}.glyphicon{position:relative;top:1px;display:inline-block;font-family:"Glyphicons Halflings";font-style:normal;font-weight:400;line-height:1;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.glyphicon-asterisk:before{content:"\002a"}.glyphicon-plus:before{content:"\002b"}.glyphicon-eur:before,.glyphicon-euro:before{content:"\20ac"}.glyphicon-minus:before{content:"\2212"}.glyphicon-cloud:before{content:"\2601"}.glyphicon-envelope:before{content:"\2709"}.glyphicon-pencil:before{content:"\270f"}.glyphicon-glass:before{content:"\e001"}.glyphicon-music:before{content:"\e002"}.glyphicon-search:before{content:"\e003"}.glyphicon-heart:before{content:"\e005"}.glyphicon-star:before{content:"\e006"}.glyphicon-star-empty:before{content:"\e007"}.glyphicon-user:before{content:"\e008"}.glyphicon-film:before{content:"\e009"}.glyphicon-th-large:before{content:"\e010"}.glyphicon-th:before{content:"\e011"}.glyphicon-th-list:before{content:"\e012"}.glyphicon-ok:before{content:"\e013"}.glyphicon-remove:before{content:"\e014"}.glyphicon-zoom-in:before{content:"\e015"}.glyphicon-zoom-out:before{content:"\e016"}.glyphicon-off:before{content:"\e017"}.glyphicon-signal:before{content:"\e018"}.glyphicon-cog:before{content:"\e019"}.glyphicon-trash:before{content:"\e020"}.glyphicon-home:before{content:"\e021"}.glyphicon-file:before{content:"\e022"}.glyphicon-time:before{content:"\e023"}.glyphicon-road:before{content:"\e024"}.glyphicon-download-alt:before{content:"\e025"}.glyphicon-download:before{content:"\e026"}.glyphicon-upload:before{content:"\e027"}.glyphicon-inbox:before{content:"\e028"}.glyphicon-play-circle:before{content:"\e029"}.glyphicon-repeat:before{content:"\e030"}.glyphicon-refresh:before{content:"\e031"}.glyphicon-list-alt:before{content:"\e032"}.glyphicon-lock:before{content:"\e033"}.glyphicon-flag:before{content:"\e034"}.glyphicon-headphones:before{content:"\e035"}.glyphicon-volume-off:before{content:"\e036"}.glyphicon-volume-down:before{content:"\e037"}.glyphicon-volume-up:before{content:"\e038"}.glyphicon-qrcode:before{content:"\e039"}.glyphicon-barcode:before{content:"\e040"}.glyphicon-tag:before{content:"\e041"}.glyphicon-tags:before{content:"\e042"}.glyphicon-book:before{content:"\e043"}.glyphicon-bookmark:before{content:"\e044"}.glyphicon-print:before{content:"\e045"}.glyphicon-camera:before{content:"\e046"}.glyphicon-font:before{content:"\e047"}.glyphicon-bold:before{content:"\e048"}.glyphicon-italic:before{content:"\e049"}.glyphicon-text-height:before{content:"\e050"}.glyphicon-text-width:before{content:"\e051"}.glyphicon-align-left:before{content:"\e052"}.glyphicon-align-center:before{content:"\e053"}.glyphicon-align-right:before{content:"\e054"}.glyphicon-align-justify:before{content:"\e055"}.glyphicon-list:before{content:"\e056"}.glyphicon-indent-left:before{content:"\e057"}.glyphicon-indent-right:before{content:"\e058"}.glyphicon-facetime-video:before{content:"\e059"}.glyphicon-picture:before{content:"\e060"}.glyphicon-map-marker:before{content:"\e062"}.glyphicon-adjust:before{content:"\e063"}.glyphicon-tint:before{content:"\e064"}.glyphicon-edit:before{content:"\e065"}.glyphicon-share:before{content:"\e066"}.glyphicon-check:before{content:"\e067"}.glyphicon-move:before{content:"\e068"}.glyphicon-step-backward:before{content:"\e069"}.glyphicon-fast-backward:before{content:"\e070"}.glyphicon-backward:before{content:"\e071"}.glyphicon-play:before{content:"\e072"}.glyphicon-pause:before{content:"\e073"}.glyphicon-stop:before{content:"\e074"}.glyphicon-forward:before{content:"\e075"}.glyphicon-fast-forward:before{content:"\e076"}.glyphicon-step-forward:before{content:"\e077"}.glyphicon-eject:before{content:"\e078"}.glyphicon-chevron-left:before{content:"\e079"}.glyphicon-chevron-right:before{content:"\e080"}.glyphicon-plus-sign:before{content:"\e081"}.glyphicon-minus-sign:before{content:"\e082"}.glyphicon-remove-sign:before{content:"\e083"}.glyphicon-ok-sign:before{content:"\e084"}.glyphicon-question-sign:before{content:"\e085"}.glyphicon-info-sign:before{content:"\e086"}.glyphicon-screenshot:before{content:"\e087"}.glyphicon-remove-circle:before{content:"\e088"}.glyphicon-ok-circle:before{content:"\e089"}.glyphicon-ban-circle:before{content:"\e090"}.glyphicon-arrow-left:before{content:"\e091"}.glyphicon-arrow-right:before{content:"\e092"}.glyphicon-arrow-up:before{content:"\e093"}.glyphicon-arrow-down:before{content:"\e094"}.glyphicon-share-alt:before{content:"\e095"}.glyphicon-resize-full:before{content:"\e096"}.glyphicon-resize-small:before{content:"\e097"}.glyphicon-exclamation-sign:before{content:"\e101"}.glyphicon-gift:before{content:"\e102"}.glyphicon-leaf:before{content:"\e103"}.glyphicon-fire:before{content:"\e104"}.glyphicon-eye-open:before{content:"\e105"}.glyphicon-eye-close:before{content:"\e106"}.glyphicon-warning-sign:before{content:"\e107"}.glyphicon-plane:before{content:"\e108"}.glyphicon-calendar:before{content:"\e109"}.glyphicon-random:before{content:"\e110"}.glyphicon-comment:before{content:"\e111"}.glyphicon-magnet:before{content:"\e112"}.glyphicon-chevron-up:before{content:"\e113"}.glyphicon-chevron-down:before{content:"\e114"}.glyphicon-retweet:before{content:"\e115"}.glyphicon-shopping-cart:before{content:"\e116"}.glyphicon-folder-close:before{content:"\e117"}.glyphicon-folder-open:before{content:"\e118"}.glyphicon-resize-vertical:before{content:"\e119"}.glyphicon-resize-horizontal:before{content:"\e120"}.glyphicon-hdd:before{content:"\e121"}.glyphicon-bullhorn:before{content:"\e122"}.glyphicon-bell:before{content:"\e123"}.glyphicon-certificate:before{content:"\e124"}.glyphicon-thumbs-up:before{content:"\e125"}.glyphicon-thumbs-down:before{content:"\e126"}.glyphicon-hand-right:before{content:"\e127"}.glyphicon-hand-left:before{content:"\e128"}.glyphicon-hand-up:before{content:"\e129"}.glyphicon-hand-down:before{content:"\e130"}.glyphicon-circle-arrow-right:before{content:"\e131"}.glyphicon-circle-arrow-left:before{content:"\e132"}.glyphicon-circle-arrow-up:before{content:"\e133"}.glyphicon-circle-arrow-down:before{content:"\e134"}.glyphicon-globe:before{content:"\e135"}.glyphicon-wrench:before{content:"\e136"}.glyphicon-tasks:before{content:"\e137"}.glyphicon-filter:before{content:"\e138"}.glyphicon-briefcase:before{content:"\e139"}.glyphicon-fullscreen:before{content:"\e140"}.glyphicon-dashboard:before{content:"\e141"}.glyphicon-paperclip:before{content:"\e142"}.glyphicon-heart-empty:before{content:"\e143"}.glyphicon-link:before{content:"\e144"}.glyphicon-phone:before{content:"\e145"}.glyphicon-pushpin:before{content:"\e146"}.glyphicon-usd:before{content:"\e148"}.glyphicon-gbp:before{content:"\e149"}.glyphicon-sort:before{content:"\e150"}.glyphicon-sort-by-alphabet:before{content:"\e151"}.glyphicon-sort-by-alphabet-alt:before{content:"\e152"}.glyphicon-sort-by-order:before{content:"\e153"}.glyphicon-sort-by-order-alt:before{content:"\e154"}.glyphicon-sort-by-attributes:before{content:"\e155"}.glyphicon-sort-by-attributes-alt:before{content:"\e156"}.glyphicon-unchecked:before{content:"\e157"}.glyphicon-expand:before{content:"\e158"}.glyphicon-collapse-down:before{content:"\e159"}.glyphicon-collapse-up:before{content:"\e160"}.glyphicon-log-in:before{content:"\e161"}.glyphicon-flash:before{content:"\e162"}.glyphicon-log-out:before{content:"\e163"}.glyphicon-new-window:before{content:"\e164"}.glyphicon-record:before{content:"\e165"}.glyphicon-save:before{content:"\e166"}.glyphicon-open:before{content:"\e167"}.glyphicon-saved:before{content:"\e168"}.glyphicon-import:before{content:"\e169"}.glyphicon-export:before{content:"\e170"}.glyphicon-send:before{content:"\e171"}.glyphicon-floppy-disk:before{content:"\e172"}.glyphicon-floppy-saved:before{content:"\e173"}.glyphicon-floppy-remove:before{content:"\e174"}.glyphicon-floppy-save:before{content:"\e175"}.glyphicon-floppy-open:before{content:"\e176"}.glyphicon-credit-card:before{content:"\e177"}.glyphicon-transfer:before{content:"\e178"}.glyphicon-cutlery:before{content:"\e179"}.glyphicon-header:before{content:"\e180"}.glyphicon-compressed:before{content:"\e181"}.glyphicon-earphone:before{content:"\e182"}.glyphicon-phone-alt:before{content:"\e183"}.glyphicon-tower:before{content:"\e184"}.glyphicon-stats:before{content:"\e185"}.glyphicon-sd-video:before{content:"\e186"}.glyphicon-hd-video:before{content:"\e187"}.glyphicon-subtitles:before{content:"\e188"}.glyphicon-sound-stereo:before{content:"\e189"}.glyphicon-sound-dolby:before{content:"\e190"}.glyphicon-sound-5-1:before{content:"\e191"}.glyphicon-sound-6-1:before{content:"\e192"}.glyphicon-sound-7-1:before{content:"\e193"}.glyphicon-copyright-mark:before{content:"\e194"}.glyphicon-registration-mark:before{content:"\e195"}.glyphicon-cloud-download:before{content:"\e197"}.glyphicon-cloud-upload:before{content:"\e198"}.glyphicon-tree-conifer:before{content:"\e199"}.glyphicon-tree-deciduous:before{content:"\e200"}.glyphicon-cd:before{content:"\e201"}.glyphicon-save-file:before{content:"\e202"}.glyphicon-open-file:before{content:"\e203"}.glyphicon-level-up:before{content:"\e204"}.glyphicon-copy:before{content:"\e205"}.glyphicon-paste:before{content:"\e206"}.glyphicon-alert:before{content:"\e209"}.glyphicon-equalizer:before{content:"\e210"}.glyphicon-king:before{content:"\e211"}.glyphicon-queen:before{content:"\e212"}.glyphicon-pawn:before{content:"\e213"}.glyphicon-bishop:before{content:"\e214"}.glyphicon-knight:before{content:"\e215"}.glyphicon-baby-formula:before{content:"\e216"}.glyphicon-tent:before{content:"\26fa"}.glyphicon-blackboard:before{content:"\e218"}.glyphicon-bed:before{content:"\e219"}.glyphicon-apple:before{content:"\f8ff"}.glyphicon-erase:before{content:"\e221"}.glyphicon-hourglass:before{content:"\231b"}.glyphicon-lamp:before{content:"\e223"}.glyphicon-duplicate:before{content:"\e224"}.glyphicon-piggy-bank:before{content:"\e225"}.glyphicon-scissors:before{content:"\e226"}.glyphicon-bitcoin:before{content:"\e227"}.glyphicon-btc:before{content:"\e227"}.glyphicon-xbt:before{content:"\e227"}.glyphicon-yen:before{content:"\00a5"}.glyphicon-jpy:before{content:"\00a5"}.glyphicon-ruble:before{content:"\20bd"}.glyphicon-rub:before{content:"\20bd"}.glyphicon-scale:before{content:"\e230"}.glyphicon-ice-lolly:before{content:"\e231"}.glyphicon-ice-lolly-tasted:before{content:"\e232"}.glyphicon-education:before{content:"\e233"}.glyphicon-option-horizontal:before{content:"\e234"}.glyphicon-option-vertical:before{content:"\e235"}.glyphicon-menu-hamburger:before{content:"\e236"}.glyphicon-modal-window:before{content:"\e237"}.glyphicon-oil:before{content:"\e238"}.glyphicon-grain:before{content:"\e239"}.glyphicon-sunglasses:before{content:"\e240"}.glyphicon-text-size:before{content:"\e241"}.glyphicon-text-color:before{content:"\e242"}.glyphicon-text-background:before{content:"\e243"}.glyphicon-object-align-top:before{content:"\e244"}.glyphicon-object-align-bottom:before{content:"\e245"}.glyphicon-object-align-horizontal:before{content:"\e246"}.glyphicon-object-align-left:before{content:"\e247"}.glyphicon-object-align-vertical:before{content:"\e248"}.glyphicon-object-align-right:before{content:"\e249"}.glyphicon-triangle-right:before{content:"\e250"}.glyphicon-triangle-left:before{content:"\e251"}.glyphicon-triangle-bottom:before{content:"\e252"}.glyphicon-triangle-top:before{content:"\e253"}.glyphicon-console:before{content:"\e254"}.glyphicon-superscript:before{content:"\e255"}.glyphicon-subscript:before{content:"\e256"}.glyphicon-menu-left:before{content:"\e257"}.glyphicon-menu-right:before{content:"\e258"}.glyphicon-menu-down:before{content:"\e259"}.glyphicon-menu-up:before{content:"\e260"}*{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}:after,:before{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}html{font-size:10px;-webkit-tap-highlight-color:rgba(0,0,0,0)}body{font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-size:14px;line-height:1.42857143;color:#333;background-color:#fff}button,input,select,textarea{font-family:inherit;font-size:inherit;line-height:inherit}a{color:#337ab7;text-decoration:none}a:focus,a:hover{color:#23527c;text-decoration:underline}a:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}figure{margin:0}img{vertical-align:middle}.carousel-inner>.item>a>img,.carousel-inner>.item>img,.img-responsive,.thumbnail a>img,.thumbnail>img{display:block;max-width:100%;height:auto}.img-rounded{border-radius:6px}.img-thumbnail{padding:4px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:all .2s ease-in-out;-o-transition:all .2s ease-in-out;transition:all .2s ease-in-out;display:inline-block;max-width:100%;height:auto}.img-circle{border-radius:50%}hr{margin-top:20px;margin-bottom:20px;border:0;border-top:1px solid #eee}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);border:0}.sr-only-focusable:active,.sr-only-focusable:focus{position:static;width:auto;height:auto;margin:0;overflow:visible;clip:auto}[role=button]{cursor:pointer}.h1,.h2,.h3,.h4,.h5,.h6,h1,h2,h3,h4,h5,h6{font-family:inherit;font-weight:500;line-height:1.1;color:inherit}.h1 .small,.h1 small,.h2 .small,.h2 small,.h3 .small,.h3 small,.h4 .small,.h4 small,.h5 .small,.h5 small,.h6 .small,.h6 small,h1 .small,h1 small,h2 .small,h2 small,h3 .small,h3 small,h4 .small,h4 small,h5 .small,h5 small,h6 .small,h6 small{font-weight:400;line-height:1;color:#777}.h1,.h2,.h3,h1,h2,h3{margin-top:20px;margin-bottom:10px}.h1 .small,.h1 small,.h2 .small,.h2 small,.h3 .small,.h3 small,h1 .small,h1 small,h2 .small,h2 small,h3 .small,h3 small{font-size:65%}.h4,.h5,.h6,h4,h5,h6{margin-top:10px;margin-bottom:10px}.h4 .small,.h4 small,.h5 .small,.h5 small,.h6 .small,.h6 small,h4 .small,h4 small,h5 .small,h5 small,h6 .small,h6 small{font-size:75%}.h1,h1{font-size:36px}.h2,h2{font-size:30px}.h3,h3{font-size:24px}.h4,h4{font-size:18px}.h5,h5{font-size:14px}.h6,h6{font-size:12px}p{margin:0 0 10px}.lead{margin-bottom:20px;font-size:16px;font-weight:300;line-height:1.4}@media (min-width:768px){.lead{font-size:21px}}.small,small{font-size:85%}.mark,mark{padding:.2em;background-color:#fcf8e3}.text-left{text-align:left}.text-right{text-align:right}.text-center{text-align:center}.text-justify{text-align:justify}.text-nowrap{white-space:nowrap}.text-lowercase{text-transform:lowercase}.text-uppercase{text-transform:uppercase}.text-capitalize{text-transform:capitalize}.text-muted{color:#777}.text-primary{color:#337ab7}a.text-primary:focus,a.text-primary:hover{color:#286090}.text-success{color:#3c763d}a.text-success:focus,a.text-success:hover{color:#2b542c}.text-info{color:#31708f}a.text-info:focus,a.text-info:hover{color:#245269}.text-warning{color:#8a6d3b}a.text-warning:focus,a.text-warning:hover{color:#66512c}.text-danger{color:#a94442}a.text-danger:focus,a.text-danger:hover{color:#843534}.bg-primary{color:#fff;background-color:#337ab7}a.bg-primary:focus,a.bg-primary:hover{background-color:#286090}.bg-success{background-color:#dff0d8}a.bg-success:focus,a.bg-success:hover{background-color:#c1e2b3}.bg-info{background-color:#d9edf7}a.bg-info:focus,a.bg-info:hover{background-color:#afd9ee}.bg-warning{background-color:#fcf8e3}a.bg-warning:focus,a.bg-warning:hover{background-color:#f7ecb5}.bg-danger{background-color:#f2dede}a.bg-danger:focus,a.bg-danger:hover{background-color:#e4b9b9}.page-header{padding-bottom:9px;margin:40px 0 20px;border-bottom:1px solid #eee}ol,ul{margin-top:0;margin-bottom:10px}ol ol,ol ul,ul ol,ul ul{margin-bottom:0}.list-unstyled{padding-left:0;list-style:none}.list-inline{padding-left:0;list-style:none;margin-left:-5px}.list-inline>li{display:inline-block;padding-right:5px;padding-left:5px}dl{margin-top:0;margin-bottom:20px}dd,dt{line-height:1.42857143}dt{font-weight:700}dd{margin-left:0}@media (min-width:768px){.dl-horizontal dt{float:left;width:160px;clear:left;text-align:right;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.dl-horizontal dd{margin-left:180px}}abbr[data-original-title],abbr[title]{cursor:help}.initialism{font-size:90%;text-transform:uppercase}blockquote{padding:10px 20px;margin:0 0 20px;font-size:17.5px;border-left:5px solid #eee}blockquote ol:last-child,blockquote p:last-child,blockquote ul:last-child{margin-bottom:0}blockquote .small,blockquote footer,blockquote small{display:block;font-size:80%;line-height:1.42857143;color:#777}blockquote .small:before,blockquote footer:before,blockquote small:before{content:"\2014 \00A0"}.blockquote-reverse,blockquote.pull-right{padding-right:15px;padding-left:0;text-align:right;border-right:5px solid #eee;border-left:0}.blockquote-reverse .small:before,.blockquote-reverse footer:before,.blockquote-reverse small:before,blockquote.pull-right .small:before,blockquote.pull-right footer:before,blockquote.pull-right small:before{content:""}.blockquote-reverse .small:after,.blockquote-reverse footer:after,.blockquote-reverse small:after,blockquote.pull-right .small:after,blockquote.pull-right footer:after,blockquote.pull-right small:after{content:"\00A0 \2014"}address{margin-bottom:20px;font-style:normal;line-height:1.42857143}code,kbd,pre,samp{font-family:Menlo,Monaco,Consolas,"Courier New",monospace}code{padding:2px 4px;font-size:90%;color:#c7254e;background-color:#f9f2f4;border-radius:4px}kbd{padding:2px 4px;font-size:90%;color:#fff;background-color:#333;border-radius:3px;-webkit-box-shadow:inset 0 -1px 0 rgba(0,0,0,.25);box-shadow:inset 0 -1px 0 rgba(0,0,0,.25)}kbd kbd{padding:0;font-size:100%;font-weight:700;-webkit-box-shadow:none;box-shadow:none}pre{display:block;padding:9.5px;margin:0 0 10px;font-size:13px;line-height:1.42857143;color:#333;word-break:break-all;word-wrap:break-word;background-color:#f5f5f5;border:1px solid #ccc;border-radius:4px}pre code{padding:0;font-size:inherit;color:inherit;white-space:pre-wrap;background-color:transparent;border-radius:0}.pre-scrollable{max-height:340px;overflow-y:scroll}.container{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}@media (min-width:768px){.container{width:750px}}@media (min-width:992px){.container{width:970px}}@media (min-width:1200px){.container{width:1170px}}.container-fluid{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}.row{margin-right:-15px;margin-left:-15px}.row-no-gutters{margin-right:0;margin-left:0}.row-no-gutters [class*=col-]{padding-right:0;padding-left:0}.col-lg-1,.col-lg-10,.col-lg-11,.col-lg-12,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9,.col-md-1,.col-md-10,.col-md-11,.col-md-12,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9,.col-sm-1,.col-sm-10,.col-sm-11,.col-sm-12,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9,.col-xs-1,.col-xs-10,.col-xs-11,.col-xs-12,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9{position:relative;min-height:1px;padding-right:15px;padding-left:15px}.col-xs-1,.col-xs-10,.col-xs-11,.col-xs-12,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9{float:left}.col-xs-12{width:100%}.col-xs-11{width:91.66666667%}.col-xs-10{width:83.33333333%}.col-xs-9{width:75%}.col-xs-8{width:66.66666667%}.col-xs-7{width:58.33333333%}.col-xs-6{width:50%}.col-xs-5{width:41.66666667%}.col-xs-4{width:33.33333333%}.col-xs-3{width:25%}.col-xs-2{width:16.66666667%}.col-xs-1{width:8.33333333%}.col-xs-pull-12{right:100%}.col-xs-pull-11{right:91.66666667%}.col-xs-pull-10{right:83.33333333%}.col-xs-pull-9{right:75%}.col-xs-pull-8{right:66.66666667%}.col-xs-pull-7{right:58.33333333%}.col-xs-pull-6{right:50%}.col-xs-pull-5{right:41.66666667%}.col-xs-pull-4{right:33.33333333%}.col-xs-pull-3{right:25%}.col-xs-pull-2{right:16.66666667%}.col-xs-pull-1{right:8.33333333%}.col-xs-pull-0{right:auto}.col-xs-push-12{left:100%}.col-xs-push-11{left:91.66666667%}.col-xs-push-10{left:83.33333333%}.col-xs-push-9{left:75%}.col-xs-push-8{left:66.66666667%}.col-xs-push-7{left:58.33333333%}.col-xs-push-6{left:50%}.col-xs-push-5{left:41.66666667%}.col-xs-push-4{left:33.33333333%}.col-xs-push-3{left:25%}.col-xs-push-2{left:16.66666667%}.col-xs-push-1{left:8.33333333%}.col-xs-push-0{left:auto}.col-xs-offset-12{margin-left:100%}.col-xs-offset-11{margin-left:91.66666667%}.col-xs-offset-10{margin-left:83.33333333%}.col-xs-offset-9{margin-left:75%}.col-xs-offset-8{margin-left:66.66666667%}.col-xs-offset-7{margin-left:58.33333333%}.col-xs-offset-6{margin-left:50%}.col-xs-offset-5{margin-left:41.66666667%}.col-xs-offset-4{margin-left:33.33333333%}.col-xs-offset-3{margin-left:25%}.col-xs-offset-2{margin-left:16.66666667%}.col-xs-offset-1{margin-left:8.33333333%}.col-xs-offset-0{margin-left:0}@media (min-width:768px){.col-sm-1,.col-sm-10,.col-sm-11,.col-sm-12,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9{float:left}.col-sm-12{width:100%}.col-sm-11{width:91.66666667%}.col-sm-10{width:83.33333333%}.col-sm-9{width:75%}.col-sm-8{width:66.66666667%}.col-sm-7{width:58.33333333%}.col-sm-6{width:50%}.col-sm-5{width:41.66666667%}.col-sm-4{width:33.33333333%}.col-sm-3{width:25%}.col-sm-2{width:16.66666667%}.col-sm-1{width:8.33333333%}.col-sm-pull-12{right:100%}.col-sm-pull-11{right:91.66666667%}.col-sm-pull-10{right:83.33333333%}.col-sm-pull-9{right:75%}.col-sm-pull-8{right:66.66666667%}.col-sm-pull-7{right:58.33333333%}.col-sm-pull-6{right:50%}.col-sm-pull-5{right:41.66666667%}.col-sm-pull-4{right:33.33333333%}.col-sm-pull-3{right:25%}.col-sm-pull-2{right:16.66666667%}.col-sm-pull-1{right:8.33333333%}.col-sm-pull-0{right:auto}.col-sm-push-12{left:100%}.col-sm-push-11{left:91.66666667%}.col-sm-push-10{left:83.33333333%}.col-sm-push-9{left:75%}.col-sm-push-8{left:66.66666667%}.col-sm-push-7{left:58.33333333%}.col-sm-push-6{left:50%}.col-sm-push-5{left:41.66666667%}.col-sm-push-4{left:33.33333333%}.col-sm-push-3{left:25%}.col-sm-push-2{left:16.66666667%}.col-sm-push-1{left:8.33333333%}.col-sm-push-0{left:auto}.col-sm-offset-12{margin-left:100%}.col-sm-offset-11{margin-left:91.66666667%}.col-sm-offset-10{margin-left:83.33333333%}.col-sm-offset-9{margin-left:75%}.col-sm-offset-8{margin-left:66.66666667%}.col-sm-offset-7{margin-left:58.33333333%}.col-sm-offset-6{margin-left:50%}.col-sm-offset-5{margin-left:41.66666667%}.col-sm-offset-4{margin-left:33.33333333%}.col-sm-offset-3{margin-left:25%}.col-sm-offset-2{margin-left:16.66666667%}.col-sm-offset-1{margin-left:8.33333333%}.col-sm-offset-0{margin-left:0}}@media (min-width:992px){.col-md-1,.col-md-10,.col-md-11,.col-md-12,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9{float:left}.col-md-12{width:100%}.col-md-11{width:91.66666667%}.col-md-10{width:83.33333333%}.col-md-9{width:75%}.col-md-8{width:66.66666667%}.col-md-7{width:58.33333333%}.col-md-6{width:50%}.col-md-5{width:41.66666667%}.col-md-4{width:33.33333333%}.col-md-3{width:25%}.col-md-2{width:16.66666667%}.col-md-1{width:8.33333333%}.col-md-pull-12{right:100%}.col-md-pull-11{right:91.66666667%}.col-md-pull-10{right:83.33333333%}.col-md-pull-9{right:75%}.col-md-pull-8{right:66.66666667%}.col-md-pull-7{right:58.33333333%}.col-md-pull-6{right:50%}.col-md-pull-5{right:41.66666667%}.col-md-pull-4{right:33.33333333%}.col-md-pull-3{right:25%}.col-md-pull-2{right:16.66666667%}.col-md-pull-1{right:8.33333333%}.col-md-pull-0{right:auto}.col-md-push-12{left:100%}.col-md-push-11{left:91.66666667%}.col-md-push-10{left:83.33333333%}.col-md-push-9{left:75%}.col-md-push-8{left:66.66666667%}.col-md-push-7{left:58.33333333%}.col-md-push-6{left:50%}.col-md-push-5{left:41.66666667%}.col-md-push-4{left:33.33333333%}.col-md-push-3{left:25%}.col-md-push-2{left:16.66666667%}.col-md-push-1{left:8.33333333%}.col-md-push-0{left:auto}.col-md-offset-12{margin-left:100%}.col-md-offset-11{margin-left:91.66666667%}.col-md-offset-10{margin-left:83.33333333%}.col-md-offset-9{margin-left:75%}.col-md-offset-8{margin-left:66.66666667%}.col-md-offset-7{margin-left:58.33333333%}.col-md-offset-6{margin-left:50%}.col-md-offset-5{margin-left:41.66666667%}.col-md-offset-4{margin-left:33.33333333%}.col-md-offset-3{margin-left:25%}.col-md-offset-2{margin-left:16.66666667%}.col-md-offset-1{margin-left:8.33333333%}.col-md-offset-0{margin-left:0}}@media (min-width:1200px){.col-lg-1,.col-lg-10,.col-lg-11,.col-lg-12,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9{float:left}.col-lg-12{width:100%}.col-lg-11{width:91.66666667%}.col-lg-10{width:83.33333333%}.col-lg-9{width:75%}.col-lg-8{width:66.66666667%}.col-lg-7{width:58.33333333%}.col-lg-6{width:50%}.col-lg-5{width:41.66666667%}.col-lg-4{width:33.33333333%}.col-lg-3{width:25%}.col-lg-2{width:16.66666667%}.col-lg-1{width:8.33333333%}.col-lg-pull-12{right:100%}.col-lg-pull-11{right:91.66666667%}.col-lg-pull-10{right:83.33333333%}.col-lg-pull-9{right:75%}.col-lg-pull-8{right:66.66666667%}.col-lg-pull-7{right:58.33333333%}.col-lg-pull-6{right:50%}.col-lg-pull-5{right:41.66666667%}.col-lg-pull-4{right:33.33333333%}.col-lg-pull-3{right:25%}.col-lg-pull-2{right:16.66666667%}.col-lg-pull-1{right:8.33333333%}.col-lg-pull-0{right:auto}.col-lg-push-12{left:100%}.col-lg-push-11{left:91.66666667%}.col-lg-push-10{left:83.33333333%}.col-lg-push-9{left:75%}.col-lg-push-8{left:66.66666667%}.col-lg-push-7{left:58.33333333%}.col-lg-push-6{left:50%}.col-lg-push-5{left:41.66666667%}.col-lg-push-4{left:33.33333333%}.col-lg-push-3{left:25%}.col-lg-push-2{left:16.66666667%}.col-lg-push-1{left:8.33333333%}.col-lg-push-0{left:auto}.col-lg-offset-12{margin-left:100%}.col-lg-offset-11{margin-left:91.66666667%}.col-lg-offset-10{margin-left:83.33333333%}.col-lg-offset-9{margin-left:75%}.col-lg-offset-8{margin-left:66.66666667%}.col-lg-offset-7{margin-left:58.33333333%}.col-lg-offset-6{margin-left:50%}.col-lg-offset-5{margin-left:41.66666667%}.col-lg-offset-4{margin-left:33.33333333%}.col-lg-offset-3{margin-left:25%}.col-lg-offset-2{margin-left:16.66666667%}.col-lg-offset-1{margin-left:8.33333333%}.col-lg-offset-0{margin-left:0}}table{background-color:transparent}table col[class*=col-]{position:static;display:table-column;float:none}table td[class*=col-],table th[class*=col-]{position:static;display:table-cell;float:none}caption{padding-top:8px;padding-bottom:8px;color:#777;text-align:left}th{text-align:left}.table{width:100%;max-width:100%;margin-bottom:20px}.table>tbody>tr>td,.table>tbody>tr>th,.table>tfoot>tr>td,.table>tfoot>tr>th,.table>thead>tr>td,.table>thead>tr>th{padding:8px;line-height:1.42857143;vertical-align:top;border-top:1px solid #ddd}.table>thead>tr>th{vertical-align:bottom;border-bottom:2px solid #ddd}.table>caption+thead>tr:first-child>td,.table>caption+thead>tr:first-child>th,.table>colgroup+thead>tr:first-child>td,.table>colgroup+thead>tr:first-child>th,.table>thead:first-child>tr:first-child>td,.table>thead:first-child>tr:first-child>th{border-top:0}.table>tbody+tbody{border-top:2px solid #ddd}.table .table{background-color:#fff}.table-condensed>tbody>tr>td,.table-condensed>tbody>tr>th,.table-condensed>tfoot>tr>td,.table-condensed>tfoot>tr>th,.table-condensed>thead>tr>td,.table-condensed>thead>tr>th{padding:5px}.table-bordered{border:1px solid #ddd}.table-bordered>tbody>tr>td,.table-bordered>tbody>tr>th,.table-bordered>tfoot>tr>td,.table-bordered>tfoot>tr>th,.table-bordered>thead>tr>td,.table-bordered>thead>tr>th{border:1px solid #ddd}.table-bordered>thead>tr>td,.table-bordered>thead>tr>th{border-bottom-width:2px}.table-striped>tbody>tr:nth-of-type(odd){background-color:#f9f9f9}.table-hover>tbody>tr:hover{background-color:#f5f5f5}.table>tbody>tr.active>td,.table>tbody>tr.active>th,.table>tbody>tr>td.active,.table>tbody>tr>th.active,.table>tfoot>tr.active>td,.table>tfoot>tr.active>th,.table>tfoot>tr>td.active,.table>tfoot>tr>th.active,.table>thead>tr.active>td,.table>thead>tr.active>th,.table>thead>tr>td.active,.table>thead>tr>th.active{background-color:#f5f5f5}.table-hover>tbody>tr.active:hover>td,.table-hover>tbody>tr.active:hover>th,.table-hover>tbody>tr:hover>.active,.table-hover>tbody>tr>td.active:hover,.table-hover>tbody>tr>th.active:hover{background-color:#e8e8e8}.table>tbody>tr.success>td,.table>tbody>tr.success>th,.table>tbody>tr>td.success,.table>tbody>tr>th.success,.table>tfoot>tr.success>td,.table>tfoot>tr.success>th,.table>tfoot>tr>td.success,.table>tfoot>tr>th.success,.table>thead>tr.success>td,.table>thead>tr.success>th,.table>thead>tr>td.success,.table>thead>tr>th.success{background-color:#dff0d8}.table-hover>tbody>tr.success:hover>td,.table-hover>tbody>tr.success:hover>th,.table-hover>tbody>tr:hover>.success,.table-hover>tbody>tr>td.success:hover,.table-hover>tbody>tr>th.success:hover{background-color:#d0e9c6}.table>tbody>tr.info>td,.table>tbody>tr.info>th,.table>tbody>tr>td.info,.table>tbody>tr>th.info,.table>tfoot>tr.info>td,.table>tfoot>tr.info>th,.table>tfoot>tr>td.info,.table>tfoot>tr>th.info,.table>thead>tr.info>td,.table>thead>tr.info>th,.table>thead>tr>td.info,.table>thead>tr>th.info{background-color:#d9edf7}.table-hover>tbody>tr.info:hover>td,.table-hover>tbody>tr.info:hover>th,.table-hover>tbody>tr:hover>.info,.table-hover>tbody>tr>td.info:hover,.table-hover>tbody>tr>th.info:hover{background-color:#c4e3f3}.table>tbody>tr.warning>td,.table>tbody>tr.warning>th,.table>tbody>tr>td.warning,.table>tbody>tr>th.warning,.table>tfoot>tr.warning>td,.table>tfoot>tr.warning>th,.table>tfoot>tr>td.warning,.table>tfoot>tr>th.warning,.table>thead>tr.warning>td,.table>thead>tr.warning>th,.table>thead>tr>td.warning,.table>thead>tr>th.warning{background-color:#fcf8e3}.table-hover>tbody>tr.warning:hover>td,.table-hover>tbody>tr.warning:hover>th,.table-hover>tbody>tr:hover>.warning,.table-hover>tbody>tr>td.warning:hover,.table-hover>tbody>tr>th.warning:hover{background-color:#faf2cc}.table>tbody>tr.danger>td,.table>tbody>tr.danger>th,.table>tbody>tr>td.danger,.table>tbody>tr>th.danger,.table>tfoot>tr.danger>td,.table>tfoot>tr.danger>th,.table>tfoot>tr>td.danger,.table>tfoot>tr>th.danger,.table>thead>tr.danger>td,.table>thead>tr.danger>th,.table>thead>tr>td.danger,.table>thead>tr>th.danger{background-color:#f2dede}.table-hover>tbody>tr.danger:hover>td,.table-hover>tbody>tr.danger:hover>th,.table-hover>tbody>tr:hover>.danger,.table-hover>tbody>tr>td.danger:hover,.table-hover>tbody>tr>th.danger:hover{background-color:#ebcccc}.table-responsive{min-height:.01%;overflow-x:auto}@media screen and (max-width:767px){.table-responsive{width:100%;margin-bottom:15px;overflow-y:hidden;-ms-overflow-style:-ms-autohiding-scrollbar;border:1px solid #ddd}.table-responsive>.table{margin-bottom:0}.table-responsive>.table>tbody>tr>td,.table-responsive>.table>tbody>tr>th,.table-responsive>.table>tfoot>tr>td,.table-responsive>.table>tfoot>tr>th,.table-responsive>.table>thead>tr>td,.table-responsive>.table>thead>tr>th{white-space:nowrap}.table-responsive>.table-bordered{border:0}.table-responsive>.table-bordered>tbody>tr>td:first-child,.table-responsive>.table-bordered>tbody>tr>th:first-child,.table-responsive>.table-bordered>tfoot>tr>td:first-child,.table-responsive>.table-bordered>tfoot>tr>th:first-child,.table-responsive>.table-bordered>thead>tr>td:first-child,.table-responsive>.table-bordered>thead>tr>th:first-child{border-left:0}.table-responsive>.table-bordered>tbody>tr>td:last-child,.table-responsive>.table-bordered>tbody>tr>th:last-child,.table-responsive>.table-bordered>tfoot>tr>td:last-child,.table-responsive>.table-bordered>tfoot>tr>th:last-child,.table-responsive>.table-bordered>thead>tr>td:last-child,.table-responsive>.table-bordered>thead>tr>th:last-child{border-right:0}.table-responsive>.table-bordered>tbody>tr:last-child>td,.table-responsive>.table-bordered>tbody>tr:last-child>th,.table-responsive>.table-bordered>tfoot>tr:last-child>td,.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}}fieldset{min-width:0;padding:0;margin:0;border:0}legend{display:block;width:100%;padding:0;margin-bottom:20px;font-size:21px;line-height:inherit;color:#333;border:0;border-bottom:1px solid #e5e5e5}label{display:inline-block;max-width:100%;margin-bottom:5px;font-weight:700}input[type=search]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;-webkit-appearance:none;-moz-appearance:none;appearance:none}input[type=checkbox],input[type=radio]{margin:4px 0 0;margin-top:1px\9;line-height:normal}fieldset[disabled] input[type=checkbox],fieldset[disabled] input[type=radio],input[type=checkbox].disabled,input[type=checkbox][disabled],input[type=radio].disabled,input[type=radio][disabled]{cursor:not-allowed}input[type=file]{display:block}input[type=range]{display:block;width:100%}select[multiple],select[size]{height:auto}input[type=checkbox]:focus,input[type=file]:focus,input[type=radio]:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}output{display:block;padding-top:7px;font-size:14px;line-height:1.42857143;color:#555}.form-control{display:block;width:100%;height:34px;padding:6px 12px;font-size:14px;line-height:1.42857143;color:#555;background-color:#fff;background-image:none;border:1px solid #ccc;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075);-webkit-transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;-o-transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;-webkit-transition:border-color ease-in-out .15s,-webkit-box-shadow ease-in-out .15s;transition:border-color ease-in-out .15s,-webkit-box-shadow ease-in-out .15s;transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s,-webkit-box-shadow ease-in-out .15s}.form-control:focus{border-color:#66afe9;outline:0;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6);box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6)}.form-control::-moz-placeholder{color:#999;opacity:1}.form-control:-ms-input-placeholder{color:#999}.form-control::-webkit-input-placeholder{color:#999}.form-control::-ms-expand{background-color:transparent;border:0}.form-control[disabled],.form-control[readonly],fieldset[disabled] .form-control{background-color:#eee;opacity:1}.form-control[disabled],fieldset[disabled] .form-control{cursor:not-allowed}textarea.form-control{height:auto}@media screen and (-webkit-min-device-pixel-ratio:0){input[type=date].form-control,input[type=datetime-local].form-control,input[type=month].form-control,input[type=time].form-control{line-height:34px}.input-group-sm input[type=date],.input-group-sm input[type=datetime-local],.input-group-sm input[type=month],.input-group-sm input[type=time],input[type=date].input-sm,input[type=datetime-local].input-sm,input[type=month].input-sm,input[type=time].input-sm{line-height:30px}.input-group-lg input[type=date],.input-group-lg input[type=datetime-local],.input-group-lg input[type=month],.input-group-lg input[type=time],input[type=date].input-lg,input[type=datetime-local].input-lg,input[type=month].input-lg,input[type=time].input-lg{line-height:46px}}.form-group{margin-bottom:15px}.checkbox,.radio{position:relative;display:block;margin-top:10px;margin-bottom:10px}.checkbox.disabled label,.radio.disabled label,fieldset[disabled] .checkbox label,fieldset[disabled] .radio label{cursor:not-allowed}.checkbox label,.radio label{min-height:20px;padding-left:20px;margin-bottom:0;font-weight:400;cursor:pointer}.checkbox input[type=checkbox],.checkbox-inline input[type=checkbox],.radio input[type=radio],.radio-inline input[type=radio]{position:absolute;margin-top:4px\9;margin-left:-20px}.checkbox+.checkbox,.radio+.radio{margin-top:-5px}.checkbox-inline,.radio-inline{position:relative;display:inline-block;padding-left:20px;margin-bottom:0;font-weight:400;vertical-align:middle;cursor:pointer}.checkbox-inline.disabled,.radio-inline.disabled,fieldset[disabled] .checkbox-inline,fieldset[disabled] .radio-inline{cursor:not-allowed}.checkbox-inline+.checkbox-inline,.radio-inline+.radio-inline{margin-top:0;margin-left:10px}.form-control-static{min-height:34px;padding-top:7px;padding-bottom:7px;margin-bottom:0}.form-control-static.input-lg,.form-control-static.input-sm{padding-right:0;padding-left:0}.input-sm{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-sm{height:30px;line-height:30px}select[multiple].input-sm,textarea.input-sm{height:auto}.form-group-sm .form-control{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.form-group-sm select.form-control{height:30px;line-height:30px}.form-group-sm select[multiple].form-control,.form-group-sm textarea.form-control{height:auto}.form-group-sm .form-control-static{height:30px;min-height:32px;padding:6px 10px;font-size:12px;line-height:1.5}.input-lg{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}select.input-lg{height:46px;line-height:46px}select[multiple].input-lg,textarea.input-lg{height:auto}.form-group-lg .form-control{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}.form-group-lg select.form-control{height:46px;line-height:46px}.form-group-lg select[multiple].form-control,.form-group-lg textarea.form-control{height:auto}.form-group-lg .form-control-static{height:46px;min-height:38px;padding:11px 16px;font-size:18px;line-height:1.3333333}.has-feedback{position:relative}.has-feedback .form-control{padding-right:42.5px}.form-control-feedback{position:absolute;top:0;right:0;z-index:2;display:block;width:34px;height:34px;line-height:34px;text-align:center;pointer-events:none}.form-group-lg .form-control+.form-control-feedback,.input-group-lg+.form-control-feedback,.input-lg+.form-control-feedback{width:46px;height:46px;line-height:46px}.form-group-sm .form-control+.form-control-feedback,.input-group-sm+.form-control-feedback,.input-sm+.form-control-feedback{width:30px;height:30px;line-height:30px}.has-success .checkbox,.has-success .checkbox-inline,.has-success .control-label,.has-success .help-block,.has-success .radio,.has-success .radio-inline,.has-success.checkbox label,.has-success.checkbox-inline label,.has-success.radio label,.has-success.radio-inline label{color:#3c763d}.has-success .form-control{border-color:#3c763d;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-success .form-control:focus{border-color:#2b542c;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #67b168;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #67b168}.has-success .input-group-addon{color:#3c763d;background-color:#dff0d8;border-color:#3c763d}.has-success .form-control-feedback{color:#3c763d}.has-warning .checkbox,.has-warning .checkbox-inline,.has-warning .control-label,.has-warning .help-block,.has-warning .radio,.has-warning .radio-inline,.has-warning.checkbox label,.has-warning.checkbox-inline label,.has-warning.radio label,.has-warning.radio-inline label{color:#8a6d3b}.has-warning .form-control{border-color:#8a6d3b;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-warning .form-control:focus{border-color:#66512c;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #c0a16b;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #c0a16b}.has-warning .input-group-addon{color:#8a6d3b;background-color:#fcf8e3;border-color:#8a6d3b}.has-warning .form-control-feedback{color:#8a6d3b}.has-error .checkbox,.has-error .checkbox-inline,.has-error .control-label,.has-error .help-block,.has-error .radio,.has-error .radio-inline,.has-error.checkbox label,.has-error.checkbox-inline label,.has-error.radio label,.has-error.radio-inline label{color:#a94442}.has-error .form-control{border-color:#a94442;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-error .form-control:focus{border-color:#843534;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #ce8483;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #ce8483}.has-error .input-group-addon{color:#a94442;background-color:#f2dede;border-color:#a94442}.has-error .form-control-feedback{color:#a94442}.has-feedback label~.form-control-feedback{top:25px}.has-feedback label.sr-only~.form-control-feedback{top:0}.help-block{display:block;margin-top:5px;margin-bottom:10px;color:#737373}@media (min-width:768px){.form-inline .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.form-inline .form-control{display:inline-block;width:auto;vertical-align:middle}.form-inline .form-control-static{display:inline-block}.form-inline .input-group{display:inline-table;vertical-align:middle}.form-inline .input-group .form-control,.form-inline .input-group .input-group-addon,.form-inline .input-group .input-group-btn{width:auto}.form-inline .input-group>.form-control{width:100%}.form-inline .control-label{margin-bottom:0;vertical-align:middle}.form-inline .checkbox,.form-inline .radio{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.form-inline .checkbox label,.form-inline .radio label{padding-left:0}.form-inline .checkbox input[type=checkbox],.form-inline .radio input[type=radio]{position:relative;margin-left:0}.form-inline .has-feedback .form-control-feedback{top:0}}.form-horizontal .checkbox,.form-horizontal .checkbox-inline,.form-horizontal .radio,.form-horizontal .radio-inline{padding-top:7px;margin-top:0;margin-bottom:0}.form-horizontal .checkbox,.form-horizontal .radio{min-height:27px}.form-horizontal .form-group{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.form-horizontal .control-label{padding-top:7px;margin-bottom:0;text-align:right}}.form-horizontal .has-feedback .form-control-feedback{right:15px}@media (min-width:768px){.form-horizontal .form-group-lg .control-label{padding-top:11px;font-size:18px}}@media (min-width:768px){.form-horizontal .form-group-sm .control-label{padding-top:6px;font-size:12px}}.btn{display:inline-block;margin-bottom:0;font-weight:400;text-align:center;white-space:nowrap;vertical-align:middle;-ms-touch-action:manipulation;touch-action:manipulation;cursor:pointer;background-image:none;border:1px solid transparent;padding:6px 12px;font-size:14px;line-height:1.42857143;border-radius:4px;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.btn.active.focus,.btn.active:focus,.btn.focus,.btn:active.focus,.btn:active:focus,.btn:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}.btn.focus,.btn:focus,.btn:hover{color:#333;text-decoration:none}.btn.active,.btn:active{background-image:none;outline:0;-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn.disabled,.btn[disabled],fieldset[disabled] .btn{cursor:not-allowed;filter:alpha(opacity=65);opacity:.65;-webkit-box-shadow:none;box-shadow:none}a.btn.disabled,fieldset[disabled] a.btn{pointer-events:none}.btn-default{color:#333;background-color:#fff;border-color:#ccc}.btn-default.focus,.btn-default:focus{color:#333;background-color:#e6e6e6;border-color:#8c8c8c}.btn-default:hover{color:#333;background-color:#e6e6e6;border-color:#adadad}.btn-default.active,.btn-default:active,.open>.dropdown-toggle.btn-default{color:#333;background-color:#e6e6e6;background-image:none;border-color:#adadad}.btn-default.active.focus,.btn-default.active:focus,.btn-default.active:hover,.btn-default:active.focus,.btn-default:active:focus,.btn-default:active:hover,.open>.dropdown-toggle.btn-default.focus,.open>.dropdown-toggle.btn-default:focus,.open>.dropdown-toggle.btn-default:hover{color:#333;background-color:#d4d4d4;border-color:#8c8c8c}.btn-default.disabled.focus,.btn-default.disabled:focus,.btn-default.disabled:hover,.btn-default[disabled].focus,.btn-default[disabled]:focus,.btn-default[disabled]:hover,fieldset[disabled] .btn-default.focus,fieldset[disabled] .btn-default:focus,fieldset[disabled] .btn-default:hover{background-color:#fff;border-color:#ccc}.btn-default .badge{color:#fff;background-color:#333}.btn-primary{color:#fff;background-color:#337ab7;border-color:#2e6da4}.btn-primary.focus,.btn-primary:focus{color:#fff;background-color:#286090;border-color:#122b40}.btn-primary:hover{color:#fff;background-color:#286090;border-color:#204d74}.btn-primary.active,.btn-primary:active,.open>.dropdown-toggle.btn-primary{color:#fff;background-color:#286090;background-image:none;border-color:#204d74}.btn-primary.active.focus,.btn-primary.active:focus,.btn-primary.active:hover,.btn-primary:active.focus,.btn-primary:active:focus,.btn-primary:active:hover,.open>.dropdown-toggle.btn-primary.focus,.open>.dropdown-toggle.btn-primary:focus,.open>.dropdown-toggle.btn-primary:hover{color:#fff;background-color:#204d74;border-color:#122b40}.btn-primary.disabled.focus,.btn-primary.disabled:focus,.btn-primary.disabled:hover,.btn-primary[disabled].focus,.btn-primary[disabled]:focus,.btn-primary[disabled]:hover,fieldset[disabled] .btn-primary.focus,fieldset[disabled] .btn-primary:focus,fieldset[disabled] .btn-primary:hover{background-color:#337ab7;border-color:#2e6da4}.btn-primary .badge{color:#337ab7;background-color:#fff}.btn-success{color:#fff;background-color:#5cb85c;border-color:#4cae4c}.btn-success.focus,.btn-success:focus{color:#fff;background-color:#449d44;border-color:#255625}.btn-success:hover{color:#fff;background-color:#449d44;border-color:#398439}.btn-success.active,.btn-success:active,.open>.dropdown-toggle.btn-success{color:#fff;background-color:#449d44;background-image:none;border-color:#398439}.btn-success.active.focus,.btn-success.active:focus,.btn-success.active:hover,.btn-success:active.focus,.btn-success:active:focus,.btn-success:active:hover,.open>.dropdown-toggle.btn-success.focus,.open>.dropdown-toggle.btn-success:focus,.open>.dropdown-toggle.btn-success:hover{color:#fff;background-color:#398439;border-color:#255625}.btn-success.disabled.focus,.btn-success.disabled:focus,.btn-success.disabled:hover,.btn-success[disabled].focus,.btn-success[disabled]:focus,.btn-success[disabled]:hover,fieldset[disabled] .btn-success.focus,fieldset[disabled] .btn-success:focus,fieldset[disabled] .btn-success:hover{background-color:#5cb85c;border-color:#4cae4c}.btn-success .badge{color:#5cb85c;background-color:#fff}.btn-info{color:#fff;background-color:#5bc0de;border-color:#46b8da}.btn-info.focus,.btn-info:focus{color:#fff;background-color:#31b0d5;border-color:#1b6d85}.btn-info:hover{color:#fff;background-color:#31b0d5;border-color:#269abc}.btn-info.active,.btn-info:active,.open>.dropdown-toggle.btn-info{color:#fff;background-color:#31b0d5;background-image:none;border-color:#269abc}.btn-info.active.focus,.btn-info.active:focus,.btn-info.active:hover,.btn-info:active.focus,.btn-info:active:focus,.btn-info:active:hover,.open>.dropdown-toggle.btn-info.focus,.open>.dropdown-toggle.btn-info:focus,.open>.dropdown-toggle.btn-info:hover{color:#fff;background-color:#269abc;border-color:#1b6d85}.btn-info.disabled.focus,.btn-info.disabled:focus,.btn-info.disabled:hover,.btn-info[disabled].focus,.btn-info[disabled]:focus,.btn-info[disabled]:hover,fieldset[disabled] .btn-info.focus,fieldset[disabled] .btn-info:focus,fieldset[disabled] .btn-info:hover{background-color:#5bc0de;border-color:#46b8da}.btn-info .badge{color:#5bc0de;background-color:#fff}.btn-warning{color:#fff;background-color:#f0ad4e;border-color:#eea236}.btn-warning.focus,.btn-warning:focus{color:#fff;background-color:#ec971f;border-color:#985f0d}.btn-warning:hover{color:#fff;background-color:#ec971f;border-color:#d58512}.btn-warning.active,.btn-warning:active,.open>.dropdown-toggle.btn-warning{color:#fff;background-color:#ec971f;background-image:none;border-color:#d58512}.btn-warning.active.focus,.btn-warning.active:focus,.btn-warning.active:hover,.btn-warning:active.focus,.btn-warning:active:focus,.btn-warning:active:hover,.open>.dropdown-toggle.btn-warning.focus,.open>.dropdown-toggle.btn-warning:focus,.open>.dropdown-toggle.btn-warning:hover{color:#fff;background-color:#d58512;border-color:#985f0d}.btn-warning.disabled.focus,.btn-warning.disabled:focus,.btn-warning.disabled:hover,.btn-warning[disabled].focus,.btn-warning[disabled]:focus,.btn-warning[disabled]:hover,fieldset[disabled] .btn-warning.focus,fieldset[disabled] .btn-warning:focus,fieldset[disabled] .btn-warning:hover{background-color:#f0ad4e;border-color:#eea236}.btn-warning .badge{color:#f0ad4e;background-color:#fff}.btn-danger{color:#fff;background-color:#d9534f;border-color:#d43f3a}.btn-danger.focus,.btn-danger:focus{color:#fff;background-color:#c9302c;border-color:#761c19}.btn-danger:hover{color:#fff;background-color:#c9302c;border-color:#ac2925}.btn-danger.active,.btn-danger:active,.open>.dropdown-toggle.btn-danger{color:#fff;background-color:#c9302c;background-image:none;border-color:#ac2925}.btn-danger.active.focus,.btn-danger.active:focus,.btn-danger.active:hover,.btn-danger:active.focus,.btn-danger:active:focus,.btn-danger:active:hover,.open>.dropdown-toggle.btn-danger.focus,.open>.dropdown-toggle.btn-danger:focus,.open>.dropdown-toggle.btn-danger:hover{color:#fff;background-color:#ac2925;border-color:#761c19}.btn-danger.disabled.focus,.btn-danger.disabled:focus,.btn-danger.disabled:hover,.btn-danger[disabled].focus,.btn-danger[disabled]:focus,.btn-danger[disabled]:hover,fieldset[disabled] .btn-danger.focus,fieldset[disabled] .btn-danger:focus,fieldset[disabled] .btn-danger:hover{background-color:#d9534f;border-color:#d43f3a}.btn-danger .badge{color:#d9534f;background-color:#fff}.btn-link{font-weight:400;color:#337ab7;border-radius:0}.btn-link,.btn-link.active,.btn-link:active,.btn-link[disabled],fieldset[disabled] .btn-link{background-color:transparent;-webkit-box-shadow:none;box-shadow:none}.btn-link,.btn-link:active,.btn-link:focus,.btn-link:hover{border-color:transparent}.btn-link:focus,.btn-link:hover{color:#23527c;text-decoration:underline;background-color:transparent}.btn-link[disabled]:focus,.btn-link[disabled]:hover,fieldset[disabled] .btn-link:focus,fieldset[disabled] .btn-link:hover{color:#777;text-decoration:none}.btn-group-lg>.btn,.btn-lg{padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}.btn-group-sm>.btn,.btn-sm{padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.btn-group-xs>.btn,.btn-xs{padding:1px 5px;font-size:12px;line-height:1.5;border-radius:3px}.btn-block{display:block;width:100%}.btn-block+.btn-block{margin-top:5px}input[type=button].btn-block,input[type=reset].btn-block,input[type=submit].btn-block{width:100%}.fade{opacity:0;-webkit-transition:opacity .15s linear;-o-transition:opacity .15s linear;transition:opacity .15s linear}.fade.in{opacity:1}.collapse{display:none}.collapse.in{display:block}tr.collapse.in{display:table-row}tbody.collapse.in{display:table-row-group}.collapsing{position:relative;height:0;overflow:hidden;-webkit-transition-property:height,visibility;-o-transition-property:height,visibility;transition-property:height,visibility;-webkit-transition-duration:.35s;-o-transition-duration:.35s;transition-duration:.35s;-webkit-transition-timing-function:ease;-o-transition-timing-function:ease;transition-timing-function:ease}.caret{display:inline-block;width:0;height:0;margin-left:2px;vertical-align:middle;border-top:4px dashed;border-top:4px solid\9;border-right:4px solid transparent;border-left:4px solid transparent}.dropdown,.dropup{position:relative}.dropdown-toggle:focus{outline:0}.dropdown-menu{position:absolute;top:100%;left:0;z-index:1000;display:none;float:left;min-width:160px;padding:5px 0;margin:2px 0 0;font-size:14px;text-align:left;list-style:none;background-color:#fff;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.15);border-radius:4px;-webkit-box-shadow:0 6px 12px rgba(0,0,0,.175);box-shadow:0 6px 12px rgba(0,0,0,.175)}.dropdown-menu.pull-right{right:0;left:auto}.dropdown-menu .divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.dropdown-menu>li>a{display:block;padding:3px 20px;clear:both;font-weight:400;line-height:1.42857143;color:#333;white-space:nowrap}.dropdown-menu>li>a:focus,.dropdown-menu>li>a:hover{color:#262626;text-decoration:none;background-color:#f5f5f5}.dropdown-menu>.active>a,.dropdown-menu>.active>a:focus,.dropdown-menu>.active>a:hover{color:#fff;text-decoration:none;background-color:#337ab7;outline:0}.dropdown-menu>.disabled>a,.dropdown-menu>.disabled>a:focus,.dropdown-menu>.disabled>a:hover{color:#777}.dropdown-menu>.disabled>a:focus,.dropdown-menu>.disabled>a:hover{text-decoration:none;cursor:not-allowed;background-color:transparent;background-image:none;filter:progid:DXImageTransform.Microsoft.gradient(enabled=false)}.open>.dropdown-menu{display:block}.open>a{outline:0}.dropdown-menu-right{right:0;left:auto}.dropdown-menu-left{right:auto;left:0}.dropdown-header{display:block;padding:3px 20px;font-size:12px;line-height:1.42857143;color:#777;white-space:nowrap}.dropdown-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:990}.pull-right>.dropdown-menu{right:0;left:auto}.dropup .caret,.navbar-fixed-bottom .dropdown .caret{content:"";border-top:0;border-bottom:4px dashed;border-bottom:4px solid\9}.dropup .dropdown-menu,.navbar-fixed-bottom .dropdown .dropdown-menu{top:auto;bottom:100%;margin-bottom:2px}@media (min-width:768px){.navbar-right .dropdown-menu{right:0;left:auto}.navbar-right .dropdown-menu-left{right:auto;left:0}}.btn-group,.btn-group-vertical{position:relative;display:inline-block;vertical-align:middle}.btn-group-vertical>.btn,.btn-group>.btn{position:relative;float:left}.btn-group-vertical>.btn.active,.btn-group-vertical>.btn:active,.btn-group-vertical>.btn:focus,.btn-group-vertical>.btn:hover,.btn-group>.btn.active,.btn-group>.btn:active,.btn-group>.btn:focus,.btn-group>.btn:hover{z-index:2}.btn-group .btn+.btn,.btn-group .btn+.btn-group,.btn-group .btn-group+.btn,.btn-group .btn-group+.btn-group{margin-left:-1px}.btn-toolbar{margin-left:-5px}.btn-toolbar .btn,.btn-toolbar .btn-group,.btn-toolbar .input-group{float:left}.btn-toolbar>.btn,.btn-toolbar>.btn-group,.btn-toolbar>.input-group{margin-left:5px}.btn-group>.btn:not(:first-child):not(:last-child):not(.dropdown-toggle){border-radius:0}.btn-group>.btn:first-child{margin-left:0}.btn-group>.btn:first-child:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn:last-child:not(:first-child),.btn-group>.dropdown-toggle:not(:first-child){border-top-left-radius:0;border-bottom-left-radius:0}.btn-group>.btn-group{float:left}.btn-group>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-bottom-left-radius:0}.btn-group .dropdown-toggle:active,.btn-group.open .dropdown-toggle{outline:0}.btn-group>.btn+.dropdown-toggle{padding-right:8px;padding-left:8px}.btn-group>.btn-lg+.dropdown-toggle{padding-right:12px;padding-left:12px}.btn-group.open .dropdown-toggle{-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn-group.open .dropdown-toggle.btn-link{-webkit-box-shadow:none;box-shadow:none}.btn .caret{margin-left:0}.btn-lg .caret{border-width:5px 5px 0;border-bottom-width:0}.dropup .btn-lg .caret{border-width:0 5px 5px}.btn-group-vertical>.btn,.btn-group-vertical>.btn-group,.btn-group-vertical>.btn-group>.btn{display:block;float:none;width:100%;max-width:100%}.btn-group-vertical>.btn-group>.btn{float:none}.btn-group-vertical>.btn+.btn,.btn-group-vertical>.btn+.btn-group,.btn-group-vertical>.btn-group+.btn,.btn-group-vertical>.btn-group+.btn-group{margin-top:-1px;margin-left:0}.btn-group-vertical>.btn:not(:first-child):not(:last-child){border-radius:0}.btn-group-vertical>.btn:first-child:not(:last-child){border-top-left-radius:4px;border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn:last-child:not(:first-child){border-top-left-radius:0;border-top-right-radius:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}.btn-group-vertical>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group-vertical>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group-vertical>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-top-right-radius:0}.btn-group-justified{display:table;width:100%;table-layout:fixed;border-collapse:separate}.btn-group-justified>.btn,.btn-group-justified>.btn-group{display:table-cell;float:none;width:1%}.btn-group-justified>.btn-group .btn{width:100%}.btn-group-justified>.btn-group .dropdown-menu{left:auto}[data-toggle=buttons]>.btn input[type=checkbox],[data-toggle=buttons]>.btn input[type=radio],[data-toggle=buttons]>.btn-group>.btn input[type=checkbox],[data-toggle=buttons]>.btn-group>.btn input[type=radio]{position:absolute;clip:rect(0,0,0,0);pointer-events:none}.input-group{position:relative;display:table;border-collapse:separate}.input-group[class*=col-]{float:none;padding-right:0;padding-left:0}.input-group .form-control{position:relative;z-index:2;float:left;width:100%;margin-bottom:0}.input-group .form-control:focus{z-index:3}.input-group-lg>.form-control,.input-group-lg>.input-group-addon,.input-group-lg>.input-group-btn>.btn{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}select.input-group-lg>.form-control,select.input-group-lg>.input-group-addon,select.input-group-lg>.input-group-btn>.btn{height:46px;line-height:46px}select[multiple].input-group-lg>.form-control,select[multiple].input-group-lg>.input-group-addon,select[multiple].input-group-lg>.input-group-btn>.btn,textarea.input-group-lg>.form-control,textarea.input-group-lg>.input-group-addon,textarea.input-group-lg>.input-group-btn>.btn{height:auto}.input-group-sm>.form-control,.input-group-sm>.input-group-addon,.input-group-sm>.input-group-btn>.btn{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-group-sm>.form-control,select.input-group-sm>.input-group-addon,select.input-group-sm>.input-group-btn>.btn{height:30px;line-height:30px}select[multiple].input-group-sm>.form-control,select[multiple].input-group-sm>.input-group-addon,select[multiple].input-group-sm>.input-group-btn>.btn,textarea.input-group-sm>.form-control,textarea.input-group-sm>.input-group-addon,textarea.input-group-sm>.input-group-btn>.btn{height:auto}.input-group .form-control,.input-group-addon,.input-group-btn{display:table-cell}.input-group .form-control:not(:first-child):not(:last-child),.input-group-addon:not(:first-child):not(:last-child),.input-group-btn:not(:first-child):not(:last-child){border-radius:0}.input-group-addon,.input-group-btn{width:1%;white-space:nowrap;vertical-align:middle}.input-group-addon{padding:6px 12px;font-size:14px;font-weight:400;line-height:1;color:#555;text-align:center;background-color:#eee;border:1px solid #ccc;border-radius:4px}.input-group-addon.input-sm{padding:5px 10px;font-size:12px;border-radius:3px}.input-group-addon.input-lg{padding:10px 16px;font-size:18px;border-radius:6px}.input-group-addon input[type=checkbox],.input-group-addon input[type=radio]{margin-top:0}.input-group .form-control:first-child,.input-group-addon:first-child,.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group>.btn,.input-group-btn:first-child>.dropdown-toggle,.input-group-btn:last-child>.btn-group:not(:last-child)>.btn,.input-group-btn:last-child>.btn:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.input-group-addon:first-child{border-right:0}.input-group .form-control:last-child,.input-group-addon:last-child,.input-group-btn:first-child>.btn-group:not(:first-child)>.btn,.input-group-btn:first-child>.btn:not(:first-child),.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group>.btn,.input-group-btn:last-child>.dropdown-toggle{border-top-left-radius:0;border-bottom-left-radius:0}.input-group-addon:last-child{border-left:0}.input-group-btn{position:relative;font-size:0;white-space:nowrap}.input-group-btn>.btn{position:relative}.input-group-btn>.btn+.btn{margin-left:-1px}.input-group-btn>.btn:active,.input-group-btn>.btn:focus,.input-group-btn>.btn:hover{z-index:2}.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group{margin-right:-1px}.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group{z-index:2;margin-left:-1px}.nav{padding-left:0;margin-bottom:0;list-style:none}.nav>li{position:relative;display:block}.nav>li>a{position:relative;display:block;padding:10px 15px}.nav>li>a:focus,.nav>li>a:hover{text-decoration:none;background-color:#eee}.nav>li.disabled>a{color:#777}.nav>li.disabled>a:focus,.nav>li.disabled>a:hover{color:#777;text-decoration:none;cursor:not-allowed;background-color:transparent}.nav .open>a,.nav .open>a:focus,.nav .open>a:hover{background-color:#eee;border-color:#337ab7}.nav .nav-divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.nav>li>a>img{max-width:none}.nav-tabs{border-bottom:1px solid #ddd}.nav-tabs>li{float:left;margin-bottom:-1px}.nav-tabs>li>a{margin-right:2px;line-height:1.42857143;border:1px solid transparent;border-radius:4px 4px 0 0}.nav-tabs>li>a:hover{border-color:#eee #eee #ddd}.nav-tabs>li.active>a,.nav-tabs>li.active>a:focus,.nav-tabs>li.active>a:hover{color:#555;cursor:default;background-color:#fff;border:1px solid #ddd;border-bottom-color:transparent}.nav-tabs.nav-justified{width:100%;border-bottom:0}.nav-tabs.nav-justified>li{float:none}.nav-tabs.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-tabs.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-tabs.nav-justified>li{display:table-cell;width:1%}.nav-tabs.nav-justified>li>a{margin-bottom:0}}.nav-tabs.nav-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:focus,.nav-tabs.nav-justified>.active>a:hover{border:1px solid #ddd}@media (min-width:768px){.nav-tabs.nav-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:focus,.nav-tabs.nav-justified>.active>a:hover{border-bottom-color:#fff}}.nav-pills>li{float:left}.nav-pills>li>a{border-radius:4px}.nav-pills>li+li{margin-left:2px}.nav-pills>li.active>a,.nav-pills>li.active>a:focus,.nav-pills>li.active>a:hover{color:#fff;background-color:#337ab7}.nav-stacked>li{float:none}.nav-stacked>li+li{margin-top:2px;margin-left:0}.nav-justified{width:100%}.nav-justified>li{float:none}.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-justified>li{display:table-cell;width:1%}.nav-justified>li>a{margin-bottom:0}}.nav-tabs-justified{border-bottom:0}.nav-tabs-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:focus,.nav-tabs-justified>.active>a:hover{border:1px solid #ddd}@media (min-width:768px){.nav-tabs-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:focus,.nav-tabs-justified>.active>a:hover{border-bottom-color:#fff}}.tab-content>.tab-pane{display:none}.tab-content>.active{display:block}.nav-tabs .dropdown-menu{margin-top:-1px;border-top-left-radius:0;border-top-right-radius:0}.navbar{position:relative;min-height:50px;margin-bottom:20px;border:1px solid transparent}@media (min-width:768px){.navbar{border-radius:4px}}@media (min-width:768px){.navbar-header{float:left}}.navbar-collapse{padding-right:15px;padding-left:15px;overflow-x:visible;border-top:1px solid transparent;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 0 rgba(255,255,255,.1);-webkit-overflow-scrolling:touch}.navbar-collapse.in{overflow-y:auto}@media (min-width:768px){.navbar-collapse{width:auto;border-top:0;-webkit-box-shadow:none;box-shadow:none}.navbar-collapse.collapse{display:block!important;height:auto!important;padding-bottom:0;overflow:visible!important}.navbar-collapse.in{overflow-y:visible}.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse,.navbar-static-top .navbar-collapse{padding-right:0;padding-left:0}}.navbar-fixed-bottom,.navbar-fixed-top{position:fixed;right:0;left:0;z-index:1030}.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse{max-height:340px}@media (max-device-width:480px) and (orientation:landscape){.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse{max-height:200px}}@media (min-width:768px){.navbar-fixed-bottom,.navbar-fixed-top{border-radius:0}}.navbar-fixed-top{top:0;border-width:0 0 1px}.navbar-fixed-bottom{bottom:0;margin-bottom:0;border-width:1px 0 0}.container-fluid>.navbar-collapse,.container-fluid>.navbar-header,.container>.navbar-collapse,.container>.navbar-header{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.container-fluid>.navbar-collapse,.container-fluid>.navbar-header,.container>.navbar-collapse,.container>.navbar-header{margin-right:0;margin-left:0}}.navbar-static-top{z-index:1000;border-width:0 0 1px}@media (min-width:768px){.navbar-static-top{border-radius:0}}.navbar-brand{float:left;height:50px;padding:15px 15px;font-size:18px;line-height:20px}.navbar-brand:focus,.navbar-brand:hover{text-decoration:none}.navbar-brand>img{display:block}@media (min-width:768px){.navbar>.container .navbar-brand,.navbar>.container-fluid .navbar-brand{margin-left:-15px}}.navbar-toggle{position:relative;float:right;padding:9px 10px;margin-right:15px;margin-top:8px;margin-bottom:8px;background-color:transparent;background-image:none;border:1px solid transparent;border-radius:4px}.navbar-toggle:focus{outline:0}.navbar-toggle .icon-bar{display:block;width:22px;height:2px;border-radius:1px}.navbar-toggle .icon-bar+.icon-bar{margin-top:4px}@media (min-width:768px){.navbar-toggle{display:none}}.navbar-nav{margin:7.5px -15px}.navbar-nav>li>a{padding-top:10px;padding-bottom:10px;line-height:20px}@media (max-width:767px){.navbar-nav .open .dropdown-menu{position:static;float:none;width:auto;margin-top:0;background-color:transparent;border:0;-webkit-box-shadow:none;box-shadow:none}.navbar-nav .open .dropdown-menu .dropdown-header,.navbar-nav .open .dropdown-menu>li>a{padding:5px 15px 5px 25px}.navbar-nav .open .dropdown-menu>li>a{line-height:20px}.navbar-nav .open .dropdown-menu>li>a:focus,.navbar-nav .open .dropdown-menu>li>a:hover{background-image:none}}@media (min-width:768px){.navbar-nav{float:left;margin:0}.navbar-nav>li{float:left}.navbar-nav>li>a{padding-top:15px;padding-bottom:15px}}.navbar-form{padding:10px 15px;margin-right:-15px;margin-left:-15px;border-top:1px solid transparent;border-bottom:1px solid transparent;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1);margin-top:8px;margin-bottom:8px}@media (min-width:768px){.navbar-form .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.navbar-form .form-control{display:inline-block;width:auto;vertical-align:middle}.navbar-form .form-control-static{display:inline-block}.navbar-form .input-group{display:inline-table;vertical-align:middle}.navbar-form .input-group .form-control,.navbar-form .input-group .input-group-addon,.navbar-form .input-group .input-group-btn{width:auto}.navbar-form .input-group>.form-control{width:100%}.navbar-form .control-label{margin-bottom:0;vertical-align:middle}.navbar-form .checkbox,.navbar-form .radio{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.navbar-form .checkbox label,.navbar-form .radio label{padding-left:0}.navbar-form .checkbox input[type=checkbox],.navbar-form .radio input[type=radio]{position:relative;margin-left:0}.navbar-form .has-feedback .form-control-feedback{top:0}}@media (max-width:767px){.navbar-form .form-group{margin-bottom:5px}.navbar-form .form-group:last-child{margin-bottom:0}}@media (min-width:768px){.navbar-form{width:auto;padding-top:0;padding-bottom:0;margin-right:0;margin-left:0;border:0;-webkit-box-shadow:none;box-shadow:none}}.navbar-nav>li>.dropdown-menu{margin-top:0;border-top-left-radius:0;border-top-right-radius:0}.navbar-fixed-bottom .navbar-nav>li>.dropdown-menu{margin-bottom:0;border-top-left-radius:4px;border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.navbar-btn{margin-top:8px;margin-bottom:8px}.navbar-btn.btn-sm{margin-top:10px;margin-bottom:10px}.navbar-btn.btn-xs{margin-top:14px;margin-bottom:14px}.navbar-text{margin-top:15px;margin-bottom:15px}@media (min-width:768px){.navbar-text{float:left;margin-right:15px;margin-left:15px}}@media (min-width:768px){.navbar-left{float:left!important}.navbar-right{float:right!important;margin-right:-15px}.navbar-right~.navbar-right{margin-right:0}}.navbar-default{background-color:#f8f8f8;border-color:#e7e7e7}.navbar-default .navbar-brand{color:#777}.navbar-default .navbar-brand:focus,.navbar-default .navbar-brand:hover{color:#5e5e5e;background-color:transparent}.navbar-default .navbar-text{color:#777}.navbar-default .navbar-nav>li>a{color:#777}.navbar-default .navbar-nav>li>a:focus,.navbar-default .navbar-nav>li>a:hover{color:#333;background-color:transparent}.navbar-default .navbar-nav>.active>a,.navbar-default .navbar-nav>.active>a:focus,.navbar-default .navbar-nav>.active>a:hover{color:#555;background-color:#e7e7e7}.navbar-default .navbar-nav>.disabled>a,.navbar-default .navbar-nav>.disabled>a:focus,.navbar-default .navbar-nav>.disabled>a:hover{color:#ccc;background-color:transparent}.navbar-default .navbar-nav>.open>a,.navbar-default .navbar-nav>.open>a:focus,.navbar-default .navbar-nav>.open>a:hover{color:#555;background-color:#e7e7e7}@media (max-width:767px){.navbar-default .navbar-nav .open .dropdown-menu>li>a{color:#777}.navbar-default .navbar-nav .open .dropdown-menu>li>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>li>a:hover{color:#333;background-color:transparent}.navbar-default .navbar-nav .open .dropdown-menu>.active>a,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:hover{color:#555;background-color:#e7e7e7}.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:hover{color:#ccc;background-color:transparent}}.navbar-default .navbar-toggle{border-color:#ddd}.navbar-default .navbar-toggle:focus,.navbar-default .navbar-toggle:hover{background-color:#ddd}.navbar-default .navbar-toggle .icon-bar{background-color:#888}.navbar-default .navbar-collapse,.navbar-default .navbar-form{border-color:#e7e7e7}.navbar-default .navbar-link{color:#777}.navbar-default .navbar-link:hover{color:#333}.navbar-default .btn-link{color:#777}.navbar-default .btn-link:focus,.navbar-default .btn-link:hover{color:#333}.navbar-default .btn-link[disabled]:focus,.navbar-default .btn-link[disabled]:hover,fieldset[disabled] .navbar-default .btn-link:focus,fieldset[disabled] .navbar-default .btn-link:hover{color:#ccc}.navbar-inverse{background-color:#222;border-color:#080808}.navbar-inverse .navbar-brand{color:#9d9d9d}.navbar-inverse .navbar-brand:focus,.navbar-inverse .navbar-brand:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-text{color:#9d9d9d}.navbar-inverse .navbar-nav>li>a{color:#9d9d9d}.navbar-inverse .navbar-nav>li>a:focus,.navbar-inverse .navbar-nav>li>a:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-nav>.active>a,.navbar-inverse .navbar-nav>.active>a:focus,.navbar-inverse .navbar-nav>.active>a:hover{color:#fff;background-color:#080808}.navbar-inverse .navbar-nav>.disabled>a,.navbar-inverse .navbar-nav>.disabled>a:focus,.navbar-inverse .navbar-nav>.disabled>a:hover{color:#444;background-color:transparent}.navbar-inverse .navbar-nav>.open>a,.navbar-inverse .navbar-nav>.open>a:focus,.navbar-inverse .navbar-nav>.open>a:hover{color:#fff;background-color:#080808}@media (max-width:767px){.navbar-inverse .navbar-nav .open .dropdown-menu>.dropdown-header{border-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu .divider{background-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a{color:#9d9d9d}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:hover{color:#fff;background-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:hover{color:#444;background-color:transparent}}.navbar-inverse .navbar-toggle{border-color:#333}.navbar-inverse .navbar-toggle:focus,.navbar-inverse .navbar-toggle:hover{background-color:#333}.navbar-inverse .navbar-toggle .icon-bar{background-color:#fff}.navbar-inverse .navbar-collapse,.navbar-inverse .navbar-form{border-color:#101010}.navbar-inverse .navbar-link{color:#9d9d9d}.navbar-inverse .navbar-link:hover{color:#fff}.navbar-inverse .btn-link{color:#9d9d9d}.navbar-inverse .btn-link:focus,.navbar-inverse .btn-link:hover{color:#fff}.navbar-inverse .btn-link[disabled]:focus,.navbar-inverse .btn-link[disabled]:hover,fieldset[disabled] .navbar-inverse .btn-link:focus,fieldset[disabled] .navbar-inverse .btn-link:hover{color:#444}.breadcrumb{padding:8px 15px;margin-bottom:20px;list-style:none;background-color:#f5f5f5;border-radius:4px}.breadcrumb>li{display:inline-block}.breadcrumb>li+li:before{padding:0 5px;color:#ccc;content:"/\00a0"}.breadcrumb>.active{color:#777}.pagination{display:inline-block;padding-left:0;margin:20px 0;border-radius:4px}.pagination>li{display:inline}.pagination>li>a,.pagination>li>span{position:relative;float:left;padding:6px 12px;margin-left:-1px;line-height:1.42857143;color:#337ab7;text-decoration:none;background-color:#fff;border:1px solid #ddd}.pagination>li>a:focus,.pagination>li>a:hover,.pagination>li>span:focus,.pagination>li>span:hover{z-index:2;color:#23527c;background-color:#eee;border-color:#ddd}.pagination>li:first-child>a,.pagination>li:first-child>span{margin-left:0;border-top-left-radius:4px;border-bottom-left-radius:4px}.pagination>li:last-child>a,.pagination>li:last-child>span{border-top-right-radius:4px;border-bottom-right-radius:4px}.pagination>.active>a,.pagination>.active>a:focus,.pagination>.active>a:hover,.pagination>.active>span,.pagination>.active>span:focus,.pagination>.active>span:hover{z-index:3;color:#fff;cursor:default;background-color:#337ab7;border-color:#337ab7}.pagination>.disabled>a,.pagination>.disabled>a:focus,.pagination>.disabled>a:hover,.pagination>.disabled>span,.pagination>.disabled>span:focus,.pagination>.disabled>span:hover{color:#777;cursor:not-allowed;background-color:#fff;border-color:#ddd}.pagination-lg>li>a,.pagination-lg>li>span{padding:10px 16px;font-size:18px;line-height:1.3333333}.pagination-lg>li:first-child>a,.pagination-lg>li:first-child>span{border-top-left-radius:6px;border-bottom-left-radius:6px}.pagination-lg>li:last-child>a,.pagination-lg>li:last-child>span{border-top-right-radius:6px;border-bottom-right-radius:6px}.pagination-sm>li>a,.pagination-sm>li>span{padding:5px 10px;font-size:12px;line-height:1.5}.pagination-sm>li:first-child>a,.pagination-sm>li:first-child>span{border-top-left-radius:3px;border-bottom-left-radius:3px}.pagination-sm>li:last-child>a,.pagination-sm>li:last-child>span{border-top-right-radius:3px;border-bottom-right-radius:3px}.pager{padding-left:0;margin:20px 0;text-align:center;list-style:none}.pager li{display:inline}.pager li>a,.pager li>span{display:inline-block;padding:5px 14px;background-color:#fff;border:1px solid #ddd;border-radius:15px}.pager li>a:focus,.pager li>a:hover{text-decoration:none;background-color:#eee}.pager .next>a,.pager .next>span{float:right}.pager .previous>a,.pager .previous>span{float:left}.pager .disabled>a,.pager .disabled>a:focus,.pager .disabled>a:hover,.pager .disabled>span{color:#777;cursor:not-allowed;background-color:#fff}.label{display:inline;padding:.2em .6em .3em;font-size:75%;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:baseline;border-radius:.25em}a.label:focus,a.label:hover{color:#fff;text-decoration:none;cursor:pointer}.label:empty{display:none}.btn .label{position:relative;top:-1px}.label-default{background-color:#777}.label-default[href]:focus,.label-default[href]:hover{background-color:#5e5e5e}.label-primary{background-color:#337ab7}.label-primary[href]:focus,.label-primary[href]:hover{background-color:#286090}.label-success{background-color:#5cb85c}.label-success[href]:focus,.label-success[href]:hover{background-color:#449d44}.label-info{background-color:#5bc0de}.label-info[href]:focus,.label-info[href]:hover{background-color:#31b0d5}.label-warning{background-color:#f0ad4e}.label-warning[href]:focus,.label-warning[href]:hover{background-color:#ec971f}.label-danger{background-color:#d9534f}.label-danger[href]:focus,.label-danger[href]:hover{background-color:#c9302c}.badge{display:inline-block;min-width:10px;padding:3px 7px;font-size:12px;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:middle;background-color:#777;border-radius:10px}.badge:empty{display:none}.btn .badge{position:relative;top:-1px}.btn-group-xs>.btn .badge,.btn-xs .badge{top:0;padding:1px 5px}a.badge:focus,a.badge:hover{color:#fff;text-decoration:none;cursor:pointer}.list-group-item.active>.badge,.nav-pills>.active>a>.badge{color:#337ab7;background-color:#fff}.list-group-item>.badge{float:right}.list-group-item>.badge+.badge{margin-right:5px}.nav-pills>li>a>.badge{margin-left:3px}.jumbotron{padding-top:30px;padding-bottom:30px;margin-bottom:30px;color:inherit;background-color:#eee}.jumbotron .h1,.jumbotron h1{color:inherit}.jumbotron p{margin-bottom:15px;font-size:21px;font-weight:200}.jumbotron>hr{border-top-color:#d5d5d5}.container .jumbotron,.container-fluid .jumbotron{padding-right:15px;padding-left:15px;border-radius:6px}.jumbotron .container{max-width:100%}@media screen and (min-width:768px){.jumbotron{padding-top:48px;padding-bottom:48px}.container .jumbotron,.container-fluid .jumbotron{padding-right:60px;padding-left:60px}.jumbotron .h1,.jumbotron h1{font-size:63px}}.thumbnail{display:block;padding:4px;margin-bottom:20px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:border .2s ease-in-out;-o-transition:border .2s ease-in-out;transition:border .2s ease-in-out}.thumbnail a>img,.thumbnail>img{margin-right:auto;margin-left:auto}a.thumbnail.active,a.thumbnail:focus,a.thumbnail:hover{border-color:#337ab7}.thumbnail .caption{padding:9px;color:#333}.alert{padding:15px;margin-bottom:20px;border:1px solid transparent;border-radius:4px}.alert h4{margin-top:0;color:inherit}.alert .alert-link{font-weight:700}.alert>p,.alert>ul{margin-bottom:0}.alert>p+p{margin-top:5px}.alert-dismissable,.alert-dismissible{padding-right:35px}.alert-dismissable .close,.alert-dismissible .close{position:relative;top:-2px;right:-21px;color:inherit}.alert-success{color:#3c763d;background-color:#dff0d8;border-color:#d6e9c6}.alert-success hr{border-top-color:#c9e2b3}.alert-success .alert-link{color:#2b542c}.alert-info{color:#31708f;background-color:#d9edf7;border-color:#bce8f1}.alert-info hr{border-top-color:#a6e1ec}.alert-info .alert-link{color:#245269}.alert-warning{color:#8a6d3b;background-color:#fcf8e3;border-color:#faebcc}.alert-warning hr{border-top-color:#f7e1b5}.alert-warning .alert-link{color:#66512c}.alert-danger{color:#a94442;background-color:#f2dede;border-color:#ebccd1}.alert-danger hr{border-top-color:#e4b9c0}.alert-danger .alert-link{color:#843534}@-webkit-keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}@-o-keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}@keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}.progress{height:20px;margin-bottom:20px;overflow:hidden;background-color:#f5f5f5;border-radius:4px;-webkit-box-shadow:inset 0 1px 2px rgba(0,0,0,.1);box-shadow:inset 0 1px 2px rgba(0,0,0,.1)}.progress-bar{float:left;width:0%;height:100%;font-size:12px;line-height:20px;color:#fff;text-align:center;background-color:#337ab7;-webkit-box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);-webkit-transition:width .6s ease;-o-transition:width .6s ease;transition:width .6s ease}.progress-bar-striped,.progress-striped .progress-bar{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);-webkit-background-size:40px 40px;background-size:40px 40px}.progress-bar.active,.progress.active .progress-bar{-webkit-animation:progress-bar-stripes 2s linear infinite;-o-animation:progress-bar-stripes 2s linear infinite;animation:progress-bar-stripes 2s linear infinite}.progress-bar-success{background-color:#5cb85c}.progress-striped .progress-bar-success{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-info{background-color:#5bc0de}.progress-striped .progress-bar-info{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-warning{background-color:#f0ad4e}.progress-striped .progress-bar-warning{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-danger{background-color:#d9534f}.progress-striped .progress-bar-danger{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.media{margin-top:15px}.media:first-child{margin-top:0}.media,.media-body{overflow:hidden;zoom:1}.media-body{width:10000px}.media-object{display:block}.media-object.img-thumbnail{max-width:none}.media-right,.media>.pull-right{padding-left:10px}.media-left,.media>.pull-left{padding-right:10px}.media-body,.media-left,.media-right{display:table-cell;vertical-align:top}.media-middle{vertical-align:middle}.media-bottom{vertical-align:bottom}.media-heading{margin-top:0;margin-bottom:5px}.media-list{padding-left:0;list-style:none}.list-group{padding-left:0;margin-bottom:20px}.list-group-item{position:relative;display:block;padding:10px 15px;margin-bottom:-1px;background-color:#fff;border:1px solid #ddd}.list-group-item:first-child{border-top-left-radius:4px;border-top-right-radius:4px}.list-group-item:last-child{margin-bottom:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}.list-group-item.disabled,.list-group-item.disabled:focus,.list-group-item.disabled:hover{color:#777;cursor:not-allowed;background-color:#eee}.list-group-item.disabled .list-group-item-heading,.list-group-item.disabled:focus .list-group-item-heading,.list-group-item.disabled:hover .list-group-item-heading{color:inherit}.list-group-item.disabled .list-group-item-text,.list-group-item.disabled:focus .list-group-item-text,.list-group-item.disabled:hover .list-group-item-text{color:#777}.list-group-item.active,.list-group-item.active:focus,.list-group-item.active:hover{z-index:2;color:#fff;background-color:#337ab7;border-color:#337ab7}.list-group-item.active .list-group-item-heading,.list-group-item.active .list-group-item-heading>.small,.list-group-item.active .list-group-item-heading>small,.list-group-item.active:focus .list-group-item-heading,.list-group-item.active:focus .list-group-item-heading>.small,.list-group-item.active:focus .list-group-item-heading>small,.list-group-item.active:hover .list-group-item-heading,.list-group-item.active:hover .list-group-item-heading>.small,.list-group-item.active:hover .list-group-item-heading>small{color:inherit}.list-group-item.active .list-group-item-text,.list-group-item.active:focus .list-group-item-text,.list-group-item.active:hover .list-group-item-text{color:#c7ddef}a.list-group-item,button.list-group-item{color:#555}a.list-group-item .list-group-item-heading,button.list-group-item .list-group-item-heading{color:#333}a.list-group-item:focus,a.list-group-item:hover,button.list-group-item:focus,button.list-group-item:hover{color:#555;text-decoration:none;background-color:#f5f5f5}button.list-group-item{width:100%;text-align:left}.list-group-item-success{color:#3c763d;background-color:#dff0d8}a.list-group-item-success,button.list-group-item-success{color:#3c763d}a.list-group-item-success .list-group-item-heading,button.list-group-item-success .list-group-item-heading{color:inherit}a.list-group-item-success:focus,a.list-group-item-success:hover,button.list-group-item-success:focus,button.list-group-item-success:hover{color:#3c763d;background-color:#d0e9c6}a.list-group-item-success.active,a.list-group-item-success.active:focus,a.list-group-item-success.active:hover,button.list-group-item-success.active,button.list-group-item-success.active:focus,button.list-group-item-success.active:hover{color:#fff;background-color:#3c763d;border-color:#3c763d}.list-group-item-info{color:#31708f;background-color:#d9edf7}a.list-group-item-info,button.list-group-item-info{color:#31708f}a.list-group-item-info .list-group-item-heading,button.list-group-item-info .list-group-item-heading{color:inherit}a.list-group-item-info:focus,a.list-group-item-info:hover,button.list-group-item-info:focus,button.list-group-item-info:hover{color:#31708f;background-color:#c4e3f3}a.list-group-item-info.active,a.list-group-item-info.active:focus,a.list-group-item-info.active:hover,button.list-group-item-info.active,button.list-group-item-info.active:focus,button.list-group-item-info.active:hover{color:#fff;background-color:#31708f;border-color:#31708f}.list-group-item-warning{color:#8a6d3b;background-color:#fcf8e3}a.list-group-item-warning,button.list-group-item-warning{color:#8a6d3b}a.list-group-item-warning .list-group-item-heading,button.list-group-item-warning .list-group-item-heading{color:inherit}a.list-group-item-warning:focus,a.list-group-item-warning:hover,button.list-group-item-warning:focus,button.list-group-item-warning:hover{color:#8a6d3b;background-color:#faf2cc}a.list-group-item-warning.active,a.list-group-item-warning.active:focus,a.list-group-item-warning.active:hover,button.list-group-item-warning.active,button.list-group-item-warning.active:focus,button.list-group-item-warning.active:hover{color:#fff;background-color:#8a6d3b;border-color:#8a6d3b}.list-group-item-danger{color:#a94442;background-color:#f2dede}a.list-group-item-danger,button.list-group-item-danger{color:#a94442}a.list-group-item-danger .list-group-item-heading,button.list-group-item-danger .list-group-item-heading{color:inherit}a.list-group-item-danger:focus,a.list-group-item-danger:hover,button.list-group-item-danger:focus,button.list-group-item-danger:hover{color:#a94442;background-color:#ebcccc}a.list-group-item-danger.active,a.list-group-item-danger.active:focus,a.list-group-item-danger.active:hover,button.list-group-item-danger.active,button.list-group-item-danger.active:focus,button.list-group-item-danger.active:hover{color:#fff;background-color:#a94442;border-color:#a94442}.list-group-item-heading{margin-top:0;margin-bottom:5px}.list-group-item-text{margin-bottom:0;line-height:1.3}.panel{margin-bottom:20px;background-color:#fff;border:1px solid transparent;border-radius:4px;-webkit-box-shadow:0 1px 1px rgba(0,0,0,.05);box-shadow:0 1px 1px rgba(0,0,0,.05)}.panel-body{padding:15px}.panel-heading{padding:10px 15px;border-bottom:1px solid transparent;border-top-left-radius:3px;border-top-right-radius:3px}.panel-heading>.dropdown .dropdown-toggle{color:inherit}.panel-title{margin-top:0;margin-bottom:0;font-size:16px;color:inherit}.panel-title>.small,.panel-title>.small>a,.panel-title>a,.panel-title>small,.panel-title>small>a{color:inherit}.panel-footer{padding:10px 15px;background-color:#f5f5f5;border-top:1px solid #ddd;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.list-group,.panel>.panel-collapse>.list-group{margin-bottom:0}.panel>.list-group .list-group-item,.panel>.panel-collapse>.list-group .list-group-item{border-width:1px 0;border-radius:0}.panel>.list-group:first-child .list-group-item:first-child,.panel>.panel-collapse>.list-group:first-child .list-group-item:first-child{border-top:0;border-top-left-radius:3px;border-top-right-radius:3px}.panel>.list-group:last-child .list-group-item:last-child,.panel>.panel-collapse>.list-group:last-child .list-group-item:last-child{border-bottom:0;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.panel-heading+.panel-collapse>.list-group .list-group-item:first-child{border-top-left-radius:0;border-top-right-radius:0}.panel-heading+.list-group .list-group-item:first-child{border-top-width:0}.list-group+.panel-footer{border-top-width:0}.panel>.panel-collapse>.table,.panel>.table,.panel>.table-responsive>.table{margin-bottom:0}.panel>.panel-collapse>.table caption,.panel>.table caption,.panel>.table-responsive>.table caption{padding-right:15px;padding-left:15px}.panel>.table-responsive:first-child>.table:first-child,.panel>.table:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child,.panel>.table:first-child>thead:first-child>tr:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table:first-child>thead:first-child>tr:first-child th:first-child{border-top-left-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table:first-child>thead:first-child>tr:first-child th:last-child{border-top-right-radius:3px}.panel>.table-responsive:last-child>.table:last-child,.panel>.table:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:first-child{border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:last-child{border-bottom-right-radius:3px}.panel>.panel-body+.table,.panel>.panel-body+.table-responsive,.panel>.table+.panel-body,.panel>.table-responsive+.panel-body{border-top:1px solid #ddd}.panel>.table>tbody:first-child>tr:first-child td,.panel>.table>tbody:first-child>tr:first-child th{border-top:0}.panel>.table-bordered,.panel>.table-responsive>.table-bordered{border:0}.panel>.table-bordered>tbody>tr>td:first-child,.panel>.table-bordered>tbody>tr>th:first-child,.panel>.table-bordered>tfoot>tr>td:first-child,.panel>.table-bordered>tfoot>tr>th:first-child,.panel>.table-bordered>thead>tr>td:first-child,.panel>.table-bordered>thead>tr>th:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:first-child,.panel>.table-responsive>.table-bordered>thead>tr>td:first-child,.panel>.table-responsive>.table-bordered>thead>tr>th:first-child{border-left:0}.panel>.table-bordered>tbody>tr>td:last-child,.panel>.table-bordered>tbody>tr>th:last-child,.panel>.table-bordered>tfoot>tr>td:last-child,.panel>.table-bordered>tfoot>tr>th:last-child,.panel>.table-bordered>thead>tr>td:last-child,.panel>.table-bordered>thead>tr>th:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:last-child,.panel>.table-responsive>.table-bordered>thead>tr>td:last-child,.panel>.table-responsive>.table-bordered>thead>tr>th:last-child{border-right:0}.panel>.table-bordered>tbody>tr:first-child>td,.panel>.table-bordered>tbody>tr:first-child>th,.panel>.table-bordered>thead>tr:first-child>td,.panel>.table-bordered>thead>tr:first-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>th,.panel>.table-responsive>.table-bordered>thead>tr:first-child>td,.panel>.table-responsive>.table-bordered>thead>tr:first-child>th{border-bottom:0}.panel>.table-bordered>tbody>tr:last-child>td,.panel>.table-bordered>tbody>tr:last-child>th,.panel>.table-bordered>tfoot>tr:last-child>td,.panel>.table-bordered>tfoot>tr:last-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>th,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>td,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}.panel>.table-responsive{margin-bottom:0;border:0}.panel-group{margin-bottom:20px}.panel-group .panel{margin-bottom:0;border-radius:4px}.panel-group .panel+.panel{margin-top:5px}.panel-group .panel-heading{border-bottom:0}.panel-group .panel-heading+.panel-collapse>.list-group,.panel-group .panel-heading+.panel-collapse>.panel-body{border-top:1px solid #ddd}.panel-group .panel-footer{border-top:0}.panel-group .panel-footer+.panel-collapse .panel-body{border-bottom:1px solid #ddd}.panel-default{border-color:#ddd}.panel-default>.panel-heading{color:#333;background-color:#f5f5f5;border-color:#ddd}.panel-default>.panel-heading+.panel-collapse>.panel-body{border-top-color:#ddd}.panel-default>.panel-heading .badge{color:#f5f5f5;background-color:#333}.panel-default>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#ddd}.panel-primary{border-color:#337ab7}.panel-primary>.panel-heading{color:#fff;background-color:#337ab7;border-color:#337ab7}.panel-primary>.panel-heading+.panel-collapse>.panel-body{border-top-color:#337ab7}.panel-primary>.panel-heading .badge{color:#337ab7;background-color:#fff}.panel-primary>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#337ab7}.panel-success{border-color:#d6e9c6}.panel-success>.panel-heading{color:#3c763d;background-color:#dff0d8;border-color:#d6e9c6}.panel-success>.panel-heading+.panel-collapse>.panel-body{border-top-color:#d6e9c6}.panel-success>.panel-heading .badge{color:#dff0d8;background-color:#3c763d}.panel-success>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#d6e9c6}.panel-info{border-color:#bce8f1}.panel-info>.panel-heading{color:#31708f;background-color:#d9edf7;border-color:#bce8f1}.panel-info>.panel-heading+.panel-collapse>.panel-body{border-top-color:#bce8f1}.panel-info>.panel-heading .badge{color:#d9edf7;background-color:#31708f}.panel-info>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#bce8f1}.panel-warning{border-color:#faebcc}.panel-warning>.panel-heading{color:#8a6d3b;background-color:#fcf8e3;border-color:#faebcc}.panel-warning>.panel-heading+.panel-collapse>.panel-body{border-top-color:#faebcc}.panel-warning>.panel-heading .badge{color:#fcf8e3;background-color:#8a6d3b}.panel-warning>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#faebcc}.panel-danger{border-color:#ebccd1}.panel-danger>.panel-heading{color:#a94442;background-color:#f2dede;border-color:#ebccd1}.panel-danger>.panel-heading+.panel-collapse>.panel-body{border-top-color:#ebccd1}.panel-danger>.panel-heading .badge{color:#f2dede;background-color:#a94442}.panel-danger>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#ebccd1}.embed-responsive{position:relative;display:block;height:0;padding:0;overflow:hidden}.embed-responsive .embed-responsive-item,.embed-responsive embed,.embed-responsive iframe,.embed-responsive object,.embed-responsive video{position:absolute;top:0;bottom:0;left:0;width:100%;height:100%;border:0}.embed-responsive-16by9{padding-bottom:56.25%}.embed-responsive-4by3{padding-bottom:75%}.well{min-height:20px;padding:19px;margin-bottom:20px;background-color:#f5f5f5;border:1px solid #e3e3e3;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.05);box-shadow:inset 0 1px 1px rgba(0,0,0,.05)}.well blockquote{border-color:#ddd;border-color:rgba(0,0,0,.15)}.well-lg{padding:24px;border-radius:6px}.well-sm{padding:9px;border-radius:3px}.close{float:right;font-size:21px;font-weight:700;line-height:1;color:#000;text-shadow:0 1px 0 #fff;filter:alpha(opacity=20);opacity:.2}.close:focus,.close:hover{color:#000;text-decoration:none;cursor:pointer;filter:alpha(opacity=50);opacity:.5}button.close{padding:0;cursor:pointer;background:0 0;border:0;-webkit-appearance:none;-moz-appearance:none;appearance:none}.modal-open{overflow:hidden}.modal{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1050;display:none;overflow:hidden;-webkit-overflow-scrolling:touch;outline:0}.modal.fade .modal-dialog{-webkit-transform:translate(0,-25%);-ms-transform:translate(0,-25%);-o-transform:translate(0,-25%);transform:translate(0,-25%);-webkit-transition:-webkit-transform .3s ease-out;-o-transition:-o-transform .3s ease-out;transition:-webkit-transform .3s ease-out;transition:transform .3s ease-out;transition:transform .3s ease-out,-webkit-transform .3s ease-out,-o-transform .3s ease-out}.modal.in .modal-dialog{-webkit-transform:translate(0,0);-ms-transform:translate(0,0);-o-transform:translate(0,0);transform:translate(0,0)}.modal-open .modal{overflow-x:hidden;overflow-y:auto}.modal-dialog{position:relative;width:auto;margin:10px}.modal-content{position:relative;background-color:#fff;background-clip:padding-box;border:1px solid #999;border:1px solid rgba(0,0,0,.2);border-radius:6px;-webkit-box-shadow:0 3px 9px rgba(0,0,0,.5);box-shadow:0 3px 9px rgba(0,0,0,.5);outline:0}.modal-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1040;background-color:#000}.modal-backdrop.fade{filter:alpha(opacity=0);opacity:0}.modal-backdrop.in{filter:alpha(opacity=50);opacity:.5}.modal-header{padding:15px;border-bottom:1px solid #e5e5e5}.modal-header .close{margin-top:-2px}.modal-title{margin:0;line-height:1.42857143}.modal-body{position:relative;padding:15px}.modal-footer{padding:15px;text-align:right;border-top:1px solid #e5e5e5}.modal-footer .btn+.btn{margin-bottom:0;margin-left:5px}.modal-footer .btn-group .btn+.btn{margin-left:-1px}.modal-footer .btn-block+.btn-block{margin-left:0}.modal-scrollbar-measure{position:absolute;top:-9999px;width:50px;height:50px;overflow:scroll}@media (min-width:768px){.modal-dialog{width:600px;margin:30px auto}.modal-content{-webkit-box-shadow:0 5px 15px rgba(0,0,0,.5);box-shadow:0 5px 15px rgba(0,0,0,.5)}.modal-sm{width:300px}}@media (min-width:992px){.modal-lg{width:900px}}.tooltip{position:absolute;z-index:1070;display:block;font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-style:normal;font-weight:400;line-height:1.42857143;line-break:auto;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;word-spacing:normal;word-wrap:normal;white-space:normal;font-size:12px;filter:alpha(opacity=0);opacity:0}.tooltip.in{filter:alpha(opacity=90);opacity:.9}.tooltip.top{padding:5px 0;margin-top:-3px}.tooltip.right{padding:0 5px;margin-left:3px}.tooltip.bottom{padding:5px 0;margin-top:3px}.tooltip.left{padding:0 5px;margin-left:-3px}.tooltip.top .tooltip-arrow{bottom:0;left:50%;margin-left:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-left .tooltip-arrow{right:5px;bottom:0;margin-bottom:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-right .tooltip-arrow{bottom:0;left:5px;margin-bottom:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.right .tooltip-arrow{top:50%;left:0;margin-top:-5px;border-width:5px 5px 5px 0;border-right-color:#000}.tooltip.left .tooltip-arrow{top:50%;right:0;margin-top:-5px;border-width:5px 0 5px 5px;border-left-color:#000}.tooltip.bottom .tooltip-arrow{top:0;left:50%;margin-left:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-left .tooltip-arrow{top:0;right:5px;margin-top:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-right .tooltip-arrow{top:0;left:5px;margin-top:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip-inner{max-width:200px;padding:3px 8px;color:#fff;text-align:center;background-color:#000;border-radius:4px}.tooltip-arrow{position:absolute;width:0;height:0;border-color:transparent;border-style:solid}.popover{position:absolute;top:0;left:0;z-index:1060;display:none;max-width:276px;padding:1px;font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-style:normal;font-weight:400;line-height:1.42857143;line-break:auto;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;word-spacing:normal;word-wrap:normal;white-space:normal;font-size:14px;background-color:#fff;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.2);border-radius:6px;-webkit-box-shadow:0 5px 10px rgba(0,0,0,.2);box-shadow:0 5px 10px rgba(0,0,0,.2)}.popover.top{margin-top:-10px}.popover.right{margin-left:10px}.popover.bottom{margin-top:10px}.popover.left{margin-left:-10px}.popover>.arrow{border-width:11px}.popover>.arrow,.popover>.arrow:after{position:absolute;display:block;width:0;height:0;border-color:transparent;border-style:solid}.popover>.arrow:after{content:"";border-width:10px}.popover.top>.arrow{bottom:-11px;left:50%;margin-left:-11px;border-top-color:#999;border-top-color:rgba(0,0,0,.25);border-bottom-width:0}.popover.top>.arrow:after{bottom:1px;margin-left:-10px;content:" ";border-top-color:#fff;border-bottom-width:0}.popover.right>.arrow{top:50%;left:-11px;margin-top:-11px;border-right-color:#999;border-right-color:rgba(0,0,0,.25);border-left-width:0}.popover.right>.arrow:after{bottom:-10px;left:1px;content:" ";border-right-color:#fff;border-left-width:0}.popover.bottom>.arrow{top:-11px;left:50%;margin-left:-11px;border-top-width:0;border-bottom-color:#999;border-bottom-color:rgba(0,0,0,.25)}.popover.bottom>.arrow:after{top:1px;margin-left:-10px;content:" ";border-top-width:0;border-bottom-color:#fff}.popover.left>.arrow{top:50%;right:-11px;margin-top:-11px;border-right-width:0;border-left-color:#999;border-left-color:rgba(0,0,0,.25)}.popover.left>.arrow:after{right:1px;bottom:-10px;content:" ";border-right-width:0;border-left-color:#fff}.popover-title{padding:8px 14px;margin:0;font-size:14px;background-color:#f7f7f7;border-bottom:1px solid #ebebeb;border-radius:5px 5px 0 0}.popover-content{padding:9px 14px}.carousel{position:relative}.carousel-inner{position:relative;width:100%;overflow:hidden}.carousel-inner>.item{position:relative;display:none;-webkit-transition:.6s ease-in-out left;-o-transition:.6s ease-in-out left;transition:.6s ease-in-out left}.carousel-inner>.item>a>img,.carousel-inner>.item>img{line-height:1}@media all and (transform-3d),(-webkit-transform-3d){.carousel-inner>.item{-webkit-transition:-webkit-transform .6s ease-in-out;-o-transition:-o-transform .6s ease-in-out;transition:-webkit-transform .6s ease-in-out;transition:transform .6s ease-in-out;transition:transform .6s ease-in-out,-webkit-transform .6s ease-in-out,-o-transform .6s ease-in-out;-webkit-backface-visibility:hidden;backface-visibility:hidden;-webkit-perspective:1000px;perspective:1000px}.carousel-inner>.item.active.right,.carousel-inner>.item.next{-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0);left:0}.carousel-inner>.item.active.left,.carousel-inner>.item.prev{-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0);left:0}.carousel-inner>.item.active,.carousel-inner>.item.next.left,.carousel-inner>.item.prev.right{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0);left:0}}.carousel-inner>.active,.carousel-inner>.next,.carousel-inner>.prev{display:block}.carousel-inner>.active{left:0}.carousel-inner>.next,.carousel-inner>.prev{position:absolute;top:0;width:100%}.carousel-inner>.next{left:100%}.carousel-inner>.prev{left:-100%}.carousel-inner>.next.left,.carousel-inner>.prev.right{left:0}.carousel-inner>.active.left{left:-100%}.carousel-inner>.active.right{left:100%}.carousel-control{position:absolute;top:0;bottom:0;left:0;width:15%;font-size:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6);background-color:rgba(0,0,0,0);filter:alpha(opacity=50);opacity:.5}.carousel-control.left{background-image:-webkit-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:-webkit-gradient(linear,left top,right top,from(rgba(0,0,0,.5)),to(rgba(0,0,0,.0001)));background-image:linear-gradient(to right,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);background-repeat:repeat-x}.carousel-control.right{right:0;left:auto;background-image:-webkit-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:-webkit-gradient(linear,left top,right top,from(rgba(0,0,0,.0001)),to(rgba(0,0,0,.5)));background-image:linear-gradient(to right,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);background-repeat:repeat-x}.carousel-control:focus,.carousel-control:hover{color:#fff;text-decoration:none;outline:0;filter:alpha(opacity=90);opacity:.9}.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next,.carousel-control .icon-prev{position:absolute;top:50%;z-index:5;display:inline-block;margin-top:-10px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{left:50%;margin-left:-10px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{right:50%;margin-right:-10px}.carousel-control .icon-next,.carousel-control .icon-prev{width:20px;height:20px;font-family:serif;line-height:1}.carousel-control .icon-prev:before{content:"\2039"}.carousel-control .icon-next:before{content:"\203a"}.carousel-indicators{position:absolute;bottom:10px;left:50%;z-index:15;width:60%;padding-left:0;margin-left:-30%;text-align:center;list-style:none}.carousel-indicators li{display:inline-block;width:10px;height:10px;margin:1px;text-indent:-999px;cursor:pointer;background-color:#000\9;background-color:rgba(0,0,0,0);border:1px solid #fff;border-radius:10px}.carousel-indicators .active{width:12px;height:12px;margin:0;background-color:#fff}.carousel-caption{position:absolute;right:15%;bottom:20px;left:15%;z-index:10;padding-top:20px;padding-bottom:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6)}.carousel-caption .btn{text-shadow:none}@media screen and (min-width:768px){.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next,.carousel-control .icon-prev{width:30px;height:30px;margin-top:-10px;font-size:30px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{margin-left:-10px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{margin-right:-10px}.carousel-caption{right:20%;left:20%;padding-bottom:30px}.carousel-indicators{bottom:20px}}.btn-group-vertical>.btn-group:after,.btn-group-vertical>.btn-group:before,.btn-toolbar:after,.btn-toolbar:before,.clearfix:after,.clearfix:before,.container-fluid:after,.container-fluid:before,.container:after,.container:before,.dl-horizontal dd:after,.dl-horizontal dd:before,.form-horizontal .form-group:after,.form-horizontal .form-group:before,.modal-footer:after,.modal-footer:before,.modal-header:after,.modal-header:before,.nav:after,.nav:before,.navbar-collapse:after,.navbar-collapse:before,.navbar-header:after,.navbar-header:before,.navbar:after,.navbar:before,.pager:after,.pager:before,.panel-body:after,.panel-body:before,.row:after,.row:before{display:table;content:" "}.btn-group-vertical>.btn-group:after,.btn-toolbar:after,.clearfix:after,.container-fluid:after,.container:after,.dl-horizontal dd:after,.form-horizontal .form-group:after,.modal-footer:after,.modal-header:after,.nav:after,.navbar-collapse:after,.navbar-header:after,.navbar:after,.pager:after,.panel-body:after,.row:after{clear:both}.center-block{display:block;margin-right:auto;margin-left:auto}.pull-right{float:right!important}.pull-left{float:left!important}.hide{display:none!important}.show{display:block!important}.invisible{visibility:hidden}.text-hide{font:0/0 a;color:transparent;text-shadow:none;background-color:transparent;border:0}.hidden{display:none!important}.affix{position:fixed}@-ms-viewport{width:device-width}.visible-lg,.visible-md,.visible-sm,.visible-xs{display:none!important}.visible-lg-block,.visible-lg-inline,.visible-lg-inline-block,.visible-md-block,.visible-md-inline,.visible-md-inline-block,.visible-sm-block,.visible-sm-inline,.visible-sm-inline-block,.visible-xs-block,.visible-xs-inline,.visible-xs-inline-block{display:none!important}@media (max-width:767px){.visible-xs{display:block!important}table.visible-xs{display:table!important}tr.visible-xs{display:table-row!important}td.visible-xs,th.visible-xs{display:table-cell!important}}@media (max-width:767px){.visible-xs-block{display:block!important}}@media (max-width:767px){.visible-xs-inline{display:inline!important}}@media (max-width:767px){.visible-xs-inline-block{display:inline-block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm{display:block!important}table.visible-sm{display:table!important}tr.visible-sm{display:table-row!important}td.visible-sm,th.visible-sm{display:table-cell!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-block{display:block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline{display:inline!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline-block{display:inline-block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md{display:block!important}table.visible-md{display:table!important}tr.visible-md{display:table-row!important}td.visible-md,th.visible-md{display:table-cell!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-block{display:block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline{display:inline!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline-block{display:inline-block!important}}@media (min-width:1200px){.visible-lg{display:block!important}table.visible-lg{display:table!important}tr.visible-lg{display:table-row!important}td.visible-lg,th.visible-lg{display:table-cell!important}}@media (min-width:1200px){.visible-lg-block{display:block!important}}@media (min-width:1200px){.visible-lg-inline{display:inline!important}}@media (min-width:1200px){.visible-lg-inline-block{display:inline-block!important}}@media (max-width:767px){.hidden-xs{display:none!important}}@media (min-width:768px) and (max-width:991px){.hidden-sm{display:none!important}}@media (min-width:992px) and (max-width:1199px){.hidden-md{display:none!important}}@media (min-width:1200px){.hidden-lg{display:none!important}}.visible-print{display:none!important}@media print{.visible-print{display:block!important}table.visible-print{display:table!important}tr.visible-print{display:table-row!important}td.visible-print,th.visible-print{display:table-cell!important}}.visible-print-block{display:none!important}@media print{.visible-print-block{display:block!important}}.visible-print-inline{display:none!important}@media print{.visible-print-inline{display:inline!important}}.visible-print-inline-block{display:none!important}@media print{.visible-print-inline-block{display:inline-block!important}}@media print{.hidden-print{display:none!important}}
+ *//*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */html{font-family:sans-serif;-webkit-text-size-adjust:100%;-ms-text-size-adjust:100%}body{margin:0}article,aside,details,figcaption,figure,footer,header,hgroup,main,menu,nav,section,summary{display:block}audio,canvas,progress,video{display:inline-block;vertical-align:baseline}audio:not([controls]){display:none;height:0}[hidden],template{display:none}a{background-color:transparent}a:active,a:hover{outline:0}abbr[title]{border-bottom:1px dotted}b,strong{font-weight:700}dfn{font-style:italic}h1{margin:.67em 0;font-size:2em}mark{color:#000;background:#ff0}small{font-size:80%}sub,sup{position:relative;font-size:75%;line-height:0;vertical-align:baseline}sup{top:-.5em}sub{bottom:-.25em}img{border:0}svg:not(:root){overflow:hidden}figure{margin:1em 40px}hr{height:0;-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box}pre{overflow:auto}code,kbd,pre,samp{font-family:monospace,monospace;font-size:1em}button,input,optgroup,select,textarea{margin:0;font:inherit;color:inherit}button{overflow:visible}button,select{text-transform:none}button,html input[type=button],input[type=reset],input[type=submit]{-webkit-appearance:button;cursor:pointer}button[disabled],html input[disabled]{cursor:default}button::-moz-focus-inner,input::-moz-focus-inner{padding:0;border:0}input{line-height:normal}input[type=checkbox],input[type=radio]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;padding:0}input[type=number]::-webkit-inner-spin-button,input[type=number]::-webkit-outer-spin-button{height:auto}input[type=search]{-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box;-webkit-appearance:textfield}input[type=search]::-webkit-search-cancel-button,input[type=search]::-webkit-search-decoration{-webkit-appearance:none}fieldset{padding:.35em .625em .75em;margin:0 2px;border:1px solid silver}legend{padding:0;border:0}textarea{overflow:auto}optgroup{font-weight:700}table{border-spacing:0;border-collapse:collapse}td,th{padding:0}/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */@media print{*,:after,:before{color:#000!important;text-shadow:none!important;background:0 0!important;-webkit-box-shadow:none!important;box-shadow:none!important}a,a:visited{text-decoration:underline}a[href]:after{content:" (" attr(href) ")"}abbr[title]:after{content:" (" attr(title) ")"}a[href^="javascript:"]:after,a[href^="#"]:after{content:""}blockquote,pre{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}img,tr{page-break-inside:avoid}img{max-width:100%!important}h2,h3,p{orphans:3;widows:3}h2,h3{page-break-after:avoid}.navbar{display:none}.btn>.caret,.dropup>.btn>.caret{border-top-color:#000!important}.label{border:1px solid #000}.table{border-collapse:collapse!important}.table td,.table th{background-color:#fff!important}.table-bordered td,.table-bordered th{border:1px solid #ddd!important}}@font-face{font-family:'Glyphicons Halflings';src:url(../fonts/glyphicons-halflings-regular.eot);src:url(../fonts/glyphicons-halflings-regular.eot?#iefix) format('embedded-opentype'),url(../fonts/glyphicons-halflings-regular.woff2) format('woff2'),url(../fonts/glyphicons-halflings-regular.woff) format('woff'),url(../fonts/glyphicons-halflings-regular.ttf) format('truetype'),url(../fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular) format('svg')}.glyphicon{position:relative;top:1px;display:inline-block;font-family:'Glyphicons Halflings';font-style:normal;font-weight:400;line-height:1;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.glyphicon-asterisk:before{content:"\002a"}.glyphicon-plus:before{content:"\002b"}.glyphicon-eur:before,.glyphicon-euro:before{content:"\20ac"}.glyphicon-minus:before{content:"\2212"}.glyphicon-cloud:before{content:"\2601"}.glyphicon-envelope:before{content:"\2709"}.glyphicon-pencil:before{content:"\270f"}.glyphicon-glass:before{content:"\e001"}.glyphicon-music:before{content:"\e002"}.glyphicon-search:before{content:"\e003"}.glyphicon-heart:before{content:"\e005"}.glyphicon-star:before{content:"\e006"}.glyphicon-star-empty:before{content:"\e007"}.glyphicon-user:before{content:"\e008"}.glyphicon-film:before{content:"\e009"}.glyphicon-th-large:before{content:"\e010"}.glyphicon-th:before{content:"\e011"}.glyphicon-th-list:before{content:"\e012"}.glyphicon-ok:before{content:"\e013"}.glyphicon-remove:before{content:"\e014"}.glyphicon-zoom-in:before{content:"\e015"}.glyphicon-zoom-out:before{content:"\e016"}.glyphicon-off:before{content:"\e017"}.glyphicon-signal:before{content:"\e018"}.glyphicon-cog:before{content:"\e019"}.glyphicon-trash:before{content:"\e020"}.glyphicon-home:before{content:"\e021"}.glyphicon-file:before{content:"\e022"}.glyphicon-time:before{content:"\e023"}.glyphicon-road:before{content:"\e024"}.glyphicon-download-alt:before{content:"\e025"}.glyphicon-download:before{content:"\e026"}.glyphicon-upload:before{content:"\e027"}.glyphicon-inbox:before{content:"\e028"}.glyphicon-play-circle:before{content:"\e029"}.glyphicon-repeat:before{content:"\e030"}.glyphicon-refresh:before{content:"\e031"}.glyphicon-list-alt:before{content:"\e032"}.glyphicon-lock:before{content:"\e033"}.glyphicon-flag:before{content:"\e034"}.glyphicon-headphones:before{content:"\e035"}.glyphicon-volume-off:before{content:"\e036"}.glyphicon-volume-down:before{content:"\e037"}.glyphicon-volume-up:before{content:"\e038"}.glyphicon-qrcode:before{content:"\e039"}.glyphicon-barcode:before{content:"\e040"}.glyphicon-tag:before{content:"\e041"}.glyphicon-tags:before{content:"\e042"}.glyphicon-book:before{content:"\e043"}.glyphicon-bookmark:before{content:"\e044"}.glyphicon-print:before{content:"\e045"}.glyphicon-camera:before{content:"\e046"}.glyphicon-font:before{content:"\e047"}.glyphicon-bold:before{content:"\e048"}.glyphicon-italic:before{content:"\e049"}.glyphicon-text-height:before{content:"\e050"}.glyphicon-text-width:before{content:"\e051"}.glyphicon-align-left:before{content:"\e052"}.glyphicon-align-center:before{content:"\e053"}.glyphicon-align-right:before{content:"\e054"}.glyphicon-align-justify:before{content:"\e055"}.glyphicon-list:before{content:"\e056"}.glyphicon-indent-left:before{content:"\e057"}.glyphicon-indent-right:before{content:"\e058"}.glyphicon-facetime-video:before{content:"\e059"}.glyphicon-picture:before{content:"\e060"}.glyphicon-map-marker:before{content:"\e062"}.glyphicon-adjust:before{content:"\e063"}.glyphicon-tint:before{content:"\e064"}.glyphicon-edit:before{content:"\e065"}.glyphicon-share:before{content:"\e066"}.glyphicon-check:before{content:"\e067"}.glyphicon-move:before{content:"\e068"}.glyphicon-step-backward:before{content:"\e069"}.glyphicon-fast-backward:before{content:"\e070"}.glyphicon-backward:before{content:"\e071"}.glyphicon-play:before{content:"\e072"}.glyphicon-pause:before{content:"\e073"}.glyphicon-stop:before{content:"\e074"}.glyphicon-forward:before{content:"\e075"}.glyphicon-fast-forward:before{content:"\e076"}.glyphicon-step-forward:before{content:"\e077"}.glyphicon-eject:before{content:"\e078"}.glyphicon-chevron-left:before{content:"\e079"}.glyphicon-chevron-right:before{content:"\e080"}.glyphicon-plus-sign:before{content:"\e081"}.glyphicon-minus-sign:before{content:"\e082"}.glyphicon-remove-sign:before{content:"\e083"}.glyphicon-ok-sign:before{content:"\e084"}.glyphicon-question-sign:before{content:"\e085"}.glyphicon-info-sign:before{content:"\e086"}.glyphicon-screenshot:before{content:"\e087"}.glyphicon-remove-circle:before{content:"\e088"}.glyphicon-ok-circle:before{content:"\e089"}.glyphicon-ban-circle:before{content:"\e090"}.glyphicon-arrow-left:before{content:"\e091"}.glyphicon-arrow-right:before{content:"\e092"}.glyphicon-arrow-up:before{content:"\e093"}.glyphicon-arrow-down:before{content:"\e094"}.glyphicon-share-alt:before{content:"\e095"}.glyphicon-resize-full:before{content:"\e096"}.glyphicon-resize-small:before{content:"\e097"}.glyphicon-exclamation-sign:before{content:"\e101"}.glyphicon-gift:before{content:"\e102"}.glyphicon-leaf:before{content:"\e103"}.glyphicon-fire:before{content:"\e104"}.glyphicon-eye-open:before{content:"\e105"}.glyphicon-eye-close:before{content:"\e106"}.glyphicon-warning-sign:before{content:"\e107"}.glyphicon-plane:before{content:"\e108"}.glyphicon-calendar:before{content:"\e109"}.glyphicon-random:before{content:"\e110"}.glyphicon-comment:before{content:"\e111"}.glyphicon-magnet:before{content:"\e112"}.glyphicon-chevron-up:before{content:"\e113"}.glyphicon-chevron-down:before{content:"\e114"}.glyphicon-retweet:before{content:"\e115"}.glyphicon-shopping-cart:before{content:"\e116"}.glyphicon-folder-close:before{content:"\e117"}.glyphicon-folder-open:before{content:"\e118"}.glyphicon-resize-vertical:before{content:"\e119"}.glyphicon-resize-horizontal:before{content:"\e120"}.glyphicon-hdd:before{content:"\e121"}.glyphicon-bullhorn:before{content:"\e122"}.glyphicon-bell:before{content:"\e123"}.glyphicon-certificate:before{content:"\e124"}.glyphicon-thumbs-up:before{content:"\e125"}.glyphicon-thumbs-down:before{content:"\e126"}.glyphicon-hand-right:before{content:"\e127"}.glyphicon-hand-left:before{content:"\e128"}.glyphicon-hand-up:before{content:"\e129"}.glyphicon-hand-down:before{content:"\e130"}.glyphicon-circle-arrow-right:before{content:"\e131"}.glyphicon-circle-arrow-left:before{content:"\e132"}.glyphicon-circle-arrow-up:before{content:"\e133"}.glyphicon-circle-arrow-down:before{content:"\e134"}.glyphicon-globe:before{content:"\e135"}.glyphicon-wrench:before{content:"\e136"}.glyphicon-tasks:before{content:"\e137"}.glyphicon-filter:before{content:"\e138"}.glyphicon-briefcase:before{content:"\e139"}.glyphicon-fullscreen:before{content:"\e140"}.glyphicon-dashboard:before{content:"\e141"}.glyphicon-paperclip:before{content:"\e142"}.glyphicon-heart-empty:before{content:"\e143"}.glyphicon-link:before{content:"\e144"}.glyphicon-phone:before{content:"\e145"}.glyphicon-pushpin:before{content:"\e146"}.glyphicon-usd:before{content:"\e148"}.glyphicon-gbp:before{content:"\e149"}.glyphicon-sort:before{content:"\e150"}.glyphicon-sort-by-alphabet:before{content:"\e151"}.glyphicon-sort-by-alphabet-alt:before{content:"\e152"}.glyphicon-sort-by-order:before{content:"\e153"}.glyphicon-sort-by-order-alt:before{content:"\e154"}.glyphicon-sort-by-attributes:before{content:"\e155"}.glyphicon-sort-by-attributes-alt:before{content:"\e156"}.glyphicon-unchecked:before{content:"\e157"}.glyphicon-expand:before{content:"\e158"}.glyphicon-collapse-down:before{content:"\e159"}.glyphicon-collapse-up:before{content:"\e160"}.glyphicon-log-in:before{content:"\e161"}.glyphicon-flash:before{content:"\e162"}.glyphicon-log-out:before{content:"\e163"}.glyphicon-new-window:before{content:"\e164"}.glyphicon-record:before{content:"\e165"}.glyphicon-save:before{content:"\e166"}.glyphicon-open:before{content:"\e167"}.glyphicon-saved:before{content:"\e168"}.glyphicon-import:before{content:"\e169"}.glyphicon-export:before{content:"\e170"}.glyphicon-send:before{content:"\e171"}.glyphicon-floppy-disk:before{content:"\e172"}.glyphicon-floppy-saved:before{content:"\e173"}.glyphicon-floppy-remove:before{content:"\e174"}.glyphicon-floppy-save:before{content:"\e175"}.glyphicon-floppy-open:before{content:"\e176"}.glyphicon-credit-card:before{content:"\e177"}.glyphicon-transfer:before{content:"\e178"}.glyphicon-cutlery:before{content:"\e179"}.glyphicon-header:before{content:"\e180"}.glyphicon-compressed:before{content:"\e181"}.glyphicon-earphone:before{content:"\e182"}.glyphicon-phone-alt:before{content:"\e183"}.glyphicon-tower:before{content:"\e184"}.glyphicon-stats:before{content:"\e185"}.glyphicon-sd-video:before{content:"\e186"}.glyphicon-hd-video:before{content:"\e187"}.glyphicon-subtitles:before{content:"\e188"}.glyphicon-sound-stereo:before{content:"\e189"}.glyphicon-sound-dolby:before{content:"\e190"}.glyphicon-sound-5-1:before{content:"\e191"}.glyphicon-sound-6-1:before{content:"\e192"}.glyphicon-sound-7-1:before{content:"\e193"}.glyphicon-copyright-mark:before{content:"\e194"}.glyphicon-registration-mark:before{content:"\e195"}.glyphicon-cloud-download:before{content:"\e197"}.glyphicon-cloud-upload:before{content:"\e198"}.glyphicon-tree-conifer:before{content:"\e199"}.glyphicon-tree-deciduous:before{content:"\e200"}.glyphicon-cd:before{content:"\e201"}.glyphicon-save-file:before{content:"\e202"}.glyphicon-open-file:before{content:"\e203"}.glyphicon-level-up:before{content:"\e204"}.glyphicon-copy:before{content:"\e205"}.glyphicon-paste:before{content:"\e206"}.glyphicon-alert:before{content:"\e209"}.glyphicon-equalizer:before{content:"\e210"}.glyphicon-king:before{content:"\e211"}.glyphicon-queen:before{content:"\e212"}.glyphicon-pawn:before{content:"\e213"}.glyphicon-bishop:before{content:"\e214"}.glyphicon-knight:before{content:"\e215"}.glyphicon-baby-formula:before{content:"\e216"}.glyphicon-tent:before{content:"\26fa"}.glyphicon-blackboard:before{content:"\e218"}.glyphicon-bed:before{content:"\e219"}.glyphicon-apple:before{content:"\f8ff"}.glyphicon-erase:before{content:"\e221"}.glyphicon-hourglass:before{content:"\231b"}.glyphicon-lamp:before{content:"\e223"}.glyphicon-duplicate:before{content:"\e224"}.glyphicon-piggy-bank:before{content:"\e225"}.glyphicon-scissors:before{content:"\e226"}.glyphicon-bitcoin:before{content:"\e227"}.glyphicon-btc:before{content:"\e227"}.glyphicon-xbt:before{content:"\e227"}.glyphicon-yen:before{content:"\00a5"}.glyphicon-jpy:before{content:"\00a5"}.glyphicon-ruble:before{content:"\20bd"}.glyphicon-rub:before{content:"\20bd"}.glyphicon-scale:before{content:"\e230"}.glyphicon-ice-lolly:before{content:"\e231"}.glyphicon-ice-lolly-tasted:before{content:"\e232"}.glyphicon-education:before{content:"\e233"}.glyphicon-option-horizontal:before{content:"\e234"}.glyphicon-option-vertical:before{content:"\e235"}.glyphicon-menu-hamburger:before{content:"\e236"}.glyphicon-modal-window:before{content:"\e237"}.glyphicon-oil:before{content:"\e238"}.glyphicon-grain:before{content:"\e239"}.glyphicon-sunglasses:before{content:"\e240"}.glyphicon-text-size:before{content:"\e241"}.glyphicon-text-color:before{content:"\e242"}.glyphicon-text-background:before{content:"\e243"}.glyphicon-object-align-top:before{content:"\e244"}.glyphicon-object-align-bottom:before{content:"\e245"}.glyphicon-object-align-horizontal:before{content:"\e246"}.glyphicon-object-align-left:before{content:"\e247"}.glyphicon-object-align-vertical:before{content:"\e248"}.glyphicon-object-align-right:before{content:"\e249"}.glyphicon-triangle-right:before{content:"\e250"}.glyphicon-triangle-left:before{content:"\e251"}.glyphicon-triangle-bottom:before{content:"\e252"}.glyphicon-triangle-top:before{content:"\e253"}.glyphicon-console:before{content:"\e254"}.glyphicon-superscript:before{content:"\e255"}.glyphicon-subscript:before{content:"\e256"}.glyphicon-menu-left:before{content:"\e257"}.glyphicon-menu-right:before{content:"\e258"}.glyphicon-menu-down:before{content:"\e259"}.glyphicon-menu-up:before{content:"\e260"}*{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}:after,:before{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}html{font-size:10px;-webkit-tap-highlight-color:rgba(0,0,0,0)}body{font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-size:14px;line-height:1.42857143;color:#333;background-color:#fff}button,input,select,textarea{font-family:inherit;font-size:inherit;line-height:inherit}a{color:#337ab7;text-decoration:none}a:focus,a:hover{color:#23527c;text-decoration:underline}a:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}figure{margin:0}img{vertical-align:middle}.carousel-inner>.item>a>img,.carousel-inner>.item>img,.img-responsive,.thumbnail a>img,.thumbnail>img{display:block;max-width:100%;height:auto}.img-rounded{border-radius:6px}.img-thumbnail{display:inline-block;max-width:100%;height:auto;padding:4px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:all .2s ease-in-out;-o-transition:all .2s ease-in-out;transition:all .2s ease-in-out}.img-circle{border-radius:50%}hr{margin-top:20px;margin-bottom:20px;border:0;border-top:1px solid #eee}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);border:0}.sr-only-focusable:active,.sr-only-focusable:focus{position:static;width:auto;height:auto;margin:0;overflow:visible;clip:auto}[role=button]{cursor:pointer}.h1,.h2,.h3,.h4,.h5,.h6,h1,h2,h3,h4,h5,h6{font-family:inherit;font-weight:500;line-height:1.1;color:inherit}.h1 .small,.h1 small,.h2 .small,.h2 small,.h3 .small,.h3 small,.h4 .small,.h4 small,.h5 .small,.h5 small,.h6 .small,.h6 small,h1 .small,h1 small,h2 .small,h2 small,h3 .small,h3 small,h4 .small,h4 small,h5 .small,h5 small,h6 .small,h6 small{font-weight:400;line-height:1;color:#777}.h1,.h2,.h3,h1,h2,h3{margin-top:20px;margin-bottom:10px}.h1 .small,.h1 small,.h2 .small,.h2 small,.h3 .small,.h3 small,h1 .small,h1 small,h2 .small,h2 small,h3 .small,h3 small{font-size:65%}.h4,.h5,.h6,h4,h5,h6{margin-top:10px;margin-bottom:10px}.h4 .small,.h4 small,.h5 .small,.h5 small,.h6 .small,.h6 small,h4 .small,h4 small,h5 .small,h5 small,h6 .small,h6 small{font-size:75%}.h1,h1{font-size:36px}.h2,h2{font-size:30px}.h3,h3{font-size:24px}.h4,h4{font-size:18px}.h5,h5{font-size:14px}.h6,h6{font-size:12px}p{margin:0 0 10px}.lead{margin-bottom:20px;font-size:16px;font-weight:300;line-height:1.4}@media (min-width:768px){.lead{font-size:21px}}.small,small{font-size:85%}.mark,mark{padding:.2em;background-color:#fcf8e3}.text-left{text-align:left}.text-right{text-align:right}.text-center{text-align:center}.text-justify{text-align:justify}.text-nowrap{white-space:nowrap}.text-lowercase{text-transform:lowercase}.text-uppercase{text-transform:uppercase}.text-capitalize{text-transform:capitalize}.text-muted{color:#777}.text-primary{color:#337ab7}a.text-primary:focus,a.text-primary:hover{color:#286090}.text-success{color:#3c763d}a.text-success:focus,a.text-success:hover{color:#2b542c}.text-info{color:#31708f}a.text-info:focus,a.text-info:hover{color:#245269}.text-warning{color:#8a6d3b}a.text-warning:focus,a.text-warning:hover{color:#66512c}.text-danger{color:#a94442}a.text-danger:focus,a.text-danger:hover{color:#843534}.bg-primary{color:#fff;background-color:#337ab7}a.bg-primary:focus,a.bg-primary:hover{background-color:#286090}.bg-success{background-color:#dff0d8}a.bg-success:focus,a.bg-success:hover{background-color:#c1e2b3}.bg-info{background-color:#d9edf7}a.bg-info:focus,a.bg-info:hover{background-color:#afd9ee}.bg-warning{background-color:#fcf8e3}a.bg-warning:focus,a.bg-warning:hover{background-color:#f7ecb5}.bg-danger{background-color:#f2dede}a.bg-danger:focus,a.bg-danger:hover{background-color:#e4b9b9}.page-header{padding-bottom:9px;margin:40px 0 20px;border-bottom:1px solid #eee}ol,ul{margin-top:0;margin-bottom:10px}ol ol,ol ul,ul ol,ul ul{margin-bottom:0}.list-unstyled{padding-left:0;list-style:none}.list-inline{padding-left:0;margin-left:-5px;list-style:none}.list-inline>li{display:inline-block;padding-right:5px;padding-left:5px}dl{margin-top:0;margin-bottom:20px}dd,dt{line-height:1.42857143}dt{font-weight:700}dd{margin-left:0}@media (min-width:768px){.dl-horizontal dt{float:left;width:160px;overflow:hidden;clear:left;text-align:right;text-overflow:ellipsis;white-space:nowrap}.dl-horizontal dd{margin-left:180px}}abbr[data-original-title],abbr[title]{cursor:help;border-bottom:1px dotted #777}.initialism{font-size:90%;text-transform:uppercase}blockquote{padding:10px 20px;margin:0 0 20px;font-size:17.5px;border-left:5px solid #eee}blockquote ol:last-child,blockquote p:last-child,blockquote ul:last-child{margin-bottom:0}blockquote .small,blockquote footer,blockquote small{display:block;font-size:80%;line-height:1.42857143;color:#777}blockquote .small:before,blockquote footer:before,blockquote small:before{content:'\2014 \00A0'}.blockquote-reverse,blockquote.pull-right{padding-right:15px;padding-left:0;text-align:right;border-right:5px solid #eee;border-left:0}.blockquote-reverse .small:before,.blockquote-reverse footer:before,.blockquote-reverse small:before,blockquote.pull-right .small:before,blockquote.pull-right footer:before,blockquote.pull-right small:before{content:''}.blockquote-reverse .small:after,.blockquote-reverse footer:after,.blockquote-reverse small:after,blockquote.pull-right .small:after,blockquote.pull-right footer:after,blockquote.pull-right small:after{content:'\00A0 \2014'}address{margin-bottom:20px;font-style:normal;line-height:1.42857143}code,kbd,pre,samp{font-family:Menlo,Monaco,Consolas,"Courier New",monospace}code{padding:2px 4px;font-size:90%;color:#c7254e;background-color:#f9f2f4;border-radius:4px}kbd{padding:2px 4px;font-size:90%;color:#fff;background-color:#333;border-radius:3px;-webkit-box-shadow:inset 0 -1px 0 rgba(0,0,0,.25);box-shadow:inset 0 -1px 0 rgba(0,0,0,.25)}kbd kbd{padding:0;font-size:100%;font-weight:700;-webkit-box-shadow:none;box-shadow:none}pre{display:block;padding:9.5px;margin:0 0 10px;font-size:13px;line-height:1.42857143;color:#333;word-break:break-all;word-wrap:break-word;background-color:#f5f5f5;border:1px solid #ccc;border-radius:4px}pre code{padding:0;font-size:inherit;color:inherit;white-space:pre-wrap;background-color:transparent;border-radius:0}.pre-scrollable{max-height:340px;overflow-y:scroll}.container{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}@media (min-width:768px){.container{width:750px}}@media (min-width:992px){.container{width:970px}}@media (min-width:1200px){.container{width:1170px}}.container-fluid{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}.row{margin-right:-15px;margin-left:-15px}.col-lg-1,.col-lg-10,.col-lg-11,.col-lg-12,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9,.col-md-1,.col-md-10,.col-md-11,.col-md-12,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9,.col-sm-1,.col-sm-10,.col-sm-11,.col-sm-12,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9,.col-xs-1,.col-xs-10,.col-xs-11,.col-xs-12,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9{position:relative;min-height:1px;padding-right:15px;padding-left:15px}.col-xs-1,.col-xs-10,.col-xs-11,.col-xs-12,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9{float:left}.col-xs-12{width:100%}.col-xs-11{width:91.66666667%}.col-xs-10{width:83.33333333%}.col-xs-9{width:75%}.col-xs-8{width:66.66666667%}.col-xs-7{width:58.33333333%}.col-xs-6{width:50%}.col-xs-5{width:41.66666667%}.col-xs-4{width:33.33333333%}.col-xs-3{width:25%}.col-xs-2{width:16.66666667%}.col-xs-1{width:8.33333333%}.col-xs-pull-12{right:100%}.col-xs-pull-11{right:91.66666667%}.col-xs-pull-10{right:83.33333333%}.col-xs-pull-9{right:75%}.col-xs-pull-8{right:66.66666667%}.col-xs-pull-7{right:58.33333333%}.col-xs-pull-6{right:50%}.col-xs-pull-5{right:41.66666667%}.col-xs-pull-4{right:33.33333333%}.col-xs-pull-3{right:25%}.col-xs-pull-2{right:16.66666667%}.col-xs-pull-1{right:8.33333333%}.col-xs-pull-0{right:auto}.col-xs-push-12{left:100%}.col-xs-push-11{left:91.66666667%}.col-xs-push-10{left:83.33333333%}.col-xs-push-9{left:75%}.col-xs-push-8{left:66.66666667%}.col-xs-push-7{left:58.33333333%}.col-xs-push-6{left:50%}.col-xs-push-5{left:41.66666667%}.col-xs-push-4{left:33.33333333%}.col-xs-push-3{left:25%}.col-xs-push-2{left:16.66666667%}.col-xs-push-1{left:8.33333333%}.col-xs-push-0{left:auto}.col-xs-offset-12{margin-left:100%}.col-xs-offset-11{margin-left:91.66666667%}.col-xs-offset-10{margin-left:83.33333333%}.col-xs-offset-9{margin-left:75%}.col-xs-offset-8{margin-left:66.66666667%}.col-xs-offset-7{margin-left:58.33333333%}.col-xs-offset-6{margin-left:50%}.col-xs-offset-5{margin-left:41.66666667%}.col-xs-offset-4{margin-left:33.33333333%}.col-xs-offset-3{margin-left:25%}.col-xs-offset-2{margin-left:16.66666667%}.col-xs-offset-1{margin-left:8.33333333%}.col-xs-offset-0{margin-left:0}@media (min-width:768px){.col-sm-1,.col-sm-10,.col-sm-11,.col-sm-12,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9{float:left}.col-sm-12{width:100%}.col-sm-11{width:91.66666667%}.col-sm-10{width:83.33333333%}.col-sm-9{width:75%}.col-sm-8{width:66.66666667%}.col-sm-7{width:58.33333333%}.col-sm-6{width:50%}.col-sm-5{width:41.66666667%}.col-sm-4{width:33.33333333%}.col-sm-3{width:25%}.col-sm-2{width:16.66666667%}.col-sm-1{width:8.33333333%}.col-sm-pull-12{right:100%}.col-sm-pull-11{right:91.66666667%}.col-sm-pull-10{right:83.33333333%}.col-sm-pull-9{right:75%}.col-sm-pull-8{right:66.66666667%}.col-sm-pull-7{right:58.33333333%}.col-sm-pull-6{right:50%}.col-sm-pull-5{right:41.66666667%}.col-sm-pull-4{right:33.33333333%}.col-sm-pull-3{right:25%}.col-sm-pull-2{right:16.66666667%}.col-sm-pull-1{right:8.33333333%}.col-sm-pull-0{right:auto}.col-sm-push-12{left:100%}.col-sm-push-11{left:91.66666667%}.col-sm-push-10{left:83.33333333%}.col-sm-push-9{left:75%}.col-sm-push-8{left:66.66666667%}.col-sm-push-7{left:58.33333333%}.col-sm-push-6{left:50%}.col-sm-push-5{left:41.66666667%}.col-sm-push-4{left:33.33333333%}.col-sm-push-3{left:25%}.col-sm-push-2{left:16.66666667%}.col-sm-push-1{left:8.33333333%}.col-sm-push-0{left:auto}.col-sm-offset-12{margin-left:100%}.col-sm-offset-11{margin-left:91.66666667%}.col-sm-offset-10{margin-left:83.33333333%}.col-sm-offset-9{margin-left:75%}.col-sm-offset-8{margin-left:66.66666667%}.col-sm-offset-7{margin-left:58.33333333%}.col-sm-offset-6{margin-left:50%}.col-sm-offset-5{margin-left:41.66666667%}.col-sm-offset-4{margin-left:33.33333333%}.col-sm-offset-3{margin-left:25%}.col-sm-offset-2{margin-left:16.66666667%}.col-sm-offset-1{margin-left:8.33333333%}.col-sm-offset-0{margin-left:0}}@media (min-width:992px){.col-md-1,.col-md-10,.col-md-11,.col-md-12,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9{float:left}.col-md-12{width:100%}.col-md-11{width:91.66666667%}.col-md-10{width:83.33333333%}.col-md-9{width:75%}.col-md-8{width:66.66666667%}.col-md-7{width:58.33333333%}.col-md-6{width:50%}.col-md-5{width:41.66666667%}.col-md-4{width:33.33333333%}.col-md-3{width:25%}.col-md-2{width:16.66666667%}.col-md-1{width:8.33333333%}.col-md-pull-12{right:100%}.col-md-pull-11{right:91.66666667%}.col-md-pull-10{right:83.33333333%}.col-md-pull-9{right:75%}.col-md-pull-8{right:66.66666667%}.col-md-pull-7{right:58.33333333%}.col-md-pull-6{right:50%}.col-md-pull-5{right:41.66666667%}.col-md-pull-4{right:33.33333333%}.col-md-pull-3{right:25%}.col-md-pull-2{right:16.66666667%}.col-md-pull-1{right:8.33333333%}.col-md-pull-0{right:auto}.col-md-push-12{left:100%}.col-md-push-11{left:91.66666667%}.col-md-push-10{left:83.33333333%}.col-md-push-9{left:75%}.col-md-push-8{left:66.66666667%}.col-md-push-7{left:58.33333333%}.col-md-push-6{left:50%}.col-md-push-5{left:41.66666667%}.col-md-push-4{left:33.33333333%}.col-md-push-3{left:25%}.col-md-push-2{left:16.66666667%}.col-md-push-1{left:8.33333333%}.col-md-push-0{left:auto}.col-md-offset-12{margin-left:100%}.col-md-offset-11{margin-left:91.66666667%}.col-md-offset-10{margin-left:83.33333333%}.col-md-offset-9{margin-left:75%}.col-md-offset-8{margin-left:66.66666667%}.col-md-offset-7{margin-left:58.33333333%}.col-md-offset-6{margin-left:50%}.col-md-offset-5{margin-left:41.66666667%}.col-md-offset-4{margin-left:33.33333333%}.col-md-offset-3{margin-left:25%}.col-md-offset-2{margin-left:16.66666667%}.col-md-offset-1{margin-left:8.33333333%}.col-md-offset-0{margin-left:0}}@media (min-width:1200px){.col-lg-1,.col-lg-10,.col-lg-11,.col-lg-12,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9{float:left}.col-lg-12{width:100%}.col-lg-11{width:91.66666667%}.col-lg-10{width:83.33333333%}.col-lg-9{width:75%}.col-lg-8{width:66.66666667%}.col-lg-7{width:58.33333333%}.col-lg-6{width:50%}.col-lg-5{width:41.66666667%}.col-lg-4{width:33.33333333%}.col-lg-3{width:25%}.col-lg-2{width:16.66666667%}.col-lg-1{width:8.33333333%}.col-lg-pull-12{right:100%}.col-lg-pull-11{right:91.66666667%}.col-lg-pull-10{right:83.33333333%}.col-lg-pull-9{right:75%}.col-lg-pull-8{right:66.66666667%}.col-lg-pull-7{right:58.33333333%}.col-lg-pull-6{right:50%}.col-lg-pull-5{right:41.66666667%}.col-lg-pull-4{right:33.33333333%}.col-lg-pull-3{right:25%}.col-lg-pull-2{right:16.66666667%}.col-lg-pull-1{right:8.33333333%}.col-lg-pull-0{right:auto}.col-lg-push-12{left:100%}.col-lg-push-11{left:91.66666667%}.col-lg-push-10{left:83.33333333%}.col-lg-push-9{left:75%}.col-lg-push-8{left:66.66666667%}.col-lg-push-7{left:58.33333333%}.col-lg-push-6{left:50%}.col-lg-push-5{left:41.66666667%}.col-lg-push-4{left:33.33333333%}.col-lg-push-3{left:25%}.col-lg-push-2{left:16.66666667%}.col-lg-push-1{left:8.33333333%}.col-lg-push-0{left:auto}.col-lg-offset-12{margin-left:100%}.col-lg-offset-11{margin-left:91.66666667%}.col-lg-offset-10{margin-left:83.33333333%}.col-lg-offset-9{margin-left:75%}.col-lg-offset-8{margin-left:66.66666667%}.col-lg-offset-7{margin-left:58.33333333%}.col-lg-offset-6{margin-left:50%}.col-lg-offset-5{margin-left:41.66666667%}.col-lg-offset-4{margin-left:33.33333333%}.col-lg-offset-3{margin-left:25%}.col-lg-offset-2{margin-left:16.66666667%}.col-lg-offset-1{margin-left:8.33333333%}.col-lg-offset-0{margin-left:0}}table{background-color:transparent}caption{padding-top:8px;padding-bottom:8px;color:#777;text-align:left}th{text-align:left}.table{width:100%;max-width:100%;margin-bottom:20px}.table>tbody>tr>td,.table>tbody>tr>th,.table>tfoot>tr>td,.table>tfoot>tr>th,.table>thead>tr>td,.table>thead>tr>th{padding:8px;line-height:1.42857143;vertical-align:top;border-top:1px solid #ddd}.table>thead>tr>th{vertical-align:bottom;border-bottom:2px solid #ddd}.table>caption+thead>tr:first-child>td,.table>caption+thead>tr:first-child>th,.table>colgroup+thead>tr:first-child>td,.table>colgroup+thead>tr:first-child>th,.table>thead:first-child>tr:first-child>td,.table>thead:first-child>tr:first-child>th{border-top:0}.table>tbody+tbody{border-top:2px solid #ddd}.table .table{background-color:#fff}.table-condensed>tbody>tr>td,.table-condensed>tbody>tr>th,.table-condensed>tfoot>tr>td,.table-condensed>tfoot>tr>th,.table-condensed>thead>tr>td,.table-condensed>thead>tr>th{padding:5px}.table-bordered{border:1px solid #ddd}.table-bordered>tbody>tr>td,.table-bordered>tbody>tr>th,.table-bordered>tfoot>tr>td,.table-bordered>tfoot>tr>th,.table-bordered>thead>tr>td,.table-bordered>thead>tr>th{border:1px solid #ddd}.table-bordered>thead>tr>td,.table-bordered>thead>tr>th{border-bottom-width:2px}.table-striped>tbody>tr:nth-of-type(odd){background-color:#f9f9f9}.table-hover>tbody>tr:hover{background-color:#f5f5f5}table col[class*=col-]{position:static;display:table-column;float:none}table td[class*=col-],table th[class*=col-]{position:static;display:table-cell;float:none}.table>tbody>tr.active>td,.table>tbody>tr.active>th,.table>tbody>tr>td.active,.table>tbody>tr>th.active,.table>tfoot>tr.active>td,.table>tfoot>tr.active>th,.table>tfoot>tr>td.active,.table>tfoot>tr>th.active,.table>thead>tr.active>td,.table>thead>tr.active>th,.table>thead>tr>td.active,.table>thead>tr>th.active{background-color:#f5f5f5}.table-hover>tbody>tr.active:hover>td,.table-hover>tbody>tr.active:hover>th,.table-hover>tbody>tr:hover>.active,.table-hover>tbody>tr>td.active:hover,.table-hover>tbody>tr>th.active:hover{background-color:#e8e8e8}.table>tbody>tr.success>td,.table>tbody>tr.success>th,.table>tbody>tr>td.success,.table>tbody>tr>th.success,.table>tfoot>tr.success>td,.table>tfoot>tr.success>th,.table>tfoot>tr>td.success,.table>tfoot>tr>th.success,.table>thead>tr.success>td,.table>thead>tr.success>th,.table>thead>tr>td.success,.table>thead>tr>th.success{background-color:#dff0d8}.table-hover>tbody>tr.success:hover>td,.table-hover>tbody>tr.success:hover>th,.table-hover>tbody>tr:hover>.success,.table-hover>tbody>tr>td.success:hover,.table-hover>tbody>tr>th.success:hover{background-color:#d0e9c6}.table>tbody>tr.info>td,.table>tbody>tr.info>th,.table>tbody>tr>td.info,.table>tbody>tr>th.info,.table>tfoot>tr.info>td,.table>tfoot>tr.info>th,.table>tfoot>tr>td.info,.table>tfoot>tr>th.info,.table>thead>tr.info>td,.table>thead>tr.info>th,.table>thead>tr>td.info,.table>thead>tr>th.info{background-color:#d9edf7}.table-hover>tbody>tr.info:hover>td,.table-hover>tbody>tr.info:hover>th,.table-hover>tbody>tr:hover>.info,.table-hover>tbody>tr>td.info:hover,.table-hover>tbody>tr>th.info:hover{background-color:#c4e3f3}.table>tbody>tr.warning>td,.table>tbody>tr.warning>th,.table>tbody>tr>td.warning,.table>tbody>tr>th.warning,.table>tfoot>tr.warning>td,.table>tfoot>tr.warning>th,.table>tfoot>tr>td.warning,.table>tfoot>tr>th.warning,.table>thead>tr.warning>td,.table>thead>tr.warning>th,.table>thead>tr>td.warning,.table>thead>tr>th.warning{background-color:#fcf8e3}.table-hover>tbody>tr.warning:hover>td,.table-hover>tbody>tr.warning:hover>th,.table-hover>tbody>tr:hover>.warning,.table-hover>tbody>tr>td.warning:hover,.table-hover>tbody>tr>th.warning:hover{background-color:#faf2cc}.table>tbody>tr.danger>td,.table>tbody>tr.danger>th,.table>tbody>tr>td.danger,.table>tbody>tr>th.danger,.table>tfoot>tr.danger>td,.table>tfoot>tr.danger>th,.table>tfoot>tr>td.danger,.table>tfoot>tr>th.danger,.table>thead>tr.danger>td,.table>thead>tr.danger>th,.table>thead>tr>td.danger,.table>thead>tr>th.danger{background-color:#f2dede}.table-hover>tbody>tr.danger:hover>td,.table-hover>tbody>tr.danger:hover>th,.table-hover>tbody>tr:hover>.danger,.table-hover>tbody>tr>td.danger:hover,.table-hover>tbody>tr>th.danger:hover{background-color:#ebcccc}.table-responsive{min-height:.01%;overflow-x:auto}@media screen and (max-width:767px){.table-responsive{width:100%;margin-bottom:15px;overflow-y:hidden;-ms-overflow-style:-ms-autohiding-scrollbar;border:1px solid #ddd}.table-responsive>.table{margin-bottom:0}.table-responsive>.table>tbody>tr>td,.table-responsive>.table>tbody>tr>th,.table-responsive>.table>tfoot>tr>td,.table-responsive>.table>tfoot>tr>th,.table-responsive>.table>thead>tr>td,.table-responsive>.table>thead>tr>th{white-space:nowrap}.table-responsive>.table-bordered{border:0}.table-responsive>.table-bordered>tbody>tr>td:first-child,.table-responsive>.table-bordered>tbody>tr>th:first-child,.table-responsive>.table-bordered>tfoot>tr>td:first-child,.table-responsive>.table-bordered>tfoot>tr>th:first-child,.table-responsive>.table-bordered>thead>tr>td:first-child,.table-responsive>.table-bordered>thead>tr>th:first-child{border-left:0}.table-responsive>.table-bordered>tbody>tr>td:last-child,.table-responsive>.table-bordered>tbody>tr>th:last-child,.table-responsive>.table-bordered>tfoot>tr>td:last-child,.table-responsive>.table-bordered>tfoot>tr>th:last-child,.table-responsive>.table-bordered>thead>tr>td:last-child,.table-responsive>.table-bordered>thead>tr>th:last-child{border-right:0}.table-responsive>.table-bordered>tbody>tr:last-child>td,.table-responsive>.table-bordered>tbody>tr:last-child>th,.table-responsive>.table-bordered>tfoot>tr:last-child>td,.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}}fieldset{min-width:0;padding:0;margin:0;border:0}legend{display:block;width:100%;padding:0;margin-bottom:20px;font-size:21px;line-height:inherit;color:#333;border:0;border-bottom:1px solid #e5e5e5}label{display:inline-block;max-width:100%;margin-bottom:5px;font-weight:700}input[type=search]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}input[type=checkbox],input[type=radio]{margin:4px 0 0;margin-top:1px\9;line-height:normal}input[type=file]{display:block}input[type=range]{display:block;width:100%}select[multiple],select[size]{height:auto}input[type=file]:focus,input[type=checkbox]:focus,input[type=radio]:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}output{display:block;padding-top:7px;font-size:14px;line-height:1.42857143;color:#555}.form-control{display:block;width:100%;height:34px;padding:6px 12px;font-size:14px;line-height:1.42857143;color:#555;background-color:#fff;background-image:none;border:1px solid #ccc;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075);-webkit-transition:border-color ease-in-out .15s,-webkit-box-shadow ease-in-out .15s;-o-transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s}.form-control:focus{border-color:#66afe9;outline:0;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6);box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6)}.form-control::-moz-placeholder{color:#999;opacity:1}.form-control:-ms-input-placeholder{color:#999}.form-control::-webkit-input-placeholder{color:#999}.form-control::-ms-expand{background-color:transparent;border:0}.form-control[disabled],.form-control[readonly],fieldset[disabled] .form-control{background-color:#eee;opacity:1}.form-control[disabled],fieldset[disabled] .form-control{cursor:not-allowed}textarea.form-control{height:auto}input[type=search]{-webkit-appearance:none}@media screen and (-webkit-min-device-pixel-ratio:0){input[type=date].form-control,input[type=time].form-control,input[type=datetime-local].form-control,input[type=month].form-control{line-height:34px}.input-group-sm input[type=date],.input-group-sm input[type=time],.input-group-sm input[type=datetime-local],.input-group-sm input[type=month],input[type=date].input-sm,input[type=time].input-sm,input[type=datetime-local].input-sm,input[type=month].input-sm{line-height:30px}.input-group-lg input[type=date],.input-group-lg input[type=time],.input-group-lg input[type=datetime-local],.input-group-lg input[type=month],input[type=date].input-lg,input[type=time].input-lg,input[type=datetime-local].input-lg,input[type=month].input-lg{line-height:46px}}.form-group{margin-bottom:15px}.checkbox,.radio{position:relative;display:block;margin-top:10px;margin-bottom:10px}.checkbox label,.radio label{min-height:20px;padding-left:20px;margin-bottom:0;font-weight:400;cursor:pointer}.checkbox input[type=checkbox],.checkbox-inline input[type=checkbox],.radio input[type=radio],.radio-inline input[type=radio]{position:absolute;margin-top:4px\9;margin-left:-20px}.checkbox+.checkbox,.radio+.radio{margin-top:-5px}.checkbox-inline,.radio-inline{position:relative;display:inline-block;padding-left:20px;margin-bottom:0;font-weight:400;vertical-align:middle;cursor:pointer}.checkbox-inline+.checkbox-inline,.radio-inline+.radio-inline{margin-top:0;margin-left:10px}fieldset[disabled] input[type=checkbox],fieldset[disabled] input[type=radio],input[type=checkbox].disabled,input[type=checkbox][disabled],input[type=radio].disabled,input[type=radio][disabled]{cursor:not-allowed}.checkbox-inline.disabled,.radio-inline.disabled,fieldset[disabled] .checkbox-inline,fieldset[disabled] .radio-inline{cursor:not-allowed}.checkbox.disabled label,.radio.disabled label,fieldset[disabled] .checkbox label,fieldset[disabled] .radio label{cursor:not-allowed}.form-control-static{min-height:34px;padding-top:7px;padding-bottom:7px;margin-bottom:0}.form-control-static.input-lg,.form-control-static.input-sm{padding-right:0;padding-left:0}.input-sm{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-sm{height:30px;line-height:30px}select[multiple].input-sm,textarea.input-sm{height:auto}.form-group-sm .form-control{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.form-group-sm select.form-control{height:30px;line-height:30px}.form-group-sm select[multiple].form-control,.form-group-sm textarea.form-control{height:auto}.form-group-sm .form-control-static{height:30px;min-height:32px;padding:6px 10px;font-size:12px;line-height:1.5}.input-lg{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}select.input-lg{height:46px;line-height:46px}select[multiple].input-lg,textarea.input-lg{height:auto}.form-group-lg .form-control{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}.form-group-lg select.form-control{height:46px;line-height:46px}.form-group-lg select[multiple].form-control,.form-group-lg textarea.form-control{height:auto}.form-group-lg .form-control-static{height:46px;min-height:38px;padding:11px 16px;font-size:18px;line-height:1.3333333}.has-feedback{position:relative}.has-feedback .form-control{padding-right:42.5px}.form-control-feedback{position:absolute;top:0;right:0;z-index:2;display:block;width:34px;height:34px;line-height:34px;text-align:center;pointer-events:none}.form-group-lg .form-control+.form-control-feedback,.input-group-lg+.form-control-feedback,.input-lg+.form-control-feedback{width:46px;height:46px;line-height:46px}.form-group-sm .form-control+.form-control-feedback,.input-group-sm+.form-control-feedback,.input-sm+.form-control-feedback{width:30px;height:30px;line-height:30px}.has-success .checkbox,.has-success .checkbox-inline,.has-success .control-label,.has-success .help-block,.has-success .radio,.has-success .radio-inline,.has-success.checkbox label,.has-success.checkbox-inline label,.has-success.radio label,.has-success.radio-inline label{color:#3c763d}.has-success .form-control{border-color:#3c763d;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-success .form-control:focus{border-color:#2b542c;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #67b168;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #67b168}.has-success .input-group-addon{color:#3c763d;background-color:#dff0d8;border-color:#3c763d}.has-success .form-control-feedback{color:#3c763d}.has-warning .checkbox,.has-warning .checkbox-inline,.has-warning .control-label,.has-warning .help-block,.has-warning .radio,.has-warning .radio-inline,.has-warning.checkbox label,.has-warning.checkbox-inline label,.has-warning.radio label,.has-warning.radio-inline label{color:#8a6d3b}.has-warning .form-control{border-color:#8a6d3b;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-warning .form-control:focus{border-color:#66512c;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #c0a16b;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #c0a16b}.has-warning .input-group-addon{color:#8a6d3b;background-color:#fcf8e3;border-color:#8a6d3b}.has-warning .form-control-feedback{color:#8a6d3b}.has-error .checkbox,.has-error .checkbox-inline,.has-error .control-label,.has-error .help-block,.has-error .radio,.has-error .radio-inline,.has-error.checkbox label,.has-error.checkbox-inline label,.has-error.radio label,.has-error.radio-inline label{color:#a94442}.has-error .form-control{border-color:#a94442;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-error .form-control:focus{border-color:#843534;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #ce8483;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #ce8483}.has-error .input-group-addon{color:#a94442;background-color:#f2dede;border-color:#a94442}.has-error .form-control-feedback{color:#a94442}.has-feedback label~.form-control-feedback{top:25px}.has-feedback label.sr-only~.form-control-feedback{top:0}.help-block{display:block;margin-top:5px;margin-bottom:10px;color:#737373}@media (min-width:768px){.form-inline .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.form-inline .form-control{display:inline-block;width:auto;vertical-align:middle}.form-inline .form-control-static{display:inline-block}.form-inline .input-group{display:inline-table;vertical-align:middle}.form-inline .input-group .form-control,.form-inline .input-group .input-group-addon,.form-inline .input-group .input-group-btn{width:auto}.form-inline .input-group>.form-control{width:100%}.form-inline .control-label{margin-bottom:0;vertical-align:middle}.form-inline .checkbox,.form-inline .radio{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.form-inline .checkbox label,.form-inline .radio label{padding-left:0}.form-inline .checkbox input[type=checkbox],.form-inline .radio input[type=radio]{position:relative;margin-left:0}.form-inline .has-feedback .form-control-feedback{top:0}}.form-horizontal .checkbox,.form-horizontal .checkbox-inline,.form-horizontal .radio,.form-horizontal .radio-inline{padding-top:7px;margin-top:0;margin-bottom:0}.form-horizontal .checkbox,.form-horizontal .radio{min-height:27px}.form-horizontal .form-group{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.form-horizontal .control-label{padding-top:7px;margin-bottom:0;text-align:right}}.form-horizontal .has-feedback .form-control-feedback{right:15px}@media (min-width:768px){.form-horizontal .form-group-lg .control-label{padding-top:11px;font-size:18px}}@media (min-width:768px){.form-horizontal .form-group-sm .control-label{padding-top:6px;font-size:12px}}.btn{display:inline-block;padding:6px 12px;margin-bottom:0;font-size:14px;font-weight:400;line-height:1.42857143;text-align:center;white-space:nowrap;vertical-align:middle;-ms-touch-action:manipulation;touch-action:manipulation;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;background-image:none;border:1px solid transparent;border-radius:4px}.btn.active.focus,.btn.active:focus,.btn.focus,.btn:active.focus,.btn:active:focus,.btn:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}.btn.focus,.btn:focus,.btn:hover{color:#333;text-decoration:none}.btn.active,.btn:active{background-image:none;outline:0;-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn.disabled,.btn[disabled],fieldset[disabled] .btn{cursor:not-allowed;filter:alpha(opacity=65);-webkit-box-shadow:none;box-shadow:none;opacity:.65}a.btn.disabled,fieldset[disabled] a.btn{pointer-events:none}.btn-default{color:#333;background-color:#fff;border-color:#ccc}.btn-default.focus,.btn-default:focus{color:#333;background-color:#e6e6e6;border-color:#8c8c8c}.btn-default:hover{color:#333;background-color:#e6e6e6;border-color:#adadad}.btn-default.active,.btn-default:active,.open>.dropdown-toggle.btn-default{color:#333;background-color:#e6e6e6;border-color:#adadad}.btn-default.active.focus,.btn-default.active:focus,.btn-default.active:hover,.btn-default:active.focus,.btn-default:active:focus,.btn-default:active:hover,.open>.dropdown-toggle.btn-default.focus,.open>.dropdown-toggle.btn-default:focus,.open>.dropdown-toggle.btn-default:hover{color:#333;background-color:#d4d4d4;border-color:#8c8c8c}.btn-default.active,.btn-default:active,.open>.dropdown-toggle.btn-default{background-image:none}.btn-default.disabled.focus,.btn-default.disabled:focus,.btn-default.disabled:hover,.btn-default[disabled].focus,.btn-default[disabled]:focus,.btn-default[disabled]:hover,fieldset[disabled] .btn-default.focus,fieldset[disabled] .btn-default:focus,fieldset[disabled] .btn-default:hover{background-color:#fff;border-color:#ccc}.btn-default .badge{color:#fff;background-color:#333}.btn-primary{color:#fff;background-color:#337ab7;border-color:#2e6da4}.btn-primary.focus,.btn-primary:focus{color:#fff;background-color:#286090;border-color:#122b40}.btn-primary:hover{color:#fff;background-color:#286090;border-color:#204d74}.btn-primary.active,.btn-primary:active,.open>.dropdown-toggle.btn-primary{color:#fff;background-color:#286090;border-color:#204d74}.btn-primary.active.focus,.btn-primary.active:focus,.btn-primary.active:hover,.btn-primary:active.focus,.btn-primary:active:focus,.btn-primary:active:hover,.open>.dropdown-toggle.btn-primary.focus,.open>.dropdown-toggle.btn-primary:focus,.open>.dropdown-toggle.btn-primary:hover{color:#fff;background-color:#204d74;border-color:#122b40}.btn-primary.active,.btn-primary:active,.open>.dropdown-toggle.btn-primary{background-image:none}.btn-primary.disabled.focus,.btn-primary.disabled:focus,.btn-primary.disabled:hover,.btn-primary[disabled].focus,.btn-primary[disabled]:focus,.btn-primary[disabled]:hover,fieldset[disabled] .btn-primary.focus,fieldset[disabled] .btn-primary:focus,fieldset[disabled] .btn-primary:hover{background-color:#337ab7;border-color:#2e6da4}.btn-primary .badge{color:#337ab7;background-color:#fff}.btn-success{color:#fff;background-color:#5cb85c;border-color:#4cae4c}.btn-success.focus,.btn-success:focus{color:#fff;background-color:#449d44;border-color:#255625}.btn-success:hover{color:#fff;background-color:#449d44;border-color:#398439}.btn-success.active,.btn-success:active,.open>.dropdown-toggle.btn-success{color:#fff;background-color:#449d44;border-color:#398439}.btn-success.active.focus,.btn-success.active:focus,.btn-success.active:hover,.btn-success:active.focus,.btn-success:active:focus,.btn-success:active:hover,.open>.dropdown-toggle.btn-success.focus,.open>.dropdown-toggle.btn-success:focus,.open>.dropdown-toggle.btn-success:hover{color:#fff;background-color:#398439;border-color:#255625}.btn-success.active,.btn-success:active,.open>.dropdown-toggle.btn-success{background-image:none}.btn-success.disabled.focus,.btn-success.disabled:focus,.btn-success.disabled:hover,.btn-success[disabled].focus,.btn-success[disabled]:focus,.btn-success[disabled]:hover,fieldset[disabled] .btn-success.focus,fieldset[disabled] .btn-success:focus,fieldset[disabled] .btn-success:hover{background-color:#5cb85c;border-color:#4cae4c}.btn-success .badge{color:#5cb85c;background-color:#fff}.btn-info{color:#fff;background-color:#5bc0de;border-color:#46b8da}.btn-info.focus,.btn-info:focus{color:#fff;background-color:#31b0d5;border-color:#1b6d85}.btn-info:hover{color:#fff;background-color:#31b0d5;border-color:#269abc}.btn-info.active,.btn-info:active,.open>.dropdown-toggle.btn-info{color:#fff;background-color:#31b0d5;border-color:#269abc}.btn-info.active.focus,.btn-info.active:focus,.btn-info.active:hover,.btn-info:active.focus,.btn-info:active:focus,.btn-info:active:hover,.open>.dropdown-toggle.btn-info.focus,.open>.dropdown-toggle.btn-info:focus,.open>.dropdown-toggle.btn-info:hover{color:#fff;background-color:#269abc;border-color:#1b6d85}.btn-info.active,.btn-info:active,.open>.dropdown-toggle.btn-info{background-image:none}.btn-info.disabled.focus,.btn-info.disabled:focus,.btn-info.disabled:hover,.btn-info[disabled].focus,.btn-info[disabled]:focus,.btn-info[disabled]:hover,fieldset[disabled] .btn-info.focus,fieldset[disabled] .btn-info:focus,fieldset[disabled] .btn-info:hover{background-color:#5bc0de;border-color:#46b8da}.btn-info .badge{color:#5bc0de;background-color:#fff}.btn-warning{color:#fff;background-color:#f0ad4e;border-color:#eea236}.btn-warning.focus,.btn-warning:focus{color:#fff;background-color:#ec971f;border-color:#985f0d}.btn-warning:hover{color:#fff;background-color:#ec971f;border-color:#d58512}.btn-warning.active,.btn-warning:active,.open>.dropdown-toggle.btn-warning{color:#fff;background-color:#ec971f;border-color:#d58512}.btn-warning.active.focus,.btn-warning.active:focus,.btn-warning.active:hover,.btn-warning:active.focus,.btn-warning:active:focus,.btn-warning:active:hover,.open>.dropdown-toggle.btn-warning.focus,.open>.dropdown-toggle.btn-warning:focus,.open>.dropdown-toggle.btn-warning:hover{color:#fff;background-color:#d58512;border-color:#985f0d}.btn-warning.active,.btn-warning:active,.open>.dropdown-toggle.btn-warning{background-image:none}.btn-warning.disabled.focus,.btn-warning.disabled:focus,.btn-warning.disabled:hover,.btn-warning[disabled].focus,.btn-warning[disabled]:focus,.btn-warning[disabled]:hover,fieldset[disabled] .btn-warning.focus,fieldset[disabled] .btn-warning:focus,fieldset[disabled] .btn-warning:hover{background-color:#f0ad4e;border-color:#eea236}.btn-warning .badge{color:#f0ad4e;background-color:#fff}.btn-danger{color:#fff;background-color:#d9534f;border-color:#d43f3a}.btn-danger.focus,.btn-danger:focus{color:#fff;background-color:#c9302c;border-color:#761c19}.btn-danger:hover{color:#fff;background-color:#c9302c;border-color:#ac2925}.btn-danger.active,.btn-danger:active,.open>.dropdown-toggle.btn-danger{color:#fff;background-color:#c9302c;border-color:#ac2925}.btn-danger.active.focus,.btn-danger.active:focus,.btn-danger.active:hover,.btn-danger:active.focus,.btn-danger:active:focus,.btn-danger:active:hover,.open>.dropdown-toggle.btn-danger.focus,.open>.dropdown-toggle.btn-danger:focus,.open>.dropdown-toggle.btn-danger:hover{color:#fff;background-color:#ac2925;border-color:#761c19}.btn-danger.active,.btn-danger:active,.open>.dropdown-toggle.btn-danger{background-image:none}.btn-danger.disabled.focus,.btn-danger.disabled:focus,.btn-danger.disabled:hover,.btn-danger[disabled].focus,.btn-danger[disabled]:focus,.btn-danger[disabled]:hover,fieldset[disabled] .btn-danger.focus,fieldset[disabled] .btn-danger:focus,fieldset[disabled] .btn-danger:hover{background-color:#d9534f;border-color:#d43f3a}.btn-danger .badge{color:#d9534f;background-color:#fff}.btn-link{font-weight:400;color:#337ab7;border-radius:0}.btn-link,.btn-link.active,.btn-link:active,.btn-link[disabled],fieldset[disabled] .btn-link{background-color:transparent;-webkit-box-shadow:none;box-shadow:none}.btn-link,.btn-link:active,.btn-link:focus,.btn-link:hover{border-color:transparent}.btn-link:focus,.btn-link:hover{color:#23527c;text-decoration:underline;background-color:transparent}.btn-link[disabled]:focus,.btn-link[disabled]:hover,fieldset[disabled] .btn-link:focus,fieldset[disabled] .btn-link:hover{color:#777;text-decoration:none}.btn-group-lg>.btn,.btn-lg{padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}.btn-group-sm>.btn,.btn-sm{padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.btn-group-xs>.btn,.btn-xs{padding:1px 5px;font-size:12px;line-height:1.5;border-radius:3px}.btn-block{display:block;width:100%}.btn-block+.btn-block{margin-top:5px}input[type=button].btn-block,input[type=reset].btn-block,input[type=submit].btn-block{width:100%}.fade{opacity:0;-webkit-transition:opacity .15s linear;-o-transition:opacity .15s linear;transition:opacity .15s linear}.fade.in{opacity:1}.collapse{display:none}.collapse.in{display:block}tr.collapse.in{display:table-row}tbody.collapse.in{display:table-row-group}.collapsing{position:relative;height:0;overflow:hidden;-webkit-transition-timing-function:ease;-o-transition-timing-function:ease;transition-timing-function:ease;-webkit-transition-duration:.35s;-o-transition-duration:.35s;transition-duration:.35s;-webkit-transition-property:height,visibility;-o-transition-property:height,visibility;transition-property:height,visibility}.caret{display:inline-block;width:0;height:0;margin-left:2px;vertical-align:middle;border-top:4px dashed;border-top:4px solid\9;border-right:4px solid transparent;border-left:4px solid transparent}.dropdown,.dropup{position:relative}.dropdown-toggle:focus{outline:0}.dropdown-menu{position:absolute;top:100%;left:0;z-index:1000;display:none;float:left;min-width:160px;padding:5px 0;margin:2px 0 0;font-size:14px;text-align:left;list-style:none;background-color:#fff;-webkit-background-clip:padding-box;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.15);border-radius:4px;-webkit-box-shadow:0 6px 12px rgba(0,0,0,.175);box-shadow:0 6px 12px rgba(0,0,0,.175)}.dropdown-menu.pull-right{right:0;left:auto}.dropdown-menu .divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.dropdown-menu>li>a{display:block;padding:3px 20px;clear:both;font-weight:400;line-height:1.42857143;color:#333;white-space:nowrap}.dropdown-menu>li>a:focus,.dropdown-menu>li>a:hover{color:#262626;text-decoration:none;background-color:#f5f5f5}.dropdown-menu>.active>a,.dropdown-menu>.active>a:focus,.dropdown-menu>.active>a:hover{color:#fff;text-decoration:none;background-color:#337ab7;outline:0}.dropdown-menu>.disabled>a,.dropdown-menu>.disabled>a:focus,.dropdown-menu>.disabled>a:hover{color:#777}.dropdown-menu>.disabled>a:focus,.dropdown-menu>.disabled>a:hover{text-decoration:none;cursor:not-allowed;background-color:transparent;background-image:none;filter:progid:DXImageTransform.Microsoft.gradient(enabled=false)}.open>.dropdown-menu{display:block}.open>a{outline:0}.dropdown-menu-right{right:0;left:auto}.dropdown-menu-left{right:auto;left:0}.dropdown-header{display:block;padding:3px 20px;font-size:12px;line-height:1.42857143;color:#777;white-space:nowrap}.dropdown-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:990}.pull-right>.dropdown-menu{right:0;left:auto}.dropup .caret,.navbar-fixed-bottom .dropdown .caret{content:"";border-top:0;border-bottom:4px dashed;border-bottom:4px solid\9}.dropup .dropdown-menu,.navbar-fixed-bottom .dropdown .dropdown-menu{top:auto;bottom:100%;margin-bottom:2px}@media (min-width:768px){.navbar-right .dropdown-menu{right:0;left:auto}.navbar-right .dropdown-menu-left{right:auto;left:0}}.btn-group,.btn-group-vertical{position:relative;display:inline-block;vertical-align:middle}.btn-group-vertical>.btn,.btn-group>.btn{position:relative;float:left}.btn-group-vertical>.btn.active,.btn-group-vertical>.btn:active,.btn-group-vertical>.btn:focus,.btn-group-vertical>.btn:hover,.btn-group>.btn.active,.btn-group>.btn:active,.btn-group>.btn:focus,.btn-group>.btn:hover{z-index:2}.btn-group .btn+.btn,.btn-group .btn+.btn-group,.btn-group .btn-group+.btn,.btn-group .btn-group+.btn-group{margin-left:-1px}.btn-toolbar{margin-left:-5px}.btn-toolbar .btn,.btn-toolbar .btn-group,.btn-toolbar .input-group{float:left}.btn-toolbar>.btn,.btn-toolbar>.btn-group,.btn-toolbar>.input-group{margin-left:5px}.btn-group>.btn:not(:first-child):not(:last-child):not(.dropdown-toggle){border-radius:0}.btn-group>.btn:first-child{margin-left:0}.btn-group>.btn:first-child:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn:last-child:not(:first-child),.btn-group>.dropdown-toggle:not(:first-child){border-top-left-radius:0;border-bottom-left-radius:0}.btn-group>.btn-group{float:left}.btn-group>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-bottom-left-radius:0}.btn-group .dropdown-toggle:active,.btn-group.open .dropdown-toggle{outline:0}.btn-group>.btn+.dropdown-toggle{padding-right:8px;padding-left:8px}.btn-group>.btn-lg+.dropdown-toggle{padding-right:12px;padding-left:12px}.btn-group.open .dropdown-toggle{-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn-group.open .dropdown-toggle.btn-link{-webkit-box-shadow:none;box-shadow:none}.btn .caret{margin-left:0}.btn-lg .caret{border-width:5px 5px 0;border-bottom-width:0}.dropup .btn-lg .caret{border-width:0 5px 5px}.btn-group-vertical>.btn,.btn-group-vertical>.btn-group,.btn-group-vertical>.btn-group>.btn{display:block;float:none;width:100%;max-width:100%}.btn-group-vertical>.btn-group>.btn{float:none}.btn-group-vertical>.btn+.btn,.btn-group-vertical>.btn+.btn-group,.btn-group-vertical>.btn-group+.btn,.btn-group-vertical>.btn-group+.btn-group{margin-top:-1px;margin-left:0}.btn-group-vertical>.btn:not(:first-child):not(:last-child){border-radius:0}.btn-group-vertical>.btn:first-child:not(:last-child){border-top-left-radius:4px;border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn:last-child:not(:first-child){border-top-left-radius:0;border-top-right-radius:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}.btn-group-vertical>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group-vertical>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group-vertical>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-top-right-radius:0}.btn-group-justified{display:table;width:100%;table-layout:fixed;border-collapse:separate}.btn-group-justified>.btn,.btn-group-justified>.btn-group{display:table-cell;float:none;width:1%}.btn-group-justified>.btn-group .btn{width:100%}.btn-group-justified>.btn-group .dropdown-menu{left:auto}[data-toggle=buttons]>.btn input[type=checkbox],[data-toggle=buttons]>.btn input[type=radio],[data-toggle=buttons]>.btn-group>.btn input[type=checkbox],[data-toggle=buttons]>.btn-group>.btn input[type=radio]{position:absolute;clip:rect(0,0,0,0);pointer-events:none}.input-group{position:relative;display:table;border-collapse:separate}.input-group[class*=col-]{float:none;padding-right:0;padding-left:0}.input-group .form-control{position:relative;z-index:2;float:left;width:100%;margin-bottom:0}.input-group .form-control:focus{z-index:3}.input-group-lg>.form-control,.input-group-lg>.input-group-addon,.input-group-lg>.input-group-btn>.btn{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}select.input-group-lg>.form-control,select.input-group-lg>.input-group-addon,select.input-group-lg>.input-group-btn>.btn{height:46px;line-height:46px}select[multiple].input-group-lg>.form-control,select[multiple].input-group-lg>.input-group-addon,select[multiple].input-group-lg>.input-group-btn>.btn,textarea.input-group-lg>.form-control,textarea.input-group-lg>.input-group-addon,textarea.input-group-lg>.input-group-btn>.btn{height:auto}.input-group-sm>.form-control,.input-group-sm>.input-group-addon,.input-group-sm>.input-group-btn>.btn{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-group-sm>.form-control,select.input-group-sm>.input-group-addon,select.input-group-sm>.input-group-btn>.btn{height:30px;line-height:30px}select[multiple].input-group-sm>.form-control,select[multiple].input-group-sm>.input-group-addon,select[multiple].input-group-sm>.input-group-btn>.btn,textarea.input-group-sm>.form-control,textarea.input-group-sm>.input-group-addon,textarea.input-group-sm>.input-group-btn>.btn{height:auto}.input-group .form-control,.input-group-addon,.input-group-btn{display:table-cell}.input-group .form-control:not(:first-child):not(:last-child),.input-group-addon:not(:first-child):not(:last-child),.input-group-btn:not(:first-child):not(:last-child){border-radius:0}.input-group-addon,.input-group-btn{width:1%;white-space:nowrap;vertical-align:middle}.input-group-addon{padding:6px 12px;font-size:14px;font-weight:400;line-height:1;color:#555;text-align:center;background-color:#eee;border:1px solid #ccc;border-radius:4px}.input-group-addon.input-sm{padding:5px 10px;font-size:12px;border-radius:3px}.input-group-addon.input-lg{padding:10px 16px;font-size:18px;border-radius:6px}.input-group-addon input[type=checkbox],.input-group-addon input[type=radio]{margin-top:0}.input-group .form-control:first-child,.input-group-addon:first-child,.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group>.btn,.input-group-btn:first-child>.dropdown-toggle,.input-group-btn:last-child>.btn-group:not(:last-child)>.btn,.input-group-btn:last-child>.btn:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.input-group-addon:first-child{border-right:0}.input-group .form-control:last-child,.input-group-addon:last-child,.input-group-btn:first-child>.btn-group:not(:first-child)>.btn,.input-group-btn:first-child>.btn:not(:first-child),.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group>.btn,.input-group-btn:last-child>.dropdown-toggle{border-top-left-radius:0;border-bottom-left-radius:0}.input-group-addon:last-child{border-left:0}.input-group-btn{position:relative;font-size:0;white-space:nowrap}.input-group-btn>.btn{position:relative}.input-group-btn>.btn+.btn{margin-left:-1px}.input-group-btn>.btn:active,.input-group-btn>.btn:focus,.input-group-btn>.btn:hover{z-index:2}.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group{margin-right:-1px}.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group{z-index:2;margin-left:-1px}.nav{padding-left:0;margin-bottom:0;list-style:none}.nav>li{position:relative;display:block}.nav>li>a{position:relative;display:block;padding:10px 15px}.nav>li>a:focus,.nav>li>a:hover{text-decoration:none;background-color:#eee}.nav>li.disabled>a{color:#777}.nav>li.disabled>a:focus,.nav>li.disabled>a:hover{color:#777;text-decoration:none;cursor:not-allowed;background-color:transparent}.nav .open>a,.nav .open>a:focus,.nav .open>a:hover{background-color:#eee;border-color:#337ab7}.nav .nav-divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.nav>li>a>img{max-width:none}.nav-tabs{border-bottom:1px solid #ddd}.nav-tabs>li{float:left;margin-bottom:-1px}.nav-tabs>li>a{margin-right:2px;line-height:1.42857143;border:1px solid transparent;border-radius:4px 4px 0 0}.nav-tabs>li>a:hover{border-color:#eee #eee #ddd}.nav-tabs>li.active>a,.nav-tabs>li.active>a:focus,.nav-tabs>li.active>a:hover{color:#555;cursor:default;background-color:#fff;border:1px solid #ddd;border-bottom-color:transparent}.nav-tabs.nav-justified{width:100%;border-bottom:0}.nav-tabs.nav-justified>li{float:none}.nav-tabs.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-tabs.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-tabs.nav-justified>li{display:table-cell;width:1%}.nav-tabs.nav-justified>li>a{margin-bottom:0}}.nav-tabs.nav-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:focus,.nav-tabs.nav-justified>.active>a:hover{border:1px solid #ddd}@media (min-width:768px){.nav-tabs.nav-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:focus,.nav-tabs.nav-justified>.active>a:hover{border-bottom-color:#fff}}.nav-pills>li{float:left}.nav-pills>li>a{border-radius:4px}.nav-pills>li+li{margin-left:2px}.nav-pills>li.active>a,.nav-pills>li.active>a:focus,.nav-pills>li.active>a:hover{color:#fff;background-color:#337ab7}.nav-stacked>li{float:none}.nav-stacked>li+li{margin-top:2px;margin-left:0}.nav-justified{width:100%}.nav-justified>li{float:none}.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-justified>li{display:table-cell;width:1%}.nav-justified>li>a{margin-bottom:0}}.nav-tabs-justified{border-bottom:0}.nav-tabs-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:focus,.nav-tabs-justified>.active>a:hover{border:1px solid #ddd}@media (min-width:768px){.nav-tabs-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:focus,.nav-tabs-justified>.active>a:hover{border-bottom-color:#fff}}.tab-content>.tab-pane{display:none}.tab-content>.active{display:block}.nav-tabs .dropdown-menu{margin-top:-1px;border-top-left-radius:0;border-top-right-radius:0}.navbar{position:relative;min-height:50px;margin-bottom:20px;border:1px solid transparent}@media (min-width:768px){.navbar{border-radius:4px}}@media (min-width:768px){.navbar-header{float:left}}.navbar-collapse{padding-right:15px;padding-left:15px;overflow-x:visible;-webkit-overflow-scrolling:touch;border-top:1px solid transparent;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 0 rgba(255,255,255,.1)}.navbar-collapse.in{overflow-y:auto}@media (min-width:768px){.navbar-collapse{width:auto;border-top:0;-webkit-box-shadow:none;box-shadow:none}.navbar-collapse.collapse{display:block!important;height:auto!important;padding-bottom:0;overflow:visible!important}.navbar-collapse.in{overflow-y:visible}.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse,.navbar-static-top .navbar-collapse{padding-right:0;padding-left:0}}.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse{max-height:340px}@media (max-device-width:480px) and (orientation:landscape){.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse{max-height:200px}}.container-fluid>.navbar-collapse,.container-fluid>.navbar-header,.container>.navbar-collapse,.container>.navbar-header{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.container-fluid>.navbar-collapse,.container-fluid>.navbar-header,.container>.navbar-collapse,.container>.navbar-header{margin-right:0;margin-left:0}}.navbar-static-top{z-index:1000;border-width:0 0 1px}@media (min-width:768px){.navbar-static-top{border-radius:0}}.navbar-fixed-bottom,.navbar-fixed-top{position:fixed;right:0;left:0;z-index:1030}@media (min-width:768px){.navbar-fixed-bottom,.navbar-fixed-top{border-radius:0}}.navbar-fixed-top{top:0;border-width:0 0 1px}.navbar-fixed-bottom{bottom:0;margin-bottom:0;border-width:1px 0 0}.navbar-brand{float:left;height:50px;padding:15px 15px;font-size:18px;line-height:20px}.navbar-brand:focus,.navbar-brand:hover{text-decoration:none}.navbar-brand>img{display:block}@media (min-width:768px){.navbar>.container .navbar-brand,.navbar>.container-fluid .navbar-brand{margin-left:-15px}}.navbar-toggle{position:relative;float:right;padding:9px 10px;margin-top:8px;margin-right:15px;margin-bottom:8px;background-color:transparent;background-image:none;border:1px solid transparent;border-radius:4px}.navbar-toggle:focus{outline:0}.navbar-toggle .icon-bar{display:block;width:22px;height:2px;border-radius:1px}.navbar-toggle .icon-bar+.icon-bar{margin-top:4px}@media (min-width:768px){.navbar-toggle{display:none}}.navbar-nav{margin:7.5px -15px}.navbar-nav>li>a{padding-top:10px;padding-bottom:10px;line-height:20px}@media (max-width:767px){.navbar-nav .open .dropdown-menu{position:static;float:none;width:auto;margin-top:0;background-color:transparent;border:0;-webkit-box-shadow:none;box-shadow:none}.navbar-nav .open .dropdown-menu .dropdown-header,.navbar-nav .open .dropdown-menu>li>a{padding:5px 15px 5px 25px}.navbar-nav .open .dropdown-menu>li>a{line-height:20px}.navbar-nav .open .dropdown-menu>li>a:focus,.navbar-nav .open .dropdown-menu>li>a:hover{background-image:none}}@media (min-width:768px){.navbar-nav{float:left;margin:0}.navbar-nav>li{float:left}.navbar-nav>li>a{padding-top:15px;padding-bottom:15px}}.navbar-form{padding:10px 15px;margin-top:8px;margin-right:-15px;margin-bottom:8px;margin-left:-15px;border-top:1px solid transparent;border-bottom:1px solid transparent;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1)}@media (min-width:768px){.navbar-form .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.navbar-form .form-control{display:inline-block;width:auto;vertical-align:middle}.navbar-form .form-control-static{display:inline-block}.navbar-form .input-group{display:inline-table;vertical-align:middle}.navbar-form .input-group .form-control,.navbar-form .input-group .input-group-addon,.navbar-form .input-group .input-group-btn{width:auto}.navbar-form .input-group>.form-control{width:100%}.navbar-form .control-label{margin-bottom:0;vertical-align:middle}.navbar-form .checkbox,.navbar-form .radio{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.navbar-form .checkbox label,.navbar-form .radio label{padding-left:0}.navbar-form .checkbox input[type=checkbox],.navbar-form .radio input[type=radio]{position:relative;margin-left:0}.navbar-form .has-feedback .form-control-feedback{top:0}}@media (max-width:767px){.navbar-form .form-group{margin-bottom:5px}.navbar-form .form-group:last-child{margin-bottom:0}}@media (min-width:768px){.navbar-form{width:auto;padding-top:0;padding-bottom:0;margin-right:0;margin-left:0;border:0;-webkit-box-shadow:none;box-shadow:none}}.navbar-nav>li>.dropdown-menu{margin-top:0;border-top-left-radius:0;border-top-right-radius:0}.navbar-fixed-bottom .navbar-nav>li>.dropdown-menu{margin-bottom:0;border-top-left-radius:4px;border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.navbar-btn{margin-top:8px;margin-bottom:8px}.navbar-btn.btn-sm{margin-top:10px;margin-bottom:10px}.navbar-btn.btn-xs{margin-top:14px;margin-bottom:14px}.navbar-text{margin-top:15px;margin-bottom:15px}@media (min-width:768px){.navbar-text{float:left;margin-right:15px;margin-left:15px}}@media (min-width:768px){.navbar-left{float:left!important}.navbar-right{float:right!important;margin-right:-15px}.navbar-right~.navbar-right{margin-right:0}}.navbar-default{background-color:#f8f8f8;border-color:#e7e7e7}.navbar-default .navbar-brand{color:#777}.navbar-default .navbar-brand:focus,.navbar-default .navbar-brand:hover{color:#5e5e5e;background-color:transparent}.navbar-default .navbar-text{color:#777}.navbar-default .navbar-nav>li>a{color:#777}.navbar-default .navbar-nav>li>a:focus,.navbar-default .navbar-nav>li>a:hover{color:#333;background-color:transparent}.navbar-default .navbar-nav>.active>a,.navbar-default .navbar-nav>.active>a:focus,.navbar-default .navbar-nav>.active>a:hover{color:#555;background-color:#e7e7e7}.navbar-default .navbar-nav>.disabled>a,.navbar-default .navbar-nav>.disabled>a:focus,.navbar-default .navbar-nav>.disabled>a:hover{color:#ccc;background-color:transparent}.navbar-default .navbar-toggle{border-color:#ddd}.navbar-default .navbar-toggle:focus,.navbar-default .navbar-toggle:hover{background-color:#ddd}.navbar-default .navbar-toggle .icon-bar{background-color:#888}.navbar-default .navbar-collapse,.navbar-default .navbar-form{border-color:#e7e7e7}.navbar-default .navbar-nav>.open>a,.navbar-default .navbar-nav>.open>a:focus,.navbar-default .navbar-nav>.open>a:hover{color:#555;background-color:#e7e7e7}@media (max-width:767px){.navbar-default .navbar-nav .open .dropdown-menu>li>a{color:#777}.navbar-default .navbar-nav .open .dropdown-menu>li>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>li>a:hover{color:#333;background-color:transparent}.navbar-default .navbar-nav .open .dropdown-menu>.active>a,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:hover{color:#555;background-color:#e7e7e7}.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:hover{color:#ccc;background-color:transparent}}.navbar-default .navbar-link{color:#777}.navbar-default .navbar-link:hover{color:#333}.navbar-default .btn-link{color:#777}.navbar-default .btn-link:focus,.navbar-default .btn-link:hover{color:#333}.navbar-default .btn-link[disabled]:focus,.navbar-default .btn-link[disabled]:hover,fieldset[disabled] .navbar-default .btn-link:focus,fieldset[disabled] .navbar-default .btn-link:hover{color:#ccc}.navbar-inverse{background-color:#222;border-color:#080808}.navbar-inverse .navbar-brand{color:#9d9d9d}.navbar-inverse .navbar-brand:focus,.navbar-inverse .navbar-brand:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-text{color:#9d9d9d}.navbar-inverse .navbar-nav>li>a{color:#9d9d9d}.navbar-inverse .navbar-nav>li>a:focus,.navbar-inverse .navbar-nav>li>a:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-nav>.active>a,.navbar-inverse .navbar-nav>.active>a:focus,.navbar-inverse .navbar-nav>.active>a:hover{color:#fff;background-color:#080808}.navbar-inverse .navbar-nav>.disabled>a,.navbar-inverse .navbar-nav>.disabled>a:focus,.navbar-inverse .navbar-nav>.disabled>a:hover{color:#444;background-color:transparent}.navbar-inverse .navbar-toggle{border-color:#333}.navbar-inverse .navbar-toggle:focus,.navbar-inverse .navbar-toggle:hover{background-color:#333}.navbar-inverse .navbar-toggle .icon-bar{background-color:#fff}.navbar-inverse .navbar-collapse,.navbar-inverse .navbar-form{border-color:#101010}.navbar-inverse .navbar-nav>.open>a,.navbar-inverse .navbar-nav>.open>a:focus,.navbar-inverse .navbar-nav>.open>a:hover{color:#fff;background-color:#080808}@media (max-width:767px){.navbar-inverse .navbar-nav .open .dropdown-menu>.dropdown-header{border-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu .divider{background-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a{color:#9d9d9d}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:hover{color:#fff;background-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:hover{color:#444;background-color:transparent}}.navbar-inverse .navbar-link{color:#9d9d9d}.navbar-inverse .navbar-link:hover{color:#fff}.navbar-inverse .btn-link{color:#9d9d9d}.navbar-inverse .btn-link:focus,.navbar-inverse .btn-link:hover{color:#fff}.navbar-inverse .btn-link[disabled]:focus,.navbar-inverse .btn-link[disabled]:hover,fieldset[disabled] .navbar-inverse .btn-link:focus,fieldset[disabled] .navbar-inverse .btn-link:hover{color:#444}.breadcrumb{padding:8px 15px;margin-bottom:20px;list-style:none;background-color:#f5f5f5;border-radius:4px}.breadcrumb>li{display:inline-block}.breadcrumb>li+li:before{padding:0 5px;color:#ccc;content:"/\00a0"}.breadcrumb>.active{color:#777}.pagination{display:inline-block;padding-left:0;margin:20px 0;border-radius:4px}.pagination>li{display:inline}.pagination>li>a,.pagination>li>span{position:relative;float:left;padding:6px 12px;margin-left:-1px;line-height:1.42857143;color:#337ab7;text-decoration:none;background-color:#fff;border:1px solid #ddd}.pagination>li:first-child>a,.pagination>li:first-child>span{margin-left:0;border-top-left-radius:4px;border-bottom-left-radius:4px}.pagination>li:last-child>a,.pagination>li:last-child>span{border-top-right-radius:4px;border-bottom-right-radius:4px}.pagination>li>a:focus,.pagination>li>a:hover,.pagination>li>span:focus,.pagination>li>span:hover{z-index:2;color:#23527c;background-color:#eee;border-color:#ddd}.pagination>.active>a,.pagination>.active>a:focus,.pagination>.active>a:hover,.pagination>.active>span,.pagination>.active>span:focus,.pagination>.active>span:hover{z-index:3;color:#fff;cursor:default;background-color:#337ab7;border-color:#337ab7}.pagination>.disabled>a,.pagination>.disabled>a:focus,.pagination>.disabled>a:hover,.pagination>.disabled>span,.pagination>.disabled>span:focus,.pagination>.disabled>span:hover{color:#777;cursor:not-allowed;background-color:#fff;border-color:#ddd}.pagination-lg>li>a,.pagination-lg>li>span{padding:10px 16px;font-size:18px;line-height:1.3333333}.pagination-lg>li:first-child>a,.pagination-lg>li:first-child>span{border-top-left-radius:6px;border-bottom-left-radius:6px}.pagination-lg>li:last-child>a,.pagination-lg>li:last-child>span{border-top-right-radius:6px;border-bottom-right-radius:6px}.pagination-sm>li>a,.pagination-sm>li>span{padding:5px 10px;font-size:12px;line-height:1.5}.pagination-sm>li:first-child>a,.pagination-sm>li:first-child>span{border-top-left-radius:3px;border-bottom-left-radius:3px}.pagination-sm>li:last-child>a,.pagination-sm>li:last-child>span{border-top-right-radius:3px;border-bottom-right-radius:3px}.pager{padding-left:0;margin:20px 0;text-align:center;list-style:none}.pager li{display:inline}.pager li>a,.pager li>span{display:inline-block;padding:5px 14px;background-color:#fff;border:1px solid #ddd;border-radius:15px}.pager li>a:focus,.pager li>a:hover{text-decoration:none;background-color:#eee}.pager .next>a,.pager .next>span{float:right}.pager .previous>a,.pager .previous>span{float:left}.pager .disabled>a,.pager .disabled>a:focus,.pager .disabled>a:hover,.pager .disabled>span{color:#777;cursor:not-allowed;background-color:#fff}.label{display:inline;padding:.2em .6em .3em;font-size:75%;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:baseline;border-radius:.25em}a.label:focus,a.label:hover{color:#fff;text-decoration:none;cursor:pointer}.label:empty{display:none}.btn .label{position:relative;top:-1px}.label-default{background-color:#777}.label-default[href]:focus,.label-default[href]:hover{background-color:#5e5e5e}.label-primary{background-color:#337ab7}.label-primary[href]:focus,.label-primary[href]:hover{background-color:#286090}.label-success{background-color:#5cb85c}.label-success[href]:focus,.label-success[href]:hover{background-color:#449d44}.label-info{background-color:#5bc0de}.label-info[href]:focus,.label-info[href]:hover{background-color:#31b0d5}.label-warning{background-color:#f0ad4e}.label-warning[href]:focus,.label-warning[href]:hover{background-color:#ec971f}.label-danger{background-color:#d9534f}.label-danger[href]:focus,.label-danger[href]:hover{background-color:#c9302c}.badge{display:inline-block;min-width:10px;padding:3px 7px;font-size:12px;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:middle;background-color:#777;border-radius:10px}.badge:empty{display:none}.btn .badge{position:relative;top:-1px}.btn-group-xs>.btn .badge,.btn-xs .badge{top:0;padding:1px 5px}a.badge:focus,a.badge:hover{color:#fff;text-decoration:none;cursor:pointer}.list-group-item.active>.badge,.nav-pills>.active>a>.badge{color:#337ab7;background-color:#fff}.list-group-item>.badge{float:right}.list-group-item>.badge+.badge{margin-right:5px}.nav-pills>li>a>.badge{margin-left:3px}.jumbotron{padding-top:30px;padding-bottom:30px;margin-bottom:30px;color:inherit;background-color:#eee}.jumbotron .h1,.jumbotron h1{color:inherit}.jumbotron p{margin-bottom:15px;font-size:21px;font-weight:200}.jumbotron>hr{border-top-color:#d5d5d5}.container .jumbotron,.container-fluid .jumbotron{padding-right:15px;padding-left:15px;border-radius:6px}.jumbotron .container{max-width:100%}@media screen and (min-width:768px){.jumbotron{padding-top:48px;padding-bottom:48px}.container .jumbotron,.container-fluid .jumbotron{padding-right:60px;padding-left:60px}.jumbotron .h1,.jumbotron h1{font-size:63px}}.thumbnail{display:block;padding:4px;margin-bottom:20px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:border .2s ease-in-out;-o-transition:border .2s ease-in-out;transition:border .2s ease-in-out}.thumbnail a>img,.thumbnail>img{margin-right:auto;margin-left:auto}a.thumbnail.active,a.thumbnail:focus,a.thumbnail:hover{border-color:#337ab7}.thumbnail .caption{padding:9px;color:#333}.alert{padding:15px;margin-bottom:20px;border:1px solid transparent;border-radius:4px}.alert h4{margin-top:0;color:inherit}.alert .alert-link{font-weight:700}.alert>p,.alert>ul{margin-bottom:0}.alert>p+p{margin-top:5px}.alert-dismissable,.alert-dismissible{padding-right:35px}.alert-dismissable .close,.alert-dismissible .close{position:relative;top:-2px;right:-21px;color:inherit}.alert-success{color:#3c763d;background-color:#dff0d8;border-color:#d6e9c6}.alert-success hr{border-top-color:#c9e2b3}.alert-success .alert-link{color:#2b542c}.alert-info{color:#31708f;background-color:#d9edf7;border-color:#bce8f1}.alert-info hr{border-top-color:#a6e1ec}.alert-info .alert-link{color:#245269}.alert-warning{color:#8a6d3b;background-color:#fcf8e3;border-color:#faebcc}.alert-warning hr{border-top-color:#f7e1b5}.alert-warning .alert-link{color:#66512c}.alert-danger{color:#a94442;background-color:#f2dede;border-color:#ebccd1}.alert-danger hr{border-top-color:#e4b9c0}.alert-danger .alert-link{color:#843534}@-webkit-keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}@-o-keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}@keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}.progress{height:20px;margin-bottom:20px;overflow:hidden;background-color:#f5f5f5;border-radius:4px;-webkit-box-shadow:inset 0 1px 2px rgba(0,0,0,.1);box-shadow:inset 0 1px 2px rgba(0,0,0,.1)}.progress-bar{float:left;width:0;height:100%;font-size:12px;line-height:20px;color:#fff;text-align:center;background-color:#337ab7;-webkit-box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);-webkit-transition:width .6s ease;-o-transition:width .6s ease;transition:width .6s ease}.progress-bar-striped,.progress-striped .progress-bar{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);-webkit-background-size:40px 40px;background-size:40px 40px}.progress-bar.active,.progress.active .progress-bar{-webkit-animation:progress-bar-stripes 2s linear infinite;-o-animation:progress-bar-stripes 2s linear infinite;animation:progress-bar-stripes 2s linear infinite}.progress-bar-success{background-color:#5cb85c}.progress-striped .progress-bar-success{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-info{background-color:#5bc0de}.progress-striped .progress-bar-info{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-warning{background-color:#f0ad4e}.progress-striped .progress-bar-warning{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-danger{background-color:#d9534f}.progress-striped .progress-bar-danger{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.media{margin-top:15px}.media:first-child{margin-top:0}.media,.media-body{overflow:hidden;zoom:1}.media-body{width:10000px}.media-object{display:block}.media-object.img-thumbnail{max-width:none}.media-right,.media>.pull-right{padding-left:10px}.media-left,.media>.pull-left{padding-right:10px}.media-body,.media-left,.media-right{display:table-cell;vertical-align:top}.media-middle{vertical-align:middle}.media-bottom{vertical-align:bottom}.media-heading{margin-top:0;margin-bottom:5px}.media-list{padding-left:0;list-style:none}.list-group{padding-left:0;margin-bottom:20px}.list-group-item{position:relative;display:block;padding:10px 15px;margin-bottom:-1px;background-color:#fff;border:1px solid #ddd}.list-group-item:first-child{border-top-left-radius:4px;border-top-right-radius:4px}.list-group-item:last-child{margin-bottom:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}a.list-group-item,button.list-group-item{color:#555}a.list-group-item .list-group-item-heading,button.list-group-item .list-group-item-heading{color:#333}a.list-group-item:focus,a.list-group-item:hover,button.list-group-item:focus,button.list-group-item:hover{color:#555;text-decoration:none;background-color:#f5f5f5}button.list-group-item{width:100%;text-align:left}.list-group-item.disabled,.list-group-item.disabled:focus,.list-group-item.disabled:hover{color:#777;cursor:not-allowed;background-color:#eee}.list-group-item.disabled .list-group-item-heading,.list-group-item.disabled:focus .list-group-item-heading,.list-group-item.disabled:hover .list-group-item-heading{color:inherit}.list-group-item.disabled .list-group-item-text,.list-group-item.disabled:focus .list-group-item-text,.list-group-item.disabled:hover .list-group-item-text{color:#777}.list-group-item.active,.list-group-item.active:focus,.list-group-item.active:hover{z-index:2;color:#fff;background-color:#337ab7;border-color:#337ab7}.list-group-item.active .list-group-item-heading,.list-group-item.active .list-group-item-heading>.small,.list-group-item.active .list-group-item-heading>small,.list-group-item.active:focus .list-group-item-heading,.list-group-item.active:focus .list-group-item-heading>.small,.list-group-item.active:focus .list-group-item-heading>small,.list-group-item.active:hover .list-group-item-heading,.list-group-item.active:hover .list-group-item-heading>.small,.list-group-item.active:hover .list-group-item-heading>small{color:inherit}.list-group-item.active .list-group-item-text,.list-group-item.active:focus .list-group-item-text,.list-group-item.active:hover .list-group-item-text{color:#c7ddef}.list-group-item-success{color:#3c763d;background-color:#dff0d8}a.list-group-item-success,button.list-group-item-success{color:#3c763d}a.list-group-item-success .list-group-item-heading,button.list-group-item-success .list-group-item-heading{color:inherit}a.list-group-item-success:focus,a.list-group-item-success:hover,button.list-group-item-success:focus,button.list-group-item-success:hover{color:#3c763d;background-color:#d0e9c6}a.list-group-item-success.active,a.list-group-item-success.active:focus,a.list-group-item-success.active:hover,button.list-group-item-success.active,button.list-group-item-success.active:focus,button.list-group-item-success.active:hover{color:#fff;background-color:#3c763d;border-color:#3c763d}.list-group-item-info{color:#31708f;background-color:#d9edf7}a.list-group-item-info,button.list-group-item-info{color:#31708f}a.list-group-item-info .list-group-item-heading,button.list-group-item-info .list-group-item-heading{color:inherit}a.list-group-item-info:focus,a.list-group-item-info:hover,button.list-group-item-info:focus,button.list-group-item-info:hover{color:#31708f;background-color:#c4e3f3}a.list-group-item-info.active,a.list-group-item-info.active:focus,a.list-group-item-info.active:hover,button.list-group-item-info.active,button.list-group-item-info.active:focus,button.list-group-item-info.active:hover{color:#fff;background-color:#31708f;border-color:#31708f}.list-group-item-warning{color:#8a6d3b;background-color:#fcf8e3}a.list-group-item-warning,button.list-group-item-warning{color:#8a6d3b}a.list-group-item-warning .list-group-item-heading,button.list-group-item-warning .list-group-item-heading{color:inherit}a.list-group-item-warning:focus,a.list-group-item-warning:hover,button.list-group-item-warning:focus,button.list-group-item-warning:hover{color:#8a6d3b;background-color:#faf2cc}a.list-group-item-warning.active,a.list-group-item-warning.active:focus,a.list-group-item-warning.active:hover,button.list-group-item-warning.active,button.list-group-item-warning.active:focus,button.list-group-item-warning.active:hover{color:#fff;background-color:#8a6d3b;border-color:#8a6d3b}.list-group-item-danger{color:#a94442;background-color:#f2dede}a.list-group-item-danger,button.list-group-item-danger{color:#a94442}a.list-group-item-danger .list-group-item-heading,button.list-group-item-danger .list-group-item-heading{color:inherit}a.list-group-item-danger:focus,a.list-group-item-danger:hover,button.list-group-item-danger:focus,button.list-group-item-danger:hover{color:#a94442;background-color:#ebcccc}a.list-group-item-danger.active,a.list-group-item-danger.active:focus,a.list-group-item-danger.active:hover,button.list-group-item-danger.active,button.list-group-item-danger.active:focus,button.list-group-item-danger.active:hover{color:#fff;background-color:#a94442;border-color:#a94442}.list-group-item-heading{margin-top:0;margin-bottom:5px}.list-group-item-text{margin-bottom:0;line-height:1.3}.panel{margin-bottom:20px;background-color:#fff;border:1px solid transparent;border-radius:4px;-webkit-box-shadow:0 1px 1px rgba(0,0,0,.05);box-shadow:0 1px 1px rgba(0,0,0,.05)}.panel-body{padding:15px}.panel-heading{padding:10px 15px;border-bottom:1px solid transparent;border-top-left-radius:3px;border-top-right-radius:3px}.panel-heading>.dropdown .dropdown-toggle{color:inherit}.panel-title{margin-top:0;margin-bottom:0;font-size:16px;color:inherit}.panel-title>.small,.panel-title>.small>a,.panel-title>a,.panel-title>small,.panel-title>small>a{color:inherit}.panel-footer{padding:10px 15px;background-color:#f5f5f5;border-top:1px solid #ddd;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.list-group,.panel>.panel-collapse>.list-group{margin-bottom:0}.panel>.list-group .list-group-item,.panel>.panel-collapse>.list-group .list-group-item{border-width:1px 0;border-radius:0}.panel>.list-group:first-child .list-group-item:first-child,.panel>.panel-collapse>.list-group:first-child .list-group-item:first-child{border-top:0;border-top-left-radius:3px;border-top-right-radius:3px}.panel>.list-group:last-child .list-group-item:last-child,.panel>.panel-collapse>.list-group:last-child .list-group-item:last-child{border-bottom:0;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.panel-heading+.panel-collapse>.list-group .list-group-item:first-child{border-top-left-radius:0;border-top-right-radius:0}.panel-heading+.list-group .list-group-item:first-child{border-top-width:0}.list-group+.panel-footer{border-top-width:0}.panel>.panel-collapse>.table,.panel>.table,.panel>.table-responsive>.table{margin-bottom:0}.panel>.panel-collapse>.table caption,.panel>.table caption,.panel>.table-responsive>.table caption{padding-right:15px;padding-left:15px}.panel>.table-responsive:first-child>.table:first-child,.panel>.table:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child,.panel>.table:first-child>thead:first-child>tr:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table:first-child>thead:first-child>tr:first-child th:first-child{border-top-left-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table:first-child>thead:first-child>tr:first-child th:last-child{border-top-right-radius:3px}.panel>.table-responsive:last-child>.table:last-child,.panel>.table:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:first-child{border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:last-child{border-bottom-right-radius:3px}.panel>.panel-body+.table,.panel>.panel-body+.table-responsive,.panel>.table+.panel-body,.panel>.table-responsive+.panel-body{border-top:1px solid #ddd}.panel>.table>tbody:first-child>tr:first-child td,.panel>.table>tbody:first-child>tr:first-child th{border-top:0}.panel>.table-bordered,.panel>.table-responsive>.table-bordered{border:0}.panel>.table-bordered>tbody>tr>td:first-child,.panel>.table-bordered>tbody>tr>th:first-child,.panel>.table-bordered>tfoot>tr>td:first-child,.panel>.table-bordered>tfoot>tr>th:first-child,.panel>.table-bordered>thead>tr>td:first-child,.panel>.table-bordered>thead>tr>th:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:first-child,.panel>.table-responsive>.table-bordered>thead>tr>td:first-child,.panel>.table-responsive>.table-bordered>thead>tr>th:first-child{border-left:0}.panel>.table-bordered>tbody>tr>td:last-child,.panel>.table-bordered>tbody>tr>th:last-child,.panel>.table-bordered>tfoot>tr>td:last-child,.panel>.table-bordered>tfoot>tr>th:last-child,.panel>.table-bordered>thead>tr>td:last-child,.panel>.table-bordered>thead>tr>th:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:last-child,.panel>.table-responsive>.table-bordered>thead>tr>td:last-child,.panel>.table-responsive>.table-bordered>thead>tr>th:last-child{border-right:0}.panel>.table-bordered>tbody>tr:first-child>td,.panel>.table-bordered>tbody>tr:first-child>th,.panel>.table-bordered>thead>tr:first-child>td,.panel>.table-bordered>thead>tr:first-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>th,.panel>.table-responsive>.table-bordered>thead>tr:first-child>td,.panel>.table-responsive>.table-bordered>thead>tr:first-child>th{border-bottom:0}.panel>.table-bordered>tbody>tr:last-child>td,.panel>.table-bordered>tbody>tr:last-child>th,.panel>.table-bordered>tfoot>tr:last-child>td,.panel>.table-bordered>tfoot>tr:last-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>th,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>td,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}.panel>.table-responsive{margin-bottom:0;border:0}.panel-group{margin-bottom:20px}.panel-group .panel{margin-bottom:0;border-radius:4px}.panel-group .panel+.panel{margin-top:5px}.panel-group .panel-heading{border-bottom:0}.panel-group .panel-heading+.panel-collapse>.list-group,.panel-group .panel-heading+.panel-collapse>.panel-body{border-top:1px solid #ddd}.panel-group .panel-footer{border-top:0}.panel-group .panel-footer+.panel-collapse .panel-body{border-bottom:1px solid #ddd}.panel-default{border-color:#ddd}.panel-default>.panel-heading{color:#333;background-color:#f5f5f5;border-color:#ddd}.panel-default>.panel-heading+.panel-collapse>.panel-body{border-top-color:#ddd}.panel-default>.panel-heading .badge{color:#f5f5f5;background-color:#333}.panel-default>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#ddd}.panel-primary{border-color:#337ab7}.panel-primary>.panel-heading{color:#fff;background-color:#337ab7;border-color:#337ab7}.panel-primary>.panel-heading+.panel-collapse>.panel-body{border-top-color:#337ab7}.panel-primary>.panel-heading .badge{color:#337ab7;background-color:#fff}.panel-primary>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#337ab7}.panel-success{border-color:#d6e9c6}.panel-success>.panel-heading{color:#3c763d;background-color:#dff0d8;border-color:#d6e9c6}.panel-success>.panel-heading+.panel-collapse>.panel-body{border-top-color:#d6e9c6}.panel-success>.panel-heading .badge{color:#dff0d8;background-color:#3c763d}.panel-success>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#d6e9c6}.panel-info{border-color:#bce8f1}.panel-info>.panel-heading{color:#31708f;background-color:#d9edf7;border-color:#bce8f1}.panel-info>.panel-heading+.panel-collapse>.panel-body{border-top-color:#bce8f1}.panel-info>.panel-heading .badge{color:#d9edf7;background-color:#31708f}.panel-info>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#bce8f1}.panel-warning{border-color:#faebcc}.panel-warning>.panel-heading{color:#8a6d3b;background-color:#fcf8e3;border-color:#faebcc}.panel-warning>.panel-heading+.panel-collapse>.panel-body{border-top-color:#faebcc}.panel-warning>.panel-heading .badge{color:#fcf8e3;background-color:#8a6d3b}.panel-warning>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#faebcc}.panel-danger{border-color:#ebccd1}.panel-danger>.panel-heading{color:#a94442;background-color:#f2dede;border-color:#ebccd1}.panel-danger>.panel-heading+.panel-collapse>.panel-body{border-top-color:#ebccd1}.panel-danger>.panel-heading .badge{color:#f2dede;background-color:#a94442}.panel-danger>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#ebccd1}.embed-responsive{position:relative;display:block;height:0;padding:0;overflow:hidden}.embed-responsive .embed-responsive-item,.embed-responsive embed,.embed-responsive iframe,.embed-responsive object,.embed-responsive video{position:absolute;top:0;bottom:0;left:0;width:100%;height:100%;border:0}.embed-responsive-16by9{padding-bottom:56.25%}.embed-responsive-4by3{padding-bottom:75%}.well{min-height:20px;padding:19px;margin-bottom:20px;background-color:#f5f5f5;border:1px solid #e3e3e3;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.05);box-shadow:inset 0 1px 1px rgba(0,0,0,.05)}.well blockquote{border-color:#ddd;border-color:rgba(0,0,0,.15)}.well-lg{padding:24px;border-radius:6px}.well-sm{padding:9px;border-radius:3px}.close{float:right;font-size:21px;font-weight:700;line-height:1;color:#000;text-shadow:0 1px 0 #fff;filter:alpha(opacity=20);opacity:.2}.close:focus,.close:hover{color:#000;text-decoration:none;cursor:pointer;filter:alpha(opacity=50);opacity:.5}button.close{-webkit-appearance:none;padding:0;cursor:pointer;background:0 0;border:0}.modal-open{overflow:hidden}.modal{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1050;display:none;overflow:hidden;-webkit-overflow-scrolling:touch;outline:0}.modal.fade .modal-dialog{-webkit-transition:-webkit-transform .3s ease-out;-o-transition:-o-transform .3s ease-out;transition:transform .3s ease-out;-webkit-transform:translate(0,-25%);-ms-transform:translate(0,-25%);-o-transform:translate(0,-25%);transform:translate(0,-25%)}.modal.in .modal-dialog{-webkit-transform:translate(0,0);-ms-transform:translate(0,0);-o-transform:translate(0,0);transform:translate(0,0)}.modal-open .modal{overflow-x:hidden;overflow-y:auto}.modal-dialog{position:relative;width:auto;margin:10px}.modal-content{position:relative;background-color:#fff;-webkit-background-clip:padding-box;background-clip:padding-box;border:1px solid #999;border:1px solid rgba(0,0,0,.2);border-radius:6px;outline:0;-webkit-box-shadow:0 3px 9px rgba(0,0,0,.5);box-shadow:0 3px 9px rgba(0,0,0,.5)}.modal-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1040;background-color:#000}.modal-backdrop.fade{filter:alpha(opacity=0);opacity:0}.modal-backdrop.in{filter:alpha(opacity=50);opacity:.5}.modal-header{padding:15px;border-bottom:1px solid #e5e5e5}.modal-header .close{margin-top:-2px}.modal-title{margin:0;line-height:1.42857143}.modal-body{position:relative;padding:15px}.modal-footer{padding:15px;text-align:right;border-top:1px solid #e5e5e5}.modal-footer .btn+.btn{margin-bottom:0;margin-left:5px}.modal-footer .btn-group .btn+.btn{margin-left:-1px}.modal-footer .btn-block+.btn-block{margin-left:0}.modal-scrollbar-measure{position:absolute;top:-9999px;width:50px;height:50px;overflow:scroll}@media (min-width:768px){.modal-dialog{width:600px;margin:30px auto}.modal-content{-webkit-box-shadow:0 5px 15px rgba(0,0,0,.5);box-shadow:0 5px 15px rgba(0,0,0,.5)}.modal-sm{width:300px}}@media (min-width:992px){.modal-lg{width:900px}}.tooltip{position:absolute;z-index:1070;display:block;font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-size:12px;font-style:normal;font-weight:400;line-height:1.42857143;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;word-spacing:normal;word-wrap:normal;white-space:normal;filter:alpha(opacity=0);opacity:0;line-break:auto}.tooltip.in{filter:alpha(opacity=90);opacity:.9}.tooltip.top{padding:5px 0;margin-top:-3px}.tooltip.right{padding:0 5px;margin-left:3px}.tooltip.bottom{padding:5px 0;margin-top:3px}.tooltip.left{padding:0 5px;margin-left:-3px}.tooltip-inner{max-width:200px;padding:3px 8px;color:#fff;text-align:center;background-color:#000;border-radius:4px}.tooltip-arrow{position:absolute;width:0;height:0;border-color:transparent;border-style:solid}.tooltip.top .tooltip-arrow{bottom:0;left:50%;margin-left:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-left .tooltip-arrow{right:5px;bottom:0;margin-bottom:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-right .tooltip-arrow{bottom:0;left:5px;margin-bottom:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.right .tooltip-arrow{top:50%;left:0;margin-top:-5px;border-width:5px 5px 5px 0;border-right-color:#000}.tooltip.left .tooltip-arrow{top:50%;right:0;margin-top:-5px;border-width:5px 0 5px 5px;border-left-color:#000}.tooltip.bottom .tooltip-arrow{top:0;left:50%;margin-left:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-left .tooltip-arrow{top:0;right:5px;margin-top:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-right .tooltip-arrow{top:0;left:5px;margin-top:-5px;border-width:0 5px 5px;border-bottom-color:#000}.popover{position:absolute;top:0;left:0;z-index:1060;display:none;max-width:276px;padding:1px;font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-size:14px;font-style:normal;font-weight:400;line-height:1.42857143;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;word-spacing:normal;word-wrap:normal;white-space:normal;background-color:#fff;-webkit-background-clip:padding-box;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.2);border-radius:6px;-webkit-box-shadow:0 5px 10px rgba(0,0,0,.2);box-shadow:0 5px 10px rgba(0,0,0,.2);line-break:auto}.popover.top{margin-top:-10px}.popover.right{margin-left:10px}.popover.bottom{margin-top:10px}.popover.left{margin-left:-10px}.popover-title{padding:8px 14px;margin:0;font-size:14px;background-color:#f7f7f7;border-bottom:1px solid #ebebeb;border-radius:5px 5px 0 0}.popover-content{padding:9px 14px}.popover>.arrow,.popover>.arrow:after{position:absolute;display:block;width:0;height:0;border-color:transparent;border-style:solid}.popover>.arrow{border-width:11px}.popover>.arrow:after{content:"";border-width:10px}.popover.top>.arrow{bottom:-11px;left:50%;margin-left:-11px;border-top-color:#999;border-top-color:rgba(0,0,0,.25);border-bottom-width:0}.popover.top>.arrow:after{bottom:1px;margin-left:-10px;content:" ";border-top-color:#fff;border-bottom-width:0}.popover.right>.arrow{top:50%;left:-11px;margin-top:-11px;border-right-color:#999;border-right-color:rgba(0,0,0,.25);border-left-width:0}.popover.right>.arrow:after{bottom:-10px;left:1px;content:" ";border-right-color:#fff;border-left-width:0}.popover.bottom>.arrow{top:-11px;left:50%;margin-left:-11px;border-top-width:0;border-bottom-color:#999;border-bottom-color:rgba(0,0,0,.25)}.popover.bottom>.arrow:after{top:1px;margin-left:-10px;content:" ";border-top-width:0;border-bottom-color:#fff}.popover.left>.arrow{top:50%;right:-11px;margin-top:-11px;border-right-width:0;border-left-color:#999;border-left-color:rgba(0,0,0,.25)}.popover.left>.arrow:after{right:1px;bottom:-10px;content:" ";border-right-width:0;border-left-color:#fff}.carousel{position:relative}.carousel-inner{position:relative;width:100%;overflow:hidden}.carousel-inner>.item{position:relative;display:none;-webkit-transition:.6s ease-in-out left;-o-transition:.6s ease-in-out left;transition:.6s ease-in-out left}.carousel-inner>.item>a>img,.carousel-inner>.item>img{line-height:1}@media all and (transform-3d),(-webkit-transform-3d){.carousel-inner>.item{-webkit-transition:-webkit-transform .6s ease-in-out;-o-transition:-o-transform .6s ease-in-out;transition:transform .6s ease-in-out;-webkit-backface-visibility:hidden;backface-visibility:hidden;-webkit-perspective:1000px;perspective:1000px}.carousel-inner>.item.active.right,.carousel-inner>.item.next{left:0;-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0)}.carousel-inner>.item.active.left,.carousel-inner>.item.prev{left:0;-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0)}.carousel-inner>.item.active,.carousel-inner>.item.next.left,.carousel-inner>.item.prev.right{left:0;-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}}.carousel-inner>.active,.carousel-inner>.next,.carousel-inner>.prev{display:block}.carousel-inner>.active{left:0}.carousel-inner>.next,.carousel-inner>.prev{position:absolute;top:0;width:100%}.carousel-inner>.next{left:100%}.carousel-inner>.prev{left:-100%}.carousel-inner>.next.left,.carousel-inner>.prev.right{left:0}.carousel-inner>.active.left{left:-100%}.carousel-inner>.active.right{left:100%}.carousel-control{position:absolute;top:0;bottom:0;left:0;width:15%;font-size:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6);background-color:rgba(0,0,0,0);filter:alpha(opacity=50);opacity:.5}.carousel-control.left{background-image:-webkit-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:-webkit-gradient(linear,left top,right top,from(rgba(0,0,0,.5)),to(rgba(0,0,0,.0001)));background-image:linear-gradient(to right,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);background-repeat:repeat-x}.carousel-control.right{right:0;left:auto;background-image:-webkit-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:-webkit-gradient(linear,left top,right top,from(rgba(0,0,0,.0001)),to(rgba(0,0,0,.5)));background-image:linear-gradient(to right,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);background-repeat:repeat-x}.carousel-control:focus,.carousel-control:hover{color:#fff;text-decoration:none;filter:alpha(opacity=90);outline:0;opacity:.9}.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next,.carousel-control .icon-prev{position:absolute;top:50%;z-index:5;display:inline-block;margin-top:-10px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{left:50%;margin-left:-10px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{right:50%;margin-right:-10px}.carousel-control .icon-next,.carousel-control .icon-prev{width:20px;height:20px;font-family:serif;line-height:1}.carousel-control .icon-prev:before{content:'\2039'}.carousel-control .icon-next:before{content:'\203a'}.carousel-indicators{position:absolute;bottom:10px;left:50%;z-index:15;width:60%;padding-left:0;margin-left:-30%;text-align:center;list-style:none}.carousel-indicators li{display:inline-block;width:10px;height:10px;margin:1px;text-indent:-999px;cursor:pointer;background-color:#000\9;background-color:rgba(0,0,0,0);border:1px solid #fff;border-radius:10px}.carousel-indicators .active{width:12px;height:12px;margin:0;background-color:#fff}.carousel-caption{position:absolute;right:15%;bottom:20px;left:15%;z-index:10;padding-top:20px;padding-bottom:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6)}.carousel-caption .btn{text-shadow:none}@media screen and (min-width:768px){.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next,.carousel-control .icon-prev{width:30px;height:30px;margin-top:-10px;font-size:30px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{margin-left:-10px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{margin-right:-10px}.carousel-caption{right:20%;left:20%;padding-bottom:30px}.carousel-indicators{bottom:20px}}.btn-group-vertical>.btn-group:after,.btn-group-vertical>.btn-group:before,.btn-toolbar:after,.btn-toolbar:before,.clearfix:after,.clearfix:before,.container-fluid:after,.container-fluid:before,.container:after,.container:before,.dl-horizontal dd:after,.dl-horizontal dd:before,.form-horizontal .form-group:after,.form-horizontal .form-group:before,.modal-footer:after,.modal-footer:before,.modal-header:after,.modal-header:before,.nav:after,.nav:before,.navbar-collapse:after,.navbar-collapse:before,.navbar-header:after,.navbar-header:before,.navbar:after,.navbar:before,.pager:after,.pager:before,.panel-body:after,.panel-body:before,.row:after,.row:before{display:table;content:" "}.btn-group-vertical>.btn-group:after,.btn-toolbar:after,.clearfix:after,.container-fluid:after,.container:after,.dl-horizontal dd:after,.form-horizontal .form-group:after,.modal-footer:after,.modal-header:after,.nav:after,.navbar-collapse:after,.navbar-header:after,.navbar:after,.pager:after,.panel-body:after,.row:after{clear:both}.center-block{display:block;margin-right:auto;margin-left:auto}.pull-right{float:right!important}.pull-left{float:left!important}.hide{display:none!important}.show{display:block!important}.invisible{visibility:hidden}.text-hide{font:0/0 a;color:transparent;text-shadow:none;background-color:transparent;border:0}.hidden{display:none!important}.affix{position:fixed}@-ms-viewport{width:device-width}.visible-lg,.visible-md,.visible-sm,.visible-xs{display:none!important}.visible-lg-block,.visible-lg-inline,.visible-lg-inline-block,.visible-md-block,.visible-md-inline,.visible-md-inline-block,.visible-sm-block,.visible-sm-inline,.visible-sm-inline-block,.visible-xs-block,.visible-xs-inline,.visible-xs-inline-block{display:none!important}@media (max-width:767px){.visible-xs{display:block!important}table.visible-xs{display:table!important}tr.visible-xs{display:table-row!important}td.visible-xs,th.visible-xs{display:table-cell!important}}@media (max-width:767px){.visible-xs-block{display:block!important}}@media (max-width:767px){.visible-xs-inline{display:inline!important}}@media (max-width:767px){.visible-xs-inline-block{display:inline-block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm{display:block!important}table.visible-sm{display:table!important}tr.visible-sm{display:table-row!important}td.visible-sm,th.visible-sm{display:table-cell!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-block{display:block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline{display:inline!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline-block{display:inline-block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md{display:block!important}table.visible-md{display:table!important}tr.visible-md{display:table-row!important}td.visible-md,th.visible-md{display:table-cell!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-block{display:block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline{display:inline!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline-block{display:inline-block!important}}@media (min-width:1200px){.visible-lg{display:block!important}table.visible-lg{display:table!important}tr.visible-lg{display:table-row!important}td.visible-lg,th.visible-lg{display:table-cell!important}}@media (min-width:1200px){.visible-lg-block{display:block!important}}@media (min-width:1200px){.visible-lg-inline{display:inline!important}}@media (min-width:1200px){.visible-lg-inline-block{display:inline-block!important}}@media (max-width:767px){.hidden-xs{display:none!important}}@media (min-width:768px) and (max-width:991px){.hidden-sm{display:none!important}}@media (min-width:992px) and (max-width:1199px){.hidden-md{display:none!important}}@media (min-width:1200px){.hidden-lg{display:none!important}}.visible-print{display:none!important}@media print{.visible-print{display:block!important}table.visible-print{display:table!important}tr.visible-print{display:table-row!important}td.visible-print,th.visible-print{display:table-cell!important}}.visible-print-block{display:none!important}@media print{.visible-print-block{display:block!important}}.visible-print-inline{display:none!important}@media print{.visible-print-inline{display:inline!important}}.visible-print-inline-block{display:none!important}@media print{.visible-print-inline-block{display:inline-block!important}}@media print{.hidden-print{display:none!important}}
 /*# sourceMappingURL=bootstrap.min.css.map */
```

### Comparing `matlab-proxy-0.5.8/gui/public/favicon.ico` & `matlab-proxy-0.5.9/gui/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/actionCreators/actionCreators.spec.js` & `matlab-proxy-0.5.9/gui/src/actionCreators/actionCreators.spec.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -34,14 +34,30 @@
         y: 12
     }],
     [actionCreators.setTriggerPosition, [52, 112], {
         type: actions.SET_TRIGGER_POSITION,
         x: 52,
         y: 112
     }],
+    [actionCreators.setAuthStatus, [true], {
+        type: actions.SET_AUTH_STATUS,
+        authInfo: true
+    }],
+    [actionCreators.setAuthStatus, [false], {
+        type: actions.SET_AUTH_STATUS,
+        authInfo: false
+    }],
+    [actionCreators.setAuthToken, ['string'], {
+        type: actions.SET_AUTH_TOKEN,
+        authInfo: 'string'
+    }],
+    [actionCreators.setAuthToken, [null], {
+        type: actions.SET_AUTH_TOKEN,
+        authInfo: null
+    }]
 ])('Test Set actionCreators', (method, input, expectedAction) => {
     test(`check if an action of type  ${expectedAction.type} is returned when method actionCreator.${method.name}() is called`, () => {
         expect(method(...input)).toEqual(expectedAction);
     });
 });
 
 
@@ -136,14 +152,19 @@
                 hasFetched: false,
                 fetchFailCount: 0,
                 licensingInfo: {
                     type: 'NLM',
                     connectionString: 'abc@nlm',
                 }
             },
+            authInfo: {
+                authEnabled: false,
+                authStatus: false,
+                authToken: null,
+            }
         });
 
         const status = {
             matlab: {
                 status: 'up',
             },
             licensing: {
@@ -253,21 +274,64 @@
                     connectionString: 'abc@nlm',
                 },
                 isFetching: false,
                 isSubmitting: false,
                 hasFetched: false,
                 fetchFailCount: 0,
             },
+            authInfo: {
+                authEnabled: false,
+                authStatus: false,
+                authToken: null,
+            },
         });
     });
 
     afterEach(() => {
         fetchMock.restore();
     });
 
+    it('dispatches SET_AUTH_STATUS when fetching auth info and not authorised', () => {
+        let token = 'token'
+        fetchMock.once('/authenticate_request', {
+            body: {
+                authStatus: false,
+                error: {
+                    message: "Token invalid. Please enter a valid token to authenticate",
+                    type: "invalidToken",
+                    logs: null,
+                }
+            }
+        });
+        const expectedActions = [actions.SET_AUTH_STATUS, actions.SET_AUTH_TOKEN];
+
+        return store.dispatch(actionCreators.updateAuthStatus(token)).then(() => {
+            const received = store.getActions();
+            expect(received.map((a) => a.type)).toEqual(expectedActions);
+        });
+    });
+
+    it('dispatches SET_AUTH_STATUS, when fetching auth info and authorised', () => {
+        let token = 'token'
+        fetchMock.once('/authenticate_request', {
+            body: {
+                authStatus: true,
+                error: null
+            }
+        });
+        const expectedActions = [actions.SET_AUTH_STATUS, actions.SET_AUTH_TOKEN];
+
+        return store.dispatch(actionCreators.updateAuthStatus(token)).then(() => {
+            const received = store.getActions();
+            expect(received.map((a) => a.type)).toEqual(expectedActions);
+        });
+    });
+
+
+
     it('dispatches REQUEST_SERVER_STATUS, RECEIVE_SERVER_STATUS when fetching status', () => {
         fetchMock.getOnce('/get_status', {
             body: {
                 matlab: {
                     status: 'down',
                 },
                 licensing: {},
```

### Comparing `matlab-proxy-0.5.8/gui/src/actionCreators/index.js` & `matlab-proxy-0.5.9/gui/src/actionCreators/index.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -13,19 +13,35 @@
     REQUEST_ENV_CONFIG,
     RECEIVE_SET_LICENSING,
     RECEIVE_TERMINATE_INTEGRATION,
     RECEIVE_STOP_MATLAB,
     RECEIVE_START_MATLAB,
     RECEIVE_ERROR,
     RECEIVE_ENV_CONFIG,
+    SET_AUTH_STATUS,
+    SET_AUTH_TOKEN
 } from '../actions';
 import {
     selectMatlabPending
 } from '../selectors';
 
+export function setAuthStatus(authInfo) {
+    return {
+        type: SET_AUTH_STATUS,
+        authInfo
+    }
+}
+
+export function setAuthToken(authInfo) {
+    return {
+        type: SET_AUTH_TOKEN,
+        authInfo
+    }
+}
+
 export function setTriggerPosition(x, y) {
     return {
         type: SET_TRIGGER_POSITION,
         x,
         y
     };
 }
@@ -158,37 +174,54 @@
             dispatch(receiveError(`HTTP Error 408 - Request Timeout. ${errorText}`, 408))
         } else {
             dispatch(receiveError("Communication with server failed.", 500))
         }
     }
 }
 
-
 export function fetchServerStatus() {
     return async function(dispatch, getState) {
 
         dispatch(requestServerStatus());
-        const response = await fetchWithTimeout(dispatch, './get_status', {}, 10000)
+        const response = await fetchWithTimeout(dispatch, './get_status', {}, 10000);
         const data = await response.json();
         dispatch(receiveServerStatus(data));
 
     }
 }
 
 export function fetchEnvConfig() {
     return async function(dispatch, getState) {
 
         dispatch(requestEnvConfig());
         const response = await fetchWithTimeout(dispatch, './get_env_config', {}, 10000);
         const data = await response.json();
         dispatch(receiveEnvConfig(data));
-
     };
 }
 
+export function updateAuthStatus(token) {
+    // make response consistent with rest of reducers (data)
+    return async function(dispatch, getState) {
+
+        const options = {
+            method: 'POST',
+            headers: {
+                'Accept': 'application/text',
+                'Content-Type': 'application/text'
+            },
+            body: token
+        };
+        const response = await fetchWithTimeout(dispatch, './authenticate_request', options, 15000);
+        const data = await response.json()
+
+        dispatch(setAuthStatus(data))
+        dispatch(setAuthToken(data))
+    }
+}
 
 export function fetchSetLicensing(info) {
     return async function(dispatch, getState) {
 
         const options = {
             method: 'PUT',
             mode: 'same-origin',
```

### Comparing `matlab-proxy-0.5.8/gui/src/actions/index.js` & `matlab-proxy-0.5.9/gui/src/actions/index.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -11,8 +11,10 @@
 export const REQUEST_START_MATLAB = 'REQUEST_START_MATLAB';
 export const RECEIVE_SET_LICENSING = 'RECEIVE_SET_LICENSING';
 export const RECEIVE_TERMINATE_INTEGRATION = 'RECEIVE_TERMINATE_INTEGRATION';
 export const RECEIVE_STOP_MATLAB = 'RECEIVE_STOP_MATLAB';
 export const RECEIVE_START_MATLAB = 'RECEIVE_START_MATLAB';
 export const RECEIVE_ERROR = 'RECEIVE_ERROR';
 export const REQUEST_ENV_CONFIG = 'REQUEST_ENV_CONFIG';
-export const RECEIVE_ENV_CONFIG = 'RECEIVE_ENV_CONFIG';
+export const RECEIVE_ENV_CONFIG = 'RECEIVE_ENV_CONFIG';
+export const SET_AUTH_STATUS = 'SET_AUTH_STATUS';
+export const SET_AUTH_TOKEN = 'SET_AUTH_TOKEN';
```

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/css/site7.min.css` & `matlab-proxy-0.5.9/gui/src/components/App/3p/css/site7.min.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot` & `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg` & `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf` & `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff` & `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2` & `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks-eps.svg` & `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-eps.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks-eps.ttf` & `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-eps.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks-eps.woff` & `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-eps.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks-pictograms.svg` & `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-pictograms.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf` & `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks-pictograms.woff` & `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-pictograms.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks.svg` & `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks.ttf` & `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/fonts/mathworks.woff` & `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/images/bug_reports/workaround.gif` & `matlab-proxy-0.5.9/gui/src/components/App/3p/images/bug_reports/workaround.gif`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg` & `matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg` & `matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg` & `matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg` & `matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/3p/images/responsive/global/ico-sprite.png` & `matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-sprite.png`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/App.css` & `matlab-proxy-0.5.9/gui/src/components/App/App.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/App.spec.js` & `matlab-proxy-0.5.9/gui/src/components/Information/Information.spec.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,228 +1,245 @@
 // Copyright (c) 2020-2022 The MathWorks, Inc.
 
 import React from 'react';
+import Information from './index';
+import App from '../App';
 import {
     render,
     fireEvent,
-    within
+    getByTestId
 } from '../../test/utils/react-test';
-import App from './index';
-import OverlayTrigger from '../OverlayTrigger';
 
-describe('App Component', () => {
-    let initialState;
-    beforeEach(() => {
-        initialState = {
-            triggerPosition: {
-                x: 539,
-                y: 0
-            },
-            tutorialHidden: false,
-            overlayVisibility: false,
-            serverStatus: {
-                licensingInfo: {
-                    type: 'MHLM',
-                    emailAddress: 'abc@mathworks.com'
-                },
-                matlabStatus: 'up',
-                matlabVersion: 'R2020b',
-                isFetching: false,
-                hasFetched: true,
-                isSubmitting: false,
-                fetchFailCount: 0,
-                wsEnv: 'mw'
-            },
-            loadUrl: null,
-            error: null,
-        };
-        const mockIntersectionObserver = jest.fn();
-        mockIntersectionObserver.mockReturnValue({
-            observe: () => null,
-            disconnect: () => null,
-        });
-
-        window.IntersectionObserver = mockIntersectionObserver;
-    });
-
-    afterEach(() => {
-        jest.clearAllMocks();
-    });
-
-    // it('renders app without crashing', () => {
-    //   const { getByTestId } = render(<App />);
-    //   expect(getByTestId('app')).toBeInTheDocument();
-    // });
-
-    it('should render overlayTrigger (after closing the tutorial)', () => {
-
-        // Hide the tutorial before rendering the component.
-        initialState.tutorialHidden = true;
-
-        const {
-            getByTestId
-        } = render( < App / > , {
-            initialState: initialState,
-        });
-
-        //grab the overlayTrigger
-        const overlayTriggerComponent = getByTestId(
-            'overlayTrigger'
-        );
-
-        expect(overlayTriggerComponent).toBeInTheDocument();
-    });
-
-    it('should render LicensingGatherer component within the App component when no licensing is provided', () => {
-
-        //Set lincensingInfo to empty object.
-        initialState.serverStatus.licensingInfo = {};
-        initialState.overlayVisibility = true;
-
-        const {
-            getByRole
-        } = render( < App / > , {
-            initialState: initialState,
-        });
-
-        const licensingGathererComponent = getByRole(
-            'document'
-        );
-        expect(licensingGathererComponent).toBeInTheDocument();
-    });
-
-    it('should render Information Component within App Component after licensing is provided', () => {
-
-        // Hide the tutorial and make the overlay visible.
-        initialState.tutorialHidden = true;
-        initialState.overlayVisibility = true;
-
-        //Rendering the App component with the above changes to the initial
-        // state should render the Information Component.
-        const {
-            getByRole
-        } = render( < App / > , {
-            initialState: initialState,
-        });
-
-        const informationComponent = getByRole('document');
-        expect(informationComponent).toBeInTheDocument();
-    });
-
-    it('should display integration terminated error', () => {
-
-        //Hide the tutorial, make the overlay visible and set fetchFailCount to 10
-        initialState.tutorialHidden = true;
-        initialState.overlayVisibility = true;
-        initialState.serverStatus.fetchFailCount = 10;
-
-        //Rendering the App component with above changes to the initial state
-        // will terminate the integration.
-        const {
-            container
-        } = render( < App / > , {
-            initialState: initialState,
-        });
-
-
-        const paragraphElements = [...container.getElementsByTagName('p')];
-
-
-        expect(
-            paragraphElements.some((p) =>
-                p.textContent.includes('integration terminated')
-            )
-        ).toBe(true);
-    });
-
-    it('should display MatlabInstallError', () => {
-        initialState.error = {
-            type: 'MatlabInstallError',
-            message: 'Matlab Installation error. Exited with status code -9',
-        };
-        initialState.serverStatus.licensingInfo = {};
-        initialState.overlayVisibility = true;
-
-        const {
-            container
-        } = render( < App / > , {
-            initialState: initialState,
-        });
-
-        const paragraphElements = [...container.getElementsByTagName('p')];
-
-        expect(
-            paragraphElements.some((p) =>
-                p.textContent.includes(initialState.error.message)
-            )
-        ).toBe(true);
-    });
-
-    it('should display Confirmation component ', () => {
-
-        //Hide the tutorial and make the overlay visible
-        initialState.tutorialHidden = true;
-        initialState.overlayVisibility = true;
-
-        const {
-            getByTestId,
-            container
-        } = render( < App / > , {
-            initialState: initialState,
-        });
-
-
-        const startMatlabBtn = getByTestId('startMatlabBtn');
-
-        fireEvent.click(startMatlabBtn);
-
-        const confirmMatlabRestart = container
-            .getElementsByClassName('modal-body')
-            .item(0);
-
-        expect(confirmMatlabRestart.textContent).toMatch('restart MATLAB?');
-
-        const confirmBtn = getByTestId('confirmButton');
-        expect(confirmBtn).toBeInTheDocument();
-    });
-
-    it('should display Help Component', () => {
-
-        //Hide the tutorial and make the overlay visible
-        initialState.tutorialHidden = true;
-        initialState.overlayVisibility = true;
-
-        const {
-            getByTestId,
-            container,
-            getByRole
-        } = render( < App / > , {
-            initialState: initialState,
-        });
-
-
-        // Grab the help button and click it.
-        const helpBtn = getByTestId('helpBtn');
-        fireEvent.click(helpBtn);
-
-        const helpElement = container.querySelector('#confirmation-dialog-title');
-
-        expect(helpElement.textContent).toMatch('Help');
-    });
-
-    it('should set the window location from state', () => {
-        initialState.loadUrl = 'http://localhost.com:5555';
-        const hrefMock = jest.fn();
-        delete window.location;
-
-        window.location = {
-            href: hrefMock
-        }
-        const {
-            debug
-        } = render( < App / > , {
-            initialState: initialState
-        });
-
-        expect(window.location.href).toMatch('localhost');
-    });
-});
+describe('Information Component', () => {
+            let closeHandler, children, initialState;
+            beforeEach(() => {
+                children = ( <
+                    div data - testid = "child" >
+                    Child1 <
+                    /div>
+                );
+                closeHandler = jest.fn().mockImplementation(() => {});
+
+                initialState = {
+                    triggerPosition: {
+                        x: 539,
+                        y: 0
+                    },
+                    tutorialHidden: false,
+                    overlayVisibility: false,
+                    serverStatus: {
+                        licensingInfo: {
+                            type: 'MHLM',
+                            emailAddress: 'abc@mathworks.com'
+                        },
+                        matlabStatus: 'up',
+                        matlabVersion: 'R2020b',
+                        isFetching: false,
+                        hasFetched: true,
+                        isSubmitting: false,
+                        fetchFailCount: 0,
+                    },
+                    loadUrl: null,
+                    error: null,
+                    authInfo: {
+                        authEnabled: false,
+                        authStatus: false,
+                        authToken: null,
+                    },
+                };
+
+                const mockIntersectionObserver = jest.fn();
+                mockIntersectionObserver.mockReturnValue({
+                    observe: () => null,
+                    disconnect: () => null,
+                });
+
+                window.IntersectionObserver = mockIntersectionObserver;
+
+            });
+            afterEach(() => {
+                jest.clearAllMocks();
+            });
+
+            it('should throw console.error when rendered without closeHandler prop', () => {
+                const errorMock = jest.spyOn(console, 'error').mockImplementation(() => {});
+
+                render( < Information / > );
+
+                expect(errorMock).toHaveBeenCalledTimes(1);
+            });
+
+            it('should render without crashing', () => {
+                    render( < Information closeHandler = {
+                            closeHandler
+                        }
+                        />);
+                    });
+
+                it('should render child nodes passed to it without crashing', () => {
+                    const {
+                        getByTestId
+                    } = render( <
+                        Information closeHandler = {
+                            closeHandler
+                        }
+                        children = {
+                            children
+                        }
+                        />
+                    );
+
+                    expect(getByTestId('child')).toBeInTheDocument();
+                });
+
+                it('should render Online Licensing info with licensing type MHLM', () => {
+                    const {
+                        container,
+                        debug,
+                        getByText
+                    } = render( <
+                        Information closeHandler = {
+                            closeHandler
+                        }
+                        children = {
+                            children
+                        }
+                        />, {
+                            initialState: initialState
+                        }
+                    );
+
+                    const licensingInfo = getByText('Licensing:');
+
+                    expect(licensingInfo.nextSibling.textContent).toContain(
+                        initialState.serverStatus.licensingInfo.emailAddress
+                    );
+                });
+
+                it('should render Online Licensing info with licensing type NLM', () => {
+                    initialState.serverStatus.licensingInfo = {
+                        type: 'NLM',
+                        connectionString: 'abc@nlm',
+                    };
+                    const {
+                        container,
+                        debug,
+                        getByText
+                    } = render( <
+                        Information closeHandler = {
+                            closeHandler
+                        }
+                        children = {
+                            children
+                        }
+                        />, {
+                            initialState: initialState
+                        }
+                    );
+
+                    const licensingInfo = getByText('Licensing:');
+
+                    expect(licensingInfo.nextSibling.textContent).toContain(
+                        initialState.serverStatus.licensingInfo.connectionString
+                    );
+                });
+
+                it('should display errors', () => {
+                    initialState.error = {
+                        message: 'Exited with exit code -9',
+                        logs: [
+                            'Matlab exited with exit code -9',
+                            'Check matlab logs for more details',
+                        ],
+                    };
+
+                    const {
+                        container
+                    } = render( <
+                        Information closeHandler = {
+                            closeHandler
+                        }
+                        children = {
+                            children
+                        }
+                        />, {
+                            initialState: initialState
+                        }
+                    );
+
+                    const errorContent = container.getElementsByClassName('error-msg').item(0)
+                        .textContent;
+
+                    expect(errorContent).toEqual(initialState.error.logs.join('\n').trim());
+                });
+
+                // it('should close overlay on button click', () => {
+                //   const { debug, container } = render(
+                //     <Information closeHandler={closeHandler} children={children} />,
+                //     { initialState: initialState }
+                //   );
+
+                //   const closeBtn = container.getElementsByClassName('close').item(0);
+
+                //   fireEvent.click(closeBtn);
+                // });
+
+
+                it('should close the Information Component and display the overlayTrigger when close button is clicked', () => {
+
+                    // Hide the tutorial and make the overlay visible.
+                    initialState.tutorialHidden = true;
+                    initialState.overlayVisibility = true;
+                    initialState.authInfo.authEnabled = true;
+                    initialState.authInfo.authStatus = true;
+
+                    //Rendering the App component with the above changes to the initial
+                    // state should render the Information Component.
+                    const {
+                        getByTestId,
+                        debug,
+                        container
+                    } = render( < App / > , {
+                        initialState: initialState,
+                    });
+
+                    const informationComponent = container.querySelector('#information');
+
+                    //Check if information dialog is displayed
+                    expect(informationComponent).toBeInTheDocument();
+
+                    // grab and click on the close button of information dialog
+                    const closeBtn = container.getElementsByClassName('close').item(0);
+                    fireEvent.click(closeBtn);
+
+                    const overlayTriggerComponent = getByTestId('overlayTrigger');
+
+                    // Check if information dialog is not displayed and overlay trigger is displayed.
+                    expect(informationComponent).not.toBeInTheDocument();
+                    expect(overlayTriggerComponent).toBeInTheDocument();
+
+                });
+
+
+                it('should call the closeHandler callback when the modal is clicked', () => {
+                    initialState.authInfo.authEnabled = true;
+                    initialState.authInfo.authStatus = true;
+                    const {
+                        getByRole
+                    } = render( <
+                        Information closeHandler = {
+                            closeHandler
+                        }
+                        children = {
+                            children
+                        }
+                        />, {
+                            initialState: initialState
+                        }
+                    );
+
+                    const modal = getByRole('dialog');
+                    fireEvent.click(modal);
+
+                    expect(closeHandler).toHaveBeenCalledTimes(1);
+                });
+            });
```

### Comparing `matlab-proxy-0.5.8/gui/src/components/App/index.js` & `matlab-proxy-0.5.9/gui/src/components/App/index.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,14 @@
 // Copyright (c) 2020-2022 The MathWorks, Inc.
 
 import React, {
     useState,
     useCallback,
-    useEffect
+    useEffect,
+    useMemo
 } from 'react';
 import {
     useSelector,
     useDispatch
 } from 'react-redux';
 import {
     useInterval
@@ -28,33 +29,44 @@
     selectHasFetchedServerStatus,
     selectLicensingProvided,
     selectMatlabUp,
     selectError,
     selectLoadUrl,
     selectIsConnectionError,
     selectHasFetchedEnvConfig,
+    selectAuthEnabled,
+    selectIsAuthenticated,
 } from '../../selectors';
 import {
     setOverlayVisibility,
     fetchServerStatus,
     fetchEnvConfig,
+    updateAuthStatus,
 } from '../../actionCreators';
+import blurredBackground from './MATLAB-env-blur.png';
 
 function App() {
     const dispatch = useDispatch();
 
     const overlayVisible = useSelector(selectOverlayVisible);
     const fetchStatusPeriod = useSelector(selectFetchStatusPeriod);
     const hasFetchedServerStatus = useSelector(selectHasFetchedServerStatus);
     const hasFetchedEnvConfig = useSelector(selectHasFetchedEnvConfig);
     const licensingProvided = useSelector(selectLicensingProvided);
     const matlabUp = useSelector(selectMatlabUp);
     const error = useSelector(selectError);
     const loadUrl = useSelector(selectLoadUrl);
     const isConnectionError = useSelector(selectIsConnectionError);
+    const isAuthenticated = useSelector(selectIsAuthenticated)
+    const authEnabled = useSelector(selectAuthEnabled);
+
+    const baseUrl = useMemo(() => {
+        const url = document.URL
+        return url.split(window.location.origin)[1].split('index.html')[0]
+    }, [])
 
     const toggleOverlayVisible = useCallback(
         () => dispatch(setOverlayVisibility(!overlayVisible)),
         [overlayVisible, dispatch]
     );
 
     const [dialogModel, setDialogModel] = useState(null);
@@ -138,27 +150,46 @@
         // Load URL
         useEffect(() => {
             if (loadUrl !== null) {
                 window.location.href = loadUrl;
             }
         }, [loadUrl]);
 
+        useEffect(() => {
+            const url = document.URL;
+
+            if (url.includes("?mwi_auth_token=")) {
+                var token = url.split("?mwi_auth_token=")[1];
+
+                if (token) {
+                    dispatch(updateAuthStatus(token))
+                }
+                window.history.replaceState(null, '', `${baseUrl}index.html`);
+            }
+        }, [dispatch, baseUrl]);
+
         // Display one of:
         // * Confirmation
         // * Help
         // * Error
         // * License gatherer
-        // * Status
+        // * Status Information
         let overlayContent;
+
         if (dialog) {
             // TODO Inline confirmation component build
             overlayContent = dialog;
-        } else if (hasFetchedServerStatus && (!licensingProvided)) {
-            overlayContent = < LicensingGatherer / > ;
-        } else if (licensingProvided && !dialog) {
+        }
+        // Give precendence to token auth over licensing info ie. once after token auth is done, show licensing if not provided.
+        else if ((!licensingProvided) && hasFetchedServerStatus && (!authEnabled || isAuthenticated)) {
+            overlayContent = < LicensingGatherer role = "licensing"
+            aria - describedby = "license-window" / > ;
+        }
+        // in all other cases, we will either ask for the token, 
+        else if (!dialog) {
             overlayContent = ( <
                 Information closeHandler = {
                     toggleOverlayVisible
                 } >
                 <
                 Controls callback = {
                     args => setDialogModel(args)
@@ -179,30 +210,40 @@
         // is addressed, use a direct URL in development mode. Once that is
         // fixed, the request will be served by the fake MATLAB Embedded Connector
         // process in development mode
         const matlabUrl = process.env.NODE_ENV === 'development' ?
             'http://localhost:31515/index-jsd-cr.html' :
             './index-jsd-cr.html';
 
-        const matlabJsd = matlabUp ? ( <
-            MatlabJsd url = {
-                matlabUrl
-            }
-            />
-        ) : null;
+        let matlabJsd = null;
+        if (matlabUp) {
+            matlabJsd = (!authEnabled || isAuthenticated) ?
+                ( < MatlabJsd url = {
+                        matlabUrl
+                    }
+                    /> ) : < img style = {
+                        {
+                            objectFit: 'fill'
+                        }
+                    }
+                    src = {
+                        blurredBackground
+                    }
+                    alt = 'Blurred MATLAB environment' / >
+                }
 
-        const overlayTrigger = overlayVisible ? null : < OverlayTrigger / > ;
+            const overlayTrigger = overlayVisible ? null : < OverlayTrigger / > ;
 
-        return ( <
-            div data - testid = "app"
-            className = "main" > {
-                overlayTrigger
-            } {
-                matlabJsd
-            } {
-                overlay
-            } <
-            /div>
-        );
-    }
+            return ( <
+                div data - testid = "app"
+                className = "main" > {
+                    overlayTrigger
+                } {
+                    matlabJsd
+                } {
+                    overlay
+                } <
+                /div>
+            );
+        }
 
-    export default App;
+        export default App;
```

### Comparing `matlab-proxy-0.5.8/gui/src/components/Confirmation/Confirmation.spec.js` & `matlab-proxy-0.5.9/gui/src/components/Confirmation/Confirmation.spec.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -40,14 +40,19 @@
                 hasFetched: true,
                 isSubmitting: false,
                 fetchFailCount: 0,
                 wsEnv: 'mw'
             },
             loadUrl: null,
             error: null,
+            authInfo: {
+                authEnabled: false,
+                authStatus: false,
+                authToken: null,
+            },
         };
     });
 
 
     afterEach(() => {
         jest.clearAllMocks();
     });
```

### Comparing `matlab-proxy-0.5.8/gui/src/components/Confirmation/index.js` & `matlab-proxy-0.5.9/gui/src/components/Confirmation/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/Controls/Controls.css` & `matlab-proxy-0.5.9/gui/src/components/Controls/Controls.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/Controls/Controls.spec.js` & `matlab-proxy-0.5.9/gui/src/components/Controls/Controls.spec.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -29,14 +29,19 @@
                     isFetching: false,
                     hasFetched: true,
                     isSubmitting: false,
                     fetchFailCount: 0,
                 },
                 loadUrl: null,
                 error: null,
+                authInfo: {
+                    authEnabled: false,
+                    authStatus: false,
+                    authToken: null,
+                },
             };
 
             callbackFn = jest.fn().mockImplementation((confirmationType) => {});
         });
 
         afterEach(() => {
             jest.clearAllMocks();
```

### Comparing `matlab-proxy-0.5.8/gui/src/components/Controls/feedback.svg` & `matlab-proxy-0.5.9/gui/src/components/Controls/feedback.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/Controls/help.svg` & `matlab-proxy-0.5.9/gui/src/components/Controls/help.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/Controls/index.js` & `matlab-proxy-0.5.9/gui/src/components/Controls/index.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -12,15 +12,17 @@
     selectSubmittingServerStatus,
     selectLicensingIsMhlm,
     selectLicensingProvided,
     selectMatlabRunning,
     selectMatlabStarting,
     selectMatlabStopping,
     selectMatlabVersion,
-    selectError
+    selectError,
+    selectIsAuthenticated,
+    selectAuthEnabled,
 } from '../../selectors';
 import {
     fetchStartMatlab,
     fetchStopMatlab,
     fetchTerminateIntegration,
     fetchUnsetLicensing
 } from '../../actionCreators';
@@ -39,15 +41,16 @@
     const licensed = useSelector(selectLicensingProvided);
     const mhlmLicense = useSelector(selectLicensingIsMhlm);
     const matlabRunning = useSelector(selectMatlabRunning);
     const matlabStarting = useSelector(selectMatlabStarting);
     const matlabStopping = useSelector(selectMatlabStopping);
     const matlabVersion = useSelector(selectMatlabVersion);
     const error = useSelector(selectError);
-
+    const authEnabled = useSelector(selectAuthEnabled);
+    const isAuthenticated = useSelector(selectIsAuthenticated);
     //     const canTerminateIntegration = !submitting;
     const canResetLicensing = licensed && !submitting;
 
     const feedbackBody = useMemo(
         () => `%0D%0A
 Thank you for providing feedback.%0D%0A
 %0D%0A
@@ -83,15 +86,15 @@
 
     function getBtnClass(btn) {
         let cls = 'btn companion_btn ';
         if (error) {
             if ((ERROR_TYPE_MAP[btn] || []).includes(error.type)) {
                 return cls + 'btn_color_blue';
             }
-        } else if (btn === 'start') {
+        } else if (btn === 'start' && (authEnabled && !isAuthenticated)) {
             // if there's no error, then highlight the "Start" button (if visible)
             return cls + 'btn_color_blue';
         }
         return cls + 'btn_color_mediumgray';
     };
 
     return ( <
@@ -103,15 +106,15 @@
         className = {
             getBtnClass(matlabRunning ? 'restart' : 'start')
         }
         onClick = {
             () => callback(Confirmations.START)
         }
         disabled = {
-            !licensed || matlabStarting || matlabStopping
+            !licensed || matlabStarting || matlabStopping || (authEnabled && !isAuthenticated)
         }
         data -
         for = "control-button-tooltip"
         data - tip = {
             `${matlabRunning ? 'Restart' : 'Start'}  your MATLAB session`
         } >
         <
@@ -127,15 +130,15 @@
         className = {
             getBtnClass('stop')
         }
         onClick = {
             () => callback(Confirmations.STOP)
         }
         disabled = {
-            !matlabRunning
+            !matlabRunning || (authEnabled && !isAuthenticated)
         }
         data -
         for = "control-button-tooltip"
         data - tip = "Stop your MATLAB session" >
         <
         span className = 'icon-custom-stop' > < /span> <
         span className = 'btn-label' > Stop MATLAB Session < /span> <
@@ -145,15 +148,15 @@
         className = {
             getBtnClass('sign-out')
         }
         onClick = {
             () => callback(Confirmations.SIGN_OUT)
         }
         disabled = {
-            !canResetLicensing
+            !canResetLicensing || (authEnabled && !isAuthenticated)
         }
         data -
         for = "control-button-tooltip"
         data - tip = {
             mhlmLicense ? 'Sign out' : 'Unset the network license manager server address'
         } >
         <
```

### Comparing `matlab-proxy-0.5.8/gui/src/components/Controls/restart.svg` & `matlab-proxy-0.5.9/gui/src/components/Controls/restart.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/Controls/sign-out.svg` & `matlab-proxy-0.5.9/gui/src/components/Controls/sign-out.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/Controls/start.svg` & `matlab-proxy-0.5.9/gui/src/components/Controls/start.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/Controls/stop.svg` & `matlab-proxy-0.5.9/gui/src/components/Controls/stop.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/Controls/terminate.svg` & `matlab-proxy-0.5.9/gui/src/components/Controls/terminate.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/Error/Error.spec.js` & `matlab-proxy-0.5.9/gui/src/components/Error/Error.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/Error/index.js` & `matlab-proxy-0.5.9/gui/src/components/Error/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/Help/Help.spec.js` & `matlab-proxy-0.5.9/gui/src/components/Help/Help.spec.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -29,14 +29,19 @@
                         isFetching: false,
                         hasFetched: true,
                         isSubmitting: false,
                         fetchFailCount: 0,
                     },
                     loadUrl: null,
                     error: null,
+                    authInfo: {
+                        authEnabled: false,
+                        authStatus: false,
+                        authToken: null,
+                    },
                 };
             });
             afterEach(() => {
                 jest.clearAllMocks();
             });
             it('should throw console.error for not passing in prop types', () => {
                 const errorMock = jest.spyOn(console, 'error').mockImplementation(() => {});
```

### Comparing `matlab-proxy-0.5.8/gui/src/components/Help/index.js` & `matlab-proxy-0.5.9/gui/src/components/Help/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/Information/Information.css` & `matlab-proxy-0.5.9/gui/src/components/Information/Information.css`

 * *Files 19% similar despite different names*

```diff
@@ -78,14 +78,29 @@
     width: var(--spinner-size);
     height: var(--spinner-size);
     margin-right: 4px;
     animation: spin 2s linear infinite;
     float: left;
 }
 
+#icon-small {
+    margin-left: 3px;
+    float: none;
+    color: green;
+}
+
+#token{
+    width: 15ch;
+    margin-right: 1rem;
+}
+
+#token-form{
+    margin-top: 1rem;
+}
+
 @keyframes spin {
     0% {
         transform: rotate(0deg);
     }
 
     100% {
         transform: rotate(360deg);
@@ -106,8 +121,39 @@
     white-space: normal;
 }
 
 @media (min-width: 768px) {
     .modal-dialog {
         width: 700px;
     }
+}
+
+.passive-link {
+    color: #888;
+    text-decoration: underline;
+    cursor: pointer;
+}
+
+.flex-container {
+    display: flex;
+    margin-bottom: 1rem;
+    align-items: center;
+}   
+
+.flex-item-1 {
+    flex-basis: 30%;
+    padding: 0.2rem;
+    align-items: center;
+}
+
+.flex-item-2 {
+    flex-basis: 70%;
+    padding: 0.2rem;
+    align-items: center;
+}
+
+.token-btn{
+    height: 2em;
+    padding-top: 5px;
+    padding-bottom: 0.3em;
+    max-width: 10ch;
 }
```

### Comparing `matlab-proxy-0.5.8/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js` & `matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -31,14 +31,19 @@
                 hasFetched: true,
                 isSubmitting: false,
                 fetchFailCount: 0,
                 wsEnv: 'abcd',
             },
             loadUrl: null,
             error: null,
+            authInfo: {
+                authEnabled: false,
+                authStatus: false,
+                authToken: null,
+            },
         };
 
     });
 
     afterEach(() => {
         jest.clearAllMocks();
     });
```

### Comparing `matlab-proxy-0.5.8/gui/src/components/LicensingGatherer/MHLM.js` & `matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/MHLM.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/LicensingGatherer/NLM.js` & `matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/NLM.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/LicensingGatherer/index.js` & `matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/MatlabJsd/MatlabJsd.spec.js` & `matlab-proxy-0.5.9/gui/src/components/MatlabJsd/MatlabJsd.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/Overlay/Overlay.css` & `matlab-proxy-0.5.9/gui/src/components/Overlay/Overlay.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/Overlay/Overlay.spec.js` & `matlab-proxy-0.5.9/gui/src/components/Overlay/Overlay.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/Overlay/index.js` & `matlab-proxy-0.5.9/gui/src/components/Overlay/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/OverlayTrigger/OverlayTrigger.css` & `matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/OverlayTrigger.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js` & `matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -34,14 +34,19 @@
                 isFetching: false,
                 hasFetched: true,
                 isSubmitting: false,
                 fetchFailCount: 0,
             },
             loadUrl: null,
             error: null,
+            authInfo: {
+                authEnabled: false,
+                authStatus: false,
+                authToken: null,
+            },
         };
 
         const mockIntersectionObserver = jest.fn();
         mockIntersectionObserver.mockReturnValue({
             observe: () => null,
             unobserve: () => null,
             disconnect: () => null,
```

### Comparing `matlab-proxy-0.5.8/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js` & `matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/OverlayTrigger/index.js` & `matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/OverlayTrigger/trigger-error.svg` & `matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/trigger-error.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/components/OverlayTrigger/trigger-ok.svg` & `matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/trigger-ok.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/index.js` & `matlab-proxy-0.5.9/gui/src/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/logo.svg` & `matlab-proxy-0.5.9/gui/src/logo.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/reducers/index.js` & `matlab-proxy-0.5.9/gui/src/reducers/index.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -18,16 +18,58 @@
     REQUEST_ENV_CONFIG,
     RECEIVE_SET_LICENSING,
     RECEIVE_TERMINATE_INTEGRATION,
     RECEIVE_STOP_MATLAB,
     RECEIVE_START_MATLAB,
     RECEIVE_ERROR,
     RECEIVE_ENV_CONFIG,
+    SET_AUTH_STATUS,
+    SET_AUTH_TOKEN,
 } from '../actions';
 
+// Stores info on whether token authentication enabled on the backend. 
+// This is enforced by the backend.
+export function authEnabled(state = false, action) {
+    switch (action.type) {
+        case RECEIVE_ENV_CONFIG:
+            return action.config.authEnabled;
+        default:
+            return state;
+    }
+}
+
+// Stores status of token authentication.
+export function authStatus(state = false, action) {
+    switch (action.type) {
+        case RECEIVE_ENV_CONFIG:
+            return action.config.authStatus;
+        case SET_AUTH_STATUS:
+            return action.authInfo.authStatus;
+        default:
+            return state;
+    }
+}
+
+// Stores auth token
+export function authToken(state = null, action) {
+    switch (action.type) {
+        case SET_AUTH_TOKEN:
+            if (!action.authInfo.error) {
+                return action.authInfo.authToken;
+            } else {
+                return state
+            }
+        case RECEIVE_ENV_CONFIG:
+            return action.config.authToken;
+
+        default:
+            return state;
+    }
+}
+
 export function triggerPosition(state = {
     x: window.innerWidth / 2 + 27,
     y: 0
 }, action) {
     switch (action.type) {
         case SET_TRIGGER_POSITION:
             return {
@@ -195,14 +237,26 @@
         default:
             return state;
     }
 }
 
 export function error(state = null, action) {
     switch (action.type) {
+        case SET_AUTH_STATUS:
+            if (action?.authInfo?.error !== null) {
+                const {
+                    message,
+                    type
+                } = action.authInfo.error
+                return {
+                    message: message,
+                    type: type,
+                    logs: null
+                }
+            } else return null;
         case RECEIVE_ERROR:
             return {
                 message: action.error,
                     statusCode: action?.statusCode,
                     logs: null
             };
         case RECEIVE_SERVER_STATUS:
@@ -219,33 +273,46 @@
             return state;
     }
 }
 
 export function envConfig(state = null, action) {
     switch (action.type) {
         case RECEIVE_ENV_CONFIG:
-            return action.config;
+            // Token authentication info is also sent as a response to /get_env_config endpoint.
+            // As its already stored in 'authStatus', 'authEnabled' and 'authToken', ignoring it in envConfig.
+            const {
+                authStatus, authEnabled, authToken, ...envConfig
+            } = action.config
+            return envConfig
         default:
             return state;
     }
 }
 
+export const authInfo = combineReducers({
+    authEnabled,
+    authStatus,
+    authToken
+});
+
 export const serverStatus = combineReducers({
     licensingInfo,
     matlabStatus,
     matlabVersion,
     wsEnv,
     isFetching,
     hasFetched,
     isSubmitting,
     fetchFailCount
 });
 
+
 export default combineReducers({
     triggerPosition,
     tutorialHidden,
     overlayVisibility,
     serverStatus,
     loadUrl,
     error,
     envConfig,
+    authInfo,
 });
```

### Comparing `matlab-proxy-0.5.8/gui/src/reducers/reducers.spec.js` & `matlab-proxy-0.5.9/gui/src/reducers/reducers.spec.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -28,14 +28,19 @@
                     status: 'up',
                     version: 'R2020b',
                 },
                 licensing: {
                     type: 'MHLM',
                 },
             },
+            authInfo: {
+                authEnabled: false,
+                authStatus: false,
+                authToken: null,
+            }
         };
 
         receiveActions.push(
             actions.RECEIVE_SERVER_STATUS,
             actions.RECEIVE_SET_LICENSING,
             actions.RECEIVE_TERMINATE_INTEGRATION,
             actions.RECEIVE_STOP_MATLAB,
@@ -97,14 +102,87 @@
             action.type = actions.RECEIVE_SET_LICENSING;
 
             expect(reducers.overlayVisibility(undefined, action)).toBe(false);
             expect(reducers.overlayVisibility(true, action)).toBe(true);
         });
     });
 
+    describe('authEnabled', () => {
+        it('should return whether token authenticaton is enabled', () => {
+
+            // default case
+            action = _.cloneDeep(genericAction);
+            expect(reducers.authEnabled(true, action)).toBe(true);
+            expect(reducers.authEnabled(false, action)).toBe(false);
+
+            // expect authEnabled to be false
+            action = _.cloneDeep(genericAction);
+            action.type = actions.RECEIVE_ENV_CONFIG;
+            action['config'] = {
+                "authEnabled": false
+            }
+            expect(reducers.authEnabled(undefined, action)).toBe(false);
+
+            // expect authEnabled to be true      
+            action = _.cloneDeep(genericAction);
+            action['config'] = {
+                "authEnabled": true
+            }
+            action.type = actions.RECEIVE_ENV_CONFIG;
+            expect(reducers.authEnabled(undefined, action)).toBe(true);
+        });
+    });
+
+    describe('authStatus', () => {
+        it('should return whether the user/client is authorised', () => {
+
+            // expect authStatus to be false
+            action = _.cloneDeep(genericAction);
+            action.type = actions.SET_AUTH_STATUS;
+            action.authInfo.authEnabled = true;
+            action.config = true
+            expect(reducers.authStatus(undefined, action)).toBe(false);
+
+            // expect authStatus to be true
+            action = _.cloneDeep(genericAction);
+            action.type = actions.SET_AUTH_STATUS;
+            action.authInfo.authStatus = true;
+
+            expect(reducers.authStatus(undefined, action)).toBe(true);
+
+            // default case
+            action = _.cloneDeep(genericAction);
+            expect(reducers.authStatus(true, action)).toBe(true);
+            expect(reducers.authStatus(false, action)).toBe(false);
+
+        });
+    });
+
+    describe('authToken', () => {
+        it('should return the value of the auth token', () => {
+
+            // expect authToken to be null
+            action = _.cloneDeep(genericAction);
+            action.type = actions.SET_AUTH_TOKEN;
+            expect(reducers.authToken(undefined, action)).toBeNull();
+
+            // expect authToken to be a string
+            action = _.cloneDeep(genericAction);
+            action.type = actions.SET_AUTH_TOKEN;
+            action.authInfo.authToken = 'string';
+            expect(reducers.authToken(undefined, action)).toBe('string');
+
+            // default case
+            action = _.cloneDeep(genericAction);
+            expect(reducers.authToken(null, action)).toBeNull();
+            expect(reducers.authToken('string', action)).toBe('string');
+
+        });
+    });
+
     describe('triggerPosition', () => {
         it('should return trigger x,y positions', () => {
 
             action = _.cloneDeep(genericAction);
             action.type = actions.SET_TRIGGER_POSITION;
 
             // expect to return the same trigger x,y positions
```

### Comparing `matlab-proxy-0.5.8/gui/src/selectors/selectors.spec.js` & `matlab-proxy-0.5.9/gui/src/selectors/selectors.spec.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -21,45 +21,59 @@
             hasFetched: false,
             licensingInfo: {
                 type: 'MHLM',
                 emailAddress: 'abc@mathworks.com',
             },
             fetchFailCount: 2,
         },
+        authInfo: {
+            authEnabled: false,
+            authStatus: false,
+            authToken: null,
+        },
     };
 
     const {
         tutorialHidden,
         serverStatus,
         loadUrl,
-        error
+        error,
+        authInfo,
     } = state;
 
     const {
         matlabVersion,
         isSubmitting,
         hasFetched,
         licensingInfo,
         fetchFailCount,
         matlabStatus,
         fetchAbortController,
     } = state.serverStatus;
 
+    const {
+        authEnabled,
+        authStatus,
+        authToken,
+    } = authInfo;
 
     const {
         selectTutorialHidden,
         selectServerStatus,
         selectLoadUrl,
         selectError,
         selectMatlabStatus,
         selectMatlabVersion,
         selectSubmittingServerStatus,
         selectHasFetchedServerStatus,
         selectLicensingInfo,
         selectServerStatusFetchFailCount,
+        selectAuthEnabled,
+        selectIsAuthenticated,
+        selectAuthToken,
         selectTriggerPosition,
         selectIsError,
         selectIsConnectionError,
         selectMatlabUp,
         selectMatlabRunning,
         selectOverlayHidable,
         selectOverlayVisibility,
@@ -69,31 +83,28 @@
         selectLicensingIsMhlm,
         selectLicensingMhlmUsername,
         selectMatlabPending,
         selectOverlayVisible,
         selectInformationDetails,
     } = selectors;
 
-    // beforeAll(() => {
-    //   // modifiedState = JSON.parse(JSON.stringify(state));
-    //   // modifiedState.triggerPosition = null;
-    // });
-
-
     describe.each([
             [selectTutorialHidden, tutorialHidden],
             [selectServerStatus, serverStatus],
             [selectLoadUrl, loadUrl],
             [selectError, error],
             [selectMatlabVersion, matlabVersion],
             [selectMatlabStatus, matlabStatus],
             [selectSubmittingServerStatus, isSubmitting],
             [selectHasFetchedServerStatus, hasFetched],
             [selectLicensingInfo, licensingInfo],
             [selectServerStatusFetchFailCount, fetchFailCount],
+            [selectAuthEnabled, authEnabled],
+            [selectIsAuthenticated, authStatus],
+            [selectAuthToken, authToken],
             [getFetchAbortController, fetchAbortController]
         ])
         ('Test simple selectors',
             (selector, expected) => {
                 test(`Check if ${selector.name} selects piece of state`, () => {
                     expect(selector(state)).toBe(expected);
                 });
@@ -188,30 +199,42 @@
 
         test('selectMatlabStarting should false when Matlab status is not starting', () => {
             modifiedState = _.cloneDeep(state);
             modifiedState.serverStatus.matlabStatus = 'up';
             expect(selectors.selectMatlabStopping(modifiedState)).toBe(false);
         });
 
-        test('selectOverlayHidable should return true when matlab is up and there is no error ', () => {
-            expect(selectOverlayHidable(state)).toBe(true);
+        test('selectOverlayHidable should return true when matlab is up and there is no error and user is authenticated or auth is not enabled', () => {
+            modifiedState = _.cloneDeep(state);
+            modifiedState.authInfo.authEnabled = true;
+            modifiedState.authInfo.authStatus = true;
+            expect(selectOverlayHidable(modifiedState)).toBe(true);
+
+            modifiedState = _.cloneDeep(state);
+            modifiedState.authInfo.authEnabled = false;
+            expect(selectOverlayHidable(modifiedState)).toBe(true);
         });
 
-        test('selectOverlayHidable should return false when matlab is not up or there is an error ', () => {
+        test('selectOverlayHidable should return false when matlab is not up or there is an error or the user is not authenticated', () => {
             modifiedState = _.cloneDeep(state);
             modifiedState.serverStatus.matlabStatus = 'down';
             expect(selectOverlayHidable(modifiedState)).toBe(false);
 
             modifiedState = _.cloneDeep(state);
             modifiedState.error = {};
             expect(selectOverlayHidable(modifiedState)).toBe(false);
+
+            modifiedState = _.cloneDeep(state);
+            modifiedState.authInfo.authEnabled = true;
+            modifiedState.authInfo.authStatus = false;
+            expect(selectOverlayHidable(modifiedState)).toBe(false);
         });
 
 
-        test('selectOverlayVisibility should return true when matlab is not up or visibility is true or there is an error ', () => {
+        test('selectOverlayVisibility should return true when matlab is not up or visibility is true or there is an error or the user is not authenticated', () => {
             //Should return true based on state.overlayVisibility
             expect(selectOverlayVisibility(state)).toBe(true);
 
             //should return true based on matlabStatus
             modifiedState = _.cloneDeep(state);
             modifiedState.serverStatus.matlabStatus = 'down';
             modifiedState.overlayVisibility = false;
@@ -219,21 +242,33 @@
 
             //should return true based on error
             modifiedState = _.cloneDeep(state);
             modifiedState.serverStatus.matlabStatus = 'down';
             modifiedState.overlayVisibility = false;
             modifiedState.error = {};
             expect(selectOverlayVisibility(modifiedState)).toBe(true);
+
+            modifiedState = _.cloneDeep(state);
+            modifiedState.overlayVisibility = false;
+            modifiedState.authInfo.authEnabled = true;
+            modifiedState.authInfo.authStatus = false;
+            expect(selectOverlayVisibility(modifiedState)).toBe(true);
         });
 
-        test('selectOverlayVisibility should return false when matlab is up and visibility is false and there is no error ', () => {
+        test('selectOverlayVisibility should return false when matlab is up and visibility is false and there is no error and user is authenticated if auth is enabled', () => {
             //Should return false matlab is up and overlayVisibility is false and there is an error
             modifiedState = _.cloneDeep(state);
             modifiedState.overlayVisibility = false;
             expect(selectOverlayVisibility(modifiedState)).toBe(false);
+
+            modifiedState = _.cloneDeep(state);
+            modifiedState.overlayVisibility = false;
+            modifiedState.authInfo.authEnabled = true;
+            modifiedState.authInfo.authStatus = true;
+            expect(selectOverlayVisibility(modifiedState)).toBe(false);
         });
 
         test('selectFetchStatusPeriod should return null if submitting to server', () => {
             expect(selectFetchStatusPeriod(state)).toBeNull();
         });
 
         test('selectFetchStatusPeriod should return 10000ms when matlab is up ', () => {
@@ -329,17 +364,19 @@
             modifiedState.serverStatus.matlabStatus = 'defaultCase';
 
             expect(() => selectInformationDetails(modifiedState)).toThrow(Error);
         })
 
         test('For MatlabStatus down and with an error, selectInformationDetails should return object with icon error', () => {
             modifiedState = _.cloneDeep(state);
+            // we are triggering the auth error by setting error to empty object here
             modifiedState.error = {};
             modifiedState.serverStatus.matlabStatus = 'down';
-
+            modifiedState.authInfo.authEnabled = true;
+            modifiedState.authInfo.authStatus = true;
             expect(selectInformationDetails(modifiedState).icon.toLowerCase()).toContain('error');
         })
 
         test('When backend is not reachable, selectInformationDetails should return object with icon warning and label unknown', () => {
             modifiedState = _.cloneDeep(state);
             modifiedState.error = {
                 message: 'HTTP request timed out',
```

### Comparing `matlab-proxy-0.5.8/gui/src/serviceWorker.js` & `matlab-proxy-0.5.9/gui/src/serviceWorker.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/gui/src/test/utils/react-test.js` & `matlab-proxy-0.5.9/gui/src/test/utils/react-test.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/__init__.py` & `matlab-proxy-0.5.9/matlab_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/app.py` & `matlab-proxy-0.5.9/matlab_proxy/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import matlab_proxy
 from matlab_proxy import settings, util
 from matlab_proxy.app_state import AppState
 from matlab_proxy.default_configuration import config
 from matlab_proxy.util import list_servers, mwi
 from matlab_proxy.util.mwi import environment_variables as mwi_env
 from matlab_proxy.util.mwi import token_auth
-from matlab_proxy.util.mwi.exceptions import LicensingError
+from matlab_proxy.util.mwi.exceptions import LicensingError, InvalidTokenError
 
 mimetypes.add_type("font/woff", ".woff")
 mimetypes.add_type("font/woff2", ".woff2")
 mimetypes.add_type("font/eot", ".eot")
 mimetypes.add_type("font/ttf", ".ttf")
 mimetypes.add_type("application/json", ".map")
 mimetypes.add_type("image/png", ".ico")
@@ -114,15 +114,25 @@
 
     Args:
         req (HTTPRequest): HTTPRequest Object.
 
     Returns:
         JSONResponse: contains a Dict representing environment specific configuration serialized to JSON
     """
-    config = req.app["state"].settings["env_config"]
+    state = req.app["state"]
+    config = state.settings["env_config"]
+    config["authEnabled"] = state.settings["mwi_is_token_auth_enabled"]
+
+    # In a previously authenticated session, if the url is accessed without the token(using session cookie), send the token as well.
+    config["authStatus"], config["authToken"] = (
+        (True, state.settings["mwi_auth_token"])
+        if await token_auth.authenticate_request(req)
+        else (False, None)
+    )
+
     return web.json_response(config)
 
 
 async def get_status(req):
     """API Endpoint to get the generic status of the server, MATLAB and MATLAB Licensing.
 
     Args:
@@ -134,23 +144,42 @@
     return await create_status_response(req.app)
 
 
 async def authenticate_request(req):
     """API Endpoint to authenticate request to access server
 
     Returns:
-        Response with status = 200 if request is authentic else return status = 401
+        JSONResponse: JSONResponse object containing information about authentication status and error if any.
     """
+    state = req.app["state"]
     if await token_auth.authenticate_request(req):
         logger.debug("!!!!!! REQUEST IS AUTHORIZED !!!!")
-        return web.Response(status=200)
+        authStatus = True
+        error = None
     else:
-        # Return HTTPUnauthorized
         logger.debug("!!!!!! REQUEST IS NOT AUTHORIZED !!!!")
-        return web.Response(status=401)
+        authStatus = False
+        error = marshal_error(
+            InvalidTokenError(
+                "Token invalid. Please enter a valid token to authenticate"
+            )
+        )
+
+    # If there is an error, state.error is not updated because the client may have set the
+    # token incorrectly which is not an error raised on the backend.
+
+    token = await req.text() if not error else ""
+
+    return web.json_response(
+        {
+            "authStatus": authStatus,
+            "authToken": token,
+            "error": error,
+        }
+    )
 
 
 async def start_matlab(req):
     """API Endpoint to start MATLAB
 
     Args:
         req (HTTPRequest): HTTPRequest Object
@@ -266,26 +295,28 @@
     to fail. Inorder to avoid this, adding the below if condition to check to skip sys.exit(0) when testing
     """
     logger.debug("Exiting with return code 0")
     if not mwi_env.is_testing_mode_enabled():
         sys.exit(0)
 
 
-@token_auth.decorator_authenticate_access
 async def root_redirect(request):
     """API Endpoint to return the root index.html file.
 
     Args:
         request (HTTPRequest): HTTPRequest Object
 
     Returns:
         HTTPResponse: HTTPResponse Object containing the index.html file.
     """
     base_url = request.app["settings"]["base_url"]
-    return aiohttp.web.HTTPFound(f"{base_url}/index.html")
+    query_params = f"?{request.query_string}" if request.query_string else ""
+    response_url = f"{base_url}/index.html{query_params}"
+
+    return aiohttp.web.HTTPFound(response_url)
 
 
 async def static_get(req):
     """Returns HTTP Response objects for the static files
 
     Args:
         req (HTTPRequest): HTTPRequest object
@@ -549,35 +580,14 @@
             task.cancel()
             try:
                 await task
             except asyncio.CancelledError:
                 pass
 
 
-@token_auth.decorator_authenticate_access
-async def get_mwi_auth_token(request):
-    """Endpoint to print the MWI token."""
-    logger.info("!!!!!! Inside get_mwi_auth_token !!!!!")
-    app_settings = request.app["settings"]
-    is_mwi_token_auth_enabled = app_settings["mwi_is_mwi_token_auth_enabled"]
-    base_url = app_settings["base_url"]
-    mwi_auth_token = app_settings["mwi_auth_token"]
-    if is_mwi_token_auth_enabled:
-        logger.info("get_mwi_auth_token: Responding with token information!!")
-        return aiohttp.web.HTTPFound(
-            f"{base_url}/token.html?mwi_auth_token={mwi_auth_token}"
-        )
-    else:
-        logger.info("get_mwi_auth_token: Token Auth mode not enabled")
-        return aiohttp.web.Response(
-            content_type="text/html",
-            body=f"Token-Based Authentication is not enabled!",
-        )
-
-
 def configure_and_start(app):
     """Configure the site for the app and update app with appropriate values
 
     Args:
         app (aiohttp.web.Application): A aiohttp web server.
 
     Returns:
@@ -640,30 +650,28 @@
         app["static_route_table"] = make_static_route_table(app)
         for key in app["static_route_table"].keys():
             app.router.add_route("GET", key, static_get)
 
     base_url = app["settings"]["base_url"]
     app.router.add_route("GET", f"{base_url}/get_status", get_status)
     app.router.add_route(
-        "GET", f"{base_url}/authenticate_request", authenticate_request
+        "POST", f"{base_url}/authenticate_request", authenticate_request
     )
     app.router.add_route("GET", f"{base_url}/get_env_config", get_env_config)
     app.router.add_route("PUT", f"{base_url}/start_matlab", start_matlab)
     app.router.add_route("DELETE", f"{base_url}/stop_matlab", stop_matlab)
     app.router.add_route("PUT", f"{base_url}/set_licensing_info", set_licensing_info)
     app.router.add_route(
         "DELETE", f"{base_url}/set_licensing_info", licensing_info_delete
     )
     app.router.add_route(
         "DELETE", f"{base_url}/terminate_integration", termination_integration_delete
     )
     app.router.add_route("*", f"{base_url}/", root_redirect)
     app.router.add_route("*", f"{base_url}", root_redirect)
-    mwi_auth_token_name = app["settings"]["mwi_auth_token_name"]
-    app.router.add_route("GET", f"{base_url}/get_mwi_auth_token", get_mwi_auth_token)
 
     app.router.add_route("*", f"{base_url}/{{proxyPath:.*}}", matlab_view)
     app.on_cleanup.append(cleanup_background_tasks)
 
     # Setup the session storage
     fernet_key = fernet.Fernet.generate_key()
     f = fernet.Fernet(fernet_key)
```

### Comparing `matlab-proxy-0.5.8/matlab_proxy/app_state.py` & `matlab-proxy-0.5.9/matlab_proxy/app_state.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/default_configuration.py` & `matlab-proxy-0.5.9/matlab_proxy/default_configuration.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/devel.py` & `matlab-proxy-0.5.9/matlab_proxy/devel.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/icons/matlab.svg` & `matlab-proxy-0.5.9/matlab_proxy/icons/matlab.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/matlab/startup.m` & `matlab-proxy-0.5.9/matlab_proxy/matlab/startup.m`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/settings.py` & `matlab-proxy-0.5.9/matlab_proxy/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     return get_mwi_config_folder(dev) / "ports"
 
 
 def get_dev_settings(config):
     devel_file = Path(__file__).resolve().parent / "./devel.py"
     mwi_config_folder = get_mwi_config_folder(dev=True)
     ws_env, ws_env_suffix = get_ws_env_settings()
+    mwi_auth_token = token_auth.generate_mwi_auth_token()
     return {
         "matlab_path": Path(),
         "matlab_version": "R2020b",
         "matlab_cmd": [
             "python",
             "-u",
             str(devel_file),
@@ -83,16 +84,17 @@
         "mwi_custom_http_headers": mwi.custom_http_headers.get(),
         "env_config": mwi.validators.validate_env_config(config),
         "ssl_context": None,
         "mwi_logs_root_dir": get_mwi_logs_root_dir(dev=True),
         "mwi_proxy_lock_file_name": "mwi_proxy.lock",
         "mw_context_tags": get_mw_context_tags(matlab_proxy.get_default_config_name()),
         "mwi_server_url": None,
-        "mwi_auth_token": None,
-        "mwi_is_mwi_token_auth_enabled": False,
+        "mwi_is_token_auth_enabled": mwi_auth_token != None,
+        "mwi_auth_status": False,
+        "mwi_auth_token": mwi_auth_token,
         "mwi_auth_token_name": mwi_env.get_env_name_mwi_auth_token().lower(),
     }
 
 
 def get(config_name=matlab_proxy.get_default_config_name(), dev=False):
     """Returns the settings specific to the environment in which the server is running in
     If the environment variable 'TEST' is set  to true, will make some changes to the dev settings.
@@ -198,16 +200,17 @@
             # a central place to store logs of all the running instances of MATLAB launched by matlab-proxy
             "mwi_logs_root_dir": get_mwi_logs_root_dir(),
             # Name of the lock file which will be created by this instance of matlab-proxy process.
             "mwi_proxy_lock_file_name": "mwi_proxy.lock",
             "mw_context_tags": get_mw_context_tags(config_name),
             # The url where the matlab-proxy server is accessible at
             "mwi_server_url": None,
+            "mwi_is_token_auth_enabled": mwi_auth_token != None,
+            "mwi_auth_status": False,
             "mwi_auth_token": mwi_auth_token,
-            "mwi_is_mwi_token_auth_enabled": mwi_auth_token != None,
             "mwi_auth_token_name": mwi_env.get_env_name_mwi_auth_token().lower(),
         }
 
 
 def get_mw_context_tags(extension_name):
     """Returns a string which combines existing MW_CONTEXT_TAGS value and context tags
     specific to where matlab-proxy is being launched from.
```

### Comparing `matlab-proxy-0.5.8/matlab_proxy/util/__init__.py` & `matlab-proxy-0.5.9/matlab_proxy/util/__init__.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/util/event_loop.py` & `matlab-proxy-0.5.9/matlab_proxy/util/event_loop.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/util/list_servers.py` & `matlab-proxy-0.5.9/matlab_proxy/util/list_servers.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/util/mw.py` & `matlab-proxy-0.5.9/matlab_proxy/util/mw.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/util/mwi/custom_http_headers.py` & `matlab-proxy-0.5.9/matlab_proxy/util/mwi/custom_http_headers.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/util/mwi/embedded_connector/helpers.py` & `matlab-proxy-0.5.9/matlab_proxy/util/mwi/embedded_connector/helpers.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/util/mwi/embedded_connector/request.py` & `matlab-proxy-0.5.9/matlab_proxy/util/mwi/embedded_connector/request.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/util/mwi/environment_variables.py` & `matlab-proxy-0.5.9/matlab_proxy/util/mwi/environment_variables.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/util/mwi/exceptions.py` & `matlab-proxy-0.5.9/matlab_proxy/util/mwi/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,14 +138,27 @@
         AppError (Class): Parent Class containing attributes to store
         messages, logs and stacktrace.
     """
 
     pass
 
 
+class InvalidTokenError(AppError):
+    """A Class which inherits the AppError class.
+
+    This class represents token authentication errors.
+
+    Args:
+        AppError (Class): Parent Class containing attributes to store
+        messages, logs and stacktrace.
+    """
+
+    pass
+
+
 def log_error(logger, err: Exception):
     """Logs any error to stdout.
 
     Args:
         logger (logging): A instance of the logging.getLogger()
         err (Class): An instance of one of the  Error classes as defined above.
         Example: OnlineLicensingError, EntitlementError
```

### Comparing `matlab-proxy-0.5.8/matlab_proxy/util/mwi/logger.py` & `matlab-proxy-0.5.9/matlab_proxy/util/mwi/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 """
 
 import logging
 import os
 
 from . import environment_variables as mwi_env
 
+logging.getLogger("aiohttp_session").setLevel(logging.ERROR)
+
 
 def get(init=False):
     """Get the logger used by this application.
         Set init=True to initialize the logger
     Returns:
         Logger: The logger used by this application.
     """
```

### Comparing `matlab-proxy-0.5.8/matlab_proxy/util/mwi/token_auth.py` & `matlab-proxy-0.5.9/matlab_proxy/util/mwi/token_auth.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,46 +18,34 @@
 def decorator_authenticate_access(endpoint):
     """Decorates any endpoint function with token authentication checks."""
     logger.debug("inside decorator_authenticate_access")
 
     async def authenticate_access(request):
         """
         If Authentication is enabled, this function expects the token to be present either in
-             the URL or in the session cookie.
+            the URL or in the session cookie.
         If token is provided and matches the expected secret, then the request is considered authentic,
             and the token is saved into the session cookie.
         """
         logger.debug(f" inside authenticate_access for request:{request}")
         app_settings = request.app["settings"]
         base_url = app_settings["base_url"]
 
         if await authenticate_request(request):
             logger.debug(
                 f" Request is authenticated, proceed to endpoint:{endpoint}{request}"
             )
             return await endpoint(request)
-        else:
-            # This branch intends to redirect users to the error page asking for TOKEN.
-            # However, we need to tell this page which page to redirect to on successful validation.
-
-            attempted_url = str(request.rel_url)
-
-            # Strip URL paramters
-            attempted_url = attempted_url.split("?", 1)[0]
-            logger.debug(f"attempted_url: {attempted_url}")
-            return web.HTTPFound(
-                f"{base_url}/authorization.html?attempted_url={request.rel_url}"
-            )
 
     return authenticate_access
 
 
 def is_mwi_token_auth_enabled(app_settings):
     """Returns True/False based on whether the mwi_auth_token_auth is enabled."""
-    return app_settings["mwi_is_mwi_token_auth_enabled"]
+    return app_settings["mwi_is_token_auth_enabled"]
 
 
 def get_mwi_auth_token_access_str(app_settings):
     """Returns formatted string with mwi token for use with server URL"""
     if is_mwi_token_auth_enabled(app_settings):
         mwi_auth_token_name = app_settings["mwi_auth_token_name"]
         mwi_auth_token = app_settings["mwi_auth_token"]
@@ -77,17 +65,17 @@
     if is_mwi_token_auth_enabled(app_settings):
         logger.debug(" Token Authentication is Enabled!!")
         the_secret_token = app_settings["mwi_auth_token"]
         token_name = app_settings["mwi_auth_token_name"]
         base_url = app_settings["base_url"]
 
         # get token if present in URL
-        parsed_url_token = request.rel_url.query.get(token_name, None)
+        parsed_url_token = await request.text()
 
-        if parsed_url_token is None:
+        if parsed_url_token == "":
             logger.debug("No Token found in URL. Checking session cookie...")
 
             # Check to see if there are cookies?
             session = await get_session(request)
             logger.debug(f"Got session cookie : {session}")
 
             if token_name in session:
@@ -99,15 +87,15 @@
                     return True
                 else:
                     logger.info("Invalid Token found in session!")
                     logger.debug(f"Expected: {the_secret_token}    ")
                     logger.debug(f"Actual  : {stored_session_token}")
                     return False
             else:
-                logger.info(f"{token_name} not found in session cookie.")
+                logger.debug(f"{token_name} not found in session cookie.")
                 return False
         else:
             logger.debug(f"Token found in URL with value: {parsed_url_token}")
             # Token is being provided, check it and stash it.
             if parsed_url_token == the_secret_token:
                 logger.debug("Token validation success!")
                 # Stash token in session for other endpoints
@@ -115,15 +103,15 @@
                 # Session Fixation. See aiohttp-session#281
                 session = await new_session(request)
                 session[token_name] = the_secret_token
                 logger.debug(f"Created session : {session} and saved cookie")
                 return True
             else:
                 logger.info("Invalid Token found in URL!")
-                logger.debug(f"Expected: {the_secret_token}    ")
+                logger.debug(f"Expected: {the_secret_token}")
                 logger.debug(f"Actual  : {parsed_url_token}")
                 return False
     else:
         # Token Authentication is not enabled
         logger.debug(" Token Authentication is NOT Enabled!!")
         return True
```

### Comparing `matlab-proxy-0.5.8/matlab_proxy/util/mwi/validators.py` & `matlab-proxy-0.5.9/matlab_proxy/util/mwi/validators.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/util/system.py` & `matlab-proxy-0.5.9/matlab_proxy/util/system.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.8/matlab_proxy/util/windows.py` & `matlab-proxy-0.5.9/matlab_proxy/util/windows.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         env=matlab_env,
         stderr=asyncio.subprocess.STDOUT,
     )
 
     # In testing mode, the devel.py file is run, which is the fake MATLAB server.
     # So, there is no need to check for an intermediate process when testing and can return
     # the same process as a psutil.Process() object.
-    if mwi_env.is_testing_mode_enabled():
+    if mwi_env.is_testing_mode_enabled() or mwi_env.is_development_mode_enabled():
         import psutil
 
         proc = psutil.Process(intermediate_proc.pid)
 
         return proc
 
     try:
```

### Comparing `matlab-proxy-0.5.8/matlab_proxy.egg-info/PKG-INFO` & `matlab-proxy-0.5.9/matlab_proxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matlab-proxy
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python® package enables you to launch MATLAB® and access it from a web browser.
 Home-page: https://github.com/mathworks/matlab-proxy/
 Author: The MathWorks, Inc.
 Author-email: cloud@mathworks.com
 License: MATHWORKS CLOUD REFERENCE ARCHITECTURE LICENSE
 Description: # MATLAB Proxy
         [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mathworks/matlab-proxy/run-tests.yml?branch=main&logo=github)](https://github.com/mathworks/matlab-proxy/actions) &nbsp; [![PyPI badge](https://img.shields.io/pypi/v/matlab-proxy.svg?logo=pypi)](https://pypi.python.org/pypi/matlab-proxy) &nbsp;  [![codecov](https://codecov.io/gh/mathworks/matlab-proxy/branch/main/graph/badge.svg?token=ZW3SESKCSS)](https://codecov.io/gh/mathworks/matlab-proxy) &nbsp; [![Downloads](https://static.pepy.tech/personalized-badge/matlab-proxy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20downloads/month)](https://pepy.tech/project/matlab-proxy)
```

### Comparing `matlab-proxy-0.5.8/matlab_proxy.egg-info/SOURCES.txt` & `matlab-proxy-0.5.9/matlab_proxy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,34 +3,30 @@
 README.md
 setup.cfg
 setup.py
 gui/.gitignore
 gui/README.md
 gui/package-lock.json
 gui/package.json
-gui/public/authorization.html
-gui/public/bootstrap.3.4.1.min.css
 gui/public/favicon.ico
 gui/public/index.html
 gui/public/manifest.json
-gui/public/navbar.css
 gui/public/robots.txt
-gui/public/signin.css
-gui/public/token.html
 gui/src/index.css
 gui/src/index.js
 gui/src/jest.config.json
 gui/src/logo.svg
 gui/src/serviceWorker.js
 gui/src/setupTests.js
 gui/src/actionCreators/actionCreators.spec.js
 gui/src/actionCreators/index.js
 gui/src/actions/index.js
 gui/src/components/App/App.css
 gui/src/components/App/App.spec.js
+gui/src/components/App/MATLAB-env-blur.png
 gui/src/components/App/index.js
 gui/src/components/App/3p/css/bootstrap.min.css
 gui/src/components/App/3p/css/site7.min.css
 gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot
 gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg
 gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf
 gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff
```

### Comparing `matlab-proxy-0.5.8/setup.py` & `matlab-proxy-0.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class InstallNpm(install):
     def run(self):
         # Ensure npm is present
         npm_path = which("npm")
         if not npm_path:
             raise Exception(
-                "npm must be installed and on the path during package install!"
+                "npm must be installered and on the path during package install!"
             )
 
         npm_install = [npm_path, "install"]
         npm_build = [npm_path, "run", "build"]
 
         pwd = Path(os.getcwd())
         gui_path = pwd / "gui"
@@ -61,15 +61,15 @@
 INSTALL_REQUIRES = ["aiohttp>=3.7.4", "psutil", "aiohttp_session[secure]"]
 
 HERE = Path(__file__).parent.resolve()
 long_description = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name="matlab-proxy",
-    version="0.5.8",
+    version="0.5.9",
     url=config["doc_url"],
     author="The MathWorks, Inc.",
     author_email="cloud@mathworks.com",
     license="MATHWORKS CLOUD REFERENCE ARCHITECTURE LICENSE",
     description="Python® package enables you to launch MATLAB® and access it from a web browser.",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -90,17 +90,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     python_requires="~=3.7",
     install_requires=INSTALL_REQUIRES,
     tests_require=TESTS_REQUIRES,
-    extras_require={
-        "dev": ["aiohttp-devtools", "black", "ruamel.yaml"] + TESTS_REQUIRES
-    },
+    extras_require={"dev": ["aiohttp-devtools", "black"] + TESTS_REQUIRES},
     # The entrypoint will be used by multiple packages that have this package as an installation
     # dependency. These packages can use the same API, get_entrypoint_name(), to make their configs discoverable
     entry_points={
         matlab_proxy.get_entrypoint_name(): [
             f"{matlab_proxy.get_default_config_name()} = matlab_proxy.default_configuration:config"
         ],
         "console_scripts": [
```

