# Comparing `tmp/django-admin-corporate-1.0.1.tar.gz` & `tmp/django-admin-corporate-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-corporate-1.0.1.tar", last modified: Wed Apr  5 10:24:30 2023, max compression
+gzip compressed data, was "django-admin-corporate-1.0.2.tar", last modified: Mon May  8 18:09:59 2023, max compression
```

## Comparing `django-admin-corporate-1.0.1.tar` & `django-admin-corporate-1.0.2.tar`

### file list

```diff
@@ -1,379 +1,379 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.929357 django-admin-corporate-1.0.1/
--rw-rw-rw-   0        0        0     1113 2023-04-04 07:23:07.000000 django-admin-corporate-1.0.1/LICENSE.md
--rw-rw-rw-   0        0        0      152 2023-04-04 07:34:47.000000 django-admin-corporate-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7213 2023-04-05 10:24:30.927354 django-admin-corporate-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6102 2023-04-05 08:27:17.000000 django-admin-corporate-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:29.142227 django-admin-corporate-1.0.1/admin_corporate/
--rw-rw-rw-   0        0        0        0 2023-04-04 07:23:07.000000 django-admin-corporate-1.0.1/admin_corporate/__init__.py
--rw-rw-rw-   0        0        0      167 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/apps.py
--rw-rw-rw-   0        0        0     2968 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:29.089153 django-admin-corporate-1.0.1/admin_corporate/static/
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:29.095678 django-admin-corporate-1.0.1/admin_corporate/static/assets/
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:29.992748 django-admin-corporate-1.0.1/admin_corporate/static/assets/css/
--rw-rw-rw-   0        0        0   523698 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/css/corporate-ui-dashboard.css
--rw-rw-rw-   0        0        0  1192544 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/css/corporate-ui-dashboard.css.map
--rw-rw-rw-   0        0        0   393282 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/css/corporate-ui-dashboard.min.css
--rw-rw-rw-   0        0        0     9756 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/css/forms.css
--rw-rw-rw-   0        0        0     9417 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/css/nucleo-icons.css
--rw-rw-rw-   0        0        0     2387 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/css/nucleo-svg.css
--rw-rw-rw-   0        0        0    12542 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/css/widgets.css
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.008859 django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/
--rw-rw-rw-   0        0        0    18516 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo-icons.eot
--rw-rw-rw-   0        0        0   126410 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo-icons.svg
--rw-rw-rw-   0        0        0    18292 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo-icons.ttf
--rw-rw-rw-   0        0        0    10220 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo-icons.woff
--rw-rw-rw-   0        0        0     8580 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo-icons.woff2
--rw-rw-rw-   0        0        0    26524 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo.eot
--rw-rw-rw-   0        0        0    26364 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo.ttf
--rw-rw-rw-   0        0        0    15168 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo.woff
--rw-rw-rw-   0        0        0    12616 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo.woff2
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.083891 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/
--rw-rw-rw-   0        0        0   260178 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/3d-cube.png
--rw-rw-rw-   0        0        0      809 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/apple-icon.png
--rw-rw-rw-   0        0        0   165177 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/bg1.jpg
--rw-rw-rw-   0        0        0    20236 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/bruce-mars.jpg
--rw-rw-rw-   0        0        0      411 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/corporate-ui-logo.svg
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.090187 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/curved-images/
--rw-rw-rw-   0        0        0   431309 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/curved-images/img-6.jpg
--rw-rw-rw-   0        0        0   379014 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/curved-images/img-7.jpg
--rw-rw-rw-   0        0        0     1111 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/down-arrow-dark.svg
--rw-rw-rw-   0        0        0      558 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/down-arrow-white.svg
--rw-rw-rw-   0        0        0     1109 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/down-arrow.svg
--rw-rw-rw-   0        0        0      809 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/favicon.png
--rw-rw-rw-   0        0        0   674338 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/header-blue-purple.jpg
--rw-rw-rw-   0        0        0   667893 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/header-orange-purple.jpg
--rw-rw-rw-   0        0        0     1095 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/icon-calendar.svg
--rw-rw-rw-   0        0        0      686 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/icon-clock.svg
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.092224 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/icons/
--rw-rw-rw-   0        0        0     1040 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/icons/add.svg
--rw-rw-rw-   0        0        0  1028477 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/image-sign-in.jpg
--rw-rw-rw-   0        0        0   819177 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/image-sign-up.jpg
--rw-rw-rw-   0        0        0   197578 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/img-1.jpg
--rw-rw-rw-   0        0        0   344305 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/img-2.jpg
--rw-rw-rw-   0        0        0   356125 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/img-3.jpg
--rw-rw-rw-   0        0        0   359597 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/img-4.jpg
--rw-rw-rw-   0        0        0   212812 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/img-5.jpg
--rw-rw-rw-   0        0        0   465599 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/img-8.jpg
--rw-rw-rw-   0        0        0   233404 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/img-9.jpg
--rw-rw-rw-   0        0        0     6956 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logo-ct-dark.png
--rw-rw-rw-   0        0        0     5756 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logo-ct.png
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.107212 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logos/
--rw-rw-rw-   0        0        0    59699 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logos/facebook-logo.svg
--rw-rw-rw-   0        0        0     2232 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logos/google-logo.svg
--rw-rw-rw-   0        0        0     6927 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logos/mastercard-white.png
--rw-rw-rw-   0        0        0      732 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logos/mastercard.png
--rw-rw-rw-   0        0        0     9046 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logos/visa-white.png
--rw-rw-rw-   0        0        0     1909 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logos/visa.png
--rw-rw-rw-   0        0        0     1733 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logos/wifi-white.png
--rw-rw-rw-   0        0        0   150148 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/marie.jpg
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.125284 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/
--rw-rw-rw-   0        0        0    96900 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/icon-sun-cloud.png
--rw-rw-rw-   0        0        0     1827 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/logo-atlassian.svg
--rw-rw-rw-   0        0        0     2232 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/logo-google.svg
--rw-rw-rw-   0        0        0     2586 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/logo-invision.svg
--rw-rw-rw-   0        0        0     1906 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/logo-jira.svg
--rw-rw-rw-   0        0        0     3209 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/logo-slack.svg
--rw-rw-rw-   0        0        0     1944 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/logo-spotify.svg
--rw-rw-rw-   0        0        0     1592 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/logo-webdev.svg
--rw-rw-rw-   0        0        0     3082 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/logo-xd.svg
--rw-rw-rw-   0        0        0   188298 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/team-1.jpg
--rw-rw-rw-   0        0        0   177150 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/team-2.jpg
--rw-rw-rw-   0        0        0   128766 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/team-3.jpg
--rw-rw-rw-   0        0        0   159925 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/team-4.jpg
--rw-rw-rw-   0        0        0    47452 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/team-5.jpg
--rw-rw-rw-   0        0        0    61542 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/team-6.jpg
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.152054 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/
--rw-rw-rw-   0        0        0    22527 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/angular.jpg
--rw-rw-rw-   0        0        0    18083 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/bootstrap.jpg
--rw-rw-rw-   0        0        0    32621 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/dribbble.png
--rw-rw-rw-   0        0        0     3729 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/dropbox.png
--rw-rw-rw-   0        0        0     2074 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/mastercard.png
--rw-rw-rw-   0        0        0     1448 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/paypal.png
--rw-rw-rw-   0        0        0    25566 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/react.jpg
--rw-rw-rw-   0        0        0    22085 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/sketch.jpg
--rw-rw-rw-   0        0        0     3523 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/slack.png
--rw-rw-rw-   0        0        0    18987 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/spotify.jpeg
--rw-rw-rw-   0        0        0    76209 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/tim.png
--rw-rw-rw-   0        0        0    12380 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/unass.jpg
--rw-rw-rw-   0        0        0     1472 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/visa.png
--rw-rw-rw-   0        0        0    18469 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/vue.jpg
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.156566 django-admin-corporate-1.0.1/admin_corporate/static/assets/js/
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.161570 django-admin-corporate-1.0.1/admin_corporate/static/assets/js/core/
--rw-rw-rw-   0        0        0    79700 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/js/core/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0    60020 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/js/core/bootstrap.min.js
--rw-rw-rw-   0        0        0    19731 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/js/core/popper.min.js
--rw-rw-rw-   0        0        0    13114 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/js/corporate-ui-dashboard.js
--rw-rw-rw-   0        0        0     7880 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/js/corporate-ui-dashboard.js.map
--rw-rw-rw-   0        0        0     8158 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/js/corporate-ui-dashboard.min.js
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.173707 django-admin-corporate-1.0.1/admin_corporate/static/assets/js/plugins/
--rw-rw-rw-   0        0        0     3863 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/js/plugins/Chart.extension.js
--rw-rw-rw-   0        0        0    16043 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/js/plugins/bootstrap-notify.js
--rw-rw-rw-   0        0        0   195101 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/js/plugins/chartjs.min.js
--rw-rw-rw-   0        0        0    19430 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/js/plugins/perfect-scrollbar.min.js
--rw-rw-rw-   0        0        0    48446 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/js/plugins/smooth-scrollbar.min.js
--rw-rw-rw-   0        0        0   143296 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/js/plugins/swiper-bundle.min.js
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.175649 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.230574 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/
--rw-rw-rw-   0        0        0      131 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_alert.scss
--rw-rw-rw-   0        0        0     2233 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_avatars.scss
--rw-rw-rw-   0        0        0      591 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_badge.scss
--rw-rw-rw-   0        0        0      780 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_breadcrumbs.scss
--rw-rw-rw-   0        0        0      184 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_button-group.scss
--rw-rw-rw-   0        0        0     4549 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_buttons.scss
--rw-rw-rw-   0        0        0     1156 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_cards.scss
--rw-rw-rw-   0        0        0     6351 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_dark-version.scss
--rw-rw-rw-   0        0        0     7381 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_dropdown.scss
--rw-rw-rw-   0        0        0     1100 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_dropup.scss
--rw-rw-rw-   0        0        0     1321 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_fixed-plugin.scss
--rw-rw-rw-   0        0        0      288 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_footer.scss
--rw-rw-rw-   0        0        0      876 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_forms.scss
--rw-rw-rw-   0        0        0      557 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_gradients.scss
--rw-rw-rw-   0        0        0      634 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_header.scss
--rw-rw-rw-   0        0        0     2972 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_info-areas.scss
--rw-rw-rw-   0        0        0     6826 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_misc.scss
--rw-rw-rw-   0        0        0     2974 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_nav.scss
--rw-rw-rw-   0        0        0    17802 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_navbar-vertical.scss
--rw-rw-rw-   0        0        0     4376 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_navbar.scss
--rw-rw-rw-   0        0        0     1250 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_pagination.scss
--rw-rw-rw-   0        0        0      135 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_popovers.scss
--rw-rw-rw-   0        0        0      245 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_progress.scss
--rw-rw-rw-   0        0        0     3400 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_rtl.scss
--rw-rw-rw-   0        0        0     1163 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_social-buttons.scss
--rw-rw-rw-   0        0        0      691 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_tables.scss
--rw-rw-rw-   0        0        0      300 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_tilt.scss
--rw-rw-rw-   0        0        0     2322 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_timeline.scss
--rw-rw-rw-   0        0        0      248 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_tooltips.scss
--rw-rw-rw-   0        0        0     5412 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_typography.scss
--rw-rw-rw-   0        0        0      206 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_utilities-extend.scss
--rw-rw-rw-   0        0        0    18067 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_utilities.scss
--rw-rw-rw-   0        0        0    69957 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_variables.scss
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.298488 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/
--rw-rw-rw-   0        0        0     4903 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_accordion.scss
--rw-rw-rw-   0        0        0     2242 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_alert.scss
--rw-rw-rw-   0        0        0     1259 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_badge.scss
--rw-rw-rw-   0        0        0     1849 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_breadcrumb.scss
--rw-rw-rw-   0        0        0     3202 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_button-group.scss
--rw-rw-rw-   0        0        0     5070 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_buttons.scss
--rw-rw-rw-   0        0        0     6970 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_card.scss
--rw-rw-rw-   0        0        0     5854 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_carousel.scss
--rw-rw-rw-   0        0        0     1167 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_close.scss
--rw-rw-rw-   0        0        0     1242 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_containers.scss
--rw-rw-rw-   0        0        0     8262 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_dropdown.scss
--rw-rw-rw-   0        0        0      265 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_forms.scss
--rw-rw-rw-   0        0        0    10860 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_functions.scss
--rw-rw-rw-   0        0        0      608 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_grid.scss
--rw-rw-rw-   0        0        0      304 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_helpers.scss
--rw-rw-rw-   0        0        0     1200 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_images.scss
--rw-rw-rw-   0        0        0     6539 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_list-group.scss
--rw-rw-rw-   0        0        0     1702 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_maps.scss
--rw-rw-rw-   0        0        0      942 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_mixins.scss
--rw-rw-rw-   0        0        0     7999 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_modal.scss
--rw-rw-rw-   0        0        0     4897 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_nav.scss
--rw-rw-rw-   0        0        0     8997 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_navbar.scss
--rw-rw-rw-   0        0        0     4628 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_offcanvas.scss
--rw-rw-rw-   0        0        0     4113 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_pagination.scss
--rw-rw-rw-   0        0        0      910 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_placeholders.scss
--rw-rw-rw-   0        0        0     7161 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_popover.scss
--rw-rw-rw-   0        0        0     1994 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_progress.scss
--rw-rw-rw-   0        0        0    12936 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_reboot.scss
--rw-rw-rw-   0        0        0     2576 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_root.scss
--rw-rw-rw-   0        0        0     2514 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_spinners.scss
--rw-rw-rw-   0        0        0     4577 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_tables.scss
--rw-rw-rw-   0        0        0     2511 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_toasts.scss
--rw-rw-rw-   0        0        0     4162 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_tooltip.scss
--rw-rw-rw-   0        0        0      452 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_transitions.scss
--rw-rw-rw-   0        0        0     1448 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_type.scss
--rw-rw-rw-   0        0        0    15464 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_utilities.scss
--rw-rw-rw-   0        0        0    70178 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_variables.scss
--rw-rw-rw-   0        0        0     1441 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/bootstrap-grid.scss
--rw-rw-rw-   0        0        0      461 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/bootstrap-reboot.scss
--rw-rw-rw-   0        0        0      434 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/bootstrap-utilities.scss
--rw-rw-rw-   0        0        0     1137 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/bootstrap.scss
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.312016 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/
--rw-rw-rw-   0        0        0     1984 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_floating-labels.scss
--rw-rw-rw-   0        0        0     4462 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-check.scss
--rw-rw-rw-   0        0        0     5914 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-control.scss
--rw-rw-rw-   0        0        0     2887 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-range.scss
--rw-rw-rw-   0        0        0     2387 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-select.scss
--rw-rw-rw-   0        0        0      230 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-text.scss
--rw-rw-rw-   0        0        0     3485 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_input-group.scss
--rw-rw-rw-   0        0        0     1178 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_labels.scss
--rw-rw-rw-   0        0        0      490 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_validation.scss
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.330619 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/
--rw-rw-rw-   0        0        0       40 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_clearfix.scss
--rw-rw-rw-   0        0        0      412 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_color-bg.scss
--rw-rw-rw-   0        0        0      462 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_colored-links.scss
--rw-rw-rw-   0        0        0      657 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_position.scss
--rw-rw-rw-   0        0        0      425 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_ratio.scss
--rw-rw-rw-   0        0        0      260 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_stacks.scss
--rw-rw-rw-   0        0        0      238 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_stretched-link.scss
--rw-rw-rw-   0        0        0       80 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_text-truncation.scss
--rw-rw-rw-   0        0        0      144 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_visually-hidden.scss
--rw-rw-rw-   0        0        0      155 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_vr.scss
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.372006 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/
--rw-rw-rw-   0        0        0      408 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_alert.scss
--rw-rw-rw-   0        0        0      342 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_backdrop.scss
--rw-rw-rw-   0        0        0     2109 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_border-radius.scss
--rw-rw-rw-   0        0        0      416 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_box-shadow.scss
--rw-rw-rw-   0        0        0     4707 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_breakpoints.scss
--rw-rw-rw-   0        0        0     3295 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_buttons.scss
--rw-rw-rw-   0        0        0     1537 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_caret.scss
--rw-rw-rw-   0        0        0      156 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_clearfix.scss
--rw-rw-rw-   0        0        0      174 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_color-scheme.scss
--rw-rw-rw-   0        0        0      419 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_container.scss
--rw-rw-rw-   0        0        0      623 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_deprecate.scss
--rw-rw-rw-   0        0        0     4234 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_forms.scss
--rw-rw-rw-   0        0        0     2003 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_gradients.scss
--rw-rw-rw-   0        0        0     4876 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_grid.scss
--rw-rw-rw-   0        0        0      411 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_image.scss
--rw-rw-rw-   0        0        0      533 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_list-group.scss
--rw-rw-rw-   0        0        0      175 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_lists.scss
--rw-rw-rw-   0        0        0      457 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_pagination.scss
--rw-rw-rw-   0        0        0      512 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_reset-text.scss
--rw-rw-rw-   0        0        0      208 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_resize.scss
--rw-rw-rw-   0        0        0     1113 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_table-variants.scss
--rw-rw-rw-   0        0        0      176 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_text-truncate.scss
--rw-rw-rw-   0        0        0      687 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_transition.scss
--rw-rw-rw-   0        0        0     3279 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_utilities.scss
--rw-rw-rw-   0        0        0     1041 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_visually-hidden.scss
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.373007 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/utilities/
--rw-rw-rw-   0        0        0     1784 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/utilities/_api.scss
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.374510 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/vendor/
--rw-rw-rw-   0        0        0    10383 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/vendor/_rfs.scss
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.375519 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/cards/
--rw-rw-rw-   0        0        0     2177 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/cards/card-background.scss
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.378521 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/custom/
--rw-rw-rw-   0        0        0        0 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/custom/_styles.scss
--rw-rw-rw-   0        0        0        0 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/custom/_variables.scss
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.389419 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/
--rw-rw-rw-   0        0        0     1708 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_form-check.scss
--rw-rw-rw-   0        0        0       53 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_form-select.scss
--rw-rw-rw-   0        0        0      914 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_form-switch.scss
--rw-rw-rw-   0        0        0      133 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_forms.scss
--rw-rw-rw-   0        0        0     1602 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_input-group.scss
--rw-rw-rw-   0        0        0      442 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_inputs.scss
--rw-rw-rw-   0        0        0      240 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_labels.scss
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.399958 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/mixins/
--rw-rw-rw-   0        0        0      270 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/mixins/_badge.scss
--rw-rw-rw-   0        0        0      190 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/mixins/_colored-shadows.scss
--rw-rw-rw-   0        0        0      302 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/mixins/_hover.scss
--rw-rw-rw-   0        0        0      825 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/mixins/_social-buttons.scss
--rw-rw-rw-   0        0        0       91 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/mixins/mixins.scss
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:29.105061 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.420044 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/
--rw-rw-rw-   0        0        0    21203 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_flatpickr.scss
--rw-rw-rw-   0        0        0     6012 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_nouislider.scss
--rw-rw-rw-   0        0        0     2714 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_perfect-scrollbar.scss
--rw-rw-rw-   0        0        0     2593 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_prism.scss
--rw-rw-rw-   0        0        0    20276 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_swiper.scss
--rw-rw-rw-   0        0        0      112 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/plugins.scss
--rw-rw-rw-   0        0        0     1464 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/theme.scss
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.469308 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/
--rw-rw-rw-   0        0        0     2157 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_animations.scss
--rw-rw-rw-   0        0        0      966 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_avatars.scss
--rw-rw-rw-   0        0        0     1547 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_badge.scss
--rw-rw-rw-   0        0        0      278 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_breadcrumb.scss
--rw-rw-rw-   0        0        0     1562 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_cards-extend.scss
--rw-rw-rw-   0        0        0     2875 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_cards.scss
--rw-rw-rw-   0        0        0      518 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_choices.scss
--rw-rw-rw-   0        0        0      918 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_dark-version.scss
--rw-rw-rw-   0        0        0     3007 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_dropdowns.scss
--rw-rw-rw-   0        0        0      316 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_fixed-plugin.scss
--rw-rw-rw-   0        0        0      106 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_form-switch.scss
--rw-rw-rw-   0        0        0      221 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_full-calendar.scss
--rw-rw-rw-   0        0        0     1099 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_header.scss
--rw-rw-rw-   0        0        0     1561 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_info-areas.scss
--rw-rw-rw-   0        0        0     2050 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_misc-extend.scss
--rw-rw-rw-   0        0        0     2646 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_misc.scss
--rw-rw-rw-   0        0        0     4018 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_navbar-vertical.scss
--rw-rw-rw-   0        0        0     1000 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_navbar.scss
--rw-rw-rw-   0        0        0      844 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_pagination.scss
--rw-rw-rw-   0        0        0       57 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_rtl.scss
--rw-rw-rw-   0        0        0     1308 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_social-buttons.scss
--rw-rw-rw-   0        0        0      871 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_table.scss
--rw-rw-rw-   0        0        0      642 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_timeline.scss
--rw-rw-rw-   0        0        0      940 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_utilities-extend.scss
--rw-rw-rw-   0        0        0     7444 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_utilities.scss
--rw-rw-rw-   0        0        0      215 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_virtual-reality.scss
--rw-rw-rw-   0        0        0      981 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard.scss
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:29.114057 django-admin-corporate-1.0.1/admin_corporate/templates/
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.482068 django-admin-corporate-1.0.1/admin_corporate/templates/accounts/
--rw-rw-rw-   0        0        0     1378 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/accounts/password-change-done.html
--rw-rw-rw-   0        0        0     2155 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/accounts/password-change.html
--rw-rw-rw-   0        0        0     1382 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/accounts/password-reset-complete.html
--rw-rw-rw-   0        0        0     1937 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/accounts/password-reset-confirm.html
--rw-rw-rw-   0        0        0     1181 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/accounts/password-reset-done.html
--rw-rw-rw-   0        0        0     2147 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/accounts/password-reset.html
--rw-rw-rw-   0        0        0     2944 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/accounts/sign-in.html
--rw-rw-rw-   0        0        0     4130 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/accounts/sign-up.html
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.506797 django-admin-corporate-1.0.1/admin_corporate/templates/admin/
--rw-rw-rw-   0        0        0     1745 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/actions.html
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:29.110054 django-admin-corporate-1.0.1/admin_corporate/templates/admin/auth/
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.508794 django-admin-corporate-1.0.1/admin_corporate/templates/admin/auth/user/
--rw-rw-rw-   0        0        0      334 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/auth/user/add_form.html
--rw-rw-rw-   0        0        0     5386 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/auth/user/change_password.html
--rw-rw-rw-   0        0        0     5912 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/change_form.html
--rw-rw-rw-   0        0        0      695 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/change_form_object_tools.html
--rw-rw-rw-   0        0        0     5598 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/change_list.html
--rw-rw-rw-   0        0        0      607 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/change_list_object_tools.html
--rw-rw-rw-   0        0        0     3141 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/change_list_results.html
--rw-rw-rw-   0        0        0     6925 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/delete_confirmation.html
--rw-rw-rw-   0        0        0     7246 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/delete_selected_confirmation.html
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.511802 django-admin-corporate-1.0.1/admin_corporate/templates/admin/edit_inline/
--rw-rw-rw-   0        0        0     3893 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/edit_inline/stacked.html
--rw-rw-rw-   0        0        0     7834 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/edit_inline/tabular.html
--rw-rw-rw-   0        0        0      643 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/filter.html
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.516361 django-admin-corporate-1.0.1/admin_corporate/templates/admin/includes/
--rw-rw-rw-   0        0        0     2572 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/includes/fieldset.html
--rw-rw-rw-   0        0        0      348 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/includes/object_delete_summary.html
--rw-rw-rw-   0        0        0    42632 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/index.html
--rw-rw-rw-   0        0        0     2727 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/invalid_setup.html
--rw-rw-rw-   0        0        0     3332 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/login.html
--rw-rw-rw-   0        0        0     3875 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/object_history.html
--rw-rw-rw-   0        0        0     2321 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/pagination.html
--rw-rw-rw-   0        0        0     2634 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/search_form.html
--rw-rw-rw-   0        0        0     1618 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/admin/submit_line.html
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.887564 django-admin-corporate-1.0.1/admin_corporate/templates/includes/
--rw-rw-rw-   0        0        0     3769 2023-04-05 10:03:50.000000 django-admin-corporate-1.0.1/admin_corporate/templates/includes/fixed_plugin.html
--rw-rw-rw-   0        0        0        0 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/includes/footer-rtl.html
--rw-rw-rw-   0        0        0      981 2023-04-05 09:07:38.000000 django-admin-corporate-1.0.1/admin_corporate/templates/includes/footer.html
--rw-rw-rw-   0        0        0     1054 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/includes/head.html
--rw-rw-rw-   0        0        0     5946 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/includes/navigation-auth.html
--rw-rw-rw-   0        0        0    10812 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/includes/navigation-fullscreen.html
--rw-rw-rw-   0        0        0     8511 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/includes/navigation-rtl.html
--rw-rw-rw-   0        0        0     8532 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/includes/navigation.html
--rw-rw-rw-   0        0        0      355 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/includes/scripts.html
--rw-rw-rw-   0        0        0    10639 2023-04-05 10:03:31.000000 django-admin-corporate-1.0.1/admin_corporate/templates/includes/sidebar-rtl.html
--rw-rw-rw-   0        0        0    15487 2023-04-05 10:03:28.000000 django-admin-corporate-1.0.1/admin_corporate/templates/includes/sidebar.html
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.892565 django-admin-corporate-1.0.1/admin_corporate/templates/layouts/
--rw-rw-rw-   0        0        0     1240 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/layouts/base-auth.html
--rw-rw-rw-   0        0        0     1868 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/layouts/base-fullscreen.html
--rw-rw-rw-   0        0        0     2016 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/layouts/base-rtl.html
--rw-rw-rw-   0        0        0     2217 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/layouts/base.html
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.903664 django-admin-corporate-1.0.1/admin_corporate/templates/pages/
--rw-rw-rw-   0        0        0    42632 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/pages/dashboard.html
--rw-rw-rw-   0        0        0    18562 2023-04-05 10:09:50.000000 django-admin-corporate-1.0.1/admin_corporate/templates/pages/profile.html
--rw-rw-rw-   0        0        0    51971 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/pages/rtl.html
--rw-rw-rw-   0        0        0    51177 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/pages/tables.html
--rw-rw-rw-   0        0        0    39396 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/pages/wallet.html
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.907611 django-admin-corporate-1.0.1/admin_corporate/templates/registration/
--rw-rw-rw-   0        0        0     1658 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/registration/logged_out.html
--rw-rw-rw-   0        0        0     2688 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/registration/password_change_done.html
--rw-rw-rw-   0        0        0     3964 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templates/registration/password_change_form.html
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.914820 django-admin-corporate-1.0.1/admin_corporate/templatetags/
--rw-rw-rw-   0        0        0        0 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templatetags/__init__.py
--rw-rw-rw-   0        0        0     2476 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templatetags/admin_corporate.py
--rw-rw-rw-   0        0        0      178 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/templatetags/replace_value.py
--rw-rw-rw-   0        0        0     1536 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/urls.py
--rw-rw-rw-   0        0        0    16522 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/utils.py
--rw-rw-rw-   0        0        0     2515 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.1/admin_corporate/views.py
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.923813 django-admin-corporate-1.0.1/django_admin_corporate.egg-info/
--rw-rw-rw-   0        0        0     7213 2023-04-05 10:24:28.000000 django-admin-corporate-1.0.1/django_admin_corporate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    22307 2023-04-05 10:24:29.000000 django-admin-corporate-1.0.1/django_admin_corporate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 10:24:28.000000 django-admin-corporate-1.0.1/django_admin_corporate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-05 08:17:35.000000 django-admin-corporate-1.0.1/django_admin_corporate.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-04-05 10:24:28.000000 django-admin-corporate-1.0.1/django_admin_corporate.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 10:24:30.925344 django-admin-corporate-1.0.1/docs/
--rw-rw-rw-   0        0        0       13 2023-04-04 07:23:08.000000 django-admin-corporate-1.0.1/docs/blank.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 10:24:30.929357 django-admin-corporate-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1359 2023-04-05 10:24:07.000000 django-admin-corporate-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.473694 django-admin-corporate-1.0.2/
+-rw-rw-rw-   0        0        0     1113 2023-04-04 07:23:07.000000 django-admin-corporate-1.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0      152 2023-04-04 07:34:47.000000 django-admin-corporate-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7213 2023-05-08 18:09:59.472689 django-admin-corporate-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6102 2023-04-05 08:27:17.000000 django-admin-corporate-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.643781 django-admin-corporate-1.0.2/admin_corporate/
+-rw-rw-rw-   0        0        0        0 2023-04-04 07:23:07.000000 django-admin-corporate-1.0.2/admin_corporate/__init__.py
+-rw-rw-rw-   0        0        0      167 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/apps.py
+-rw-rw-rw-   0        0        0     2968 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.563660 django-admin-corporate-1.0.2/admin_corporate/static/
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.574234 django-admin-corporate-1.0.2/admin_corporate/static/assets/
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.660303 django-admin-corporate-1.0.2/admin_corporate/static/assets/css/
+-rw-rw-rw-   0        0        0   523652 2023-05-08 17:56:00.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/css/corporate-ui-dashboard.css
+-rw-rw-rw-   0        0        0  1192544 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/css/corporate-ui-dashboard.css.map
+-rw-rw-rw-   0        0        0   393282 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/css/corporate-ui-dashboard.min.css
+-rw-rw-rw-   0        0        0     9756 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/css/forms.css
+-rw-rw-rw-   0        0        0     9417 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/css/nucleo-icons.css
+-rw-rw-rw-   0        0        0     2387 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/css/nucleo-svg.css
+-rw-rw-rw-   0        0        0    12542 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/css/widgets.css
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.690143 django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/
+-rw-rw-rw-   0        0        0    18516 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo-icons.eot
+-rw-rw-rw-   0        0        0   126410 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo-icons.svg
+-rw-rw-rw-   0        0        0    18292 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo-icons.ttf
+-rw-rw-rw-   0        0        0    10220 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo-icons.woff
+-rw-rw-rw-   0        0        0     8580 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo-icons.woff2
+-rw-rw-rw-   0        0        0    26524 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo.eot
+-rw-rw-rw-   0        0        0    26364 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo.ttf
+-rw-rw-rw-   0        0        0    15168 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo.woff
+-rw-rw-rw-   0        0        0    12616 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo.woff2
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.813650 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/
+-rw-rw-rw-   0        0        0   260178 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/3d-cube.png
+-rw-rw-rw-   0        0        0      809 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/apple-icon.png
+-rw-rw-rw-   0        0        0   165177 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/bg1.jpg
+-rw-rw-rw-   0        0        0    20236 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/bruce-mars.jpg
+-rw-rw-rw-   0        0        0      411 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/corporate-ui-logo.svg
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.821658 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/curved-images/
+-rw-rw-rw-   0        0        0   431309 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/curved-images/img-6.jpg
+-rw-rw-rw-   0        0        0   379014 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/curved-images/img-7.jpg
+-rw-rw-rw-   0        0        0     1111 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/down-arrow-dark.svg
+-rw-rw-rw-   0        0        0      558 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/down-arrow-white.svg
+-rw-rw-rw-   0        0        0     1109 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/down-arrow.svg
+-rw-rw-rw-   0        0        0      809 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/favicon.png
+-rw-rw-rw-   0        0        0   674338 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/header-blue-purple.jpg
+-rw-rw-rw-   0        0        0   667893 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/header-orange-purple.jpg
+-rw-rw-rw-   0        0        0     1095 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/icon-calendar.svg
+-rw-rw-rw-   0        0        0      686 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/icon-clock.svg
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.824934 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/icons/
+-rw-rw-rw-   0        0        0     1040 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/icons/add.svg
+-rw-rw-rw-   0        0        0  1028477 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/image-sign-in.jpg
+-rw-rw-rw-   0        0        0   819177 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/image-sign-up.jpg
+-rw-rw-rw-   0        0        0   197578 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/img-1.jpg
+-rw-rw-rw-   0        0        0   344305 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/img-2.jpg
+-rw-rw-rw-   0        0        0   356125 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/img-3.jpg
+-rw-rw-rw-   0        0        0   359597 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/img-4.jpg
+-rw-rw-rw-   0        0        0   212812 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/img-5.jpg
+-rw-rw-rw-   0        0        0   465599 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/img-8.jpg
+-rw-rw-rw-   0        0        0   233404 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/img-9.jpg
+-rw-rw-rw-   0        0        0     6956 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logo-ct-dark.png
+-rw-rw-rw-   0        0        0     5756 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logo-ct.png
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.839047 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logos/
+-rw-rw-rw-   0        0        0    59699 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logos/facebook-logo.svg
+-rw-rw-rw-   0        0        0     2232 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logos/google-logo.svg
+-rw-rw-rw-   0        0        0     6927 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logos/mastercard-white.png
+-rw-rw-rw-   0        0        0      732 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logos/mastercard.png
+-rw-rw-rw-   0        0        0     9046 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logos/visa-white.png
+-rw-rw-rw-   0        0        0     1909 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logos/visa.png
+-rw-rw-rw-   0        0        0     1733 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logos/wifi-white.png
+-rw-rw-rw-   0        0        0   150148 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/marie.jpg
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.855797 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/
+-rw-rw-rw-   0        0        0    96900 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/icon-sun-cloud.png
+-rw-rw-rw-   0        0        0     1827 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/logo-atlassian.svg
+-rw-rw-rw-   0        0        0     2232 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/logo-google.svg
+-rw-rw-rw-   0        0        0     2586 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/logo-invision.svg
+-rw-rw-rw-   0        0        0     1906 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/logo-jira.svg
+-rw-rw-rw-   0        0        0     3209 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/logo-slack.svg
+-rw-rw-rw-   0        0        0     1944 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/logo-spotify.svg
+-rw-rw-rw-   0        0        0     1592 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/logo-webdev.svg
+-rw-rw-rw-   0        0        0     3082 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/logo-xd.svg
+-rw-rw-rw-   0        0        0   188298 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/team-1.jpg
+-rw-rw-rw-   0        0        0   177150 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/team-2.jpg
+-rw-rw-rw-   0        0        0   128766 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/team-3.jpg
+-rw-rw-rw-   0        0        0   159925 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/team-4.jpg
+-rw-rw-rw-   0        0        0    47452 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/team-5.jpg
+-rw-rw-rw-   0        0        0    61542 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/team-6.jpg
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.883979 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/
+-rw-rw-rw-   0        0        0    22527 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/angular.jpg
+-rw-rw-rw-   0        0        0    18083 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/bootstrap.jpg
+-rw-rw-rw-   0        0        0    32621 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/dribbble.png
+-rw-rw-rw-   0        0        0     3729 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/dropbox.png
+-rw-rw-rw-   0        0        0     2074 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/mastercard.png
+-rw-rw-rw-   0        0        0     1448 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/paypal.png
+-rw-rw-rw-   0        0        0    25566 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/react.jpg
+-rw-rw-rw-   0        0        0    22085 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/sketch.jpg
+-rw-rw-rw-   0        0        0     3523 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/slack.png
+-rw-rw-rw-   0        0        0    18987 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/spotify.jpeg
+-rw-rw-rw-   0        0        0    76209 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/tim.png
+-rw-rw-rw-   0        0        0    12380 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/unass.jpg
+-rw-rw-rw-   0        0        0     1472 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/visa.png
+-rw-rw-rw-   0        0        0    18469 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/vue.jpg
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.888990 django-admin-corporate-1.0.2/admin_corporate/static/assets/js/
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.895565 django-admin-corporate-1.0.2/admin_corporate/static/assets/js/core/
+-rw-rw-rw-   0        0        0    79700 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/js/core/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0    60020 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/js/core/bootstrap.min.js
+-rw-rw-rw-   0        0        0    19731 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/js/core/popper.min.js
+-rw-rw-rw-   0        0        0    13114 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/js/corporate-ui-dashboard.js
+-rw-rw-rw-   0        0        0     7880 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/js/corporate-ui-dashboard.js.map
+-rw-rw-rw-   0        0        0     8085 2023-05-08 17:56:44.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/js/corporate-ui-dashboard.min.js
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.908101 django-admin-corporate-1.0.2/admin_corporate/static/assets/js/plugins/
+-rw-rw-rw-   0        0        0     3863 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/js/plugins/Chart.extension.js
+-rw-rw-rw-   0        0        0    16043 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/js/plugins/bootstrap-notify.js
+-rw-rw-rw-   0        0        0   195101 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/js/plugins/chartjs.min.js
+-rw-rw-rw-   0        0        0    19430 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/js/plugins/perfect-scrollbar.min.js
+-rw-rw-rw-   0        0        0    48446 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/js/plugins/smooth-scrollbar.min.js
+-rw-rw-rw-   0        0        0   143251 2023-05-08 17:56:48.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/js/plugins/swiper-bundle.min.js
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.910132 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.975091 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/
+-rw-rw-rw-   0        0        0      131 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_alert.scss
+-rw-rw-rw-   0        0        0     2233 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_avatars.scss
+-rw-rw-rw-   0        0        0      591 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_badge.scss
+-rw-rw-rw-   0        0        0      780 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_breadcrumbs.scss
+-rw-rw-rw-   0        0        0      184 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_button-group.scss
+-rw-rw-rw-   0        0        0     4549 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_buttons.scss
+-rw-rw-rw-   0        0        0     1156 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_cards.scss
+-rw-rw-rw-   0        0        0     6351 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_dark-version.scss
+-rw-rw-rw-   0        0        0     7381 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_dropdown.scss
+-rw-rw-rw-   0        0        0     1100 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_dropup.scss
+-rw-rw-rw-   0        0        0     1321 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_fixed-plugin.scss
+-rw-rw-rw-   0        0        0      288 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_footer.scss
+-rw-rw-rw-   0        0        0      876 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_forms.scss
+-rw-rw-rw-   0        0        0      557 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_gradients.scss
+-rw-rw-rw-   0        0        0      634 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_header.scss
+-rw-rw-rw-   0        0        0     2972 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_info-areas.scss
+-rw-rw-rw-   0        0        0     6826 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_misc.scss
+-rw-rw-rw-   0        0        0     2974 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_nav.scss
+-rw-rw-rw-   0        0        0    17802 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_navbar-vertical.scss
+-rw-rw-rw-   0        0        0     4376 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_navbar.scss
+-rw-rw-rw-   0        0        0     1250 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_pagination.scss
+-rw-rw-rw-   0        0        0      135 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_popovers.scss
+-rw-rw-rw-   0        0        0      245 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_progress.scss
+-rw-rw-rw-   0        0        0     3400 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_rtl.scss
+-rw-rw-rw-   0        0        0     1163 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_social-buttons.scss
+-rw-rw-rw-   0        0        0      691 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_tables.scss
+-rw-rw-rw-   0        0        0      300 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_tilt.scss
+-rw-rw-rw-   0        0        0     2322 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_timeline.scss
+-rw-rw-rw-   0        0        0      248 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_tooltips.scss
+-rw-rw-rw-   0        0        0     5412 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_typography.scss
+-rw-rw-rw-   0        0        0      206 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_utilities-extend.scss
+-rw-rw-rw-   0        0        0    18067 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_utilities.scss
+-rw-rw-rw-   0        0        0    69957 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_variables.scss
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.058587 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/
+-rw-rw-rw-   0        0        0     4903 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_accordion.scss
+-rw-rw-rw-   0        0        0     2242 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_alert.scss
+-rw-rw-rw-   0        0        0     1259 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_badge.scss
+-rw-rw-rw-   0        0        0     1849 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_breadcrumb.scss
+-rw-rw-rw-   0        0        0     3202 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_button-group.scss
+-rw-rw-rw-   0        0        0     5070 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_buttons.scss
+-rw-rw-rw-   0        0        0     6970 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_card.scss
+-rw-rw-rw-   0        0        0     5854 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_carousel.scss
+-rw-rw-rw-   0        0        0     1167 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_close.scss
+-rw-rw-rw-   0        0        0     1242 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_containers.scss
+-rw-rw-rw-   0        0        0     8262 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_dropdown.scss
+-rw-rw-rw-   0        0        0      265 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_forms.scss
+-rw-rw-rw-   0        0        0    10860 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_functions.scss
+-rw-rw-rw-   0        0        0      608 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_grid.scss
+-rw-rw-rw-   0        0        0      304 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_helpers.scss
+-rw-rw-rw-   0        0        0     1200 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_images.scss
+-rw-rw-rw-   0        0        0     6539 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_list-group.scss
+-rw-rw-rw-   0        0        0     1702 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_maps.scss
+-rw-rw-rw-   0        0        0      942 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_mixins.scss
+-rw-rw-rw-   0        0        0     7999 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_modal.scss
+-rw-rw-rw-   0        0        0     4897 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_nav.scss
+-rw-rw-rw-   0        0        0     8997 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_navbar.scss
+-rw-rw-rw-   0        0        0     4628 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_offcanvas.scss
+-rw-rw-rw-   0        0        0     4113 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_pagination.scss
+-rw-rw-rw-   0        0        0      910 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_placeholders.scss
+-rw-rw-rw-   0        0        0     7161 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_popover.scss
+-rw-rw-rw-   0        0        0     1994 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_progress.scss
+-rw-rw-rw-   0        0        0    12936 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_reboot.scss
+-rw-rw-rw-   0        0        0     2576 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_root.scss
+-rw-rw-rw-   0        0        0     2514 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_spinners.scss
+-rw-rw-rw-   0        0        0     4577 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_tables.scss
+-rw-rw-rw-   0        0        0     2511 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_toasts.scss
+-rw-rw-rw-   0        0        0     4162 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_tooltip.scss
+-rw-rw-rw-   0        0        0      452 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_transitions.scss
+-rw-rw-rw-   0        0        0     1448 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_type.scss
+-rw-rw-rw-   0        0        0    15464 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_utilities.scss
+-rw-rw-rw-   0        0        0    70178 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_variables.scss
+-rw-rw-rw-   0        0        0     1441 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/bootstrap-grid.scss
+-rw-rw-rw-   0        0        0      461 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/bootstrap-reboot.scss
+-rw-rw-rw-   0        0        0      434 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/bootstrap-utilities.scss
+-rw-rw-rw-   0        0        0     1137 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/bootstrap.scss
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.078218 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/
+-rw-rw-rw-   0        0        0     1984 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_floating-labels.scss
+-rw-rw-rw-   0        0        0     4462 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-check.scss
+-rw-rw-rw-   0        0        0     5914 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-control.scss
+-rw-rw-rw-   0        0        0     2887 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-range.scss
+-rw-rw-rw-   0        0        0     2387 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-select.scss
+-rw-rw-rw-   0        0        0      230 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-text.scss
+-rw-rw-rw-   0        0        0     3485 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_input-group.scss
+-rw-rw-rw-   0        0        0     1178 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_labels.scss
+-rw-rw-rw-   0        0        0      490 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_validation.scss
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.099384 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/
+-rw-rw-rw-   0        0        0       40 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_clearfix.scss
+-rw-rw-rw-   0        0        0      412 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_color-bg.scss
+-rw-rw-rw-   0        0        0      462 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_colored-links.scss
+-rw-rw-rw-   0        0        0      657 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_position.scss
+-rw-rw-rw-   0        0        0      425 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_ratio.scss
+-rw-rw-rw-   0        0        0      260 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_stacks.scss
+-rw-rw-rw-   0        0        0      238 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_stretched-link.scss
+-rw-rw-rw-   0        0        0       80 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_text-truncation.scss
+-rw-rw-rw-   0        0        0      144 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_visually-hidden.scss
+-rw-rw-rw-   0        0        0      155 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_vr.scss
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.150753 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/
+-rw-rw-rw-   0        0        0      408 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_alert.scss
+-rw-rw-rw-   0        0        0      342 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_backdrop.scss
+-rw-rw-rw-   0        0        0     2109 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_border-radius.scss
+-rw-rw-rw-   0        0        0      416 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_box-shadow.scss
+-rw-rw-rw-   0        0        0     4707 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_breakpoints.scss
+-rw-rw-rw-   0        0        0     3295 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_buttons.scss
+-rw-rw-rw-   0        0        0     1537 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_caret.scss
+-rw-rw-rw-   0        0        0      156 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_clearfix.scss
+-rw-rw-rw-   0        0        0      174 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_color-scheme.scss
+-rw-rw-rw-   0        0        0      419 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_container.scss
+-rw-rw-rw-   0        0        0      623 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_deprecate.scss
+-rw-rw-rw-   0        0        0     4234 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_forms.scss
+-rw-rw-rw-   0        0        0     2003 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_gradients.scss
+-rw-rw-rw-   0        0        0     4876 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_grid.scss
+-rw-rw-rw-   0        0        0      411 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_image.scss
+-rw-rw-rw-   0        0        0      533 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_list-group.scss
+-rw-rw-rw-   0        0        0      175 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_lists.scss
+-rw-rw-rw-   0        0        0      457 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_pagination.scss
+-rw-rw-rw-   0        0        0      512 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_reset-text.scss
+-rw-rw-rw-   0        0        0      208 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_resize.scss
+-rw-rw-rw-   0        0        0     1113 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_table-variants.scss
+-rw-rw-rw-   0        0        0      176 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_text-truncate.scss
+-rw-rw-rw-   0        0        0      687 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_transition.scss
+-rw-rw-rw-   0        0        0     3279 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_utilities.scss
+-rw-rw-rw-   0        0        0     1041 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_visually-hidden.scss
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.153233 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/utilities/
+-rw-rw-rw-   0        0        0     1784 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/utilities/_api.scss
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.155243 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/vendor/
+-rw-rw-rw-   0        0        0    10383 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/vendor/_rfs.scss
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.157240 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/cards/
+-rw-rw-rw-   0        0        0     2177 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/cards/card-background.scss
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.160245 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/custom/
+-rw-rw-rw-   0        0        0        0 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/custom/_styles.scss
+-rw-rw-rw-   0        0        0        0 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/custom/_variables.scss
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.175913 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/
+-rw-rw-rw-   0        0        0     1708 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_form-check.scss
+-rw-rw-rw-   0        0        0       53 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_form-select.scss
+-rw-rw-rw-   0        0        0      914 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_form-switch.scss
+-rw-rw-rw-   0        0        0      133 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_forms.scss
+-rw-rw-rw-   0        0        0     1602 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_input-group.scss
+-rw-rw-rw-   0        0        0      442 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_inputs.scss
+-rw-rw-rw-   0        0        0      240 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_labels.scss
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.195981 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/mixins/
+-rw-rw-rw-   0        0        0      270 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/mixins/_badge.scss
+-rw-rw-rw-   0        0        0      190 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/mixins/_colored-shadows.scss
+-rw-rw-rw-   0        0        0      302 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/mixins/_hover.scss
+-rw-rw-rw-   0        0        0      825 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/mixins/_social-buttons.scss
+-rw-rw-rw-   0        0        0       91 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/mixins/mixins.scss
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.584754 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.226298 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/
+-rw-rw-rw-   0        0        0    21203 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_flatpickr.scss
+-rw-rw-rw-   0        0        0     6012 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_nouislider.scss
+-rw-rw-rw-   0        0        0     2714 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_perfect-scrollbar.scss
+-rw-rw-rw-   0        0        0     2593 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_prism.scss
+-rw-rw-rw-   0        0        0    20276 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_swiper.scss
+-rw-rw-rw-   0        0        0      112 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/plugins.scss
+-rw-rw-rw-   0        0        0     1464 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/theme.scss
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.311085 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/
+-rw-rw-rw-   0        0        0     2157 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_animations.scss
+-rw-rw-rw-   0        0        0      966 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_avatars.scss
+-rw-rw-rw-   0        0        0     1547 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_badge.scss
+-rw-rw-rw-   0        0        0      278 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_breadcrumb.scss
+-rw-rw-rw-   0        0        0     1562 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_cards-extend.scss
+-rw-rw-rw-   0        0        0     2875 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_cards.scss
+-rw-rw-rw-   0        0        0      518 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_choices.scss
+-rw-rw-rw-   0        0        0      918 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_dark-version.scss
+-rw-rw-rw-   0        0        0     3007 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_dropdowns.scss
+-rw-rw-rw-   0        0        0      316 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_fixed-plugin.scss
+-rw-rw-rw-   0        0        0      106 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_form-switch.scss
+-rw-rw-rw-   0        0        0      221 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_full-calendar.scss
+-rw-rw-rw-   0        0        0     1099 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_header.scss
+-rw-rw-rw-   0        0        0     1561 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_info-areas.scss
+-rw-rw-rw-   0        0        0     2050 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_misc-extend.scss
+-rw-rw-rw-   0        0        0     2646 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_misc.scss
+-rw-rw-rw-   0        0        0     4018 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_navbar-vertical.scss
+-rw-rw-rw-   0        0        0     1000 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_navbar.scss
+-rw-rw-rw-   0        0        0      844 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_pagination.scss
+-rw-rw-rw-   0        0        0       57 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_rtl.scss
+-rw-rw-rw-   0        0        0     1308 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_social-buttons.scss
+-rw-rw-rw-   0        0        0      871 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_table.scss
+-rw-rw-rw-   0        0        0      642 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_timeline.scss
+-rw-rw-rw-   0        0        0      940 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_utilities-extend.scss
+-rw-rw-rw-   0        0        0     7444 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_utilities.scss
+-rw-rw-rw-   0        0        0      215 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_virtual-reality.scss
+-rw-rw-rw-   0        0        0      981 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard.scss
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.608638 django-admin-corporate-1.0.2/admin_corporate/templates/
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.325116 django-admin-corporate-1.0.2/admin_corporate/templates/accounts/
+-rw-rw-rw-   0        0        0     1378 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/accounts/password-change-done.html
+-rw-rw-rw-   0        0        0     2155 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/accounts/password-change.html
+-rw-rw-rw-   0        0        0     1382 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/accounts/password-reset-complete.html
+-rw-rw-rw-   0        0        0     1937 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/accounts/password-reset-confirm.html
+-rw-rw-rw-   0        0        0     1181 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/accounts/password-reset-done.html
+-rw-rw-rw-   0        0        0     2147 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/accounts/password-reset.html
+-rw-rw-rw-   0        0        0     2944 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/accounts/sign-in.html
+-rw-rw-rw-   0        0        0     4130 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/accounts/sign-up.html
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.355841 django-admin-corporate-1.0.2/admin_corporate/templates/admin/
+-rw-rw-rw-   0        0        0     1745 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/actions.html
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:58.590764 django-admin-corporate-1.0.2/admin_corporate/templates/admin/auth/
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.358841 django-admin-corporate-1.0.2/admin_corporate/templates/admin/auth/user/
+-rw-rw-rw-   0        0        0      334 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/auth/user/add_form.html
+-rw-rw-rw-   0        0        0     5386 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/auth/user/change_password.html
+-rw-rw-rw-   0        0        0     5912 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/change_form.html
+-rw-rw-rw-   0        0        0      695 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/change_form_object_tools.html
+-rw-rw-rw-   0        0        0     5598 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/change_list.html
+-rw-rw-rw-   0        0        0      607 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/change_list_object_tools.html
+-rw-rw-rw-   0        0        0     3141 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/change_list_results.html
+-rw-rw-rw-   0        0        0     6925 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/delete_confirmation.html
+-rw-rw-rw-   0        0        0     7246 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/delete_selected_confirmation.html
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.364890 django-admin-corporate-1.0.2/admin_corporate/templates/admin/edit_inline/
+-rw-rw-rw-   0        0        0     3893 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/edit_inline/stacked.html
+-rw-rw-rw-   0        0        0     7834 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/edit_inline/tabular.html
+-rw-rw-rw-   0        0        0      643 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/filter.html
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.371884 django-admin-corporate-1.0.2/admin_corporate/templates/admin/includes/
+-rw-rw-rw-   0        0        0     2572 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/includes/fieldset.html
+-rw-rw-rw-   0        0        0      348 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/includes/object_delete_summary.html
+-rw-rw-rw-   0        0        0    42632 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/index.html
+-rw-rw-rw-   0        0        0     2727 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/invalid_setup.html
+-rw-rw-rw-   0        0        0     3332 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/login.html
+-rw-rw-rw-   0        0        0     3875 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/object_history.html
+-rw-rw-rw-   0        0        0     2321 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/pagination.html
+-rw-rw-rw-   0        0        0     2634 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/search_form.html
+-rw-rw-rw-   0        0        0     1618 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/admin/submit_line.html
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.429189 django-admin-corporate-1.0.2/admin_corporate/templates/includes/
+-rw-rw-rw-   0        0        0     3769 2023-04-05 10:03:50.000000 django-admin-corporate-1.0.2/admin_corporate/templates/includes/fixed_plugin.html
+-rw-rw-rw-   0        0        0        0 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/includes/footer-rtl.html
+-rw-rw-rw-   0        0        0      981 2023-04-05 09:07:38.000000 django-admin-corporate-1.0.2/admin_corporate/templates/includes/footer.html
+-rw-rw-rw-   0        0        0     1054 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/includes/head.html
+-rw-rw-rw-   0        0        0     5946 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/includes/navigation-auth.html
+-rw-rw-rw-   0        0        0    10812 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/includes/navigation-fullscreen.html
+-rw-rw-rw-   0        0        0     8511 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/includes/navigation-rtl.html
+-rw-rw-rw-   0        0        0     8532 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/includes/navigation.html
+-rw-rw-rw-   0        0        0      355 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/includes/scripts.html
+-rw-rw-rw-   0        0        0    10639 2023-04-05 10:03:31.000000 django-admin-corporate-1.0.2/admin_corporate/templates/includes/sidebar-rtl.html
+-rw-rw-rw-   0        0        0    15487 2023-04-05 10:03:28.000000 django-admin-corporate-1.0.2/admin_corporate/templates/includes/sidebar.html
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.437698 django-admin-corporate-1.0.2/admin_corporate/templates/layouts/
+-rw-rw-rw-   0        0        0     1240 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/layouts/base-auth.html
+-rw-rw-rw-   0        0        0     1868 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/layouts/base-fullscreen.html
+-rw-rw-rw-   0        0        0     2016 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/layouts/base-rtl.html
+-rw-rw-rw-   0        0        0     2217 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/layouts/base.html
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.448936 django-admin-corporate-1.0.2/admin_corporate/templates/pages/
+-rw-rw-rw-   0        0        0    42632 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/pages/dashboard.html
+-rw-rw-rw-   0        0        0    18562 2023-04-05 10:09:50.000000 django-admin-corporate-1.0.2/admin_corporate/templates/pages/profile.html
+-rw-rw-rw-   0        0        0    51971 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/pages/rtl.html
+-rw-rw-rw-   0        0        0    51177 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/pages/tables.html
+-rw-rw-rw-   0        0        0    39396 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/pages/wallet.html
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.454301 django-admin-corporate-1.0.2/admin_corporate/templates/registration/
+-rw-rw-rw-   0        0        0     1658 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/registration/logged_out.html
+-rw-rw-rw-   0        0        0     2688 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/registration/password_change_done.html
+-rw-rw-rw-   0        0        0     3964 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templates/registration/password_change_form.html
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.459304 django-admin-corporate-1.0.2/admin_corporate/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     2476 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templatetags/admin_corporate.py
+-rw-rw-rw-   0        0        0      178 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/templatetags/replace_value.py
+-rw-rw-rw-   0        0        0     1536 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/urls.py
+-rw-rw-rw-   0        0        0    16522 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/utils.py
+-rw-rw-rw-   0        0        0     2515 2023-04-05 08:14:23.000000 django-admin-corporate-1.0.2/admin_corporate/views.py
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.469145 django-admin-corporate-1.0.2/django_admin_corporate.egg-info/
+-rw-rw-rw-   0        0        0     7213 2023-05-08 18:09:57.000000 django-admin-corporate-1.0.2/django_admin_corporate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    22307 2023-05-08 18:09:58.000000 django-admin-corporate-1.0.2/django_admin_corporate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 18:09:57.000000 django-admin-corporate-1.0.2/django_admin_corporate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-05 08:17:35.000000 django-admin-corporate-1.0.2/django_admin_corporate.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-05-08 18:09:58.000000 django-admin-corporate-1.0.2/django_admin_corporate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 18:09:59.471149 django-admin-corporate-1.0.2/docs/
+-rw-rw-rw-   0        0        0       13 2023-04-04 07:23:08.000000 django-admin-corporate-1.0.2/docs/blank.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 18:09:59.474697 django-admin-corporate-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1359 2023-05-08 18:06:33.000000 django-admin-corporate-1.0.2/setup.py
```

### Comparing `django-admin-corporate-1.0.1/LICENSE.md` & `django-admin-corporate-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/PKG-INFO` & `django-admin-corporate-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-corporate
-Version: 1.0.1
+Version: 1.0.2
 Summary: Modern template for Django admin interface
 Home-page: https://appseed.us/product/corporate-ui-dashboard/django/
 Author: AppSeed.us
 Author-email: support@appseed.us
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `django-admin-corporate-1.0.1/README.md` & `django-admin-corporate-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/forms.py` & `django-admin-corporate-1.0.2/admin_corporate/forms.py`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/css/corporate-ui-dashboard.css` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/css/corporate-ui-dashboard.css`

 * *Files 0% similar despite different names*

```diff
@@ -27572,8 +27572,7 @@
 
 .swiper-button-next:after,
 .swiper-button-prev:after {
   font-size: 1rem;
   color: #0f172a;
 }
 
-/*# sourceMappingURL=dashboard-free.css.map */
```

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/css/corporate-ui-dashboard.css.map` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/css/corporate-ui-dashboard.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/css/corporate-ui-dashboard.min.css` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/css/corporate-ui-dashboard.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/css/forms.css` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/css/forms.css`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/css/nucleo-icons.css` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/css/nucleo-icons.css`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/css/nucleo-svg.css` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/css/nucleo-svg.css`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/css/widgets.css` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/css/widgets.css`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo-icons.eot` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo-icons.eot`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo-icons.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo-icons.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo-icons.ttf` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo-icons.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo-icons.woff` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo-icons.woff`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo-icons.woff2` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo-icons.woff2`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo.eot` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo.eot`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo.ttf` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo.woff` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo.woff`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/fonts/nucleo.woff2` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/fonts/nucleo.woff2`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/3d-cube.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/3d-cube.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/apple-icon.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/apple-icon.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/bg1.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/bg1.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/bruce-mars.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/bruce-mars.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/curved-images/img-6.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/curved-images/img-6.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/curved-images/img-7.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/curved-images/img-7.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/down-arrow-dark.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/down-arrow-dark.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/down-arrow-white.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/down-arrow-white.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/down-arrow.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/down-arrow.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/favicon.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/favicon.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/header-blue-purple.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/header-blue-purple.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/header-orange-purple.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/header-orange-purple.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/icon-calendar.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/icon-calendar.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/icon-clock.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/icon-clock.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/icons/add.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/icons/add.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/image-sign-in.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/image-sign-in.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/image-sign-up.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/image-sign-up.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/img-1.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/img-1.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/img-2.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/img-2.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/img-3.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/img-3.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/img-4.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/img-4.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/img-5.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/img-5.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/img-8.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/img-8.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/img-9.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/img-9.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logo-ct-dark.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logo-ct-dark.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logo-ct.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logo-ct.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logos/facebook-logo.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logos/facebook-logo.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logos/google-logo.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logos/google-logo.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logos/mastercard-white.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logos/mastercard-white.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logos/mastercard.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logos/mastercard.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logos/visa-white.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logos/visa-white.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logos/visa.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logos/visa.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/logos/wifi-white.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/logos/wifi-white.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/marie.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/marie.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/icon-sun-cloud.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/icon-sun-cloud.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/logo-atlassian.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/logo-atlassian.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/logo-google.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/logo-google.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/logo-invision.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/logo-invision.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/logo-jira.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/logo-jira.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/logo-slack.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/logo-slack.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/logo-spotify.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/logo-spotify.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/logo-webdev.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/logo-webdev.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/small-logos/logo-xd.svg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/small-logos/logo-xd.svg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/team-1.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/team-1.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/team-2.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/team-2.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/team-3.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/team-3.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/team-4.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/team-4.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/team-5.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/team-5.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/team-6.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/team-6.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/angular.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/angular.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/bootstrap.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/bootstrap.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/dribbble.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/dribbble.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/dropbox.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/dropbox.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/mastercard.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/mastercard.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/paypal.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/paypal.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/react.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/react.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/sketch.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/sketch.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/slack.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/slack.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/spotify.jpeg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/spotify.jpeg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/tim.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/tim.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/unass.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/unass.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/visa.png` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/visa.png`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/img/theme/vue.jpg` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/img/theme/vue.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/js/core/bootstrap.bundle.min.js` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/js/core/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/js/core/bootstrap.min.js` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/js/core/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/js/core/popper.min.js` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/js/core/popper.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/js/corporate-ui-dashboard.js` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/js/corporate-ui-dashboard.js`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/js/corporate-ui-dashboard.js.map` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/js/corporate-ui-dashboard.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/js/corporate-ui-dashboard.min.js` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/js/corporate-ui-dashboard.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -149,9 +149,8 @@
     let e = document.querySelectorAll('[onclick="sidebarType(this)"]');
     window.innerWidth < 1200 ? e.forEach(function(e) {
         e.classList.add("disabled")
     }) : e.forEach(function(e) {
         e.classList.remove("disabled")
     })
 }
-window.addEventListener("resize", sidenavTypeOnResize), window.addEventListener("load", sidenavTypeOnResize);
-//# sourceMappingURL=_site_dashboard_free/assets/js/dashboard-free.js.map
+window.addEventListener("resize", sidenavTypeOnResize), window.addEventListener("load", sidenavTypeOnResize);
```

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/js/plugins/Chart.extension.js` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/js/plugins/Chart.extension.js`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/js/plugins/bootstrap-notify.js` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/js/plugins/bootstrap-notify.js`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/js/plugins/chartjs.min.js` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/js/plugins/chartjs.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/js/plugins/perfect-scrollbar.min.js` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/js/plugins/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/js/plugins/smooth-scrollbar.min.js` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/js/plugins/smooth-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/js/plugins/swiper-bundle.min.js` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/js/plugins/swiper-bundle.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4872,9 +4872,8 @@
             overwriteParams: () => ({
                 watchSlidesProgress: !0,
                 virtualTranslate: !t.params.cssMode
             })
         })
     }];
     return V.use(re), V
-}));
-//# sourceMappingURL=swiper-bundle.min.js.map
+}));
```

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_avatars.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_avatars.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_badge.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_badge.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_breadcrumbs.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_breadcrumbs.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_buttons.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_buttons.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_cards.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_cards.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_dark-version.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_dark-version.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_dropdown.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_dropup.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_dropup.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_fixed-plugin.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_fixed-plugin.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_forms.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_forms.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_gradients.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_gradients.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_header.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_header.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_info-areas.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_info-areas.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_misc.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_misc.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_nav.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_nav.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_navbar-vertical.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_navbar-vertical.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_navbar.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_navbar.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_pagination.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_pagination.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_rtl.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_rtl.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_social-buttons.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_tables.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_tables.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_timeline.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_timeline.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_typography.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_typography.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_utilities.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_utilities.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/_variables.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_accordion.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_accordion.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_alert.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_alert.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_badge.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_badge.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_breadcrumb.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_button-group.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_button-group.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_buttons.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_buttons.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_card.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_card.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_carousel.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_carousel.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_close.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_close.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_containers.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_containers.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_dropdown.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_functions.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_functions.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_grid.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_grid.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_images.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_images.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_list-group.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_list-group.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_maps.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_maps.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_mixins.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_mixins.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_modal.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_modal.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_nav.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_nav.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_navbar.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_navbar.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_offcanvas.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_pagination.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_pagination.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_placeholders.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_popover.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_popover.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_progress.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_progress.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_reboot.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_reboot.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_root.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_root.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_spinners.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_spinners.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_tables.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_tables.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_toasts.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_toasts.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_tooltip.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_type.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_type.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_utilities.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_utilities.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_variables.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/bootstrap-grid.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/bootstrap.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_floating-labels.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-check.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-control.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-range.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-select.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_input-group.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_labels.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_position.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_border-radius.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_breakpoints.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_buttons.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_caret.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_deprecate.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_forms.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_gradients.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_grid.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_list-group.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_list-group.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_reset-text.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_reset-text.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_table-variants.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_transition.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_utilities.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_visually-hidden.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/utilities/_api.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/vendor/_rfs.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/bootstrap/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/cards/card-background.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/cards/card-background.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_form-check.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_form-switch.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_form-switch.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_input-group.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/mixins/_social-buttons.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/mixins/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_flatpickr.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_flatpickr.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_nouislider.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_nouislider.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_perfect-scrollbar.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_perfect-scrollbar.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_prism.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_prism.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_swiper.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/plugins/free/_swiper.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/theme.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/theme.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_animations.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_animations.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_avatars.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_avatars.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_badge.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_badge.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_cards-extend.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_cards-extend.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_cards.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_cards.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_choices.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_choices.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_dark-version.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_dark-version.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_dropdowns.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_dropdowns.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_header.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_header.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_info-areas.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_info-areas.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_misc-extend.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_misc-extend.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_misc.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_misc.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_navbar-vertical.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_navbar-vertical.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_navbar.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_navbar.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_pagination.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_pagination.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_social-buttons.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_table.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_table.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_timeline.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_timeline.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_utilities-extend.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_utilities-extend.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_utilities.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard/variables/_utilities.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/static/assets/scss/corporate-ui-dashboard.scss` & `django-admin-corporate-1.0.2/admin_corporate/static/assets/scss/corporate-ui-dashboard.scss`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/accounts/password-change-done.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/accounts/password-change-done.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/accounts/password-change.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/accounts/password-change.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/accounts/password-reset-complete.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/accounts/password-reset-complete.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/accounts/password-reset-confirm.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/accounts/password-reset-confirm.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/accounts/password-reset-done.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/accounts/password-reset-done.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/accounts/password-reset.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/accounts/password-reset.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/accounts/sign-in.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/accounts/sign-in.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/accounts/sign-up.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/accounts/sign-up.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/actions.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/auth/user/change_password.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/change_form.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/change_form_object_tools.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/change_list.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/change_list_object_tools.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/change_list_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/change_list_results.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/delete_confirmation.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/delete_selected_confirmation.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/edit_inline/stacked.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/edit_inline/tabular.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/filter.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/filter.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/includes/fieldset.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/index.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/invalid_setup.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/invalid_setup.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/login.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/object_history.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/pagination.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/search_form.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/admin/submit_line.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/includes/fixed_plugin.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/includes/fixed_plugin.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/includes/footer.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/includes/footer.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/includes/head.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/includes/head.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/includes/navigation-auth.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/includes/navigation-auth.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/includes/navigation-fullscreen.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/includes/navigation-fullscreen.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/includes/navigation-rtl.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/includes/navigation-rtl.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/includes/navigation.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/includes/navigation.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/includes/sidebar-rtl.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/includes/sidebar-rtl.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/includes/sidebar.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/includes/sidebar.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/layouts/base-auth.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/layouts/base-auth.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/layouts/base-fullscreen.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/layouts/base-fullscreen.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/layouts/base-rtl.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/layouts/base-rtl.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/layouts/base.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/layouts/base.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/pages/dashboard.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/pages/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/pages/profile.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/pages/profile.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/pages/rtl.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/pages/rtl.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/pages/tables.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/pages/tables.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/pages/wallet.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/pages/wallet.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/registration/logged_out.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/registration/password_change_done.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templates/registration/password_change_form.html` & `django-admin-corporate-1.0.2/admin_corporate/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/templatetags/admin_corporate.py` & `django-admin-corporate-1.0.2/admin_corporate/templatetags/admin_corporate.py`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/urls.py` & `django-admin-corporate-1.0.2/admin_corporate/urls.py`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/utils.py` & `django-admin-corporate-1.0.2/admin_corporate/utils.py`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/admin_corporate/views.py` & `django-admin-corporate-1.0.2/admin_corporate/views.py`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/django_admin_corporate.egg-info/PKG-INFO` & `django-admin-corporate-1.0.2/django_admin_corporate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-corporate
-Version: 1.0.1
+Version: 1.0.2
 Summary: Modern template for Django admin interface
 Home-page: https://appseed.us/product/corporate-ui-dashboard/django/
 Author: AppSeed.us
 Author-email: support@appseed.us
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `django-admin-corporate-1.0.1/django_admin_corporate.egg-info/SOURCES.txt` & `django-admin-corporate-1.0.2/django_admin_corporate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-corporate-1.0.1/setup.py` & `django-admin-corporate-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
 name='django-admin-corporate',
-version='1.0.1',
+version='1.0.2',
 zip_safe=False,
 packages=find_packages(),
 include_package_data=True,
 description='Modern template for Django admin interface',
 long_description=README,
 long_description_content_type="text/markdown",
 url='https://appseed.us/product/corporate-ui-dashboard/django/',
```

